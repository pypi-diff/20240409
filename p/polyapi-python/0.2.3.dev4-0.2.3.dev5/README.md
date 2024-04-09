# Comparing `tmp/polyapi-python-0.2.3.dev4.tar.gz` & `tmp/polyapi-python-0.2.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi-python-0.2.3.dev4.tar", last modified: Tue Apr  9 15:47:16 2024, max compression
+gzip compressed data, was "polyapi-python-0.2.3.dev5.tar", last modified: Tue Apr  9 19:29:34 2024, max compression
```

## Comparing `polyapi-python-0.2.3.dev4.tar` & `polyapi-python-0.2.3.dev5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:16.059063 polyapi-python-0.2.3.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 15:47:16.059063 polyapi-python-0.2.3.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:16.055063 polyapi-python-0.2.3.dev4/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:16.059063 polyapi-python-0.2.3.dev4/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 15:47:16.000000 polyapi-python-0.2.3.dev4/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 15:47:16.000000 polyapi-python-0.2.3.dev4/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:47:16.000000 polyapi-python-0.2.3.dev4/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 15:47:16.000000 polyapi-python-0.2.3.dev4/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 15:47:16.000000 polyapi-python-0.2.3.dev4/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:47:16.059063 polyapi-python-0.2.3.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:16.059063 polyapi-python-0.2.3.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 15:47:12.000000 polyapi-python-0.2.3.dev4/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.820026 polyapi-python-0.2.3.dev5/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.820026 polyapi-python-0.2.3.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_variables.py
```

### Comparing `polyapi-python-0.2.3.dev4/LICENSE` & `polyapi-python-0.2.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/PKG-INFO` & `polyapi-python-0.2.3.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev4
+Version: 0.2.3.dev5
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi-python-0.2.3.dev4/README.md` & `polyapi-python-0.2.3.dev5/README.md`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/api.py` & `polyapi-python-0.2.3.dev5/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/auth.py` & `polyapi-python-0.2.3.dev5/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/cli.py` & `polyapi-python-0.2.3.dev5/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/config.py` & `polyapi-python-0.2.3.dev5/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/error_handler.py` & `polyapi-python-0.2.3.dev5/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/execute.py` & `polyapi-python-0.2.3.dev5/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/function_cli.py` & `polyapi-python-0.2.3.dev5/polyapi/function_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import ast
 import argparse
 import json
 import types
 import sys
-from typing import Dict, List, Tuple
+from typing import Dict, List, Mapping, Optional, Tuple
 from typing_extensions import _TypedDictMeta  # type: ignore
 import requests
 from stdlib_list import stdlib_list
 from pydantic import TypeAdapter
 from importlib.metadata import packages_distributions
 from polyapi.generate import get_functions_and_parse, generate_functions
 from polyapi.config import get_api_key_and_url
 from polyapi.constants import PYTHON_TO_JSONSCHEMA_TYPE_MAP
 from polyapi.utils import get_auth_headers, print_green, print_red, print_yellow
 import importlib
 
 
 # these libraries are already installed in the base docker image
 # and shouldnt be included in additional requirements
-BASE_REQUIREMENTS = {"polyapi", "requests", "typing_extensions", "jsonschema-gentypes", "pydantic"}
+BASE_REQUIREMENTS = {"polyapi", "requests", "typing_extensions", "jsonschema-gentypes", "pydantic", "cloudevents"}
 all_stdlib_symbols = stdlib_list('.'.join([str(v) for v in sys.version_info[0:2]]))
 BASE_REQUIREMENTS.update(all_stdlib_symbols)  # dont need to pip install stuff in the python standard library
 
 
 def _get_schemas(code: str) -> List[Dict]:
     schemas = []
     user_code = types.SimpleNamespace()
@@ -100,14 +100,27 @@
     if not expr:
         return "Any", None
     python_type = get_python_type_from_ast(expr)
     json_type = _get_jsonschema_type(python_type)
     return json_type, _get_type_schema(json_type, python_type, schemas)
 
 
+def _get_req_name_if_not_in_base(n: Optional[str], pip_name_lookup: Mapping[str, List[str]]) -> Optional[str]:
+    if not n:
+        return None
+
+    if "." in n:
+        n = n.split(".")[0]
+
+    if n in BASE_REQUIREMENTS:
+        return None
+    else:
+        return pip_name_lookup[n][0]
+
+
 def _parse_code(code: str, function_name: str):
     parsed_args = []
     return_type = None
     return_type_schema = None
     requirements: List[str] = []
 
     schemas = _get_schemas(code)
@@ -117,21 +130,24 @@
     # the pip name and the import name might be different
     # e.g. kube_hunter is the import name, but the pip name is kube-hunter
     # see https://stackoverflow.com/a/75144378
     pip_name_lookup = packages_distributions()
 
     for node in ast.iter_child_nodes(parsed_code):
         if isinstance(node, ast.Import):
+            # TODO maybe handle `import foo.bar` case?
             for name in node.names:
-                if name.name not in BASE_REQUIREMENTS:
-                    requirements.append(name.name)
+                req = _get_req_name_if_not_in_base(name.name, pip_name_lookup)
+                if req:
+                    requirements.append(req)
         elif isinstance(node, ast.ImportFrom):
-            if node.module and node.module not in BASE_REQUIREMENTS:
-                req = pip_name_lookup[node.module][0]
-                requirements.append(req)
+            if node.module:
+                req = _get_req_name_if_not_in_base(node.module, pip_name_lookup)
+                if req:
+                    requirements.append(req)
 
         elif isinstance(node, ast.FunctionDef) and node.name == function_name:
             function_args = [arg for arg in node.args.args]
             for arg in function_args:
                 json_type, type_schema = _get_type(arg.annotation, schemas)
                 json_arg = {
                     "key": arg.arg,
```

### Comparing `polyapi-python-0.2.3.dev4/polyapi/generate.py` & `polyapi-python-0.2.3.dev5/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/schema.py` & `polyapi-python-0.2.3.dev5/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/server.py` & `polyapi-python-0.2.3.dev5/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/typedefs.py` & `polyapi-python-0.2.3.dev5/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/utils.py` & `polyapi-python-0.2.3.dev5/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/variables.py` & `polyapi-python-0.2.3.dev5/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi/webhook.py` & `polyapi-python-0.2.3.dev5/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/polyapi_python.egg-info/PKG-INFO` & `polyapi-python-0.2.3.dev5/polyapi_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev4
+Version: 0.2.3.dev5
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi-python-0.2.3.dev4/polyapi_python.egg-info/SOURCES.txt` & `polyapi-python-0.2.3.dev5/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/pyproject.toml` & `polyapi-python-0.2.3.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.3.dev4"
+version = "0.2.3.dev5"
 description = "The PolyAPI Python Client"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi-python-0.2.3.dev4/tests/test_api.py` & `polyapi-python-0.2.3.dev5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/tests/test_auth.py` & `polyapi-python-0.2.3.dev5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/tests/test_function_cli.py` & `polyapi-python-0.2.3.dev5/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/tests/test_server.py` & `polyapi-python-0.2.3.dev5/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/tests/test_utils.py` & `polyapi-python-0.2.3.dev5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev4/tests/test_variables.py` & `polyapi-python-0.2.3.dev5/tests/test_variables.py`

 * *Files identical despite different names*

