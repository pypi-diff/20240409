# Comparing `tmp/jarpcdantic-0.0.1.tar.gz` & `tmp/jarpcdantic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarpcdantic-0.0.1.tar", last modified: Wed Apr  3 06:53:24 2024, max compression
+gzip compressed data, was "jarpcdantic-0.0.2.tar", last modified: Mon Apr  8 23:42:43 2024, max compression
```

## Comparing `jarpcdantic-0.0.1.tar` & `jarpcdantic-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-03 06:53:24.488667 jarpcdantic-0.0.1/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-03 06:53:24.488667 jarpcdantic-0.0.1/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.1/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-03 06:53:24.488667 jarpcdantic-0.0.1/jarpc/
--rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-03 06:51:06.000000 jarpcdantic-0.0.1/jarpc/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8862 2024-04-03 06:35:31.000000 jarpcdantic-0.0.1/jarpc/client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1191 2024-04-03 01:07:54.000000 jarpcdantic-0.0.1/jarpc/dispatcher.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.1/jarpc/errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-03 06:42:52.000000 jarpcdantic-0.0.1/jarpc/format.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8450 2024-04-03 04:59:02.000000 jarpcdantic-0.0.1/jarpc/manager.py
--rw-r--r--   0 white     (1000) wjite     (1001)     2571 2024-04-03 05:33:09.000000 jarpcdantic-0.0.1/jarpc/router.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-03 06:53:24.488667 jarpcdantic-0.0.1/jarpcdantic.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-03 06:53:24.000000 jarpcdantic-0.0.1/jarpcdantic.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-03 06:53:24.000000 jarpcdantic-0.0.1/jarpcdantic.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-03 06:53:24.000000 jarpcdantic-0.0.1/jarpcdantic.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-03 06:53:24.000000 jarpcdantic-0.0.1/jarpcdantic.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-03 06:53:24.488667 jarpcdantic-0.0.1/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.1/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-03 06:53:24.488667 jarpcdantic-0.0.1/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     7042 2024-04-03 06:42:52.000000 jarpcdantic-0.0.1/tests/test_client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.1/tests/test_errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-03 06:47:24.000000 jarpcdantic-0.0.1/tests/test_format.py
--rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.1/tests/test_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.2/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.508643 jarpcdantic-0.0.2/jarpc/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-08 23:42:30.000000 jarpcdantic-0.0.2/jarpc/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.2/jarpc/client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1519 2024-04-08 23:42:35.000000 jarpcdantic-0.0.2/jarpc/dispatcher.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.2/jarpc/errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.2/jarpc/format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8450 2024-04-03 04:59:02.000000 jarpcdantic-0.0.2/jarpc/manager.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6256 2024-04-08 23:42:35.000000 jarpcdantic-0.0.2/jarpc/router.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/jarpcdantic.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.2/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.2/tests/test_client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.2/tests/test_errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.2/tests/test_format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.2/tests/test_manager.py
```

### Comparing `jarpcdantic-0.0.1/jarpc/__init__.py` & `jarpcdantic-0.0.2/jarpc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "JarpcRequest",
     "JarpcResponse",
     # manager
     "AsyncJarpcManager",
     "JarpcManager",
 )
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

### Comparing `jarpcdantic-0.0.1/jarpc/client.py` & `jarpcdantic-0.0.2/jarpc/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 # -*- coding: utf-8 -*-
 import time
 import uuid
-from typing import Optional, Callable, Any, Union, Awaitable
+from typing import Optional, Callable, Any, Union, Awaitable, Type
 
 from pydantic import ValidationError
 
-from .format import json_loads, json_dumps, JarpcRequest, JarpcResponse, RequestT, ResponseT
-from .errors import raise_exception, JarpcError, JarpcServerError, JarpcParseError, JarpcInvalidRequest
+from .format import (
+    json_loads,
+    json_dumps,
+    JarpcRequest,
+    JarpcResponse,
+    RequestT,
+    ResponseT,
+)
+from .errors import (
+    raise_exception,
+    JarpcError,
+    JarpcServerError,
+    JarpcParseError,
+    JarpcInvalidRequest,
+)
 
 
 class JarpcClient:
     """
     JARPC Client implementation.
 
     To make RPC it requires transport.
@@ -52,15 +65,17 @@
     salad = kitchen.cook_salad(name='Caesar')
     ```
     """
 
     def __init__(
         self,
         # transport: Callable[[str, JarpcRequest, **kwargs], Union[str, None]]
-        transport: Callable[[str, JarpcRequest, Any | None], Awaitable[str | None] | str | None],
+        transport: Callable[
+            [str, JarpcRequest, Any | None], Awaitable[str | None] | str | None
+        ],
         default_ttl: Optional[float] = None,
         default_rpc_ttl: Optional[float] = None,
         default_notification_ttl: Optional[float] = None,
     ):
         """
         :param transport: callable to send request
         :param default_ttl: float time interval while calling still actual
@@ -136,19 +151,26 @@
                 rsvp=rsvp,
             )
         except ValidationError as e:
             raise JarpcInvalidRequest(e) from e
 
         return request
 
-    def _parse_response(self, response_string: str, rsvp: bool, generic_response_type: ResponseT = Any) -> JarpcResponse[ResponseT] | None:
+    def _parse_response(
+        self,
+        response_string: str,
+        rsvp: bool,
+        generic_response_type: Type[ResponseT] = Any,
+    ) -> JarpcResponse[ResponseT] | None:
         """Parse response and either return result or raise JARPC error."""
         if rsvp:
             try:
-                response = JarpcResponse[generic_response_type].model_validate_json(response_string)
+                response = JarpcResponse[generic_response_type].model_validate_json(
+                    response_string
+                )
             except ValidationError as e:
                 raise JarpcServerError(e) from e
             if response.success:
                 return response.result
             else:
                 error = response.error
                 raise_exception(
@@ -213,25 +235,27 @@
         method: str,
         params: RequestT,
         ts: Optional[float] = None,
         ttl: Optional[float] = None,
         request_id: Optional[str] = None,
         rsvp: bool = True,
         durable: bool = False,
-        generic_response_type: ResponseT | None = None,
+        generic_request_type: Type[RequestT] = Any,
+        generic_response_type: Type[ResponseT] = Any,
         **transport_kwargs
     ) -> str:
-        request = self._prepare_request(
+        request: JarpcRequest[RequestT] = self._prepare_request(
             method, params, ts, ttl, request_id, rsvp, durable
         )
         request_string = request.model_dump_json()
 
         try:
             response_string = await self._transport(
                 request_string, request, **transport_kwargs
             )
         except JarpcError:
             raise
         except Exception as e:
             raise JarpcServerError(e)
 
+        response = self._parse_response(response_string, rsvp, generic_response_type)
         return self._parse_response(response_string, rsvp)
```

### Comparing `jarpcdantic-0.0.1/jarpc/dispatcher.py` & `jarpcdantic-0.0.2/jarpc/dispatcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,25 @@
     def rpc_method(self, f):
         """Decorator: adds `f` as RPC method.
         `f` can retrieve JarpcRequest object through optional `jarpc_request` argument.
         """
         self.method_map[f.__name__] = f
         return f
 
+    def declare_method(self, name: str | None = None):
+        """Decorator: adds `f` as RPC method.
+        `f` can retrieve JarpcRequest object through optional `jarpc_request` argument.
+        """
+
+        def decorated(f):
+            self.method_map[name or f.__name__] = f
+            return f
+
+        return decorated
+
     def add_rpc_method(self, f, name=None):
         """Adds `f` as RPC method.
         If `name` is not None, it is used as method name.
         `f` can retrieve JarpcRequest object through optional `jarpc_request` argument.
         """
         self.method_map[name or f.__name__] = f
```

### Comparing `jarpcdantic-0.0.1/jarpc/errors.py` & `jarpcdantic-0.0.2/jarpc/errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.1/jarpc/format.py` & `jarpcdantic-0.0.2/jarpc/format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.1/jarpc/manager.py` & `jarpcdantic-0.0.2/jarpc/manager.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.1/setup.py` & `jarpcdantic-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.1/tests/test_client.py` & `jarpcdantic-0.0.2/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
 
         call_kwargs = dict(
             method="method", params={"param1": 1}, id=request_id, extra_kwarg=1
         )
         call_result = jarpc_client(**call_kwargs)
         assert call_result == response["result"]
 
-
     @pytest.mark.parametrize("is_async", [False, True])
     @pytest.mark.asyncio
     @freeze_time("2012-01-14")
     async def test_call_simple_syntax(self, is_async):
         response = {
             "result": "some result",
             "request_id": "no check",
```

### Comparing `jarpcdantic-0.0.1/tests/test_errors.py` & `jarpcdantic-0.0.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.1/tests/test_format.py` & `jarpcdantic-0.0.2/tests/test_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "method": "get_result",
     "params": {"a": 1, "b": 2},
     "ts": 0.0,
     "ttl": 10.0,
     "id": "429284302",
     "rsvp": True,
 }
-VALID_REQUEST_DATA = {**VALID_REQUEST_KWARGS, 'version': '1.0'}
+VALID_REQUEST_DATA = {**VALID_REQUEST_KWARGS, "version": "1.0"}
 
 
 class TestJarpcRequest:
     @freeze_time("1996-06-06 06:06:06")
     def test_expired(self):
         jarpc_request = JarpcRequest(**VALID_REQUEST_KWARGS)
         jarpc_request.ttl = 1
```

### Comparing `jarpcdantic-0.0.1/tests/test_manager.py` & `jarpcdantic-0.0.2/tests/test_manager.py`

 * *Files identical despite different names*

