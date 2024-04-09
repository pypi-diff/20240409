# Comparing `tmp/polyapi-python-0.2.3.dev2.tar.gz` & `tmp/polyapi-python-0.2.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi-python-0.2.3.dev2.tar", last modified: Tue Apr  9 15:04:50 2024, max compression
+gzip compressed data, was "polyapi-python-0.2.3.dev3.tar", last modified: Tue Apr  9 15:44:38 2024, max compression
```

## Comparing `polyapi-python-0.2.3.dev2.tar` & `polyapi-python-0.2.3.dev3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:50.610627 polyapi-python-0.2.3.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 15:04:50.610627 polyapi-python-0.2.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:50.606626 polyapi-python-0.2.3.dev2/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:50.606626 polyapi-python-0.2.3.dev2/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 15:04:50.000000 polyapi-python-0.2.3.dev2/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 15:04:50.000000 polyapi-python-0.2.3.dev2/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:04:50.000000 polyapi-python-0.2.3.dev2/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 15:04:50.000000 polyapi-python-0.2.3.dev2/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 15:04:50.000000 polyapi-python-0.2.3.dev2/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:04:50.610627 polyapi-python-0.2.3.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:04:50.606626 polyapi-python-0.2.3.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 15:04:45.000000 polyapi-python-0.2.3.dev2/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:44:38.811116 polyapi-python-0.2.3.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 15:44:38.811116 polyapi-python-0.2.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:44:38.811116 polyapi-python-0.2.3.dev3/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:44:38.811116 polyapi-python-0.2.3.dev3/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 15:44:38.000000 polyapi-python-0.2.3.dev3/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 15:44:38.000000 polyapi-python-0.2.3.dev3/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:44:38.000000 polyapi-python-0.2.3.dev3/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 15:44:38.000000 polyapi-python-0.2.3.dev3/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 15:44:38.000000 polyapi-python-0.2.3.dev3/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:44:38.811116 polyapi-python-0.2.3.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:44:38.811116 polyapi-python-0.2.3.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 15:44:31.000000 polyapi-python-0.2.3.dev3/tests/test_variables.py
```

### Comparing `polyapi-python-0.2.3.dev2/LICENSE` & `polyapi-python-0.2.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/PKG-INFO` & `polyapi-python-0.2.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev2
+Version: 0.2.3.dev3
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,15 @@
 Project-URL: Homepage, https://github.com/polyapi/polyapi-python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: jsonschema-gentypes==2.4.0
-Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic==2.5.3
 Requires-Dist: stdlib_list==0.10.0
 Requires-Dist: colorama==0.4.4
 Requires-Dist: python-socketio[asyncio_client]==5.11.1
 Requires-Dist: truststore==0.8.0
 
 # PolyAPI Python Library
```

### Comparing `polyapi-python-0.2.3.dev2/README.md` & `polyapi-python-0.2.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/api.py` & `polyapi-python-0.2.3.dev3/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/auth.py` & `polyapi-python-0.2.3.dev3/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/cli.py` & `polyapi-python-0.2.3.dev3/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/config.py` & `polyapi-python-0.2.3.dev3/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/error_handler.py` & `polyapi-python-0.2.3.dev3/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/execute.py` & `polyapi-python-0.2.3.dev3/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/function_cli.py` & `polyapi-python-0.2.3.dev3/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/generate.py` & `polyapi-python-0.2.3.dev3/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/schema.py` & `polyapi-python-0.2.3.dev3/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/server.py` & `polyapi-python-0.2.3.dev3/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/typedefs.py` & `polyapi-python-0.2.3.dev3/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/utils.py` & `polyapi-python-0.2.3.dev3/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/variables.py` & `polyapi-python-0.2.3.dev3/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi/webhook.py` & `polyapi-python-0.2.3.dev3/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/polyapi_python.egg-info/PKG-INFO` & `polyapi-python-0.2.3.dev3/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev2
+Version: 0.2.3.dev3
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,15 @@
 Project-URL: Homepage, https://github.com/polyapi/polyapi-python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: jsonschema-gentypes==2.4.0
-Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic==2.5.3
 Requires-Dist: stdlib_list==0.10.0
 Requires-Dist: colorama==0.4.4
 Requires-Dist: python-socketio[asyncio_client]==5.11.1
 Requires-Dist: truststore==0.8.0
 
 # PolyAPI Python Library
```

### Comparing `polyapi-python-0.2.3.dev2/polyapi_python.egg-info/SOURCES.txt` & `polyapi-python-0.2.3.dev3/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/pyproject.toml` & `polyapi-python-0.2.3.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.3.dev2"
+version = "0.2.3.dev3"
 description = "The PolyAPI Python Client"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
-    "pydantic==2.6.4",
+    "pydantic==2.5.3",
     "stdlib_list==0.10.0",
     "colorama==0.4.4",
     "python-socketio[asyncio_client]==5.11.1",
     "truststore==0.8.0",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `polyapi-python-0.2.3.dev2/tests/test_api.py` & `polyapi-python-0.2.3.dev3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/tests/test_auth.py` & `polyapi-python-0.2.3.dev3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/tests/test_function_cli.py` & `polyapi-python-0.2.3.dev3/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/tests/test_server.py` & `polyapi-python-0.2.3.dev3/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/tests/test_utils.py` & `polyapi-python-0.2.3.dev3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev2/tests/test_variables.py` & `polyapi-python-0.2.3.dev3/tests/test_variables.py`

 * *Files identical despite different names*

