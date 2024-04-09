# Comparing `tmp/vloc_plugin-0.0.3.tar.gz` & `tmp/vloc_plugin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc_plugin-0.0.3.tar", last modified: Tue Apr  9 03:40:11 2024, max compression
+gzip compressed data, was "vloc_plugin-0.0.4.tar", last modified: Tue Apr  9 06:42:41 2024, max compression
```

## Comparing `vloc_plugin-0.0.3.tar` & `vloc_plugin-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:40:11.771937 vloc_plugin-0.0.3/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.3/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 03:40:11.771735 vloc_plugin-0.0.3/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.3/README.md
--rw-r--r--   0 byron      (501) staff       (20)      536 2024-04-09 03:13:34.000000 vloc_plugin-0.0.3/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 03:40:11.771973 vloc_plugin-0.0.3/setup.cfg
--rw-------   0 byron      (501) staff       (20)      583 2024-04-08 09:39:30.000000 vloc_plugin-0.0.3/setup.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:40:11.770685 vloc_plugin-0.0.3/vloc/
--rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:40:26.000000 vloc_plugin-0.0.3/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:40:11.771542 vloc_plugin-0.0.3/vloc_plugin.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      202 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.258962 vloc_plugin-0.0.4/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.4/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 06:42:41.258775 vloc_plugin-0.0.4/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.4/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      479 2024-04-09 06:42:04.000000 vloc_plugin-0.0.4/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 06:42:41.259001 vloc_plugin-0.0.4/setup.cfg
+-rw-------   0 byron      (501) staff       (20)      583 2024-04-08 09:39:30.000000 vloc_plugin-0.0.4/setup.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.257599 vloc_plugin-0.0.4/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:40:26.000000 vloc_plugin-0.0.4/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.257957 vloc_plugin-0.0.4/vloc/plugin/
+-rw-r--r--   0 byron      (501) staff       (20)     1439 2024-04-09 02:44:26.000000 vloc_plugin-0.0.4/vloc/plugin/__info__.py
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-09 02:39:51.000000 vloc_plugin-0.0.4/vloc/plugin/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)      299 2024-04-09 03:13:08.000000 vloc_plugin-0.0.4/vloc/plugin/catalog.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 06:42:41.258611 vloc_plugin-0.0.4/vloc_plugin.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      273 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 06:42:41.000000 vloc_plugin-0.0.4/vloc_plugin.egg-info/top_level.txt
```

### Comparing `vloc_plugin-0.0.3/LICENSE.txt` & `vloc_plugin-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc_plugin-0.0.3/setup.py` & `vloc_plugin-0.0.4/setup.py`

 * *Files identical despite different names*

