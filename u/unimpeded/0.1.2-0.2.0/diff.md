# Comparing `tmp/unimpeded-0.1.2.tar.gz` & `tmp/unimpeded-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimpeded-0.1.2.tar", last modified: Fri Jun 30 10:57:23 2023, max compression
+gzip compressed data, was "unimpeded-0.2.0.tar", last modified: Tue Apr  9 09:35:17 2024, max compression
```

## Comparing `unimpeded-0.1.2.tar` & `unimpeded-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:57:23.673622 unimpeded-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 10:57:13.000000 unimpeded-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-30 10:57:23.673622 unimpeded-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-30 10:57:13.000000 unimpeded-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-30 10:57:13.000000 unimpeded-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 10:57:23.673622 unimpeded-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:57:23.673622 unimpeded-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-30 10:57:13.000000 unimpeded-0.1.2/tests/test_zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:57:23.673622 unimpeded-0.1.2/unimpeded/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 10:57:13.000000 unimpeded-0.1.2/unimpeded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 10:57:13.000000 unimpeded-0.1.2/unimpeded/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-06-30 10:57:13.000000 unimpeded-0.1.2/unimpeded/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:57:23.673622 unimpeded-0.1.2/unimpeded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-30 10:57:23.000000 unimpeded-0.1.2/unimpeded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-30 10:57:23.000000 unimpeded-0.1.2/unimpeded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:57:23.000000 unimpeded-0.1.2/unimpeded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 10:57:23.000000 unimpeded-0.1.2/unimpeded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 10:57:23.000000 unimpeded-0.1.2/unimpeded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:35:17.970121 unimpeded-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 09:35:13.000000 unimpeded-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-09 09:35:17.970121 unimpeded-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-09 09:35:13.000000 unimpeded-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-09 09:35:13.000000 unimpeded-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 09:35:17.970121 unimpeded-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:35:17.970121 unimpeded-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 09:35:13.000000 unimpeded-0.2.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:35:17.970121 unimpeded-0.2.0/unimpeded/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 09:35:13.000000 unimpeded-0.2.0/unimpeded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 09:35:13.000000 unimpeded-0.2.0/unimpeded/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:35:17.970121 unimpeded-0.2.0/unimpeded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-09 09:35:17.000000 unimpeded-0.2.0/unimpeded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 09:35:17.000000 unimpeded-0.2.0/unimpeded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:35:17.000000 unimpeded-0.2.0/unimpeded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 09:35:17.000000 unimpeded-0.2.0/unimpeded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:35:17.000000 unimpeded-0.2.0/unimpeded.egg-info/top_level.txt
```

### Comparing `unimpeded-0.1.2/LICENSE` & `unimpeded-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unimpeded-0.1.2/PKG-INFO` & `unimpeded-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.1.2
+Version: 0.2.0
 Summary: Universal model comparison & parameter estimation over diverse datasets
 Author-email: Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,24 +39,35 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: anesthetic
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pydocstyle; extra == "test"
+Requires-Dist: packaging; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
 
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.1.2
+:Version: 0.2.0
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.1.2/README.rst` & `unimpeded-0.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.1.2
+:Version: 0.2.0
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.1.2/pyproject.toml` & `unimpeded-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unimpeded-0.1.2/unimpeded.egg-info/PKG-INFO` & `unimpeded-0.2.0/unimpeded.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.1.2
+Version: 0.2.0
 Summary: Universal model comparison & parameter estimation over diverse datasets
 Author-email: Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,24 +39,35 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: anesthetic
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pydocstyle; extra == "test"
+Requires-Dist: packaging; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
 
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.1.2
+:Version: 0.2.0
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

