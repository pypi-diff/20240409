# Comparing `tmp/unifyai-0.7.0.tar.gz` & `tmp/unifyai-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.7.0.tar", max compression
+gzip compressed data, was "unifyai-0.7.1.tar", max compression
```

## Comparing `unifyai-0.7.0.tar` & `unifyai-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.7.0/LICENSE
--rw-r--r--   0        0        0     6205 2024-04-09 08:55:32.372336 unifyai-0.7.0/README.md
--rw-r--r--   0        0        0     1019 2024-04-09 08:55:21.824336 unifyai-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      135 2024-04-09 08:55:37.160336 unifyai-0.7.0/unifyai/__init__.py
--rw-r--r--   0        0        0     3623 2024-04-09 09:03:52.572359 unifyai-0.7.0/unifyai/chat.py
--rw-r--r--   0        0        0    15103 2024-04-08 11:43:25.750203 unifyai-0.7.0/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.7.0/unifyai/exceptions.py
--rw-r--r--   0        0        0     4325 2024-04-08 11:43:25.750203 unifyai-0.7.0/unifyai/tests.py
--rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.7.0/unifyai/utils.py
--rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 unifyai-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6205 2024-04-09 08:55:32.372336 unifyai-0.7.1/README.md
+-rw-r--r--   0        0        0     1019 2024-04-09 09:30:12.528433 unifyai-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-04-09 09:26:47.592423 unifyai-0.7.1/unifyai/__init__.py
+-rw-r--r--   0        0        0     3631 2024-04-09 09:29:52.252432 unifyai-0.7.1/unifyai/chat.py
+-rw-r--r--   0        0        0    15103 2024-04-08 11:43:25.750203 unifyai-0.7.1/unifyai/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.7.1/unifyai/exceptions.py
+-rw-r--r--   0        0        0     4325 2024-04-08 11:43:25.750203 unifyai-0.7.1/unifyai/tests.py
+-rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.7.1/unifyai/utils.py
+-rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 unifyai-0.7.1/PKG-INFO
```

### Comparing `unifyai-0.7.0/LICENSE` & `unifyai-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.0/README.md` & `unifyai-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.0/pyproject.toml` & `unifyai-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.7.0"
+version = "0.7.1"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify-llm-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.7.0/unifyai/chat.py` & `unifyai-0.7.1/unifyai/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from unifyai import Unify
+from unifyai.clients import Unify
 
 
 class ChatBot:  # noqa: WPS338
     """Agent class represents an LLM chat agent."""
 
     def __init__(self, endpoint: str) -> None:
         """
```

### Comparing `unifyai-0.7.0/unifyai/clients.py` & `unifyai-0.7.1/unifyai/clients.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.0/unifyai/exceptions.py` & `unifyai-0.7.1/unifyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.0/unifyai/tests.py` & `unifyai-0.7.1/unifyai/tests.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.0/unifyai/utils.py` & `unifyai-0.7.1/unifyai/utils.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.7.0/PKG-INFO` & `unifyai-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify-llm-python
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

