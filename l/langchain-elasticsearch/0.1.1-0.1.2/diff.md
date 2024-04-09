# Comparing `tmp/langchain_elasticsearch-0.1.1.tar.gz` & `tmp/langchain_elasticsearch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_elasticsearch-0.1.1.tar", max compression
+gzip compressed data, was "langchain_elasticsearch-0.1.2.tar", max compression
```

## Comparing `langchain_elasticsearch-0.1.1.tar` & `langchain_elasticsearch-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/LICENSE
--rw-r--r--   0        0        0     2493 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/README.md
--rw-r--r--   0        0        0      618 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/__init__.py
--rw-r--r--   0        0        0     3211 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/_utilities.py
--rw-r--r--   0        0        0     5417 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/chat_history.py
--rw-r--r--   0        0        0     1094 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/client.py
--rw-r--r--   0        0        0     7862 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/embeddings.py
--rw-r--r--   0        0        0        0 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/py.typed
--rw-r--r--   0        0        0     3859 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/retrievers.py
--rw-r--r--   0        0        0    46916 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/langchain_elasticsearch/vectorstores.py
--rw-r--r--   0        0        0     2640 2024-03-12 17:22:41.932676 langchain_elasticsearch-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3272 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/README.md
+-rw-r--r--   0        0        0      618 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4075 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/_utilities.py
+-rw-r--r--   0        0        0     5417 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/chat_history.py
+-rw-r--r--   0        0        0     1094 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/client.py
+-rw-r--r--   0        0        0     7862 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/py.typed
+-rw-r--r--   0        0        0     4764 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/retrievers.py
+-rw-r--r--   0        0        0    49912 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/langchain_elasticsearch/vectorstores.py
+-rw-r--r--   0        0        0     2315 2024-04-09 12:49:24.467584 langchain_elasticsearch-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.1.2/PKG-INFO
```

### Comparing `langchain_elasticsearch-0.1.1/LICENSE` & `langchain_elasticsearch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.1/README.md` & `langchain_elasticsearch-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -45,14 +45,45 @@
     es_cloud_id="your-cloud-id",
     es_api_key="your-api-key",
     index_name="your-index-name",
     embeddings=embeddings,
 )
 ```
 
+### ElasticsearchRetriever
+
+The `ElasticsearchRetriever` class can be user to implement more complex queries.
+This can be useful for power users and necessary if data was ingested outside of LangChain
+(for example using a web crawler).
+
+```python
+def fuzzy_query(search_query: str) -> Dict:
+    return {
+        "query": {
+            "match": {
+                text_field: {
+                    "query": search_query,
+                    "fuzziness": "AUTO",
+                }
+            },
+        },
+    }
+
+
+fuzzy_retriever = ElasticsearchRetriever.from_es_params(
+    es_cloud_id="your-cloud-id",
+    es_api_key="your-api-key",
+    index_name="your-index-name",
+    body_func=fuzzy_query,
+    content_field=text_field,
+)
+
+fuzzy_retriever.get_relevant_documents("fooo")
+```
+
 ### ElasticsearchEmbeddings
 
 The `ElasticsearchEmbeddings` class provides an interface to generate embeddings using a model
 deployed in an Elasticsearch cluster.
 
 ```python
 from langchain_elasticsearch import ElasticsearchEmbeddings
```

### Comparing `langchain_elasticsearch-0.1.1/langchain_elasticsearch/__init__.py` & `langchain_elasticsearch-0.1.2/langchain_elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.1/langchain_elasticsearch/chat_history.py` & `langchain_elasticsearch-0.1.2/langchain_elasticsearch/chat_history.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.1/langchain_elasticsearch/client.py` & `langchain_elasticsearch-0.1.2/langchain_elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.1/langchain_elasticsearch/embeddings.py` & `langchain_elasticsearch-0.1.2/langchain_elasticsearch/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.1/langchain_elasticsearch/retrievers.py` & `langchain_elasticsearch-0.1.2/langchain_elasticsearch/retrievers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Union, cast
 
 from elasticsearch import Elasticsearch
 from langchain_core.callbacks import CallbackManagerForRetrieverRun
 from langchain_core.documents import Document
 from langchain_core.retrievers import BaseRetriever
 
 from langchain_elasticsearch._utilities import with_user_agent_header
@@ -15,49 +15,59 @@
 class ElasticsearchRetriever(BaseRetriever):
     """
     Elasticsearch retriever
 
     Args:
         es_client: Elasticsearch client connection. Alternatively you can use the
             `from_es_params` method with parameters to initialize the client.
-        index_name: The name of the index to query.
+        index_name: The name of the index to query. Can also be a list of names.
         body_func: Function to create an Elasticsearch DSL query body from a search
             string. The returned query body must fit what you would normally send in a
             POST request the the _search endpoint. If applicable, it also includes
             parameters the `size` parameter etc.
-        content_field: The document field name that contains the page content.
+        content_field: The document field name that contains the page content. If
+            multiple indices are queried, specify a dict {index_name: field_name} here.
         document_mapper: Function to map Elasticsearch hits to LangChain Documents.
     """
 
     es_client: Elasticsearch
-    index_name: str
+    index_name: Union[str, Sequence[str]]
     body_func: Callable[[str], Dict]
-    content_field: Optional[str] = None
-    document_mapper: Optional[Callable[[Dict], Document]] = None
+    content_field: Optional[Union[str, Mapping[str, str]]] = None
+    document_mapper: Optional[Callable[[Mapping], Document]] = None
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
         if self.content_field is None and self.document_mapper is None:
             raise ValueError("One of content_field or document_mapper must be defined.")
         if self.content_field is not None and self.document_mapper is not None:
             raise ValueError(
                 "Both content_field and document_mapper are defined. "
                 "Please provide only one."
             )
 
-        self.document_mapper = self.document_mapper or self._field_mapper
+        if not self.document_mapper:
+            if isinstance(self.content_field, str):
+                self.document_mapper = self._single_field_mapper
+            elif isinstance(self.content_field, Mapping):
+                self.document_mapper = self._multi_field_mapper
+            else:
+                raise ValueError(
+                    "unknown type for content_field, expected string or dict."
+                )
+
         self.es_client = with_user_agent_header(self.es_client, "langchain-py-r")
 
     @staticmethod
     def from_es_params(
-        index_name: str,
+        index_name: Union[str, Sequence[str]],
         body_func: Callable[[str], Dict],
-        content_field: Optional[str] = None,
-        document_mapper: Optional[Callable[[Dict], Document]] = None,
+        content_field: Optional[Union[str, Mapping[str, str]]] = None,
+        document_mapper: Optional[Callable[[Mapping], Document]] = None,
         url: Optional[str] = None,
         cloud_id: Optional[str] = None,
         api_key: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         params: Optional[Dict[str, Any]] = None,
     ) -> "ElasticsearchRetriever":
@@ -89,10 +99,16 @@
         if not self.es_client or not self.document_mapper:
             raise ValueError("faulty configuration")  # should not happen
 
         body = self.body_func(query)
         results = self.es_client.search(index=self.index_name, body=body)
         return [self.document_mapper(hit) for hit in results["hits"]["hits"]]
 
-    def _field_mapper(self, hit: Dict[str, Any]) -> Document:
+    def _single_field_mapper(self, hit: Mapping[str, Any]) -> Document:
         content = hit["_source"].pop(self.content_field)
         return Document(page_content=content, metadata=hit)
+
+    def _multi_field_mapper(self, hit: Mapping[str, Any]) -> Document:
+        self.content_field = cast(Mapping, self.content_field)
+        field = self.content_field[hit["_index"]]
+        content = hit["_source"].pop(field)
+        return Document(page_content=content, metadata=hit)
```

### Comparing `langchain_elasticsearch-0.1.1/langchain_elasticsearch/vectorstores.py` & `langchain_elasticsearch-0.1.2/langchain_elasticsearch/vectorstores.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
 from langchain_elasticsearch._utilities import (
     DistanceStrategy,
     maximal_marginal_relevance,
+    model_must_be_deployed,
     with_user_agent_header,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class BaseRetrievalStrategy(ABC):
@@ -65,24 +66,26 @@
         """
 
     @abstractmethod
     def index(
         self,
         dims_length: Union[int, None],
         vector_query_field: str,
+        text_field: str,
         similarity: Union[DistanceStrategy, None],
     ) -> Dict:
         """
         Executes when the index is created.
 
         Args:
             dims_length: Numeric length of the embedding vectors,
                         or None if not using vector-based query.
             vector_query_field: The field containing the vector
                                 representations in the index.
+            text_field: The field containing the text data in the index.
             similarity: The similarity strategy to use,
                         or None if not using one.
 
         Returns:
             Dict: The Elasticsearch settings and mappings for the strategy.
         """
 
@@ -195,18 +198,25 @@
             elif isinstance(self.rrf, bool) and self.rrf is True:
                 query_body["rank"] = {"rrf": {}}
 
             return query_body
         else:
             return {"knn": knn}
 
+    def before_index_setup(
+        self, client: "Elasticsearch", text_field: str, vector_query_field: str
+    ) -> None:
+        if self.query_model_id:
+            model_must_be_deployed(client, self.query_model_id)
+
     def index(
         self,
         dims_length: Union[int, None],
         vector_query_field: str,
+        text_field: str,
         similarity: Union[DistanceStrategy, None],
     ) -> Dict:
         """Create the mapping for the Elasticsearch index."""
 
         if similarity is DistanceStrategy.COSINE:
             similarityAlgo = "cosine"
         elif similarity is DistanceStrategy.EUCLIDEAN_DISTANCE:
@@ -278,14 +288,15 @@
             }
         }
 
     def index(
         self,
         dims_length: Union[int, None],
         vector_query_field: str,
+        text_field: str,
         similarity: Union[DistanceStrategy, None],
     ) -> Dict:
         """Create the mapping for the Elasticsearch index."""
 
         return {
             "mappings": {
                 "properties": {
@@ -336,16 +347,18 @@
 
     def _get_pipeline_name(self) -> str:
         return f"{self.model_id}_sparse_embedding"
 
     def before_index_setup(
         self, client: "Elasticsearch", text_field: str, vector_query_field: str
     ) -> None:
-        # If model_id is provided, create a pipeline for the model
         if self.model_id:
+            model_must_be_deployed(client, self.model_id)
+
+            # Create a pipeline for the model
             client.ingest.put_pipeline(
                 id=self._get_pipeline_name(),
                 description="Embedding pipeline for langchain vectorstore",
                 processors=[
                     {
                         "inference": {
                             "model_id": self.model_id,
@@ -359,14 +372,15 @@
                 ],
             )
 
     def index(
         self,
         dims_length: Union[int, None],
         vector_query_field: str,
+        text_field: str,
         similarity: Union[DistanceStrategy, None],
     ) -> Dict:
         return {
             "mappings": {
                 "properties": {
                     vector_query_field: {
                         "properties": {"tokens": {"type": "rank_features"}}
@@ -376,14 +390,84 @@
             "settings": {"default_pipeline": self._get_pipeline_name()},
         }
 
     def require_inference(self) -> bool:
         return False
 
 
+class BM25RetrievalStrategy(BaseRetrievalStrategy):
+    """Retrieval strategy using the native BM25 algorithm of Elasticsearch."""
+
+    def __init__(self, k1: Union[float, None] = None, b: Union[float, None] = None):
+        self.k1 = k1
+        self.b = b
+
+    def query(
+        self,
+        query_vector: Union[List[float], None],
+        query: Union[str, None],
+        k: int,
+        fetch_k: int,
+        vector_query_field: str,
+        text_field: str,
+        filter: List[dict],
+        similarity: Union[DistanceStrategy, None],
+    ) -> Dict:
+        return {
+            "query": {
+                "bool": {
+                    "must": [
+                        {
+                            "match": {
+                                text_field: {
+                                    "query": query,
+                                }
+                            },
+                        },
+                    ],
+                    "filter": filter,
+                },
+            },
+        }
+
+    def index(
+        self,
+        dims_length: Union[int, None],
+        vector_query_field: str,
+        text_field: str,
+        similarity: Union[DistanceStrategy, None],
+    ) -> Dict:
+        mappings: Dict = {
+            "properties": {
+                text_field: {
+                    "type": "text",
+                    "similarity": "custom_bm25",
+                },
+            },
+        }
+        settings: Dict = {
+            "similarity": {
+                "custom_bm25": {
+                    "type": "BM25",
+                },
+            },
+        }
+
+        if self.k1 is not None:
+            settings["similarity"]["custom_bm25"]["k1"] = self.k1
+
+        if self.b is not None:
+            settings["similarity"]["custom_bm25"]["b"] = self.b
+
+        return {"mappings": mappings, "settings": settings}
+
+    def require_inference(self) -> bool:
+        return False
+
+
 class ElasticsearchStore(VectorStore):
     """`Elasticsearch` vector store.
 
     Example:
         .. code-block:: python
 
             from langchain_elasticsearch.vectorstores import ElasticsearchStore
@@ -892,14 +976,15 @@
                 client=self.client,
                 text_field=self.query_field,
                 vector_query_field=self.vector_query_field,
             )
 
             indexSettings = self.strategy.index(
                 vector_query_field=self.vector_query_field,
+                text_field=self.query_field,
                 dims_length=dims_length,
                 similarity=self.distance_strategy,
             )
             logger.debug(
                 f"Creating index {index_name} with mappings {indexSettings['mappings']}"
             )
             self.client.indices.create(index=index_name, **indexSettings)
@@ -1271,7 +1356,21 @@
         Args:
             model_id: Optional. Default is ".elser_model_1".
                     ID of the model to use to embed the query text
                     within the stack. Requires embedding model to be
                     deployed to Elasticsearch.
         """
         return SparseRetrievalStrategy(model_id=model_id)
+
+    @staticmethod
+    def BM25RetrievalStrategy(
+        k1: Union[float, None] = None, b: Union[float, None] = None
+    ) -> "BM25RetrievalStrategy":
+        """Used to apply BM25 without vector search.
+
+        Args:
+            k1: Optional. This corresponds to the BM25 parameter, k1. Default is None,
+                which uses the default setting of Elasticsearch.
+            b: Optional. This corresponds to the BM25 parameter, b. Default is None,
+               which uses the default setting of Elasticsearch.
+        """
+        return BM25RetrievalStrategy(k1=k1, b=b)
```

### Comparing `langchain_elasticsearch-0.1.1/pyproject.toml` & `langchain_elasticsearch-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "langchain-elasticsearch"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting Elasticsearch and LangChain"
 authors = []
 readme = "README.md"
-repository = "https://github.com/langchain-ai/langchain"
+repository = "https://github.com/langchain-ai/langchain-elastic"
 license = "MIT"
 
 [tool.poetry.urls]
-"Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/elasticsearch"
+"Source Code" = "https://github.com/langchain-ai/langchain-elastic/tree/main/libs/elasticsearch"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1"
 elasticsearch = "^8.12.0"
 numpy = "^1"
 
@@ -22,17 +22,16 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain = { path = "../../langchain", develop = true }
-langchain-core = { path = "../../core", develop = true }
-langchain-text-splitters = {path = "../../text-splitters", develop = true}
+langchain = "^0.1.13"
+langchain-text-splitters = ">=0.0.1,<0.1"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -40,21 +39,19 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
-langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 
 
@@ -87,10 +84,9 @@
 # --snapshot-warn-unused    Prints a warning on unused snapshots rather than fail the test suite.
 addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
 # Registering custom markers.
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
-  "compile: mark placeholder test used to compile integration tests without running them",
 ]
 asyncio_mode = "auto"
```

