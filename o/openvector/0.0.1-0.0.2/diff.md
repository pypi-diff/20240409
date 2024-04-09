# Comparing `tmp/openvector-0.0.1.tar.gz` & `tmp/openvector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvector-0.0.1.tar", last modified: Mon Apr  8 21:47:31 2024, max compression
+gzip compressed data, was "openvector-0.0.2.tar", last modified: Mon Apr  8 22:04:41 2024, max compression
```

## Comparing `openvector-0.0.1.tar` & `openvector-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 21:47:31.329138 openvector-0.0.1/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-08 21:28:19.000000 openvector-0.0.1/LICENSE
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      518 2024-04-08 21:47:31.329018 openvector-0.0.1/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       80 2024-04-08 21:46:15.000000 openvector-0.0.1/README.md
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 21:47:31.328251 openvector-0.0.1/openvector/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 21:31:08.000000 openvector-0.0.1/openvector/__init__.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       43 2024-04-08 21:44:57.000000 openvector-0.0.1/openvector/openvector.py
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 21:47:31.328828 openvector-0.0.1/openvector.egg-info/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      518 2024-04-08 21:47:31.000000 openvector-0.0.1/openvector.egg-info/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      210 2024-04-08 21:47:31.000000 openvector-0.0.1/openvector.egg-info/SOURCES.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-08 21:47:31.000000 openvector-0.0.1/openvector.egg-info/dependency_links.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-08 21:47:31.000000 openvector-0.0.1/openvector.egg-info/top_level.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-08 21:47:31.329184 openvector-0.0.1/setup.cfg
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      699 2024-04-08 21:47:05.000000 openvector-0.0.1/setup.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 22:04:41.508068 openvector-0.0.2/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-08 21:28:19.000000 openvector-0.0.2/LICENSE
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      699 2024-04-08 22:04:41.507937 openvector-0.0.2/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      294 2024-04-08 22:01:29.000000 openvector-0.0.2/README.md
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 22:04:41.506948 openvector-0.0.2/openvector/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 21:31:08.000000 openvector-0.0.2/openvector/__init__.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       43 2024-04-08 21:44:57.000000 openvector-0.0.2/openvector/openvector.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-08 22:04:41.507704 openvector-0.0.2/openvector.egg-info/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      699 2024-04-08 22:04:41.000000 openvector-0.0.2/openvector.egg-info/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      210 2024-04-08 22:04:41.000000 openvector-0.0.2/openvector.egg-info/SOURCES.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-08 22:04:41.000000 openvector-0.0.2/openvector.egg-info/dependency_links.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-08 22:04:41.000000 openvector-0.0.2/openvector.egg-info/top_level.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-08 22:04:41.508118 openvector-0.0.2/setup.cfg
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      660 2024-04-08 22:04:30.000000 openvector-0.0.2/setup.py
```

### Comparing `openvector-0.0.1/LICENSE` & `openvector-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openvector-0.0.1/PKG-INFO` & `openvector-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: openvector
-Version: 0.0.1
+Version: 0.0.2
 Summary: An open source vector embeddings database.
 Home-page: https://github.com/eddyjin1/openvector
 Author: Eddy Jin
-Author-email: eddy_jin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openvector
 
 An open source vector embeddings database.
 https://openvector.net
+
+https://pypi.org/project/openvector/
+
+```python
+pip install openvector
+```
+
+
+### Build and upload
+
+```shell
+pip install setuptools wheel twine
+
+python setup.py sdist bdist_wheel
+
+python -m twine upload dist/*
+```
```

### Comparing `openvector-0.0.1/openvector.egg-info/PKG-INFO` & `openvector-0.0.2/openvector.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 Metadata-Version: 2.1
 Name: openvector
-Version: 0.0.1
+Version: 0.0.2
 Summary: An open source vector embeddings database.
 Home-page: https://github.com/eddyjin1/openvector
 Author: Eddy Jin
-Author-email: eddy_jin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openvector
 
 An open source vector embeddings database.
 https://openvector.net
+
+https://pypi.org/project/openvector/
+
+```python
+pip install openvector
+```
+
+
+### Build and upload
+
+```shell
+pip install setuptools wheel twine
+
+python setup.py sdist bdist_wheel
+
+python -m twine upload dist/*
+```
```

### Comparing `openvector-0.0.1/setup.py` & `openvector-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="openvector",
-    version="0.0.1",
+    version="0.0.2",
     author="Eddy Jin",
-    author_email="eddy_jin@gmail.com",
     description="An open source vector embeddings database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eddyjin1/openvector",
     packages=setuptools.find_packages(),
     install_requires = [],
     classifiers=[
```

