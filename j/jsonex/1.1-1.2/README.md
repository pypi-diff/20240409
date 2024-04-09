# Comparing `tmp/jsonex-1.1.tar.gz` & `tmp/jsonex-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonex-1.1.tar", last modified: Mon Apr  8 14:31:39 2024, max compression
+gzip compressed data, was "jsonex-1.2.tar", last modified: Tue Apr  9 18:53:04 2024, max compression
```

## Comparing `jsonex-1.1.tar` & `jsonex-1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:31:39.183510 jsonex-1.1/
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1073 2024-04-04 20:07:48.000000 jsonex-1.1/LICENSE
--rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2054 2024-04-08 14:31:39.183510 jsonex-1.1/PKG-INFO
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1748 2024-04-08 14:31:14.000000 jsonex-1.1/README.md
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:31:39.179510 jsonex-1.1/jsonex/
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2030 2024-04-08 14:31:14.000000 jsonex-1.1/jsonex/__init__.py
-drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-08 14:31:39.183510 jsonex-1.1/jsonex.egg-info/
--rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2054 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/PKG-INFO
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      165 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/SOURCES.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        1 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/dependency_links.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        7 2024-04-08 14:31:39.000000 jsonex-1.1/jsonex.egg-info/top_level.txt
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       38 2024-04-08 14:31:39.183510 jsonex-1.1/setup.cfg
--rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      555 2024-04-08 14:31:14.000000 jsonex-1.1/setup.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-09 18:53:04.919156 jsonex-1.2/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1073 2024-04-04 20:07:48.000000 jsonex-1.2/LICENSE
+-rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2143 2024-04-09 18:53:04.919156 jsonex-1.2/PKG-INFO
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1837 2024-04-09 18:48:24.000000 jsonex-1.2/README.md
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-09 18:53:04.915156 jsonex-1.2/jsonex/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2197 2024-04-09 18:48:24.000000 jsonex-1.2/jsonex/__init__.py
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      418 2024-04-09 18:48:24.000000 jsonex-1.2/jsonex/custom_data.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-09 18:53:04.919156 jsonex-1.2/jsonex.egg-info/
+-rw-r--r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     2143 2024-04-09 18:53:04.000000 jsonex-1.2/jsonex.egg-info/PKG-INFO
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      205 2024-04-09 18:53:04.000000 jsonex-1.2/jsonex.egg-info/SOURCES.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        1 2024-04-09 18:53:04.000000 jsonex-1.2/jsonex.egg-info/dependency_links.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       13 2024-04-09 18:53:04.000000 jsonex-1.2/jsonex.egg-info/top_level.txt
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)       38 2024-04-09 18:53:04.919156 jsonex-1.2/setup.cfg
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)      555 2024-04-09 18:52:53.000000 jsonex-1.2/setup.py
+drwxrwxr-x   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)        0 2024-04-09 18:53:04.919156 jsonex-1.2/tests/
+-rw-rw-r--   0 krzyzstofzylka  (1000) krzyzstofzylka  (1000)     1841 2024-04-09 18:48:53.000000 jsonex-1.2/tests/__init__.py
```

### Comparing `jsonex-1.1/LICENSE` & `jsonex-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonex-1.1/PKG-INFO` & `jsonex-1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonex
-Version: 1.1
+Version: 1.2
 Summary: Json library
 Author: Krzysztof Żyłka
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,20 @@
 From now on, attempting to save `list`, `dicts`, `set`, and custom objects to JSON should not cause any problems. For objects that cannot be formatted into JSON, 
 the following value will be returned:
 
 ```python
 f"[custom type: {type(value).__name__}]"
 ```
 
+## Custom data auto convert:
+```text
+pandas DataFrame => dict
+numpy ndarray => list
+```
+
 ## Encode json
 ```python
 from jsonex import JsonEx
 
 JsonEx.dump({})
 ```
```

### Comparing `jsonex-1.1/README.md` & `jsonex-1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 From now on, attempting to save `list`, `dicts`, `set`, and custom objects to JSON should not cause any problems. For objects that cannot be formatted into JSON, 
 the following value will be returned:
 
 ```python
 f"[custom type: {type(value).__name__}]"
 ```
 
+## Custom data auto convert:
+```text
+pandas DataFrame => dict
+numpy ndarray => list
+```
+
 ## Encode json
 ```python
 from jsonex import JsonEx
 
 JsonEx.dump({})
 ```
```

### Comparing `jsonex-1.1/jsonex/__init__.py` & `jsonex-1.2/jsonex/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-
+import jsonex.custom_data as custom_data
 
 class JsonEx:
 
     @staticmethod
     def dump(
             data,
             skipkeys=False,
@@ -31,14 +31,17 @@
             object_pairs_hook=None
     ):
         return json.loads(data, cls=cls, object_hook=object_hook, parse_float=parse_float, parse_int=parse_int, parse_constant=parse_constant, object_pairs_hook=object_pairs_hook)
 
     @staticmethod
     def _fix_data(data):
         for key, value in JsonEx._data_iteration(data):
+            value = custom_data.convert_dataframe_to_dict(value)
+            value = custom_data.convert_numpy_to_list(value)
+
             if JsonEx._is_custom_type(value):
                 data[key] = f"[custom type: {type(value).__name__}]"
             elif isinstance(value, dict):
                 data[key] = JsonEx._fix_data(value)
             elif isinstance(value, list):
                 data[key] = JsonEx._fix_data(value)
             elif isinstance(value, set):
```

### Comparing `jsonex-1.1/jsonex.egg-info/PKG-INFO` & `jsonex-1.2/jsonex.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonex
-Version: 1.1
+Version: 1.2
 Summary: Json library
 Author: Krzysztof Żyłka
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,20 @@
 From now on, attempting to save `list`, `dicts`, `set`, and custom objects to JSON should not cause any problems. For objects that cannot be formatted into JSON, 
 the following value will be returned:
 
 ```python
 f"[custom type: {type(value).__name__}]"
 ```
 
+## Custom data auto convert:
+```text
+pandas DataFrame => dict
+numpy ndarray => list
+```
+
 ## Encode json
 ```python
 from jsonex import JsonEx
 
 JsonEx.dump({})
 ```
```

### Comparing `jsonex-1.1/setup.py` & `jsonex-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='jsonex',
-    version='1.1',
+    version='1.2',
     description='Json library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Krzysztof Żyłka',
     install_requires=[],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ],
-)
+    ]
+)
```

