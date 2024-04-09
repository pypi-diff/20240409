# Comparing `tmp/alamos-0.2.9.tar.gz` & `tmp/alamos-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alamos-0.2.9.tar", max compression
+gzip compressed data, was "alamos-0.3.1.tar", max compression
```

## Comparing `alamos-0.2.9.tar` & `alamos-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-08-11 20:26:13.181582 alamos-0.2.9/README.md
--rw-r--r--   0        0        0      493 2023-10-31 15:49:45.865537 alamos-0.2.9/alamos/__init__.py
--rw-r--r--   0        0        0     1240 2023-10-11 16:45:00.246609 alamos-0.2.9/alamos/dev/__init__.py
--rw-r--r--   0        0        0     1221 2023-10-11 16:45:00.246390 alamos-0.2.9/alamos/environment.py
--rw-r--r--   0        0        0     4455 2023-10-11 16:45:00.246409 alamos-0.2.9/alamos/instrumentation.py
--rw-r--r--   0        0        0     1708 2023-10-11 16:45:00.246555 alamos-0.2.9/alamos/log.py
--rw-r--r--   0        0        0     1001 2023-10-11 16:45:00.246423 alamos-0.2.9/alamos/meta.py
--rw-r--r--   0        0        0      988 2023-10-11 16:45:00.246503 alamos-0.2.9/alamos/noop.py
--rw-r--r--   0        0        0     6530 2024-03-10 00:38:28.197835 alamos-0.2.9/alamos/trace.py
--rw-r--r--   0        0        0      613 2024-03-10 01:24:13.916212 alamos-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 04:54:54.650056 alamos-0.3.1/README.md
+-rw-r--r--   0        0        0      493 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/dev/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/environment.py
+-rw-r--r--   0        0        0     4455 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/instrumentation.py
+-rw-r--r--   0        0        0     1708 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/log.py
+-rw-r--r--   0        0        0     1001 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/meta.py
+-rw-r--r--   0        0        0      988 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/noop.py
+-rw-r--r--   0        0        0     6530 2024-04-09 04:54:54.650056 alamos-0.3.1/alamos/trace.py
+-rw-r--r--   0        0        0      613 2024-04-09 04:55:04.698087 alamos-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.1/PKG-INFO
```

### Comparing `alamos-0.2.9/alamos/dev/__init__.py` & `alamos-0.3.1/alamos/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/alamos/environment.py` & `alamos-0.3.1/alamos/environment.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/alamos/instrumentation.py` & `alamos-0.3.1/alamos/instrumentation.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/alamos/log.py` & `alamos-0.3.1/alamos/log.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/alamos/meta.py` & `alamos-0.3.1/alamos/meta.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/alamos/noop.py` & `alamos-0.3.1/alamos/noop.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/alamos/trace.py` & `alamos-0.3.1/alamos/trace.py`

 * *Files identical despite different names*

### Comparing `alamos-0.2.9/pyproject.toml` & `alamos-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alamos"
-version = "0.2.9"
+version = "0.3.1"
 description = ""
 authors = ["Emiliano Bonilla <ebonilla@synnaxlabs.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.0"
```

### Comparing `alamos-0.2.9/PKG-INFO` & `alamos-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alamos
-Version: 0.2.9
+Version: 0.3.1
 Summary: 
 Author: Emiliano Bonilla
 Author-email: ebonilla@synnaxlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

