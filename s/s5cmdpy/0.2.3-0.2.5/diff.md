# Comparing `tmp/s5cmdpy-0.2.3.tar.gz` & `tmp/s5cmdpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5cmdpy-0.2.3.tar", max compression
+gzip compressed data, was "s5cmdpy-0.2.5.tar", max compression
```

## Comparing `s5cmdpy-0.2.3.tar` & `s5cmdpy-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2598 2024-03-13 04:33:58.917349 s5cmdpy-0.2.3/README.md
--rw-r--r--   0        0        0      335 2024-03-13 04:33:58.917349 s5cmdpy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       37 2024-03-13 04:33:58.917349 s5cmdpy-0.2.3/s5cmdpy/__init__.py
--rw-r--r--   0        0        0    15036 2024-03-13 04:33:58.917349 s5cmdpy-0.2.3/s5cmdpy/s5cmd_runner.py
--rw-r--r--   0        0        0     4592 2024-03-13 04:33:58.917349 s5cmdpy-0.2.3/s5cmdpy/uni_logger_standalone.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 s5cmdpy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2598 2024-04-09 02:24:22.440728 s5cmdpy-0.2.5/README.md
+-rw-r--r--   0        0        0      335 2024-04-09 02:24:22.440728 s5cmdpy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-09 02:24:22.440728 s5cmdpy-0.2.5/s5cmdpy/__init__.py
+-rw-r--r--   0        0        0    16547 2024-04-09 02:24:22.440728 s5cmdpy-0.2.5/s5cmdpy/s5cmd_runner.py
+-rw-r--r--   0        0        0     4592 2024-04-09 02:24:22.440728 s5cmdpy-0.2.5/s5cmdpy/uni_logger_standalone.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 s5cmdpy-0.2.5/PKG-INFO
```

### Comparing `s5cmdpy-0.2.3/README.md` & `s5cmdpy-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `s5cmdpy-0.2.3/s5cmdpy/s5cmd_runner.py` & `s5cmdpy-0.2.5/s5cmdpy/s5cmd_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 import platform
 import requests
 import re
 from tqdm.auto import tqdm
 from urllib.parse import urlparse
 import time
 import shutil
+import hashlib
 
 from s5cmdpy.uni_logger_standalone import UniLogger
 
+from typing import List
+
 class S5CmdRunner:
     """
     A class that provides methods for interacting with s5cmd, a command-line tool for efficient S3 data transfer.
 
     Attributes:
         s5cmd_path (str): The path to the s5cmd executable.
 
@@ -32,16 +35,15 @@
         run(txt_uri): Runs s5cmd with a command file specified by a local path, URL, or S3 URI.
     """
 
     def __init__(self):
         # if on windows
         binary_name = 's5cmd' if os.name != 'nt' else 's5cmd.exe'
         self.s5cmd_path = os.path.expanduser(f'~/{binary_name}')
-
-        self.s5cmd_path = os.path.expanduser('~/s5cmd')
+        
         self.logger = UniLogger()
         if not self.has_s5cmd():
             self.get_s5cmd()
 
     def has_s5cmd(self) -> bool:
         return os.path.exists(self.s5cmd_path) and os.access(self.s5cmd_path, os.X_OK)
 
@@ -93,22 +95,48 @@
                 return process
             except Exception as e:
                 self.logger.error(f"Error starting subprocess: {e}")
                 return None
         else:
             subprocess.run([command, *args])
 
-    def generate_s5cmd_file(self, s3_uris, dest_dir):
-        command_file_path = '/tmp/s5cmd_commands.txt'
+    @staticmethod
+    def fast_list_hash(s3_uris: List[str]) -> str:
+        """Generate a hash for a list of S3 URIs.
+        """
+        if not s3_uris:
+            raise ValueError("The s3_uris list cannot be empty.")
+
+        # Generate a simplified identifier based on the URIs list characteristics
+        first_uri = s3_uris[0]
+        last_uri = s3_uris[-1]
+        middle_uri = s3_uris[len(s3_uris) // 2]
+        total_length = sum(len(uri) for uri in s3_uris)
+        num_uris = len(s3_uris)
+        identifier = hashlib.md5(f"{num_uris}-{len(first_uri)}-{len(last_uri)}-{len(middle_uri)}-{total_length}".encode()).hexdigest()
+        return identifier[:8]
+
+
+    def generate_s5cmd_file(self, s3_uris: List[str], dest_dir:str):        
+        if not s3_uris:
+            raise ValueError("The s3_uris list cannot be empty.")
+
+        # Generate a simplified identifier based on the URIs list characteristics
+        identifier = self.fast_list_hash(s3_uris)
+        date_str = time.strftime("%Y%m%d-%H%M%S")
+        command_file_path = f'/tmp/s5cmd_commands_{date_str}_{identifier}.txt'
+
         with open(command_file_path, 'w') as file:
             for s3_uri in s3_uris:
                 command = f"cp {s3_uri} {dest_dir}/{os.path.basename(s3_uri)}\n"
                 file.write(command)
+        
         return command_file_path
 
+
     def _update_progress_bar(self, process, total=None, report_interval=5):
         """
         Updates a progress bar based on subprocess output.
         
         Args:
             process (subprocess.Popen): The subprocess.Popen object.
             total (int, optional): The total number of items expected to process. If None, progress bar is indeterminate.
@@ -142,15 +170,27 @@
             process = self.call_function(
                 self.s5cmd_path, "run", command_file_path, capture_output=True)
             if process and process.stdout:
                 self._update_progress_bar(process, total=len(s3_uris))
             else:
                 self.logger.error("Failed to start s5cmd subprocess with output capture.")
         else:
+            self.logger.info(f"Generated command file: {command_file_path}")
+
+            self.logger.info(f"Downloading {len(s3_uris)} files from S3 to {dest_dir}")
             self.call_function(self.s5cmd_path, "run", command_file_path)
+            self.logger.info(f"Downloaded {len(s3_uris)} files from S3 to {dest_dir}")
+
+            print(f"removing command file: {command_file_path}")
+
+        # remove the command file after use
+        try:
+            os.remove(command_file_path)
+        except Exception as e:
+            self.logger.error(f"Failed to remove command file: {e}")
 
     def is_local_file(self, path):
         return os.path.isfile(path)
 
     def get_filename_from_url(self, url):
         """
         Extract the filename from a URL.
```

### Comparing `s5cmdpy-0.2.3/s5cmdpy/uni_logger_standalone.py` & `s5cmdpy-0.2.5/s5cmdpy/uni_logger_standalone.py`

 * *Files identical despite different names*

### Comparing `s5cmdpy-0.2.3/PKG-INFO` & `s5cmdpy-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s5cmdpy
-Version: 0.2.3
+Version: 0.2.5
 Summary: python binding for using s5cmd to download and upload files to s3 efficiently
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

