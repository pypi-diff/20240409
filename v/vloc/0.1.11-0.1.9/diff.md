# Comparing `tmp/vloc-0.1.11.tar.gz` & `tmp/vloc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc-0.1.11.tar", last modified: Tue Apr  9 04:29:37 2024, max compression
+gzip compressed data, was "vloc-0.1.9.tar", last modified: Tue Apr  9 04:08:57 2024, max compression
```

## Comparing `vloc-0.1.11.tar` & `vloc-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,14 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:29:37.138477 vloc-0.1.11/
--rw-r--r--   0 byron      (501) staff       (20)     3142 2024-04-09 03:42:38.000000 vloc-0.1.11/.gitignore
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.11/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      382 2024-04-09 04:29:37.138237 vloc-0.1.11/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.11/README.md
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 04:29:37.138515 vloc-0.1.11/setup.cfg
--rw-------   0 byron      (501) staff       (20)      596 2024-04-09 04:27:58.000000 vloc-0.1.11/setup.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:29:37.136510 vloc-0.1.11/vloc/
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 04:15:40.000000 vloc-0.1.11/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:29:37.137230 vloc-0.1.11/vloc/config/
--rw-r--r--   0 byron      (501) staff       (20)     2291 2024-04-08 03:52:10.000000 vloc-0.1.11/vloc/config/__config__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:31:37.000000 vloc-0.1.11/vloc/config/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)      801 2024-04-08 03:51:03.000000 vloc-0.1.11/vloc/config/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:29:37.137538 vloc-0.1.11/vloc/detect/
--rw-r--r--   0 byron      (501) staff       (20)      152 2024-04-08 09:28:17.000000 vloc-0.1.11/vloc/detect/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:31:37.000000 vloc-0.1.11/vloc/detect/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)     6221 2024-04-09 04:01:08.000000 vloc-0.1.11/vloc/detect/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:29:37.137855 vloc-0.1.11/vloc/exception/
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:31:37.000000 vloc-0.1.11/vloc/exception/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)      211 2024-04-08 03:31:37.000000 vloc-0.1.11/vloc/exception/catalog.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:29:37.138018 vloc-0.1.11/vloc.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      382 2024-04-09 04:29:37.000000 vloc-0.1.11/vloc.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      367 2024-04-09 04:29:37.000000 vloc-0.1.11/vloc.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 04:29:37.000000 vloc-0.1.11/vloc.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 04:29:37.000000 vloc-0.1.11/vloc.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.549106 vloc-0.1.9/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.9/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      482 2024-04-09 04:08:57.548887 vloc-0.1.9/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.9/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      625 2024-04-09 04:08:12.000000 vloc-0.1.9/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 04:08:57.549143 vloc-0.1.9/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.547789 vloc-0.1.9/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 03:59:47.000000 vloc-0.1.9/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:08:57.548685 vloc-0.1.9/vloc.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      482 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      192 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)       63 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/requires.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 04:08:57.000000 vloc-0.1.9/vloc.egg-info/top_level.txt
```

### Comparing `vloc-0.1.11/LICENSE.txt` & `vloc-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

