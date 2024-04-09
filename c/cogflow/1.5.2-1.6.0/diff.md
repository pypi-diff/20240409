# Comparing `tmp/cogflow-1.5.2.tar.gz` & `tmp/cogflow-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.5.2.tar", last modified: Tue Mar 26 23:03:36 2024, max compression
+gzip compressed data, was "cogflow-1.6.0.tar", last modified: Tue Mar 26 22:16:51 2024, max compression
```

## Comparing `cogflow-1.5.2.tar` & `cogflow-1.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:03:36.126283 cogflow-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-26 23:03:36.126283 cogflow-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-26 23:03:23.000000 cogflow-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:03:36.122283 cogflow-1.5.2/cogflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 23:03:23.000000 cogflow-1.5.2/cogflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18896 2024-03-26 23:03:23.000000 cogflow-1.5.2/cogflow/cog_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-26 23:03:23.000000 cogflow-1.5.2/cogflow/constant_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 23:03:36.126283 cogflow-1.5.2/cogflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-26 23:03:36.000000 cogflow-1.5.2/cogflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-26 23:03:36.000000 cogflow-1.5.2/cogflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 23:03:36.000000 cogflow-1.5.2/cogflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-26 23:03:36.000000 cogflow-1.5.2/cogflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 23:03:36.000000 cogflow-1.5.2/cogflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 23:03:36.126283 cogflow-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-26 23:03:23.000000 cogflow-1.5.2/setup.py
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/
+-rw-r--r--   0 bola      (1000) bola      (1000)      681 2024-03-26 22:16:51.068174 cogflow-1.6.0/PKG-INFO
+-rw-rw-r--   0 bola      (1000) bola      (1000)     3878 2024-03-18 14:03:47.000000 cogflow-1.6.0/README.md
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/cogflow/
+-rw-rw-r--   0 bola      (1000) bola      (1000)        0 2024-03-18 14:03:47.000000 cogflow-1.6.0/cogflow/__init__.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)    18896 2024-03-26 21:19:58.000000 cogflow-1.6.0/cogflow/cog_framework.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)      197 2024-03-18 14:03:47.000000 cogflow-1.6.0/cogflow/constant_vars.py
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/cogflow.egg-info/
+-rw-r--r--   0 bola      (1000) bola      (1000)      681 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/PKG-INFO
+-rw-rw-r--   0 bola      (1000) bola      (1000)      242 2024-03-26 22:16:51.000000 cogflow-1.6.0/cogflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)        1 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)      144 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/requires.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)        8 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/top_level.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)       38 2024-03-26 22:16:51.068174 cogflow-1.6.0/setup.cfg
+-rw-rw-r--   0 bola      (1000) bola      (1000)      808 2024-03-26 21:20:18.000000 cogflow-1.6.0/setup.py
```

### Comparing `cogflow-1.5.2/PKG-INFO` & `cogflow-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.5.2
+Version: 1.6.0
 Summary: cog modules
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `cogflow-1.5.2/README.md` & `cogflow-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.5.2/cogflow/cog_framework.py` & `cogflow-1.6.0/cogflow/cog_framework.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.5.2/cogflow.egg-info/PKG-INFO` & `cogflow-1.6.0/cogflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.5.2
+Version: 1.6.0
 Summary: cog modules
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `cogflow-1.5.2/setup.py` & `cogflow-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cogflow",
-    version="1.5.2",
+    version="1.6.0",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
```

