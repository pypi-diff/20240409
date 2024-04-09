# Comparing `tmp/mcda-0.6.1.tar.gz` & `tmp/mcda-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcda-0.6.1.tar", last modified: Mon Feb  5 15:07:20 2024, max compression
+gzip compressed data, was "mcda-0.7.0.tar", last modified: Mon Apr  8 16:22:12 2024, max compression
```

## Comparing `mcda-0.6.1.tar` & `mcda-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.812504 mcda-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-02-05 15:07:08.000000 mcda-0.6.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-02-05 15:07:08.000000 mcda-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3915 2024-02-05 15:07:20.812504 mcda-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2118 2024-02-05 15:07:08.000000 mcda-0.6.1/README.PYPI.md
--rw-rw-rw-   0 root         (0) root         (0)     2502 2024-02-05 15:07:08.000000 mcda-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-02-05 15:07:08.000000 mcda-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-05 15:07:20.812504 mcda-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.802504 mcda-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.804504 mcda-0.6.1/src/mcda/
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.809504 mcda-0.6.1/src/mcda/core/
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23763 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/aggregators.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/aliases.py
--rw-rw-rw-   0 root         (0) root         (0)     2762 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/categories.py
--rw-rw-rw-   0 root         (0) root         (0)    13399 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/criteria_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15372 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    37711 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    18271 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/relations.py
--rw-rw-rw-   0 root         (0) root         (0)    25027 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/scales.py
--rw-rw-rw-   0 root         (0) root         (0)    18845 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/set_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    21430 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/transformers.py
--rw-rw-rw-   0 root         (0) root         (0)    12412 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/core/values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.809504 mcda-0.6.1/src/mcda/dea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/dea/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.809504 mcda-0.6.1/src/mcda/mavt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/mavt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25938 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/mavt/uta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.811504 mcda-0.6.1/src/mcda/outranking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/outranking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39245 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/outranking/electre.py
--rw-rw-rw-   0 root         (0) root         (0)    32330 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/outranking/promethee.py
--rw-rw-rw-   0 root         (0) root         (0)    38038 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/outranking/srmp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.811504 mcda-0.6.1/src/mcda/plot/
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42793 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-02-05 15:07:08.000000 mcda-0.6.1/src/mcda/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 15:07:20.811504 mcda-0.6.1/src/mcda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3915 2024-02-05 15:07:20.000000 mcda-0.6.1/src/mcda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      862 2024-02-05 15:07:20.000000 mcda-0.6.1/src/mcda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-05 15:07:20.000000 mcda-0.6.1/src/mcda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-02-05 15:07:20.000000 mcda-0.6.1/src/mcda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-02-05 15:07:20.000000 mcda-0.6.1/src/mcda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.167923 mcda-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-08 16:22:01.000000 mcda-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-08 16:22:01.000000 mcda-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4365 2024-04-08 16:22:12.167923 mcda-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-04-08 16:22:01.000000 mcda-0.7.0/README.PYPI.md
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-08 16:22:01.000000 mcda-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2024-04-08 16:22:01.000000 mcda-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 16:22:12.167923 mcda-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.154923 mcda-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.158923 mcda-0.7.0/src/mcda/
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.159923 mcda-0.7.0/src/mcda/internal/
+-rw-rw-rw-   0 root         (0) root         (0)      218 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.162923 mcda-0.7.0/src/mcda/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24045 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/aggregators.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/aliases.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)    13489 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/criteria_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15171 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    46938 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    21757 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    23860 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    19032 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    21526 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15038 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/core/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.163923 mcda-0.7.0/src/mcda/internal/dea/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/dea/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.163923 mcda-0.7.0/src/mcda/internal/mavt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/mavt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26220 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/mavt/uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.164923 mcda-0.7.0/src/mcda/internal/outranking/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39391 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/electre.py
+-rw-rw-rw-   0 root         (0) root         (0)    32686 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/promethee.py
+-rw-rw-rw-   0 root         (0) root         (0)    38234 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/outranking/srmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.164923 mcda-0.7.0/src/mcda/internal/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44068 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/internal/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/matrices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.165923 mcda-0.7.0/src/mcda/mavt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/mavt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/mavt/aggregators.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/mavt/uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.166923 mcda-0.7.0/src/mcda/outranking/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/electre.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/promethee.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/outranking/srmp.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/scales.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-08 16:22:01.000000 mcda-0.7.0/src/mcda/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:22:12.166923 mcda-0.7.0/src/mcda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4365 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 16:22:12.000000 mcda-0.7.0/src/mcda.egg-info/top_level.txt
```

### Comparing `mcda-0.6.1/LICENSE` & `mcda-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcda-0.6.1/PKG-INFO` & `mcda-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mcda
-Version: 0.6.1
+Version: 0.7.0
 Summary: Package for Multi Criteria Decision Analysis
-Author-email: Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>
+Author-email: Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>, Patrick Meyer <patrick.meyer@imt-atlantique.fr>
 License: Copyright IMT Atlantique, 2021
         
         Project leaders:
           Patrick Meyer <patrick.meyer@imt-atlantique.fr>
           Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>
         
         This software is an all-in-one package for Multi-Criteria Decision Analysis.
@@ -29,21 +29,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: matplotlib
 Requires-Dist: pulp
-Requires-Dist: graphviz
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: Deprecated
 Requires-Dist: typing_extensions; python_version < "3.11"
+Provides-Extra: plot
+Requires-Dist: graphviz; extra == "plot"
+Requires-Dist: matplotlib; extra == "plot"
+Provides-Extra: all
+Requires-Dist: mcda[plot]; extra == "all"
 
 Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
@@ -68,14 +71,27 @@
 
 If you want to simply use this package, simply install it from [PyPI](https://pypi.org/project/mcda/):
 
 ```bash
 pip install mcda
 ```
 
+**Note:**
+
+This package can be installed with different optional dependencies to unlock full features:
+
+* plot: unlock plotting utilities
+* all: include all the above optional dependencies
+
+If you want all optional dependencies for instance, do:
+
+```bash
+pip install "mcda[all]"
+```
+
 Once you installed our package, you can have a look at our [notebooks](https://py-mcda.readthedocs.io/en/latest/notebooks.html) section which contains examples on how to use our package.
 
 If you want to contribute to this package development, we recommend you to read the next section.
 
 
 # Contributors
```

### Comparing `mcda-0.6.1/README.PYPI.md` & `mcda-0.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+
 Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
+# Table of contents
+
+[TOC]
+
+
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
 It also contains relatively low-level plotting functions to visualize a MCDA problem and its solution.
 
 It is released on PyPI as [mcda](https://pypi.org/project/mcda/).
 
@@ -25,17 +31,48 @@
 
 If you want to simply use this package, simply install it from [PyPI](https://pypi.org/project/mcda/):
 
 ```bash
 pip install mcda
 ```
 
-Once you installed our package, you can have a look at our [notebooks](https://py-mcda.readthedocs.io/en/latest/notebooks.html) section which contains examples on how to use our package.
+**Note:**
+
+This package can be installed with different optional dependencies to unlock full features:
+
+* plot: unlock plotting utilities
+* all: include all the above optional dependencies
+
+If you want all optional dependencies for instance, do:
+
+```bash
+pip install "mcda[all]"
+```
+
+Once you installed our package, you can have a look at our [notebooks](examples/) section which contains examples on how to use our package.
+
+If you want to contribute to this package development, we recommend you to read [this](#contributors).
+
+
+# Documentation
+
+Documentation on this package can be found [here](https://py-mcda.readthedocs.io/).
+
+It also can be built locally by executing the following command in the package root folder:
+
+```bash
+make doc
+```
+
+and then visiting `doc/html/index.html` (this can be useful if you're not using a released version of this package).
+
+
+# Notebooks
 
-If you want to contribute to this package development, we recommend you to read the next section.
+We added [jupyter notebooks](https://jupyter.org/) that can be run as examples in [examples/](examples/).
 
 
 # Contributors
 
 This package is growing continuously and contributions are welcomed.
 Contributions can come in the form of new features, bug fixes, documentation improvements
 or any combination thereof.
@@ -45,13 +82,13 @@
 If you have any new ideas or have found bugs, feel free to [create an issue](https://gitlab.com/decide.imt-atlantique/pymcda/-/issues/new>).
 Finally, any contribution must be proposed for integration as a [Merge Request](https://gitlab.com/decide.imt-atlantique/pymcda/-/merge_requests/new).
 
 
 # License
 
 This software is licensed under the [European Union Public Licence (EUPL) v1.2](https://joinup.ec.europa.eu/page/eupl-text-11-12).
-For more information see [LICENSE](https://gitlab.com/decide.imt-atlantique/pymcda/-/blob/master/LICENSE).
+For more information see [LICENSE](LICENSE).
 
 
 # Citations
 
 @todo write section
```

### Comparing `mcda-0.6.1/README.md` & `mcda-0.7.0/README.PYPI.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-
 Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
-# Table of contents
-
-[TOC]
-
-
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
 It also contains relatively low-level plotting functions to visualize a MCDA problem and its solution.
 
 It is released on PyPI as [mcda](https://pypi.org/project/mcda/).
 
@@ -31,35 +25,30 @@
 
 If you want to simply use this package, simply install it from [PyPI](https://pypi.org/project/mcda/):
 
 ```bash
 pip install mcda
 ```
 
-Once you installed our package, you can have a look at our [notebooks](examples/) section which contains examples on how to use our package.
+**Note:**
 
-If you want to contribute to this package development, we recommend you to read [this](#contributors).
+This package can be installed with different optional dependencies to unlock full features:
 
+* plot: unlock plotting utilities
+* all: include all the above optional dependencies
 
-# Documentation
-
-Documentation on this package can be found [here](https://py-mcda.readthedocs.io/).
-
-It also can be built locally by executing the following command in the package root folder:
+If you want all optional dependencies for instance, do:
 
 ```bash
-make doc
+pip install "mcda[all]"
 ```
 
-and then visiting `doc/html/index.html` (this can be useful if you're not using a released version of this package).
-
-
-# Notebooks
+Once you installed our package, you can have a look at our [notebooks](https://py-mcda.readthedocs.io/en/latest/notebooks.html) section which contains examples on how to use our package.
 
-We added [jupyter notebooks](https://jupyter.org/) that can be run as examples in [examples/](examples/).
+If you want to contribute to this package development, we recommend you to read the next section.
 
 
 # Contributors
 
 This package is growing continuously and contributions are welcomed.
 Contributions can come in the form of new features, bug fixes, documentation improvements
 or any combination thereof.
@@ -69,13 +58,13 @@
 If you have any new ideas or have found bugs, feel free to [create an issue](https://gitlab.com/decide.imt-atlantique/pymcda/-/issues/new>).
 Finally, any contribution must be proposed for integration as a [Merge Request](https://gitlab.com/decide.imt-atlantique/pymcda/-/merge_requests/new).
 
 
 # License
 
 This software is licensed under the [European Union Public Licence (EUPL) v1.2](https://joinup.ec.europa.eu/page/eupl-text-11-12).
-For more information see [LICENSE](LICENSE).
+For more information see [LICENSE](https://gitlab.com/decide.imt-atlantique/pymcda/-/blob/master/LICENSE).
 
 
 # Citations
 
 @todo write section
```

### Comparing `mcda-0.6.1/pyproject.toml` & `mcda-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
 
 [project]
 name = "mcda"
-version = "0.6.1"
+version = "0.7.0"
 authors = [
   { name="Nicolas Duminy", email="nicolas.duminy@imt-atlantique.fr" },
+  { name="Patrick Meyer", email="patrick.meyer@imt-atlantique.fr" },
 ]
 description = "Package for Multi Criteria Decision Analysis"
 readme = "README.PYPI.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -31,20 +32,28 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
     "numpy",
-    "matplotlib",
     "pulp",
-    "graphviz",
     "scikit-learn",
     "pandas",
     "Deprecated",
     "typing_extensions; python_version < '3.11'",
 ]
 
+[project.optional-dependencies]
+plot = [
+    "graphviz",
+    "matplotlib"
+]
+all = [
+    "mcda[plot]"
+]
+
+
 [project.urls]
 Homepage = "https://py-mcda.readthedocs.io"
 Source = "https://gitlab.com/decide.imt-atlantique/pymcda"
 Issues = "https://gitlab.com/decide.imt-atlantique/pymcda/issues"
```

### Comparing `mcda-0.6.1/src/mcda/core/aggregators.py` & `mcda-0.7.0/src/mcda/internal/core/aggregators.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     FuzzyScale,
     QuantitativeScale,
     Scale,
     common_scale_type,
 )
 from ..core.set_functions import ISetFunction, Mobius
 from ..core.values import CommensurableValues, Values
+from .utils import set_module
 
 I_S = TypeVar("I_S", bound=Scale, covariant=True)
 O_S = TypeVar("O_S", bound=Scale, covariant=True)
 
 
 class Aggregator(Generic[I_S, O_S], ABC):
     """This abstract class represents a typical aggregator.
@@ -241,14 +242,15 @@
         if isinstance(data, DataFrame):
             return self._aggregate_dataframe(data, *args, **kwargs)
         if isinstance(data, Values):
             return self._aggregate_values(data, *args, **kwargs)
         return self._aggregate_series(data, *args, **kwargs)
 
 
+@set_module("mcda.mavt.aggregators")
 class Sum(Aggregator[QuantitativeScale, QuantitativeScale]):
     """This class represents a simple sum aggregator.
 
     :param in_scales: input scales (inferred from input if not provided)
     :param out_scale: output scales (inferred from output if not provided)
     """
 
@@ -257,14 +259,15 @@
 
         :param series:
         :return:
         """
         return series.sum()
 
 
+@set_module("mcda.mavt.aggregators")
 class WeightedSum(Sum):
     """This class represents a weighted sum aggregator.
 
     :param criteria_weights:
     :param in_scales: input scales (inferred from input if not provided)
     :param out_scale: output scales (inferred from output if not provided)
 
@@ -304,14 +307,15 @@
 
         :param series:
         :return:
         """
         return super()._aggregate_series(series * self.criteria_weights)
 
 
+@set_module("mcda.mavt.aggregators")
 class NormalizedWeightedSum(WeightedSum):
     """This class represents a normalized weighted sum aggregator.
 
     :param criteria_weights:
     :param in_scales: input scales (inferred from input if not provided)
     :param out_scale: output scales (inferred from output if not provided)
 
@@ -321,14 +325,15 @@
     def _aggregate_series(self, series: Series, *args, **kwargs) -> float:
         return (
             super()._aggregate_series(series, *args, **kwargs)
             / self.criteria_weights.sum()
         )
 
 
+@set_module("mcda.mavt.aggregators")
 class ChoquetIntegral(Aggregator[QuantitativeScale, QuantitativeScale]):
     """This class represents a Choquet integral aggregator.
 
     :param capacity:
         capacity used for aggregation (either in regular or Möbius
         representation)
     :param in_scales: input scales (inferred from input if not provided)
@@ -393,14 +398,15 @@
         :return:
         """
         if isinstance(self.capacity, Mobius):
             return self._choquet_integral_mobius(series)
         return self._choquet_integral_capacity(series)
 
 
+@set_module("mcda.mavt.aggregators")
 class OWA(Aggregator[QuantitativeScale, QuantitativeScale]):
     """This class represents an Ordered Weighted Aggregator (OWA).
 
     :param weights:
     :param in_scales: input scales (inferred from input if not provided)
     :param out_scale: output scales (inferred from output if not provided)
 
@@ -545,14 +551,15 @@
         :return:
 
         .. note:: :math:`W^*` as defined in :cite:p:`yager1988owa`
         """
         return cls(cast(List[float], [1] + [0] * (size - 1)))
 
 
+@set_module("mcda.mavt.aggregators")
 class ULOWA(Aggregator[FuzzyScale, FuzzyScale]):
     """This class represents an Unbalanced Linguistic Weighted Average (ULOWA)
     aggregator.
 
     :param weights:
     :param scale: fuzzy scale used for the average
 
@@ -640,14 +647,15 @@
         )
         weights[-2] += weights[-1]
         return self._aggregate_series(
             Series(values[:-1]), weights=weights[:-1]
         )
 
 
+@set_module("mcda.functions")
 class AdditiveValueFunctions(CriteriaFunctions[I_S, QuantitativeScale]):
     """This class represents multi-attribute additive value functions.
 
     :param functions: either :class:`CriterionFunction` or functions
     :param in_scales:
         input scales (ignored if :class:`CriterionFunction` supplied)
     :param out_scales:
```

### Comparing `mcda-0.6.1/src/mcda/core/categories.py` & `mcda-0.7.0/src/mcda/internal/core/categories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 from typing import Any, List, Union, cast
 
 from .matrices import PerformanceTable
+from .utils import set_module
 from .values import Values
 
 
+@set_module("mcda.categories")
 class BoundedCategoryProfile:
     """This class represents a category defined by profiles as its limits.
 
     :param lower: lower profile
     :param upper: upper profile
 
     :raise ValueError: if `upper` doesn't dominate `lower`
@@ -70,14 +72,15 @@
             if lowest:
                 res += [cls(lower=values[-1])]
             return res
         except ValueError:
             raise ValueError("any profile must dominate its predecessor")
 
 
+@set_module("mcda.categories")
 class CentralCategoryProfile:
     """This class represents a category defined by a central profile.
 
     :param center:
     """
 
     def __init__(self, center: Values):
```

### Comparing `mcda-0.6.1/src/mcda/core/criteria_functions.py` & `mcda-0.7.0/src/mcda/internal/core/criteria_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from typing import Any, Generic, Mapping, Type, TypeVar, Union, cast, overload
 
 from pandas import DataFrame, Series
 
 from .aliases import Function
 from .matrices import PartialValueMatrix, PerformanceTable
 from .scales import Scale
+from .utils import set_module
 from .values import CommensurableValues, Values
 
 I_S = TypeVar("I_S", bound=Scale, covariant=True)
 O_S = TypeVar("O_S", bound=Scale, covariant=True)
 
 
+@set_module("mcda.functions")
 class CriterionFunction(Generic[I_S, O_S]):
     """This class defines a function and its input/output scale.
 
     :param function:
     :param in_scale: input scale (if not provided, inferred from input)
     :param out_scale: output scale (if not provided, inferred from output)
     :param in_stype: input scale type (if not provided, inferred from input)
@@ -119,14 +121,15 @@
         if isinstance(x, CommensurableValues):
             return self._apply_criterion_values(x)
         if isinstance(x, Series):
             return self._apply_series(x)
         return self.function(x)
 
 
+@set_module("mcda.functions")
 class CriteriaFunctions(Generic[I_S, O_S]):
     """This class represents a multi-attribute scale functions.
 
     :param functions: either :class:`CriterionFunction` or functions
     :param in_scales:
         input scales (ignored if :class:`CriterionFunction` supplied)
     :param out_scales:
```

### Comparing `mcda-0.6.1/src/mcda/core/functions.py` & `mcda-0.7.0/src/mcda/internal/core/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 from typing import Any, Dict, List, Union, cast
 
 from .aliases import NumericFunction
+from .utils import set_module
 
 
+@set_module("mcda.functions")
 class AffineFunction:
     """This class defines a callable affine function.
 
     :param slope:
     :param constant:
     :param segment:
         a list of two points on the affine function line, each point being
@@ -64,14 +66,15 @@
 
         :param x:
         :return: result
         """
         return self.slope * x + self.constant
 
 
+@set_module("mcda.functions")
 class Interval:
     """This class describes a numeric interval.
 
     :param dmin: min boundary of interval
     :param dmax: max boundary of interval
     :param min_in: is min boundary inside interval or not
     :param max_in: is max boundary inside interval or not
@@ -118,37 +121,29 @@
         :return:
         """
         return (
             f"{self.__class__.__name__}(dmin={self.dmin}, dmax={self.dmax},"
             f"min_in={self.min_in}, max_in={self.max_in})"
         )
 
+    @property
     def is_empty(self) -> bool:
         """Check if interval is empty.
 
         :return: ``True`` if interval is empty, ``False`` otherwise.
         """
         return self.dmin == self.dmax and (not self.min_in or not self.max_in)
 
     def __contains__(self, x: float) -> bool:
         """Check whether value is inside interval or not.
 
         :param x:
         :return:
         """
-        return self.inside(x)
-
-    def inside(self, x: float) -> bool:
-        """Check whether value is inside interval or not.
-
-        :param x:
-        :return:
-        :rtype: bool
-        """
-        if self.is_empty():
+        if self.is_empty:
             return False
         if self.dmin < x < self.dmax:
             return True
         if self.min_in and x == self.dmin:
             return True
         if self.max_in and x == self.dmax:
             return True
@@ -217,15 +212,15 @@
         """Compute union of two intervals.
 
         :param other:
         :return:
 
         .. note :: Returns ``None`` if intervals don't coïncide
         """
-        if self.intersect(other).is_empty():
+        if self.intersect(other).is_empty:
             return Interval(0, 0, False, False)
         return self.join(other)
 
     def continuous(self, other: "Interval") -> bool:
         """Check continuity with following interval.
 
         :param other:
@@ -250,53 +245,46 @@
             self.dmin == other.dmin
             and self.dmax == other.dmax
             and self.min_in == other.min_in
             and self.max_in == other.max_in
         )
 
 
+@set_module("mcda.functions")
 class DiscreteFunction:
     """This class implements discrete function.
 
     :param values: function description, abscissa as keys, ordinates as values
     """
 
     def __init__(self, values: Dict[Any, Any]):
         """Constructor method"""
         self.values = {}
         self.values.update(values)
 
-    def apply(self, x: Any) -> Any:
-        """Apply function to single value.
-
-        :param x:
-        :return:
-        :raises IndexError: if `x` is not in `values`
-        """
-        if x not in self.values:
-            raise IndexError(f"discrete value '{x}' unknown")
-        return self.values[x]
-
     def __repr__(self) -> str:  # pragma: nocover
         """Return string representation of function.
 
         :return:
         """
         return f"{self.__class__.__name__}(values={self.values})"
 
     def __call__(self, x: Any) -> Any:
         """Apply function to single value.
 
         :param x:
         :return:
         :raises IndexError: if `x` is not in `values`
         """
-        return self.apply(x)
+        if x not in self.values:
+            raise IndexError(f"discrete value '{x}' unknown")
+        return self.values[x]
 
 
+@set_module("mcda.functions")
 class PieceWiseFunction:
     """This class implements piecewise MCDA function.
 
     :param functions:
     :param segments: list of segments defining piecewise linear functions
 
     .. note::
@@ -351,14 +339,15 @@
         for seg in segments:
             a = seg[0] if len(seg[0]) > 2 else seg[0] + [True]
             b = seg[1] if len(seg[1]) > 2 else seg[1] + [True]
             self.functions[Interval(a[0], b[0], a[2], b[2])] = AffineFunction(
                 segment=seg
             )
 
+    @property
     def continuous(self) -> bool:
         """Check intervals and functions are ordered and continuous.
 
         :return:
         """
         if len(self.intervals) <= 1:
             return True
@@ -370,15 +359,15 @@
             if not math.isclose(
                 self.functions[interval](interval.dmax),
                 self.functions[successor](successor.dmin),
             ):
                 return False
         return True
 
-    def apply(self, x: float) -> float:
+    def _apply(self, x: float) -> float:
         """Apply function to single value.
 
         :param x:
         :raises ValueError: if `x` is not inside an interval
         :return:
         """
         for interval, f in self.functions.items():
@@ -391,17 +380,18 @@
     def __call__(self, x: float) -> float:
         """Apply function to single value.
 
         :param x:
         :raises ValueError: if `x` is not inside an interval
         :return:
         """
-        return self.apply(x)
+        return self._apply(x)
 
 
+@set_module("mcda.functions")
 class FuzzyNumber(PieceWiseFunction):
     """This class implements a trapezoidal fuzzy number.
 
     A fuzzy number is described by its 4 abscissa in increasing order.
     Its ordinates are fixed at ``[0, 1, 1, 0]``.
 
     Triangular fuzzy number can be represented by having two consecutive
@@ -464,24 +454,24 @@
     def __repr__(self) -> str:  # pragma: nocover
         """Return string representation of fuzzy number.
 
         :return:
         """
         return f"{self.__class__.__name__}(abscissa={self.abscissa})"
 
-    def apply(self, x: float) -> float:
+    def _apply(self, x: float) -> float:
         """Apply function to single value.
 
         :param x:
         :return:
 
         .. note:: returns ``0`` if value is not in the fuzzy set
         """
         try:
-            return super().apply(x)
+            return super()._apply(x)
         except ValueError:
             return 0
 
     @property
     def average(self) -> float:
         """Computes the average of all intervals boundaries.
```

### Comparing `mcda-0.6.1/src/mcda/core/interfaces.py` & `mcda-0.7.0/src/mcda/internal/core/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         """Select a subset of alternatives.
 
         :return: selected alternatives
         """
         pass
 
 
-class Clusterizor(ABC):
-    """Interface to implement clustering MCDA algorithms."""
+class Sorter(ABC):
+    """Interface to implement clustering/sorting MCDA algorithms."""
 
     @abstractmethod
     def clusterize(self, **kwargs) -> CommensurableValues:  # pragma: nocover
         """Clusterize alternatives.
 
         :return: cluster of each alternative
         """
```

### Comparing `mcda-0.6.1/src/mcda/core/matrices.py` & `mcda-0.7.0/src/mcda/internal/core/matrices.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,85 @@
 """This module contains all functions related to matrices.
 """
 from __future__ import annotations
 
+import functools
 import sys
 from abc import ABC, abstractmethod
 from itertools import product
 from typing import (
     Any,
     Generic,
+    Iterator,
     List,
     Literal,
     Mapping,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-from graphviz import Digraph
 from pandas import DataFrame, Series, concat
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import connected_components, floyd_warshall
 
 from .scales import (
     BinaryScale,
+    DiscreteQuantitativeScale,
     OrdinalScale,
     QuantitativeScale,
     Scale,
     common_scale_type,
 )
+from .utils import set_module
 from .values import CommensurableValues, Values
 
 if sys.version_info >= (3, 11):  # pragma: nocover
     from typing import Self
 else:
     from typing_extensions import Self
 
 
+try:
+    from graphviz import Digraph
+
+    _has_graphviz = True
+except ImportError:  # pragma: nocover
+    import warnings
+
+    warnings.warn(
+        "Graph plotting features not available. "
+        "If you need those, please install 'graphviz' or this package "
+        "optional plotting dependencies 'mcda[plot]'."
+    )
+    _has_graphviz = False
+
+
+def requires_graphviz(func):
+    """Wrap a class or function that requires graphviz to function.
+
+    :param obj: either a class or function
+    :raises ImportError: if graphviz is not installed
+    :return: wrapped class or function
+    """
+
+    @functools.wraps(func)
+    def wrapped(*args, **kwargs):
+        if not _has_graphviz:  # pragma: nocover
+            raise ImportError("This function requires 'graphviz'")
+        return func(*args, **kwargs)
+
+    return wrapped
+
+
 def dataframe_equals(df1: DataFrame, df2: DataFrame) -> bool:
     """Check if two dataframes have the same values.
 
     It will realign the indexes and columns if they are ordered differently.
 
     :param df1:
     :param df2:
@@ -116,118 +151,141 @@
 
     The adjacency matrix is represented internally by a
     :class:`pandas.DataFrame` with vertices as the indexes and columns.
 
     :param data: adjacency matrix in an array-like or dict-structure
     :param vertices:
 
-    :raise ValueError: if columns and rows have different sets of labels
     :raise KeyError:
-        * if some indexes are duplicated
-        * if some columns are duplicated
+        * if columns and rows have different sets of labels
+        * if some vertices are duplicated
 
     .. note:: the cells of the matrix can be of any type (not just numerics)
     """
 
     def __init__(self, data, vertices: Union[List, None] = None, **kwargs):
         df = DataFrame(
             data.values if isinstance(data, DataFrame) and vertices else data,
             index=vertices,
             columns=vertices,
         )
         if df.columns.tolist() != df.index.tolist():
-            raise ValueError(
+            raise KeyError(
                 f"{self.__class__} supports only same labelled"
                 "index and columns"
             )
         super().__init__(df, **kwargs)
 
     @property
     def vertices(self) -> List:
         """Return list of vertices"""
         return self.rows
 
-    def to_graph(
-        self,
-        edge_label: bool = False,
-        self_loop: bool = False,
-    ) -> Digraph:
-        """Create a graph for adjacency matrix.
 
-        This function creates a Graph using graphviz.
+S = TypeVar("S", bound=Scale, covariant=True)
 
-        :param edge_label: (optional) parameter to display the value of edges
-        :param self_loop: (optional) parameter to display self looping edges
-        :return: graph
-        """
-        graph = Digraph("graph", strict=True)
-        graph.attr("node", shape="box")
 
-        for v in self.vertices:
-            graph.node(str(v))
-        for a in self.data.index:
-            for b in self.data.columns:
-                if not self_loop and a == b:
-                    continue
-                elif self.data.at[a, b] == 0:
-                    continue
+class RowView(Mapping[Any, Values[S]], Generic[S]):
+    """This class defines a view of a value matrix per row.
 
-                graph.edge(
-                    str(a),
-                    str(b),
-                    label=str(self.data.at[a, b]) if edge_label else None,
-                )
-        return graph
+    :param matrix:
+    """
 
-    def plot(
-        self,
-        edge_label: bool = False,
-        self_loop: bool = False,
-    ) -> Digraph:  # pragma: nocover
-        """Plot adjacency matrix as a graph.
+    def __init__(self, matrix: IValueMatrix[S]):
+        self._matrix = matrix
 
-        :param edge_label: (optional) parameter to display the value of edges
-        :param self_loop: (optional) parameter to display self looping edges
-        :return: graph
+    @property
+    def _data(self) -> DataFrame:
+        """Dataframe of the value matrix"""
+        return self._matrix.data
 
-        .. note::
-            You need an environment that will actually display the graph (such
-            as a jupyter notebook), otherwise the function only returns the
-            graph.
-        """
-        return self.to_graph(edge_label=edge_label, self_loop=self_loop)
+    @property
+    def _scales(self) -> Mapping[Any, S]:
+        """Scales of the value matrix"""
+        return self._matrix.scales
 
-    def save_plot(
-        self,
-        edge_label: bool = False,
-        self_loop: bool = False,
-    ) -> str:  # pragma: nocover
-        """Plot adjacency matrix as a graph and save it.
+    @property
+    def _stype(self) -> Type[S]:
+        """Scale type of the value matrix"""
+        return self._matrix.stype
 
-        :param edge_label: (optional) parameter to display the value of edges
-        :param self_loop: (optional) parameter to display self looping edges
-        :return: file name where plot is saved
+    def __len__(self) -> int:
+        """Number of rows in the value matrix"""
+        return len(self._matrix.rows)
+
+    def __getitem__(self, key: Any) -> Values[S]:
+        """Return values at row.
+
+        :param key: row index
+        :raises KeyError: if `key` row doesn't exist
+        :return:
         """
-        return self.plot(edge_label=edge_label, self_loop=self_loop).render()
+        return Values[S](self._data.loc[key], self._scales, self._stype)
 
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the rows"""
+        return iter(self._matrix.rows)
 
-S = TypeVar("S", bound=Scale, covariant=True)
+
+class ColumnView(Mapping[Any, CommensurableValues[S]], Generic[S]):
+    """This class defines a view of a value matrix per column.
+
+    :param matrix:
+    """
+
+    def __init__(self, matrix: IValueMatrix[S]):
+        self._matrix = matrix
+
+    @property
+    def _data(self) -> DataFrame:
+        """Dataframe of the value matrix"""
+        return self._matrix.data
+
+    @property
+    def _scales(self) -> Mapping[Any, S]:
+        """Scales of the value matrix"""
+        return self._matrix.scales
+
+    @property
+    def _stype(self) -> Type[S]:
+        """Scale type of the value matrix"""
+        return self._matrix.stype
+
+    def __len__(self) -> int:
+        """Number of columns in the value matrix"""
+        return len(self._matrix.columns)
+
+    def __getitem__(self, key: Any) -> CommensurableValues[S]:
+        """Return values at column.
+
+        :param key: column index
+        :raises KeyError: if `key` column doesn't exist
+        :return:
+        """
+        return CommensurableValues[S](
+            self._data[key], self._scales[key], self._stype
+        )
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the columns"""
+        return iter(self._matrix.columns)
 
 
 class IValueMatrix(IMatrix, Generic[S], ABC):
     """This class defines a matrix with associated scales (one per column).
 
     :param data:
     :param scales:
         data scale(s) (one per column or one shared, will be inferred from data
         if absent using :meth:`Scale.fit`)
     :param stype: scales type used
     :raise KeyError:
         * if some indexes are duplicated
         * if some columns are duplicated
+    :raise TypeError: if `stype` and `scales` types mismatch
 
     .. todo:: remove this class completely, put its code in current subclasses
     """
 
     def __init__(
         self,
         data,
@@ -270,28 +328,20 @@
         return Values[S](
             Series(self.data.values.flatten().tolist()), stype=self.stype
         ).bounds
 
     @property
     def rows_values(self) -> Mapping[Any, Values[S]]:
         """Iterator on the table alternatives values"""
-        return {
-            a: Values[S](self.data.loc[a], self.scales, self.stype)
-            for a in self.rows
-        }
+        return RowView[S](self)
 
     @property
     def columns_values(self) -> Mapping[Any, CommensurableValues[S]]:
         """Iterator on the table criteria values"""
-        return {
-            c: CommensurableValues[S](
-                self.data[c], self.scales.get(c), self.stype
-            )
-            for c in self.columns
-        }
+        return ColumnView[S](self)
 
     @property
     @abstractmethod
     def to_numeric(self) -> IValueMatrix[QuantitativeScale]:  # pragma: nocover
         """Return numeric conversion of ordinal values.
 
         :raise TypeError: if :attr:`scales` are not ordinal
@@ -381,27 +431,29 @@
     def copy(self) -> Self:
         """Return a copy of the object"""
         return self.__class__(
             self.data.copy(), scales=dict(self.scales), stype=self.stype
         )
 
 
+@set_module("mcda")
 class PerformanceTable(IValueMatrix[S], Generic[S]):
     """This class defines a performance table.
 
     :param data:
     :param scales:
         data scale(s) (one per column or one shared, will be inferred from data
         if absent using :meth:`Scale.fit`)
     :param alternatives: if not set, inferred from `data`
     :param criteria:  if not set, inferred from `data`
     :param stype: scales type used
     :raise KeyError:
         * if some indexes are duplicated
         * if some columns are duplicated
+    :raise TypeError: if `stype` and `scales` types mismatch
     """
 
     def __init__(
         self,
         data,
         scales: Union[S, Mapping[Any, S], None] = None,
         alternatives: Union[List, None] = None,
@@ -541,26 +593,175 @@
             dataframes.append(t.data)
             for c, s in t.scales.items():
                 scales.setdefault(c, s)
         df = concat(dataframes, axis=axis)
         return cls(df, scales=scales)
 
 
+class PartialRowView(Mapping[Any, PerformanceTable[S]], Generic[S]):
+    """This class defines a view of a partial value matrix per row.
+
+    :param matrix:
+    """
+
+    def __init__(self, matrix: PartialValueMatrix[S]):
+        self._matrix = matrix
+
+    @property
+    def _data(self) -> DataFrame:
+        """Dataframe of the partial value matrix"""
+        return self._matrix.data
+
+    @property
+    def _scales(self) -> Mapping[Any, S]:
+        """Scales of the partial value matrix"""
+        return self._matrix.scales
+
+    @property
+    def _stype(self) -> Type[S]:
+        """Scale type of the partial value matrix"""
+        return self._matrix.stype
+
+    def __len__(self) -> int:
+        """Number of vertices in the partial value matrix"""
+        return len(self._matrix.vertices)
+
+    def __getitem__(self, key: Any) -> PerformanceTable[S]:
+        """Return values at row.
+
+        :param key: vertex
+        :raises KeyError: if `key` vertex doesn't exist
+        :return:
+        """
+        return PerformanceTable(
+            DataFrame(
+                [s.tolist() for s in self._data.loc[key].tolist()],
+                index=self._matrix.vertices,
+                columns=self._matrix.criteria,
+            ),
+            self._scales,
+            stype=self._stype,
+        )
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the vertices"""
+        return iter(self._matrix.vertices)
+
+
+class PartialColumnView(Mapping[Any, PerformanceTable[S]], Generic[S]):
+    """This class defines a view of a partial value matrix per column.
+
+    :param matrix:
+    """
+
+    def __init__(self, matrix: PartialValueMatrix[S]):
+        self._matrix = matrix
+
+    @property
+    def _data(self) -> DataFrame:
+        """Dataframe of the partial value matrix"""
+        return self._matrix.data
+
+    @property
+    def _scales(self) -> Mapping[Any, S]:
+        """Scales of the partial value matrix"""
+        return self._matrix.scales
+
+    @property
+    def _stype(self) -> Type[S]:
+        """Scale type of the partial value matrix"""
+        return self._matrix.stype
+
+    def __len__(self) -> int:
+        """Number of vertices in the partial value matrix"""
+        return len(self._matrix.vertices)
+
+    def __getitem__(self, key: Any) -> PerformanceTable[S]:
+        """Return values at column.
+
+        :param key: vertex
+        :raises KeyError: if `key` vertex doesn't exist
+        :return:
+        """
+        return PerformanceTable(
+            DataFrame(
+                [s.tolist() for s in self._data[key].tolist()],
+                index=self._matrix.vertices,
+                columns=self._matrix.criteria,
+            ),
+            self._scales,
+            stype=self._stype,
+        )
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the vertices"""
+        return iter(self._matrix.vertices)
+
+
+class PartialCriterionView(
+    Mapping[Any, "AdjacencyValueMatrix[S]"], Generic[S]
+):
+    """This class defines a view of a partial value matrix per criterion.
+
+    :param matrix:
+    """
+
+    def __init__(self, matrix: PartialValueMatrix[S]):
+        self._matrix = matrix
+
+    @property
+    def _data(self) -> DataFrame:
+        """Dataframe of the partial value matrix"""
+        return self._matrix.data
+
+    @property
+    def _scales(self) -> Mapping[Any, S]:
+        """Scales of the partial value matrix"""
+        return self._matrix.scales
+
+    @property
+    def _stype(self) -> Type[S]:
+        """Scale type of the partial value matrix"""
+        return self._matrix.stype
+
+    def __len__(self) -> int:
+        """Number of criteria in the partial value matrix"""
+        return len(self._matrix.criteria)
+
+    def __getitem__(self, key: Any) -> AdjacencyValueMatrix[S]:
+        """Return values at criterion.
+
+        :param key: criterion
+        :raises KeyError: if `key` criterion doesn't exist
+        :return:
+        """
+        return AdjacencyValueMatrix(
+            self._data.applymap(lambda s: s[key]),
+            scale=self._scales[key],
+            stype=self._stype,
+        )
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the criteria"""
+        return iter(self._matrix.criteria)
+
+
+@set_module("mcda.matrices")
 class PartialValueMatrix(IAdjacencyMatrix, Generic[S]):
     """This class describes a matrix of partial values.
 
     :param data:
     :param vertices: labels used to identify both rows and columns
     :param criteria: labels used for the values in each cell
     :param scales:
     :param stype: scales type used
     :raise KeyError:
-        * if some indexes are duplicated
-        * if some columns are duplicated
-        * if matrix cells don't share the same labels
+        * if columns and rows have different sets of labels
+        * if some vertices are duplicated
+    :raise TypeError: if `stype` and `scale` type mismatch
     """
 
     def __init__(
         self,
         data,
         vertices: Union[List, None] = None,
         criteria: Union[List, None] = None,
@@ -571,14 +772,16 @@
         super().__init__(data, vertices, **kwargs)
         if criteria is None:
             criteria = (
                 cast(Series, self.data.iloc[0, 0]).index.tolist()
                 if isinstance(self.data.iloc[0, 0], Series)
                 else list(range(len(self.data.iloc[0, 0])))
             )
+        if len(set(criteria)) != len(criteria):
+            raise KeyError("criteria must be uniques")
         self.data = self.data.applymap(
             lambda s: Series(list(s), index=criteria)
         )
         self.scales: Mapping[Any, S] = {}
         _stype = cast(Type[S], Scale if stype is None else stype)
         for c in criteria:
             if isinstance(scales, Mapping) and c in scales:
@@ -611,52 +814,25 @@
         :return: inferred scales
         """
         return {c: m.union_bounds for c, m in self.criteria_matrices.items()}
 
     @property
     def row_matrices(self) -> Mapping[Any, PerformanceTable[S]]:
         """Iterator on the table rows."""
-        return {
-            a: PerformanceTable(
-                DataFrame(
-                    [s.tolist() for s in self.data.loc[a].tolist()],
-                    index=self.vertices,
-                    columns=self.criteria,
-                ),
-                self.scales,
-                stype=self.stype,
-            )
-            for a in self.vertices
-        }
+        return PartialRowView[S](self)
 
     @property
     def column_matrices(self) -> Mapping[Any, PerformanceTable[S]]:
         """Iterator on the table columns."""
-        return {
-            a: PerformanceTable(
-                DataFrame(
-                    [s.tolist() for s in self.data[a].tolist()],
-                    index=self.vertices,
-                    columns=self.criteria,
-                ),
-                self.scales,
-                stype=self.stype,
-            )
-            for a in self.vertices
-        }
+        return PartialColumnView[S](self)
 
     @property
     def criteria_matrices(self) -> Mapping[Any, AdjacencyValueMatrix[S]]:
         """Iterator on the table criteria."""
-        return {
-            c: AdjacencyValueMatrix(
-                self.data.applymap(lambda s: s[c]), scale=s, stype=self.stype
-            )
-            for c, s in self.scales.items()
-        }
+        return PartialCriterionView[S](self)
 
     @property
     def cell(self) -> Mapping[Tuple[Any, Any], Values[S]]:
         """Return matrix cell accessor"""
         return {
             (r, c): Values(
                 self.data.at[r, c], scales=self.scales, stype=self.stype
@@ -762,14 +938,15 @@
             scales={
                 criterion: self.scales[criterion] for criterion in criteria
             },
             stype=self.stype,
         )
 
 
+@set_module("mcda.matrices")
 class AdditivePerformanceTable(PerformanceTable[QuantitativeScale]):
     """This class defines a performance table with additive values.
 
     :param data:
     :param scales:
         data scale(s) (one per column or one shared, will be inferred from data
         if absent using :meth:`Scale.fit`)
@@ -777,14 +954,19 @@
         output scale of row-wise aggregation (inferred if not provided)
     :param alternatives: if not set, inferred from `data`
     :param criteria:  if not set, inferred from `data`
     :param stype: scales type used
     :raise KeyError:
         * if some indexes are duplicated
         * if some columns are duplicated
+    :raise TypeError: if `stype` and `scales` types mismatch
+
+    .. note::
+        This class is not intended for general use, it can though be the output
+        of some algorithms.
     """
 
     def __init__(
         self,
         data,
         scales: Union[
             QuantitativeScale, Mapping[Any, QuantitativeScale], None
@@ -839,29 +1021,108 @@
                 self.data.sum(axis=axis),
                 scale=self.aggregated_scale,
                 stype=QuantitativeScale,
             )
         return super().sum(axis=axis)
 
 
+class VertexRowView(Mapping[Any, CommensurableValues[S]], Generic[S]):
+    """This class defines a view of an adjacency value matrix per row.
+
+    :param matrix:
+    """
+
+    def __init__(self, matrix: AdjacencyValueMatrix[S]):
+        self._matrix: AdjacencyValueMatrix[S] = matrix
+
+    @property
+    def _data(self) -> DataFrame:
+        """Dataframe of the value matrix"""
+        return self._matrix.data
+
+    @property
+    def _stype(self) -> Type[S]:
+        """Scale type of the value matrix"""
+        return self._matrix.stype
+
+    @property
+    def _scale(self) -> S:
+        """Scales of the adjacency value matrix"""
+        return self._matrix.scale
+
+    def __len__(self) -> int:
+        """Number of vertices in the adjacency value matrix"""
+        return len(self._matrix.vertices)
+
+    def __getitem__(self, key: Any) -> CommensurableValues[S]:
+        """Return values at row.
+
+        :param key: vertex
+        :raises KeyError: if `key` vertex doesn't exist
+        :return:
+        """
+        return CommensurableValues[S](
+            self._data.loc[key], self._scale, self._stype
+        )
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the vertices"""
+        return iter(self._matrix.vertices)
+
+
+class VertexColumnView(ColumnView[S], Generic[S]):
+    """This class defines a view of an adjacency value matrix per column.
+
+    :param matrix:
+    """
+
+    def __init__(self, matrix: AdjacencyValueMatrix[S]):
+        self._matrix: AdjacencyValueMatrix[S] = matrix
+
+    @property
+    def _scale(self) -> S:
+        """Scale of the adjacency value matrix"""
+        return self._matrix.scale
+
+    def __len__(self) -> int:
+        """Number of vertices in the adjacency value matrix"""
+        return len(self._matrix.vertices)
+
+    def __getitem__(self, key: Any) -> CommensurableValues[S]:
+        """Return values at column.
+
+        :param key: vertex
+        :raises KeyError: if `key` vertex doesn't exist
+        :return:
+        """
+        return CommensurableValues[S](
+            self._data[key], self._scale, self._stype
+        )
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate on the vertices"""
+        return iter(self._matrix.vertices)
+
+
+@set_module("mcda.matrices")
 class AdjacencyValueMatrix(IAdjacencyMatrix, IValueMatrix[S], Generic[S]):
     """This class implements graphs as an adjacency value matrix.
 
     The adjacency matrix is represented internally by a
     :class:`pandas.DataFrame` with vertices as the indexes and columns.
 
     :param data: adjacency matrix in an array-like or dict-structure
     :param vertices:
     :param scale:
     :param stype: scales type used
 
-    :raise ValueError: if columns and rows have different sets of labels
     :raise KeyError:
-        * if some indexes are duplicated
-        * if some columns are duplicated
+        * if columns and rows have different sets of labels
+        * if some vertices are duplicated
+    :raise TypeError: if `stype` and `scale` type mismatch
 
     .. note:: the cells of the matrix can be of any type (not just numerics)
     """
 
     def __init__(
         self,
         data,
@@ -875,18 +1136,20 @@
         )
         self.scale = self.union_bounds if scale is None else scale
         self.scales = {c: self.scale for c in self.vertices}
 
     @property
     def rows_values(self) -> Mapping[Any, CommensurableValues[S]]:
         """Iterator on the table alternatives values"""
-        return {
-            a: CommensurableValues[S](self.data.loc[a], self.scale, self.stype)
-            for a in self.rows
-        }
+        return VertexRowView[S](self)
+
+    @property
+    def columns_values(self) -> Mapping[Any, CommensurableValues[S]]:
+        """Iterator on the table alternatives values"""
+        return VertexColumnView[S](self)
 
     @property
     def to_numeric(self) -> AdjacencyValueMatrix[QuantitativeScale]:
         """Return numeric conversion of ordinal values.
 
         :raise TypeError: if :attr:`scales` are not ordinal
         """
@@ -906,17 +1169,15 @@
 
     @property
     def is_binary(self) -> bool:
         """Check whether adjacency value matrix is binary.
 
         :return:
         """
-        return (
-            issubclass(self.stype, BinaryScale) or self.scale == BinaryScale()
-        )
+        return self.scale == DiscreteQuantitativeScale.binary()
 
     @property
     def transitive_closure(self) -> OutrankingMatrix:
         """Return transitive closure of matrix.
 
         :return:
         :raise TypeError: if matrix is not binary
@@ -1142,14 +1403,80 @@
 
     def copy(self) -> Self:
         """Return a copy of the object"""
         return self.__class__(
             self.data.copy(), scale=self.scale, stype=self.stype
         )
 
+    @requires_graphviz
+    def to_graph(
+        self,
+        edge_label: bool = False,
+        self_loop: bool = False,
+    ) -> Digraph:
+        """Create a graph for adjacency matrix.
+
+        This function creates a Graph using graphviz.
+
+        :param edge_label: (optional) parameter to display the value of edges
+        :param self_loop: (optional) parameter to display self looping edges
+        :return: graph
+        """
+        graph = Digraph("graph", strict=True)
+        graph.attr("node", shape="box")
+
+        for v in self.vertices:
+            graph.node(str(v))
+        for a in self.data.index:
+            for b in self.data.columns:
+                if not self_loop and a == b:
+                    continue
+                elif self.data.at[a, b] == 0:
+                    continue
+
+                graph.edge(
+                    str(a),
+                    str(b),
+                    label=str(self.data.at[a, b]) if edge_label else None,
+                )
+        return graph
+
+    @requires_graphviz
+    def plot(
+        self,
+        edge_label: bool = False,
+        self_loop: bool = False,
+    ) -> Digraph:  # pragma: nocover
+        """Plot adjacency matrix as a graph.
+
+        :param edge_label: (optional) parameter to display the value of edges
+        :param self_loop: (optional) parameter to display self looping edges
+        :return: graph
+
+        .. note::
+            You need an environment that will actually display the graph (such
+            as a jupyter notebook), otherwise the function only returns the
+            graph.
+        """
+        return self.to_graph(edge_label=edge_label, self_loop=self_loop)
+
+    @requires_graphviz
+    def save_plot(
+        self,
+        edge_label: bool = False,
+        self_loop: bool = False,
+    ) -> str:  # pragma: nocover
+        """Plot adjacency matrix as a graph and save it.
+
+        :param edge_label: (optional) parameter to display the value of edges
+        :param self_loop: (optional) parameter to display self looping edges
+        :return: file name where plot is saved
+        """
+        return self.plot(edge_label=edge_label, self_loop=self_loop).render()
+
     @classmethod
     def from_ordered_alternatives_groups(
         cls,
         categories: List[List],
     ) -> OutrankingMatrix:
         """Convert a ranking of categories of alternatives into an outranking
         matrix.
@@ -1177,25 +1504,26 @@
     data, vertices: Union[List, None] = None, **kwargs
 ) -> OutrankingMatrix:
     """Create an outranking matrix.
 
     :param data: adjacency matrix in an array-like or dict-structure
     :param vertices:
 
-    :raise ValueError:
-        * if non-binary values are in the matrix
-        * if columns and rows have different sets of labels
     :raise KeyError:
-        * if some indexes are duplicated
-        * if some columns are duplicated
+        * if columns and rows have different sets of labels
+        * if some vertices are duplicated
+    :raise TypeError: if `data` is not binary
 
     .. note::
         This function is just an easier way to create
         :class:`AdjacencyValueMatrix` with binary scale
     """
     kwargs.pop("stype", None)
-    return OutrankingMatrix(
+    m = AdjacencyValueMatrix(
         data,
         vertices=vertices,
-        stype=BinaryScale,
+        scale=DiscreteQuantitativeScale.binary(),
         **kwargs,
     )
+    if not m.is_within_scales:
+        raise TypeError("outranking matrix data must be binary")
+    return m
```

### Comparing `mcda-0.6.1/src/mcda/core/relations.py` & `mcda-0.7.0/src/mcda/internal/core/relations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 from __future__ import annotations
 
 import sys
 from abc import ABC
-from typing import Any, Dict, Iterator, List, Tuple, Union, cast
+from typing import Any, Dict, Iterator, List, Mapping, Tuple, Type, Union
 
-from graphviz import Digraph
 from numpy import fill_diagonal
 from pandas import DataFrame, Series
 
-from .matrices import OutrankingMatrix, create_outranking_matrix
+from .matrices import (
+    OutrankingMatrix,
+    create_outranking_matrix,
+    requires_graphviz,
+)
 from .scales import PreferenceDirection, QuantitativeScale
-from .values import Ranking
+from .utils import set_module
+from .values import CommensurableValues, Ranking
 
 if sys.version_info >= (3, 11):  # pragma: nocover
     from typing import Self
 else:
     from typing_extensions import Self
 
 
+try:
+    from graphviz import Digraph
+except ImportError:  # pragma: nocover
+    import warnings
+
+    warnings.warn(
+        "Graph plotting features not available. "
+        "If you need those, please install 'graphviz' or this package "
+        "optional plotting dependencies 'mcda[plot]'."
+    )
+
+
+@set_module("mcda.types")
 class Relation(ABC):
     """This class represents a pairwise relation between two elements.
 
     :param a: first element
     :param b: second element
 
     :attribute a:
@@ -31,15 +48,15 @@
 
     _RELATION_TYPE = ""
     DRAW_STYLE: Dict[str, Any] = {"style": "invis"}
 
     def __init__(self, a: Any, b: Any):
         self.a = a
         self.b = b
-        self.validate()
+        self._validate()
 
     def __str__(self) -> str:
         """Return string representation of object.
 
         :return:
         """
         return f"{self.a} {self._RELATION_TYPE} {self.b}"
@@ -52,15 +69,15 @@
         return f"{self.__class__.__name__}({self.a}, {self.b})"
 
     @property
     def elements(self) -> Tuple[Any, Any]:
         """Return elements of the relation"""
         return self.a, self.b
 
-    def validate(self):
+    def _validate(self):
         """Check whether a relation is valid or not."""
         pass
 
     def same_elements(self, relation: Relation) -> bool:
         """Check whether the relations are about the same pair of alternatives.
 
         :param relation: second relation
@@ -106,56 +123,60 @@
         :param other:
         :return: check result
 
         .. warning:: Does not check for relations' validity!
         """
         return self == other or not self.same_elements(other)
 
-    @classmethod
-    def types(cls) -> List:
+    @staticmethod
+    def types() -> List:
         """Return list of relation types.
 
         :return:
         """
-        return cls.__subclasses__()
+        return Relation.__subclasses__()
 
+    @requires_graphviz
     def _draw(self, graph: Digraph):
         """Draw relation on provided graph"""
         graph.edge(str(self.a), str(self.b), **self.DRAW_STYLE)
 
 
+@set_module("mcda.relations")
 class PreferenceRelation(Relation):
     """This class represents a preference relation between two elements.
 
     A relation is read `aPb`.
 
     :param a: first element
     :param b: second element
+    :raise ValueError: if relation is reflexive
 
     :attribute a:
     :attribute b:
     :attribute DRAW_STYLE: (class) key args for plotting all instances
 
     .. note:: this relation is antisymmetric and irreflexive
     """
 
     _RELATION_TYPE = "P"
     DRAW_STYLE: Dict[str, Any] = {}
 
-    def validate(self):
+    def _validate(self):
         """Check whether a relation is valid or not.
 
         :raise ValueError: if relation is reflexive
         """
         if self.a == self.b:
             raise ValueError(
                 f"Preference relations are irreflexive: {self.a} == {self.b}"
             )
 
 
+@set_module("mcda.relations")
 class IndifferenceRelation(Relation):
     """This class represents an indifference relation between two elements.
 
     A relation is read `aIb`.
 
     :param a: first element
     :param b: second element
@@ -181,21 +202,23 @@
         .. warning:: Does not check for relations' validity!
         """
         if type(other) == type(self):
             return self.same_elements(other)
         return False
 
 
+@set_module("mcda.relations")
 class IncomparableRelation(Relation):
     """This class represents an incomparable relation between two elements.
 
     A relation is read `aRb`.
 
     :param a: first element
     :param b: second element
+    :raise ValueError: if relation is reflexive
 
     :attribute a:
     :attribute b:
     :attribute DRAW_STYLE: (class) key args for plotting all instances
 
     .. note:: this relation is symmetric and irreflexive
     """
@@ -213,101 +236,226 @@
 
         .. warning:: Does not check for relations' validity!
         """
         if type(other) == type(self):
             return self.same_elements(other)
         return False
 
-    def validate(self):
+    def _validate(self):
         """Check whether a relation is valid or not.
 
         :raise ValueError: if relation is reflexive
         """
         if self.a == self.b:
             raise ValueError(
                 f"Incomparable relations are irreflexive: {self.a} == {self.b}"
             )
 
 
-P = PreferenceRelation
-"""Type alias for user-friendly definition of :class:`PreferenceRelation`"""
+class RelationTypeView(Mapping[Type[Relation], "PreferenceStructure"]):
+    """This class is a view of a :class:`PreferenceStructure` per type of
+    relation.
+
+    :param obj: preference structure
+    """
+
+    def __init__(self, obj: PreferenceStructure):
+        self._preference_structure = obj
+
+    def __len__(self) -> int:
+        """Number of relation types"""
+        return len(Relation.types())
+
+    def __getitem__(self, key: Type[Relation]) -> PreferenceStructure:
+        """Return preference structure with selected relation type.
+
+        :param key: type of relation
+        :return:
+        """
+        res = PreferenceStructure()
+        for r in self._preference_structure.relations:
+            if isinstance(r, key):
+                res += r
+        return res
+
+    def __iter__(self) -> Iterator[Type[Relation]]:
+        """Iterate on the relation types"""
+        return iter(Relation.types())
+
+
+class ElementView(Mapping[Any, "PreferenceStructure"]):
+    """This class is a view of a :class:`PreferenceStructure` per element.
+
+    :param obj: preference structure
+    """
+
+    def __init__(self, obj: PreferenceStructure):
+        self._preference_structure = obj
+
+    def __len__(self) -> int:
+        """Number of elements"""
+        return len(self._preference_structure.elements)
+
+    def __getitem__(self, key: Any) -> PreferenceStructure:
+        """Return preference structure pertaining to one element.
+
+        :param key: element
+        :return:
+        """
+        relations: List[Relation] = []
+        for r in self._preference_structure.relations:
+            if key in r.elements:
+                relations.append(r)
+        return PreferenceStructure(relations)
+
+    def __iter__(self) -> Iterator:
+        """Iterate on the elements"""
+        return iter(self._preference_structure.elements)
 
 
-I = IndifferenceRelation  # noqa: E741
-"""Type alias for user-friendly definition of :class:`IndifferenceRelation`"""
+class ElementsPairView(Mapping[Tuple[Any, Any], Union[Relation, None]]):
+    """This class is a view of a :class:`PreferenceStructure` per pair of
+    elements.
 
+    :param obj: preference structure
+    """
 
-R = IncomparableRelation
-"""Type alias for user-friendly definition of :class:`IncomparableRelation`"""
+    def __init__(self, obj: PreferenceStructure):
+        self._preference_structure = obj
+
+    def __len__(self) -> int:
+        """Number of relations"""
+        return len(self._preference_structure.relations)
 
+    def __getitem__(self, pair: Tuple[Any, Any]) -> Relation | None:
+        """Return relation between elements.
 
+        :param a:
+        :param b:
+        :return: relation between `a` and `b` if existing, else ``None``
+        """
+        _pair = set(pair)
+        for r in self._preference_structure.relations:
+            if set(r.elements) == _pair:
+                return r
+        return None
+
+    def __iter__(self) -> Iterator[Tuple[Any, Any]]:
+        """Iterate on the elements pairs with an existing relation"""
+        for r in self._preference_structure.relations:
+            yield r.elements
+
+
+@set_module("mcda.relations")
 class PreferenceStructure:
     """This class represents a list of relations.
 
     Any type of relations is accepted, so this represents the union of P, I and
     R.
 
     :param data:
+    :param validate: whether to check compatibility of :attr:`relations`
+    :raise ValueError:
+        if :attr:`relations` are not compatible and `validate` is ``True``
     """
 
     def __init__(
         self,
         data: Union[
             List[Relation], Relation, PreferenceStructure, None
         ] = None,
+        validate: bool = True,
     ):
         data = [] if data is None else data
         if isinstance(data, Relation):
             relations = [data]
         elif isinstance(data, PreferenceStructure):
             relations = data.relations
         else:
             relations = data
         self._relations = list(set(relations))
-        self.validate()
+        if validate:
+            self._validate()
 
     @property
     def elements(self) -> List:
         """Return elements present in relations list."""
         return sorted(set(e for r in self._relations for e in r.elements))
 
     @property
     def relations(self) -> List[Relation]:
-        """Return copy of relations list."""
-        return self._relations.copy()
+        """Return relations list."""
+        return self._relations
+
+    @property
+    def elements_structures(self) -> Mapping[Any, PreferenceStructure]:
+        """Return this preference structure viewed by each element"""
+        return ElementView(self)
+
+    @property
+    def elements_pairs_relations(
+        self,
+    ) -> Mapping[Tuple[Any, Any], Union[Relation, None]]:
+        """Return the relations keyed by elements pairs"""
+        return ElementsPairView(self)
 
-    def validate(self):
+    @property
+    def typed_structures(self) -> Mapping[Type[Relation], PreferenceStructure]:
+        """Return the preference structures for each type of relation"""
+        return RelationTypeView(self)
+
+    def substructure(
+        self,
+        elements: List | None = None,
+        types: List[Type[Relation]] | None = None,
+    ) -> PreferenceStructure:
+        """Return a new preference structure containing only set arguments.
+
+        :param elements: if ``None`` all :attr:`elements` are used
+        :param types: if ``None``, all types of relations are used
+        :return:
+        """
+        res = PreferenceStructure()
+        for r in self._relations:
+            if types is not None and type(r) not in types:
+                continue
+            if elements is not None and (
+                r.a not in elements or r.b not in elements
+            ):
+                continue
+            res += r
+        return res
+
+    def _validate(self):
         """Check whether the relations are all valid.
 
         :raise ValueError: if at least two relations are incompatible
         """
         for i, r1 in enumerate(self._relations):
             for r2 in self._relations[(i + 1) :]:
                 if not r1.compatible(r2):
                     raise ValueError(f"incompatible relations: {r1}, {r2}")
 
     @property
     def is_total_preorder(self) -> bool:
         """Check whether relations list is a total preorder or not"""
         return (
-            len(
-                PreferenceStructure(
-                    self.transitive_closure[IncomparableRelation]
-                )
-            )
+            len(self.transitive_closure.typed_structures[IncomparableRelation])
             == 0
         )
 
     @property
     def is_total_order(self) -> bool:
         """Check whether relations list is a total order or not"""
-        res = self.transitive_closure
         return (
-            len(PreferenceStructure(res[IncomparableRelation]))
-            + len(PreferenceStructure(res[IndifferenceRelation]))
+            len(
+                self.transitive_closure.substructure(
+                    types=[IndifferenceRelation, IncomparableRelation]
+                )
+            )
             == 0
         )
 
     def __eq__(self, other: Any):
         """Check if preference structure is equal to another.
 
         Equality is defined as having the same set of relations.
@@ -337,118 +485,69 @@
     def __repr__(self) -> str:  # pragma: nocover
         """Return representation of relations contained in structure
 
         :return:
         """
         return f"{self.__class__.__name__}({repr(self._relations)})"
 
-    def _relation(
-        self,
-        *args: Any,
-    ) -> Union[Relation, PreferenceStructure, None]:
-        """Return all relations between given elements of given types.
-
-        If no relation type is supplied, all are considered.
-        If no element is supplied, all are considered.
-
-        :param *args:
-        :return:
-
-        .. warning:: Does not check for a relation's validity or redundancy!
-        """
-        elements = []
-        types = []
-        for arg in args:
-            if isinstance(arg, type) and issubclass(arg, Relation):
-                types.append(arg)
-            else:
-                elements.append(arg)
-        elements = self.elements if len(elements) == 0 else elements
-        types = Relation.types() if len(types) == 0 else types
-        res = None
-        for r in self._relations:
-            if r.a in elements and r.b in elements and r.__class__ in types:
-                res = r if res is None else cast(Relation, res) + r
-        return res
-
-    def _element_relations(
-        self, a: Any
-    ) -> Union[Relation, PreferenceStructure, None]:
-        """Return all relations involving given element.
-
-        :param a: element
-        :return:
-
-        .. warning:: Does not check for a relation's validity or redundancy!
-        """
-        res = None
-        for r in self._relations:
-            if a in r.elements:
-                res = r if res is None else cast(Relation, res) + r
-        return res
-
-    def __getitem__(
-        self, item: Any
-    ) -> Union[Relation, PreferenceStructure, None]:
-        """Return all relations matching the request
-
-        :param item:
-        :return:
-            Depending on `item` type:
-                * pair of elements: search first relation with this elements
-                pair
-                * element: all relations involving element
-                * relation class: all relations of this class
-        """
-        if isinstance(item, tuple):
-            return self._relation(*item)
-        if isinstance(item, type):
-            return self._relation(item)
-        return self._element_relations(item)
-
-    def __delitem__(self, item: Any):
-        """Remove all relations matching the request
-
-        :param item:
-        :return:
-            Depending on `item` type:
-                * pair of elements: search first relation with this elements
-                pair
-                * element: all relations involving element
-                * relation class: all relations of this class
-        """
-        r = self[item]
-        to_delete = PreferenceStructure(r)._relations
-        self._relations = [rr for rr in self._relations if rr not in to_delete]
-
     def __contains__(self, item: Any) -> bool:
         """Check whether a relation is already in the preference structure.
 
         :param item: relation
         :return: check result
 
         .. warning:: Does not check for a relation's validity!
         """
         for r in self._relations:
             if r == item:
                 return True
         return False
 
-    def __add__(self, other: Any) -> PreferenceStructure:
+    def __add__(
+        self, other: Relation | PreferenceStructure
+    ) -> PreferenceStructure:
         """Create new preference structure with appended relations.
 
         :param other:
             * :class:`Relation`: relation is appended into new object
             * :class:`PreferenceStructure`: all relations are appended into new
             object
         :return:
         """
-        if hasattr(other, "__iter__"):
-            return self.__class__(self._relations + [r for r in other])
-        return self.__class__(self._relations + [other])
+        if isinstance(other, PreferenceStructure):
+            for r1 in other:
+                for r2 in self:
+                    if not r1.compatible(r2):
+                        raise ValueError(f"incompatible relations: {r1}, {r2}")
+            return self.__class__(
+                self._relations + other._relations, validate=False
+            )
+        for r2 in self:
+            if not other.compatible(r2):
+                raise ValueError(f"incompatible relations: {other}, {r2}")
+        return self.__class__(self._relations + [other], validate=False)
+
+    def __sub__(
+        self, other: Relation | PreferenceStructure
+    ) -> PreferenceStructure:
+        """Create new preference structure with deleted relations.
+
+        :param other:
+            * :class:`Relation`: relation is removed in new object
+            * :class:`PreferenceStructure`: all relations are removed in new
+            object
+        :return:
+        """
+        if isinstance(other, PreferenceStructure):
+            return self.__class__(
+                list(set(self._relations) - {r for r in other}), validate=False
+            )
+        return self.__class__(
+            list(set(self._relations) - {other}), validate=False
+        )
 
     def __iter__(self) -> Iterator[Relation]:
         """Return iterator over relations
 
         :return:
         """
         return iter(self._relations)
@@ -465,15 +564,15 @@
             (w.r.t transitivity of preference and indifference relations)
         """
         res: List[Relation] = []
         for i, a in enumerate(ranking.labels):
             for b in ranking.labels[(i + 1) :]:
                 if ranking[a] == ranking[b]:
                     res.append(IndifferenceRelation(a, b))
-                elif ranking.scale.is_better(ranking[a], ranking[b]):
+                elif ranking[a] > ranking[b]:
                     res.append(PreferenceRelation(a, b))
                 else:
                     res.append(PreferenceRelation(b, a))
         return cls(res)
 
     @classmethod
     def from_outranking_matrix(
@@ -495,15 +594,15 @@
                 elif outranking_matrix.data.at[j, i]:
                     relations.append(PreferenceRelation(j, i))
                 else:
                     relations.append(IncomparableRelation(i, j))
         return cls(relations)
 
     @property
-    def ranking(self) -> Ranking:
+    def ranking(self) -> CommensurableValues[QuantitativeScale]:
         """Convert preference structure to ranking.
 
         :raises ValueError: if `preference_structure` is not a total pre-order
         :return:
 
         .. note:: returned ranking goes for 0 to n-1 (with 0 the best rank)
         """
@@ -511,20 +610,27 @@
             raise ValueError(
                 "only total pre-order can be represented as Ranking"
             )
         s = Series(0, index=self.elements)
         pref_copy = self.transitive_closure
         while len(pref_copy.elements) > 0:
             bad_alternatives = set()
-            for r in PreferenceStructure(pref_copy[PreferenceRelation]):
+            for r in pref_copy.typed_structures[PreferenceRelation]:
                 bad_alternatives.add(r.b)
             s[[*bad_alternatives]] += 1
-            for a in set(pref_copy.elements) - bad_alternatives:
-                del pref_copy[a]
-        return Ranking(
+            remaining_relations = []
+            elements_to_delete = set(pref_copy.elements) - bad_alternatives
+            for r in pref_copy.relations:
+                if (
+                    r.a not in elements_to_delete
+                    and r.b not in elements_to_delete
+                ):
+                    remaining_relations.append(r)
+            pref_copy = PreferenceStructure(remaining_relations)
+        return CommensurableValues(
             s,
             QuantitativeScale(preference_direction=PreferenceDirection.MIN),
         )
 
     @property
     def outranking_matrix(self) -> OutrankingMatrix:
         """Transform a preference structure into an outranking matrix.
@@ -561,14 +667,15 @@
 
         .. warning:: This function may bundle together multiple elements
         """
         return PreferenceStructure.from_outranking_matrix(
             self.outranking_matrix.transitive_reduction
         )
 
+    @requires_graphviz
     def plot(self) -> Digraph:
         """Create graph from preference structure and plot it.
 
         :return: graph
 
         .. note::
             You need an environment that will actually display the graph (such
@@ -579,14 +686,15 @@
         relation_graph.attr("node", shape="box")
         for e in self.elements:
             relation_graph.node(str(e))
         for r in self._relations:
             r._draw(relation_graph)
         return relation_graph
 
+    @requires_graphviz
     def save_plot(self) -> str:  # pragma: nocover
         """Plot preference structure as a graph and save it.
 
         :return: file name where plot is saved
         """
         return self.plot().render()
```

### Comparing `mcda-0.6.1/src/mcda/core/scales.py` & `mcda-0.7.0/src/mcda/internal/core/scales.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from typing import Any, List, Type, TypeVar, Union, cast
 
 import numpy as np
 from pandas import Series
 from pandas.api.types import is_numeric_dtype
 
 from .functions import FuzzyNumber, Interval
+from .utils import set_module
 
 if sys.version_info >= (3, 11):  # pragma: nocover
     from typing import Self
 else:
     from typing_extensions import Self
 
 
+@set_module("mcda.scales")
 class PreferenceDirection(Enum):
     """Enumeration of MCDA preference directions."""
 
     MIN = "MIN"
     MAX = "MAX"
 
     @classmethod
@@ -38,22 +40,15 @@
 
         :return:
         """
         s = ", ".join(f"{item}: {item.value}" for item in cls)
         return "PreferenceDirection only has following values " + s
 
 
-MIN = PreferenceDirection.MIN
-"""User-friendly way to call :attr:`PreferenceDirection.MIN`"""
-
-
-MAX = PreferenceDirection.MAX
-"""User-friendly way to call :attr:`PreferenceDirection.MAX`"""
-
-
+@set_module("mcda.types")
 class Scale(ABC):
     """Basic abstract class for MCDA scale.
 
     :attr preference_direction:
     """
 
     def __init__(self, **kwargs) -> None:
@@ -117,14 +112,15 @@
         if is_numeric_dtype(data):
             scale = QuantitativeScale.fit(data, **kwargs)
         else:
             scale = NominalScale.fit(data, **kwargs)
         return cast(Self, scale)
 
 
+@set_module("mcda.scales")
 class NominalScale(Scale):
     """This class implements a MCDA nominal scale.
 
     :param labels:
     """
 
     def __init__(self, labels: List, **kwargs):
@@ -174,14 +170,15 @@
 
         :param data:
         :return: scale
         """
         return cls(data.unique().tolist())
 
 
+@set_module("mcda.types")
 class OrdinalScale(Scale, ABC):
     """This class defines a MCDA ordinal scale.
 
     :param preference_direction:
     """
 
     def __init__(
@@ -256,14 +253,15 @@
         else:
             scale = QualitativeScale.fit(
                 data, preference_direction=preference_direction, **kwargs
             )
         return cast(Self, scale)
 
 
+@set_module("mcda.scales")
 class QuantitativeScale(OrdinalScale):
     """Class for quantitative scale (interval based).
 
     :param arg1: min boundary of scale or complete interval
     :param dmax:
         max boundary of scale (only considered if `arg1` type is not interval)
     :param min_in: is min boundary inside scale or not
@@ -293,21 +291,21 @@
         return self._interval
 
     @property
     def numeric(self) -> QuantitativeScale:
         """Return corresponding numeric scale."""
         return self
 
-    @classmethod
-    def normal(cls) -> NormalScale:
+    @staticmethod
+    def normal() -> NormalScale:
         """Return normal scale.
 
         :return:
         """
-        return NormalScale()
+        return QuantitativeScale(0, 1)
 
     def __repr__(self) -> str:  # pragma: nocover
         """Return string representation of interval.
 
         :return:
         """
         if self.preference_direction:
@@ -397,39 +395,19 @@
         if not is_numeric_dtype(data):
             raise TypeError(f"{cls} can only fit numeric data")
         return cls(
             data.min(), data.max(), preference_direction=preference_direction
         )
 
 
-class NormalScale(QuantitativeScale):
-    """This class represents the normal quantitative scale."""
-
-    def __init__(self):
-        super().__init__(0, 1)
-
-    @classmethod
-    def fit(
-        cls,
-        data: Series,
-        preference_direction: Union[PreferenceDirection, None] = None,
-        **kwargs,
-    ) -> Self:
-        """Create a scale that fits the data.
-
-        :param data:
-        :param preference_direction: always ignored here
-        :return: scale
-        :raise TypeError: if `data` is not normalized
-        """
-        if (data < 0).any() or (data > 1).any():
-            raise TypeError(f"{cls} can only fit normalized data")
-        return cls()
+NormalScale = QuantitativeScale
+"""Type alias for normal scale"""
 
 
+@set_module("mcda.scales")
 class DiscreteQuantitativeScale(QuantitativeScale):
     """Class for discrete quantitative scale.
 
     :param values: numeric values that constitute the scale
     :param preference_direction:
     """
 
@@ -443,21 +421,21 @@
         super().__init__(
             min(self.values),
             max(self.values),
             preference_direction=preference_direction,
             **kwargs,
         )
 
-    @classmethod
-    def binary(cls) -> BinaryScale:
+    @staticmethod
+    def binary() -> BinaryScale:
         """Return binary scale.
 
         :return:
         """
-        return BinaryScale()
+        return DiscreteQuantitativeScale([0, 1])
 
     def __repr__(self) -> str:  # pragma: nocover
         """Return string representation of scale.
 
         :return:
         """
         if self.preference_direction:
@@ -516,39 +494,19 @@
         if not is_numeric_dtype(data):
             raise TypeError(f"{cls} can only fit numeric data")
         return cls(
             data.unique().tolist(), preference_direction=preference_direction
         )
 
 
-class BinaryScale(DiscreteQuantitativeScale):
-    """This class represents the binary discrete quantitative scale."""
-
-    def __init__(self):
-        super().__init__([0, 1])
-
-    @classmethod
-    def fit(
-        cls,
-        data: Series,
-        preference_direction: Union[PreferenceDirection, None] = None,
-        **kwargs,
-    ) -> Self:
-        """Create a scale that fits the data.
-
-        :param data:
-        :param preference_direction: always ignored here
-        :return: scale
-        :raise TypeError: if `data` is not binary
-        """
-        if not set(data.unique().tolist()).issubset({0, 1}):
-            raise TypeError(f"{cls} can only fit binary data")
-        return cls()
+BinaryScale = DiscreteQuantitativeScale
+"""Type alias for binary scale"""
 
 
+@set_module("mcda.scales")
 class QualitativeScale(OrdinalScale, NominalScale):
     """This class implements a MCDA qualitative scale.
 
     :param values: numeric series with labels as index
     :param preference_direction:
     :raises TypeError:
         * if `values` contains non-numeric values
@@ -657,14 +615,15 @@
         uniques = data.unique()
         return cls(
             Series(list(range(len(uniques))), index=uniques),
             preference_direction,
         )
 
 
+@set_module("mcda.scales")
 class FuzzyScale(QualitativeScale):
     """This class implements a MCDA fuzzy qualitative scale.
 
     :param fuzzy:
     :param preference_direction:
     :param defuzzify_method:
     :raises TypeError:
@@ -817,15 +776,15 @@
         """Return label associated to given number.
 
         :param x:
         :raises ValueError: if `x` corresponds to no label
         :return: most probable label associated to given value
         """
 
-        confidences = self.fuzzy.apply(lambda f, xx=x: f.apply(xx))
+        confidences = self.fuzzy.apply(lambda f, xx=x: f(xx))
         confidences.sort_values(ascending=False)
 
         if confidences.iloc[0] <= 0:
             raise ValueError(f"value outside scale: {x}")
         return confidences.index.tolist()[0]
 
     @classmethod
```

### Comparing `mcda-0.6.1/src/mcda/core/set_functions.py` & `mcda-0.7.0/src/mcda/internal/core/set_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 from abc import ABC
 from math import factorial, isclose
 from typing import Dict, List, Union
 
 import numpy as np
 from pandas import DataFrame, Series
 
+from .utils import set_module
+
 if sys.version_info >= (3, 11):  # pragma: nocover
     from typing import Self
 else:
     from typing_extensions import Self
 
 
+@set_module("mcda.set_functions")
 class HashableSet(set):
     """This class adds the hashable property to a set object.
 
     It is intended as a replacement of the native set structure whenever
     a set needs to be hashed (e.g when using sets as dictionary keys).
     """
 
@@ -140,14 +143,15 @@
         if ``True``, raises an error when building an invalid instance
     """
 
     def __init__(
         self,
         values: Union[List, Dict, ISetFunction],
         ensemble: Union[List, None] = None,
+        validate: bool = True,
     ):
         if isinstance(values, ISetFunction):
             self._values = values.values
             self._ensemble = values.ensemble
         elif isinstance(values, dict):
             self._values = {HashableSet(k): v for k, v in values.items()}
             self._ensemble = (
@@ -161,17 +165,18 @@
                 if ensemble is None
                 else ensemble
             )
             self._values = {
                 HashableSet.from_index(i, ensemble): v
                 for i, v in enumerate(values)
             }
-        self.validate()
+        if validate:
+            self._validate()
 
-    def validate(self):
+    def _validate(self):
         """Validate the instance if it respects its properties.
 
         The properties are the following:
             * the set is defined on a subset of the ensemble
 
         :raise KeyError:
             if set function is defined on keys outside the ensemble
@@ -437,14 +442,15 @@
         """Call this set function on the set composed of all provided arguments
 
         :return: value
         """
         return self._values[HashableSet([*args])]
 
 
+@set_module("mcda.set_functions")
 class SetFunction(ISetFunction):
     """This class represents a set function.
 
     :param values:
         values of the function as either:
             * a list ordered as a binary mask on the `ensemble`
             * a dictionary with :class:`HashableSet` as keys
@@ -475,16 +481,16 @@
         :param k:
         :return:
 
         .. note:: use :func:`math.isclose` to add absolute tolerance
         """
         return self.mobius.is_k_additive(k)
 
-    @classmethod
-    def uniform_capacity(cls, ensemble: List) -> SetFunction:
+    @staticmethod
+    def uniform_capacity(ensemble: List) -> SetFunction:
         """Return uniform capacity of given ensemble.
 
         The uniform capacity on an ensemble `N` of size `size` is given by:
 
         .. math::
 
             \\mu^*(T) = t/n, \\forall T \\subseteq N
@@ -495,14 +501,15 @@
         .. note:: Formula is based on :cite:p:`grabisch2008review`.
         """
         res = SetFunction([0] * 2 ** len(ensemble), ensemble)
         res._values = {k: len(k) / res.size for k in res}
         return res
 
 
+@set_module("mcda.set_functions")
 class Mobius(ISetFunction):
     """This class represents the Möbius transform of a set function.
 
     :param values:
         values of the function as either:
             * a list ordered as a binary mask on the `ensemble`
             * a dictionary with :class:`HashableSet` as keys
```

### Comparing `mcda-0.6.1/src/mcda/core/transformers.py` & `mcda-0.7.0/src/mcda/internal/core/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     NormalScale,
     OrdinalScale,
     PreferenceDirection,
     QualitativeScale,
     QuantitativeScale,
     Scale,
 )
+from .utils import set_module
 from .values import CommensurableValues, Values
 
 S = TypeVar("S", bound=Scale)
 
 
 class ITransformer(ABC):
     """This abstract class describes a generic transformer class."""
@@ -603,14 +604,15 @@
         elif isinstance(data, PartialValueMatrix):
             return cls._transform_partial_values(data, out_scales)
         elif isinstance(in_scales, Scale) and isinstance(out_scales, Scale):
             return cls._transform_one(data, in_scales, out_scales)
         raise TypeError("type of arguments not supported")
 
 
+@set_module("mcda.transformers")
 class Transformer(ITransformer):
     """This class defines the basic transformer methods.
 
     It uses normalization and denormalization methods to transform values
     between scales, based on quantitative interval boundaries mapping.
     """
 
@@ -665,14 +667,15 @@
         :return: transformed value
 
         .. note:: not intended for general usage
         """
         return cls._denormalize_one(cls._normalize_one(x, in_scale), out_scale)
 
 
+@set_module("mcda.transformers")
 class ClosestTransformer(Transformer):
     """This transformer associates out-of-scale values with closest preferred
     ones in discrete ordinal scales.
     """
 
     @classmethod
     def _denormalize_one(cls, x: float, out_scale: S) -> Any:
```

### Comparing `mcda-0.6.1/src/mcda/core/values.py` & `mcda-0.7.0/src/mcda/internal/core/values.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from __future__ import annotations
 
 import sys
 from abc import ABC, abstractmethod
+from functools import total_ordering
 from typing import (
     Any,
     Generic,
     Iterator,
     List,
     Mapping,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from pandas import Series
 
-from .scales import (
-    OrdinalScale,
-    PreferenceDirection,
-    QuantitativeScale,
-    Scale,
-    common_scale_type,
-)
+from .scales import OrdinalScale, QuantitativeScale, Scale, common_scale_type
+from .utils import set_module
 
 if sys.version_info >= (3, 11):  # pragma: nocover
     from typing import Self
 else:
     from typing_extensions import Self
 
 
@@ -122,37 +118,89 @@
         return sum(self.data)
 
     @abstractmethod
     def copy(self) -> Self:  # pragma: nocover
         """Return a copy of the object"""
         pass
 
-    def __iter__(self) -> Iterator:
-        """Return an iterator over the data."""
-        return iter(self.data)
 
-    def __getitem__(self, item: Any) -> Any:
-        """Return the value of the data at a specific label.
+S = TypeVar("S", bound=Scale, covariant=True)
+
+
+@total_ordering
+@set_module("mcda.values")
+class Value(Generic[S]):
+    """This class define a single value along its scale.
+
+    Those instances are comparable with each other, as long as they share a
+    common :attr:`scale`, and can be compared to raw values.
+    In the latter case, the :attr:`scale` is assumed as beign the scale of the
+    raw value.
+
+    :param value:
+    :param scale:
+
+    .. note::
+        This class is not intended for general use, it is only intended for
+        the inspection of :class:`Values` cells.
+    """
 
+    def __init__(self, value: Any, scale: S):
+        self.value = value
+        self.scale = scale
+
+    def __gt__(self, other: Any) -> bool:
+        """Check if this value is greater than another.
+
+        :param other: either a raw value or a :class:`Value`
+        :raises ValueError:
+            if `other` is a :class:`Value` but have a different scale
+        :raises TypeError: if `other` is not a :class:`Value` instance
+        :return:
+            ``True`` if this value is greater than the other, else ``False``
+        """
+        if not isinstance(other, Value):
+            raise TypeError("cannot compare with a scale-less object")
+        if self.scale != other.scale:
+            raise ValueError("cannot compare values of different scales")
+        return self.scale.is_better(self.value, other.value)
+
+    def __eq__(self, other: Any) -> bool:
+        """Check if this value is equal to another.
+
+        :param other: either a raw value or a :class:`Value`
+        :raises ValueError:
+            if `other` is a :class:`Value` but have a different scale
+        :raises TypeError: if `other` is not a :class:`Value` instance
         :return:
+            ``True`` if this value is equal to the other, else ``False``
         """
-        return self.data[item]
-
-    def __setitem__(self, key: Any, value: Any):
-        """Set the value of the data at a specific label."""
-        self.data[key] = value
+        if not isinstance(other, Value):
+            raise TypeError("cannot compare with a scale-less object")
+        if self.scale != other.scale:
+            raise ValueError("cannot compare values of different scales")
+        return self.value == other.value
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Representation of the object"""
+        return f"<Value value={self.value} scale={repr(self.scale)}>"
 
-S = TypeVar("S", bound=Scale, covariant=True)
+    def __str__(self) -> str:  # pragma: nocover
+        """Convert object to string"""
+        return f"Value(value={self.value}, scale={str(self.scale)})"
 
 
-class Values(IVector, Generic[S]):
+@set_module("mcda.values")
+class Values(IVector, Mapping[Any, Value[S]], Generic[S]):
     """This class associates a data :class:`pandas.Series` with their
     multiple :class:`mcda.core.Scale`.
 
+    Instances are also immutable mapping of labels and :class:`Value` objects
+    and can be accessed, iterated over, as such.
+
     :param data: series containing the data
     :param scales:
         data scale(s) (one per value or one shared, will be inferred from data
         if absent using :meth:`Scale.fit`)
     :param stype: scales type used
     :raise KeyError: if some labels are duplicated
     :raise TypeError: if `stype` and `scales` types mismatch
@@ -186,14 +234,32 @@
                 Type[S],
                 common_scale_type([type(s) for s in self.scales.values()]),
             )
             if stype is None
             else stype
         )
 
+    def __len__(self) -> int:
+        """Return number of values.
+
+        :return:
+        """
+        return len(self.data)
+
+    def __iter__(self) -> Iterator:
+        """Return an iterator over the labels."""
+        return iter(self.labels)
+
+    def __getitem__(self, item: Any) -> Value[S]:
+        """Return the value of the data at a specific label.
+
+        :return:
+        """
+        return Value[S](self.data[item], self.scales[item])
+
     def __eq__(self, other: Any) -> bool:
         """Check equality of scale values.
 
         Equality is defines as having the same set of scales, and having the
         same data.
 
         :return: ``True`` if both are equal
@@ -329,21 +395,26 @@
         return True
 
     def copy(self) -> Self:
         """Return a copy of the object."""
         return self.__class__(self.data.copy(), dict(self.scales), self.stype)
 
 
+@set_module("mcda.values")
 class CommensurableValues(Values[S], Generic[S]):
     """This class describes values with a single scale.
 
+    Instances are also immutable mapping of labels and :class:`Value` objects
+    and can be accessed, iterated over, as such.
+
     :param data:
     :param scale:
     :param stype: scales type used
     :raise KeyError: if some labels are duplicated
+    :raise TypeError: if `stype` and `scale` type mismatch
 
     :attr data: internal representation of data
     """
 
     def __init__(
         self,
         data: Series,
@@ -396,29 +467,21 @@
         :return:
         :raise TypeError: if values are not ordinal
 
         .. warning:: :attr:`scales` are not taken into account
         """
         if not self.is_ordinal:
             raise TypeError("cannot sort non-ordinal values")
-        numerics = self.to_numeric
-        ascending = (
-            not ascending
-            if numerics.scale.preference_direction == PreferenceDirection.MIN
-            else ascending
-        )
         copy = self.copy()
-        copy.data = self.data[
-            numerics.data.sort_values(ascending=ascending).index
-        ]
+        ordered_labels = sorted(
+            copy.labels, key=lambda k: copy[k], reverse=not ascending
+        )
+        copy.data = self.data[ordered_labels]
         return copy
 
     def copy(self) -> Self:
         """Return a copy of the object."""
         return self.__class__(self.data.copy(), self.scale, self.stype)
 
 
-OS = TypeVar("OS", bound=OrdinalScale, covariant=True)
-
-
-Ranking = CommensurableValues[OS]
+Ranking = CommensurableValues[OrdinalScale]
 """Type alias for all ranking objects."""
```

### Comparing `mcda-0.6.1/src/mcda/mavt/uta.py` & `mcda-0.7.0/src/mcda/internal/mavt/uta.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,19 @@
     NormalScale,
     OrdinalScale,
     PreferenceDirection,
     QualitativeScale,
     QuantitativeScale,
 )
 from ..core.transformers import Transformer
+from ..core.utils import set_module
 from ..core.values import Ranking, Values
 
 
+@set_module("mcda.mavt.uta")
 class UTA(Learner[AdditiveValueFunctions[OrdinalScale]], Ranker):
     """This class represents the UTA disaggregator.
 
     :param performance_table:
     :param preference_structure:
     :param criteria_segments: number of segments per criteria
     :param delta: discrimination threshold for preference relations
@@ -76,15 +78,18 @@
         preference_structure: PreferenceStructure,
         criteria_segments: Union[Dict[Any, int], None] = None,
         delta: float = 0.001,
         post_optimality: bool = False,
         post_optimality_coeff: float = 0,
         solver_args: Union[Dict, None] = None,
     ):
-        if preference_structure[IncomparableRelation] is not None:
+        if (
+            len(preference_structure.typed_structures[IncomparableRelation])
+            > 0
+        ):
             raise TypeError(
                 f"{self.__class__} does not support IncomparableRelation "
                 "structures"
             )
         self.performance_table = performance_table
         self.preference_structure = preference_structure
         self.criteria_segments = (
@@ -289,15 +294,20 @@
                     {
                         v: function(Transformer.normalize(v, scale))
                         for v in scale.labels
                     }
                 )
             else:
                 npoints = [
-                    [Transformer.transform(x_ij, scale, NormalScale()), y_ij]
+                    [
+                        Transformer.transform(
+                            x_ij, scale, QuantitativeScale.normal()
+                        ),
+                        y_ij,
+                    ]
                     for x_ij, y_ij in zip(x[criterion], y[criterion])
                 ]
                 if scale.preference_direction == PreferenceDirection.MIN:
                     npoints = npoints[::-1]
                 nsegments = [
                     [p1, p2] for p1, p2 in zip(npoints[:-1], npoints[1:])
                 ]
@@ -446,14 +456,15 @@
             for u_ij, u_ij1 in zip(u_i[:-1], u_i[1:]):
                 problem += u_ij1 - u_ij >= 0
 
         # Utility normalization constraint
         problem += lpSum(u_i[-1] for u_i in u_var.values()) == 1
 
 
+@set_module("mcda.mavt.uta")
 class UTAstar(UTA):
     """This class represents the UTA\\* disaggregator.
 
     :param performance_table:
     :param criteria_segments: number of segments per criteria
     :param preference_structure:
     :param delta: discrimination threshold for preference relations
```

### Comparing `mcda-0.6.1/src/mcda/outranking/electre.py` & `mcda-0.7.0/src/mcda/internal/outranking/electre.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     Relation,
 )
 from ..core.scales import (
     PreferenceDirection,
     QualitativeScale,
     QuantitativeScale,
 )
-from ..core.values import Ranking, Values
+from ..core.utils import set_module
+from ..core.values import CommensurableValues, Values
 
 T = TypeVar("T")
 
 
 class IElectre(Generic[T], ABC):
     """This class represents the common interface between all Electre
     algorithms
@@ -123,17 +124,15 @@
         .. warning::
             this method assumes that alternatives values have the same scales
         """
         concordance_value = 0.0
         for k in alternative_values1.labels:
             concordance_value = (
                 concordance_value + self.criteria_weights[k]
-                if alternative_values1.scales[k].is_better_or_equal(
-                    alternative_values1[k], alternative_values2[k]
-                )
+                if alternative_values1[k] >= alternative_values2[k]
                 else concordance_value
             )
         concordance_value = concordance_value / sum(
             self.criteria_weights.values()
         )
         return concordance_value
 
@@ -171,18 +170,18 @@
         :return: discordance index
 
         .. warning::
             this method assumes that alternatives values have the same scales
         """
         return Series(
             {
-                c: abs(alternative_values2[c] - alternative_values1[c])
-                if alternative_values1.scales[c].is_better(
-                    alternative_values2[c], alternative_values1[c]
+                c: abs(
+                    alternative_values2.data[c] - alternative_values1.data[c]
                 )
+                if alternative_values2[c] > alternative_values1[c]
                 else 0
                 for c in alternative_values1.labels
             }
         )
 
     def discordance(
         self,
@@ -203,14 +202,15 @@
                 for ai in self.performance_table.alternatives
             ],
             vertices=self.performance_table.alternatives,
             stype=QuantitativeScale,
         )
 
 
+@set_module("mcda.outranking.electre")
 class Electre1(IElectre1[OutrankingMatrix], Selector):
     """This class implements the Electre I algorithm.
 
     :param performance_table:
     :param criteria_weights:
     :param concordance_threshold:
     :param veto_thresholds:
@@ -320,14 +320,15 @@
         """
         matrix = self.construct()
         return self.exploit(
             matrix, cycle_reduction=cycle_reduction, transitivity=transitivity
         )
 
 
+@set_module("mcda.outranking.electre")
 class Electre2(IElectre1[Tuple[OutrankingMatrix, OutrankingMatrix]], Ranker):
     """This class implements the Electre II algorithm.
 
     :param performance_table:
     :param criteria_weights:
     :param weak_concordance_threshold:
     :param strong_concordance_threshold:
@@ -567,16 +568,16 @@
             this method assumes that alternatives values have the same scales
         """
 
         scales = alternative_values1.scales
         return sum(
             self.criteria_weights[i]
             * self._concordance_index(
-                alternative_values1[i],
-                alternative_values2[i],
+                alternative_values1.data[i],
+                alternative_values2.data[i],
                 self.preference_thresholds[i],
                 self.indifference_thresholds[i],
                 scales[i].preference_direction,
             )
             for i in self.criteria_weights
         ) / sum(self.criteria_weights.values())
 
@@ -777,14 +778,15 @@
                 for i in performance_table.alternatives
             ],
             vertices=performance_table.alternatives,
             stype=QuantitativeScale,
         )
 
 
+@set_module("mcda.outranking.electre")
 class Electre3(IElectre3, Ranker):
     """This class implements the Electre III algorithm.
 
     :param performance_table:
     :param criteria_weights:
     :param indifference_thresholds:
     :param preference_thresholds:
@@ -921,14 +923,15 @@
         """Compute the complete Electre III algorithm
 
         :return: final outranking matrix
         """
         return self.exploit(self.construct())
 
 
+@set_module("mcda.outranking.electre")
 class ElectreTri(IElectre3, Assignator, Ranker):
     """This class implements the Electre-Tri B algorithm.
 
     :param performance_table:
     :param criteria_weights:
     :param profiles: profiles in ascending dominance order
     :param indifference_thresholds:
@@ -1119,15 +1122,15 @@
         return classes
 
     def exploit(
         self,
         outranking_structure: AdjacencyValueMatrix[QuantitativeScale],
         pessimistic: bool = False,
         **kwargs,
-    ) -> Ranking[QualitativeScale]:
+    ) -> CommensurableValues[QualitativeScale]:
         """Compute the exploitation procedure (either optimistically or
         pessimistically).
 
         :param outranking_structure: credibility matrix
         :param pessimistic: if ``True`` performs procedure pessimistically
         :return: alternative assignments
 
@@ -1143,21 +1146,21 @@
         alternatives = outranking_structure.vertices[
             : -len(self.profiles.alternatives)
         ]
         assignments = {}
         for cat, a_set in categories.items():
             assignments.update({a: cat for a in a_set})
         values = Series(assignments)
-        return Ranking(values[alternatives], scale=self.categories)
+        return CommensurableValues(values[alternatives], scale=self.categories)
 
     def assign(
         self,
         pessimistic: bool = False,
         **kwargs,
-    ) -> Ranking[QualitativeScale]:
+    ) -> CommensurableValues[QualitativeScale]:
         """Assign alternatives to categories.
 
         :param pessimistic:
         :return: alternative assignments
 
         .. note::
             the category profiles defining the categories are the ones from
@@ -1168,15 +1171,15 @@
             pessimistic=pessimistic,
         )
 
     def rank(
         self,
         pessimistic: bool = False,
         **kwargs,
-    ) -> Ranking[QualitativeScale]:
+    ) -> CommensurableValues[QualitativeScale]:
         """Rank alternatives by their assigned ordered category.
 
         :param pessimistic:
         :return: alternative assignments
 
         .. note::
             the category profiles defining the categories are the ones from
```

### Comparing `mcda-0.6.1/src/mcda/outranking/promethee.py` & `mcda-0.7.0/src/mcda/internal/outranking/promethee.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,22 @@
     PerformanceTable,
 )
 from ..core.relations import (
     IncomparableRelation,
     IndifferenceRelation,
     PreferenceRelation,
     PreferenceStructure,
-    Ranking,
     Relation,
 )
 from ..core.scales import PreferenceDirection, QuantitativeScale
+from ..core.utils import set_module
 from ..core.values import CommensurableValues, Values
 
 
+@set_module("mcda.functions")
 class UShapeFunction:
     """This class implements the u-shape preference function.
 
     :param q: the indifference threshold
     """
 
     def __init__(self, p: float = 0):
@@ -46,14 +47,15 @@
 
         :param x: criteria values difference
         :return:
         """
         return 1 if x > self.p else 0
 
 
+@set_module("mcda.functions")
 class VShapeFunction:
     """This class implements the linear level preference function.
 
     :param p: preference threshold
     :param q: indifference threshold
     """
 
@@ -74,14 +76,15 @@
             if x > self.p
             else (abs(x) - self.q) / (self.p - self.q)
             if x > self.q
             else 0
         )
 
 
+@set_module("mcda.functions")
 class LevelFunction:
     """This class implements the level preference function.
 
     :param p: preference threshold
     :param q: indifference threshold
     """
 
@@ -96,14 +99,15 @@
 
         :param x: criteria values difference
         :return:
         """
         return 1 if x > self.p else 0.5 if x > self.q else 0
 
 
+@set_module("mcda.functions")
 class GaussianFunction:
     """This class implements the gaussian preference function.
 
     :param s: standard deviation
     """
 
     def __init__(self, s: float):
@@ -831,14 +835,15 @@
 
         :param preferences:
         :return: flows
         """
         pass
 
 
+@set_module("mcda.outranking.promethee")
 class Promethee1(
     Promethee,
     Ranker,
 ):
     """This class implements Promethee I.
 
     Implementation and notations are based on :cite:p:`vincke1998promethee1`.
@@ -928,14 +933,15 @@
             for b in self.performance_table.alternatives[(i + 1) :]:
                 res += self._flow_intersection(
                     a, b, pos_flow[a], pos_flow[b], neg_flow[a], neg_flow[b]
                 )
         return res
 
 
+@set_module("mcda.outranking.promethee")
 class Promethee2(
     Promethee,
     Ranker,
 ):
     """This class implements Promethee II.
 
     Implementation and notations are based on :cite:p:`vincke1998promethee1`.
@@ -969,24 +975,27 @@
         """Computes net outranking flows.
 
         :param preferences:
         :return: net outranking flows
         """
         return net_outranking_flows(preferences)
 
-    def rank(self, **kwargs) -> Ranking:
+    def rank(self, **kwargs) -> CommensurableValues[QuantitativeScale]:
         """Apply Promethee II algorithm.
 
         :return: result as scores
         """
         partial_preferences = self.partial_preferences()
         preferences = self.preferences(partial_preferences)
-        return Ranking(self.flows(preferences))
+        return CommensurableValues(
+            self.flows(preferences), stype=QuantitativeScale
+        )
 
 
+@set_module("mcda.outranking.promethee")
 class PrometheeGaia(Promethee2):
     """This class is used to represent and draw a Promethee GAIA plane.
 
     Implementations naming conventions are taken from
     :cite:p:`figueira2005mcda`
 
     :param performance_table:
```

### Comparing `mcda-0.6.1/src/mcda/outranking/srmp.py` & `mcda-0.7.0/src/mcda/internal/outranking/srmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,38 +24,39 @@
 from ..core.interfaces import Learner, Ranker
 from ..core.matrices import PerformanceTable
 from ..core.relations import (
     IndifferenceRelation,
     OutrankingMatrix,
     PreferenceRelation,
     PreferenceStructure,
-    Ranking,
     create_outranking_matrix,
 )
 from ..core.scales import (
     DiscreteQuantitativeScale,
     PreferenceDirection,
     QuantitativeScale,
 )
 from ..core.transformers import ClosestTransformer
-from ..core.values import Values
+from ..core.utils import set_module
+from ..core.values import CommensurableValues, Values
 from ..plot.plot import (
     Annotation,
     AreaPlot,
     Axis,
     BarPlot,
     Figure,
     HorizontalStripes,
     LinePlot,
     ParallelCoordinatesPlot,
     StackedBarPlot,
     Text,
 )
 
 
+@set_module("mcda.outranking.srmp")
 class ProfileWiseOutranking(Ranker):
     """This class infers outranking relations related to a single profile.
 
     The relation compares each criterion of each alternative values with the
     category profile (``1`` if better or equal, ``0`` otherwise), apply
     the `criteria_weights` as a weighted sum for each alternative and compare
     those scores.
@@ -81,17 +82,17 @@
         :return:
         """
         conditional_weighted_sum = Series(
             {
                 a: sum(
                     [
                         self.criteria_weights[c]
-                        if s.is_better_or_equal(av[c], self.profile[c])
+                        if av[c] >= self.profile[c]
                         else 0
-                        for c, s in av.scales.items()
+                        for c in av
                     ]
                 )
                 for a, av in self.performance_table.alternatives_values.items()
             }
         )
 
         return create_outranking_matrix(
@@ -107,14 +108,15 @@
                 index=self.performance_table.alternatives,
                 columns=self.performance_table.alternatives,
                 dtype="int64",
             )
         )
 
 
+@set_module("mcda.outranking.srmp")
 class SRMP(Ranker):
     """This class implements the SRMP algorithm.
 
     :param performance_table:
     :param criteria_weights:
     :param profiles:
     :param lexicographic_order: profile indices used sequentially to rank
@@ -154,15 +156,15 @@
         """
         return [sub_srmp.rank() for sub_srmp in self.sub_srmp]
 
     def exploit(
         self,
         outranking_matrices: List[OutrankingMatrix],
         lexicographic_order: Union[List[int], None] = None,
-    ) -> Ranking:
+    ) -> CommensurableValues[DiscreteQuantitativeScale]:
         """Merge outranking matrices built by profiles in lexicographic
         order using SRMP exploitation method.
 
         :param outranking_matrices:
             outranking matrix constructed in :attr:`profiles` order
         :param lexicographic_order: (if not supplied, use attribute)
         :return:
@@ -187,23 +189,23 @@
         )
         outranking_matrix = score - score.transpose() >= 0
         scores = outranking_matrix.sum(1)
         scores_ordered = sorted(set(scores.values), reverse=True)
         ranks = cast(
             Series, scores.apply(lambda x: scores_ordered.index(x) + 1)
         )
-        return Ranking(
+        return CommensurableValues(
             ranks,
             scale=DiscreteQuantitativeScale(
                 ranks.tolist(),
                 PreferenceDirection.MIN,
             ),
         )
 
-    def rank(self, **kwargs) -> Ranking:
+    def rank(self, **kwargs) -> CommensurableValues[DiscreteQuantitativeScale]:
         """Compute the SRMP algorithm
 
         :return:
             the outranking total order as a ranking
         """
         return self.exploit(self.construct())
 
@@ -685,14 +687,15 @@
                     box=True,
                 )
             )
             previous_ranks = current_ranks
         fig.draw()
 
 
+@set_module("mcda.outranking.srmp")
 class SRMPLearner(Learner[Optional[SRMP]]):
     """This class gathers functions used to learn a SRMP model.
 
     :param performance_table:
     :param relations:
     :param max_profiles_number: highest number of reference profiles
     :param profiles_number: number of reference profiles
@@ -800,22 +803,22 @@
         # Number of profiles
         k = len(lexicographic_order)
         # Indices of profiles
         profile_indices = list(range(1, k + 1))
         # Lexicographic order
         sigma = [0] + [profile + 1 for profile in lexicographic_order]
         # Binary comparisons with preference
-        preference_relations = PreferenceStructure(
-            self.relations[PreferenceRelation]
-        )
+        preference_relations = self.relations.typed_structures[
+            PreferenceRelation
+        ]
         preference_relations_indices = range(len(preference_relations))
         # Binary comparisons with indifference
-        indifference_relations = PreferenceStructure(
-            self.relations[IndifferenceRelation]
-        )
+        indifference_relations = self.relations.typed_structures[
+            IndifferenceRelation
+        ]
         indifference_relations_indices = range(len(indifference_relations))
 
         #############
         # Variables #
         #############
 
         # Weights
```

### Comparing `mcda-0.6.1/src/mcda/plot/plot.py` & `mcda-0.7.0/src/mcda/internal/plot/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,71 @@
 """This module gathers all plotting functions.
 
 All those functions use `matplotlib <https://matplotlib.org/>`
 and `graphviz <https://graphviz.org/>`.
 """
 from __future__ import annotations
 
+import functools
 from typing import Any, List, Optional, Sequence, Tuple, Union, cast
 
-import matplotlib.colors as mcolors
-import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.patches import Circle, RegularPolygon
-from matplotlib.path import Path as MPath
-from matplotlib.projections import register_projection
-from matplotlib.projections.polar import PolarAxes
-from matplotlib.spines import Spine
-from matplotlib.ticker import FixedLocator
-from matplotlib.transforms import Affine2D
 from pandas import DataFrame, Index, Series
 
+try:
+    import matplotlib.colors as mcolors
+    import matplotlib.pyplot as plt
+    from matplotlib.patches import Circle, RegularPolygon
+    from matplotlib.path import Path as MPath
+    from matplotlib.projections import register_projection
+    from matplotlib.projections.polar import PolarAxes
+    from matplotlib.spines import Spine
+    from matplotlib.ticker import FixedLocator
+    from matplotlib.transforms import Affine2D
+
+    _has_matplotlib = True
+except ImportError:  # pragma: nocover
+    import warnings
+
+    warnings.warn(
+        "Plotting features not available. "
+        "If you need those, please install 'matplotlib' or this package "
+        "optional plotting dependencies 'mcda[plot]'."
+    )
+    _has_matplotlib = False
+
+
+def requires_matplotlib(obj):
+    """Wrap a class or function that requires matplotlib to function.
+
+    :param obj: either a class or function
+    :raises ImportError: if matplotlib is not installed
+    :return: wrapped class or function
+    """
+    if isinstance(obj, type):
+        # obj is a class
+        orig_init = obj.__init__
+
+        def init(self, *args, **kwargs):
+            if not _has_matplotlib:  # pragma: nocover
+                raise ImportError("This class requires 'matplotlib'")
+            return orig_init(self, *args, **kwargs)
+
+        obj.__init__ = init
+        return obj
+    else:
+        # obj is a function
+        @functools.wraps(obj)
+        def wrapped(*args, **kwargs):
+            if not _has_matplotlib:  # pragma: nocover
+                raise ImportError("This function requires 'matplotlib'")
+            return obj(*args, **kwargs)
+
+        return wrapped
+
 
 def piecewise_linear_colormap(
     colors: Any, name: str = "cmap"
 ) -> mcolors.LinearSegmentedColormap:
     """Create piecewise linear colormap.
 
     :param colors: list of any type of color accepted by :mod:`matplotlib`
```

### Comparing `mcda-0.6.1/src/mcda.egg-info/PKG-INFO` & `mcda-0.7.0/src/mcda.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mcda
-Version: 0.6.1
+Version: 0.7.0
 Summary: Package for Multi Criteria Decision Analysis
-Author-email: Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>
+Author-email: Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>, Patrick Meyer <patrick.meyer@imt-atlantique.fr>
 License: Copyright IMT Atlantique, 2021
         
         Project leaders:
           Patrick Meyer <patrick.meyer@imt-atlantique.fr>
           Nicolas Duminy <nicolas.duminy@imt-atlantique.fr>
         
         This software is an all-in-one package for Multi-Criteria Decision Analysis.
@@ -29,21 +29,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: matplotlib
 Requires-Dist: pulp
-Requires-Dist: graphviz
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: Deprecated
 Requires-Dist: typing_extensions; python_version < "3.11"
+Provides-Extra: plot
+Requires-Dist: graphviz; extra == "plot"
+Requires-Dist: matplotlib; extra == "plot"
+Provides-Extra: all
+Requires-Dist: mcda[plot]; extra == "all"
 
 Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
 # Package description
 
 This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
@@ -68,14 +71,27 @@
 
 If you want to simply use this package, simply install it from [PyPI](https://pypi.org/project/mcda/):
 
 ```bash
 pip install mcda
 ```
 
+**Note:**
+
+This package can be installed with different optional dependencies to unlock full features:
+
+* plot: unlock plotting utilities
+* all: include all the above optional dependencies
+
+If you want all optional dependencies for instance, do:
+
+```bash
+pip install "mcda[all]"
+```
+
 Once you installed our package, you can have a look at our [notebooks](https://py-mcda.readthedocs.io/en/latest/notebooks.html) section which contains examples on how to use our package.
 
 If you want to contribute to this package development, we recommend you to read the next section.
 
 
 # Contributors
```

