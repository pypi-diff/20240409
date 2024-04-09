# Comparing `tmp/pyegeria-0.3.0.tar.gz` & `tmp/pyegeria-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegeria-0.3.0.tar", last modified: Mon Apr  8 22:44:49 2024, max compression
+gzip compressed data, was "pyegeria-0.3.1.tar", last modified: Tue Apr  9 01:05:09 2024, max compression
```

## Comparing `pyegeria-0.3.0.tar` & `pyegeria-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.899583 pyegeria-0.3.0/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-02-13 19:55:10.000000 pyegeria-0.3.0/LICENSE
--rw-r--r--   0 dwolfson   (501) staff       (20)        0 2024-02-13 19:55:10.000000 pyegeria-0.3.0/MANIFEST.in
--rw-r--r--   0 dwolfson   (501) staff       (20)     2420 2024-04-08 22:44:49.899366 pyegeria-0.3.0/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1489 2024-04-08 21:13:57.000000 pyegeria-0.3.0/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)     1016 2024-04-08 22:38:07.000000 pyegeria-0.3.0/pyproject.toml
--rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-08 22:44:49.899624 pyegeria-0.3.0/setup.cfg
--rw-r--r--   0 dwolfson   (501) staff       (20)     1165 2024-04-08 22:44:45.000000 pyegeria-0.3.0/setup.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.885802 pyegeria-0.3.0/src/
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.893242 pyegeria-0.3.0/src/pyegeria/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1601 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-08 15:06:56.000000 pyegeria-0.3.0/src/pyegeria/_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-03-18 16:53:12.000000 pyegeria-0.3.0/src/pyegeria/_exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-02-09 22:22:39.000000 pyegeria-0.3.0/src/pyegeria/_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-08 15:19:41.000000 pyegeria-0.3.0/src/pyegeria/_validators.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    99125 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    94359 2024-04-08 13:45:02.000000 pyegeria-0.3.0/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42704 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    35897 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    19930 2024-04-08 15:06:56.000000 pyegeria-0.3.0/src/pyegeria/gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6272 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/governance_author.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42436 2024-04-08 13:51:18.000000 pyegeria-0.3.0/src/pyegeria/my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    43011 2024-04-08 15:06:56.000000 pyegeria-0.3.0/src/pyegeria/platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     7502 2024-03-18 16:53:12.000000 pyegeria-0.3.0/src/pyegeria/registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    16273 2024-04-08 13:04:49.000000 pyegeria-0.3.0/src/pyegeria/server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-08 01:36:23.000000 pyegeria-0.3.0/src/pyegeria/utils.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.899016 pyegeria-0.3.0/src/pyegeria.egg-info/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2420 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1130 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/SOURCES.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/dependency_links.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/requires.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/top_level.txt
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.898749 pyegeria-0.3.0/tests/
--rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_automated_curation_omvs_cray.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-08 15:17:39.000000 pyegeria-0.3.0/tests/test_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10522 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     9624 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    40009 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3836 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-08 21:13:57.000000 pyegeria-0.3.0/tests/test_util_exp.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-08 20:18:54.000000 pyegeria-0.3.0/tests/test_validators.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 01:05:09.986959 pyegeria-0.3.1/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-02-13 19:55:10.000000 pyegeria-0.3.1/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)        0 2024-02-13 19:55:10.000000 pyegeria-0.3.1/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-09 01:05:09.986768 pyegeria-0.3.1/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-09 01:04:24.000000 pyegeria-0.3.1/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1016 2024-04-09 01:04:56.000000 pyegeria-0.3.1/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-09 01:05:09.987006 pyegeria-0.3.1/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1165 2024-04-09 01:04:24.000000 pyegeria-0.3.1/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 01:05:09.981007 pyegeria-0.3.1/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 01:05:09.983978 pyegeria-0.3.1/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1601 2024-04-08 21:13:57.000000 pyegeria-0.3.1/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-08 15:06:56.000000 pyegeria-0.3.1/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-03-18 16:53:12.000000 pyegeria-0.3.1/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-02-09 22:22:39.000000 pyegeria-0.3.1/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-08 15:19:41.000000 pyegeria-0.3.1/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    99125 2024-04-08 21:13:57.000000 pyegeria-0.3.1/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    94359 2024-04-08 13:45:02.000000 pyegeria-0.3.1/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42704 2024-04-08 21:13:57.000000 pyegeria-0.3.1/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    35897 2024-04-08 21:13:57.000000 pyegeria-0.3.1/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19930 2024-04-08 15:06:56.000000 pyegeria-0.3.1/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6272 2024-04-08 21:13:57.000000 pyegeria-0.3.1/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42436 2024-04-08 13:51:18.000000 pyegeria-0.3.1/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    43011 2024-04-08 15:06:56.000000 pyegeria-0.3.1/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     7502 2024-03-18 16:53:12.000000 pyegeria-0.3.1/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16273 2024-04-08 13:04:49.000000 pyegeria-0.3.1/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-08 01:36:23.000000 pyegeria-0.3.1/src/pyegeria/utils.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 01:05:09.986477 pyegeria-0.3.1/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-09 01:05:09.000000 pyegeria-0.3.1/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1130 2024-04-09 01:05:09.000000 pyegeria-0.3.1/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-09 01:05:09.000000 pyegeria-0.3.1/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-09 01:05:09.000000 pyegeria-0.3.1/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-09 01:05:09.000000 pyegeria-0.3.1/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-09 01:05:09.986306 pyegeria-0.3.1/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_automated_curation_omvs_cray.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-08 15:17:39.000000 pyegeria-0.3.1/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10522 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9624 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40009 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3836 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-08 15:06:56.000000 pyegeria-0.3.1/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-08 21:13:57.000000 pyegeria-0.3.1/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-08 20:18:54.000000 pyegeria-0.3.1/tests/test_validators.py
```

### Comparing `pyegeria-0.3.0/LICENSE` & `pyegeria-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/PKG-INFO` & `pyegeria-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
@@ -24,15 +24,15 @@
 Requires-Dist: httpx~=0.26.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 <!-- SPDX-License-Identifier: CC-BY-4.0 -->
 <!-- Copyright Contributors to the ODPi Egeria project. -->
 
-![Egeria Logo](https://github.com/odpi/egeria/blob/master/assets/img/ODPi_Egeria_Logo_color.png?raw=true)
+![Egeria Logo](https://egeria-project.org/assets/images/egeria-header.png)
 
 [![GitHub](https://img.shields.io/github/license/odpi/egeria)](LICENSE)
 
 
 # pyegeria: a python client for Egeria
 
 This is an experimental package for easily using the Egeria
```

### Comparing `pyegeria-0.3.0/README.md` & `pyegeria-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- SPDX-License-Identifier: CC-BY-4.0 -->
 <!-- Copyright Contributors to the ODPi Egeria project. -->
 
-![Egeria Logo](https://github.com/odpi/egeria/blob/master/assets/img/ODPi_Egeria_Logo_color.png?raw=true)
+![Egeria Logo](https://egeria-project.org/assets/images/egeria-header.png)
 
 [![GitHub](https://img.shields.io/github/license/odpi/egeria)](LICENSE)
 
 
 # pyegeria: a python client for Egeria
 
 This is an experimental package for easily using the Egeria
```

### Comparing `pyegeria-0.3.0/pyproject.toml` & `pyegeria-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #requires = ["hatchling"]
 requires = ["setuptools", "wheel"]
 #build-backend = "hatchling.build"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.3.0"
+version = "0.3.1"
 #license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
 description = "A python client for Egeria"
 readme= "README.md"
 requires-python = ">=3.10"
```

### Comparing `pyegeria-0.3.0/setup.py` & `pyegeria-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pyegeria',
     extras_require=dict(tests=["pytest"]),
     # packages=find_packages(where="src"),
     package_dir={"": "src"},
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(where="src"),
     url="https://egeria-project.org/egeria-python",
     project_urls={
         "Issues": "https://github.com/odpi/egeria-python/issues",
     },
     #license='Apache 2.0',
     author='Dan Wolfson',
```

### Comparing `pyegeria-0.3.0/src/pyegeria/__init__.py` & `pyegeria-0.3.1/src/pyegeria/__init__.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/_client.py` & `pyegeria-0.3.1/src/pyegeria/_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/_exceptions.py` & `pyegeria-0.3.1/src/pyegeria/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/_globals.py` & `pyegeria-0.3.1/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/_validators.py` & `pyegeria-0.3.1/src/pyegeria/_validators.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/automated_curation_omvs.py` & `pyegeria-0.3.1/src/pyegeria/automated_curation_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.1/src/pyegeria/core_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/full_omag_server_config.py` & `pyegeria-0.3.1/src/pyegeria/full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.1/src/pyegeria/glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/gov_engine.py` & `pyegeria-0.3.1/src/pyegeria/gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/governance_author.py` & `pyegeria-0.3.1/src/pyegeria/governance_author.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/my_profile_omvs.py` & `pyegeria-0.3.1/src/pyegeria/my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/platform_services.py` & `pyegeria-0.3.1/src/pyegeria/platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/registered_info.py` & `pyegeria-0.3.1/src/pyegeria/registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/server_operations.py` & `pyegeria-0.3.1/src/pyegeria/server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria/utils.py` & `pyegeria-0.3.1/src/pyegeria/utils.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/src/pyegeria.egg-info/PKG-INFO` & `pyegeria-0.3.1/src/pyegeria.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
@@ -24,15 +24,15 @@
 Requires-Dist: httpx~=0.26.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 <!-- SPDX-License-Identifier: CC-BY-4.0 -->
 <!-- Copyright Contributors to the ODPi Egeria project. -->
 
-![Egeria Logo](https://github.com/odpi/egeria/blob/master/assets/img/ODPi_Egeria_Logo_color.png?raw=true)
+![Egeria Logo](https://egeria-project.org/assets/images/egeria-header.png)
 
 [![GitHub](https://img.shields.io/github/license/odpi/egeria)](LICENSE)
 
 
 # pyegeria: a python client for Egeria
 
 This is an experimental package for easily using the Egeria
```

### Comparing `pyegeria-0.3.0/src/pyegeria.egg-info/SOURCES.txt` & `pyegeria-0.3.1/src/pyegeria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_automated_curation_omvs.py` & `pyegeria-0.3.1/tests/test_automated_curation_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_automated_curation_omvs_cray.py` & `pyegeria-0.3.1/tests/test_automated_curation_omvs_cray.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_client.py` & `pyegeria-0.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_core_omag_server_config.py` & `pyegeria-0.3.1/tests/test_core_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_full_omag_server_config.py` & `pyegeria-0.3.1/tests/test_full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_glossary_omvs.py` & `pyegeria-0.3.1/tests/test_glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_gov_engine.py` & `pyegeria-0.3.1/tests/test_gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_my_profile_omvs.py` & `pyegeria-0.3.1/tests/test_my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_platform_services.py` & `pyegeria-0.3.1/tests/test_platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_registered_info.py` & `pyegeria-0.3.1/tests/test_registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_server_operations.py` & `pyegeria-0.3.1/tests/test_server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_util_exp.py` & `pyegeria-0.3.1/tests/test_util_exp.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.0/tests/test_validators.py` & `pyegeria-0.3.1/tests/test_validators.py`

 * *Files identical despite different names*

