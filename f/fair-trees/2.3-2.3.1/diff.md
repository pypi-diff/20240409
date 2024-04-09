# Comparing `tmp/fair_trees-2.3.tar.gz` & `tmp/fair_trees-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.tar", last modified: Tue Apr  9 14:17:01 2024, max compression
+gzip compressed data, was "fair_trees-2.3.1.tar", last modified: Tue Apr  9 15:23:44 2024, max compression
```

## Comparing `fair_trees-2.3.tar` & `fair_trees-2.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:17:01.339892 fair_trees-2.3/
--rw-rw-rw-   0        0        0      343 2024-04-09 14:17:01.339892 fair_trees-2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 14:17:01.334840 fair_trees-2.3/fair_trees/
--rw-rw-rw-   0        0        0       24 2024-04-09 14:16:42.000000 fair_trees-2.3/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:17:01.338878 fair_trees-2.3/fair_trees.egg-info/
--rw-rw-rw-   0        0        0      343 2024-04-09 14:17:01.000000 fair_trees-2.3/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-09 14:17:01.000000 fair_trees-2.3/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:17:01.000000 fair_trees-2.3/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 14:17:01.000000 fair_trees-2.3/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 14:17:01.000000 fair_trees-2.3/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 14:17:01.339892 fair_trees-2.3/setup.cfg
--rw-rw-rw-   0        0        0      571 2024-04-09 14:16:54.000000 fair_trees-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:23:44.452975 fair_trees-2.3.1/
+-rw-rw-rw-   0        0        0      345 2024-04-09 15:23:44.452975 fair_trees-2.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 15:23:44.448021 fair_trees-2.3.1/fair_trees/
+-rw-rw-rw-   0        0        0       91 2024-04-09 15:21:26.000000 fair_trees-2.3.1/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.1/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:23:44.452008 fair_trees-2.3.1/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:23:44.452975 fair_trees-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-04-09 15:23:39.000000 fair_trees-2.3.1/setup.py
```

### Comparing `fair_trees-2.3/fair_trees/fair_trees.py` & `fair_trees-2.3.1/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3/setup.py` & `fair_trees-2.3.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fair_trees",
-    version="2.3",
+    version="2.3.1",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
     install_requires=[
         "scipy",
```

