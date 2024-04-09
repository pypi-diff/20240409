# Comparing `tmp/mongodb_atlas_haystack-0.2.0.tar.gz` & `tmp/mongodb_atlas_haystack-0.2.1.tar.gz`

## Comparing `mongodb_atlas_haystack-0.2.0.tar` & `mongodb_atlas_haystack-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/examples/example.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/pydoc/config.yml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/src/haystack_integrations/components/retrievers/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/src/haystack_integrations/document_stores/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/src/haystack_integrations/document_stores/mongodb_atlas/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/tests/test_embedding_retrieval.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/README.md
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/examples/example.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/pydoc/config.yml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/components/retrievers/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    12792 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/test_document_store.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/test_embedding_retrieval.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/README.md
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/PKG-INFO
```

### Comparing `mongodb_atlas_haystack-0.2.0/examples/example.py` & `mongodb_atlas_haystack-0.2.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/pydoc/config.yml` & `mongodb_atlas_haystack-0.2.1/pydoc/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -20,11 +20,12 @@
   excerpt: MongoDB Atlas integration for Haystack
   category_slug: integrations-api
   title: MongoDB Atlas
   slug: integrations-mongodb-atlas
   order: 160
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_mongodb_atlas.md
```

### Comparing `mongodb_atlas_haystack-0.2.0/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py` & `mongodb_atlas_haystack-0.2.1/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py` & `mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -166,15 +166,27 @@
             if not isinstance(documents[0], Document):
                 msg = "param 'documents' must contain a list of objects of type Document"
                 raise ValueError(msg)
 
         if policy == DuplicatePolicy.NONE:
             policy = DuplicatePolicy.FAIL
 
-        mongo_documents = [doc.to_dict(flatten=False) for doc in documents]
+        mongo_documents = []
+        for doc in documents:
+            doc_dict = doc.to_dict(flatten=False)
+            if "sparse_embedding" in doc_dict:
+                sparse_embedding = doc_dict.pop("sparse_embedding", None)
+                if sparse_embedding:
+                    logger.warning(
+                        "Document %s has the `sparse_embedding` field set,"
+                        "but storing sparse embeddings in MongoDB Atlas is not currently supported."
+                        "The `sparse_embedding` field will be ignored.",
+                        doc.id,
+                    )
+            mongo_documents.append(doc_dict)
         operations: List[Union[UpdateOne, InsertOne, ReplaceOne]]
         written_docs = len(documents)
 
         if policy == DuplicatePolicy.SKIP:
             operations = [UpdateOne({"id": doc["id"]}, {"$setOnInsert": doc}, upsert=True) for doc in mongo_documents]
             existing_documents = self.collection.count_documents({"id": {"$in": [doc.id for doc in documents]}})
             written_docs -= existing_documents
```

### Comparing `mongodb_atlas_haystack-0.2.0/src/haystack_integrations/document_stores/mongodb_atlas/filters.py` & `mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/filters.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/tests/test_document_store.py` & `mongodb_atlas_haystack-0.2.1/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/tests/test_embedding_retrieval.py` & `mongodb_atlas_haystack-0.2.1/tests/test_embedding_retrieval.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/tests/test_retriever.py` & `mongodb_atlas_haystack-0.2.1/tests/test_retriever.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from unittest.mock import Mock
+from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 from haystack.dataclasses import Document
 from haystack.utils.auth import EnvVarSecret
 from haystack_integrations.components.retrievers.mongodb_atlas import MongoDBAtlasEmbeddingRetriever
 from haystack_integrations.document_stores.mongodb_atlas import MongoDBAtlasDocumentStore
 
 
-@pytest.fixture
-def document_store():
-    store = MongoDBAtlasDocumentStore(
-        database_name="haystack_integration_test",
-        collection_name="test_embeddings_collection",
-        vector_search_index="cosine_index",
-    )
-    return store
-
-
 class TestRetriever:
-    def test_init_default(self, document_store: MongoDBAtlasDocumentStore):
-        retriever = MongoDBAtlasEmbeddingRetriever(document_store=document_store)
-        assert retriever.document_store == document_store
+
+    @pytest.fixture
+    def mock_client(self):
+        with patch(
+            "haystack_integrations.document_stores.mongodb_atlas.document_store.MongoClient"
+        ) as mock_mongo_client:
+            mock_connection = MagicMock()
+            mock_database = MagicMock()
+            mock_collection_names = MagicMock(return_value=["test_embeddings_collection"])
+            mock_database.list_collection_names = mock_collection_names
+            mock_connection.__getitem__.return_value = mock_database
+            mock_mongo_client.return_value = mock_connection
+            yield mock_mongo_client
+
+    def test_init_default(self):
+        mock_store = Mock(spec=MongoDBAtlasDocumentStore)
+        retriever = MongoDBAtlasEmbeddingRetriever(document_store=mock_store)
+        assert retriever.document_store == mock_store
         assert retriever.filters == {}
         assert retriever.top_k == 10
 
-    def test_init(self, document_store: MongoDBAtlasDocumentStore):
+    def test_init(self):
+        mock_store = Mock(spec=MongoDBAtlasDocumentStore)
         retriever = MongoDBAtlasEmbeddingRetriever(
-            document_store=document_store,
+            document_store=mock_store,
             filters={"field": "value"},
             top_k=5,
         )
-        assert retriever.document_store == document_store
+        assert retriever.document_store == mock_store
         assert retriever.filters == {"field": "value"}
         assert retriever.top_k == 5
 
-    def test_to_dict(self, document_store: MongoDBAtlasDocumentStore):
+    def test_to_dict(self, mock_client, monkeypatch):  # noqa: ARG002  mock_client appears unused but is required
+        monkeypatch.setenv("MONGO_CONNECTION_STRING", "test_conn_str")
+
+        document_store = MongoDBAtlasDocumentStore(
+            database_name="haystack_integration_test",
+            collection_name="test_embeddings_collection",
+            vector_search_index="cosine_index",
+        )
+
         retriever = MongoDBAtlasEmbeddingRetriever(document_store=document_store, filters={"field": "value"}, top_k=5)
         res = retriever.to_dict()
         assert res == {
             "type": "haystack_integrations.components.retrievers.mongodb_atlas.embedding_retriever.MongoDBAtlasEmbeddingRetriever",  # noqa: E501
             "init_parameters": {
                 "document_store": {
                     "type": "haystack_integrations.document_stores.mongodb_atlas.document_store.MongoDBAtlasDocumentStore",  # noqa: E501
@@ -57,15 +71,17 @@
                     },
                 },
                 "filters": {"field": "value"},
                 "top_k": 5,
             },
         }
 
-    def test_from_dict(self):
+    def test_from_dict(self, mock_client, monkeypatch):  # noqa: ARG002  mock_client appears unused but is required
+        monkeypatch.setenv("MONGO_CONNECTION_STRING", "test_conn_str")
+
         data = {
             "type": "haystack_integrations.components.retrievers.mongodb_atlas.embedding_retriever.MongoDBAtlasEmbeddingRetriever",  # noqa: E501
             "init_parameters": {
                 "document_store": {
                     "type": "haystack_integrations.document_stores.mongodb_atlas.document_store.MongoDBAtlasDocumentStore",  # noqa: E501
                     "init_parameters": {
                         "mongo_connection_string": {
```

### Comparing `mongodb_atlas_haystack-0.2.0/.gitignore` & `mongodb_atlas_haystack-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/LICENSE.txt` & `mongodb_atlas_haystack-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/README.md` & `mongodb_atlas_haystack-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.0/pyproject.toml` & `mongodb_atlas_haystack-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "haystack-ai>=2.0.0b6",
+  "haystack-ai",
   "pymongo[srv]",
 ]
 
 [project.urls]
 Source = "https://github.com/deepset-ai/haystack-core-integrations"
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/mongodb_atlas/README.md"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
@@ -90,20 +90,20 @@
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
```

### Comparing `mongodb_atlas_haystack-0.2.0/PKG-INFO` & `mongodb_atlas_haystack-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mongodb-atlas-haystack
-Version: 0.2.0
+Version: 0.2.1
 Summary: An integration of MongoDB Atlas with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/mongodb_atlas/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: haystack-ai>=2.0.0b6
+Requires-Dist: haystack-ai
 Requires-Dist: pymongo[srv]
 Description-Content-Type: text/markdown
 
 # mongodb-atlas-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mongodb-atlas-haystack.svg)](https://pypi.org/project/mongodb-atlas-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mongodb-atlas-haystack.svg)](https://pypi.org/project/mongodb-atlas-haystack)
```

