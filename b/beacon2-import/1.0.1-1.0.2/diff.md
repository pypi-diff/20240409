# Comparing `tmp/beacon2-import-1.0.1.tar.gz` & `tmp/beacon2-import-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beacon2-import-1.0.1.tar", last modified: Mon Apr  8 12:44:53 2024, max compression
+gzip compressed data, was "beacon2-import-1.0.2.tar", last modified: Mon Apr  8 15:21:13 2024, max compression
```

## Comparing `beacon2-import-1.0.1.tar` & `beacon2-import-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 12:44:53.119631 beacon2-import-1.0.1/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      211 2024-04-08 12:44:53.119631 beacon2-import-1.0.1/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.1/README.md
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 12:44:53.115631 beacon2-import-1.0.1/beacon2_import.egg-info/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      211 2024-04-08 12:44:53.000000 beacon2-import-1.0.1/beacon2_import.egg-info/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      368 2024-04-08 12:44:53.000000 beacon2-import-1.0.1/beacon2_import.egg-info/SOURCES.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-04-08 12:44:53.000000 beacon2-import-1.0.1/beacon2_import.egg-info/dependency_links.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      124 2024-04-08 12:44:53.000000 beacon2-import-1.0.1/beacon2_import.egg-info/entry_points.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       85 2024-04-08 12:44:53.000000 beacon2-import-1.0.1/beacon2_import.egg-info/requires.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       14 2024-04-08 12:44:53.000000 beacon2-import-1.0.1/beacon2_import.egg-info/top_level.txt
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 12:44:53.115631 beacon2-import-1.0.1/import/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.1/import/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    16575 2024-04-08 11:19:40.000000 beacon2-import-1.0.1/import/beacon2_import.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.1/import/utils.py
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 12:44:53.115631 beacon2-import-1.0.1/search/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.1/search/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2-import-1.0.1/search/beacon2_search.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.1/search/utils.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-04-08 12:44:53.119631 beacon2-import-1.0.1/setup.cfg
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      830 2024-04-08 12:44:42.000000 beacon2-import-1.0.1/setup.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 15:21:13.855253 beacon2-import-1.0.2/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      211 2024-04-08 15:21:13.855253 beacon2-import-1.0.2/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.2/README.md
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 15:21:13.851253 beacon2-import-1.0.2/beacon2_import/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.2/beacon2_import/__init__.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    16575 2024-04-08 11:19:40.000000 beacon2-import-1.0.2/beacon2_import/beacon2_import.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.2/beacon2_import/utils.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 15:21:13.851253 beacon2-import-1.0.2/beacon2_import.egg-info/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      211 2024-04-08 15:21:13.000000 beacon2-import-1.0.2/beacon2_import.egg-info/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      392 2024-04-08 15:21:13.000000 beacon2-import-1.0.2/beacon2_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-04-08 15:21:13.000000 beacon2-import-1.0.2/beacon2_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      140 2024-04-08 15:21:13.000000 beacon2-import-1.0.2/beacon2_import.egg-info/entry_points.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       63 2024-04-08 15:21:13.000000 beacon2-import-1.0.2/beacon2_import.egg-info/requires.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       22 2024-04-08 15:21:13.000000 beacon2-import-1.0.2/beacon2_import.egg-info/top_level.txt
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-04-08 15:21:13.851253 beacon2-import-1.0.2/search/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.2/search/__init__.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2-import-1.0.2/search/beacon2_search.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.2/search/utils.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-04-08 15:21:13.855253 beacon2-import-1.0.2/setup.cfg
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      795 2024-04-08 15:20:06.000000 beacon2-import-1.0.2/setup.py
```

### Comparing `beacon2-import-1.0.1/import/beacon2_import.py` & `beacon2-import-1.0.2/beacon2_import/beacon2_import.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.1/import/utils.py` & `beacon2-import-1.0.2/beacon2_import/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.1/search/beacon2_search.py` & `beacon2-import-1.0.2/search/beacon2_search.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.1/search/utils.py` & `beacon2-import-1.0.2/search/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.1/setup.py` & `beacon2-import-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beacon2-import',
-    version='1.0.1',
+    version='1.0.2',
     author='Khaled Jumah',
     author_email='khalled.jooma@yahoo.com',
     description='Seamlessly import and query genomic variant data from a beacon',
     license = 'CC-BY-NC-4.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'beacon2-import = import.beacon2_import:beacon2_import',
-            'beacon2-search = search.beacon2_search:beacon_query'
+            'beacon2-import = beacon2_import.beacon2_import:beacon2_import',
+            'beacon2-search = beacon2_search.beacon2_search:beacon_query'
         ]
     },
     install_requires=[
        'jsonschema',
        'argparse',
-       'asyncio',
-       'datetime',
        'dataclasses',
        'typing',
        'bioblend',
        'cyvcf2',
        'pymongo',
-       'conf'
     ],
     dependency_links=[
         'git+https://github.com/CSCfi/beacon-python#egg=beacon-python',
     ]
 )
```

