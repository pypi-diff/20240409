# Comparing `tmp/os2borgerpc_client-2.4.1.tar.gz` & `tmp/os2borgerpc_client-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2borgerpc_client-2.4.1.tar", last modified: Wed Dec 20 08:21:54 2023, max compression
+gzip compressed data, was "os2borgerpc_client-2.5.0.tar", last modified: Tue Apr  9 08:43:57 2024, max compression
```

## Comparing `os2borgerpc_client-2.4.1.tar` & `os2borgerpc_client-2.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.714370 os2borgerpc_client-2.4.1/
--rw-rw-r--   0 ap        (1000) ap        (1000)    35149 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/LICENSE
--rw-rw-r--   0 ap        (1000) ap        (1000)     1219 2023-12-20 08:21:54.714370 os2borgerpc_client-2.4.1/PKG-INFO
--rw-rw-r--   0 ap        (1000) ap        (1000)      764 2023-11-07 13:19:02.000000 os2borgerpc_client-2.4.1/README.rst
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.710369 os2borgerpc_client-2.4.1/bin/
--rwxrwxr-x   0 ap        (1000) ap        (1000)      561 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/bin/admin_connect.sh
--rwxrwxr-x   0 ap        (1000) ap        (1000)      731 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/bin/get_os2borgerpc_config
--rwxrwxr-x   0 ap        (1000) ap        (1000)     1766 2023-05-15 13:16:05.000000 os2borgerpc_client-2.4.1/bin/jobmanager
--rwxrwxr-x   0 ap        (1000) ap        (1000)      949 2023-02-21 15:50:01.000000 os2borgerpc_client-2.4.1/bin/os2borgerpc_push_config_keys
--rwxrwxr-x   0 ap        (1000) ap        (1000)      800 2023-11-07 13:19:02.000000 os2borgerpc_client-2.4.1/bin/os2borgerpc_register_in_admin
--rwxrwxr-x   0 ap        (1000) ap        (1000)     2373 2023-11-16 14:25:36.000000 os2borgerpc_client-2.4.1/bin/randomize_jobmanager.sh
--rwxrwxr-x   0 ap        (1000) ap        (1000)     4582 2023-12-20 08:17:13.000000 os2borgerpc_client-2.4.1/bin/register_new_os2borgerpc_client.sh
--rwxrwxr-x   0 ap        (1000) ap        (1000)      606 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/bin/set_os2borgerpc_config
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.706369 os2borgerpc_client-2.4.1/os2borgerpc/
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.710369 os2borgerpc_client-2.4.1/os2borgerpc/client/
--rw-rw-r--   0 ap        (1000) ap        (1000)       38 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/__init__.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     2963 2023-11-29 07:38:54.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/admin_client.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     5518 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/config.py
--rw-rw-r--   0 ap        (1000) ap        (1000)    19518 2023-11-07 13:19:02.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/jobmanager.py
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.710369 os2borgerpc_client-2.4.1/os2borgerpc/client/security/
--rw-rw-r--   0 ap        (1000) ap        (1000)       53 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/security/__init__.py
--rw-rw-r--   0 ap        (1000) ap        (1000)      391 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/security/csv_writer.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     1029 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/security/log_read.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     5254 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/security/security.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     1382 2023-05-08 08:26:25.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/updater.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     2768 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/os2borgerpc/client/utils.py
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.714370 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/
--rw-r--r--   0 ap        (1000) ap        (1000)     1219 2023-12-20 08:21:54.000000 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/PKG-INFO
--rw-rw-r--   0 ap        (1000) ap        (1000)      926 2023-12-20 08:21:54.000000 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ap        (1000) ap        (1000)        1 2023-12-20 08:21:54.000000 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ap        (1000) ap        (1000)        1 2023-02-21 15:51:30.000000 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/not-zip-safe
--rw-rw-r--   0 ap        (1000) ap        (1000)       38 2023-12-20 08:21:54.000000 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/requires.txt
--rw-rw-r--   0 ap        (1000) ap        (1000)       12 2023-12-20 08:21:54.000000 os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/top_level.txt
--rw-rw-r--   0 ap        (1000) ap        (1000)       38 2023-12-20 08:21:54.714370 os2borgerpc_client-2.4.1/setup.cfg
--rw-rw-r--   0 ap        (1000) ap        (1000)     1181 2023-12-20 08:17:13.000000 os2borgerpc_client-2.4.1/setup.py
-drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2023-12-20 08:21:54.714370 os2borgerpc_client-2.4.1/tests/
--rw-rw-r--   0 ap        (1000) ap        (1000)     8738 2022-10-06 12:18:04.000000 os2borgerpc_client-2.4.1/tests/test_jobmanager.py
--rw-rw-r--   0 ap        (1000) ap        (1000)    11647 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/tests/test_security.py
--rw-rw-r--   0 ap        (1000) ap        (1000)     3346 2022-09-08 12:54:09.000000 os2borgerpc_client-2.4.1/tests/test_security_utils.py
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.719553 os2borgerpc_client-2.5.0/
+-rw-rw-r--   0 ap        (1000) ap        (1000)    35149 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/LICENSE
+-rw-rw-r--   0 ap        (1000) ap        (1000)     1219 2024-04-09 08:43:57.719553 os2borgerpc_client-2.5.0/PKG-INFO
+-rw-rw-r--   0 ap        (1000) ap        (1000)      764 2023-11-07 13:19:02.000000 os2borgerpc_client-2.5.0/README.rst
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.715553 os2borgerpc_client-2.5.0/bin/
+-rwxrwxr-x   0 ap        (1000) ap        (1000)      561 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/bin/admin_connect.sh
+-rwxrwxr-x   0 ap        (1000) ap        (1000)      731 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/bin/get_os2borgerpc_config
+-rwxrwxr-x   0 ap        (1000) ap        (1000)     1766 2023-05-15 13:16:05.000000 os2borgerpc_client-2.5.0/bin/jobmanager
+-rwxrwxr-x   0 ap        (1000) ap        (1000)      949 2023-02-21 15:50:01.000000 os2borgerpc_client-2.5.0/bin/os2borgerpc_push_config_keys
+-rwxrwxr-x   0 ap        (1000) ap        (1000)      800 2023-11-07 13:19:02.000000 os2borgerpc_client-2.5.0/bin/os2borgerpc_register_in_admin
+-rwxrwxr-x   0 ap        (1000) ap        (1000)     2373 2023-11-16 14:25:36.000000 os2borgerpc_client-2.5.0/bin/randomize_jobmanager.sh
+-rwxrwxr-x   0 ap        (1000) ap        (1000)     4759 2024-04-09 07:06:35.000000 os2borgerpc_client-2.5.0/bin/register_new_os2borgerpc_client.sh
+-rwxrwxr-x   0 ap        (1000) ap        (1000)      606 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/bin/set_os2borgerpc_config
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.715553 os2borgerpc_client-2.5.0/os2borgerpc/
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.715553 os2borgerpc_client-2.5.0/os2borgerpc/client/
+-rw-rw-r--   0 ap        (1000) ap        (1000)       38 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/__init__.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     4046 2024-04-09 07:06:35.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/admin_client.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     5518 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/config.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)    20507 2024-04-09 08:20:17.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/jobmanager.py
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.715553 os2borgerpc_client-2.5.0/os2borgerpc/client/security/
+-rw-rw-r--   0 ap        (1000) ap        (1000)       53 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/security/__init__.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)      391 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/security/csv_writer.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     1029 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/security/log_read.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     5255 2024-04-09 07:06:35.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/security/security.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     1382 2023-05-08 08:26:25.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/updater.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     2768 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/os2borgerpc/client/utils.py
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.719553 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/
+-rw-r--r--   0 ap        (1000) ap        (1000)     1219 2024-04-09 08:43:57.000000 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ap        (1000) ap        (1000)      926 2024-04-09 08:43:57.000000 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ap        (1000) ap        (1000)        1 2024-04-09 08:43:57.000000 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ap        (1000) ap        (1000)        1 2023-02-21 15:51:30.000000 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/not-zip-safe
+-rw-rw-r--   0 ap        (1000) ap        (1000)       38 2024-04-09 08:43:57.000000 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/requires.txt
+-rw-rw-r--   0 ap        (1000) ap        (1000)       12 2024-04-09 08:43:57.000000 os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/top_level.txt
+-rw-rw-r--   0 ap        (1000) ap        (1000)       38 2024-04-09 08:43:57.719553 os2borgerpc_client-2.5.0/setup.cfg
+-rw-rw-r--   0 ap        (1000) ap        (1000)     1181 2024-04-09 08:43:01.000000 os2borgerpc_client-2.5.0/setup.py
+drwxrwxr-x   0 ap        (1000) ap        (1000)        0 2024-04-09 08:43:57.719553 os2borgerpc_client-2.5.0/tests/
+-rw-rw-r--   0 ap        (1000) ap        (1000)     8738 2022-10-06 12:18:04.000000 os2borgerpc_client-2.5.0/tests/test_jobmanager.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)    11647 2024-02-29 08:20:47.000000 os2borgerpc_client-2.5.0/tests/test_security.py
+-rw-rw-r--   0 ap        (1000) ap        (1000)     3346 2022-09-08 12:54:09.000000 os2borgerpc_client-2.5.0/tests/test_security_utils.py
```

### Comparing `os2borgerpc_client-2.4.1/LICENSE` & `os2borgerpc_client-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/PKG-INFO` & `os2borgerpc_client-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2borgerpc_client
-Version: 2.4.1
+Version: 2.5.0
 Summary: Client for the OS2borgerPC system
 Home-page: https://github.com/OS2borgerPC/
 Author: Magenta ApS
 Author-email: info@magenta-aps.dk
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `os2borgerpc_client-2.4.1/README.rst` & `os2borgerpc_client-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/admin_connect.sh` & `os2borgerpc_client-2.5.0/bin/admin_connect.sh`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/get_os2borgerpc_config` & `os2borgerpc_client-2.5.0/bin/get_os2borgerpc_config`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/jobmanager` & `os2borgerpc_client-2.5.0/bin/jobmanager`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/os2borgerpc_push_config_keys` & `os2borgerpc_client-2.5.0/bin/os2borgerpc_push_config_keys`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/os2borgerpc_register_in_admin` & `os2borgerpc_client-2.5.0/bin/os2borgerpc_register_in_admin`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/randomize_jobmanager.sh` & `os2borgerpc_client-2.5.0/bin/randomize_jobmanager.sh`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/bin/register_new_os2borgerpc_client.sh` & `os2borgerpc_client-2.5.0/bin/register_new_os2borgerpc_client.sh`

 * *Files 8% similar despite different names*

```diff
@@ -108,29 +108,34 @@
         fi
     fi
     set_os2borgerpc_config admin_url "$ADMIN_URL"
 
     # - set additional config values
     PC_MODEL=$(dmidecode --type system | grep Product | cut --delimiter : --fields 2)
     [ -z "$PC_MODEL" ] && PC_MODEL="Identification failed"
+    PC_MODEL=${PC_MODEL:0:100}
     set_os2borgerpc_config pc_model "$PC_MODEL"
 
     PC_MANUFACTURER=$(dmidecode --type system | grep Manufacturer | cut --delimiter : --fields 2)
     [ -z "$PC_MANUFACTURER" ] && PC_MANUFACTURER="Identification failed"
+    PC_MANUFACTURER=${PC_MANUFACTURER:0:100}
     set_os2borgerpc_config pc_manufacturer "$PC_MANUFACTURER"
 
     # xargs is there to remove the leading space
-    CPUS_BASE_INFO="$(dmidecode -t processor | grep Version | cut --delimiter ':' --fields 2 | xargs)"
+    CPUS_BASE_INFO="$(dmidecode --type processor | grep Version | cut --delimiter ':' --fields 2 | xargs)"
+    CPUS_BASE_INFO=${CPUS_BASE_INFO:0:100}
     CPU_CORES="$(grep ^"core id" /proc/cpuinfo | sort -u | wc -l)"
+    CPU_CORES=${CPU_CORES:0:100}
     CPUS="$CPUS_BASE_INFO - $CPU_CORES physical cores"
     [ -z "$CPUS" ] && CPUS="Identification failed"
     set_os2borgerpc_config pc_cpus "$CPUS"
 
     RAM="$(LANG=c lsmem | grep "Total online" | cut --delimiter ':' --fields 2 | xargs)"
     [ -z "$RAM" ] && RAM="Identification failed"
+    RAM=${RAM:0:100}
     set_os2borgerpc_config pc_ram "$RAM"
 
     # OK, we got the config.
     # Do the deed.
     if ! os2borgerpc_register_in_admin "$NEW_COMPUTER_NAME"; then
         fatal "Registration failed" && continue || exit 1
     fi
```

### Comparing `os2borgerpc_client-2.4.1/bin/set_os2borgerpc_config` & `os2borgerpc_client-2.5.0/bin/set_os2borgerpc_config`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc/client/config.py` & `os2borgerpc_client-2.5.0/os2borgerpc/client/config.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc/client/jobmanager.py` & `os2borgerpc_client-2.5.0/os2borgerpc/client/jobmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Module for jobmanager."""
+
 import json
 import os.path
 import re
 import socket
 import stat
 import subprocess
 import sys
 import traceback
 import unicodedata
 import urllib.parse
 import urllib.request
 from datetime import datetime
+from os import stat as os_stat
 
 import chardet
 import distro
 import pkg_resources
 
 from os2borgerpc.client.admin_client import OS2borgerPCAdmin
 from os2borgerpc.client.config import has_config
@@ -183,17 +185,17 @@
         if full_info is not False:
             self.read_property_from_file("executable_code", self.executable_path)
             self.load_local_parameters()
 
     def handle_unsupported_file_encoding(self, prop, file_path):
         """Error handling in case a file has an unsupported file encoding."""
         if file_path == self.log_path:  # If the current property is a log file
-            self[
-                prop
-            ] = "The log had an unsupported file encoding (neither utf-8 nor latin-1)"
+            self[prop] = (
+                "The log had an unsupported file encoding (neither utf-8 nor latin-1)"
+            )
         else:
             self[prop] = ""
 
     def read_property_from_file(self, prop, file_path):
         """Read property from file."""
         try:
             with open(file_path, "rb") as file_detect:
@@ -296,26 +298,23 @@
         self.read_property_from_file("status", self.status_path)
         if self["status"] != "SUBMITTED":
             sys.stderr.write(
                 "Job %s: Will only run jobs with status %s\n"
                 % (self.id, self["status"])
             )
             return
-        log = open(self.log_path, "a")
+        log = open(self.log_path, "w+")
         self.load_local_parameters()
         self.set_status("RUNNING")
         cmd = [self.executable_path]
         log_params = []
 
         for param in self["local_parameters"]:
             cmd.append(param["value"])
-            if param["type"] == "PASSWORD":
-                log_params.append("•••••")
-            else:
-                log_params.append(param["value"])
+            log_params.append(param["value"])
 
         self.mark_started()
         log.write(
             ">>> Starting process '%s' with arguments [%s] at %s\n"
             % (
                 self.executable_path,
                 ", ".join(log_params),
@@ -333,14 +332,25 @@
             log.write(">>> Succeeded at %s\n" % self["finished"])
         else:
             self.set_status("FAILED")
             log.write(
                 ">>> Failed with exit status %s at %s\n" % (ret_val, self["finished"])
             )
         os.remove(self.parameters_path)
+
+        log.seek(0)
+        log_content = log.read()
+
+        for param in self["local_parameters"]:
+            if param["type"] == "PASSWORD" and len(param["value"]) > 1:
+                log_content = log_content.replace(param["value"], "*****")
+
+        log.seek(0)
+        log.write(log_content)
+        log.truncate()
         log.close()
 
 
 def get_job_timeout():
     """Return the set job timeout, may be the default."""
     config = OS2borgerPCConfig()
 
@@ -429,15 +439,15 @@
 
     # Sanitize log output so we're sure it's valid XML before XMLRPC request
     for job in joblist:
         # Remove terminal control characters except newlines
         job["log_output"] = "".join(
             ch
             for ch in job["log_output"]
-            if unicodedata.category(ch)[0] != "C" or ch == "\n"
+            if unicodedata.category(ch)[0] != "C" or ch == "\n" or ch == "\t"
         )
 
     try:
         # This returns 0 on various interpretations of success
         return remote.send_status_info(
             uid, None, joblist, update_required=check_outstanding_packages()
         )
@@ -547,14 +557,29 @@
     os_release = distro.version()
     try:
         ip_addresses = subprocess.run(
             ["hostname", "--all-ip-addresses"], capture_output=True, text=True
         ).stdout.strip()
     except subprocess.CalledProcessError:
         ip_addresses = ""
+    try:
+        kernel_version = subprocess.run(
+            ["uname", "-r"], capture_output=True, text=True
+        ).stdout.strip()
+    except subprocess.CalledProcessError:
+        kernel_version = ""
+    if os.path.isfile("/var/lib/apt/periodic/unattended-upgrades-stamp"):
+        last_automatic_update_time = os_stat(
+            "/var/lib/apt/periodic/unattended-upgrades-stamp"
+        ).st_mtime
+        last_automatic_update_time = datetime.fromtimestamp(last_automatic_update_time).strftime(
+            "%Y-%m-%d %H:%M"
+        )
+    else:
+        last_automatic_update_time = ""
     if has_config("job_timeout"):
         try:
             job_timeout = int(config.get_value("job_timeout"))
         except ValueError:
             job_timeout = DEFAULT_JOB_TIMEOUT
     else:
         job_timeout = DEFAULT_JOB_TIMEOUT
@@ -564,14 +589,16 @@
             try:
                 send_config_values(
                     {
                         "_os2borgerpc.client_version": OS2BORGERPC_CLIENT_VERSION,
                         "_os_release": os_release,
                         "_os_name": os_name,
                         "_ip_addresses": ip_addresses,
+                        "_kernel_version": kernel_version,
+                        "_last_automatic_update_time": last_automatic_update_time,
                     }
                 )
                 instructions = get_instructions()
                 if "jobs" in instructions:
                     import_jobs(instructions["jobs"])
                 if "configuration" in instructions:
                     update_configuration_from_server(instructions["configuration"])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc/client/security/log_read.py` & `os2borgerpc_client-2.5.0/os2borgerpc/client/security/log_read.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc/client/security/security.py` & `os2borgerpc_client-2.5.0/os2borgerpc/client/security/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Security module."""
+
 from datetime import datetime
 from pathlib import Path
 import os
 import os.path
 import stat
 import subprocess
 import sys
```

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc/client/updater.py` & `os2borgerpc_client-2.5.0/os2borgerpc/client/updater.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc/client/utils.py` & `os2borgerpc_client-2.5.0/os2borgerpc/client/utils.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/PKG-INFO` & `os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2borgerpc-client
-Version: 2.4.1
+Version: 2.5.0
 Summary: Client for the OS2borgerPC system
 Home-page: https://github.com/OS2borgerPC/
 Author: Magenta ApS
 Author-email: info@magenta-aps.dk
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `os2borgerpc_client-2.4.1/os2borgerpc_client.egg-info/SOURCES.txt` & `os2borgerpc_client-2.5.0/os2borgerpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/setup.py` & `os2borgerpc_client-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     # Keep this name in sync with the one in os2borgerpc_client/jobmanager.py
     name="os2borgerpc_client",
-    version="2.4.1",
+    version="2.5.0",
     description="Client for the OS2borgerPC system",
     long_description=long_description,
     url="https://github.com/OS2borgerPC/",
     author="Magenta ApS",
     author_email="info@magenta-aps.dk",
     license="GPLv3",
     packages=["os2borgerpc.client", "os2borgerpc.client.security"],
```

### Comparing `os2borgerpc_client-2.4.1/tests/test_jobmanager.py` & `os2borgerpc_client-2.5.0/tests/test_jobmanager.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/tests/test_security.py` & `os2borgerpc_client-2.5.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.4.1/tests/test_security_utils.py` & `os2borgerpc_client-2.5.0/tests/test_security_utils.py`

 * *Files identical despite different names*

