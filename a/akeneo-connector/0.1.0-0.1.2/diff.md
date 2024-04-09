# Comparing `tmp/akeneo_connector-0.1.0.tar.gz` & `tmp/akeneo_connector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo_connector-0.1.0.tar", last modified: Tue Apr  9 06:59:00 2024, max compression
+gzip compressed data, was "akeneo_connector-0.1.2.tar", last modified: Tue Apr  9 07:33:12 2024, max compression
```

## Comparing `akeneo_connector-0.1.0.tar` & `akeneo_connector-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-04-09 06:59:00.146032 akeneo_connector-0.1.0/
--rw-r--r--   0 robin      (501) staff       (20)     1065 2024-04-08 14:20:27.000000 akeneo_connector-0.1.0/LICENSE
--rw-r--r--   0 robin      (501) staff       (20)     4263 2024-04-09 06:59:00.145536 akeneo_connector-0.1.0/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)     3544 2024-04-09 06:53:49.000000 akeneo_connector-0.1.0/README.md
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-04-09 06:59:00.142439 akeneo_connector-0.1.0/akeneo_connector/
--rw-r--r--   0 robin      (501) staff       (20)      133 2024-04-09 06:57:15.000000 akeneo_connector-0.1.0/akeneo_connector/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)     5187 2024-04-08 15:05:33.000000 akeneo_connector-0.1.0/akeneo_connector/akeneo_connector.py
--rw-r--r--   0 robin      (501) staff       (20)     4395 2024-04-08 15:00:44.000000 akeneo_connector-0.1.0/akeneo_connector/akeneo_paginator.py
--rw-r--r--   0 robin      (501) staff       (20)     7259 2024-04-08 15:04:04.000000 akeneo_connector-0.1.0/akeneo_connector/akeneo_product.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-04-09 06:59:00.145030 akeneo_connector-0.1.0/akeneo_connector.egg-info/
--rw-r--r--   0 robin      (501) staff       (20)     4263 2024-04-09 06:59:00.000000 akeneo_connector-0.1.0/akeneo_connector.egg-info/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)      363 2024-04-09 06:59:00.000000 akeneo_connector-0.1.0/akeneo_connector.egg-info/SOURCES.txt
--rw-r--r--   0 robin      (501) staff       (20)        1 2024-04-09 06:59:00.000000 akeneo_connector-0.1.0/akeneo_connector.egg-info/dependency_links.txt
--rw-r--r--   0 robin      (501) staff       (20)       38 2024-04-09 06:59:00.000000 akeneo_connector-0.1.0/akeneo_connector.egg-info/requires.txt
--rw-r--r--   0 robin      (501) staff       (20)       17 2024-04-09 06:59:00.000000 akeneo_connector-0.1.0/akeneo_connector.egg-info/top_level.txt
--rw-r--r--   0 robin      (501) staff       (20)       38 2024-04-09 06:59:00.146163 akeneo_connector-0.1.0/setup.cfg
--rw-r--r--   0 robin      (501) staff       (20)      968 2024-04-09 06:58:11.000000 akeneo_connector-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/akeneo_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/akeneo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/akeneo_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/akeneo_product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/akeneo_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 07:33:09.000000 akeneo_connector-0.1.2/setup.py
```

### Comparing `akeneo_connector-0.1.0/LICENSE` & `akeneo_connector-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.0/PKG-INFO` & `akeneo_connector-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.0
+Version: 0.1.2
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,15 +37,15 @@
 ```python
 from akeneo_connector import AkeneoConnector
 
 # Initialize the connector
 connector = AkeneoConnector(username='your_username', password='your_password', auth_token='your_auth_token', auth_url='your_auth_url')
 
 # Use the connector to make API requests
-products = connector.get(connect.products_url)
+products = connector.get(connector.products_url)
 print(products)
 ```
 
 
 ## AkeneoPaginator
 `AkeneoPaginator` handles pagination in responses from the Akeneo API. It's designed to work seamlessly with `AkeneoConnector`, providing an easy way to iterate through pages of API responses.
```

### Comparing `akeneo_connector-0.1.0/README.md` & `akeneo_connector-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```python
 from akeneo_connector import AkeneoConnector
 
 # Initialize the connector
 connector = AkeneoConnector(username='your_username', password='your_password', auth_token='your_auth_token', auth_url='your_auth_url')
 
 # Use the connector to make API requests
-products = connector.get(connect.products_url)
+products = connector.get(connector.products_url)
 print(products)
 ```
 
 
 ## AkeneoPaginator
 `AkeneoPaginator` handles pagination in responses from the Akeneo API. It's designed to work seamlessly with `AkeneoConnector`, providing an easy way to iterate through pages of API responses.
```

### Comparing `akeneo_connector-0.1.0/akeneo_connector/akeneo_connector.py` & `akeneo_connector-0.1.2/akeneo_connector/akeneo_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,27 +125,21 @@
         batch_strings = [json.dumps(p) for p in payloads]
 
         # Join the JSON-strings into a single string
         data_str = "\n".join(batch_strings)
 
         # Set the payload to the joined JSON-strings
         print(f"PATCH {url}")
-        print(data_str)
-        #response = req.patch(url, headers=self.headers, data=data_str)
-        response = {
-            'status_code': 200,
-            'text': 'Success'
-        }
-        return response
+        response = req.patch(url, headers=self.headers, data=data_str)
 
-        # # Check if the request was successful
-        # if response.status_code < 200 or response.status_code >= 300:
-        #     print(f"Request error: {response.status_code} - {response.text}")
-        #     return None
+        # Check if the request was successful
+        if response.status_code < 200 or response.status_code >= 300:
+            print(f"Request error: {response.status_code} - {response.text}")
+            return None
         
-        # # Try to parse the response as JSON
-        # try:
-        #     data = response.json()
-        # except:
-        #     data = response.text
+        # Try to parse the response as JSON
+        try:
+            data = response.json()
+        except:
+            data = response.text
 
-        # return data
+        return data
```

### Comparing `akeneo_connector-0.1.0/akeneo_connector/akeneo_paginator.py` & `akeneo_connector-0.1.2/akeneo_connector/akeneo_paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from akeneo.akeneo_connector import AkeneoConnector
-from akeneo.akeneo_product import AkeneoProduct
+from akeneo_connector.akeneo_connector import AkeneoConnector
+from akeneo_connector.akeneo_product import AkeneoProduct
 
 
 
 class AkeneoPaginator:
     """
     The AkeneoPaginator class is used to paginate through the Akeneo API.
 
@@ -28,15 +28,15 @@
         if url not in [
             AkeneoConnector.PRODUCTS_URL,
         ]:
             raise ValueError(f'Invalid URL: {url}.')
 
         # Add version
         url = url.format(version=version)
-        
+
         # Initialize the AkeneoPaginator class
         self.response = None
         self.items: list[AkeneoProduct] | list[dict] = []
         self.initial_url = url
         self.links = {
             'self': url + f'?limit={page_size}',
             'first': None,
```

### Comparing `akeneo_connector-0.1.0/akeneo_connector/akeneo_product.py` & `akeneo_connector-0.1.2/akeneo_connector/akeneo_product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypedDict, Optional
 
-from akeneo.akeneo_connector import AkeneoConnector
+from akeneo_connector.akeneo_connector import AkeneoConnector
 
 class Value(TypedDict):
      locale: Optional[str]
      scope: Optional[str]
      data: str
 
 class AkeneoProduct:
```

### Comparing `akeneo_connector-0.1.0/akeneo_connector.egg-info/PKG-INFO` & `akeneo_connector-0.1.2/akeneo_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.0
+Version: 0.1.2
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,15 +37,15 @@
 ```python
 from akeneo_connector import AkeneoConnector
 
 # Initialize the connector
 connector = AkeneoConnector(username='your_username', password='your_password', auth_token='your_auth_token', auth_url='your_auth_url')
 
 # Use the connector to make API requests
-products = connector.get(connect.products_url)
+products = connector.get(connector.products_url)
 print(products)
 ```
 
 
 ## AkeneoPaginator
 `AkeneoPaginator` handles pagination in responses from the Akeneo API. It's designed to work seamlessly with `AkeneoConnector`, providing an easy way to iterate through pages of API responses.
```

### Comparing `akeneo_connector-0.1.0/setup.py` & `akeneo_connector-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="akeneo_connector",
-    version="0.1.0",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

