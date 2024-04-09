# Comparing `tmp/image-sorting-tool-1.1.1.tar.gz` & `tmp/image-sorting-tool-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-sorting-tool-1.1.1.tar", last modified: Mon Feb 26 16:41:22 2024, max compression
+gzip compressed data, was "image-sorting-tool-1.1.2.tar", last modified: Tue Apr  9 02:06:46 2024, max compression
```

## Comparing `image-sorting-tool-1.1.1.tar` & `image-sorting-tool-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:41:22.878408 image-sorting-tool-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-02-26 16:41:22.878408 image-sorting-tool-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:41:22.878408 image-sorting-tool-1.1.1/image_sorting_tool/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/image_sorting_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/image_sorting_tool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/image_sorting_tool/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/image_sorting_tool/image_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:41:22.878408 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-02-26 16:41:22.000000 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-26 16:41:22.000000 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:41:22.000000 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-26 16:41:22.000000 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-26 16:41:22.000000 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-26 16:41:22.000000 image-sorting-tool-1.1.1/image_sorting_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 16:41:22.878408 image-sorting-tool-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-26 16:41:13.000000 image-sorting-tool-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:06:46.034187 image-sorting-tool-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-09 02:06:46.034187 image-sorting-tool-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:06:46.030187 image-sorting-tool-1.1.2/image_sorting_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/image_sorting_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/image_sorting_tool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16185 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/image_sorting_tool/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/image_sorting_tool/image_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:06:46.034187 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-09 02:06:46.000000 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-09 02:06:46.000000 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 02:06:46.000000 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 02:06:46.000000 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 02:06:46.000000 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 02:06:46.000000 image-sorting-tool-1.1.2/image_sorting_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 02:06:46.034187 image-sorting-tool-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-09 02:06:41.000000 image-sorting-tool-1.1.2/setup.py
```

### Comparing `image-sorting-tool-1.1.1/LICENSE` & `image-sorting-tool-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image-sorting-tool-1.1.1/PKG-INFO` & `image-sorting-tool-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-sorting-tool
-Version: 1.1.1
+Version: 1.1.2
 Summary: Graphical tool to sort images into a folder structure based on the date the images were taken
 Home-page: https://github.com/ThorpeJosh/image-sorting-tool
 Author: Joshua Thorpe
 Author-email: josh@thorpe.engineering
 License: MIT
 Keywords: image,sort,gui,executable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,21 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow~=10.2.0
+Requires-Dist: Pillow~=10.3.0
 Requires-Dist: python-dateutil~=2.8
 Provides-Extra: dev
-Requires-Dist: pytest==8.0.*; extra == "dev"
+Requires-Dist: pytest==8.1.*; extra == "dev"
 Requires-Dist: pylint==3.1.*; extra == "dev"
-Requires-Dist: black==24.2.*; extra == "dev"
-Requires-Dist: setuptools==69.1.*; extra == "dev"
+Requires-Dist: black==24.3.*; extra == "dev"
+Requires-Dist: setuptools==69.2.*; extra == "dev"
 
 # Image Sorting Tool
 [![Python Checks](https://github.com/ThorpeJosh/image-sorting-tool/actions/workflows/python-test.yml/badge.svg)](https://github.com/ThorpeJosh/image-sorting-tool/actions/workflows/python-test.yml)
 [![PyPI version](https://img.shields.io/pypi/v/image-sorting-tool.svg)](https://pypi.org/project/image-sorting-tool/)
 [![PyPI version](https://img.shields.io/pypi/pyversions/image-sorting-tool.svg)](https://pypi.org/project/image-sorting-tool/)
 [![PyPI license](https://img.shields.io/pypi/l/image-sorting-tool.svg)](https://pypi.org/project/image-sorting-tool/)  
 ![Screenshot](https://raw.githubusercontent.com/ThorpeJosh/image-sorting-tool/main/assets/ImageSortingTool.png)
```

### Comparing `image-sorting-tool-1.1.1/README.md` & `image-sorting-tool-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `image-sorting-tool-1.1.1/image_sorting_tool/__main__.py` & `image-sorting-tool-1.1.2/image_sorting_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `image-sorting-tool-1.1.1/image_sorting_tool/gui.py` & `image-sorting-tool-1.1.2/image_sorting_tool/gui.py`

 * *Files identical despite different names*

### Comparing `image-sorting-tool-1.1.1/image_sorting_tool/image_sort.py` & `image-sorting-tool-1.1.2/image_sorting_tool/image_sort.py`

 * *Files identical despite different names*

### Comparing `image-sorting-tool-1.1.1/image_sorting_tool.egg-info/PKG-INFO` & `image-sorting-tool-1.1.2/image_sorting_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-sorting-tool
-Version: 1.1.1
+Version: 1.1.2
 Summary: Graphical tool to sort images into a folder structure based on the date the images were taken
 Home-page: https://github.com/ThorpeJosh/image-sorting-tool
 Author: Joshua Thorpe
 Author-email: josh@thorpe.engineering
 License: MIT
 Keywords: image,sort,gui,executable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,21 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow~=10.2.0
+Requires-Dist: Pillow~=10.3.0
 Requires-Dist: python-dateutil~=2.8
 Provides-Extra: dev
-Requires-Dist: pytest==8.0.*; extra == "dev"
+Requires-Dist: pytest==8.1.*; extra == "dev"
 Requires-Dist: pylint==3.1.*; extra == "dev"
-Requires-Dist: black==24.2.*; extra == "dev"
-Requires-Dist: setuptools==69.1.*; extra == "dev"
+Requires-Dist: black==24.3.*; extra == "dev"
+Requires-Dist: setuptools==69.2.*; extra == "dev"
 
 # Image Sorting Tool
 [![Python Checks](https://github.com/ThorpeJosh/image-sorting-tool/actions/workflows/python-test.yml/badge.svg)](https://github.com/ThorpeJosh/image-sorting-tool/actions/workflows/python-test.yml)
 [![PyPI version](https://img.shields.io/pypi/v/image-sorting-tool.svg)](https://pypi.org/project/image-sorting-tool/)
 [![PyPI version](https://img.shields.io/pypi/pyversions/image-sorting-tool.svg)](https://pypi.org/project/image-sorting-tool/)
 [![PyPI license](https://img.shields.io/pypi/l/image-sorting-tool.svg)](https://pypi.org/project/image-sorting-tool/)  
 ![Screenshot](https://raw.githubusercontent.com/ThorpeJosh/image-sorting-tool/main/assets/ImageSortingTool.png)
```

### Comparing `image-sorting-tool-1.1.1/setup.py` & `image-sorting-tool-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Setup module to allow packaging, distributing and pip installing"""
 
 from setuptools import setup
 from image_sorting_tool import __version__ as version
 
-REQUIREMENTS = ["Pillow~=10.2.0", "python-dateutil~=2.8"]
+REQUIREMENTS = ["Pillow~=10.3.0", "python-dateutil~=2.8"]
 DEV_REQUIREMENTS = {
     "dev": [
-        "pytest==8.0.*",
+        "pytest==8.1.*",
         "pylint==3.1.*",
-        "black==24.2.*",
-        "setuptools==69.1.*",
+        "black==24.3.*",
+        "setuptools==69.2.*",
     ]
 }
 
 with open("README.md", encoding="utf-8") as readme_file:
     LONG_DESCRIPTION = "".join(readme_file.readlines())
 
 setup(
```

