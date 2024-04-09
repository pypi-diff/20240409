# Comparing `tmp/ptars-0.0.1.tar.gz` & `tmp/ptars-0.0.1rc1.tar.gz`

## Comparing `ptars-0.0.1.tar` & `ptars-0.0.1rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 ptars-0.0.1/Cargo.toml
--rw-r--r--   0     1001      127     1124 2024-04-09 12:36:59.000000 ptars-0.0.1/DEVELOPMENT.md
--rw-r--r--   0     1001      127    11357 2024-04-09 12:36:59.000000 ptars-0.0.1/LICENSE
--rw-r--r--   0     1001      127      701 2024-04-09 12:36:59.000000 ptars-0.0.1/Makefile
--rw-r--r--   0     1001      127     2620 2024-04-09 12:36:59.000000 ptars-0.0.1/README.md
--rw-r--r--   0     1001      127   170098 2024-04-09 12:36:59.000000 ptars-0.0.1/poetry.lock
--rw-r--r--   0     1001      127     7016 2024-04-09 12:36:59.000000 ptars-0.0.1/protos/bench.proto
--rw-r--r--   0     1001      127     3465 2024-04-09 12:36:59.000000 ptars-0.0.1/protos/simple.proto
--rw-r--r--   0     1001      127        0 2024-04-09 12:36:59.000000 ptars-0.0.1/python/__init__.py
--rw-r--r--   0     1001      127       66 2024-04-09 12:36:59.000000 ptars-0.0.1/python/ptars/__init__.py
--rw-r--r--   0     1001      127     1468 2024-04-09 12:36:59.000000 ptars-0.0.1/python/ptars/internal.py
--rw-r--r--   0     1001      127     1381 2024-04-09 12:36:59.000000 ptars-0.0.1/scripts/protoc.py
--rw-r--r--   0     1001      127    24603 2024-04-09 12:36:59.000000 ptars-0.0.1/src/lib.rs
--rw-r--r--   0     1001      127    30653 2024-04-09 12:36:59.000000 ptars-0.0.1/Cargo.lock
--rw-r--r--   0     1001      127     2195 2024-04-09 12:36:59.000000 ptars-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3166 1970-01-01 00:00:00.000000 ptars-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 ptars-0.0.1rc1/Cargo.toml
+-rw-r--r--   0     1001      127     1124 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/DEVELOPMENT.md
+-rw-r--r--   0     1001      127    11357 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/LICENSE
+-rw-r--r--   0     1001      127      701 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/Makefile
+-rw-r--r--   0     1001      127     2620 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/README.md
+-rw-r--r--   0     1001      127   170098 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/poetry.lock
+-rw-r--r--   0     1001      127     7016 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/protos/bench.proto
+-rw-r--r--   0     1001      127     3465 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/protos/simple.proto
+-rw-r--r--   0     1001      127        0 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/python/__init__.py
+-rw-r--r--   0     1001      127       66 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/python/ptars/__init__.py
+-rw-r--r--   0     1001      127     1468 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/python/ptars/internal.py
+-rw-r--r--   0     1001      127     1381 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/scripts/protoc.py
+-rw-r--r--   0     1001      127    24603 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/src/lib.rs
+-rw-r--r--   0     1001      127    30657 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/Cargo.lock
+-rw-r--r--   0     1001      127     2199 2024-04-09 12:21:34.000000 ptars-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 ptars-0.0.1rc1/PKG-INFO
```

### Comparing `ptars-0.0.1/Cargo.toml` & `ptars-0.0.1rc1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ptarslib"
-version = "0.0.1"
+version = "0.0.1-rc1"
 authors = ["0x26res <0x26res@gmail.net>"]
 edition = "2021"
 description = "Fast python conversion from protobuf to arrow using rust"
 homepage = "https://github.com/0x26res/ptars"
 repository = "https://github.com/0x26res/ptars"
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `ptars-0.0.1/DEVELOPMENT.md` & `ptars-0.0.1rc1/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/LICENSE` & `ptars-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/Makefile` & `ptars-0.0.1rc1/Makefile`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/README.md` & `ptars-0.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/poetry.lock` & `ptars-0.0.1rc1/poetry.lock`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/protos/bench.proto` & `ptars-0.0.1rc1/protos/bench.proto`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/protos/simple.proto` & `ptars-0.0.1rc1/protos/simple.proto`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/python/ptars/internal.py` & `ptars-0.0.1rc1/python/ptars/internal.py`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/scripts/protoc.py` & `ptars-0.0.1rc1/scripts/protoc.py`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/src/lib.rs` & `ptars-0.0.1rc1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ptars-0.0.1/Cargo.lock` & `ptars-0.0.1rc1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -738,15 +738,15 @@
 checksum = "e1ed294a835b0f30810e13616b1cd34943c6d1e84a8f3b0dcfe466d256c3e7e7"
 dependencies = [
  "thiserror",
 ]
 
 [[package]]
 name = "ptarslib"
-version = "0.0.1"
+version = "0.0.1-rc1"
 dependencies = [
  "arrow",
  "arrow-array",
  "arrow-schema",
  "chrono",
  "protobuf",
  "pyo3",
```

### Comparing `ptars-0.0.1/pyproject.toml` & `ptars-0.0.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requires-python = ">=3.8"
 dependencies = [
     'protobuf > 3',
 ]
 
 [tool.poetry]
 name = "ptars"
-version = "0.0.1"
+version = "0.0.1-rc1"
 description = "Convert from protobuf to arrow and back in rust"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [    { include = "ptars", from = "python" } ]
 include = ["ptars/*",  "ptarslib/*", "ptarslib/src/*"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `ptars-0.0.1/PKG-INFO` & `ptars-0.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ptars
-Version: 0.0.1
+Version: 0.0.1rc1
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: protobuf >3
 License-File: LICENSE
 Summary: Fast python conversion from protobuf to arrow using rust
 Home-Page: https://github.com/0x26res/ptars
 Author: 0x26res <0x26res@gmail.net>
```

