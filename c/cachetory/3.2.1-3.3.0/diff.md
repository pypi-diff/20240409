# Comparing `tmp/cachetory-3.2.1.tar.gz` & `tmp/cachetory-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-3.2.1.tar", max compression
+gzip compressed data, was "cachetory-3.3.0.tar", max compression
```

## Comparing `cachetory-3.2.1.tar` & `cachetory-3.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11355 2024-03-01 12:13:40.484739 cachetory-3.2.1/LICENSE
--rw-r--r--   0        0        0     1337 2024-03-01 12:13:40.484739 cachetory-3.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/__init__.py
--rw-r--r--   0        0        0     1300 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     2557 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/async_/django.py
--rw-r--r--   0        0        0     1520 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1725 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2769 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0     1294 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     2422 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/sync/django.py
--rw-r--r--   0        0        0     1408 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2340 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2494 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     5524 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/caches/async_.py
--rw-r--r--   0        0        0      120 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/caches/private.py
--rw-r--r--   0        0        0     4915 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     4224 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/decorators/async_.py
--rw-r--r--   0        0        0     1096 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     3648 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     4277 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3665 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      481 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/private/datetime.py
--rw-r--r--   0        0        0      909 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/private/functools.py
--rw-r--r--   0        0        0      205 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/py.typed
--rw-r--r--   0        0        0      776 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     3342 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1548 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     2081 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      762 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/json.py
--rw-r--r--   0        0        0      948 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      873 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1694 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0       38 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/shortcuts/__init__.py
--rw-r--r--   0        0        0      696 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/shortcuts/async_.py
--rw-r--r--   0        0        0      692 2024-03-01 12:13:40.484739 cachetory-3.2.1/cachetory/shortcuts/sync.py
--rw-r--r--   0        0        0     3735 2024-03-01 12:13:51.064747 cachetory-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 cachetory-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-09 09:46:55.096301 cachetory-3.3.0/LICENSE
+-rw-r--r--   0        0        0     1337 2024-04-09 09:46:55.096301 cachetory-3.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0     1300 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/async_/django.py
+-rw-r--r--   0        0        0     1520 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1725 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2769 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0     1294 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/sync/django.py
+-rw-r--r--   0        0        0     1408 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2340 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2494 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     5524 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      120 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     4915 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0     1096 2024-04-09 09:46:55.096301 cachetory-3.3.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     3648 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     4277 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3665 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      481 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      909 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/py.typed
+-rw-r--r--   0        0        0      776 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     3342 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     2081 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      762 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      948 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      873 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1694 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0       38 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/shortcuts/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/shortcuts/async_.py
+-rw-r--r--   0        0        0      692 2024-04-09 09:46:55.100301 cachetory-3.3.0/cachetory/shortcuts/sync.py
+-rw-r--r--   0        0        0     3745 2024-04-09 09:47:06.288249 cachetory-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 cachetory-3.3.0/PKG-INFO
```

### Comparing `cachetory-3.2.1/LICENSE` & `cachetory-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/README.md` & `cachetory-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/async_/__init__.py` & `cachetory-3.3.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/async_/django.py` & `cachetory-3.3.0/cachetory/backends/async_/django.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/async_/dummy.py` & `cachetory-3.3.0/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/async_/memory.py` & `cachetory-3.3.0/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/async_/redis.py` & `cachetory-3.3.0/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/sync/__init__.py` & `cachetory-3.3.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/sync/django.py` & `cachetory-3.3.0/cachetory/backends/sync/django.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/sync/dummy.py` & `cachetory-3.3.0/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/sync/memory.py` & `cachetory-3.3.0/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/backends/sync/redis.py` & `cachetory-3.3.0/cachetory/backends/sync/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/caches/async_.py` & `cachetory-3.3.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/caches/sync.py` & `cachetory-3.3.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/decorators/async_.py` & `cachetory-3.3.0/cachetory/decorators/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/decorators/shared.py` & `cachetory-3.3.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/decorators/sync.py` & `cachetory-3.3.0/cachetory/decorators/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/interfaces/backends/async_.py` & `cachetory-3.3.0/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/interfaces/backends/private.py` & `cachetory-3.3.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/interfaces/backends/sync.py` & `cachetory-3.3.0/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/interfaces/serializers.py` & `cachetory-3.3.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/private/functools.py` & `cachetory-3.3.0/cachetory/private/functools.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/__init__.py` & `cachetory-3.3.0/cachetory/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/chained.py` & `cachetory-3.3.0/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/compressors/zlib.py` & `cachetory-3.3.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/compressors/zstd.py` & `cachetory-3.3.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/json.py` & `cachetory-3.3.0/cachetory/serializers/json.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/msgpack.py` & `cachetory-3.3.0/cachetory/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/noop.py` & `cachetory-3.3.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/serializers/pickle.py` & `cachetory-3.3.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/shortcuts/async_.py` & `cachetory-3.3.0/cachetory/shortcuts/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/cachetory/shortcuts/sync.py` & `cachetory-3.3.0/cachetory/shortcuts/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-3.2.1/pyproject.toml` & `cachetory-3.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "3.2.1"
+version = "3.3.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,15 +30,15 @@
 ]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.dependencies]
-django = {version = "^4.0.0", optional = true}
+django = {version = "^4.0.0 || ^5.0.0", optional = true}
 ormsgpack = {version = "^1.4.0", optional = true, markers = "platform_python_implementation == 'CPython'"}
 pydantic = ">2.0.0.0, <3.0.0.0"
 python = "^3.8.0"
 redis = {version = "^4.4.2 || ^5.0.0", optional = true}
 typing-extensions = "^4.4.0"
 zstd = {version = "^1.5.2.6", optional = true}
 
@@ -49,33 +49,33 @@
 zstd = ["zstd"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 freezegun = "1.4.0"
-mypy = "1.8.0"
-pytest = "7.4.4"
-pytest-asyncio = "0.23.5"
-pytest-cov = "4.1.0"
-ruff = "0.3.0"
+mypy = "1.9.0"
+pytest = "8.1.1"
+pytest-asyncio = "0.23.6"
+pytest-cov = "5.0.0"
+ruff = "0.3.5"
 types-redis = "^4.4.0.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-black = "24.2.0"
+black = "24.3.0"
 cairosvg = "2.7.1"
 mkdocs-autorefs = "1.0.1"
 mkdocs-git-committers-plugin-2 = "2.3.0"
 mkdocs-git-revision-date-localized-plugin = "1.2.4"
-mkdocs-material = "9.5.12"
-mkdocstrings = { version = "0.24.1", extras = ["python"] }
-pillow = "10.2.0"
+mkdocs-material = "9.5.17"
+mkdocstrings = { version = "0.24.3", extras = ["python"] }
+pillow = "10.3.0"
 
 [tool.black]
 line-length = 120
 target_version = ["py38", "py39", "py310", "py311"]
 
 [tool.ruff]
 line-length = 120
```

### Comparing `cachetory-3.2.1/PKG-INFO` & `cachetory-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 3.2.1
+Version: 3.3.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Typing :: Typed
 Provides-Extra: django
 Provides-Extra: ormsgpack
 Provides-Extra: redis
 Provides-Extra: zstd
-Requires-Dist: django (>=4.0.0,<5.0.0) ; extra == "django"
+Requires-Dist: django (>=4.0.0,<6.0.0) ; extra == "django"
 Requires-Dist: ormsgpack (>=1.4.0,<2.0.0) ; (platform_python_implementation == "CPython") and (extra == "ormsgpack")
 Requires-Dist: pydantic (>2.0.0.0,<3.0.0.0)
 Requires-Dist: redis (>=4.4.2,<6.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: zstd (>=1.5.2.6,<2.0.0.0) ; extra == "zstd"
 Project-URL: Repository, https://github.com/kpn/cachetory
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: cachetory Version: 3.2.1 Summary: Caching library
+Metadata-Version: 2.1 Name: cachetory Version: 3.3.0 Summary: Caching library
 with support for multiple cache backends Home-page: https://github.com/kpn/
 cachetory License: Apache-2.0 Keywords: cache Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Topic :: Internet ::
 WWW/HTTP Classifier: Typing :: Typed Provides-Extra: django Provides-Extra:
 ormsgpack Provides-Extra: redis Provides-Extra: zstd Requires-Dist: django
-(>=4.0.0,<5.0.0) ; extra == "django" Requires-Dist: ormsgpack (>=1.4.0,<2.0.0)
+(>=4.0.0,<6.0.0) ; extra == "django" Requires-Dist: ormsgpack (>=1.4.0,<2.0.0)
 ; (platform_python_implementation == "CPython") and (extra == "ormsgpack")
 Requires-Dist: pydantic (>2.0.0.0,<3.0.0.0) Requires-Dist: redis
 (>=4.4.2,<6.0.0) ; extra == "redis" Requires-Dist: typing-extensions
 (>=4.4.0,<5.0.0) Requires-Dist: zstd (>=1.5.2.6,<2.0.0.0) ; extra == "zstd"
 Project-URL: Repository, https://github.com/kpn/cachetory Description-Content-
 Type: text/markdown # Cachetory [![PyPI](https://img.shields.io/pypi/v/
 cachetory?logo=python&logoColor=yellow)](https://pypi.org/project/cachetory/)
```

