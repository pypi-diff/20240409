# Comparing `tmp/alamos-0.3.1.tar.gz` & `tmp/alamos-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alamos-0.3.1.tar", max compression
+gzip compressed data, was "alamos-0.3.2.tar", max compression
```

## Comparing `alamos-0.3.1.tar` & `alamos-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-09 04:54:54.650056 alamos-0.3.1/README.md
--rw-r--r--   0        0        0      493 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/__init__.py
--rw-r--r--   0        0        0     1240 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/dev/__init__.py
--rw-r--r--   0        0        0     1221 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/environment.py
--rw-r--r--   0        0        0     4455 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/instrumentation.py
--rw-r--r--   0        0        0     1708 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/log.py
--rw-r--r--   0        0        0     1001 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/meta.py
--rw-r--r--   0        0        0      988 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/noop.py
--rw-r--r--   0        0        0     6530 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/trace.py
--rw-r--r--   0        0        0      613 2024-04-09 04:55:04.698087 alamos-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 05:22:01.788031 alamos-0.3.2/README.md
+-rw-r--r--   0        0        0      493 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/dev/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/environment.py
+-rw-r--r--   0        0        0     4455 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/instrumentation.py
+-rw-r--r--   0        0        0     1708 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/log.py
+-rw-r--r--   0        0        0     1001 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/meta.py
+-rw-r--r--   0        0        0      988 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/noop.py
+-rw-r--r--   0        0        0     6530 2024-04-09 05:22:01.788031 alamos-0.3.2/alamos/trace.py
+-rw-r--r--   0        0        0      613 2024-04-09 05:22:16.840123 alamos-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.2/PKG-INFO
```

### Comparing `alamos-0.3.1/alamos/dev/__init__.py` & `alamos-0.3.2/alamos/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/alamos/environment.py` & `alamos-0.3.2/alamos/environment.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/alamos/instrumentation.py` & `alamos-0.3.2/alamos/instrumentation.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/alamos/log.py` & `alamos-0.3.2/alamos/log.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/alamos/meta.py` & `alamos-0.3.2/alamos/meta.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/alamos/noop.py` & `alamos-0.3.2/alamos/noop.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/alamos/trace.py` & `alamos-0.3.2/alamos/trace.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.1/pyproject.toml` & `alamos-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alamos"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Emiliano Bonilla <ebonilla@synnaxlabs.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.0"
```

### Comparing `alamos-0.3.1/PKG-INFO` & `alamos-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alamos
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Emiliano Bonilla
 Author-email: ebonilla@synnaxlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

