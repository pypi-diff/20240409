# Comparing `tmp/verifit-5.0.0.tar.gz` & `tmp/verifit-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-5.0.0.tar", last modified: Tue Apr  9 08:14:59 2024, max compression
+gzip compressed data, was "verifit-5.0.1.tar", last modified: Tue Apr  9 10:48:37 2024, max compression
```

## Comparing `verifit-5.0.0.tar` & `verifit-5.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 08:14:59.528126 verifit-5.0.0/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-5.0.0/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-09 06:39:01.000000 verifit-5.0.0/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    14455 2024-04-09 08:14:59.527801 verifit-5.0.0/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)    12633 2024-04-08 17:41:02.000000 verifit-5.0.0/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)      881 2024-04-09 07:47:22.000000 verifit-5.0.0/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)       52 2024-04-09 07:03:59.000000 verifit-5.0.0/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-09 08:14:59.528169 verifit-5.0.0/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 08:14:59.526658 verifit-5.0.0/src/
--rw-r--r--   0 sorel      (501) staff       (20)       72 2024-04-09 07:49:54.000000 verifit-5.0.0/src/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     3269 2024-04-09 07:37:28.000000 verifit-5.0.0/src/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)     1396 2024-04-09 07:40:13.000000 verifit-5.0.0/src/date_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)     4254 2024-04-09 08:03:59.000000 verifit-5.0.0/src/endpoint_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)     1574 2024-04-09 07:44:26.000000 verifit-5.0.0/src/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     2122 2024-04-09 07:21:31.000000 verifit-5.0.0/src/login.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 08:14:59.527573 verifit-5.0.0/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    14455 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      319 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       20 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 10:48:37.684053 verifit-5.0.1/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-5.0.1/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-09 06:39:01.000000 verifit-5.0.1/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)     4962 2024-04-09 10:48:37.683833 verifit-5.0.1/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)     3140 2024-04-09 10:47:34.000000 verifit-5.0.1/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)      881 2024-04-09 10:48:21.000000 verifit-5.0.1/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)       52 2024-04-09 07:03:59.000000 verifit-5.0.1/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-09 10:48:37.684102 verifit-5.0.1/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 10:48:37.682697 verifit-5.0.1/src/
+-rw-r--r--   0 sorel      (501) staff       (20)       72 2024-04-09 07:49:54.000000 verifit-5.0.1/src/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     3269 2024-04-09 07:37:28.000000 verifit-5.0.1/src/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1396 2024-04-09 07:40:13.000000 verifit-5.0.1/src/date_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)     4254 2024-04-09 08:03:59.000000 verifit-5.0.1/src/endpoint_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1574 2024-04-09 07:44:26.000000 verifit-5.0.1/src/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2122 2024-04-09 07:21:31.000000 verifit-5.0.1/src/login.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 10:48:37.683609 verifit-5.0.1/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)     4962 2024-04-09 10:48:37.000000 verifit-5.0.1/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      319 2024-04-09 10:48:37.000000 verifit-5.0.1/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-09 10:48:37.000000 verifit-5.0.1/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       20 2024-04-09 10:48:37.000000 verifit-5.0.1/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-09 10:48:37.000000 verifit-5.0.1/verifit.egg-info/top_level.txt
```

### Comparing `verifit-5.0.0/LICENSE` & `verifit-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-5.0.0/pyproject.toml` & `verifit-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "__pycache__/**/*"]
 
 [project]
 name = "verifit"
-version = "5.0.0"
+version = "5.0.1"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-5.0.0/src/cache.py` & `verifit-5.0.1/src/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-5.0.0/src/date_tools.py` & `verifit-5.0.1/src/date_tools.py`

 * *Files identical despite different names*

### Comparing `verifit-5.0.0/src/endpoint_tools.py` & `verifit-5.0.1/src/endpoint_tools.py`

 * *Files identical despite different names*

### Comparing `verifit-5.0.0/src/json_web_token.py` & `verifit-5.0.1/src/json_web_token.py`

 * *Files identical despite different names*

### Comparing `verifit-5.0.0/src/login.py` & `verifit-5.0.1/src/login.py`

 * *Files identical despite different names*

