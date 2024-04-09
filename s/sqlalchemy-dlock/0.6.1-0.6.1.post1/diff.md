# Comparing `tmp/sqlalchemy-dlock-0.6.1.tar.gz` & `tmp/sqlalchemy-dlock-0.6.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-dlock-0.6.1.tar", last modified: Sat Apr  6 15:24:39 2024, max compression
+gzip compressed data, was "sqlalchemy-dlock-0.6.1.post1.tar", last modified: Tue Apr  9 11:22:32 2024, max compression
```

## Comparing `sqlalchemy-dlock-0.6.1.tar` & `sqlalchemy-dlock-0.6.1.post1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.416332 sqlalchemy-dlock-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:24:39.416332 sqlalchemy-dlock-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.404332 sqlalchemy-dlock-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.408332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_sa_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_sa_types_backward.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.408332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/_sa_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.953820 sqlalchemy-dlock-0.6.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-09 11:22:32.953820 sqlalchemy-dlock-0.6.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:22:32.953820 sqlalchemy-dlock-0.6.1.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.945820 sqlalchemy-dlock-0.6.1.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.949820 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/_sa_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/_sa_types_backward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:22:32.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.949820 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/_sa_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.949820 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.949820 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.949820 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/statement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/statement/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/statement/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 11:22:21.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:22:32.949820 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-09 11:22:32.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-09 11:22:32.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:22:32.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 11:22:32.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 11:22:32.000000 sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/top_level.txt
```

### Comparing `sqlalchemy-dlock-0.6.1/CHANGELOG.md` & `sqlalchemy-dlock-0.6.1.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/LICENSE` & `sqlalchemy-dlock-0.6.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/PKG-INFO` & `sqlalchemy-dlock-0.6.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.6.1
+Version: 0.6.1.post1
 Summary: A distributed lock implementation based on SQLAlchemy
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
 Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
 Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
 Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
```

### Comparing `sqlalchemy-dlock-0.6.1/README.md` & `sqlalchemy-dlock-0.6.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/pyproject.toml` & `sqlalchemy-dlock-0.6.1.post1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -76,11 +76,9 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 write_to = "src/sqlalchemy_dlock/_version.py"
 
-[tool.black]
-line-length = 128
-[tool.isort]
-profile = "black"
+[tool.setuptools.package-data]
+sqlalchemy_dlock = ["sqlalchemy_dlock/py.typed"]
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_sa_types_backward.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/_sa_types_backward.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/factory.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from ..utils import pascal_case, safe_name
 from .lock.base import BaseAsyncSadLock, TAsyncConnectionOrSession
 
 __all__ = ["create_async_sadlock"]
 
 
 def create_async_sadlock(
-    connection_or_session: TAsyncConnectionOrSession, key, contextual_timeout: Union[float, int, None] = None, **kwargs
+    connection_or_session: TAsyncConnectionOrSession,
+    key,
+    contextual_timeout: Union[float, int, None] = None,
+    **kwargs,
 ) -> BaseAsyncSadLock:
     if isinstance(connection_or_session, AsyncConnection):
         sync_engine = connection_or_session.sync_engine
     else:
         bind = connection_or_session.get_bind()
         if isinstance(bind, Connection):
             sync_engine = bind.engine
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/base.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         return self
 
     async def __aexit__(self, exc_type, exc_value, exc_tb):
         await self.close()
 
     def __str__(self):  # pragma: no cover
         return "<{} {} key={} at 0x{:x}>".format(
-            "locked" if self._acquired else "unlocked", self.__class__.__name__, self._key, id(self)
+            "locked" if self._acquired else "unlocked",
+            self.__class__.__name__,
+            self._key,
+            id(self),
         )
 
     @property
     def connection_or_session(self) -> TAsyncConnectionOrSession:
         return self._connection_or_session
 
     @property
@@ -45,15 +48,19 @@
         return self._key
 
     @property
     def locked(self) -> bool:
         return self._acquired
 
     async def acquire(
-        self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs
+        self,
+        block: bool = True,
+        timeout: Union[float, int, None] = None,
+        *args,
+        **kwargs,
     ) -> bool:  # pragma: no cover
         raise NotImplementedError()
 
     async def release(self, *args, **kwargs):  # pragma: no cover
         raise NotImplementedError()
 
     async def close(self, *args, **kwargs):
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/mysql.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/mysql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/postgresql.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/asyncio/lock/postgresql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/factory.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 else:  # pragma: no cover
     from ._sa_types_backward import TConnectionOrSession
 
 __all__ = ["create_sadlock"]
 
 
 def create_sadlock(
-    connection_or_session: TConnectionOrSession, key, /, contextual_timeout: Union[float, int, None] = None, **kwargs
+    connection_or_session: TConnectionOrSession,
+    key,
+    /,
+    contextual_timeout: Union[float, int, None] = None,
+    **kwargs,
 ) -> BaseSadLock:
     """Create a database distributed lock object
 
     All arguments will be passed to a sub-class of :class:`.BaseSadLock`, depend on the type of ``connection_session``'s SQLAlchemy engine.
 
     Args:
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/base.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,18 @@
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         self.close()
 
     def __str__(self):  # pragma: no cover
         return "<{} {} key={} at 0x{:x}>".format(
-            "locked" if self._acquired else "unlocked", self.__class__.__name__, self._key, id(self)
+            "locked" if self._acquired else "unlocked",
+            self.__class__.__name__,
+            self._key,
+            id(self),
         )
 
     @property
     def connection_or_session(self) -> TConnectionOrSession:
         """Connection or Session object SQL locking functions will be invoked on it
 
         It returns ``connection_or_session`` parameter of the class's constructor.
@@ -111,15 +114,21 @@
     def locked(self) -> bool:
         """locked/unlocked state property
 
         :data:`True` if the lock is acquired, else :data:`False`
         """
         return self._acquired
 
-    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:  # pragma: no cover
+    def acquire(
+        self,
+        block: bool = True,
+        timeout: Union[float, int, None] = None,
+        *args,
+        **kwargs,
+    ) -> bool:  # pragma: no cover
         """Acquire a lock, blocking or non-blocking.
 
         * With the ``block`` argument set to :data:`True` (the default), the method call will block until the lock is in an unlocked state, then set it to locked and return :data:`True`.
 
         * With the ``block`` argument set to :data:`False`, the method call does not block.
           If the lock is currently in a locked state, return :data:`False`; otherwise set the lock to a locked state and return :data:`True`.
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/mysql.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/mysql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/postgresql.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/lock/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,21 @@
     from .._sa_types_backward import TConnectionOrSession
 
 
 class PostgresqlSadLockMixin:
     """A Mix-in class for PostgreSQL advisory lock"""
 
     def __init__(
-        self, *, key, shared: bool = False, xact: bool = False, convert: Optional[Callable[[Any], int]] = None, **kwargs
+        self,
+        *,
+        key,
+        shared: bool = False,
+        xact: bool = False,
+        convert: Optional[Callable[[Any], int]] = None,
+        **kwargs,
     ):
         """
         Args:
             key: PostgreSQL advisory lock requires the key given by ``INT64``.
 
                 * When ``key`` is :class:`int`, the constructor tries to ensure it to be ``INT64``.
                   :class:`OverflowError` is raised if too big or too small for that.
@@ -64,30 +70,29 @@
         else:
             key = to_int64_key(key)
         self._actual_key = key
         #
         self._shared = bool(shared)
         self._xact = bool(xact)
         #
+        self._stmt_unlock = None
         if not shared and not xact:
             self._stmt_lock = LOCK.params(key=key)
             self._stmt_try_lock = TRY_LOCK.params(key=key)
             self._stmt_unlock = UNLOCK.params(key=key)
         elif shared and not xact:
             self._stmt_lock = LOCK_SHARED.params(key=key)
             self._stmt_try_lock = TRY_LOCK_SHARED.params(key=key)
             self._stmt_unlock = UNLOCK_SHARED.params(key=key)
         elif not shared and xact:
             self._stmt_lock = LOCK_XACT.params(key=key)
             self._stmt_try_lock = TRY_LOCK_XACT.params(key=key)
-            self._stmt_unlock = None
         else:
             self._stmt_lock = LOCK_XACT_SHARED.params(key=key)
             self._stmt_try_lock = TRY_LOCK_XACT_SHARED.params(key=key)
-            self._stmt_unlock = None
 
     @property
     def shared(self):
         """Is the advisory lock shared or exclusive"""
         return self._shared
 
     @property
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/postgresql.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/statement/postgresql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/utils.py` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,55 +43,54 @@
 
     Args:
         s: String to convert
 
     Returns:
         Camel case string.
     """
-    s = re.sub(r"\w[\s\W]+\w", "", str(s))
+    s = re.sub(r"\w[\s\W]+\w", "", s)
     if not s:
         return s
-    return lower_case(s[0]) + re.sub(r"[\-_\.\s]([a-z])", lambda matched: upper_case(matched.group(1)), s[1:])
+    return lower_case(s[0]) + re.sub(r"[\-_\.\s]([a-z])", lambda x: upper_case(str(x.group(1))), s[1:])
 
 
 def lower_case(s: str) -> str:
     """Convert string into lower case.
 
     Args:
         s: String to convert
 
     Returns:
         Lowercase case string.
     """
-    return str(s).lower()
+    return s.lower()
 
 
 def upper_case(s: str) -> str:
     """Convert string into upper case.
 
     Args:
         s: String to convert
 
     Returns:
         Uppercase case string.
     """
-    return str(s).upper()
+    return s.upper()
 
 
 def capital_case(s: str) -> str:
     """Convert string into capital case.
     First letters will be uppercase.
 
     Args:
         s: String to convert
 
     Returns:
         Capital case string.
     """
-    s = str(s)
     if not s:
         return s
     return upper_case(s[0]) + s[1:]
 
 
 def pascal_case(s: str) -> str:
     """Convert string into pascal case.
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/PKG-INFO` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.6.1
+Version: 0.6.1.post1
 Summary: A distributed lock implementation based on SQLAlchemy
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
 Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
 Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
 Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
```

### Comparing `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt` & `sqlalchemy-dlock-0.6.1.post1/src/sqlalchemy_dlock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+mypy.ini
 pyproject.toml
 requirements.txt
 src/sqlalchemy_dlock/.gitignore
 src/sqlalchemy_dlock/__init__.py
 src/sqlalchemy_dlock/_sa_types.py
 src/sqlalchemy_dlock/_sa_types_backward.py
 src/sqlalchemy_dlock/_version.py
 src/sqlalchemy_dlock/exceptions.py
 src/sqlalchemy_dlock/factory.py
+src/sqlalchemy_dlock/py.typed
 src/sqlalchemy_dlock/utils.py
 src/sqlalchemy_dlock.egg-info/PKG-INFO
 src/sqlalchemy_dlock.egg-info/SOURCES.txt
 src/sqlalchemy_dlock.egg-info/dependency_links.txt
 src/sqlalchemy_dlock.egg-info/requires.txt
 src/sqlalchemy_dlock.egg-info/top_level.txt
 src/sqlalchemy_dlock/asyncio/__init__.py
```

