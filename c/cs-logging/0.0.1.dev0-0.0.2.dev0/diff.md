# Comparing `tmp/cs_logging-0.0.1.dev0.tar.gz` & `tmp/cs_logging-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs_logging-0.0.1.dev0.tar", last modified: Tue Apr  9 12:53:12 2024, max compression
+gzip compressed data, was "cs_logging-0.0.2.dev0.tar", last modified: Tue Apr  9 12:56:54 2024, max compression
```

## Comparing `cs_logging-0.0.1.dev0.tar` & `cs_logging-0.0.2.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:53:12.318012 cs_logging-0.0.1.dev0/
--rw-r--r--   0 arelius   (1000) arelius   (1000)      670 2024-04-09 12:53:12.318012 cs_logging-0.0.1.dev0/PKG-INFO
--rw-rw-r--   0 arelius   (1000) arelius   (1000)     1559 2024-04-09 12:53:10.000000 cs_logging-0.0.1.dev0/pyproject.toml
--rw-rw-r--   0 arelius   (1000) arelius   (1000)       38 2024-04-09 12:53:12.318012 cs_logging-0.0.1.dev0/setup.cfg
--rw-rw-r--   0 arelius   (1000) arelius   (1000)       38 2024-04-08 20:53:37.000000 cs_logging-0.0.1.dev0/setup.py
-drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:53:12.314012 cs_logging-0.0.1.dev0/src/
-drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:53:12.314012 cs_logging-0.0.1.dev0/src/cs_logging/
--rw-rw-r--   0 arelius   (1000) arelius   (1000)       10 2024-04-08 20:54:06.000000 cs_logging-0.0.1.dev0/src/cs_logging/VERSION.txt
--rw-rw-r--   0 arelius   (1000) arelius   (1000)        0 2024-04-08 20:53:49.000000 cs_logging-0.0.1.dev0/src/cs_logging/__init__.py
--rw-rw-r--   0 arelius   (1000) arelius   (1000)     3027 2024-04-09 12:39:33.000000 cs_logging-0.0.1.dev0/src/cs_logging/logger.py
-drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:53:12.314012 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/
--rw-r--r--   0 arelius   (1000) arelius   (1000)      670 2024-04-09 12:53:12.000000 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/PKG-INFO
--rw-rw-r--   0 arelius   (1000) arelius   (1000)      324 2024-04-09 12:53:12.000000 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 arelius   (1000) arelius   (1000)        1 2024-04-09 12:53:12.000000 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 arelius   (1000) arelius   (1000)       37 2024-04-09 12:53:12.000000 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/requires.txt
--rw-rw-r--   0 arelius   (1000) arelius   (1000)       11 2024-04-09 12:53:12.000000 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/top_level.txt
--rw-rw-r--   0 arelius   (1000) arelius   (1000)        1 2024-04-08 21:19:22.000000 cs_logging-0.0.1.dev0/src/cs_logging.egg-info/zip-safe
+drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:56:54.075012 cs_logging-0.0.2.dev0/
+-rw-r--r--   0 arelius   (1000) arelius   (1000)      684 2024-04-09 12:56:54.075012 cs_logging-0.0.2.dev0/PKG-INFO
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)     1573 2024-04-09 12:54:19.000000 cs_logging-0.0.2.dev0/pyproject.toml
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)       38 2024-04-09 12:56:54.075012 cs_logging-0.0.2.dev0/setup.cfg
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)       38 2024-04-08 20:53:37.000000 cs_logging-0.0.2.dev0/setup.py
+drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:56:54.071012 cs_logging-0.0.2.dev0/src/
+drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:56:54.075012 cs_logging-0.0.2.dev0/src/cs_logging/
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)       11 2024-04-09 12:55:34.000000 cs_logging-0.0.2.dev0/src/cs_logging/VERSION.txt
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)        0 2024-04-08 20:53:49.000000 cs_logging-0.0.2.dev0/src/cs_logging/__init__.py
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)     3027 2024-04-09 12:39:33.000000 cs_logging-0.0.2.dev0/src/cs_logging/logger.py
+drwxrwxr-x   0 arelius   (1000) arelius   (1000)        0 2024-04-09 12:56:54.075012 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/
+-rw-r--r--   0 arelius   (1000) arelius   (1000)      684 2024-04-09 12:56:54.000000 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)      324 2024-04-09 12:56:54.000000 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)        1 2024-04-09 12:56:54.000000 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)       37 2024-04-09 12:56:54.000000 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/requires.txt
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)       11 2024-04-09 12:56:54.000000 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/top_level.txt
+-rw-rw-r--   0 arelius   (1000) arelius   (1000)        1 2024-04-08 21:19:22.000000 cs_logging-0.0.2.dev0/src/cs_logging.egg-info/zip-safe
```

### Comparing `cs_logging-0.0.1.dev0/PKG-INFO` & `cs_logging-0.0.2.dev0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cs_logging
-Version: 0.0.1.dev0
-Summary: denoising tool for utter library
+Version: 0.0.2.dev0
+Summary: logging configuration based on ttbuda hpp file
 Author-email: Clark Saben <csaben@mail.umw.edu>
 Project-URL: code, https://github.com/csaben/cs-logging
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.0
```

### Comparing `cs_logging-0.0.1.dev0/pyproject.toml` & `cs_logging-0.0.2.dev0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=58.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cs_logging"
-description= "denoising tool for utter library"
+description= "logging configuration based on ttbuda hpp file"
 readme = "README.md"
 requires-python = ">=3.10.0"
 authors = [{ name = "Clark Saben", email = "csaben@mail.umw.edu"}]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `cs_logging-0.0.1.dev0/src/cs_logging/logger.py` & `cs_logging-0.0.2.dev0/src/cs_logging/logger.py`

 * *Files identical despite different names*

### Comparing `cs_logging-0.0.1.dev0/src/cs_logging.egg-info/PKG-INFO` & `cs_logging-0.0.2.dev0/src/cs_logging.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cs_logging
-Version: 0.0.1.dev0
-Summary: denoising tool for utter library
+Version: 0.0.2.dev0
+Summary: logging configuration based on ttbuda hpp file
 Author-email: Clark Saben <csaben@mail.umw.edu>
 Project-URL: code, https://github.com/csaben/cs-logging
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.0
```

