# Comparing `tmp/akeneo_connector-0.1.2.tar.gz` & `tmp/akeneo_connector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo_connector-0.1.2.tar", last modified: Tue Apr  9 07:33:12 2024, max compression
+gzip compressed data, was "akeneo_connector-0.1.3.tar", last modified: Tue Apr  9 08:22:49 2024, max compression
```

## Comparing `akeneo_connector-0.1.2.tar` & `akeneo_connector-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/akeneo_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/akeneo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/akeneo_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-09 07:33:06.000000 akeneo_connector-0.1.2/akeneo_connector/akeneo_product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/akeneo_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 07:33:12.000000 akeneo_connector-0.1.2/akeneo_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:33:12.070887 akeneo_connector-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 07:33:09.000000 akeneo_connector-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/akeneo_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/akeneo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/akeneo_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/akeneo_product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/akeneo_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 08:22:46.000000 akeneo_connector-0.1.3/setup.py
```

### Comparing `akeneo_connector-0.1.2/LICENSE` & `akeneo_connector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.2/PKG-INFO` & `akeneo_connector-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.2
+Version: 0.1.3
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 Here's how to use `AkeneoPaginator` to iterate through products:
 
 ```python
 from akeneo_connector import AkeneoConnector
 from akeneo_paginator import AkeneoPaginator
 
 # Initialize the paginator
-paginator = AkeneoPaginator(AkeneoPaginator.PRODUCTS_URL)
+paginator = AkeneoPaginator(AkeneoPaginator.products_url)
 
 # Fetch and print all products
 while paginator.next():
     for product in paginator.items:
         print(product)
 
 # Or iterate over all products directly
```

### Comparing `akeneo_connector-0.1.2/README.md` & `akeneo_connector-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 Here's how to use `AkeneoPaginator` to iterate through products:
 
 ```python
 from akeneo_connector import AkeneoConnector
 from akeneo_paginator import AkeneoPaginator
 
 # Initialize the paginator
-paginator = AkeneoPaginator(AkeneoPaginator.PRODUCTS_URL)
+paginator = AkeneoPaginator(AkeneoPaginator.products_url)
 
 # Fetch and print all products
 while paginator.next():
     for product in paginator.items:
         print(product)
 
 # Or iterate over all products directly
```

### Comparing `akeneo_connector-0.1.2/akeneo_connector/akeneo_connector.py` & `akeneo_connector-0.1.3/akeneo_connector/akeneo_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,42 +17,42 @@
         auth_url (str): The URL to authenticate with.
         access_token (str): The access token to use.
         headers (dict): The headers to use for the request.
         version (str): The version of the API to use.
     """
 
     # Constants
-    PRODUCT_URL = 'https://bordex.cloud.akeneo.com/api/rest/{version}/products/{identifier}'
-    PRODUCTS_URL = 'https://bordex.cloud.akeneo.com/api/rest/{version}/products'
+    PRODUCT_URL = 'https://{origin}/api/rest/{version}/products/{identifier}'
+    PRODUCTS_URL = 'https://{origin}/api/rest/{version}/products'
 
 
-    def __init__(self, username = None, password = None, auth_token = None, auth_url = None, version='v1'):
+    def __init__(self, origin: str | None = None, username = None, password = None, auth_token = None, auth_url = None, version='v1'):
         """
         Initializes an instance of the AkeneoConnector class.
 
         Args:
             username (str): The username to authenticate with.
             password (str): The password to authenticate with.
             auth_token (str): The authentication token to use.
             auth_url (str): The URL to authenticate with.
         """
         # Initialize the AkeneoConnector class
-        self.products_url = os.getenv('AKENEO_PRODUCTS_URL')
+        self.origin = os.getenv('AKENEO_ORIGIN') if origin is None else origin
         self.username = os.getenv('AKENEO_USERNAME') if username is None else username
         self.password = os.getenv('AKENEO_PASSWORD') if password is None else password
         self.auth_token = base64.b64encode((os.getenv('AKENEO_AUTH_TOKEN')  if auth_token is None else auth_token).encode()).decode()
         self.auth_url = os.getenv('AKENEO_AUTH_URL') if auth_url is None else auth_url
         self.access_token = self.get_access_token()
         self.headers = {
             'Authorization': 'Bearer ' + self.access_token,
             'Content-type': 'application/vnd.akeneo.collection+json'
         }
         self.version = version
-        self.product_url = self.PRODUCT_URL.format(version=self.version, identifier='{identifier}')
-        self.products_url = self.PRODUCTS_URL.format(version=self.version)
+        self.product_url = self.PRODUCT_URL.format(origin=self.origin, version=self.version, identifier='{identifier}')
+        self.products_url = self.PRODUCTS_URL.format(origin=self.origin, version=self.version)
 
     def get_access_token(self):
         """
         Gets the access token from Akeneo.
 
         Returns:
             str: The access token.
```

### Comparing `akeneo_connector-0.1.2/akeneo_connector/akeneo_paginator.py` & `akeneo_connector-0.1.3/akeneo_connector/akeneo_paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,14 @@
     def __init__(self, url: str | None = None, page_size: int = 10, version='v1'):
         """
         Initializes an instance of the AkeneoPaginator class.
 
         Args:
             response (dict): The response from the Akeneo API.
         """
-        if url is None:
-            url = AkeneoConnector.PRODUCTS_URL
-        
-        if url not in [
-            AkeneoConnector.PRODUCTS_URL,
-        ]:
-            raise ValueError(f'Invalid URL: {url}.')
-
-        # Add version
-        url = url.format(version=version)
 
         # Initialize the AkeneoPaginator class
         self.response = None
         self.items: list[AkeneoProduct] | list[dict] = []
         self.initial_url = url
         self.links = {
             'self': url + f'?limit={page_size}',
@@ -43,15 +33,23 @@
             'previous': None,
             'next': None,
             'last': None
         }
         self.page_size = page_size
         self.current_page = 1
         self.page_size = page_size
-        self.connector = AkeneoConnector()
+        self.connector = AkeneoConnector(version=version)
+
+        if url is None:
+            url = self.connector.products_url
+        
+        if url not in [
+            self.connector.products_url,
+        ]:
+            raise ValueError(f'Invalid URL: {url}.')
 
     def set(self, response):
         """
         Sets the response of the paginator.
 
         Args:
             response (dict): The response from the Akeneo API.
```

### Comparing `akeneo_connector-0.1.2/akeneo_connector/akeneo_product.py` & `akeneo_connector-0.1.3/akeneo_connector/akeneo_product.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,14 @@
         associations (dict): The associations of the product.
         quantified_associations (dict): The quantified associations of the product.
         metadata (dict): The metadata of the product.
         connector (AkeneoConnector): The Akeneo connector to use.
 
     """
 
-    # Constants
-    PRODUCT_URL = 'https://bordex.cloud.akeneo.com/api/rest/{version}/products/{identifier}'
-
     def __init__(self, data: dict = {}, connector: AkeneoConnector = AkeneoConnector()):
         # Initialize the AkeneoProduct classs
         self.set(data)
 
         self.connector = connector
 
     def set(self, data: dict):
```

### Comparing `akeneo_connector-0.1.2/akeneo_connector.egg-info/PKG-INFO` & `akeneo_connector-0.1.3/akeneo_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.2
+Version: 0.1.3
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 Here's how to use `AkeneoPaginator` to iterate through products:
 
 ```python
 from akeneo_connector import AkeneoConnector
 from akeneo_paginator import AkeneoPaginator
 
 # Initialize the paginator
-paginator = AkeneoPaginator(AkeneoPaginator.PRODUCTS_URL)
+paginator = AkeneoPaginator(AkeneoPaginator.products_url)
 
 # Fetch and print all products
 while paginator.next():
     for product in paginator.items:
         print(product)
 
 # Or iterate over all products directly
```

### Comparing `akeneo_connector-0.1.2/setup.py` & `akeneo_connector-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="akeneo_connector",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

