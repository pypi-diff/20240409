# Comparing `tmp/ommx-0.0.1.tar.gz` & `tmp/ommx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommx-0.0.1.tar", last modified: Fri Apr  5 06:38:03 2024, max compression
+gzip compressed data, was "ommx-0.1.0.tar", last modified: Tue Apr  9 07:59:20 2024, max compression
```

## Comparing `ommx-0.0.1.tar` & `ommx-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:38:03.336600 ommx-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 06:37:57.000000 ommx-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-05 06:38:03.336600 ommx-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-05 06:37:57.000000 ommx-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:38:03.332600 ommx-0.0.1/ommx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:38:03.336600 ommx-0.0.1/ommx/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/constraint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/constraint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/decision_variables_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/decision_variables_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/linear_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/linear_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/polynomial_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/polynomial_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/quadratic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/quadratic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/solution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/solution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-05 06:37:57.000000 ommx-0.0.1/ommx/v1/sparse_matrix_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:38:03.336600 ommx-0.0.1/ommx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-05 06:38:03.000000 ommx-0.0.1/ommx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-05 06:38:03.000000 ommx-0.0.1/ommx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:38:03.000000 ommx-0.0.1/ommx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 06:38:03.000000 ommx-0.0.1/ommx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 06:38:03.000000 ommx-0.0.1/ommx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 06:37:57.000000 ommx-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:38:03.336600 ommx-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.870624 ommx-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 07:59:15.000000 ommx-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-09 07:59:20.870624 ommx-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-09 07:59:15.000000 ommx-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.866624 ommx-0.1.0/ommx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.870624 ommx-0.1.0/ommx/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/constraint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/constraint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/decision_variables_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/decision_variables_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/linear_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/linear_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/polynomial_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/polynomial_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/quadratic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/quadratic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/solution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/solution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/sparse_matrix_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.870624 ommx-0.1.0/ommx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 07:59:15.000000 ommx-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:59:20.870624 ommx-0.1.0/setup.cfg
```

### Comparing `ommx-0.0.1/PKG-INFO` & `ommx-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ommx
-Version: 0.0.1
+Version: 0.1.0
 Summary: Open Mathematical prograMming eXchange (OMMX)
 Author-email: "Jij Inc." <info@j-ij.com>
 Project-URL: Homepage, https://github.com/Jij-Inc/ommx
 Project-URL: Issues, https://github.com/Jij-Inc/ommx/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,40 +17,45 @@
 Description-Content-Type: text/markdown
 Requires-Dist: protobuf<6.0.0,>=5.26.1
 Provides-Extra: dev
 Requires-Dist: mypy>=0.910; extra == "dev"
 Requires-Dist: mypy-protobuf; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
+Requires-Dist: sphinx_fontawesome; extra == "dev"
+Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: types-protobuf>=0.1.14; extra == "dev"
 
 # OMMX
+[![PyPI - Version](https://img.shields.io/pypi/v/ommx)](https://pypi.org/project/ommx/)
+[![Crates.io Version](https://img.shields.io/crates/v/ommx)](https://crates.io/crates/ommx)
 
 Open Mathematical prograMming eXchange (OMMX) is an open ecosystem that empowers mathematical programming and optimization developers and reserchers.
 
 # API Reference
 
 - [Protobuf](https://jij-inc.github.io/ommx/protobuf.html)
 - [Rust](https://jij-inc.github.io/ommx/rust/ommx/index.html)
+- [Python](https://jij-inc.github.io/ommx/python/index.html)
 
 # Compatibility
 
 This project manages several versions as follows:
 
 ## Protocol buffers schema
 
 - OMMX defines a protocol buffers schema with version like `v1`, `v2`, etc. `v1` schema has a namesapce `ommx.v1`.
-- Schemas in `ommx.v1` will be compatible after [`1.0.0` release](https://github.com/Jij-Inc/ommx/milestone/3). Note that the schema can be changed incompatible way until this release.
-- `v2` schema with namespace `ommx.v2` will start developing if we need to change the schema in incompatible way after `1.0.0` release. Compatible changes will be made in `v1` schema also after `1.0.0` release. We never create namespaces like `ommx.v1_1`.
+- Schemas in `ommx.v1` will be compatible after [ommx.v1 schema release](https://github.com/Jij-Inc/ommx/milestone/3). Note that the schema can be changed incompatible way until this release.
+- `v2` schema with namespace `ommx.v2` will start developing if we need to change the schema in incompatible way after `ommx.v1` release. Compatible changes will be made in `v1` schema also after its release. We never create namespaces like `ommx.v1_1`.
 
-## `ommx` Rust crate
-TBW
-
-## `ommx` Python package
-TBW
+## Language specific bindings
+This project consists of main protobuf schema and language specific bindings.
+Their versions are managed independently, and adopts semantic versioning.
 
 # License
 © 2024 Jij Inc.
 
 This project is licensed under either of
 
 - Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
```

### Comparing `ommx-0.0.1/README.md` & `ommx-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # OMMX
+[![PyPI - Version](https://img.shields.io/pypi/v/ommx)](https://pypi.org/project/ommx/)
+[![Crates.io Version](https://img.shields.io/crates/v/ommx)](https://crates.io/crates/ommx)
 
 Open Mathematical prograMming eXchange (OMMX) is an open ecosystem that empowers mathematical programming and optimization developers and reserchers.
 
 # API Reference
 
 - [Protobuf](https://jij-inc.github.io/ommx/protobuf.html)
 - [Rust](https://jij-inc.github.io/ommx/rust/ommx/index.html)
+- [Python](https://jij-inc.github.io/ommx/python/index.html)
 
 # Compatibility
 
 This project manages several versions as follows:
 
 ## Protocol buffers schema
 
 - OMMX defines a protocol buffers schema with version like `v1`, `v2`, etc. `v1` schema has a namesapce `ommx.v1`.
-- Schemas in `ommx.v1` will be compatible after [`1.0.0` release](https://github.com/Jij-Inc/ommx/milestone/3). Note that the schema can be changed incompatible way until this release.
-- `v2` schema with namespace `ommx.v2` will start developing if we need to change the schema in incompatible way after `1.0.0` release. Compatible changes will be made in `v1` schema also after `1.0.0` release. We never create namespaces like `ommx.v1_1`.
+- Schemas in `ommx.v1` will be compatible after [ommx.v1 schema release](https://github.com/Jij-Inc/ommx/milestone/3). Note that the schema can be changed incompatible way until this release.
+- `v2` schema with namespace `ommx.v2` will start developing if we need to change the schema in incompatible way after `ommx.v1` release. Compatible changes will be made in `v1` schema also after its release. We never create namespaces like `ommx.v1_1`.
 
-## `ommx` Rust crate
-TBW
-
-## `ommx` Python package
-TBW
+## Language specific bindings
+This project consists of main protobuf schema and language specific bindings.
+Their versions are managed independently, and adopts semantic versioning.
 
 # License
 © 2024 Jij Inc.
 
 This project is licensed under either of
 
 - Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
```

### Comparing `ommx-0.0.1/ommx/v1/constraint_pb2.py` & `ommx-0.1.0/ommx/v1/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/constraint_pb2.pyi` & `ommx-0.1.0/ommx/v1/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/decision_variables_pb2.py` & `ommx-0.1.0/ommx/v1/decision_variables_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/decision_variables_pb2.pyi` & `ommx-0.1.0/ommx/v1/decision_variables_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/function_pb2.py` & `ommx-0.1.0/ommx/v1/function_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/function_pb2.pyi` & `ommx-0.1.0/ommx/v1/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/instance_pb2.py` & `ommx-0.1.0/ommx/v1/instance_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/instance_pb2.pyi` & `ommx-0.1.0/ommx/v1/instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/linear_pb2.py` & `ommx-0.1.0/ommx/v1/linear_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/linear_pb2.pyi` & `ommx-0.1.0/ommx/v1/linear_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/polynomial_pb2.py` & `ommx-0.1.0/ommx/v1/polynomial_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/polynomial_pb2.pyi` & `ommx-0.1.0/ommx/v1/polynomial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/quadratic_pb2.py` & `ommx-0.1.0/ommx/v1/quadratic_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/quadratic_pb2.pyi` & `ommx-0.1.0/ommx/v1/quadratic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/solution_pb2.py` & `ommx-0.1.0/ommx/v1/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/solution_pb2.pyi` & `ommx-0.1.0/ommx/v1/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx/v1/sparse_matrix_pb2.py` & `ommx-0.1.0/ommx/v1/sparse_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.0.1/ommx.egg-info/PKG-INFO` & `ommx-0.1.0/ommx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ommx
-Version: 0.0.1
+Version: 0.1.0
 Summary: Open Mathematical prograMming eXchange (OMMX)
 Author-email: "Jij Inc." <info@j-ij.com>
 Project-URL: Homepage, https://github.com/Jij-Inc/ommx
 Project-URL: Issues, https://github.com/Jij-Inc/ommx/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,40 +17,45 @@
 Description-Content-Type: text/markdown
 Requires-Dist: protobuf<6.0.0,>=5.26.1
 Provides-Extra: dev
 Requires-Dist: mypy>=0.910; extra == "dev"
 Requires-Dist: mypy-protobuf; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
+Requires-Dist: sphinx_fontawesome; extra == "dev"
+Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: types-protobuf>=0.1.14; extra == "dev"
 
 # OMMX
+[![PyPI - Version](https://img.shields.io/pypi/v/ommx)](https://pypi.org/project/ommx/)
+[![Crates.io Version](https://img.shields.io/crates/v/ommx)](https://crates.io/crates/ommx)
 
 Open Mathematical prograMming eXchange (OMMX) is an open ecosystem that empowers mathematical programming and optimization developers and reserchers.
 
 # API Reference
 
 - [Protobuf](https://jij-inc.github.io/ommx/protobuf.html)
 - [Rust](https://jij-inc.github.io/ommx/rust/ommx/index.html)
+- [Python](https://jij-inc.github.io/ommx/python/index.html)
 
 # Compatibility
 
 This project manages several versions as follows:
 
 ## Protocol buffers schema
 
 - OMMX defines a protocol buffers schema with version like `v1`, `v2`, etc. `v1` schema has a namesapce `ommx.v1`.
-- Schemas in `ommx.v1` will be compatible after [`1.0.0` release](https://github.com/Jij-Inc/ommx/milestone/3). Note that the schema can be changed incompatible way until this release.
-- `v2` schema with namespace `ommx.v2` will start developing if we need to change the schema in incompatible way after `1.0.0` release. Compatible changes will be made in `v1` schema also after `1.0.0` release. We never create namespaces like `ommx.v1_1`.
+- Schemas in `ommx.v1` will be compatible after [ommx.v1 schema release](https://github.com/Jij-Inc/ommx/milestone/3). Note that the schema can be changed incompatible way until this release.
+- `v2` schema with namespace `ommx.v2` will start developing if we need to change the schema in incompatible way after `ommx.v1` release. Compatible changes will be made in `v1` schema also after its release. We never create namespaces like `ommx.v1_1`.
 
-## `ommx` Rust crate
-TBW
-
-## `ommx` Python package
-TBW
+## Language specific bindings
+This project consists of main protobuf schema and language specific bindings.
+Their versions are managed independently, and adopts semantic versioning.
 
 # License
 © 2024 Jij Inc.
 
 This project is licensed under either of
 
 - Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
```

### Comparing `ommx-0.0.1/ommx.egg-info/SOURCES.txt` & `ommx-0.1.0/ommx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 ommx/__init__.py
 ommx.egg-info/PKG-INFO
 ommx.egg-info/SOURCES.txt
 ommx.egg-info/dependency_links.txt
 ommx.egg-info/requires.txt
 ommx.egg-info/top_level.txt
+ommx/v1/__init__.py
 ommx/v1/constraint_pb2.py
 ommx/v1/constraint_pb2.pyi
 ommx/v1/decision_variables_pb2.py
 ommx/v1/decision_variables_pb2.pyi
 ommx/v1/function_pb2.py
 ommx/v1/function_pb2.pyi
 ommx/v1/instance_pb2.py
```

### Comparing `ommx-0.0.1/pyproject.toml` & `ommx-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ommx"
-version = "0.0.1"
+version = "0.1.0"
 description = "Open Mathematical prograMming eXchange (OMMX)"
 authors = [
     { name="Jij Inc.", email="info@j-ij.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -24,14 +24,18 @@
 
 [project.optional-dependencies]
 dev = [
     "mypy>=0.910",
     "mypy-protobuf",
     "pyright",
     "pytest",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "sphinx_fontawesome",
+    "sphinx-autoapi",
     "types-protobuf>=0.1.14",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/Jij-Inc/ommx"
 Issues = "https://github.com/Jij-Inc/ommx/issues"
```

