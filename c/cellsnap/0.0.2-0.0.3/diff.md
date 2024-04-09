# Comparing `tmp/CellSNAP-0.0.2.tar.gz` & `tmp/cellsnap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellSNAP-0.0.2.tar", last modified: Mon Apr  8 04:50:41 2024, max compression
+gzip compressed data, was "cellsnap-0.0.3.tar", last modified: Tue Apr  9 03:53:33 2024, max compression
```

## Comparing `CellSNAP-0.0.2.tar` & `cellsnap-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-08 04:50:41.554561 CellSNAP-0.0.2/
--rwxrwxrwx   0 sheng     (1001) sheng     (1001)     1066 2023-06-05 07:35:42.000000 CellSNAP-0.0.2/LICENSE
--rw-rw-r--   0 sheng     (1001) sheng     (1001)     1145 2024-04-08 04:50:41.554561 CellSNAP-0.0.2/PKG-INFO
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)      866 2024-04-07 03:42:26.000000 CellSNAP-0.0.2/README.md
--rw-rw-r--   0 sheng     (1001) sheng     (1001)      103 2024-04-08 01:46:40.000000 CellSNAP-0.0.2/pyproject.toml
--rw-rw-r--   0 sheng     (1001) sheng     (1001)      979 2024-04-08 04:50:41.554561 CellSNAP-0.0.2/setup.cfg
--rw-rw-r--   0 sheng     (1001) sheng     (1001)     1865 2024-04-08 04:49:48.000000 CellSNAP-0.0.2/setup.py
-drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-08 04:50:41.554561 CellSNAP-0.0.2/src/
-drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-08 04:50:41.554561 CellSNAP-0.0.2/src/CellSNAP/
--rw-rw-r--   0 sheng     (1001) sheng     (1001)        0 2024-04-08 00:49:10.000000 CellSNAP-0.0.2/src/CellSNAP/__init__.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)    17005 2024-04-07 03:42:26.000000 CellSNAP-0.0.2/src/CellSNAP/cellsnap.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)     8483 2024-04-07 03:42:26.000000 CellSNAP-0.0.2/src/CellSNAP/datasets.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)     9949 2024-04-06 23:36:55.000000 CellSNAP-0.0.2/src/CellSNAP/graph.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)     2721 2024-04-07 23:21:07.000000 CellSNAP-0.0.2/src/CellSNAP/main.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)     4659 2024-04-07 01:38:43.000000 CellSNAP-0.0.2/src/CellSNAP/models.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)     7322 2024-04-06 23:36:55.000000 CellSNAP-0.0.2/src/CellSNAP/preprocessing.py
--rwxrwxr-x   0 sheng     (1001) sheng     (1001)     9084 2024-04-07 03:07:57.000000 CellSNAP-0.0.2/src/CellSNAP/utils.py
-drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-08 04:50:41.554561 CellSNAP-0.0.2/src/CellSNAP.egg-info/
--rw-rw-r--   0 sheng     (1001) sheng     (1001)     1145 2024-04-08 04:50:41.000000 CellSNAP-0.0.2/src/CellSNAP.egg-info/PKG-INFO
--rw-rw-r--   0 sheng     (1001) sheng     (1001)      423 2024-04-08 04:50:41.000000 CellSNAP-0.0.2/src/CellSNAP.egg-info/SOURCES.txt
--rw-rw-r--   0 sheng     (1001) sheng     (1001)        1 2024-04-08 04:50:41.000000 CellSNAP-0.0.2/src/CellSNAP.egg-info/dependency_links.txt
--rw-rw-r--   0 sheng     (1001) sheng     (1001)      239 2024-04-08 04:50:41.000000 CellSNAP-0.0.2/src/CellSNAP.egg-info/requires.txt
--rw-rw-r--   0 sheng     (1001) sheng     (1001)        9 2024-04-08 04:50:41.000000 CellSNAP-0.0.2/src/CellSNAP.egg-info/top_level.txt
+drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-09 03:53:33.762865 cellsnap-0.0.3/
+-rwxrwxrwx   0 sheng     (1001) sheng     (1001)     1066 2023-06-05 07:35:42.000000 cellsnap-0.0.3/LICENSE
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)     1145 2024-04-09 03:53:33.762865 cellsnap-0.0.3/PKG-INFO
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)      866 2024-04-07 03:42:26.000000 cellsnap-0.0.3/README.md
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)      103 2024-04-08 01:46:40.000000 cellsnap-0.0.3/pyproject.toml
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)      979 2024-04-09 03:53:33.762865 cellsnap-0.0.3/setup.cfg
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)     1865 2024-04-09 03:53:20.000000 cellsnap-0.0.3/setup.py
+drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-09 03:53:33.758865 cellsnap-0.0.3/src/
+drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-09 03:53:33.758865 cellsnap-0.0.3/src/CellSNAP/
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)        0 2024-04-08 00:49:10.000000 cellsnap-0.0.3/src/CellSNAP/__init__.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)    17005 2024-04-07 03:42:26.000000 cellsnap-0.0.3/src/CellSNAP/cellsnap.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)     8483 2024-04-07 03:42:26.000000 cellsnap-0.0.3/src/CellSNAP/datasets.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)     9949 2024-04-06 23:36:55.000000 cellsnap-0.0.3/src/CellSNAP/graph.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)     2721 2024-04-07 23:21:07.000000 cellsnap-0.0.3/src/CellSNAP/main.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)     4659 2024-04-07 01:38:43.000000 cellsnap-0.0.3/src/CellSNAP/models.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)     7322 2024-04-06 23:36:55.000000 cellsnap-0.0.3/src/CellSNAP/preprocessing.py
+-rwxrwxr-x   0 sheng     (1001) sheng     (1001)     9084 2024-04-07 03:07:57.000000 cellsnap-0.0.3/src/CellSNAP/utils.py
+drwxrwxr-x   0 sheng     (1001) sheng     (1001)        0 2024-04-09 03:53:33.762865 cellsnap-0.0.3/src/cellsnap.egg-info/
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)     1145 2024-04-09 03:53:33.000000 cellsnap-0.0.3/src/cellsnap.egg-info/PKG-INFO
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)      423 2024-04-09 03:53:33.000000 cellsnap-0.0.3/src/cellsnap.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)        1 2024-04-09 03:53:33.000000 cellsnap-0.0.3/src/cellsnap.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)      239 2024-04-09 03:53:33.000000 cellsnap-0.0.3/src/cellsnap.egg-info/requires.txt
+-rw-rw-r--   0 sheng     (1001) sheng     (1001)        9 2024-04-09 03:53:33.000000 cellsnap-0.0.3/src/cellsnap.egg-info/top_level.txt
```

### Comparing `CellSNAP-0.0.2/LICENSE` & `cellsnap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/PKG-INFO` & `cellsnap-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: CellSNAP
-Version: 0.0.2
+Name: cellsnap
+Version: 0.0.3
 Summary: A package for enhancing single-cell population delineation by integrating cross-domain information.
 Home-page: https://github.com/sggao/CellSNAP
 Author: Sheng Gao, Bokai Zhu
 Author-email: gaosheng0321@gmail.com, zhubokai@mit.edu
 Project-URL: Bug Tracker, https://github.com/sggao/CellSNAP/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CellSNAP-0.0.2/README.md` & `cellsnap-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/setup.cfg` & `cellsnap-0.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-name = CellSNAP
-version = 0.0.2
+name = cellsnap
+version = 0.0.3
 author = Sheng Gao, Bokai Zhu
 author_email = gaosheng0321@gmail.com, zhubokai@mit.edu
 description = A package for learning single-cell representations embedding by integrating cross-domain information.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sggao/CellSNAP
 project_urls =
```

### Comparing `CellSNAP-0.0.2/setup.py` & `cellsnap-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="CellSNAP",
-    version="0.0.2",
+    name="cellsnap",
+    version="0.0.3",
     author="Sheng Gao, Bokai Zhu",
     author_email="gaosheng0321@gmail.com, zhubokai@mit.edu",
     description="A package for enhancing single-cell population delineation by integrating cross-domain information.",
     long_description="Official implementation of Cell Spatial And Neighborhood Pattern (CellSNAP), a computational method that learns a single-cell representation embedding by integrating cross-domain information from tissue samples. Through the analysis of datasets spanning spatial proteomic and spatial transcriptomic modalities, and across different tissue types and disease settings, we demonstrate CellSNAP’s capability to elucidate biologically relevant cell populations that were previously elusive due to the relinquished tissue morphological information from images",
     long_description_content_type="text/markdown",
     url="https://github.com/sggao/CellSNAP",
     packages=setuptools.find_packages(),
```

### Comparing `CellSNAP-0.0.2/src/CellSNAP/cellsnap.py` & `cellsnap-0.0.3/src/CellSNAP/cellsnap.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP/datasets.py` & `cellsnap-0.0.3/src/CellSNAP/datasets.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP/graph.py` & `cellsnap-0.0.3/src/CellSNAP/graph.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP/main.py` & `cellsnap-0.0.3/src/CellSNAP/main.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP/models.py` & `cellsnap-0.0.3/src/CellSNAP/models.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP/preprocessing.py` & `cellsnap-0.0.3/src/CellSNAP/preprocessing.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP/utils.py` & `cellsnap-0.0.3/src/CellSNAP/utils.py`

 * *Files identical despite different names*

### Comparing `CellSNAP-0.0.2/src/CellSNAP.egg-info/PKG-INFO` & `cellsnap-0.0.3/src/cellsnap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: CellSNAP
-Version: 0.0.2
+Name: cellsnap
+Version: 0.0.3
 Summary: A package for enhancing single-cell population delineation by integrating cross-domain information.
 Home-page: https://github.com/sggao/CellSNAP
 Author: Sheng Gao, Bokai Zhu
 Author-email: gaosheng0321@gmail.com, zhubokai@mit.edu
 Project-URL: Bug Tracker, https://github.com/sggao/CellSNAP/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

