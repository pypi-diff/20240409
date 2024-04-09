# Comparing `tmp/apitally-0.7.1.tar.gz` & `tmp/apitally-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apitally-0.7.1.tar", max compression
+gzip compressed data, was "apitally-0.8.0.tar", max compression
```

## Comparing `apitally-0.7.1.tar` & `apitally-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2024-03-29 13:07:14.099801 apitally-0.7.1/LICENSE
--rw-r--r--   0        0        0     4629 2024-03-29 13:07:14.099801 apitally-0.7.1/README.md
--rw-r--r--   0        0        0       22 2024-03-29 13:07:29.707877 apitally-0.7.1/apitally/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 13:07:14.099801 apitally-0.7.1/apitally/client/__init__.py
--rw-r--r--   0        0        0     4433 2024-03-29 13:07:14.099801 apitally-0.7.1/apitally/client/asyncio.py
--rw-r--r--   0        0        0     8511 2024-03-29 13:07:14.099801 apitally-0.7.1/apitally/client/base.py
--rw-r--r--   0        0        0      507 2024-03-29 13:07:14.099801 apitally-0.7.1/apitally/client/logging.py
--rw-r--r--   0        0        0     4831 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/client/threading.py
--rw-r--r--   0        0        0     1088 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/common.py
--rw-r--r--   0        0        0    12124 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/django.py
--rw-r--r--   0        0        0       82 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/django_ninja.py
--rw-r--r--   0        0        0       82 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/django_rest_framework.py
--rw-r--r--   0        0        0       85 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/fastapi.py
--rw-r--r--   0        0        0     4769 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/flask.py
--rw-r--r--   0        0        0     7171 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/litestar.py
--rw-r--r--   0        0        0        0 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/py.typed
--rw-r--r--   0        0        0     7345 2024-03-29 13:07:14.103801 apitally-0.7.1/apitally/starlette.py
--rw-r--r--   0        0        0     2952 2024-03-29 13:07:29.707877 apitally-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 apitally-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-09 06:59:15.713354 apitally-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4629 2024-04-09 06:59:15.713354 apitally-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 06:59:33.141271 apitally-0.8.0/apitally/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/client/__init__.py
+-rw-r--r--   0        0        0     4433 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/client/asyncio.py
+-rw-r--r--   0        0        0    11351 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/client/base.py
+-rw-r--r--   0        0        0      507 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/client/logging.py
+-rw-r--r--   0        0        0     4831 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/client/threading.py
+-rw-r--r--   0        0        0     1088 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/common.py
+-rw-r--r--   0        0        0    12812 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/django.py
+-rw-r--r--   0        0        0       82 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/django_ninja.py
+-rw-r--r--   0        0        0       82 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/django_rest_framework.py
+-rw-r--r--   0        0        0       85 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/fastapi.py
+-rw-r--r--   0        0        0     5552 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/flask.py
+-rw-r--r--   0        0        0     7978 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/litestar.py
+-rw-r--r--   0        0        0        0 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/py.typed
+-rw-r--r--   0        0        0     7767 2024-04-09 06:59:15.713354 apitally-0.8.0/apitally/starlette.py
+-rw-r--r--   0        0        0     2952 2024-04-09 06:59:33.141271 apitally-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 apitally-0.8.0/PKG-INFO
```

### Comparing `apitally-0.7.1/LICENSE` & `apitally-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apitally-0.7.1/README.md` & `apitally-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `apitally-0.7.1/apitally/client/asyncio.py` & `apitally-0.8.0/apitally/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `apitally-0.7.1/apitally/client/threading.py` & `apitally-0.8.0/apitally/client/threading.py`

 * *Files identical despite different names*

### Comparing `apitally-0.7.1/apitally/common.py` & `apitally-0.8.0/apitally/common.py`

 * *Files identical despite different names*

### Comparing `apitally-0.7.1/apitally/django.py` & `apitally-0.8.0/apitally/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,30 @@
                                 consumer=consumer,
                                 method=request.method,
                                 path=path,
                                 detail=body["detail"],
                             )
                 except Exception:  # pragma: no cover
                     logger.exception("Failed to log validation errors")
+            if response.status_code == 500 and hasattr(request, "unhandled_exception"):
+                try:
+                    self.client.server_error_counter.add_server_error(
+                        consumer=consumer,
+                        method=request.method,
+                        path=path,
+                        exception=getattr(request, "unhandled_exception"),
+                    )
+                except Exception:  # pragma: no cover
+                    logger.exception("Failed to log server error")
         return response
 
+    def process_exception(self, request: HttpRequest, exception: Exception) -> None:
+        setattr(request, "unhandled_exception", exception)
+        return None
+
     def get_path(self, request: HttpRequest) -> Optional[str]:
         if (match := request.resolver_match) is not None:
             try:
                 if self.callbacks and match.func not in self.callbacks:
                     return None
                 if self.drf_endpoint_enumerator is not None:
                     from rest_framework.schemas.generators import is_api_view
```

### Comparing `apitally-0.7.1/apitally/flask.py` & `apitally-0.8.0/apitally/flask.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import time
 from threading import Timer
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple
 
 from flask import Flask, g
+from flask.wrappers import Response
 from werkzeug.datastructures import Headers
 from werkzeug.exceptions import NotFound
 from werkzeug.test import Client
 
 from apitally.client.threading import ApitallyClient
 from apitally.common import get_versions
 
@@ -30,14 +31,15 @@
         app_version: Optional[str] = None,
         openapi_url: Optional[str] = None,
         filter_unhandled_paths: bool = True,
     ) -> None:
         self.app = app
         self.wsgi_app = app.wsgi_app
         self.filter_unhandled_paths = filter_unhandled_paths
+        self.patch_handle_exception()
         self.client = ApitallyClient(client_id=client_id, env=env)
         self.client.start_sync_loop()
         self.delayed_set_app_info(app_version, openapi_url)
 
     def delayed_set_app_info(self, app_version: Optional[str] = None, openapi_url: Optional[str] = None) -> None:
         # Short delay to allow app routes to be registered first
         timer = Timer(1.0, self._delayed_set_app_info, kwargs={"app_version": app_version, "openapi_url": openapi_url})
@@ -64,28 +66,48 @@
                 environ=environ,
                 status_code=status_code,
                 response_time=time.perf_counter() - start_time,
                 response_headers=response_headers,
             )
         return response
 
+    def patch_handle_exception(self) -> None:
+        original_handle_exception = self.app.handle_exception
+
+        def handle_exception(e: Exception) -> Response:
+            g.unhandled_exception = e
+            return original_handle_exception(e)
+
+        self.app.handle_exception = handle_exception  # type: ignore[method-assign]
+
     def add_request(
-        self, environ: WSGIEnvironment, status_code: int, response_time: float, response_headers: Headers
+        self,
+        environ: WSGIEnvironment,
+        status_code: int,
+        response_time: float,
+        response_headers: Headers,
     ) -> None:
         rule, is_handled_path = self.get_rule(environ)
         if is_handled_path or not self.filter_unhandled_paths:
             self.client.request_counter.add_request(
                 consumer=self.get_consumer(),
                 method=environ["REQUEST_METHOD"],
                 path=rule,
                 status_code=status_code,
                 response_time=response_time,
                 request_size=environ.get("CONTENT_LENGTH"),
                 response_size=response_headers.get("Content-Length", type=int),
             )
+            if status_code == 500 and "unhandled_exception" in g:
+                self.client.server_error_counter.add_server_error(
+                    consumer=self.get_consumer(),
+                    method=environ["REQUEST_METHOD"],
+                    path=rule,
+                    exception=g.unhandled_exception,
+                )
 
     def get_rule(self, environ: WSGIEnvironment) -> Tuple[str, bool]:
         url_adapter = self.app.url_map.bind_to_environ(environ)
         try:
             endpoint, _ = url_adapter.match()
             rule = self.app.url_map._rules_by_endpoint[endpoint][0]
             return rule.rule, True
```

### Comparing `apitally-0.7.1/apitally/litestar.py` & `apitally-0.8.0/apitally/litestar.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,35 +28,44 @@
         filter_openapi_paths: bool = True,
         identify_consumer_callback: Optional[Callable[[Request], Optional[str]]] = None,
     ) -> None:
         self.client = ApitallyClient(client_id=client_id, env=env)
         self.app_version = app_version
         self.filter_openapi_paths = filter_openapi_paths
         self.identify_consumer_callback = identify_consumer_callback
-        self.openapi_path: Optional[str] = None
+        self.openapi_path = "/schema"
 
     def on_app_init(self, app_config: AppConfig) -> AppConfig:
         app_config.on_startup.append(self.on_startup)
         app_config.on_shutdown.append(self.client.handle_shutdown)
         app_config.middleware.append(self.middleware_factory)
+        app_config.after_exception.append(self.after_exception)
         return app_config
 
     def on_startup(self, app: Litestar) -> None:
         openapi_config = app.openapi_config or DEFAULT_OPENAPI_CONFIG
-        self.openapi_path = openapi_config.openapi_controller.path
+        if openapi_config.openapi_controller is not None:
+            self.openapi_path = openapi_config.openapi_controller.path
+        elif hasattr(openapi_config, "openapi_router") and openapi_config.openapi_router is not None:
+            self.openapi_path = openapi_config.openapi_router.path
+        elif openapi_config.path is not None:
+            self.openapi_path = openapi_config.path
 
         app_info = {
             "openapi": _get_openapi(app),
             "paths": [route for route in _get_routes(app) if not self.filter_path(route["path"])],
             "versions": get_versions("litestar", app_version=self.app_version),
             "client": "python:litestar",
         }
         self.client.set_app_info(app_info)
         self.client.start_sync_loop()
 
+    def after_exception(self, exception: Exception, scope: Scope) -> None:
+        scope["state"]["exception"] = exception
+
     def middleware_factory(self, app: ASGIApp) -> ASGIApp:
         async def middleware(scope: Scope, receive: Receive, send: Send) -> None:
             if scope["type"] == "http" and scope["method"] != "OPTIONS":
                 request = Request(scope)
                 response_status = 0
                 response_time = 0.0
                 response_headers = Headers()
@@ -130,14 +139,21 @@
                                 "msg": error["message"],
                                 "type": "",
                             }
                             for error in parsed_body["extra"]
                             if "key" in error and "message" in error
                         ],
                     )
+        if response_status == 500 and "exception" in request.state:
+            self.client.server_error_counter.add_server_error(
+                consumer=consumer,
+                method=request.method,
+                path=path,
+                exception=request.state["exception"],
+            )
 
     def get_path(self, request: Request) -> Optional[str]:
         path: List[str] = []
         for layer in request.route_handler.ownership_layers:
             if isinstance(layer, HTTPRouteHandler):
                 if len(layer.paths) == 0:
                     return None  # pragma: no cover
```

### Comparing `apitally-0.7.1/apitally/starlette.py` & `apitally-0.8.0/apitally/starlette.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,27 +60,33 @@
             response = await call_next(request)
         except BaseException as e:
             await self.add_request(
                 request=request,
                 response=None,
                 status_code=HTTP_500_INTERNAL_SERVER_ERROR,
                 response_time=time.perf_counter() - start_time,
+                exception=e,
             )
             raise e from None
         else:
             await self.add_request(
                 request=request,
                 response=response,
                 status_code=response.status_code,
                 response_time=time.perf_counter() - start_time,
             )
         return response
 
     async def add_request(
-        self, request: Request, response: Optional[Response], status_code: int, response_time: float
+        self,
+        request: Request,
+        response: Optional[Response],
+        status_code: int,
+        response_time: float,
+        exception: Optional[BaseException] = None,
     ) -> None:
         path_template, is_handled_path = self.get_path_template(request)
         if is_handled_path or not self.filter_unhandled_paths:
             consumer = self.get_consumer(request)
             self.client.request_counter.add_request(
                 consumer=consumer,
                 method=request.method,
@@ -100,14 +106,21 @@
                     # Log FastAPI / Pydantic validation errors
                     self.client.validation_error_counter.add_validation_errors(
                         consumer=consumer,
                         method=request.method,
                         path=path_template,
                         detail=body["detail"],
                     )
+            if status_code == 500 and exception is not None:
+                self.client.server_error_counter.add_server_error(
+                    consumer=consumer,
+                    method=request.method,
+                    path=path_template,
+                    exception=exception,
+                )
 
     @staticmethod
     async def get_response_json(response: Response) -> Any:
         if hasattr(response, "body"):
             try:
                 return json.loads(response.body)
             except json.JSONDecodeError:  # pragma: no cover
```

### Comparing `apitally-0.7.1/pyproject.toml` & `apitally-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "apitally"
-version = "0.7.1"
+version = "0.8.0"
 description = "API monitoring for REST APIs built with FastAPI, Flask, Django, Starlette and Litestar."
 readme = "README.md"
 authors = ["Apitally <hello@apitally.io>"]
 license = "MIT License"
 homepage = "https://apitally.io"
 documentation = "https://docs.apitally.io"
 repository = "https://github.com/apitally/python-client"
```

### Comparing `apitally-0.7.1/PKG-INFO` & `apitally-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apitally
-Version: 0.7.1
+Version: 0.8.0
 Summary: API monitoring for REST APIs built with FastAPI, Flask, Django, Starlette and Litestar.
 Home-page: https://apitally.io
 License: MIT
 Author: Apitally
 Author-email: hello@apitally.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: apitally Version: 0.7.1 Summary: API monitoring for
+Metadata-Version: 2.1 Name: apitally Version: 0.8.0 Summary: API monitoring for
 REST APIs built with FastAPI, Flask, Django, Starlette and Litestar. Home-page:
 https://apitally.io License: MIT Author: Apitally Author-email:
 hello@apitally.io Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 5 - Production/Stable Classifier: Framework :: Django Classifier: Framework ::
 FastAPI Classifier: Framework :: Flask Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

