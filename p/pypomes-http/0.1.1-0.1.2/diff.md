# Comparing `tmp/pypomes_http-0.1.1.tar.gz` & `tmp/pypomes_http-0.1.2.tar.gz`

## Comparing `pypomes_http-0.1.1.tar` & `pypomes_http-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    12540 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/PKG-INFO
```

### Comparing `pypomes_http-0.1.1/src/pypomes_http/__init__.py` & `pypomes_http-0.1.2/src/pypomes_http/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 )
 from .http_pomes import (
     HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_code, http_status_name, http_status_description,
-    http_get_parameters, http_delete, http_get, http_post, http_put,
+    http_delete, http_get, http_post, http_put,
+    http_get_parameter, http_get_parameters,
 )
 
 __all__ = [
     # http_async
     "HttpAsync",
     # http_pomes
     "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
     "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
     "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
     "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
     "http_status_code", "http_status_name", "http_status_description",
-    "http_get_parameters", "http_delete", "http_get", "http_post", "http_put",
+    "http_delete", "http_get", "http_post", "http_put",
+    "http_get_parameter", "http_get_parameters",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_http")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_http-0.1.1/src/pypomes_http/http_async.py` & `pypomes_http-0.1.2/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.1/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.2/src/pypomes_http/http_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import requests
 import sys
 from flask import Request
 from pypomes_core import APP_PREFIX, env_get_int, exc_format
 from pypomes_security import access_get_token
 from requests import Response
-from typing import Final
+from typing import Any, Final
 
 from .http_statuses import _HTTP_STATUSES
 
 HTTP_DELETE_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_DELETE_TIMEOUT", 300)
 HTTP_GET_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_GET_TIMEOUT", 300)
 HTTP_POST_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_POST_TIMEOUT", 300)
 HTTP_PUT_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_PUT_TIMEOUT", 300)
@@ -67,32 +67,71 @@
     :param lang: optional language ('en' or 'pt' - defaults to 'en')
     :return: the corresponding HTTP status description, in the given language
     """
     item: dict = _HTTP_STATUSES.get(status_code)
     return (item or {"en": "Unknown status code", "pt": "Status desconhecido"}).get(lang)
 
 
+def http_get_parameter(request: Request, param: str) -> Any:
+    """
+    Obtain the *request*'s input parameter name *param_name*.
+
+    Until *param* is found, the following are sequentially attempted:
+        - elements in a HTML form
+        - parameters in the URL's query part
+        - key/value pairs in a *JSON* structure in the request's body
+
+    :param request: the Request object
+    :param param: name of parameter to retrieve
+    :return: the parameter's value, or 'None' if not found
+    """
+    # initialize the return variable
+    result: Any = None
+
+    # look for parameter in form
+    params: dict = request.form
+    if params:
+        result = params.get(param)
+
+    # was it found ?
+    if result is None:
+        # no, look for parameter in the URL query
+        # ruff: noqa: PD011
+        params = request.values
+        if params:
+            result = params.get(param)
+
+            # still not found, and the request's content type is JSON ?
+            if result is None and request.mimetype == MIMETYPE_JSON:
+                # yes, look for parameter in the request's body
+                params: dict = request.get_json()
+                if params:
+                    result = params.get(param)
+
+    return result
+
+
 def http_get_parameters(request: Request) -> dict:
     """
     Obtain the *request*'s input parameters.
 
-    The following are attempted in sequence as input parameters:
+    The following are cumulatively attempted, in sequence:
         - key/value pairs in a *JSON* structure in the request's body
         - parameters in the URL's query part
         - elements in a HTML form
 
     :param request: the Request object
     :return: dict containing the input parameters (empty, if no input data exist)
     """
-    # declare the return variable
+    # initialize the return variable
     result: dict = {}
 
     # is JSON the content type of the request ?
     if request.mimetype == MIMETYPE_JSON:
-        # yes, retrieve it
+        # yes, retrieve the JSON data
         result.update(request.get_json())
 
     # obtain parameters in URL query
     result.update(request.values)  # noqa (bug: Ruff reports PD011)
 
     # obtain parameters in form
     result.update(request.form)
```

### Comparing `pypomes_http-0.1.1/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.2/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.1/LICENSE` & `pypomes_http-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.1/pyproject.toml` & `pypomes_http-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.7.3",
+    "pypomes_core>=0.8.3",
     "pypomes_security>=0.1.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_http-0.1.1/PKG-INFO` & `pypomes_http-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.7.3
+Requires-Dist: pypomes-core>=0.8.3
 Requires-Dist: pypomes-security>=0.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

