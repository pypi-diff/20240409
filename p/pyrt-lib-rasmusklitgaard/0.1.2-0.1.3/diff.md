# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.1.2.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.1.2.tar", last modified: Tue Apr  9 08:40:23 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.1.3.tar", last modified: Tue Apr  9 08:45:06 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.1.2.tar` & `pyrt_lib_rasmusklitgaard-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:40:23.234348 pyrt_lib_rasmusklitgaard-0.1.2/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.2/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 08:40:23.234348 pyrt_lib_rasmusklitgaard-0.1.2/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.2/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-09 08:39:44.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:40:23.230348 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      156 2024-04-09 08:39:30.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-09 08:40:21.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-09 08:40:21.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:40:21.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12163 2024-04-09 08:40:21.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-09 08:40:21.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-09 08:40:21.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:40:23.234348 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 08:40:23.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-09 08:40:23.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-09 08:40:23.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-09 08:40:23.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-09 08:40:23.000000 pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-09 08:40:23.234348 pyrt_lib_rasmusklitgaard-0.1.2/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:45:06.848228 pyrt_lib_rasmusklitgaard-0.1.3/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.3/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 08:45:06.848228 pyrt_lib_rasmusklitgaard-0.1.3/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.3/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-09 08:44:56.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:45:06.848228 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      126 2024-04-09 08:44:27.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-09 08:45:04.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-09 08:45:04.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12163 2024-04-09 08:45:04.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-09 08:45:04.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-09 08:45:04.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:45:06.848228 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 08:45:06.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-09 08:45:06.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-09 08:45:06.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-09 08:45:06.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-09 08:45:06.000000 pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-09 08:45:06.848228 pyrt_lib_rasmusklitgaard-0.1.3/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/LICENSE` & `pyrt_lib_rasmusklitgaard-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.1.2
+Version: 0.1.3
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/README.md` & `pyrt_lib_rasmusklitgaard-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.1.2
+Version: 0.1.3
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.2/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.1.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

