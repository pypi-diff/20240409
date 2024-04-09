# Comparing `tmp/frid-0.0.6.tar.gz` & `tmp/frid-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.6.tar", last modified: Mon Apr  8 19:17:54 2024, max compression
+gzip compressed data, was "frid-0.0.7.tar", last modified: Mon Apr  8 22:01:28 2024, max compression
```

## Comparing `frid-0.0.6.tar` & `frid-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 19:17:54.582288 frid-0.0.6/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.6/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 19:17:54.582288 frid-0.0.6/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.6/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 19:17:54.572288 frid-0.0.6/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.6/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24357 2024-04-05 19:29:01.000000 frid-0.0.6/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-04 18:04:22.000000 frid-0.0.6/frid/autils.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.6/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16096 2024-04-08 17:34:14.000000 frid-0.0.6/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.6/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8489 2024-04-06 00:48:32.000000 frid-0.0.6/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.6/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    22617 2024-04-05 19:23:00.000000 frid-0.0.6/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.6/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.6/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2288 2024-04-05 19:32:20.000000 frid-0.0.6/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.6/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 19:17:54.572288 frid-0.0.6/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-08 19:17:54.000000 frid-0.0.6/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-08 19:12:08.000000 frid-0.0.6/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-08 19:17:54.582288 frid-0.0.6/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 22:01:28.912291 frid-0.0.7/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.7/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 22:01:28.912291 frid-0.0.7/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.7/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 22:01:28.912291 frid-0.0.7/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.7/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24357 2024-04-05 19:29:01.000000 frid-0.0.7/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-08 21:10:44.000000 frid-0.0.7/frid/autils.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.7/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16096 2024-04-08 17:34:14.000000 frid-0.0.7/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.7/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8575 2024-04-08 19:51:11.000000 frid-0.0.7/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.7/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    22617 2024-04-05 19:23:00.000000 frid-0.0.7/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.7/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.7/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2351 2024-04-08 20:00:06.000000 frid-0.0.7/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.7/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-08 22:01:28.912291 frid-0.0.7/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-08 22:01:28.000000 frid-0.0.7/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-08 22:01:04.000000 frid-0.0.7/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-08 22:01:28.912291 frid-0.0.7/setup.cfg
```

### Comparing `frid-0.0.6/LICENSE` & `frid-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/PKG-INFO` & `frid-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.6/README.md` & `frid-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/__init__.py` & `frid-0.0.7/frid/__init__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/__main__.py` & `frid-0.0.7/frid/__main__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/autils.py` & `frid-0.0.7/frid/autils.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/chrono.py` & `frid-0.0.7/frid/chrono.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/dumper.py` & `frid-0.0.7/frid/dumper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/errors.py` & `frid-0.0.7/frid/errors.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/guards.py` & `frid-0.0.7/frid/guards.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,21 +122,23 @@
 def as_type(dtype: type[V], data, /, allow_none: bool=False) -> V|None:
     if data is None and allow_none:
         return None
     if not isinstance(data, dtype):
         raise ValueError(f"Expecting type {dtype}, got {type(data).__name__}")
     return data
 @overload
-def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
-                /, allow_none: Literal[False]=False) -> V: ...
+def get_as_type(dtype: type[V], map: StrKeyMap, /, key: str, default: V|None=None,
+                *, allow_none: Literal[False]=False) -> V: ...
 @overload
-def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
-                /, allow_none: Literal[True]|bool) -> V|None: ...
-def get_as_type(dtype: type[V], map: StrKeyMap, key: str, /, allow_none: bool=False) -> V|None:
-    return as_type(dtype, map.get(key), allow_none=allow_none)
+def get_as_type(dtype: type[V], map: StrKeyMap, /, key: str, default: V|None=None,
+                *, allow_none: Literal[True]|bool) -> V|None: ...
+def get_as_type(
+        dtype: type[V], map: StrKeyMap, /, key: str, default=None, *, allow_none: bool=False
+) -> V|None:
+    return as_type(dtype, map.get(key, default), allow_none=allow_none)
 
 def as_key_value_pair(
         data: Sequence[tuple[K,V]]|Mapping[K,V]|Iterable
 ) -> Sequence[tuple[K,V]]:
     """Converts the `data` to a sequence of key value pairs.
     - If the `data` is a map, convert it to a list of pairs.
     - If the `data` is already a sequence, return it as is.
```

### Comparing `frid-0.0.6/frid/helper.py` & `frid-0.0.7/frid/helper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/loader.py` & `frid-0.0.7/frid/loader.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/pretty.py` & `frid-0.0.7/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/strops.py` & `frid-0.0.7/frid/strops.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid/typing.py` & `frid-0.0.7/frid/typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import types
 from abc import ABC, abstractmethod
 from datetime import date as dateonly, time as timeonly, datetime
 from collections.abc import Mapping, Sequence, Set
+from typing import TypeVar
 
 # Quick union types used in many places
 BlobTypes = bytes|bytearray|memoryview
 DateTypes = dateonly|timeonly|datetime   # Note that datetime in Python is deriveed from date
 
 # FRID types follow (Flexibly represented inteactive data)
 
+T = TypeVar('T', bound='FridMixin')
+
 class FridMixin(ABC):
     """The abstract base frid class to be loadable and dumpable.
 
     A frid class needs to implement three methods:
     - A class method `frid_keys()` that returns a list of acceptable keys
       for the class (default includes the class name);
     - A class method `frid_from()` that constructs and object of this class
@@ -25,15 +28,15 @@
     """
     @classmethod
     def frid_keys(cls) -> Sequence[str]:
         """The list of keys that the class provides; the default containing class name only."""
         return [cls.__name__]
 
     @classmethod
-    def frid_from(cls, name: str, *args: 'FridValue', **kwds: 'FridValue') -> 'FridMixin':
+    def frid_from(cls: type[T], name: str, *args: 'FridValue', **kwds: 'FridValue') -> T:
         """Construct an instance with given name and arguments."""
         assert name in cls.frid_keys()
         return cls(*args, **kwds)
 
     @abstractmethod
     def frid_repr(self) -> tuple[str,Sequence['FridValue'],Mapping[str,'FridValue']]:
         """Converts an instance to a triplet of name, a list of positional values,
```

### Comparing `frid-0.0.6/frid/webapp.py` & `frid-0.0.7/frid/webapp.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.6/frid.egg-info/PKG-INFO` & `frid-0.0.7/frid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.6/pyproject.toml` & `frid-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

