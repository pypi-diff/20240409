# Comparing `tmp/unifyai-0.6.0.tar.gz` & `tmp/unifyai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.6.0.tar", max compression
+gzip compressed data, was "unifyai-0.7.0.tar", max compression
```

## Comparing `unifyai-0.6.0.tar` & `unifyai-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.6.0/LICENSE
--rw-r--r--   0        0        0     5948 2024-04-08 11:43:57.646202 unifyai-0.6.0/README.md
--rw-r--r--   0        0        0     1019 2024-04-08 11:43:25.750203 unifyai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.6.0/unifyai/__init__.py
--rw-r--r--   0        0        0    15103 2024-04-08 11:43:25.750203 unifyai-0.6.0/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.6.0/unifyai/exceptions.py
--rw-r--r--   0        0        0     4325 2024-04-08 11:43:25.750203 unifyai-0.6.0/unifyai/tests.py
--rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.6.0/unifyai/utils.py
--rw-r--r--   0        0        0     6631 1970-01-01 00:00:00.000000 unifyai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6205 2024-04-09 08:55:32.372336 unifyai-0.7.0/README.md
+-rw-r--r--   0        0        0     1019 2024-04-09 08:55:21.824336 unifyai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-04-09 08:55:37.160336 unifyai-0.7.0/unifyai/__init__.py
+-rw-r--r--   0        0        0     3623 2024-04-09 09:03:52.572359 unifyai-0.7.0/unifyai/chat.py
+-rw-r--r--   0        0        0    15103 2024-04-08 11:43:25.750203 unifyai-0.7.0/unifyai/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.7.0/unifyai/exceptions.py
+-rw-r--r--   0        0        0     4325 2024-04-08 11:43:25.750203 unifyai-0.7.0/unifyai/tests.py
+-rw-r--r--   0        0        0     1822 2024-04-08 11:43:25.750203 unifyai-0.7.0/unifyai/utils.py
+-rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 unifyai-0.7.0/PKG-INFO
```

### Comparing `unifyai-0.6.0/LICENSE` & `unifyai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.6.0/README.md` & `unifyai-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -163,7 +163,16 @@
 You can see the provider chosen by printing the `.provider` attribute of the client:
 
 ```python
 print(unify.provider)
 ```
 
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
+
+## ChatBot Agent
+Our `ChatBot` allows you to start an interactive chat session with any of our supported llm endpoints with only a few lines of code:
+
+```python
+from unifyai import ChatBot
+chat = ChatBot(endpoint="llama-2-7b-chat@anyscale")
+chat.run()
+```
```

### Comparing `unifyai-0.6.0/pyproject.toml` & `unifyai-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.6.0"
+version = "0.7.0"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify-llm-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.6.0/unifyai/clients.py` & `unifyai-0.7.0/unifyai/clients.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.6.0/unifyai/exceptions.py` & `unifyai-0.7.0/unifyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.6.0/unifyai/tests.py` & `unifyai-0.7.0/unifyai/tests.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.6.0/unifyai/utils.py` & `unifyai-0.7.0/unifyai/utils.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.6.0/PKG-INFO` & `unifyai-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify-llm-python
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -182,7 +182,16 @@
 
 ```python
 print(unify.provider)
 ```
 
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
 
+## ChatBot Agent
+Our `ChatBot` allows you to start an interactive chat session with any of our supported llm endpoints with only a few lines of code:
+
+```python
+from unifyai import ChatBot
+chat = ChatBot(endpoint="llama-2-7b-chat@anyscale")
+chat.run()
+```
+
```

