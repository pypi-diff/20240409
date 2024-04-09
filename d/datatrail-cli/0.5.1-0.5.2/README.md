# Comparing `tmp/datatrail_cli-0.5.1.tar.gz` & `tmp/datatrail_cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.5.1.tar", max compression
+gzip compressed data, was "datatrail_cli-0.5.2.tar", max compression
```

## Comparing `datatrail_cli-0.5.1.tar` & `datatrail_cli-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2024-01-09 19:14:10.829548 datatrail_cli-0.5.1/LICENSE
--rw-r--r--   0        0        0     3558 2024-01-09 19:14:10.829548 datatrail_cli-0.5.1/README.md
--rw-r--r--   0        0        0      214 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/__init__.py
--rw-r--r--   0        0        0     4590 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/clear.py
--rw-r--r--   0        0        0     1437 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/cli.py
--rw-r--r--   0        0        0     4037 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/config.py
--rw-r--r--   0        0        0     1062 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/config.yaml
--rw-r--r--   0        0        0     3806 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/ls.py
--rw-r--r--   0        0        0     7846 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/ps.py
--rw-r--r--   0        0        0     4576 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/pull.py
--rw-r--r--   0        0        0    15634 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     3089 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1071 2024-01-09 19:14:10.841548 datatrail_cli-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 datatrail_cli-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-09 18:55:51.200617 datatrail_cli-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3558 2024-04-09 18:55:51.200617 datatrail_cli-0.5.2/README.md
+-rw-r--r--   0        0        0      214 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/__init__.py
+-rw-r--r--   0        0        0     4590 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/clear.py
+-rw-r--r--   0        0        0     1437 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/cli.py
+-rw-r--r--   0        0        0     4037 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/config.yaml
+-rw-r--r--   0        0        0     3806 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/ls.py
+-rw-r--r--   0        0        0     7846 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/ps.py
+-rw-r--r--   0        0        0     4576 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/pull.py
+-rw-r--r--   0        0        0    15634 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     3089 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1073 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.2/PKG-INFO
```

### Comparing `datatrail_cli-0.5.1/LICENSE` & `datatrail_cli-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/README.md` & `datatrail_cli-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/clear.py` & `datatrail_cli-0.5.2/dtcli/clear.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/cli.py` & `datatrail_cli-0.5.2/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/config.py` & `datatrail_cli-0.5.2/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/config.yaml` & `datatrail_cli-0.5.2/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/ls.py` & `datatrail_cli-0.5.2/dtcli/ls.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/ps.py` & `datatrail_cli-0.5.2/dtcli/ps.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/pull.py` & `datatrail_cli-0.5.2/dtcli/pull.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/src/functions.py` & `datatrail_cli-0.5.2/dtcli/src/functions.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.5.2/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/dtcli/utilities/utilities.py` & `datatrail_cli-0.5.2/dtcli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.1/pyproject.toml` & `datatrail_cli-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.5.1"
+version = "0.5.2"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.3"
 requests = "^2.29.0"
 rich = "^13.3.5"
 pyaml = "^21.10.1"
 cadcutils = "^1.5.1.1"
-cadcdata = "^2.4"
+cadcdata = "^2.5.0"
 cadctap = "^0.9.11"
 mergedeep = "^1.3.4"
 dill = "^0.3.6"
 lxml = "^4.9.2"
 click-aliasing = "^1.0.0"
 
 [tool.poetry.scripts]
```

### Comparing `datatrail_cli-0.5.1/PKG-INFO` & `datatrail_cli-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cadcdata (>=2.4,<3.0)
+Requires-Dist: cadcdata (>=2.5.0,<3.0.0)
 Requires-Dist: cadctap (>=0.9.11,<0.10.0)
 Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliasing (>=1.0.0,<2.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.1 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.2 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: cadcdata (>=2.4,<3.0) Requires-Dist: cadctap
+Python :: 3.12 Requires-Dist: cadcdata (>=2.5.0,<3.0.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
 click (>=8.1.3,<9.0.0) Requires-Dist: click-aliasing (>=1.0.0,<2.0.0) Requires-
 Dist: dill (>=0.3.6,<0.4.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist:
 mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pyaml (>=21.10.1,<22.0.0) Requires-
 Dist: requests (>=2.29.0,<3.0.0) Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
                                  height="100">
```

