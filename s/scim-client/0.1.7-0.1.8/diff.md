# Comparing `tmp/scim_client-0.1.7.tar.gz` & `tmp/scim_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim_client-0.1.7.tar", last modified: Thu Apr  4 07:48:36 2024, max compression
+gzip compressed data, was "scim_client-0.1.8.tar", last modified: Tue Apr  9 07:18:59 2024, max compression
```

## Comparing `scim_client-0.1.7.tar` & `scim_client-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.287819 scim_client-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 07:48:32.000000 scim_client-0.1.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-04 07:48:32.000000 scim_client-0.1.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 07:48:32.000000 scim_client-0.1.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-04 07:48:32.000000 scim_client-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 07:48:32.000000 scim_client-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 07:48:36.287819 scim_client-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-04 07:48:32.000000 scim_client-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.283819 scim_client-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4842 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.283819 scim_client-0.1.7/scim_client/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/scim_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.287819 scim_client-0.1.7/scim_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 07:48:36.287819 scim_client-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-04 07:48:32.000000 scim_client-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.287819 scim_client-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 07:48:32.000000 scim_client-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-04 07:48:32.000000 scim_client-0.1.7/tests/test_scim_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:18:59.061258 scim_client-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 07:18:54.000000 scim_client-0.1.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-09 07:18:54.000000 scim_client-0.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 07:18:54.000000 scim_client-0.1.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 07:18:54.000000 scim_client-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 07:18:54.000000 scim_client-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 07:18:59.061258 scim_client-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 07:18:54.000000 scim_client-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:18:59.057258 scim_client-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4842 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 07:18:54.000000 scim_client-0.1.8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:18:59.061258 scim_client-0.1.8/scim_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/scim_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-09 07:18:54.000000 scim_client-0.1.8/scim_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:18:59.061258 scim_client-0.1.8/scim_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 07:18:59.000000 scim_client-0.1.8/scim_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-09 07:18:59.000000 scim_client-0.1.8/scim_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:18:59.000000 scim_client-0.1.8/scim_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:18:58.000000 scim_client-0.1.8/scim_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 07:18:59.000000 scim_client-0.1.8/scim_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 07:18:59.061258 scim_client-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-09 07:18:54.000000 scim_client-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:18:59.061258 scim_client-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 07:18:54.000000 scim_client-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-09 07:18:54.000000 scim_client-0.1.8/tests/test_scim_client.py
```

### Comparing `scim_client-0.1.7/CONTRIBUTING.rst` & `scim_client-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/LICENSE` & `scim_client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/PKG-INFO` & `scim_client-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim_client
-Version: 0.1.7
+Version: 0.1.8
 Summary: SCIM v2 API client
 Home-page: https://github.com/Aplopio/python-scim-client
 Author: Mitratech Development Team
 Author-email: devs@mitratech.com
 License: MIT license
 Keywords: scim_client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `scim_client-0.1.7/README.rst` & `scim_client-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/docs/Makefile` & `scim_client-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/docs/conf.py` & `scim_client-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/docs/installation.rst` & `scim_client-0.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/docs/make.bat` & `scim_client-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/scim_client/resources.py` & `scim_client-0.1.8/scim_client/resources.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/scim_client/response.py` & `scim_client-0.1.8/scim_client/response.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/scim_client/scim_client.py` & `scim_client-0.1.8/scim_client/scim_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import json
 import logging
 import time
 import urllib.request
-from typing import Dict, List, Optional, Any, Type
+from typing import Dict, Optional, Type
 from urllib.error import HTTPError
 from urllib.parse import urlencode
 from urllib.request import Request
 
 from .resources import User, UserSearch
 from .response import SCIMResponse
 
@@ -31,30 +31,33 @@
     base_url: str
     token: str
     timeout: int
     default_headers: Dict[str, str]
     logger: logging.Logger
     UserCls: Type[User]
     UserSearchCls: Type[UserSearch]
+    verify_ssl: bool
 
     def __init__(
         self,
         base_url: str,
         token: str,
         timeout: int = 30,
         max_retries: int = 3,
         default_headers: Optional[Dict[str, str]] = None,
         logger: Optional[logging.Logger] = None,
+        verify_ssl: bool = True,
     ):
         self.token = token
         self.timeout = timeout
         self.base_url = base_url
         self.default_headers = default_headers if default_headers else {}
         self.logger = logger if logger is not None else logging.getLogger(__name__)
         self.max_retries = max_retries
+        self.verify_ssl = verify_ssl
 
     def search_users(self, q: str, count: int = 20, start_index: int = 0) -> UserSearch:
         """Search or filter users by query."""
 
         scim_response = self._make_request(
             method="GET",
             resource="Users",
@@ -129,15 +132,17 @@
         if query_params is not None:
             url = url + "?" + urlencode(query_params)
 
         retries_left = self.max_retries
         http_error = None
         while retries_left > 0:
             try:
-                request = Request(**request_kwargs, method=method)
+                request = Request(
+                    **request_kwargs, method=method, unverifiable=not self.verify_ssl
+                )
                 with urllib.request.urlopen(request) as resp:
                     if 500 <= resp.status < 600:
                         raise HTTPError(
                             url=url,
                             code=resp.status,
                             msg=f"{resp.status} Server Error",
                             fp=resp,
```

### Comparing `scim_client-0.1.7/scim_client/utils.py` & `scim_client-0.1.8/scim_client/utils.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/scim_client.egg-info/PKG-INFO` & `scim_client-0.1.8/scim_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim_client
-Version: 0.1.7
+Version: 0.1.8
 Summary: SCIM v2 API client
 Home-page: https://github.com/Aplopio/python-scim-client
 Author: Mitratech Development Team
 Author-email: devs@mitratech.com
 License: MIT license
 Keywords: scim_client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `scim_client-0.1.7/scim_client.egg-info/SOURCES.txt` & `scim_client-0.1.8/scim_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/setup.py` & `scim_client-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.7/tests/test_scim_client.py` & `scim_client-0.1.8/tests/test_scim_client.py`

 * *Files identical despite different names*

