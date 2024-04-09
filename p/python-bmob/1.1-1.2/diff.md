# Comparing `tmp/python-bmob-1.1.tar.gz` & `tmp/python-bmob-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-bmob-1.1.tar", last modified: Tue Apr  9 14:04:25 2024, max compression
+gzip compressed data, was "dist\python-bmob-1.2.tar", last modified: Tue Apr  9 14:55:33 2024, max compression
```

## Comparing `python-bmob-1.1.tar` & `python-bmob-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:04:25.332369 python-bmob-1.1/
--rw-rw-rw-   0        0        0      278 2024-04-09 14:04:25.332369 python-bmob-1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 14:04:25.321150 python-bmob-1.1/bmobpy/
--rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.1/bmobpy/__init__.py
--rw-rw-rw-   0        0        0    19744 2024-04-09 14:01:42.000000 python-bmob-1.1/bmobpy/bmob.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:04:25.331241 python-bmob-1.1/python_bmob.egg-info/
--rw-rw-rw-   0        0        0      278 2024-04-09 14:04:25.000000 python-bmob-1.1/python_bmob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-09 14:04:25.000000 python-bmob-1.1/python_bmob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:04:25.000000 python-bmob-1.1/python_bmob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 14:04:25.000000 python-bmob-1.1/python_bmob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 14:04:25.332369 python-bmob-1.1/setup.cfg
--rw-rw-rw-   0        0        0      406 2024-04-09 14:03:35.000000 python-bmob-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:33.656922 python-bmob-1.2/
+-rw-rw-rw-   0        0        0      278 2024-04-09 14:55:33.656922 python-bmob-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:33.647743 python-bmob-1.2/bmobpy/
+-rw-rw-rw-   0        0        0       25 2024-04-09 14:54:42.000000 python-bmob-1.2/bmobpy/__init__.py
+-rw-rw-rw-   0        0        0    19744 2024-04-09 14:01:42.000000 python-bmob-1.2/bmobpy/bmob.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:33.656922 python-bmob-1.2/python_bmob.egg-info/
+-rw-rw-rw-   0        0        0      278 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:55:33.660472 python-bmob-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      406 2024-04-09 14:54:55.000000 python-bmob-1.2/setup.py
```

### Comparing `python-bmob-1.1/bmobpy/bmob.py` & `python-bmob-1.2/bmobpy/bmob.py`

 * *Files identical despite different names*

