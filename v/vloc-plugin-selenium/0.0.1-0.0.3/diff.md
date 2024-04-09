# Comparing `tmp/vloc_plugin_selenium-0.0.1.tar.gz` & `tmp/vloc_plugin_selenium-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc_plugin_selenium-0.0.1.tar", last modified: Tue Apr  9 01:51:57 2024, max compression
+gzip compressed data, was "vloc_plugin_selenium-0.0.3.tar", last modified: Tue Apr  9 03:31:49 2024, max compression
```

## Comparing `vloc_plugin_selenium-0.0.1.tar` & `vloc_plugin_selenium-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 01:51:57.015454 vloc_plugin_selenium-0.0.1/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.1/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      431 2024-04-09 01:51:57.015261 vloc_plugin_selenium-0.0.1/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.1/README.md
--rw-r--r--   0 byron      (501) staff       (20)      599 2024-04-09 01:51:48.000000 vloc_plugin_selenium-0.0.1/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 01:51:57.015490 vloc_plugin_selenium-0.0.1/setup.cfg
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 01:51:57.014058 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium/
--rw-r--r--   0 byron      (501) staff       (20)      660 2024-04-08 06:42:15.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 06:35:36.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 01:51:57.015058 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      431 2024-04-09 01:51:57.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      321 2024-04-09 01:51:57.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 01:51:57.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)       12 2024-04-09 01:51:57.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium.egg-info/requires.txt
--rw-r--r--   0 byron      (501) staff       (20)       21 2024-04-09 01:51:57.000000 vloc_plugin_selenium-0.0.1/vloc_plugin_selenium.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:31:49.349644 vloc_plugin_selenium-0.0.3/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.3/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      433 2024-04-09 03:31:49.349460 vloc_plugin_selenium-0.0.3/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 06:35:29.000000 vloc_plugin_selenium-0.0.3/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      585 2024-04-09 03:31:24.000000 vloc_plugin_selenium-0.0.3/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-09 03:31:49.349678 vloc_plugin_selenium-0.0.3/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:31:49.348415 vloc_plugin_selenium-0.0.3/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:42:34.000000 vloc_plugin_selenium-0.0.3/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-09 03:31:49.349279 vloc_plugin_selenium-0.0.3/vloc_plugin_selenium.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      433 2024-04-09 03:31:49.000000 vloc_plugin_selenium-0.0.3/vloc_plugin_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      272 2024-04-09 03:31:49.000000 vloc_plugin_selenium-0.0.3/vloc_plugin_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-09 03:31:49.000000 vloc_plugin_selenium-0.0.3/vloc_plugin_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)       12 2024-04-09 03:31:49.000000 vloc_plugin_selenium-0.0.3/vloc_plugin_selenium.egg-info/requires.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-09 03:31:49.000000 vloc_plugin_selenium-0.0.3/vloc_plugin_selenium.egg-info/top_level.txt
```

### Comparing `vloc_plugin_selenium-0.0.1/LICENSE.txt` & `vloc_plugin_selenium-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc_plugin_selenium-0.0.1/pyproject.toml` & `vloc_plugin_selenium-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["vloc_plugin_selenium"]
+include = ["vloc"]
 
 [project]
 name = "vloc_plugin_selenium"
-version = "0.0.1"
-urls = { text = "https://github.com/linyeh1129/vloc_plugin_selenium" }
+version = "0.0.3"
+urls = { GitHub = "https://github.com/linyeh1129/vloc_plugin_selenium" }
 authors = [{ name = 'Lin Yeh', email = 'lin_yeh@outlook.com' }]
 description = "Plugin functions for vloc"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ['ui aumomation', 'computer vision']
 classifiers = [
```

