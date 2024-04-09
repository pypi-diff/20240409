# Comparing `tmp/shipyard_ftp-0.2.2a0.tar.gz` & `tmp/shipyard_ftp-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_ftp-0.2.2a0.tar", max compression
+gzip compressed data, was "shipyard_ftp-0.2.2a1.tar", max compression
```

## Comparing `shipyard_ftp-0.2.2a0.tar` & `shipyard_ftp-0.2.2a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.2a0/README.md
--rw-r--r--   0        0        0      531 2024-04-09 16:31:06.068748 shipyard_ftp-0.2.2a0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.2a0/shipyard_ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.2a0/shipyard_ftp/cli/__init__.py
--rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.2a0/shipyard_ftp/cli/authtest.py
--rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.2a0/shipyard_ftp/cli/delete.py
--rw-r--r--   0        0        0     5464 2024-04-09 14:58:06.527184 shipyard_ftp-0.2.2a0/shipyard_ftp/cli/download.py
--rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.2a0/shipyard_ftp/cli/move.py
--rw-r--r--   0        0        0     2961 2024-04-09 16:30:58.886882 shipyard_ftp-0.2.2a0/shipyard_ftp/cli/upload.py
--rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.2a0/shipyard_ftp/exceptions.py
--rw-r--r--   0        0        0     9882 2024-04-09 14:35:09.153859 shipyard_ftp-0.2.2a0/shipyard_ftp/ftp.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.2a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.2a1/README.md
+-rw-r--r--   0        0        0      531 2024-04-09 16:45:31.213773 shipyard_ftp-0.2.2a1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.2a1/shipyard_ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.2a1/shipyard_ftp/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.2a1/shipyard_ftp/cli/authtest.py
+-rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.2a1/shipyard_ftp/cli/delete.py
+-rw-r--r--   0        0        0     5464 2024-04-09 14:58:06.527184 shipyard_ftp-0.2.2a1/shipyard_ftp/cli/download.py
+-rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.2a1/shipyard_ftp/cli/move.py
+-rw-r--r--   0        0        0     3011 2024-04-09 16:40:32.076025 shipyard_ftp-0.2.2a1/shipyard_ftp/cli/upload.py
+-rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.2a1/shipyard_ftp/exceptions.py
+-rw-r--r--   0        0        0     9882 2024-04-09 14:35:09.153859 shipyard_ftp-0.2.2a1/shipyard_ftp/ftp.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.2a1/PKG-INFO
```

### Comparing `shipyard_ftp-0.2.2a0/pyproject.toml` & `shipyard_ftp-0.2.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-ftp"
-version = "0.2.2a0"
+version = "0.2.2a1"
 description = "A local client for connecting and working with FTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_ftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/cli/authtest.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/cli/delete.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/cli/delete.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/cli/download.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/cli/download.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/cli/move.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/cli/upload.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,19 @@
 
 
 def main():
     try:
         args = get_args()
 
         source_file_name = args.source_file_name
-        source_folder_name = args.source_folder_name
+        source_folder_name = os.path.normpath(args.source_folder_name)
         destination_filename = args.destination_file_name or source_file_name
-        destination_folder_name = os.path.normpath(args.destination_folder_name)
+        destination_folder_name = shipyard.clean_folder_name(
+            args.destination_folder_name
+        )
 
         ftp_client = FtpClient(
             host=args.host, port=args.port, user=args.username, pwd=args.password
         )
         files = shipyard.file_match(
             search_term=source_file_name,
             files=shipyard.fetch_file_paths_from_directory(source_folder_name),
```

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/exceptions.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.2a0/shipyard_ftp/ftp.py` & `shipyard_ftp-0.2.2a1/shipyard_ftp/ftp.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.2a0/PKG-INFO` & `shipyard_ftp-0.2.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-ftp
-Version: 0.2.2a0
+Version: 0.2.2a1
 Summary: A local client for connecting and working with FTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

