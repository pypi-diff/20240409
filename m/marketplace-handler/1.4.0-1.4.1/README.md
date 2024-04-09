# Comparing `tmp/marketplace_handler-1.4.0.tar.gz` & `tmp/marketplace_handler-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketplace_handler-1.4.0.tar", last modified: Mon Apr  1 06:16:45 2024, max compression
+gzip compressed data, was "marketplace_handler-1.4.1.tar", last modified: Tue Apr  9 18:10:07 2024, max compression
```

## Comparing `marketplace_handler-1.4.0.tar` & `marketplace_handler-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-01 06:16:45.961569 marketplace_handler-1.4.0/
--rw-r--r--   0 derijablya  (1000) derijablya  (1000)     1024 2024-04-01 06:16:45.961569 marketplace_handler-1.4.0/PKG-INFO
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      696 2024-03-29 15:24:29.000000 marketplace_handler-1.4.0/README.md
-drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-01 06:16:45.961569 marketplace_handler-1.4.0/marketpalce_handler/
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       51 2024-03-29 12:19:53.000000 marketplace_handler-1.4.0/marketpalce_handler/__init__.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     1429 2024-03-29 12:19:53.000000 marketplace_handler-1.4.0/marketpalce_handler/collector.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      421 2024-03-29 14:24:33.000000 marketplace_handler-1.4.0/marketpalce_handler/config.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      103 2024-03-07 08:33:17.000000 marketplace_handler-1.4.0/marketpalce_handler/exceptions.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      466 2024-02-12 18:26:47.000000 marketplace_handler-1.4.0/marketpalce_handler/logger.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     2434 2024-03-29 15:21:42.000000 marketplace_handler-1.4.0/marketpalce_handler/mapping.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      592 2024-02-12 18:26:47.000000 marketplace_handler-1.4.0/marketpalce_handler/marketplace.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     5552 2024-03-29 12:37:34.000000 marketplace_handler-1.4.0/marketpalce_handler/ozon.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      735 2024-03-29 12:19:53.000000 marketplace_handler-1.4.0/marketpalce_handler/schemas.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      291 2024-03-29 12:19:53.000000 marketplace_handler-1.4.0/marketpalce_handler/utils.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     1952 2024-03-29 15:14:50.000000 marketplace_handler-1.4.0/marketpalce_handler/validators.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)    14791 2024-04-01 06:13:58.000000 marketplace_handler-1.4.0/marketpalce_handler/wb.py
-drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-01 06:16:45.961569 marketplace_handler-1.4.0/marketplace_handler.egg-info/
--rw-r--r--   0 derijablya  (1000) derijablya  (1000)     1024 2024-04-01 06:16:45.000000 marketplace_handler-1.4.0/marketplace_handler.egg-info/PKG-INFO
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      666 2024-04-01 06:16:45.000000 marketplace_handler-1.4.0/marketplace_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)        1 2024-04-01 06:16:45.000000 marketplace_handler-1.4.0/marketplace_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       33 2024-04-01 06:16:45.000000 marketplace_handler-1.4.0/marketplace_handler.egg-info/requires.txt
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       20 2024-04-01 06:16:45.000000 marketplace_handler-1.4.0/marketplace_handler.egg-info/top_level.txt
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      536 2024-03-29 15:29:51.000000 marketplace_handler-1.4.0/pyproject.toml
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       38 2024-04-01 06:16:45.961569 marketplace_handler-1.4.0/setup.cfg
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      565 2024-04-01 06:16:44.000000 marketplace_handler-1.4.0/setup.py
-drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-01 06:16:45.961569 marketplace_handler-1.4.0/tests/
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     4239 2024-03-29 12:19:53.000000 marketplace_handler-1.4.0/tests/test_ozon.py
--rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     6831 2024-03-29 15:21:42.000000 marketplace_handler-1.4.0/tests/test_wb.py
+drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-09 18:10:07.671141 marketplace_handler-1.4.1/
+-rw-r--r--   0 derijablya  (1000) derijablya  (1000)     1024 2024-04-09 18:10:07.671141 marketplace_handler-1.4.1/PKG-INFO
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      696 2024-03-29 15:24:29.000000 marketplace_handler-1.4.1/README.md
+drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-09 18:10:07.671141 marketplace_handler-1.4.1/marketpalce_handler/
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       51 2024-03-29 12:19:53.000000 marketplace_handler-1.4.1/marketpalce_handler/__init__.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      844 2024-04-09 17:56:01.000000 marketplace_handler-1.4.1/marketpalce_handler/collector.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      421 2024-03-29 14:24:33.000000 marketplace_handler-1.4.1/marketpalce_handler/config.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      103 2024-03-07 08:33:17.000000 marketplace_handler-1.4.1/marketpalce_handler/exceptions.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      466 2024-02-12 18:26:47.000000 marketplace_handler-1.4.1/marketpalce_handler/logger.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     2434 2024-03-29 15:21:42.000000 marketplace_handler-1.4.1/marketpalce_handler/mapping.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      592 2024-02-12 18:26:47.000000 marketplace_handler-1.4.1/marketpalce_handler/marketplace.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     5552 2024-03-29 12:37:34.000000 marketplace_handler-1.4.1/marketpalce_handler/ozon.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      798 2024-04-09 18:03:01.000000 marketplace_handler-1.4.1/marketpalce_handler/schemas.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      291 2024-03-29 12:19:53.000000 marketplace_handler-1.4.1/marketpalce_handler/utils.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     1952 2024-03-29 15:14:50.000000 marketplace_handler-1.4.1/marketpalce_handler/validators.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)    14791 2024-04-01 06:13:58.000000 marketplace_handler-1.4.1/marketpalce_handler/wb.py
+drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-09 18:10:07.671141 marketplace_handler-1.4.1/marketplace_handler.egg-info/
+-rw-r--r--   0 derijablya  (1000) derijablya  (1000)     1024 2024-04-09 18:10:07.000000 marketplace_handler-1.4.1/marketplace_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      666 2024-04-09 18:10:07.000000 marketplace_handler-1.4.1/marketplace_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)        1 2024-04-09 18:10:07.000000 marketplace_handler-1.4.1/marketplace_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       33 2024-04-09 18:10:07.000000 marketplace_handler-1.4.1/marketplace_handler.egg-info/requires.txt
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       20 2024-04-09 18:10:07.000000 marketplace_handler-1.4.1/marketplace_handler.egg-info/top_level.txt
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      469 2024-04-09 18:05:03.000000 marketplace_handler-1.4.1/pyproject.toml
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)       38 2024-04-09 18:10:07.671141 marketplace_handler-1.4.1/setup.cfg
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)      565 2024-04-09 18:10:06.000000 marketplace_handler-1.4.1/setup.py
+drwxrwxr-x   0 derijablya  (1000) derijablya  (1000)        0 2024-04-09 18:10:07.671141 marketplace_handler-1.4.1/tests/
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     4239 2024-03-29 12:19:53.000000 marketplace_handler-1.4.1/tests/test_ozon.py
+-rw-rw-r--   0 derijablya  (1000) derijablya  (1000)     6831 2024-03-29 15:21:42.000000 marketplace_handler-1.4.1/tests/test_wb.py
```

### Comparing `marketplace_handler-1.4.0/PKG-INFO` & `marketplace_handler-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace_handler
-Version: 1.4.0
+Version: 1.4.1
 Summary: Module to interact with marketplaces
 Home-page: https://github.com/derijablya/marketplace-interface
 Author: derijabyla
 Author-email: dulugov@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.6.1
 Requires-Dist: requests>=2.31.0
```

### Comparing `marketplace_handler-1.4.0/README.md` & `marketplace_handler-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/marketpalce_handler/mapping.py` & `marketplace_handler-1.4.1/marketpalce_handler/mapping.py`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/marketpalce_handler/marketplace.py` & `marketplace_handler-1.4.1/marketpalce_handler/marketplace.py`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/marketpalce_handler/ozon.py` & `marketplace_handler-1.4.1/marketpalce_handler/ozon.py`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/marketpalce_handler/schemas.py` & `marketplace_handler-1.4.1/marketpalce_handler/schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 
 from pydantic import BaseModel, constr
 
 
 class MsItem(BaseModel):
     ms_id: str
     barcodes: str
@@ -29,11 +29,11 @@
     ms_ids: List[constr(strip_whitespace=True, min_length=1)]
     values: List[int]
     warehouse_ids: List[int]
 
 
 class CollectorItem(BaseModel):
     ms_id: str
-    product_id: str
-    offer_id: str
-    price: int
-    sku: str
+    product_id: Optional[str] = None
+    offer_id: Optional[str] = None
+    price: float
+    sku: Optional[str] = None
```

### Comparing `marketplace_handler-1.4.0/marketpalce_handler/validators.py` & `marketplace_handler-1.4.1/marketpalce_handler/validators.py`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/marketpalce_handler/wb.py` & `marketplace_handler-1.4.1/marketpalce_handler/wb.py`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/marketplace_handler.egg-info/PKG-INFO` & `marketplace_handler-1.4.1/marketplace_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace_handler
-Version: 1.4.0
+Version: 1.4.1
 Summary: Module to interact with marketplaces
 Home-page: https://github.com/derijablya/marketplace-interface
 Author: derijabyla
 Author-email: dulugov@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.6.1
 Requires-Dist: requests>=2.31.0
```

### Comparing `marketplace_handler-1.4.0/marketplace_handler.egg-info/SOURCES.txt` & `marketplace_handler-1.4.1/marketplace_handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/setup.py` & `marketplace_handler-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
     name="marketplace_handler",
-    version="1.4.0",
+    version="1.4.1",
     author="derijabyla",
     author_email="dulugov@gmail.com",
     description="Module to interact with marketplaces",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/derijablya/marketplace-interface",
     packages=find_packages(),
```

### Comparing `marketplace_handler-1.4.0/tests/test_ozon.py` & `marketplace_handler-1.4.1/tests/test_ozon.py`

 * *Files identical despite different names*

### Comparing `marketplace_handler-1.4.0/tests/test_wb.py` & `marketplace_handler-1.4.1/tests/test_wb.py`

 * *Files identical despite different names*
