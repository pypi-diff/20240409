# Comparing `tmp/jarpcdantic-0.0.4.tar.gz` & `tmp/jarpcdantic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarpcdantic-0.0.4.tar", last modified: Tue Apr  9 06:41:22 2024, max compression
+gzip compressed data, was "jarpcdantic-0.0.5.tar", last modified: Tue Apr  9 06:42:36 2024, max compression
```

## Comparing `jarpcdantic-0.0.4.tar` & `jarpcdantic-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:41:22.693979 jarpcdantic-0.0.4/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:41:22.693979 jarpcdantic-0.0.4/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.4/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:41:22.673980 jarpcdantic-0.0.4/jarpc/
--rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 06:41:18.000000 jarpcdantic-0.0.4/jarpc/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.4/jarpc/client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.4/jarpc/dispatcher.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.4/jarpc/errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.4/jarpc/format.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8450 2024-04-03 04:59:02.000000 jarpcdantic-0.0.4/jarpc/manager.py
--rw-r--r--   0 white     (1000) wjite     (1001)     6807 2024-04-09 06:41:18.000000 jarpcdantic-0.0.4/jarpc/router.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:41:22.693979 jarpcdantic-0.0.4/jarpcdantic.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:41:22.000000 jarpcdantic-0.0.4/jarpcdantic.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 06:41:22.000000 jarpcdantic-0.0.4/jarpcdantic.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 06:41:22.000000 jarpcdantic-0.0.4/jarpcdantic.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 06:41:22.000000 jarpcdantic-0.0.4/jarpcdantic.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 06:41:22.693979 jarpcdantic-0.0.4/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.4/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:41:22.693979 jarpcdantic-0.0.4/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.4/tests/test_client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.4/tests/test_errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.4/tests/test_format.py
--rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.4/tests/test_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.5/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/jarpc/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 06:42:01.000000 jarpcdantic-0.0.5/jarpc/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.5/jarpc/client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.5/jarpc/dispatcher.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.5/jarpc/errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.5/jarpc/format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8442 2024-04-09 06:42:01.000000 jarpcdantic-0.0.5/jarpc/manager.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6807 2024-04-09 06:41:18.000000 jarpcdantic-0.0.5/jarpc/router.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/jarpcdantic.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 06:42:36.000000 jarpcdantic-0.0.5/jarpcdantic.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.5/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:42:36.718644 jarpcdantic-0.0.5/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.5/tests/test_client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.5/tests/test_errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.5/tests/test_format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.5/tests/test_manager.py
```

### Comparing `jarpcdantic-0.0.4/jarpc/__init__.py` & `jarpcdantic-0.0.5/jarpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "JarpcRequest",
     "JarpcResponse",
     # manager
     "AsyncJarpcManager",
     "JarpcManager",
 )
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

### Comparing `jarpcdantic-0.0.4/jarpc/client.py` & `jarpcdantic-0.0.5/jarpc/client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/jarpc/dispatcher.py` & `jarpcdantic-0.0.5/jarpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/jarpc/errors.py` & `jarpcdantic-0.0.5/jarpc/errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/jarpc/format.py` & `jarpcdantic-0.0.5/jarpc/format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/jarpc/manager.py` & `jarpcdantic-0.0.5/jarpc/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             return jarpc_response.serialize(dumps=self.dumps)
 
     def get_response(self, request_string: str) -> Optional[JarpcResponse]:
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

### Comparing `jarpcdantic-0.0.4/jarpc/router.py` & `jarpcdantic-0.0.5/jarpc/router.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/setup.py` & `jarpcdantic-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/tests/test_client.py` & `jarpcdantic-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/tests/test_errors.py` & `jarpcdantic-0.0.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/tests/test_format.py` & `jarpcdantic-0.0.5/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.4/tests/test_manager.py` & `jarpcdantic-0.0.5/tests/test_manager.py`

 * *Files identical despite different names*

