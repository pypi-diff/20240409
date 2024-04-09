# Comparing `tmp/convergence-0.6.1.tar.gz` & `tmp/convergence-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convergence-0.6.1.tar", last modified: Tue Apr  9 16:54:44 2024, max compression
+gzip compressed data, was "convergence-0.6.3.tar", last modified: Tue Apr  9 17:05:53 2024, max compression
```

## Comparing `convergence-0.6.1.tar` & `convergence-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.855396 convergence-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-09 16:54:39.000000 convergence-0.6.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-09 16:54:44.851396 convergence-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-09 16:54:39.000000 convergence-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 16:54:39.000000 convergence-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:54:44.855396 convergence-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/src/convergence/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25047 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/src/convergence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 16:54:39.000000 convergence-0.6.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-09 16:54:39.000000 convergence-0.6.1/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:05:53.400479 convergence-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-09 17:04:10.000000 convergence-0.6.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-09 17:05:53.400479 convergence-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-09 17:04:10.000000 convergence-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 17:05:42.000000 convergence-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:05:53.400479 convergence-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:05:53.396479 convergence-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:05:53.396479 convergence-0.6.3/src/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 17:04:10.000000 convergence-0.6.3/src/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-09 17:04:10.000000 convergence-0.6.3/src/convergence/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25047 2024-04-09 17:04:10.000000 convergence-0.6.3/src/convergence/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-04-09 17:04:10.000000 convergence-0.6.3/src/convergence/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:05:53.400479 convergence-0.6.3/src/convergence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-09 17:05:53.000000 convergence-0.6.3/src/convergence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 17:05:53.000000 convergence-0.6.3/src/convergence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:05:53.000000 convergence-0.6.3/src/convergence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 17:05:53.000000 convergence-0.6.3/src/convergence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 17:05:53.000000 convergence-0.6.3/src/convergence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:05:53.400479 convergence-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 17:04:10.000000 convergence-0.6.3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-09 17:04:10.000000 convergence-0.6.3/tests/test_interface.py
```

### Comparing `convergence-0.6.1/COPYING` & `convergence-0.6.3/COPYING`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/PKG-INFO` & `convergence-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convergence
-Version: 0.6.1
+Version: 0.6.3
 Summary: A Python program to Perform Calculations Associated with a Grid Convergence Study
 Author-email: Mathew Topper <damm_horse@yahoo.co.uk>
 Project-URL: Homepage, https://github.com/Data-Only-Greater/convergence
 Project-URL: Issues, https://github.com/Data-Only-Greater/convergence/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `convergence-0.6.1/README.md` & `convergence-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/pyproject.toml` & `convergence-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "convergence"
-version = "0.6.1"
+version = "0.6.3"
 authors = [
   {name = "Mathew Topper", email = "damm_horse@yahoo.co.uk"}
 ]
 description = "A Python program to Perform Calculations Associated with a Grid Convergence Study"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `convergence-0.6.1/src/convergence/__init__.py` & `convergence-0.6.3/src/convergence/__init__.py`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/src/convergence/functions.py` & `convergence-0.6.3/src/convergence/functions.py`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/src/convergence/interface.py` & `convergence-0.6.3/src/convergence/interface.py`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/src/convergence/tables.py` & `convergence-0.6.3/src/convergence/tables.py`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/src/convergence.egg-info/PKG-INFO` & `convergence-0.6.3/src/convergence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convergence
-Version: 0.6.1
+Version: 0.6.3
 Summary: A Python program to Perform Calculations Associated with a Grid Convergence Study
 Author-email: Mathew Topper <damm_horse@yahoo.co.uk>
 Project-URL: Homepage, https://github.com/Data-Only-Greater/convergence
 Project-URL: Issues, https://github.com/Data-Only-Greater/convergence/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `convergence-0.6.1/tests/test_functions.py` & `convergence-0.6.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `convergence-0.6.1/tests/test_interface.py` & `convergence-0.6.3/tests/test_interface.py`

 * *Files identical despite different names*

