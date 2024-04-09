# Comparing `tmp/akeneo_connector-0.1.4.tar.gz` & `tmp/akeneo_connector-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo_connector-0.1.4.tar", last modified: Tue Apr  9 09:36:22 2024, max compression
+gzip compressed data, was "akeneo_connector-0.1.5.tar", last modified: Tue Apr  9 10:15:46 2024, max compression
```

## Comparing `akeneo_connector-0.1.4.tar` & `akeneo_connector-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:36:22.271719 akeneo_connector-0.1.4/akeneo_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/akeneo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/akeneo_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/akeneo_product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/akeneo_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 09:36:19.000000 akeneo_connector-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:15:46.692841 akeneo_connector-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 10:15:41.000000 akeneo_connector-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 10:15:46.692841 akeneo_connector-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 10:15:41.000000 akeneo_connector-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:15:46.692841 akeneo_connector-0.1.5/akeneo_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 10:15:41.000000 akeneo_connector-0.1.5/akeneo_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-09 10:15:41.000000 akeneo_connector-0.1.5/akeneo_connector/akeneo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 10:15:41.000000 akeneo_connector-0.1.5/akeneo_connector/akeneo_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-09 10:15:41.000000 akeneo_connector-0.1.5/akeneo_connector/akeneo_product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:15:46.692841 akeneo_connector-0.1.5/akeneo_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 10:15:46.000000 akeneo_connector-0.1.5/akeneo_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 10:15:46.000000 akeneo_connector-0.1.5/akeneo_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:15:46.000000 akeneo_connector-0.1.5/akeneo_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:15:46.000000 akeneo_connector-0.1.5/akeneo_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 10:15:46.000000 akeneo_connector-0.1.5/akeneo_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:15:46.692841 akeneo_connector-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 10:15:43.000000 akeneo_connector-0.1.5/setup.py
```

### Comparing `akeneo_connector-0.1.4/LICENSE` & `akeneo_connector-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.4/PKG-INFO` & `akeneo_connector-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.4
+Version: 0.1.5
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.4/README.md` & `akeneo_connector-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.4/akeneo_connector/akeneo_connector.py` & `akeneo_connector-0.1.5/akeneo_connector/akeneo_connector.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.4/akeneo_connector/akeneo_paginator.py` & `akeneo_connector-0.1.5/akeneo_connector/akeneo_paginator.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.4/akeneo_connector/akeneo_product.py` & `akeneo_connector-0.1.5/akeneo_connector/akeneo_product.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,22 @@
         associations (dict): The associations of the product.
         quantified_associations (dict): The quantified associations of the product.
         metadata (dict): The metadata of the product.
         connector (AkeneoConnector): The Akeneo connector to use.
 
     """
 
-    def __init__(self, data: dict = {}, connector: AkeneoConnector = AkeneoConnector()):
+    def __init__(self, data: dict = {}, connector: AkeneoConnector | None = None):
         # Initialize the AkeneoProduct classs
         self.set(data)
 
-        self.connector = connector
+        if connector is None:
+            self.connector = AkeneoConnector()
+        else:
+            self.connector = connector
 
     def set(self, data: dict):
         """
         Sets the data of the product.
 
         Args:
             data (dict): The data of the product.
```

### Comparing `akeneo_connector-0.1.4/akeneo_connector.egg-info/PKG-INFO` & `akeneo_connector-0.1.5/akeneo_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.4
+Version: 0.1.5
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.4/setup.py` & `akeneo_connector-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="akeneo_connector",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

