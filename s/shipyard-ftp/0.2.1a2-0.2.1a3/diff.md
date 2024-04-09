# Comparing `tmp/shipyard_ftp-0.2.1a2.tar.gz` & `tmp/shipyard_ftp-0.2.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_ftp-0.2.1a2.tar", max compression
+gzip compressed data, was "shipyard_ftp-0.2.1a3.tar", max compression
```

## Comparing `shipyard_ftp-0.2.1a2.tar` & `shipyard_ftp-0.2.1a3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a2/README.md
--rw-r--r--   0        0        0      531 2024-04-09 14:15:11.341416 shipyard_ftp-0.2.1a2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a2/shipyard_ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/__init__.py
--rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/authtest.py
--rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/delete.py
--rw-r--r--   0        0        0     5139 2024-04-09 14:15:07.948010 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/download.py
--rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/move.py
--rw-r--r--   0        0        0     2995 2024-04-09 14:11:43.413045 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/upload.py
--rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a2/shipyard_ftp/exceptions.py
--rw-r--r--   0        0        0    10073 2024-03-26 14:34:21.376542 shipyard_ftp-0.2.1a2/shipyard_ftp/ftp.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a3/README.md
+-rw-r--r--   0        0        0      531 2024-04-09 14:29:02.386675 shipyard_ftp-0.2.1a3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a3/shipyard_ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/authtest.py
+-rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/delete.py
+-rw-r--r--   0        0        0     5849 2024-04-09 14:29:02.380595 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/download.py
+-rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/move.py
+-rw-r--r--   0        0        0     2995 2024-04-09 14:11:43.413045 shipyard_ftp-0.2.1a3/shipyard_ftp/cli/upload.py
+-rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a3/shipyard_ftp/exceptions.py
+-rw-r--r--   0        0        0    10130 2024-04-09 14:28:26.891723 shipyard_ftp-0.2.1a3/shipyard_ftp/ftp.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a3/PKG-INFO
```

### Comparing `shipyard_ftp-0.2.1a2/pyproject.toml` & `shipyard_ftp-0.2.1a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-ftp"
-version = "0.2.1a2"
+version = "0.2.1a3"
 description = "A local client for connecting and working with FTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_ftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/authtest.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/delete.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/delete.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/download.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import sys
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import ExitCodeException, CloudStorage
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
-from shipyard_ftp.exceptions import EXIT_CODE_DOWNLOAD_ERROR
+from shipyard_ftp.exceptions import EXIT_CODE_NO_MATCHES_FOUND, EXIT_CODE_DOWNLOAD_ERROR
 from shipyard_ftp.ftp import FtpClient
 
 logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
@@ -60,81 +60,89 @@
     try:
         args = get_args()
         host = args.host
         port = args.port
         username = args.username
         password = args.password
         source_file_name = args.source_file_name
-
-        source_folder_name = shipyard.clean_folder_name(args.source_folder_name.strip("/"))
+        source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
         source_full_path = shipyard.combine_folder_and_file_name(
             folder_name=source_folder_name, file_name=source_file_name
         )
+        source_file_name_match_type = args.source_file_name_match_type
         destination_folder_name = shipyard.clean_folder_name(
-            args.destination_folder_name
+            args.destination_folder_name.strip("/")
         )
         errors = []
         if destination_folder_name:
             shipyard.create_folder_if_dne(destination_folder_name)
         client = FtpClient(host=host, port=port, user=username, pwd=password)
 
         logger.info("Beginning the download process...")
+        if source_file_name_match_type == "exact_match":
+            try:
+                destination_name = shipyard.determine_destination_full_path(
+                    destination_folder_name=destination_folder_name,
+                    destination_file_name=args.destination_file_name,
+                    source_full_path=source_full_path,
+                )
+                client.download(source_full_path, destination_name)
 
-        folders = [source_folder_name]
-        files = []
-        while folders:
-            folder_filter = folders[0]
-            files, folders = client.find_files_in_directory(
-                folder_filter=folder_filter, files=files, folders=folders
-            )
-
-        matching_files = shipyard.file_match(
-            search_term=source_file_name,
-            files=files,
-            source_directory=source_folder_name,
-            destination_directory=destination_folder_name,
-            destination_filename=args.destination_file_name,
-            match_type=args.source_file_name_match_type,
-        )
+            except Exception as e:
+                logger.error(
+                    f"Failed to download {source_full_path} due to {e}\n"
+                    f"Most likely, the file name/folder name you specified has typos or the full folder name was "
+                    f"not provided. Check these and try again."
+                )
+                raise e
+        elif source_file_name_match_type == "regex_match":
+            folders = [source_folder_name]
+            files = []
+            while folders:
+                folder_filter = folders[0]
+                files, folders = client.find_files_in_directory(
+                    folder_filter=folder_filter, files=files, folders=folders
+                )
 
-        logger.info(f"{len(matching_files)} file(s) found. Preparing to download...")
-        for file in matching_files:
-            source_file = file["source_path"]
-            destination_full_path = file["destination_filename"]
+            matching_file_names = shipyard.find_all_file_matches(
+                files, re.compile(source_file_name)
+            )
 
-            try:
-                logger.info(
-                    f"Attempting to download file: {source_file} to {destination_full_path}..."
+            if number_of_matches := len(matching_file_names) == 0:
+                logger.info(f'No matches were found for regex "{source_file_name}".')
+                sys.exit(EXIT_CODE_NO_MATCHES_FOUND)
+
+            logger.info(f"{number_of_matches} files found. Preparing to download...")
+            for index, file_name in enumerate(matching_file_names, start=1):
+                destination_name = shipyard.determine_destination_full_path(
+                    destination_folder_name=destination_folder_name,
+                    destination_file_name=args.destination_file_name,
+                    source_full_path=file_name,
+                    file_number=index if number_of_matches > 1 else None,
                 )
-                client.download(source_file, destination_full_path)
+
                 logger.info(
-                    f"Successfully downloaded {source_file} to {destination_full_path}."
+                    f"Attempting to download file {index} of {number_of_matches}: {file_name} to {destination_name}..."
                 )
-            except Exception as e:
-                if args.source_file_name_match_type == "exact_match":
-                    logger.error(
-                        f"Failed to download {source_full_path} due to {e}\n"
-                        f"Most likely, the file name/folder name you specified has typos or the full folder name "
-                        f"was not provided. Check these and try again."
+                try:
+                    client.download(file_name, destination_name)
+                    logger.info(
+                        f"Successfully downloaded {file_name} to {destination_name}."
                     )
-                    raise e
-                else:
-                    logger.error(f"Failed to download {source_file} due to {e}")
-                    errors.append(file)
+                except Exception as e:
+                    logger.error(f"Failed to download {file_name} due to {e}")
+                    errors.append(file_name)
 
         logger.info("Download process complete.")
 
         if errors:
             logger.error(
                 "Failed to download the following files:\n" + "\n".join(errors)
             )
             sys.exit(EXIT_CODE_DOWNLOAD_ERROR)
-    except FileNotFoundError as e:
-        logger.error(f"File not found: {e}")
-        sys.exit(CloudStorage.EXIT_CODE_FILE_MATCH_ERROR)
     except ExitCodeException as e:
         logger.error(e.message)
         sys.exit(e.exit_code)
     except Exception as e:
         logger.error(f"An error occurred during the download process: {e}")
         sys.exit(CloudStorage.EXIT_CODE_UNKNOWN_ERROR)
```

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/move.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/upload.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/exceptions.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a2/shipyard_ftp/ftp.py` & `shipyard_ftp-0.2.1a3/shipyard_ftp/ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,16 @@
         Raises:
             InvalidCredentials: If the credentials are invalid
             DownloadError: If the file cannot be downloaded
         """
         if not self.client:
             self.get_client()
 
-        os.makedirs(os.path.dirname(destination_full_path), exist_ok=True)
+        if destination_folder := os.path.dirname(destination_full_path):
+            os.makedirs(destination_folder, exist_ok=True)
         try:
             logger.info(f"Attempting to download {file_name}...")
             with open(destination_full_path, "wb") as f:
                 self.client.retrbinary(f"RETR {file_name}", f.write)
             logger.info(
                 f"{file_name} successfully downloaded to {destination_full_path}"
             )
```

### Comparing `shipyard_ftp-0.2.1a2/PKG-INFO` & `shipyard_ftp-0.2.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-ftp
-Version: 0.2.1a2
+Version: 0.2.1a3
 Summary: A local client for connecting and working with FTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

