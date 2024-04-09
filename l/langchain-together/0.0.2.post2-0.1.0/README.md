# Comparing `tmp/langchain_together-0.0.2.post2.tar.gz` & `tmp/langchain_together-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_together-0.0.2.post2.tar", max compression
+gzip compressed data, was "langchain_together-0.1.0.tar", max compression
```

## Comparing `langchain_together-0.0.2.post2.tar` & `langchain_together-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/LICENSE
--rw-r--r--   0        0        0     1031 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/README.md
--rw-r--r--   0        0        0      233 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/langchain_together/__init__.py
--rw-r--r--   0        0        0     1657 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/langchain_together/embeddings.py
--rw-r--r--   0        0        0     8059 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/langchain_together/llms.py
--rw-r--r--   0        0        0        0 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/langchain_together/py.typed
--rw-r--r--   0        0        0      232 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/langchain_together/version.py
--rw-r--r--   0        0        0     2569 2024-04-09 19:19:04.727754 langchain_together-0.0.2.post2/pyproject.toml
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 langchain_together-0.0.2.post2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 19:24:18.852840 langchain_together-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1031 2024-04-09 19:24:18.852840 langchain_together-0.1.0/README.md
+-rw-r--r--   0        0        0      233 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/__init__.py
+-rw-r--r--   0        0        0     1657 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/embeddings.py
+-rw-r--r--   0        0        0     8059 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/llms.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/py.typed
+-rw-r--r--   0        0        0      232 2024-04-09 19:24:18.852840 langchain_together-0.1.0/langchain_together/version.py
+-rw-r--r--   0        0        0     2563 2024-04-09 19:24:18.852840 langchain_together-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1927 1970-01-01 00:00:00.000000 langchain_together-0.1.0/PKG-INFO
```

### Comparing `langchain_together-0.0.2.post2/LICENSE` & `langchain_together-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_together-0.0.2.post2/README.md` & `langchain_together-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_together-0.0.2.post2/langchain_together/embeddings.py` & `langchain_together-0.1.0/langchain_together/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_together-0.0.2.post2/langchain_together/llms.py` & `langchain_together-0.1.0/langchain_together/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_together-0.0.2.post2/pyproject.toml` & `langchain_together-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-together"
-version = "0.0.2.post2"
+version = "0.1.0"
 description = "An integration package connecting Together and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_together-0.0.2.post2/PKG-INFO` & `langchain_together-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-together
-Version: 0.0.2.post2
+Version: 0.1.0
 Summary: An integration package connecting Together and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

