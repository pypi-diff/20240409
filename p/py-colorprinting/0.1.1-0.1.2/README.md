# Comparing `tmp/py-colorprinting-0.1.1.tar.gz` & `tmp/py-colorprinting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-colorprinting-0.1.1.tar", last modified: Tue Apr  9 20:24:25 2024, max compression
+gzip compressed data, was "py-colorprinting-0.1.2.tar", last modified: Tue Apr  9 20:30:45 2024, max compression
```

## Comparing `py-colorprinting-0.1.1.tar` & `py-colorprinting-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:24:25.757093 py-colorprinting-0.1.1/
--rw-rw-rw-   0        0        0      220 2024-04-09 20:24:25.748246 py-colorprinting-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-09 17:18:23.000000 py-colorprinting-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:24:25.716181 py-colorprinting-0.1.1/colorprint/
--rw-rw-rw-   0        0        0       67 2024-04-09 17:16:29.000000 py-colorprinting-0.1.1/colorprint/__init__.py
--rw-rw-rw-   0        0        0      549 2024-04-09 20:17:38.000000 py-colorprinting-0.1.1/colorprint/core.py
--rw-rw-rw-   0        0        0     1366 2024-04-09 20:18:32.000000 py-colorprinting-0.1.1/colorprint/test.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:24:25.748246 py-colorprinting-0.1.1/py_colorprinting.egg-info/
--rw-rw-rw-   0        0        0      220 2024-04-09 20:24:25.000000 py-colorprinting-0.1.1/py_colorprinting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-09 20:24:25.000000 py-colorprinting-0.1.1/py_colorprinting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:24:25.000000 py-colorprinting-0.1.1/py_colorprinting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-09 20:24:25.000000 py-colorprinting-0.1.1/py_colorprinting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 20:24:25.000000 py-colorprinting-0.1.1/py_colorprinting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 20:24:25.757093 py-colorprinting-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      401 2024-04-09 20:24:14.000000 py-colorprinting-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:30:45.357574 py-colorprinting-0.1.2/
+-rw-rw-rw-   0        0        0      220 2024-04-09 20:30:45.357574 py-colorprinting-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-09 17:18:23.000000 py-colorprinting-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 20:30:45.321815 py-colorprinting-0.1.2/colorprint/
+-rw-rw-rw-   0        0        0       67 2024-04-09 17:16:29.000000 py-colorprinting-0.1.2/colorprint/__init__.py
+-rw-rw-rw-   0        0        0     2166 2024-04-09 20:30:30.000000 py-colorprinting-0.1.2/colorprint/core.py
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:30:33.000000 py-colorprinting-0.1.2/colorprint/test.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:30:45.357574 py-colorprinting-0.1.2/py_colorprinting.egg-info/
+-rw-rw-rw-   0        0        0      220 2024-04-09 20:30:44.000000 py-colorprinting-0.1.2/py_colorprinting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-09 20:30:45.000000 py-colorprinting-0.1.2/py_colorprinting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:30:44.000000 py-colorprinting-0.1.2/py_colorprinting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-09 20:30:44.000000 py-colorprinting-0.1.2/py_colorprinting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 20:30:44.000000 py-colorprinting-0.1.2/py_colorprinting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 20:30:45.357574 py-colorprinting-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      401 2024-04-09 20:30:35.000000 py-colorprinting-0.1.2/setup.py
```

