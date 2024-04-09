# Comparing `tmp/shipyard_ftp-0.2.1a1.tar.gz` & `tmp/shipyard_ftp-0.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_ftp-0.2.1a1.tar", max compression
+gzip compressed data, was "shipyard_ftp-0.2.1a2.tar", max compression
```

## Comparing `shipyard_ftp-0.2.1a1.tar` & `shipyard_ftp-0.2.1a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a1/README.md
--rw-r--r--   0        0        0      531 2024-04-09 14:11:47.926767 shipyard_ftp-0.2.1a1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a1/shipyard_ftp/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a1/shipyard_ftp/cli/__init__.py
--rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a1/shipyard_ftp/cli/authtest.py
--rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a1/shipyard_ftp/cli/delete.py
--rw-r--r--   0        0        0     5134 2024-04-09 14:11:43.412370 shipyard_ftp-0.2.1a1/shipyard_ftp/cli/download.py
--rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a1/shipyard_ftp/cli/move.py
--rw-r--r--   0        0        0     2995 2024-04-09 14:11:43.413045 shipyard_ftp-0.2.1a1/shipyard_ftp/cli/upload.py
--rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a1/shipyard_ftp/exceptions.py
--rw-r--r--   0        0        0    10073 2024-03-26 14:34:21.376542 shipyard_ftp-0.2.1a1/shipyard_ftp/ftp.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858792 shipyard_ftp-0.2.1a2/README.md
+-rw-r--r--   0        0        0      531 2024-04-09 14:15:11.341416 shipyard_ftp-0.2.1a2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-12 18:48:21.830827 shipyard_ftp-0.2.1a2/shipyard_ftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.435846 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-03-14 04:10:23.523728 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/authtest.py
+-rw-r--r--   0        0        0     3526 2024-03-14 04:10:23.524393 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/delete.py
+-rw-r--r--   0        0        0     5139 2024-04-09 14:15:07.948010 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/download.py
+-rw-r--r--   0        0        0     4659 2024-03-27 16:08:43.683003 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/move.py
+-rw-r--r--   0        0        0     2995 2024-04-09 14:11:43.413045 shipyard_ftp-0.2.1a2/shipyard_ftp/cli/upload.py
+-rw-r--r--   0        0        0     1270 2024-03-14 04:10:23.526823 shipyard_ftp-0.2.1a2/shipyard_ftp/exceptions.py
+-rw-r--r--   0        0        0    10073 2024-03-26 14:34:21.376542 shipyard_ftp-0.2.1a2/shipyard_ftp/ftp.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 shipyard_ftp-0.2.1a2/PKG-INFO
```

### Comparing `shipyard_ftp-0.2.1a1/pyproject.toml` & `shipyard_ftp-0.2.1a2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-ftp"
-version = "0.2.1a1"
+version = "0.2.1a2"
 description = "A local client for connecting and working with FTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_ftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/cli/authtest.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/cli/delete.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/delete.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/cli/download.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                     f"Attempting to download file: {source_file} to {destination_full_path}..."
                 )
                 client.download(source_file, destination_full_path)
                 logger.info(
                     f"Successfully downloaded {source_file} to {destination_full_path}."
                 )
             except Exception as e:
-                if args.source_file_match_type == "exact_match":
+                if args.source_file_name_match_type == "exact_match":
                     logger.error(
                         f"Failed to download {source_full_path} due to {e}\n"
                         f"Most likely, the file name/folder name you specified has typos or the full folder name "
                         f"was not provided. Check these and try again."
                     )
                     raise e
                 else:
```

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/cli/move.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/cli/upload.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/exceptions.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a1/shipyard_ftp/ftp.py` & `shipyard_ftp-0.2.1a2/shipyard_ftp/ftp.py`

 * *Files identical despite different names*

### Comparing `shipyard_ftp-0.2.1a1/PKG-INFO` & `shipyard_ftp-0.2.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-ftp
-Version: 0.2.1a1
+Version: 0.2.1a2
 Summary: A local client for connecting and working with FTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

