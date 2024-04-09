# Comparing `tmp/jarpcdantic-0.0.8.tar.gz` & `tmp/jarpcdantic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarpcdantic-0.0.8.tar", last modified: Tue Apr  9 07:02:33 2024, max compression
+gzip compressed data, was "jarpcdantic-0.0.9.tar", last modified: Tue Apr  9 07:04:12 2024, max compression
```

## Comparing `jarpcdantic-0.0.8.tar` & `jarpcdantic-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.8/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/jarpc/
--rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 07:02:30.000000 jarpcdantic-0.0.8/jarpc/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.8/jarpc/client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.8/jarpc/dispatcher.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.8/jarpc/errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.8/jarpc/format.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8442 2024-04-09 06:42:01.000000 jarpcdantic-0.0.8/jarpc/manager.py
--rw-r--r--   0 white     (1000) wjite     (1001)     6950 2024-04-09 07:02:30.000000 jarpcdantic-0.0.8/jarpc/router.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/jarpcdantic.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.8/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.8/tests/test_client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.8/tests/test_errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.8/tests/test_format.py
--rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.8/tests/test_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:04:12.200279 jarpcdantic-0.0.9/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 07:04:12.200279 jarpcdantic-0.0.9/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.9/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:04:12.200279 jarpcdantic-0.0.9/jarpc/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 07:04:09.000000 jarpcdantic-0.0.9/jarpc/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.9/jarpc/client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.9/jarpc/dispatcher.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.9/jarpc/errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.9/jarpc/format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8420 2024-04-09 07:04:09.000000 jarpcdantic-0.0.9/jarpc/manager.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6950 2024-04-09 07:02:30.000000 jarpcdantic-0.0.9/jarpc/router.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:04:12.200279 jarpcdantic-0.0.9/jarpcdantic.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 07:04:12.000000 jarpcdantic-0.0.9/jarpcdantic.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 07:04:12.000000 jarpcdantic-0.0.9/jarpcdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 07:04:12.000000 jarpcdantic-0.0.9/jarpcdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 07:04:12.000000 jarpcdantic-0.0.9/jarpcdantic.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 07:04:12.200279 jarpcdantic-0.0.9/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.9/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:04:12.200279 jarpcdantic-0.0.9/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.9/tests/test_client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.9/tests/test_errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.9/tests/test_format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.9/tests/test_manager.py
```

### Comparing `jarpcdantic-0.0.8/jarpc/__init__.py` & `jarpcdantic-0.0.9/jarpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "JarpcRequest",
     "JarpcResponse",
     # manager
     "AsyncJarpcManager",
     "JarpcManager",
 )
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `jarpcdantic-0.0.8/jarpc/client.py` & `jarpcdantic-0.0.9/jarpc/client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/jarpc/dispatcher.py` & `jarpcdantic-0.0.9/jarpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/jarpc/errors.py` & `jarpcdantic-0.0.9/jarpc/errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/jarpc/format.py` & `jarpcdantic-0.0.9/jarpc/format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/jarpc/manager.py` & `jarpcdantic-0.0.9/jarpc/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         self.loads = loads
         self.dumps = dumps
 
     def handle(self, request: str) -> Optional[str]:
         """Handle request string, producing either response string or None if no response is required."""
         jarpc_response = self.get_response(request_string=request)
         if jarpc_response is not None:
-            return jarpc_response.serialize(dumps=self.dumps)
+            return jarpc_response.model_dump_json()
 
     def get_response(self, request_string: str) -> Optional[JarpcResponse]:
         """Returns either JarpcResponse or None if no response is required."""
         request_id = None
         rsvp = True
         try:
             request = JarpcRequest.model_validate_json(request_string)
@@ -169,22 +169,22 @@
 
 
 class AsyncJarpcManager(JarpcManager):
     async def handle(self, request: str) -> Optional[str]:
         """Handle request string, producing either response string or None if no response is required."""
         jarpc_response = await self.get_response(request_string=request)
         if jarpc_response is not None:
-            return jarpc_response.serialize(self.dumps)
+            return jarpc_response.model_dump_json()
 
     async def get_response(self, request_string: str) -> Optional[JarpcResponse]:
         """Returns either JarpcResponse or None if no response is required."""
         request_id = None
         rsvp = True
         try:
-            request = JarpcRequest.from_json(request_string, loads=self.loads)
+            request = JarpcRequest.model_validate_json(request_string)
             if request.expired:
                 logger.warning(f"Request arrived too late: {request}")
                 return None
 
             request_id = request.response_id
             rsvp = request.rsvp
```

### Comparing `jarpcdantic-0.0.8/jarpc/router.py` & `jarpcdantic-0.0.9/jarpc/router.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/setup.py` & `jarpcdantic-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/tests/test_client.py` & `jarpcdantic-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/tests/test_errors.py` & `jarpcdantic-0.0.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/tests/test_format.py` & `jarpcdantic-0.0.9/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.8/tests/test_manager.py` & `jarpcdantic-0.0.9/tests/test_manager.py`

 * *Files identical despite different names*

