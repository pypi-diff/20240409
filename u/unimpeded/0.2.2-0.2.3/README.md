# Comparing `tmp/unimpeded-0.2.2.tar.gz` & `tmp/unimpeded-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimpeded-0.2.2.tar", last modified: Tue Apr  9 18:32:48 2024, max compression
+gzip compressed data, was "unimpeded-0.2.3.tar", last modified: Tue Apr  9 19:49:00 2024, max compression
```

## Comparing `unimpeded-0.2.2.tar` & `unimpeded-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:32:48.905645 unimpeded-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 18:32:44.000000 unimpeded-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-09 18:32:48.905645 unimpeded-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-09 18:32:44.000000 unimpeded-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-09 18:32:44.000000 unimpeded-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 18:32:48.905645 unimpeded-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:32:48.901645 unimpeded-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 18:32:44.000000 unimpeded-0.2.2/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:32:48.901645 unimpeded-0.2.2/unimpeded/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 18:32:44.000000 unimpeded-0.2.2/unimpeded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 18:32:44.000000 unimpeded-0.2.2/unimpeded/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:32:48.905645 unimpeded-0.2.2/unimpeded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-09 18:32:48.000000 unimpeded-0.2.2/unimpeded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 18:32:48.000000 unimpeded-0.2.2/unimpeded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:32:48.000000 unimpeded-0.2.2/unimpeded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 18:32:48.000000 unimpeded-0.2.2/unimpeded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 18:32:48.000000 unimpeded-0.2.2/unimpeded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:49:00.752035 unimpeded-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 19:48:56.000000 unimpeded-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-09 19:49:00.752035 unimpeded-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-09 19:48:56.000000 unimpeded-0.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-09 19:48:56.000000 unimpeded-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:49:00.752035 unimpeded-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:49:00.752035 unimpeded-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 19:48:56.000000 unimpeded-0.2.3/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:49:00.752035 unimpeded-0.2.3/unimpeded/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 19:48:56.000000 unimpeded-0.2.3/unimpeded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 19:48:56.000000 unimpeded-0.2.3/unimpeded/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:49:00.752035 unimpeded-0.2.3/unimpeded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-09 19:49:00.000000 unimpeded-0.2.3/unimpeded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 19:49:00.000000 unimpeded-0.2.3/unimpeded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:49:00.000000 unimpeded-0.2.3/unimpeded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 19:49:00.000000 unimpeded-0.2.3/unimpeded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 19:49:00.000000 unimpeded-0.2.3/unimpeded.egg-info/top_level.txt
```

### Comparing `unimpeded-0.2.2/LICENSE` & `unimpeded-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unimpeded-0.2.2/PKG-INFO` & `unimpeded-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.2.2
+Version: 0.2.3
 Summary: Universal model comparison & parameter estimation over diverse datasets
 Author-email: Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,15 +59,15 @@
 Requires-Dist: pre-commit; extra == "test"
 
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.2.2
+:Version: 0.2.3
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.2.2/README.rst` & `unimpeded-0.2.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.2.2
+:Version: 0.2.3
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.2.2/pyproject.toml` & `unimpeded-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unimpeded-0.2.2/unimpeded.egg-info/PKG-INFO` & `unimpeded-0.2.3/unimpeded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.2.2
+Version: 0.2.3
 Summary: Universal model comparison & parameter estimation over diverse datasets
 Author-email: Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,15 +59,15 @@
 Requires-Dist: pre-commit; extra == "test"
 
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.2.2
+:Version: 0.2.3
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

