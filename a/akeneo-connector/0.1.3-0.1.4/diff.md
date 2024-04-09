# Comparing `tmp/akeneo_connector-0.1.3.tar.gz` & `tmp/akeneo_connector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo_connector-0.1.3.tar", last modified: Tue Apr  9 08:22:49 2024, max compression
+gzip compressed data, was "akeneo_connector-0.1.4.tar", last modified: Tue Apr  9 09:36:22 2024, max compression
```

## Comparing `akeneo_connector-0.1.3.tar` & `akeneo_connector-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/akeneo_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/akeneo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/akeneo_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-09 08:22:38.000000 akeneo_connector-0.1.3/akeneo_connector/akeneo_product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/akeneo_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 08:22:49.000000 akeneo_connector-0.1.3/akeneo_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:22:49.438053 akeneo_connector-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 08:22:46.000000 akeneo_connector-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:36:22.271719 akeneo_connector-0.1.4/akeneo_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/akeneo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/akeneo_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-09 09:36:14.000000 akeneo_connector-0.1.4/akeneo_connector/akeneo_product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/akeneo_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 09:36:22.000000 akeneo_connector-0.1.4/akeneo_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:36:22.275719 akeneo_connector-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 09:36:19.000000 akeneo_connector-0.1.4/setup.py
```

### Comparing `akeneo_connector-0.1.3/LICENSE` & `akeneo_connector-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.3/PKG-INFO` & `akeneo_connector-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.3/README.md` & `akeneo_connector-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.3/akeneo_connector/akeneo_connector.py` & `akeneo_connector-0.1.4/akeneo_connector/akeneo_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,23 @@
         Args:
             username (str): The username to authenticate with.
             password (str): The password to authenticate with.
             auth_token (str): The authentication token to use.
             auth_url (str): The URL to authenticate with.
         """
         # Initialize the AkeneoConnector class
+        # Initialize the AkeneoConnector class
+        auth_token = os.getenv('AKENEO_AUTH_TOKEN') if auth_token is None else auth_token
+        if auth_token is None:
+            raise ValueError("auth_token is required")
+        
         self.origin = os.getenv('AKENEO_ORIGIN') if origin is None else origin
         self.username = os.getenv('AKENEO_USERNAME') if username is None else username
         self.password = os.getenv('AKENEO_PASSWORD') if password is None else password
-        self.auth_token = base64.b64encode((os.getenv('AKENEO_AUTH_TOKEN')  if auth_token is None else auth_token).encode()).decode()
+        self.auth_token = base64.b64encode(auth_token.encode()).decode()
         self.auth_url = os.getenv('AKENEO_AUTH_URL') if auth_url is None else auth_url
         self.access_token = self.get_access_token()
         self.headers = {
             'Authorization': 'Bearer ' + self.access_token,
             'Content-type': 'application/vnd.akeneo.collection+json'
         }
         self.version = version
```

### Comparing `akeneo_connector-0.1.3/akeneo_connector/akeneo_paginator.py` & `akeneo_connector-0.1.4/akeneo_connector/akeneo_paginator.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.3/akeneo_connector/akeneo_product.py` & `akeneo_connector-0.1.4/akeneo_connector/akeneo_product.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.3/akeneo_connector.egg-info/PKG-INFO` & `akeneo_connector-0.1.4/akeneo_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.3/setup.py` & `akeneo_connector-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="akeneo_connector",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

