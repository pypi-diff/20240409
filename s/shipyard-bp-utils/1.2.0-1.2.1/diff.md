# Comparing `tmp/shipyard_bp_utils-1.2.0.tar.gz` & `tmp/shipyard_bp_utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_bp_utils-1.2.0.tar", max compression
+gzip compressed data, was "shipyard_bp_utils-1.2.1.tar", max compression
```

## Comparing `shipyard_bp_utils-1.2.0.tar` & `shipyard_bp_utils-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4165 2024-02-05 15:18:12.483291 shipyard_bp_utils-1.2.0/README.md
--rw-r--r--   0        0        0      496 2024-03-21 17:44:04.770034 shipyard_bp_utils-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       58 2024-02-07 15:09:08.397039 shipyard_bp_utils-1.2.0/shipyard_bp_utils/__init__.py
--rw-r--r--   0        0        0     2973 2024-02-23 20:44:50.409581 shipyard_bp_utils-1.2.0/shipyard_bp_utils/args.py
--rw-r--r--   0        0        0     3475 2024-03-14 04:10:25.272748 shipyard_bp_utils-1.2.0/shipyard_bp_utils/artifacts.py
--rw-r--r--   0        0        0    16093 2024-03-21 18:26:17.152912 shipyard_bp_utils-1.2.0/shipyard_bp_utils/files.py
--rw-r--r--   0        0        0      794 2024-02-05 15:18:12.485764 shipyard_bp_utils-1.2.0/shipyard_bp_utils/text.py
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 shipyard_bp_utils-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4165 2024-02-05 15:18:12.483291 shipyard_bp_utils-1.2.1/README.md
+-rw-r--r--   0        0        0      496 2024-04-09 14:56:39.521458 shipyard_bp_utils-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-02-07 15:09:08.397039 shipyard_bp_utils-1.2.1/shipyard_bp_utils/__init__.py
+-rw-r--r--   0        0        0     2973 2024-02-23 20:44:50.409581 shipyard_bp_utils-1.2.1/shipyard_bp_utils/args.py
+-rw-r--r--   0        0        0     3475 2024-03-14 04:10:25.272748 shipyard_bp_utils-1.2.1/shipyard_bp_utils/artifacts.py
+-rw-r--r--   0        0        0    16176 2024-04-09 14:54:59.804470 shipyard_bp_utils-1.2.1/shipyard_bp_utils/files.py
+-rw-r--r--   0        0        0      794 2024-02-05 15:18:12.485764 shipyard_bp_utils-1.2.1/shipyard_bp_utils/text.py
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 shipyard_bp_utils-1.2.1/PKG-INFO
```

### Comparing `shipyard_bp_utils-1.2.0/README.md` & `shipyard_bp_utils-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_bp_utils-1.2.0/shipyard_bp_utils/args.py` & `shipyard_bp_utils-1.2.1/shipyard_bp_utils/args.py`

 * *Files identical despite different names*

### Comparing `shipyard_bp_utils-1.2.0/shipyard_bp_utils/artifacts.py` & `shipyard_bp_utils-1.2.1/shipyard_bp_utils/artifacts.py`

 * *Files identical despite different names*

### Comparing `shipyard_bp_utils-1.2.0/shipyard_bp_utils/files.py` & `shipyard_bp_utils-1.2.1/shipyard_bp_utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
     Args:
     folder_name (str): The folder name to be cleaned.
 
     Returns:
     str: The cleaned folder name.
     """
-    folder_name = os.path.normpath(folder_name)
+    folder_name = folder_name.strip("/")
+    if folder_name != "":
+        folder_name = os.path.normpath(folder_name.strip("/"))
+
     logger.debug(f"Cleaned folder name: {folder_name}")
     return folder_name
 
 
 def create_folder_if_dne(destination_folder_name: str) -> None:
     """
     Creates a folder and all required subfolders if it does not already exist.
```

### Comparing `shipyard_bp_utils-1.2.0/shipyard_bp_utils/text.py` & `shipyard_bp_utils-1.2.1/shipyard_bp_utils/text.py`

 * *Files identical despite different names*

### Comparing `shipyard_bp_utils-1.2.0/PKG-INFO` & `shipyard_bp_utils-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-bp-utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: Utility functions for blueprints
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

