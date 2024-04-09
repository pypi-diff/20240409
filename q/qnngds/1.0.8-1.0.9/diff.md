# Comparing `tmp/qnngds-1.0.8.tar.gz` & `tmp/qnngds-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-1.0.8.tar", last modified: Tue Apr  9 15:48:38 2024, max compression
+gzip compressed data, was "qnngds-1.0.9.tar", last modified: Tue Apr  9 16:39:55 2024, max compression
```

## Comparing `qnngds-1.0.8.tar` & `qnngds-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-04-09 15:48:35.969437 qnngds-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-09 15:48:35.969437 qnngds-1.0.8/README.md
--rw-r--r--   0        0        0     1161 2024-04-09 15:48:38.669437 qnngds-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      111 2024-04-09 15:48:35.977437 qnngds-1.0.8/src/qnngds/__init__.py
--rw-r--r--   0        0        0    10600 2024-04-09 15:48:35.977437 qnngds-1.0.8/src/qnngds/circuits.py
--rw-r--r--   0        0        0    51283 2024-04-09 15:48:35.977437 qnngds-1.0.8/src/qnngds/design.py
--rw-r--r--   0        0        0     8019 2024-04-09 15:48:35.977437 qnngds-1.0.8/src/qnngds/devices.py
--rw-r--r--   0        0        0     8244 2024-04-09 15:48:35.977437 qnngds-1.0.8/src/qnngds/geometries.py
--rw-r--r--   0        0        0    21375 2024-04-09 15:48:35.977437 qnngds-1.0.8/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 qnngds-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-09 16:39:51.869940 qnngds-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-09 16:39:51.869940 qnngds-1.0.9/README.md
+-rw-r--r--   0        0        0     1161 2024-04-09 16:39:55.025935 qnngds-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-04-09 16:39:51.873940 qnngds-1.0.9/src/qnngds/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-09 16:39:51.877940 qnngds-1.0.9/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    51283 2024-04-09 16:39:51.877940 qnngds-1.0.9/src/qnngds/design.py
+-rw-r--r--   0        0        0     8019 2024-04-09 16:39:51.877940 qnngds-1.0.9/src/qnngds/devices.py
+-rw-r--r--   0        0        0     8244 2024-04-09 16:39:51.877940 qnngds-1.0.9/src/qnngds/geometries.py
+-rw-r--r--   0        0        0    21375 2024-04-09 16:39:51.877940 qnngds-1.0.9/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 qnngds-1.0.9/PKG-INFO
```

### Comparing `qnngds-1.0.8/LICENSE.txt` & `qnngds-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/README.md` & `qnngds-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/pyproject.toml` & `qnngds-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-1.0.8/src/qnngds/circuits.py` & `qnngds-1.0.9/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/src/qnngds/design.py` & `qnngds-1.0.9/src/qnngds/design.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/src/qnngds/devices.py` & `qnngds-1.0.9/src/qnngds/devices.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/src/qnngds/geometries.py` & `qnngds-1.0.9/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/src/qnngds/utilities.py` & `qnngds-1.0.9/src/qnngds/utilities.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.0.8/PKG-INFO` & `qnngds-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 1.0.8
+Version: 1.0.9
 Summary: The QNN library for creating gds files
 Keywords: phidl nanowire_electronics nanofabrication gds
 Author-Email: A. Jacquillat <audrey01@mit.edu>, A. Jacquillat <audrey.jacquillat@gmail.com>, R. Foster <reedf@mit.edu>
 Maintainer-Email: A. Jacquillat <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

