# Comparing `tmp/fair_trees-2.3.1.tar.gz` & `tmp/fair_trees-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.1.tar", last modified: Tue Apr  9 15:23:44 2024, max compression
+gzip compressed data, was "fair_trees-2.3.2.tar", last modified: Tue Apr  9 15:38:24 2024, max compression
```

## Comparing `fair_trees-2.3.1.tar` & `fair_trees-2.3.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 15:23:44.452975 fair_trees-2.3.1/
--rw-rw-rw-   0        0        0      345 2024-04-09 15:23:44.452975 fair_trees-2.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 15:23:44.448021 fair_trees-2.3.1/fair_trees/
--rw-rw-rw-   0        0        0       91 2024-04-09 15:21:26.000000 fair_trees-2.3.1/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.1/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 15:23:44.452008 fair_trees-2.3.1/fair_trees.egg-info/
--rw-rw-rw-   0        0        0      345 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 15:23:44.000000 fair_trees-2.3.1/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 15:23:44.452975 fair_trees-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-04-09 15:23:39.000000 fair_trees-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:38:24.361981 fair_trees-2.3.2/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.2/LICENSE
+-rw-rw-rw-   0        0        0     4902 2024-04-09 15:38:24.360982 fair_trees-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2024-04-09 15:35:47.000000 fair_trees-2.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:38:24.355983 fair_trees-2.3.2/fair_trees/
+-rw-rw-rw-   0        0        0       91 2024-04-09 15:36:28.000000 fair_trees-2.3.2/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.2/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:38:24.359981 fair_trees-2.3.2/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4902 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:38:24.361981 fair_trees-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-04-09 15:37:49.000000 fair_trees-2.3.2/setup.py
```

### Comparing `fair_trees-2.3.1/fair_trees/fair_trees.py` & `fair_trees-2.3.2/fair_trees/fair_trees.py`

 * *Files identical despite different names*

