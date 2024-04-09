# Comparing `tmp/loopsim-0.5.0.tar.gz` & `tmp/loopsim-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopsim-0.5.0.tar", max compression
+gzip compressed data, was "loopsim-0.5.1.tar", max compression
```

## Comparing `loopsim-0.5.0.tar` & `loopsim-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1119 2023-07-01 09:29:45.124005 loopsim-0.5.0/LICENSE
--rw-r--r--   0        0        0       22 2023-09-25 17:18:46.233359 loopsim-0.5.0/loopsim/__init__.py
--rw-r--r--   0        0        0       59 2023-04-12 00:42:22.535797 loopsim-0.5.0/loopsim/__main__.py
--rwxr-xr-x   0        0        0     2715 2023-06-26 14:56:26.502571 loopsim-0.5.0/loopsim/analyze.py
--rw-r--r--   0        0        0     3243 2023-07-04 10:54:37.475195 loopsim-0.5.0/loopsim/batch_analyze.py
--rw-r--r--   0        0        0      753 2023-07-04 11:17:20.278702 loopsim-0.5.0/loopsim/cli.py
--rw-r--r--   0        0        0      322 2023-04-12 00:42:22.536114 loopsim-0.5.0/loopsim/common.py
--rwxr-xr-x   0        0        0     6538 2024-02-20 23:10:00.383152 loopsim-0.5.0/loopsim/simulate.py
--rw-r--r--   0        0        0     5725 2023-07-04 11:40:26.672482 loopsim-0.5.0/loopsim/validate.py
--rwxr-xr-x   0        0        0     2356 2023-04-12 00:42:22.536362 loopsim-0.5.0/loopsim/visualize.py
--rw-r--r--   0        0        0     1103 2024-04-09 19:09:59.119814 loopsim-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 loopsim-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-07-01 09:29:45.124005 loopsim-0.5.1/LICENSE
+-rw-r--r--   0        0        0       22 2024-04-09 19:26:26.933225 loopsim-0.5.1/loopsim/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-12 00:42:22.535797 loopsim-0.5.1/loopsim/__main__.py
+-rwxr-xr-x   0        0        0     2715 2023-06-26 14:56:26.502571 loopsim-0.5.1/loopsim/analyze.py
+-rw-r--r--   0        0        0     3243 2023-07-04 10:54:37.475195 loopsim-0.5.1/loopsim/batch_analyze.py
+-rw-r--r--   0        0        0      753 2023-07-04 11:17:20.278702 loopsim-0.5.1/loopsim/cli.py
+-rw-r--r--   0        0        0      322 2023-04-12 00:42:22.536114 loopsim-0.5.1/loopsim/common.py
+-rwxr-xr-x   0        0        0     6538 2024-02-20 23:10:00.383152 loopsim-0.5.1/loopsim/simulate.py
+-rw-r--r--   0        0        0     5725 2023-07-04 11:40:26.672482 loopsim-0.5.1/loopsim/validate.py
+-rwxr-xr-x   0        0        0     2356 2023-04-12 00:42:22.536362 loopsim-0.5.1/loopsim/visualize.py
+-rw-r--r--   0        0        0     1103 2024-04-09 19:26:40.299878 loopsim-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 loopsim-0.5.1/PKG-INFO
```

### Comparing `loopsim-0.5.0/LICENSE` & `loopsim-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/loopsim/analyze.py` & `loopsim-0.5.1/loopsim/analyze.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/loopsim/batch_analyze.py` & `loopsim-0.5.1/loopsim/batch_analyze.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/loopsim/cli.py` & `loopsim-0.5.1/loopsim/cli.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/loopsim/simulate.py` & `loopsim-0.5.1/loopsim/simulate.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/loopsim/validate.py` & `loopsim-0.5.1/loopsim/validate.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/loopsim/visualize.py` & `loopsim-0.5.1/loopsim/visualize.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.0/pyproject.toml` & `loopsim-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loopsim"
-version = "0.5.0"
+version = "0.5.1"
 description = "Loopsim: Enrichment Analysis of Chromosome Conformation Capture with Fast Empirical Distribution Simulation"
 authors = ["Gideon Shaked <gshaked@umich.edu>"]
 maintainers = ["Gideon Shaked <gshaked@umich.edu>"]
 repository = "https://github.com/CutaneousBioinf/loopsim"
 classifiers = ["Environment :: Console",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `loopsim-0.5.0/PKG-INFO` & `loopsim-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopsim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Loopsim: Enrichment Analysis of Chromosome Conformation Capture with Fast Empirical Distribution Simulation
 Home-page: https://github.com/CutaneousBioinf/loopsim
 License: MIT
 Author: Gideon Shaked
 Author-email: gshaked@umich.edu
 Maintainer: Gideon Shaked
 Maintainer-email: gshaked@umich.edu
```

