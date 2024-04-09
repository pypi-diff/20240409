# Comparing `tmp/pygranta-2024.1.0.tar.gz` & `tmp/pygranta-2024.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygranta-2024.1.0.tar", max compression
+gzip compressed data, was "pygranta-2024.2.0a0.tar", max compression
```

## Comparing `pygranta-2024.1.0.tar` & `pygranta-2024.2.0a0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-01-17 22:24:35.753782 pygranta-2024.1.0/LICENSE
--rw-r--r--   0        0        0     3786 2024-01-17 22:24:35.753782 pygranta-2024.1.0/README.rst
--rw-r--r--   0        0        0     1463 2024-01-17 22:24:35.753782 pygranta-2024.1.0/pyproject.toml
--rw-r--r--   0        0        0      289 2024-01-17 22:24:35.753782 pygranta-2024.1.0/src/pygranta/__init__.py
--rw-r--r--   0        0        0     5004 1970-01-01 00:00:00.000000 pygranta-2024.1.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-04-09 19:26:07.541670 pygranta-2024.2.0a0/AUTHORS
+-rw-r--r--   0        0        0     1089 2024-04-09 19:26:07.541670 pygranta-2024.2.0a0/LICENSE
+-rw-r--r--   0        0        0     3786 2024-04-09 19:26:07.541670 pygranta-2024.2.0a0/README.rst
+-rw-r--r--   0        0        0     1461 2024-04-09 19:26:07.541670 pygranta-2024.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0      289 2024-04-09 19:26:07.541670 pygranta-2024.2.0a0/src/pygranta/__init__.py
+-rw-r--r--   0        0        0     5002 1970-01-01 00:00:00.000000 pygranta-2024.2.0a0/PKG-INFO
```

### Comparing `pygranta-2024.1.0/LICENSE` & `pygranta-2024.2.0a0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 ANSYS, Inc. All rights reserved.
+Copyright (c) 2024 ANSYS, Inc. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pygranta-2024.1.0/README.rst` & `pygranta-2024.2.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `pygranta-2024.1.0/pyproject.toml` & `pygranta-2024.2.0a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pygranta"
 description = "Pythonic interfaces to Ansys Granta MI"
-version = "2024.1.0"
+version = "2024.2.0a0"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 repository = "https://github.com/ansys/pygranta"
 documentation = "https://grantami.docs.pyansys.com"
 readme = "README.rst"
 classifiers = [
-  "Development Status :: 5 - Production/Stable",
+  "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Information Analysis",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 packages = [{ include = "**/*.py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ansys-grantami-bomanalytics = "2.0.0"
-ansys-grantami-bomanalytics-openapi = "2.0.0"
-ansys-grantami-recordlists = "1.1.0"
-ansys-grantami-serverapi-openapi = "2.0.0"
+ansys-grantami-bomanalytics = "2.1.0a0"
+ansys-grantami-bomanalytics-openapi = "3.0.0a1"
+ansys-grantami-recordlists = "1.2.0a0"
+ansys-grantami-serverapi-openapi = "3.0.0a3"
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 Sphinx = "^7.0.1"
-ansys-sphinx-theme = "^0.13.1"
+ansys-sphinx-theme = "^0.15.2"
 sphinx-copybutton = "^0.5.0"
 sphinx-design = "^0.5.0"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
```

### Comparing `pygranta-2024.1.0/PKG-INFO` & `pygranta-2024.2.0a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pygranta
-Version: 2024.1.0
+Version: 2024.2.0a0
 Summary: Pythonic interfaces to Ansys Granta MI
 Home-page: https://github.com/ansys/pygranta
 License: MIT
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Dist: ansys-grantami-bomanalytics (==2.0.0)
-Requires-Dist: ansys-grantami-bomanalytics-openapi (==2.0.0)
-Requires-Dist: ansys-grantami-recordlists (==1.1.0)
-Requires-Dist: ansys-grantami-serverapi-openapi (==2.0.0)
+Requires-Dist: ansys-grantami-bomanalytics (==2.1.0a0)
+Requires-Dist: ansys-grantami-bomanalytics-openapi (==3.0.0a1)
+Requires-Dist: ansys-grantami-recordlists (==1.2.0a0)
+Requires-Dist: ansys-grantami-serverapi-openapi (==3.0.0a3)
 Project-URL: Documentation, https://grantami.docs.pyansys.com
 Project-URL: Repository, https://github.com/ansys/pygranta
 Description-Content-Type: text/x-rst
 
 PyGranta metapackage
 ====================
 |pyansys| |python| |pypi| |GH-CI| |MIT| |black| |pre-commit|
```

