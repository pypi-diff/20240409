# Comparing `tmp/robocorp_actions-0.1.1.tar.gz` & `tmp/robocorp_actions-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_actions-0.1.1.tar", max compression
+gzip compressed data, was "robocorp_actions-0.1.2.tar", max compression
```

## Comparing `robocorp_actions-0.1.1.tar` & `robocorp_actions-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2958 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/README.md
--rw-r--r--   0        0        0      965 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3596 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/__init__.py
--rw-r--r--   0        0        0       81 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/__main__.py
--rw-r--r--   0        0        0      140 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_action_options.py
--rw-r--r--   0        0        0     5199 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     4243 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_fixtures.py
--rw-r--r--   0        0        0    11967 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_lint_action.py
--rw-r--r--   0        0        0     1211 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_managed_parameters.py
--rw-r--r--   0        0        0      314 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_protocols.py
--rw-r--r--   0        0        0     2907 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/_request_impl.py
--rw-r--r--   0        0        0     2123 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/cli.py
--rw-r--r--   0        0        0        0 2024-04-08 10:13:29.000947 robocorp_actions-0.1.1/src/robocorp/actions/py.typed
--rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 robocorp_actions-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2958 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/README.md
+-rw-r--r--   0        0        0      965 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3596 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/__main__.py
+-rw-r--r--   0        0        0      140 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_action_options.py
+-rw-r--r--   0        0        0     5199 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     4243 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_fixtures.py
+-rw-r--r--   0        0        0    11967 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_lint_action.py
+-rw-r--r--   0        0        0     1211 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_managed_parameters.py
+-rw-r--r--   0        0        0      314 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_protocols.py
+-rw-r--r--   0        0        0     2907 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/_request_impl.py
+-rw-r--r--   0        0        0     2123 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:28:14.340092 robocorp_actions-0.1.2/src/robocorp/actions/py.typed
+-rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 robocorp_actions-0.1.2/PKG-INFO
```

### Comparing `robocorp_actions-0.1.1/README.md` & `robocorp_actions-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/pyproject.toml` & `robocorp_actions-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "robocorp-actions"
-version = "0.1.1"
+version = "0.1.2"
 description = "Robocorp Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
 packages = [{ include = "robocorp", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 # robocorp-actions is tighly coupled with robocorp-tasks, so,
 # the version must be an exact match up to the minor version.
-robocorp-tasks = "3.0.0"
+robocorp-tasks = "3.0.2"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = { path = "../devutils/", develop = true }
 
 # We just need it for tests. In runtime duck-typing is used to
 # check for `cls.parse_obj(dict)` and `cls.model_json_schema()`
 pydantic = "^2.6"
```

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/__init__.py` & `robocorp_actions-0.1.2/src/robocorp/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Callable, Optional, overload
 
 from ._action_options import ActionOptions
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/_args_dispatcher.py` & `robocorp_actions-0.1.2/src/robocorp/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/_fixtures.py` & `robocorp_actions-0.1.2/src/robocorp/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/_lint_action.py` & `robocorp_actions-0.1.2/src/robocorp/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/_managed_parameters.py` & `robocorp_actions-0.1.2/src/robocorp/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/_request.py` & `robocorp_actions-0.1.2/src/robocorp/actions/_request.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/_request_impl.py` & `robocorp_actions-0.1.2/src/robocorp/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/src/robocorp/actions/cli.py` & `robocorp_actions-0.1.2/src/robocorp/actions/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.1.1/PKG-INFO` & `robocorp_actions-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: robocorp-actions
-Version: 0.1.1
+Version: 0.1.2
 Summary: Robocorp Actions
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: robocorp-tasks (==3.0.0)
+Requires-Dist: robocorp-tasks (==3.0.2)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # ⚡️ robocorp-actions
 
 A Python library designed to simplify the development of Python actions _(AI or otherwise)_ to be run with the [Robocorp Action Server](../action_server/).
```

