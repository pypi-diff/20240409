# Comparing `tmp/shipyard_ftp-0.2.0a7.tar.gz` & `tmp/shipyard_ftp-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_ftp-0.2.0a7.tar", max compression
+gzip compressed data, was "shipyard_ftp-0.2.1a0.tar", max compression
```

## Comparing `shipyard_ftp-0.2.0a7.tar` & `shipyard_ftp-0.2.1a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.0a7/README.md
--rw-r--r--   0        0        0      531 2024-03-26 13:29:31.061351 shipyard_ftp-0.2.0a7/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.0a7/shipyard_ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/__init__.py
--rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/authtest.py
--rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/delete.py
--rw-r--r--   0        0        0     5838 2024-03-14 04:10:23.524953 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/download.py
--rw-r--r--   0        0        0     4616 2024-03-26 13:26:23.262083 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/move.py
--rw-r--r--   0        0        0     3037 2024-03-26 13:24:43.869714 shipyard_ftp-0.2.0a7/shipyard_ftp/cli/upload.py
--rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.0a7/shipyard_ftp/exceptions.py
--rw-r--r--   0        0        0    10073 2024-03-14 04:10:23.527921 shipyard_ftp-0.2.0a7/shipyard_ftp/ftp.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.0a7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a0/README.md
+-rw-r--r--   0        0        0      531 2024-04-09 13:28:09.651142 shipyard_ftp-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a0/shipyard_ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a0/shipyard_ftp/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a0/shipyard_ftp/cli/authtest.py
+-rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a0/shipyard_ftp/cli/delete.py
+-rw-r--r--   0        0        0     5850 2024-04-09 13:25:08.758906 shipyard_ftp-0.2.1a0/shipyard_ftp/cli/download.py
+-rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a0/shipyard_ftp/cli/move.py
+-rw-r--r--   0        0        0     2995 2024-04-09 13:26:35.170835 shipyard_ftp-0.2.1a0/shipyard_ftp/cli/upload.py
+-rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a0/shipyard_ftp/exceptions.py
+-rw-r--r--   0        0        0    10073 2024-03-26 14:34:21.376542 shipyard_ftp-0.2.1a0/shipyard_ftp/ftp.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a0/PKG-INFO
```

### Comparing `shipyard_ftp-0.2.0a7/pyproject.toml` & `shipyard_ftp-0.2.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-ftp"
-version = "0.2.0a7"
+version = "0.2.1a0"
 description = "A local client for connecting and working with FTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_ftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/authtest.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/delete.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/cli/delete.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/download.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/cli/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     try:
         args = get_args()
         host = args.host
         port = args.port
         username = args.username
         password = args.password
         source_file_name = args.source_file_name
-        source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
+
+        source_folder_name = shipyard.clean_folder_name(args.source_folder_name.strip("/"))
         source_full_path = shipyard.combine_folder_and_file_name(
             folder_name=source_folder_name, file_name=source_file_name
         )
         source_file_name_match_type = args.source_file_name_match_type
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name
         )
```

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/move.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/cli/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         host = args.host
         port = args.port
         username = args.username
         password = args.password
         source_file_name = args.source_file_name
         source_folder_name = args.source_folder_name
 
-        destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
+        destination_folder_name = shipyard.clean_folder_name(
+            args.destination_folder_name
+        )
         source_file_name_match_type = args.source_file_name_match_type
         ftp_client = FtpClient(host=host, port=port, user=username, pwd=password)
         # if the source folder name is omitted, then use the current working directory
         source_folder_name = source_folder_name or ftp_client.client.pwd()
         if source_file_name_match_type == "exact_match":
             source_full_path = shipyard.combine_folder_and_file_name(
                 source_folder_name, source_file_name
@@ -97,15 +99,16 @@
                 )
                 if len(destination_full_path.split("/")) > 1:
                     path, file_name = destination_full_path.rsplit("/", 1)
                     ftp_client.create_new_folders(path)
 
                 logger.info(f"Moving file {index} of {number_of_matches}")
                 ftp_client.move(
-                    source_full_path=key_name, destination_full_path=destination_full_path
+                    source_full_path=key_name,
+                    destination_full_path=destination_full_path,
                 )
     except ExitCodeException as e:
         logger.error(e.message)
         sys.exit(e.exit_code)
     except Exception as e:
         logger.error(e)
         sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
```

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/cli/upload.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/cli/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,27 +43,33 @@
 def main():
     try:
         args = get_args()
 
         source_file_name = args.source_file_name
         source_folder_name = args.source_folder_name
         destination_filename = args.destination_file_name or source_file_name
-        destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
+        destination_folder_name = shipyard.clean_folder_name(
+            args.destination_folder_name.strip("/")
+        )
 
-        ftp_client = FtpClient(host=args.host, port=args.port, user=args.username, pwd=args.password)
-        files = shipyard.file_match(search_term=source_file_name,
-                                    files=shipyard.fetch_file_paths_from_directory(source_folder_name),
-                                    source_directory=source_folder_name,
-                                    destination_directory=destination_folder_name,
-                                    destination_filename=destination_filename,
-                                    match_type=args.source_file_name_match_type)
+        ftp_client = FtpClient(
+            host=args.host, port=args.port, user=args.username, pwd=args.password
+        )
+        files = shipyard.file_match(
+            search_term=source_file_name,
+            files=shipyard.fetch_file_paths_from_directory(source_folder_name),
+            source_directory=source_folder_name,
+            destination_directory=destination_folder_name,
+            destination_filename=destination_filename,
+            match_type=args.source_file_name_match_type,
+        )
 
         for file in files:
-            source_file = file['source_path']
-            destination_full_path = file['destination_filename']
+            source_file = file["source_path"]
+            destination_full_path = file["destination_filename"]
             if len(destination_full_path.split("/")) > 1:
                 path, file_name = destination_full_path.rsplit("/", 1)
                 ftp_client.create_new_folders(path)
             ftp_client.upload(source_file, destination_full_path)
 
     except ExitCodeException as e:
         logger.error(e.message)
```

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/exceptions.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.0a7/shipyard_ftp/ftp.py` & `shipyard_ftp-0.2.1a0/shipyard_ftp/ftp.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.0a7/PKG-INFO` & `shipyard_ftp-0.2.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-ftp
-Version: 0.2.0a7
+Version: 0.2.1a0
 Summary: A local client for connecting and working with FTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

