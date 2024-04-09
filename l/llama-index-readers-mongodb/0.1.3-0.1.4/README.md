# Comparing `tmp/llama_index_readers_mongodb-0.1.3.tar.gz` & `tmp/llama_index_readers_mongodb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_mongodb-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_mongodb-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_mongodb-0.1.3.tar` & `llama_index_readers_mongodb-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       40 2024-02-13 13:53:01.832381 llama_index_readers_mongodb-0.1.3/README.md
--rw-r--r--   0        0        0       96 2024-02-13 13:53:01.832601 llama_index_readers_mongodb-0.1.3/llama_index/readers/mongodb/__init__.py
--rw-r--r--   0        0        0     3511 2024-02-13 13:53:01.832655 llama_index_readers_mongodb-0.1.3/llama_index/readers/mongodb/base.py
--rw-r--r--   0        0        0     1489 2024-02-21 20:27:01.027155 llama_index_readers_mongodb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 llama_index_readers_mongodb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/README.md
+-rw-r--r--   0        0        0       96 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/llama_index/readers/mongodb/__init__.py
+-rw-r--r--   0        0        0     3629 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/llama_index/readers/mongodb/base.py
+-rw-r--r--   0        0        0     1489 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 llama_index_readers_mongodb-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_mongodb-0.1.3/llama_index/readers/mongodb/base.py` & `llama_index_readers_mongodb-0.1.4/llama_index/readers/mongodb/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,19 @@
                 to the metadata attribute of the Document. Defaults to None
 
         Returns:
             List[Document]: A list of documents.
 
         """
         db = self.client[db_name]
-        cursor = db[collection_name].find(filter=query_dict or {}, limit=max_docs)
+        cursor = db[collection_name].find(
+            filter=query_dict or {},
+            limit=max_docs,
+            projection={name: 1 for name in field_names + (metadata_names or [])},
+        )
 
         for item in cursor:
             try:
                 texts = [item[name] for name in field_names]
             except KeyError as err:
                 raise ValueError(
                     f"{err.args[0]} field not found in Mongo document."
```

### Comparing `llama_index_readers_mongodb-0.1.3/pyproject.toml` & `llama_index_readers_mongodb-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers mongodb integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["jerryjliu"]
 name = "llama-index-readers-mongodb"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymongo = "^4.6.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_mongodb-0.1.3/PKG-INFO` & `llama_index_readers_mongodb-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-mongodb
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers mongodb integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: jerryjliu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: pymongo (>=4.6.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Readers Integration: Mongo
```

