# Comparing `tmp/fair_trees-2.0.tar.gz` & `tmp/fair_trees-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.0.tar", last modified: Tue Apr  9 13:43:07 2024, max compression
+gzip compressed data, was "fair_trees-2.1.tar", last modified: Tue Apr  9 14:04:12 2024, max compression
```

## Comparing `fair_trees-2.0.tar` & `fair_trees-2.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:07.108720 fair_trees-2.0/
--rw-rw-rw-   0        0        0      343 2024-04-09 13:43:07.108720 fair_trees-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:07.107720 fair_trees-2.0/fair_trees.egg-info/
--rw-rw-rw-   0        0        0      343 2024-04-09 13:43:06.000000 fair_trees-2.0/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-09 13:43:06.000000 fair_trees-2.0/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:43:06.000000 fair_trees-2.0/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 13:43:06.000000 fair_trees-2.0/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:43:06.000000 fair_trees-2.0/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 13:43:07.108720 fair_trees-2.0/setup.cfg
--rw-rw-rw-   0        0        0      571 2024-04-09 13:41:35.000000 fair_trees-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:04:12.499498 fair_trees-2.1/
+-rw-rw-rw-   0        0        0      343 2024-04-09 14:04:12.498461 fair_trees-2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 14:04:12.493395 fair_trees-2.1/fair_trees/
+-rw-rw-rw-   0        0        0        0 2024-04-09 13:37:37.000000 fair_trees-2.1/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.1/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:04:12.498461 fair_trees-2.1/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-04-09 14:04:12.000000 fair_trees-2.1/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-09 14:04:12.000000 fair_trees-2.1/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:04:12.000000 fair_trees-2.1/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-09 14:04:12.000000 fair_trees-2.1/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 14:04:12.000000 fair_trees-2.1/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:04:12.499498 fair_trees-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      566 2024-04-09 14:03:51.000000 fair_trees-2.1/setup.py
```

### Comparing `fair_trees-2.0/setup.py` & `fair_trees-2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fair_trees",
-    version="2.0",
+    version="2.1",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
     install_requires=[
         "scipy",
         "numpy",
         "pandas",
         "joblib",
-        "scikit-learn"
+        "sklearn"
     ],
 )
```

