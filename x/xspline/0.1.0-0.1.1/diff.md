# Comparing `tmp/xspline-0.1.0.tar.gz` & `tmp/xspline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspline-0.1.0.tar", last modified: Thu Aug 10 07:13:41 2023, max compression
+gzip compressed data, was "xspline-0.1.1.tar", last modified: Tue Apr  9 09:49:23 2024, max compression
```

## Comparing `xspline-0.1.0.tar` & `xspline-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:13:41.866325 xspline-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-10 07:13:13.000000 xspline-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-10 07:13:41.866325 xspline-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-10 07:13:13.000000 xspline-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-10 07:13:13.000000 xspline-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-10 07:13:41.866325 xspline-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:13:41.862325 xspline-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:13:41.866325 xspline-0.1.0/src/xspline/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/bspl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/indi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/xfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-10 07:13:13.000000 xspline-0.1.0/src/xspline/xspl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:13:41.866325 xspline-0.1.0/src/xspline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-10 07:13:41.000000 xspline-0.1.0/src/xspline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-10 07:13:41.000000 xspline-0.1.0/src/xspline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-10 07:13:41.000000 xspline-0.1.0/src/xspline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-10 07:13:41.000000 xspline-0.1.0/src/xspline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-10 07:13:41.000000 xspline-0.1.0/src/xspline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 07:13:41.866325 xspline-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-10 07:13:13.000000 xspline-0.1.0/tests/test_basis_xfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-10 07:13:13.000000 xspline-0.1.0/tests/test_bspl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-10 07:13:13.000000 xspline-0.1.0/tests/test_indi.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-10 07:13:13.000000 xspline-0.1.0/tests/test_poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-10 07:13:13.000000 xspline-0.1.0/tests/test_xfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-10 07:13:13.000000 xspline-0.1.0/tests/test_xspl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:49:23.138893 xspline-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-09 09:49:08.000000 xspline-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-09 09:49:23.138893 xspline-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 09:49:08.000000 xspline-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-09 09:49:08.000000 xspline-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:49:23.138893 xspline-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:49:23.130893 xspline-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:49:23.134893 xspline-0.1.1/src/xspline/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/bspl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/indi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/xfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-09 09:49:08.000000 xspline-0.1.1/src/xspline/xspl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:49:23.138893 xspline-0.1.1/src/xspline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-09 09:49:23.000000 xspline-0.1.1/src/xspline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 09:49:23.000000 xspline-0.1.1/src/xspline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:49:23.000000 xspline-0.1.1/src/xspline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 09:49:23.000000 xspline-0.1.1/src/xspline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 09:49:23.000000 xspline-0.1.1/src/xspline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:49:23.134893 xspline-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-09 09:49:08.000000 xspline-0.1.1/tests/test_basis_xfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 09:49:08.000000 xspline-0.1.1/tests/test_bspl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-09 09:49:08.000000 xspline-0.1.1/tests/test_indi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 09:49:08.000000 xspline-0.1.1/tests/test_poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-09 09:49:08.000000 xspline-0.1.1/tests/test_xfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 09:49:08.000000 xspline-0.1.1/tests/test_xspl.py
```

### Comparing `xspline-0.1.0/LICENSE` & `xspline-0.1.1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2023, IHME Math Sciences
+Copyright (c) 2019-2024, IHME Math Sciences
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `xspline-0.1.0/README.rst` & `xspline-0.1.1/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 .. image:: https://img.shields.io/pypi/l/xspline
-    :target: https://github.com/zhengp0/xspline/blob/main/LICENSE
+    :target: https://github.com/ihmeuw-msca/xspline/blob/main/LICENSE
 
 .. image:: https://img.shields.io/pypi/v/xspline
     :target: https://pypi.org/project/xspline
 
-.. image:: https://img.shields.io/github/actions/workflow/status/zhengp0/xspline/python-build.yml?branch=main
-    :target: https://github.com/zhengp0/xspline/actions
+.. image:: https://img.shields.io/github/actions/workflow/status/ihmeuw-msca/xspline/python-build.yml?branch=main
+    :target: https://github.com/ihmeuw-msca/xspline/actions
 
 .. image:: https://img.shields.io/badge/docs-here-green
-    :target: https://zhengp0.github.io/xspline
+    :target: https://ihmeuw-msca.github.io/xspline
 
-.. image:: https://codecov.io/gh/zhengp0/xspline/branch/main/graph/badge.svg?token=WUV5OR77N8 
-    :target: https://codecov.io/gh/zhengp0/xspline
+.. image:: https://img.shields.io/codecov/c/github/ihmeuw-msca/xspline
+    :target: https://codecov.io/gh/ihmeuw-msca/xspline
 
-.. image:: https://app.codacy.com/project/badge/Grade/308cc2771871498fbcdaee3440e56ad0
-    :target: https://app.codacy.com/gh/zhengp0/xspline/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+.. image:: https://img.shields.io/codacy/grade/f1646d62d6764e77a59d6c71df262ed4
+    :target: https://app.codacy.com/gh/ihmeuw-msca/xspline/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 
 XSpline
 =======
 
 Advanced spline package that provides b-spline bases, their derivatives and integrals.
 
 
-* `Installation <https://zhengp0.github.io/xspline/installation.html>`_
-* `Quickstart <https://zhengp0.github.io/xspline/quickstart.html>`_
+* `Installation <https://ihmeuw-msca.github.io/xspline/installation.html>`_
+* `Quickstart <https://ihmeuw-msca.github.io/xspline/quickstart.html>`_
```

### Comparing `xspline-0.1.0/pyproject.toml` & `xspline-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xspline"
-version = "0.1.0"
+version = "0.1.1"
 description = "Advanced spline package that provides b-spline bases, their derivatives and integrals"
 readme = "README.rst"
 requires-python = ">=3.10"
-license = { file = "LICENSE" }
+license = { text = "BSD 2-Clause" }
 authors = [
     { name = "IHME Math Sciences", email = "ihme.math.sciences@gmail.com" },
 ]
 dependencies = ["numpy>=1.25.1"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 docs = ["sphinx", "sphinx-autodoc-typehints", "furo"]
 
 [project.urls]
-github = "https://github.com/zhengp0/xspline"
-
-[tool.sphinx]
-project = "xspline"
-author = "IHME Math Sciences"
-copyright = "2023, IHME Math Sciences"
-version = "0.1.0"
+github = "https://github.com/ihmeuw-msca/xspline"
```

### Comparing `xspline-0.1.0/src/xspline/bspl.py` & `xspline-0.1.1/src/xspline/bspl.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/src/xspline/indi.py` & `xspline-0.1.1/src/xspline/indi.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/src/xspline/poly.py` & `xspline-0.1.1/src/xspline/poly.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/src/xspline/typing.py` & `xspline-0.1.1/src/xspline/typing.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/src/xspline/xfunction.py` & `xspline-0.1.1/src/xspline/xfunction.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/src/xspline/xspl.py` & `xspline-0.1.1/src/xspline/xspl.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/tests/test_basis_xfunction.py` & `xspline-0.1.1/tests/test_basis_xfunction.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/tests/test_bspl.py` & `xspline-0.1.1/tests/test_bspl.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/tests/test_indi.py` & `xspline-0.1.1/tests/test_indi.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/tests/test_poly.py` & `xspline-0.1.1/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/tests/test_xfunction.py` & `xspline-0.1.1/tests/test_xfunction.py`

 * *Files identical despite different names*

### Comparing `xspline-0.1.0/tests/test_xspl.py` & `xspline-0.1.1/tests/test_xspl.py`

 * *Files identical despite different names*

