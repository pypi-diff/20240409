# Comparing `tmp/shipyard_ftp-0.2.1a3.tar.gz` & `tmp/shipyard_ftp-0.2.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_ftp-0.2.1a3.tar", max compression
+gzip compressed data, was "shipyard_ftp-0.2.1a4.tar", max compression
```

## Comparing `shipyard_ftp-0.2.1a3.tar` & `shipyard_ftp-0.2.1a4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a3/README.md
--rw-r--r--   0        0        0      531 2024-04-09 14:29:02.386675 shipyard_ftp-0.2.1a3/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a3/shipyard_ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/__init__.py
--rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/authtest.py
--rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/delete.py
--rw-r--r--   0        0        0     5849 2024-04-09 14:29:02.380595 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/download.py
--rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/move.py
--rw-r--r--   0        0        0     2995 2024-04-09 14:11:43.413045 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/upload.py
--rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a3/shipyard_ftp/exceptions.py
--rw-r--r--   0        0        0    10130 2024-04-09 14:28:26.891723 shipyard_ftp-0.2.1a3/shipyard_ftp/ftp.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a4/README.md
+-rw-r--r--   0        0        0      531 2024-04-09 14:35:09.151006 shipyard_ftp-0.2.1a4/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a4/shipyard_ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a4/shipyard_ftp/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a4/shipyard_ftp/cli/authtest.py
+-rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a4/shipyard_ftp/cli/delete.py
+-rw-r--r--   0        0        0     5849 2024-04-09 14:29:02.380595 shipyard_ftp-0.2.1a4/shipyard_ftp/cli/download.py
+-rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a4/shipyard_ftp/cli/move.py
+-rw-r--r--   0        0        0     2995 2024-04-09 14:11:43.413045 shipyard_ftp-0.2.1a4/shipyard_ftp/cli/upload.py
+-rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a4/shipyard_ftp/exceptions.py
+-rw-r--r--   0        0        0     9882 2024-04-09 14:35:09.153859 shipyard_ftp-0.2.1a4/shipyard_ftp/ftp.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a4/PKG-INFO
```

### Comparing `shipyard_ftp-0.2.1a3/pyproject.toml` & `shipyard_ftp-0.2.1a4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-ftp"
-version = "0.2.1a3"
+version = "0.2.1a4"
 description = "A local client for connecting and working with FTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_ftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/authtest.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/delete.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/cli/delete.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/download.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/cli/download.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/move.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/upload.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/exceptions.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a3/shipyard_ftp/ftp.py` & `shipyard_ftp-0.2.1a4/shipyard_ftp/ftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,23 +153,19 @@
         Raises:
             InvalidCredentials: If the credentials are invalid
             DownloadError: If the file cannot be downloaded
         """
         if not self.client:
             self.get_client()
 
-        if destination_folder := os.path.dirname(destination_full_path):
-            os.makedirs(destination_folder, exist_ok=True)
         try:
             logger.info(f"Attempting to download {file_name}...")
             with open(destination_full_path, "wb") as f:
                 self.client.retrbinary(f"RETR {file_name}", f.write)
-            logger.info(
-                f"{file_name} successfully downloaded to {destination_full_path}"
-            )
+
         except exceptions.InvalidCredentials:
             raise
 
         except Exception as e:
             os.remove(destination_full_path)
             raise exceptions.DownloadError(
                 f"Failed to download {file_name}. Message from server: {e}"
@@ -260,15 +256,15 @@
                 return True
         except exceptions.InvalidCredentials:
             raise
         except Exception:
             return False
 
     def get_all_nested_items(
-        self, working_directory: str, dir_list: list = None
+            self, working_directory: str, dir_list: list = None
     ) -> list:
         """
         Recursive function to get all the nested files and directories on the FTP server.
 
         Args:
             working_directory (str): The full path of the working directory
             dir_list (list): A list of directories
```

### Comparing `shipyard_ftp-0.2.1a3/PKG-INFO` & `shipyard_ftp-0.2.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-ftp
-Version: 0.2.1a3
+Version: 0.2.1a4
 Summary: A local client for connecting and working with FTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

