# Comparing `tmp/vloc-0.1.10.tar.gz` & `tmp/vloc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc-0.1.10.tar", last modified: Tue Apr  9 04:17:23 2024, max compression
+gzip compressed data, was "vloc-0.1.9.tar", last modified: Tue Apr  9 04:08:57 2024, max compression
```

## Comparing `vloc-0.1.10.tar` & `vloc-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:17:23.448860 vloc-0.1.10/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 03:31:37.000000 vloc-0.1.10/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      483 2024-04-09 04:17:23.448625 vloc-0.1.10/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 03:32:50.000000 vloc-0.1.10/README.md
--rw-r--r--   0 byron      (501) staff       (20)      626 2024-04-09 04:16:18.000000 vloc-0.1.10/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 04:17:23.448912 vloc-0.1.10/setup.cfg
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:17:23.447755 vloc-0.1.10/vloc/
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 04:15:40.000000 vloc-0.1.10/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 04:17:23.448438 vloc-0.1.10/vloc.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      483 2024-04-09 04:17:23.000000 vloc-0.1.10/vloc.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      192 2024-04-09 04:17:23.000000 vloc-0.1.10/vloc.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 04:17:23.000000 vloc-0.1.10/vloc.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)       63 2024-04-09 04:17:23.000000 vloc-0.1.10/vloc.egg-info/requires.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 04:17:23.000000 vloc-0.1.10/vloc.egg-info/top_level.txt
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

### Comparing `vloc-0.1.10/LICENSE.txt` & `vloc-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc-0.1.10/pyproject.toml` & `vloc-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["vloc"]
 
 [project]
 name = "vloc"
-version = "0.1.10"
+version = "0.1.9"
 urls = { GitHub = "https://github.com/linyeh1129/vloc" }
 authors = [{ name = 'Lin Yeh', email = 'lin_yeh@outlook.com' }]
 description = "Plugin functions for vloc"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ['ui aumomation', 'computer vision']
```

