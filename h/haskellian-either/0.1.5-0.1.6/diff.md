# Comparing `tmp/haskellian-either-0.1.5.tar.gz` & `tmp/haskellian-either-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-either-0.1.5.tar", last modified: Mon Apr  8 10:51:53 2024, max compression
+gzip compressed data, was "haskellian-either-0.1.6.tar", last modified: Tue Apr  9 15:05:50 2024, max compression
```

## Comparing `haskellian-either-0.1.5.tar` & `haskellian-either-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-08 10:51:50.000000 haskellian-either-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.309388 haskellian-either-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.309388 haskellian-either-0.1.5/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-04-05 17:36:56.000000 haskellian-either-0.1.5/src/haskellian/either/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/src/haskellian/either/extras/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian-either-0.1.5/src/haskellian/either/extras/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian-either-0.1.5/src/haskellian/either/extras/pydantic.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-04-08 10:51:36.000000 haskellian-either-0.1.5/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      294 2024-04-08 10:48:52.000000 haskellian-either-0.1.5/src/haskellian/either/narrowing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1942 2024-04-08 10:51:32.000000 haskellian-either-0.1.5/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 10:51:53.319388 haskellian-either-0.1.5/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-08 10:51:53.000000 haskellian-either-0.1.5/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.930682 haskellian-either-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-09 15:05:50.930682 haskellian-either-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-09 15:05:48.000000 haskellian-either-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 15:05:50.930682 haskellian-either-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-04-05 17:36:56.000000 haskellian-either-0.1.6/src/haskellian/either/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian/either/extras/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian-either-0.1.6/src/haskellian/either/extras/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian-either-0.1.6/src/haskellian/either/extras/pydantic.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-04-08 10:51:36.000000 haskellian-either-0.1.6/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-04-08 13:18:48.000000 haskellian-either-0.1.6/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2082 2024-04-09 09:12:43.000000 haskellian-either-0.1.6/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/top_level.txt
```

### Comparing `haskellian-either-0.1.5/pyproject.toml` & `haskellian-either-0.1.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-either"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple Either type"
 dependencies = []
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `haskellian-either-0.1.5/src/haskellian/either/funcs.py` & `haskellian-either-0.1.6/src/haskellian/either/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-either-0.1.5/src/haskellian/either/type.py` & `haskellian-either-0.1.6/src/haskellian/either/type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from typing import Generic, TypeVar, Literal, Callable, Any, TypeGuard
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
-A = TypeVar('A')
+A = TypeVar('A', covariant=True)
 L = TypeVar('L', covariant=True)
 R = TypeVar('R', covariant=True)
 L2 = TypeVar('L2')
 R2 = TypeVar('R2')
 
 @dataclass(eq=False)
 class IsLeft(BaseException, Generic[L]):
   value: L
 
 class EitherBase(ABC, Generic[L, R]):
 
   @abstractmethod
+  def _match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> int:
+    """Unwrap an `Either` by matching both branches"""
+  
   def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
     """Unwrap an `Either` by matching both branches"""
+    return self._match(on_left, on_right)
 
   @abstractmethod
   def unsafe(self) -> R:
     """Unwraps the value or throws an `IsLeft` exception
     
     (`IsLeft.value` will contain the wrapped value)"""
     
@@ -42,29 +46,29 @@
   """Alias of `bind`"""
   
   def match_(self, on_left: Callable[[], A], on_right: Callable[[], A]) -> A:
     """Like `match`, but handlers don't get the wrapped value"""
     return self.match(lambda _: on_left(), lambda _: on_right())
   
 @dataclass
-class Left(EitherBase[L, Any], Generic[L]):
-  value: L
+class Left(EitherBase[L, R], Generic[L, R]):
+  value: L = None
   tag: Literal['left'] = 'left'
 
-  def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
+  def _match(self, on_left, on_right):
     return on_left(self.value)
   
   def unsafe(self):
     raise IsLeft(self.value)
 
 @dataclass
-class Right(EitherBase[Any, R], Generic[R]):
-  value: R
+class Right(EitherBase[L, R], Generic[L, R]):
+  value: R = None
   tag: Literal['right'] = 'right'
 
-  def match(self, on_left: Callable[[L], A], on_right: Callable[[R], A]) -> A:
+  def _match(self, on_left, on_right):
     return on_right(self.value)
   
   def unsafe(self) -> R:
     return self.value
 
-Either = Left[L] | Right[R]
+Either = Left[L, R] | Right[L, R]
```

