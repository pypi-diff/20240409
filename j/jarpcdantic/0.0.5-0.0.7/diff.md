# Comparing `tmp/jarpcdantic-0.0.5.tar.gz` & `tmp/jarpcdantic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarpcdantic-0.0.5.tar", last modified: Tue Apr  9 06:42:36 2024, max compression
+gzip compressed data, was "jarpcdantic-0.0.7.tar", last modified: Tue Apr  9 06:54:46 2024, max compression
```

## Comparing `jarpcdantic-0.0.5.tar` & `jarpcdantic-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.5/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/jarpc/
--rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 06:42:01.000000 jarpcdantic-0.0.5/jarpc/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.5/jarpc/client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.5/jarpc/dispatcher.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.5/jarpc/errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.5/jarpc/format.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8442 2024-04-09 06:42:01.000000 jarpcdantic-0.0.5/jarpc/manager.py
--rw-r--r--   0 white     (1000) wjite     (1001)     6807 2024-04-09 06:41:18.000000 jarpcdantic-0.0.5/jarpc/router.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/jarpcdantic.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.5/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.5/tests/test_client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.5/tests/test_errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.5/tests/test_format.py
--rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.5/tests/test_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.7/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.047507 jarpcdantic-0.0.7/jarpc/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 06:54:38.000000 jarpcdantic-0.0.7/jarpc/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.7/jarpc/client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.7/jarpc/dispatcher.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.7/jarpc/errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.7/jarpc/format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8442 2024-04-09 06:42:01.000000 jarpcdantic-0.0.7/jarpc/manager.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6948 2024-04-09 06:54:20.000000 jarpcdantic-0.0.7/jarpc/router.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/jarpcdantic.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.7/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.7/tests/test_client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.7/tests/test_errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.7/tests/test_format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.7/tests/test_manager.py
```

### Comparing `jarpcdantic-0.0.5/jarpc/__init__.py` & `jarpcdantic-0.0.7/jarpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "JarpcRequest",
     "JarpcResponse",
     # manager
     "AsyncJarpcManager",
     "JarpcManager",
 )
 
-__version__ = "0.0.5"
+__version__ = "0.0.7"
```

### Comparing `jarpcdantic-0.0.5/jarpc/client.py` & `jarpcdantic-0.0.7/jarpc/client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/jarpc/dispatcher.py` & `jarpcdantic-0.0.7/jarpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/jarpc/errors.py` & `jarpcdantic-0.0.7/jarpc/errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/jarpc/format.py` & `jarpcdantic-0.0.7/jarpc/format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/jarpc/manager.py` & `jarpcdantic-0.0.7/jarpc/manager.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/jarpc/router.py` & `jarpcdantic-0.0.7/jarpc/router.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,18 +48,18 @@
             if k not in ["self", "args", "kwargs"] and not k.startswith("_")
         }
 
         model: Type[BaseModel] | None = None
 
         if "_model" in attr_signature.parameters:
             model: Type[BaseModel] = attr_signature.parameters["_model"].default
-        elif len(clear_parameters) == 1:
+        elif len(clear_parameters) == 1 and issubclass(clear_parameters[list(clear_parameters.keys())[0]].annotation, BaseModel):
             parameter = clear_parameters[list(clear_parameters.keys())[0]]
             model = parameter.annotation if parameter.annotation is not _empty else None
-        elif len(clear_parameters) > 1:
+        elif len(clear_parameters) >= 1:
             model = create_model(
                 "DynamicModel",
                 **{
                     k: (
                         Any if v.annotation is _empty else v.annotation,
                         ... if v.default is _empty else v.default,
                     )
@@ -118,15 +118,15 @@
                 for index, value in enumerate(args):
                     args_with_default[
                         list(attr_signature_parameters.items())[index + 1][0]
                     ] = value
                 if issubclass(model, BaseModel):
                     params = model(**(args_with_default | clear_kwargs))
                 else:
-                    params = args_with_default | clear_kwargs
+                    params = {k: v for k, v in (args_with_default | clear_kwargs).items() if v is not _empty}
             else:
                 params = {}
 
             if self._client is not None:
                 await self._client(method=self._prefix + "." if self._prefix else "" + method, params=params, **service_kwargs)
             else:
                 print("client is None, call", self._prefix + "." + method, params)
@@ -166,15 +166,15 @@
             self, name: str, a, age: int = 33, b=44, _model=CustomModel, **kwargs
         ) -> None:
             """
             params=CustomModel(name, a, age, b)
             """
             ...
 
-        async def get_status(self, b=22, **kwargs) -> None:
+        async def get_status(self, b: int = 22, **kwargs) -> None:
             """
             params=22
             """
             ...
 
         async def invalidate(self, data: str, a, **kwargs) -> None:
             """
@@ -192,15 +192,15 @@
             ...
 
     async def main():
         router = MvdRouter(prefix="mvd")
         await router.get_status()
         print("---")
         await router.passport.register("eugene", 1, 33, 55)
-        await router.passport.get_status("eugene")
+        await router.passport.get_status("22")
         await router.passport.invalidate(data="22", a="33")
         await router.passport.test.register("22", a="33")
 
         dispatcher = JarpcDispatcher()
 
         @dispatcher.declare_method(router.passport.test.register)
         async def heh(data: str, a: any):
```

### Comparing `jarpcdantic-0.0.5/setup.py` & `jarpcdantic-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/tests/test_client.py` & `jarpcdantic-0.0.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/tests/test_errors.py` & `jarpcdantic-0.0.7/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/tests/test_format.py` & `jarpcdantic-0.0.7/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.5/tests/test_manager.py` & `jarpcdantic-0.0.7/tests/test_manager.py`

 * *Files identical despite different names*

