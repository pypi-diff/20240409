# Comparing `tmp/llama_index_storage_index_store_elasticsearch-0.1.2.tar.gz` & `tmp/llama_index_storage_index_store_elasticsearch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_index_store_elasticsearch-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_storage_index_store_elasticsearch-0.1.3.tar", max compression
```

## Comparing `llama_index_storage_index_store_elasticsearch-0.1.2.tar` & `llama_index_storage_index_store_elasticsearch-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       64 2024-03-25 01:30:08.809882 llama_index_storage_index_store_elasticsearch-0.1.2/README.md
--rw-r--r--   0        0        0      126 2024-03-25 01:30:08.809882 llama_index_storage_index_store_elasticsearch-0.1.2/llama_index/storage/index_store/elasticsearch/__init__.py
--rw-r--r--   0        0        0      682 2024-03-25 01:30:08.809882 llama_index_storage_index_store_elasticsearch-0.1.2/llama_index/storage/index_store/elasticsearch/base.py
--rw-r--r--   0        0        0     1549 2024-03-25 01:30:08.809882 llama_index_storage_index_store_elasticsearch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 llama_index_storage_index_store_elasticsearch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-04-09 18:35:55.042438 llama_index_storage_index_store_elasticsearch-0.1.3/README.md
+-rw-r--r--   0        0        0      126 2024-04-09 18:35:55.042438 llama_index_storage_index_store_elasticsearch-0.1.3/llama_index/storage/index_store/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-09 18:35:55.042438 llama_index_storage_index_store_elasticsearch-0.1.3/llama_index/storage/index_store/elasticsearch/base.py
+-rw-r--r--   0        0        0     1549 2024-04-09 18:35:55.042438 llama_index_storage_index_store_elasticsearch-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 llama_index_storage_index_store_elasticsearch-0.1.3/PKG-INFO
```

### Comparing `llama_index_storage_index_store_elasticsearch-0.1.2/llama_index/storage/index_store/elasticsearch/base.py` & `llama_index_storage_index_store_elasticsearch-0.1.3/llama_index/storage/index_store/elasticsearch/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,11 +12,16 @@
         namespace (str): namespace for the index store
 
     """
 
     def __init__(
         self,
         elasticsearch_kvstore: ElasticsearchKVStore,
+        collection_index: Optional[str] = None,
         namespace: Optional[str] = None,
     ) -> None:
         """Init a ElasticsearchIndexStore."""
         super().__init__(elasticsearch_kvstore, namespace=namespace)
+        if collection_index:
+            self._collection = collection_index
+        else:
+            self._collection = f"llama_index-index_store.data-{self._namespace}"
```

### Comparing `llama_index_storage_index_store_elasticsearch-0.1.2/pyproject.toml` & `llama_index_storage_index_store_elasticsearch-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index index_store elasticsearch integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-index-store-elasticsearch"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-storage-kvstore-elasticsearch = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_storage_index_store_elasticsearch-0.1.2/PKG-INFO` & `llama_index_storage_index_store_elasticsearch-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-index-store-elasticsearch
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index index_store elasticsearch integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

