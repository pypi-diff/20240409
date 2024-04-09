# Comparing `tmp/jarpcdantic-0.0.2.tar.gz` & `tmp/jarpcdantic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarpcdantic-0.0.2.tar", last modified: Mon Apr  8 23:42:43 2024, max compression
+gzip compressed data, was "jarpcdantic-0.0.3.tar", last modified: Tue Apr  9 04:48:22 2024, max compression
```

## Comparing `jarpcdantic-0.0.2.tar` & `jarpcdantic-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.2/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.508643 jarpcdantic-0.0.2/jarpc/
--rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-08 23:42:30.000000 jarpcdantic-0.0.2/jarpc/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.2/jarpc/client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1519 2024-04-08 23:42:35.000000 jarpcdantic-0.0.2/jarpc/dispatcher.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.2/jarpc/errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.2/jarpc/format.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8450 2024-04-03 04:59:02.000000 jarpcdantic-0.0.2/jarpc/manager.py
--rw-r--r--   0 white     (1000) wjite     (1001)     6256 2024-04-08 23:42:35.000000 jarpcdantic-0.0.2/jarpc/router.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/jarpcdantic.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-08 23:42:43.000000 jarpcdantic-0.0.2/jarpcdantic.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.2/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-08 23:42:43.511977 jarpcdantic-0.0.2/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.2/tests/test_client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.2/tests/test_errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.2/tests/test_format.py
--rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.2/tests/test_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 04:48:22.827259 jarpcdantic-0.0.3/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 04:48:22.827259 jarpcdantic-0.0.3/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.3/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 04:48:22.823926 jarpcdantic-0.0.3/jarpc/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 04:48:04.000000 jarpcdantic-0.0.3/jarpc/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.3/jarpc/client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.3/jarpc/dispatcher.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.3/jarpc/errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.3/jarpc/format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8450 2024-04-03 04:59:02.000000 jarpcdantic-0.0.3/jarpc/manager.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6788 2024-04-09 04:26:07.000000 jarpcdantic-0.0.3/jarpc/router.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 04:48:22.827259 jarpcdantic-0.0.3/jarpcdantic.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 04:48:22.000000 jarpcdantic-0.0.3/jarpcdantic.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 04:48:22.000000 jarpcdantic-0.0.3/jarpcdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 04:48:22.000000 jarpcdantic-0.0.3/jarpcdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 04:48:22.000000 jarpcdantic-0.0.3/jarpcdantic.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 04:48:22.827259 jarpcdantic-0.0.3/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.3/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 04:48:22.827259 jarpcdantic-0.0.3/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.3/tests/test_client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.3/tests/test_errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.3/tests/test_format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.3/tests/test_manager.py
```

### Comparing `jarpcdantic-0.0.2/jarpc/__init__.py` & `jarpcdantic-0.0.3/jarpc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "JarpcRequest",
     "JarpcResponse",
     # manager
     "AsyncJarpcManager",
     "JarpcManager",
 )
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

### Comparing `jarpcdantic-0.0.2/jarpc/client.py` & `jarpcdantic-0.0.3/jarpc/client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/jarpc/dispatcher.py` & `jarpcdantic-0.0.3/jarpc/dispatcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def declare_method(self, name: str | None = None):
         """Decorator: adds `f` as RPC method.
         `f` can retrieve JarpcRequest object through optional `jarpc_request` argument.
         """
 
         def decorated(f):
-            self.method_map[name or f.__name__] = f
+            self.method_map[(name.__str__() if name else None) or f.__name__] = f
             return f
 
         return decorated
 
     def add_rpc_method(self, f, name=None):
         """Adds `f` as RPC method.
         If `name` is not None, it is used as method name.
```

### Comparing `jarpcdantic-0.0.2/jarpc/errors.py` & `jarpcdantic-0.0.3/jarpc/errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/jarpc/format.py` & `jarpcdantic-0.0.3/jarpc/format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/jarpc/manager.py` & `jarpcdantic-0.0.3/jarpc/manager.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/jarpc/router.py` & `jarpcdantic-0.0.3/jarpc/router.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from inspect import _empty
 from typing import Any, Type, OrderedDict
 
 from pydantic import create_model, BaseModel
 
-from jarpc import JarpcClient, AsyncJarpcClient
+from jarpc import JarpcClient, AsyncJarpcClient, JarpcDispatcher
 
 
 class JarpcClientRouter:
     def __init__(
         self,
         prefix: str | None = None,
         client: AsyncJarpcClient | JarpcClient | None = None,
@@ -17,24 +17,25 @@
         self._client: AsyncJarpcClient | JarpcClient | None = client
         self._prefix: str | None = prefix
         self._is_absolute_prefix: bool = is_absolute_prefix
         self._method_map: dict = {}
 
         self._decorate_methods()
 
-    def _decorate_methods(self):
+    def _decorate_methods(self, is_nested: bool = False):
         for attr_name, attr_value in self.__class__.__dict__.items():
             if attr_name.startswith("_") or isinstance(attr_value, property):
                 continue
 
             if isinstance(attr_value, JarpcClientRouter):
                 self._proceed_nested_router(attr_name, attr_value)
 
             if (
-                not attr_name.startswith("_")
+                not is_nested
+                and not attr_name.startswith("_")
                 and hasattr(attr_value, "__annotations__")
                 and "return" in attr_value.__annotations__
             ):
                 self._proceed_endpoint(attr_name, attr_value)
 
     def _proceed_endpoint(self, endpoint_name, endpoint_method):
         attr_signature = inspect.signature(endpoint_method)
@@ -92,14 +93,17 @@
                 + ("." if prefix and nested_router._prefix else "")
                 + nested_router._prefix
             )
 
         if nested_router._client is None and self._client is not None:
             nested_router._client = self._client
 
+        nested_router._decorate_methods(is_nested=True)
+
+
     @staticmethod
     def _wrap(
         self,
         method: str,
         model: Type[BaseModel] | None,
         attr_signature_parameters: OrderedDict,
     ):
@@ -121,15 +125,21 @@
                     params = [*args, *kwargs.values()][0]
             else:
                 params = None
 
             if self._client is not None:
                 await self._client(method=method, params=params, **service_kwargs)
             else:
-                print("client is None, call", method, params)
+                print("client is None, call", self._prefix + "." + method, params)
+
+        def __str__(*args, **kwargs) -> str:
+            return self._prefix + "." + method
+
+        wrapped.__str__ = __str__
+        wrapped.__repr__ = __str__
 
         return wrapped
 
 
 class CustomModel(BaseModel):
     name: str
     a: Any
@@ -186,8 +196,16 @@
         await router.get_status()
         print("---")
         await router.passport.register("eugene", 1, 33, 55)
         await router.passport.get_status("eugene")
         await router.passport.invalidate(data="22", a="33")
         await router.passport.test.register("22", a="33")
 
+        dispatcher = JarpcDispatcher()
+
+        @dispatcher.declare_method(router.passport.test.register)
+        async def heh(data: str, a: any):
+            print(data, a)
+
+        print(dispatcher.method_map)
+
     asyncio.run(main())
```

### Comparing `jarpcdantic-0.0.2/setup.py` & `jarpcdantic-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/tests/test_client.py` & `jarpcdantic-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/tests/test_errors.py` & `jarpcdantic-0.0.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/tests/test_format.py` & `jarpcdantic-0.0.3/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.2/tests/test_manager.py` & `jarpcdantic-0.0.3/tests/test_manager.py`

 * *Files identical despite different names*

