# Comparing `tmp/robocorp_tasks-3.0.2.tar.gz` & `tmp/robocorp_tasks-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-3.0.2.tar", max compression
+gzip compressed data, was "robocorp_tasks-3.0.3.tar", max compression
```

## Comparing `robocorp_tasks-3.0.2.tar` & `robocorp_tasks-3.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rwxr-xr-x   0        0        0     2189 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/README.md
--rw-r--r--   0        0        0     1565 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     4325 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     7959 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1494 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     8261 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    28952 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      331 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_constants.py
--rw-r--r--   0        0        0        0 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/__init__.py
--rw-r--r--   0        0        0      572 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_extension_points.py
--rw-r--r--   0        0        0     9934 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      242 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     5399 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_fixtures.py
--rw-r--r--   0        0        0     2396 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     7491 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     1022 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2881 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     4362 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0    13594 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_remove_refs.py
--rw-r--r--   0        0        0    10927 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     3837 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 robocorp_tasks-3.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     2189 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/README.md
+-rw-r--r--   0        0        0     1565 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4325 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     7959 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1494 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     8261 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    28952 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      331 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_constants.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9934 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      242 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     5399 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_fixtures.py
+-rw-r--r--   0        0        0     2396 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     1022 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2881 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     4362 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0    13594 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_remove_refs.py
+-rw-r--r--   0        0        0    10927 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     3837 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:03:05.685310 robocorp_tasks-3.0.3/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 robocorp_tasks-3.0.3/PKG-INFO
```

### Comparing `robocorp_tasks-3.0.2/README.md` & `robocorp_tasks-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/pyproject.toml` & `robocorp_tasks-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "3.0.2"
+version = "3.0.3"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
@@ -19,19 +19,19 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 robocorp-log = ">=2.4,<3"
 psutil = "^5.0"
 docstring_parser_fork = "^0.0.5"
+packaging = "^24.0"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 types-psutil = "^5.9"
-packaging = "^24.0"
 
 # We just need it for tests. In runtime duck-typing is used to
 # check for `cls.parse_obj(dict)` and `cls.model_json_schema()`
 pydantic = "^2.6"
 
 [tool.isort]
 profile = "black"
```

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/__init__.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import Dict, Optional
 
 from ._fixtures import setup, teardown
 from ._protocols import ITask, Status
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(*args, **kwargs):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_callback.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_commands.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_commands.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_config.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_extension_points.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_plugin_manager.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_fixtures.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_interrupts.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_interrupts.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_remove_refs.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/_task.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/src/robocorp/tasks/cli.py` & `robocorp_tasks-3.0.3/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.2/PKG-INFO` & `robocorp_tasks-3.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 3.0.2
+Version: 3.0.3
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: docstring_parser_fork (>=0.0.5,<0.0.6)
+Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: psutil (>=5.0,<6.0)
 Requires-Dist: robocorp-log (>=2.4,<3)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
```

