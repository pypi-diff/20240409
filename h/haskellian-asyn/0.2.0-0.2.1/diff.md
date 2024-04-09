# Comparing `tmp/haskellian-asyn-0.2.0.tar.gz` & `tmp/haskellian-asyn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-asyn-0.2.0.tar", last modified: Mon Apr  8 18:50:21 2024, max compression
+gzip compressed data, was "haskellian-asyn-0.2.1.tar", last modified: Mon Apr  8 18:54:33 2024, max compression
```

## Comparing `haskellian-asyn-0.2.0.tar` & `haskellian-asyn-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.2.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-08 18:50:14.000000 haskellian-asyn-0.2.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/asyn/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      179 2024-04-08 18:50:05.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/ops.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/awaitables/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      128 2024-04-08 18:49:12.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1659 2024-04-08 18:48:40.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/iterables.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      756 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      567 2024-04-08 18:48:30.000000 haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:50:21.190289 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      564 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-08 18:50:21.000000 haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.2.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-08 18:54:31.000000 haskellian-asyn-0.2.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/asyn/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      195 2024-04-08 18:53:43.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      103 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/awaitables/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-04-08 18:53:36.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2062 2024-04-08 18:53:32.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/iterables.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      756 2024-04-08 18:47:33.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      567 2024-04-08 18:48:30.000000 haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-08 18:54:33.042542 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      268 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      564 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-08 18:54:33.000000 haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/top_level.txt
```

### Comparing `haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/iterables.py` & `haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/iterables.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,30 @@
-from typing import AsyncIterable, Callable, TypeVar, Iterable
+from typing import AsyncIterable, Awaitable, Callable, TypeVar, Iterable
+import os
 import ramda as R
 
 A = TypeVar("A")
 B = TypeVar("B")
 
 @R.curry
 async def map(f: Callable[[A], B], xs: AsyncIterable[A]) -> AsyncIterable[B]:
     async for x in xs:
         yield f(x)
+
+@R.curry
+async def concurrent_map(f: Callable[[A], Awaitable[B]], xs: AsyncIterable[A], num_parallel: int | None = None) -> AsyncIterable[B]:
+  num_parallel = num_parallel or os.cpu_count() or 1
+  coros: list[Awaitable[B]] = []
+  async for x in xs:
+    if len(coros) >= num_parallel:
+      yield await coros.pop(0)
+    coros.append(f(x))
+  for coro in coros:
+    yield await coro
+
         
 async def flatten(xxs: AsyncIterable[Iterable[A]]) -> AsyncIterable[A]:
     async for xs in xxs:
         for x in xs:
             yield x 
 
 async def enumerate(xs: AsyncIterable[A]) -> AsyncIterable[tuple[int, A]]:
```

### Comparing `haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/managed.py` & `haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-0.2.0/src/haskellian/asyn/iterables/prefetching.py` & `haskellian-asyn-0.2.1/src/haskellian/asyn/iterables/prefetching.py`

 * *Files identical despite different names*

### Comparing `haskellian-asyn-0.2.0/src/haskellian_asyn.egg-info/SOURCES.txt` & `haskellian-asyn-0.2.1/src/haskellian_asyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

