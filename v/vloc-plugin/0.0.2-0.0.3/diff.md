# Comparing `tmp/vloc_plugin-0.0.2.tar.gz` & `tmp/vloc_plugin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc_plugin-0.0.2.tar", last modified: Mon Apr  8 09:41:08 2024, max compression
+gzip compressed data, was "vloc_plugin-0.0.3.tar", last modified: Tue Apr  9 03:40:11 2024, max compression
```

## Comparing `vloc_plugin-0.0.2.tar` & `vloc_plugin-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-08 09:41:08.506343 vloc_plugin-0.0.2/
--rw-r--r--   0 byron      (501) staff       (20)     3115 2024-04-08 07:58:14.000000 vloc_plugin-0.0.2/.gitignore
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.2/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      369 2024-04-08 09:41:08.506037 vloc_plugin-0.0.2/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.2/README.md
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-08 09:41:08.506394 vloc_plugin-0.0.2/setup.cfg
--rw-------   0 byron      (501) staff       (20)      583 2024-04-08 09:39:30.000000 vloc_plugin-0.0.2/setup.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-08 09:41:08.505135 vloc_plugin-0.0.2/vloc_plugin/
--rw-r--r--   0 byron      (501) staff       (20)     1439 2024-04-08 09:37:06.000000 vloc_plugin-0.0.2/vloc_plugin/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:27:12.000000 vloc_plugin-0.0.2/vloc_plugin/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-08 09:41:08.505740 vloc_plugin-0.0.2/vloc_plugin.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      369 2024-04-08 09:41:08.000000 vloc_plugin-0.0.2/vloc_plugin.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      229 2024-04-08 09:41:08.000000 vloc_plugin-0.0.2/vloc_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-08 09:41:08.000000 vloc_plugin-0.0.2/vloc_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)       12 2024-04-08 09:41:08.000000 vloc_plugin-0.0.2/vloc_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:40:11.771937 vloc_plugin-0.0.3/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.3/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 03:40:11.771735 vloc_plugin-0.0.3/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.3/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      536 2024-04-09 03:13:34.000000 vloc_plugin-0.0.3/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 03:40:11.771973 vloc_plugin-0.0.3/setup.cfg
+-rw-------   0 byron      (501) staff       (20)      583 2024-04-08 09:39:30.000000 vloc_plugin-0.0.3/setup.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:40:11.770685 vloc_plugin-0.0.3/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:40:26.000000 vloc_plugin-0.0.3/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:40:11.771542 vloc_plugin-0.0.3/vloc_plugin.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      457 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      202 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 03:40:11.000000 vloc_plugin-0.0.3/vloc_plugin.egg-info/top_level.txt
```

### Comparing `vloc_plugin-0.0.2/LICENSE.txt` & `vloc_plugin-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc_plugin-0.0.2/setup.py` & `vloc_plugin-0.0.3/setup.py`

 * *Files identical despite different names*

