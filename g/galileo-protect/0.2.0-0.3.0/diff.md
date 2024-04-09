# Comparing `tmp/galileo_protect-0.2.0.tar.gz` & `tmp/galileo_protect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.2.0.tar", max compression
+gzip compressed data, was "galileo_protect-0.3.0.tar", max compression
```

## Comparing `galileo_protect-0.2.0.tar` & `galileo_protect-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    10946 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/LICENSE
--rw-r--r--   0        0        0      118 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/README.md
--rw-r--r--   0        0        0     2529 2024-04-08 23:28:32.505848 galileo_protect-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      203 2024-04-08 23:28:32.505848 galileo_protect-0.2.0/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/constants/__init__.py
--rw-r--r--   0        0        0      269 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/helpers/__init__.py
--rw-r--r--   0        0        0      530 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/helpers/config.py
--rw-r--r--   0        0        0     1402 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/invoke.py
--rw-r--r--   0        0        0      638 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/project.py
--rw-r--r--   0        0        0      612 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/schemas/__init__.py
--rw-r--r--   0        0        0      212 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/schemas/invoke.py
--rw-r--r--   0        0        0      124 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/schemas/stage.py
--rw-r--r--   0        0        0     1324 2024-04-08 23:28:31.425848 galileo_protect-0.2.0/src/galileo_protect/stage.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-09 00:25:55.591543 galileo_protect-0.3.0/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-09 00:25:55.591543 galileo_protect-0.3.0/README.md
+-rw-r--r--   0        0        0     2529 2024-04-09 00:25:57.499530 galileo_protect-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      395 2024-04-09 00:25:57.499530 galileo_protect-0.3.0/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     1402 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0      638 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/project.py
+-rw-r--r--   0        0        0      665 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/invoke.py
+-rw-r--r--   0        0        0      266 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/rule.py
+-rw-r--r--   0        0        0      124 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/stage.py
+-rw-r--r--   0        0        0     1324 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/stage.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.3.0/PKG-INFO
```

### Comparing `galileo_protect-0.2.0/LICENSE` & `galileo_protect-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.2.0/pyproject.toml` & `galileo_protect-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.2.0"
+version = "0.3.0"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_protect-0.2.0/src/galileo_protect/helpers/config.py` & `galileo_protect-0.3.0/src/galileo_protect/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.2.0/src/galileo_protect/invoke.py` & `galileo_protect-0.3.0/src/galileo_protect/invoke.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.2.0/src/galileo_protect/project.py` & `galileo_protect-0.3.0/src/galileo_protect/project.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.2.0/src/galileo_protect/schemas/__init__.py` & `galileo_protect-0.3.0/src/galileo_protect/schemas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 from galileo_core.schemas.protect.payload import Payload
 from galileo_core.schemas.protect.request import Request
 from galileo_core.schemas.protect.rule import Rule, RuleOperator
 from galileo_core.schemas.protect.ruleset import Ruleset
 from galileo_core.schemas.protect.stage import Stage
 
 from galileo_protect.schemas.invoke import Response
+from galileo_protect.schemas.rule import RuleMetrics
```

### Comparing `galileo_protect-0.2.0/src/galileo_protect/stage.py` & `galileo_protect-0.3.0/src/galileo_protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.2.0/PKG-INFO` & `galileo_protect-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-protect
-Version: 0.2.0
+Version: 0.3.0
 Summary: 🛡️ Secure your Generative AI applications with Galileo Protect!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

