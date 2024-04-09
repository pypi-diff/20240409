# Comparing `tmp/jarpcdantic-0.0.7.tar.gz` & `tmp/jarpcdantic-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarpcdantic-0.0.7.tar", last modified: Tue Apr  9 06:54:46 2024, max compression
+gzip compressed data, was "jarpcdantic-0.0.8.tar", last modified: Tue Apr  9 07:02:33 2024, max compression
```

## Comparing `jarpcdantic-0.0.7.tar` & `jarpcdantic-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.7/README.md
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.047507 jarpcdantic-0.0.7/jarpc/
--rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 06:54:38.000000 jarpcdantic-0.0.7/jarpc/__init__.py
--rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.7/jarpc/client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.7/jarpc/dispatcher.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.7/jarpc/errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.7/jarpc/format.py
--rw-r--r--   0 white     (1000) wjite     (1001)     8442 2024-04-09 06:42:01.000000 jarpcdantic-0.0.7/jarpc/manager.py
--rw-r--r--   0 white     (1000) wjite     (1001)     6948 2024-04-09 06:54:20.000000 jarpcdantic-0.0.7/jarpc/router.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/jarpcdantic.egg-info/
--rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 06:54:46.000000 jarpcdantic-0.0.7/jarpcdantic.egg-info/top_level.txt
--rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/setup.cfg
--rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.7/setup.py
-drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 06:54:46.050840 jarpcdantic-0.0.7/tests/
--rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.7/tests/test_client.py
--rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.7/tests/test_errors.py
--rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.7/tests/test_format.py
--rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.7/tests/test_manager.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)       30 2024-04-03 01:04:51.000000 jarpcdantic-0.0.8/README.md
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/jarpc/
+-rw-r--r--   0 white     (1000) wjite     (1001)     1177 2024-04-09 07:02:30.000000 jarpcdantic-0.0.8/jarpc/__init__.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     9187 2024-04-08 04:09:44.000000 jarpcdantic-0.0.8/jarpc/client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1549 2024-04-09 04:17:03.000000 jarpcdantic-0.0.8/jarpc/dispatcher.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3527 2024-04-03 01:07:54.000000 jarpcdantic-0.0.8/jarpc/errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1733 2024-04-04 03:49:54.000000 jarpcdantic-0.0.8/jarpc/format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     8442 2024-04-09 06:42:01.000000 jarpcdantic-0.0.8/jarpc/manager.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     6950 2024-04-09 07:02:30.000000 jarpcdantic-0.0.8/jarpc/router.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/jarpcdantic.egg-info/
+-rw-r--r--   0 white     (1000) wjite     (1001)      271 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) wjite     (1001)      372 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        1 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)        6 2024-04-09 07:02:33.000000 jarpcdantic-0.0.8/jarpcdantic.egg-info/top_level.txt
+-rw-r--r--   0 white     (1000) wjite     (1001)      100 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/setup.cfg
+-rw-r--r--   0 white     (1000) wjite     (1001)      753 2024-04-03 06:53:06.000000 jarpcdantic-0.0.8/setup.py
+drwxr-xr-x   0 white     (1000) wjite     (1001)        0 2024-04-09 07:02:33.404169 jarpcdantic-0.0.8/tests/
+-rw-r--r--   0 white     (1000) wjite     (1001)     7041 2024-04-04 06:06:48.000000 jarpcdantic-0.0.8/tests/test_client.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     1641 2024-04-03 05:48:50.000000 jarpcdantic-0.0.8/tests/test_errors.py
+-rw-r--r--   0 white     (1000) wjite     (1001)     3366 2024-04-04 06:06:48.000000 jarpcdantic-0.0.8/tests/test_format.py
+-rw-r--r--   0 white     (1000) wjite     (1001)    20349 2024-04-03 05:48:50.000000 jarpcdantic-0.0.8/tests/test_manager.py
```

### Comparing `jarpcdantic-0.0.7/jarpc/__init__.py` & `jarpcdantic-0.0.8/jarpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     "JarpcRequest",
     "JarpcResponse",
     # manager
     "AsyncJarpcManager",
     "JarpcManager",
 )
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

### Comparing `jarpcdantic-0.0.7/jarpc/client.py` & `jarpcdantic-0.0.8/jarpc/client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/jarpc/dispatcher.py` & `jarpcdantic-0.0.8/jarpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/jarpc/errors.py` & `jarpcdantic-0.0.8/jarpc/errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/jarpc/format.py` & `jarpcdantic-0.0.8/jarpc/format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/jarpc/manager.py` & `jarpcdantic-0.0.8/jarpc/manager.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/jarpc/router.py` & `jarpcdantic-0.0.8/jarpc/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                     params = model(**(args_with_default | clear_kwargs))
                 else:
                     params = {k: v for k, v in (args_with_default | clear_kwargs).items() if v is not _empty}
             else:
                 params = {}
 
             if self._client is not None:
-                await self._client(method=self._prefix + "." if self._prefix else "" + method, params=params, **service_kwargs)
+                await self._client(method=self._prefix + ("." if self._prefix else "") + method, params=params, **service_kwargs)
             else:
                 print("client is None, call", self._prefix + "." + method, params)
 
         def __str__(*args, **kwargs) -> str:
             return self._prefix + "." + method
 
         wrapped.__str__ = __str__
```

### Comparing `jarpcdantic-0.0.7/setup.py` & `jarpcdantic-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/tests/test_client.py` & `jarpcdantic-0.0.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/tests/test_errors.py` & `jarpcdantic-0.0.8/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/tests/test_format.py` & `jarpcdantic-0.0.8/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `jarpcdantic-0.0.7/tests/test_manager.py` & `jarpcdantic-0.0.8/tests/test_manager.py`

 * *Files identical despite different names*

