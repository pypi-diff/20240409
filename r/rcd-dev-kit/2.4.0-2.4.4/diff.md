# Comparing `tmp/rcd_dev_kit-2.4.0.tar.gz` & `tmp/rcd_dev_kit-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcd_dev_kit-2.4.0.tar", max compression
+gzip compressed data, was "rcd_dev_kit-2.4.4.tar", max compression
```

## Comparing `rcd_dev_kit-2.4.0.tar` & `rcd_dev_kit-2.4.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rwxr-xr-x   0        0        0     1079 2024-03-18 17:22:34.548471 rcd_dev_kit-2.4.0/LICENSE
--rw-r--r--   0        0        0     5662 2024-03-18 17:22:34.548471 rcd_dev_kit-2.4.0/README.md
--rw-r--r--   0        0        0     3593 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      135 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/__init__.py
--rw-r--r--   0        0        0     7119 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/README.md
--rw-r--r--   0        0        0      840 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/__init__.py
--rw-r--r--   0        0        0    15566 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/directus_operator.py
--rw-r--r--   0        0        0    24695 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
--rw-r--r--   0        0        0     8970 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/gcloud_operator.py
--rw-r--r--   0        0        0     4039 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/mview_operator.py
--rw-r--r--   0        0        0      484 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/mysql_operator.py
--rw-r--r--   0        0        0     3129 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/oip_api_operator.py
--rw-r--r--   0        0        0    68735 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/redshift_operator.py
--rw-r--r--   0        0        0     7856 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/s3_operator.py
--rw-r--r--   0        0        0    41001 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/snowflake_operator.py
--rw-r--r--   0        0        0     1567 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/README.md
--rw-r--r--   0        0        0       73 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/__init__.py
--rw-r--r--   0        0        0     4602 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/dictionary.py
--rw-r--r--   0        0        0     2805 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
--rw-r--r--   0        0        0      632 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/README.md
--rw-r--r--   0        0        0       75 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/__init__.py
--rw-r--r--   0        0        0      530 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/debug_decorator.py
--rw-r--r--   0        0        0      628 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/functional_decorator.py
--rw-r--r--   0        0        0     3567 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/README.md
--rw-r--r--   0        0        0      270 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/__init__.py
--rw-r--r--   0        0        0      334 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_as_bytes.py
--rw-r--r--   0        0        0     1711 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_detector.py
--rw-r--r--   0        0        0     8908 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_downloader.py
--rw-r--r--   0        0        0     2118 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_operator.py
--rw-r--r--   0        0        0     1390 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_writer.py
--rw-r--r--   0        0        0     1386 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/README.md
--rw-r--r--   0        0        0      206 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/__init__.py
--rw-r--r--   0        0        0     4115 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/checker.py
--rw-r--r--   0        0        0     3570 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/detector.py
--rw-r--r--   0        0        0     1127 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/io.py
--rw-r--r--   0        0        0      579 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/manipulator.py
--rw-r--r--   0        0        0     6152 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/normalizer.py
--rw-r--r--   0        0        0       85 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/sql_utils/__init__.py
--rw-r--r--   0        0        0    21107 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/sql_utils/sql2sf.py
--rw-r--r--   0        0        0     9032 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
--rw-r--r--   0        0        0        0 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/verification_utils/__init__.py
--rw-r--r--   0        0        0     1158 2024-03-18 17:22:34.552471 rcd_dev_kit-2.4.0/src/rcd_dev_kit/verification_utils/verifification.py
--rw-r--r--   0        0        0     8111 1970-01-01 00:00:00.000000 rcd_dev_kit-2.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1079 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/LICENSE
+-rw-r--r--   0        0        0     5662 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/README.md
+-rw-r--r--   0        0        0     3990 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/__init__.py
+-rw-r--r--   0        0        0     7119 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/README.md
+-rw-r--r--   0        0        0      840 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/__init__.py
+-rw-r--r--   0        0        0    15566 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/directus_operator.py
+-rw-r--r--   0        0        0    25464 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
+-rw-r--r--   0        0        0     8970 2024-04-09 11:23:41.328250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/gcloud_operator.py
+-rw-r--r--   0        0        0     4039 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/mview_operator.py
+-rw-r--r--   0        0        0      484 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/mysql_operator.py
+-rw-r--r--   0        0        0     3129 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/oip_api_operator.py
+-rw-r--r--   0        0        0    68735 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/redshift_operator.py
+-rw-r--r--   0        0        0     7856 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/s3_operator.py
+-rw-r--r--   0        0        0    41001 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/snowflake_operator.py
+-rw-r--r--   0        0        0     1567 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/README.md
+-rw-r--r--   0        0        0       73 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/__init__.py
+-rw-r--r--   0        0        0     4602 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/dictionary.py
+-rw-r--r--   0        0        0     2805 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
+-rw-r--r--   0        0        0      632 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/README.md
+-rw-r--r--   0        0        0       75 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/debug_decorator.py
+-rw-r--r--   0        0        0      628 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/functional_decorator.py
+-rw-r--r--   0        0        0     3567 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/README.md
+-rw-r--r--   0        0        0      270 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/__init__.py
+-rw-r--r--   0        0        0      334 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_as_bytes.py
+-rw-r--r--   0        0        0     1711 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_detector.py
+-rw-r--r--   0        0        0     8908 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_downloader.py
+-rw-r--r--   0        0        0     2118 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_operator.py
+-rw-r--r--   0        0        0     1390 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_writer.py
+-rw-r--r--   0        0        0     1386 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/README.md
+-rw-r--r--   0        0        0      206 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/__init__.py
+-rw-r--r--   0        0        0     4115 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/checker.py
+-rw-r--r--   0        0        0     3570 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/detector.py
+-rw-r--r--   0        0        0     1127 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/io.py
+-rw-r--r--   0        0        0      579 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/manipulator.py
+-rw-r--r--   0        0        0     6152 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/normalizer.py
+-rw-r--r--   0        0        0       85 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/sql_utils/__init__.py
+-rw-r--r--   0        0        0    21107 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/sql_utils/sql2sf.py
+-rw-r--r--   0        0        0     9032 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
+-rw-r--r--   0        0        0        0 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/verification_utils/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-09 11:23:41.332250 rcd_dev_kit-2.4.4/src/rcd_dev_kit/verification_utils/verifification.py
+-rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 rcd_dev_kit-2.4.4/PKG-INFO
```

### Comparing `rcd_dev_kit-2.4.0/LICENSE` & `rcd_dev_kit-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/README.md` & `rcd_dev_kit-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/pyproject.toml` & `rcd_dev_kit-2.4.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rcd-dev-kit"
-version = "2.4.0"
+version = "2.4.4"
 description = "Interact with OIP ecosystem."
 authors = ["Maxime KIEFFER", "Robin Sarfati"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
@@ -34,15 +34,15 @@
 elasticsearch = "^8.8.2"
 python-dotenv = "^1.0.0"
 py-markdown-table = "^0.4.0"
 tqdm = "^4.65.0"
 statsmodels = "^0.14.0"
 scikit-learn = "^1.3.0"
 sqlalchemy-redshift = "^0.8.14"
-
+nltk = "^3.8.1"
 # pyTest packages to be installed via extra package rcd-dev-kit[py_test]
 pytest = { version = "^7.4.0", optional = true }
 pytest-cov = { version = "^4.1.0", optional = true }
 
 # Google packages to be installed via extra package rcd-dev-kit[google]
 google = { version = "^3.0.0", optional = true }
 google-api-python-client = { version = "^2.47.0", optional = true }
@@ -55,20 +55,29 @@
 # Those packages are used mainly to generate automatically the doc html of the package.
 Sphinx = { version = "^7.2.6", optional = true }
 sphinx-rtd-theme = { version = "1.3.0", optional = true }
 sphinxcontrib-napoleon = { version = "0.7", optional = true }
 sphinx-autoapi = { version = "^3.0.0", optional = true }
 myst-parser = { version = "^2.0.0", optional = true }
 
+# llama dependency for ...
+# llama-index-vector-stores-elasticsearch = { version = "^0.1.5", optional = true }
+# llama-index-readers-elasticsearch = { version = "^0.1.3", optional = true }
+# llama-index-embeddings-huggingface = { version = "^0.2.0", optional = true }
+
 # Connectorx dependency for parallel reading from redshift
-connectorx = { version = "^0.3.2", optional = true }
-llama-index-vector-stores-elasticsearch = "^0.1.5"
-llama-index-readers-elasticsearch = "^0.1.3"
-llama-index-embeddings-huggingface = "^0.1.4"
+
+connectorx = "^0.3.2"
+
 [tool.poetry.extras]
+llama = [
+    "llama-index-vector-stores-elasticsearch",
+    "llama-index-readers-elasticsearch",
+    "llama-index-embeddings-huggingface",
+]
 py_test = ["pytest", "pytest-cov"]
 google = [
     "google",
     "google-api-python-client",
     "google-cloud-storage",
     "googletrans",
 ]
@@ -94,7 +103,12 @@
 
 [tool.pytest.ini_options] # Pytest Init Configs
 addopts = "-p no:warnings"
 
 [build-system] # setuptools
 requires = ["setuptools>=42", "wheel", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[[tool.poetry.source]]
+name = "tekkare-pypi"
+url = "https://europe-west1-python.pkg.dev/oip-cluster/tekkare-pypi/"
+priority = "supplemental"
```

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/README.md` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/__init__.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/directus_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/directus_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/elasticsearch_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/elasticsearch_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 import re
 import json
 import certifi
+import numpy as np
 import pandas as pd
 from datetime import datetime
 from typing import Any, Generator, Optional
 from elasticsearch import Elasticsearch
 from elasticsearch.exceptions import ConnectionTimeout
 from elasticsearch.helpers import parallel_bulk, bulk, scan
 from .. import decorator_manager
 from .directus_operator import upsert_es_indices
 from tqdm import tqdm
-
-from llama_index.embeddings.huggingface import HuggingFaceEmbedding
-from llama_index.vector_stores.elasticsearch import ElasticsearchStore
-from llama_index.core import (
-    VectorStoreIndex,
-    StorageContext,
-    Settings,
-    Document
-)
+import logging
+# from llama_index.embeddings.huggingface import HuggingFaceEmbedding
+# from llama_index.vector_stores.elasticsearch import ElasticsearchStore
+# from llama_index.core import (
+#     VectorStoreIndex,
+#     StorageContext,
+#     Settings,
+#     Document
+# )
+import sys
 def index_json_bulk_parallel(index: str, method: str, custom_mapping_json: Optional[dict] = None,
                              **kwargs: Any) -> None:
     """
     Function index_json_bulk_parallel.
     Use this function to send data to elasticsearch with bulk indexing and multi-threading.
 
     Args:
@@ -503,78 +505,90 @@
                 actions=self.get_generator(),  # This should return a generator of actions.
                 request_timeout=self._request_timeout,
         ):
             if not success:
                 # Print error information for unsuccessful indexing operations.
                 print(info)
 
-    @decorator_manager.timeit(program_name="Create a vector store")
-    def generate_vector_store(self, df:pd.DataFrame, index_name:str, field_concat_for_embedding:list[str], metadata_fields:list[str], model_name="NeuML/pubmedbert-base-embeddings"):
-        """
-        Creates a vector store by generating embeddings for each document in the provided DataFrame and indexing these documents into an Elasticsearch vector store.
-
-        This method processes the DataFrame by concatenating specified fields to create a text for each document, attaching specified metadata, generating embeddings using the SentenceTransformer library based on the concatenated text, and finally indexing these documents into Elasticsearch.
-
-        Parameters:
-        - df (pd.DataFrame): The DataFrame containing the data to be processed. Each row represents a document.
-        - index (str): The base name for the Elasticsearch index where the documents will be stored. The final index name will be '{index}_vstore'.
-        - field_concat_for_embedding (list of str): Fields from the DataFrame to be concatenated to form the text content of each document.
-        - metadata_fields (list of str): Fields from the DataFrame to be included as metadata for each document.
-        - model_name (str, optional): The model name to be used with the SentenceTransformer for generating embeddings. Defaults to "NeuML/pubmedbert-base-embeddings".
-
-        The method also uses class attributes for Elasticsearch connection details (host, user, password) to determine whether to connect to a local or remote Elasticsearch instance.
-
-        The generated vector store can be used for searching, similarity comparisons, and other vector-based operations supported by Elasticsearch.
-        """
-        documents = []
+    # disabling to avoid dependency on llama_index which is not stable enough
+    # @decorator_manager.timeit(program_name="Create a vector store")
+    # def generate_vector_store(self, df:pd.DataFrame, index_name:str, field_concat_for_embedding:list[str], metadata_fields:list[str], model_name="NeuML/pubmedbert-base-embeddings"):
+    #     """
+    #     Creates a vector store by generating embeddings for each document in the provided DataFrame and indexing these documents into an Elasticsearch vector store.
+
+    #     This method processes the DataFrame by concatenating specified fields to create a text for each document, attaching specified metadata, generating embeddings using the SentenceTransformer library based on the concatenated text, and finally indexing these documents into Elasticsearch.
+
+    #     Parameters:
+    #     - df (pd.DataFrame): The DataFrame containing the data to be processed. Each row represents a document.
+    #     - index (str): The base name for the Elasticsearch index where the documents will be stored. The final index name will be '{index}_vstore'.
+    #     - field_concat_for_embedding (list of str): Fields from the DataFrame to be concatenated to form the text content of each document.
+    #     - metadata_fields (list of str): Fields from the DataFrame to be included as metadata for each document.
+    #     - model_name (str, optional): The model name to be used with the SentenceTransformer for generating embeddings. Defaults to "NeuML/pubmedbert-base-embeddings".
+
+    #     The method also uses class attributes for Elasticsearch connection details (host, user, password) to determine whether to connect to a local or remote Elasticsearch instance.
+
+    #     The generated vector store can be used for searching, similarity comparisons, and other vector-based operations supported by Elasticsearch.
+    #     """
+    #     documents = []
         
-        # Iterate through DataFrame rows with a progress bar
-        for index, row in tqdm(df.iterrows(), total=df.shape[0], desc="Generating documents"):
-            # Create text by concatenating specified fields
-            text = ' '.join([str(row[field]) for field in field_concat_for_embedding])
+    #     # Iterate through DataFrame rows with a progress bar
+    #     for index, row in tqdm(df.iterrows(), total=df.shape[0], desc="Generating documents"):
+    #         # Create text by concatenating specified fields
+    #         text = ' '.join([str(row[field]) for field in field_concat_for_embedding])
             
-            # Prepare metadata using specified fields
-            metadata = {field: row[field] for field in metadata_fields}
-            
-            # Create Document with text and metadata
-            document = Document(text=text, metadata=metadata)
-            documents.append(document)
+    #         # Prepare metadata using specified fields
+    #         metadata = {field: row[field] for field in metadata_fields if not (isinstance(row[field], (list, np.ndarray)) and not row[field])}
+    #         for field in metadata_fields:
+    #             try:
+    #                 if pd.notnull(row[field]):
+    #                     # This line is just for debugging; remove or replace with appropriate handling
+    #                     # print(f"Field {field} is not null.")
+    #                     pass  # Add an indented block here
+    #             except ValueError as e:
+    #                 print(f"Error with field {field}: {e}")
 
-        Settings.embed_model = HuggingFaceEmbedding(
-             model_name=model_name
-        )
-        host = os.environ.get("ELASTICSEARCH_HOST")
-        user = os.environ.get("ELASTICSEARCH_USER")
-        password = os.environ.get("ELASTICSEARCH_PASSWORD")
-        scheme = os.environ.get("ELASTICSEARCH_SCHEME")
-        port = int(os.environ.get("ELASTICSEARCH_PORT"))
-        url = scheme+'://'+host+':'+str(port)
-        print(url)
 
-        if not "localhost" in host:
-            vector_store = ElasticsearchStore(
-                es_url=url,
-                es_user=user,
-                es_password=password,
-                index_name=index_name+'_vstore',
-            )
-        else: 
-            vector_store = ElasticsearchStore(
-                es_url=url,
-                index_name=index_name+'_vstore',
-            )
 
-        storage_context = StorageContext.from_defaults(vector_store=vector_store)
-        print(documents[0])
-        index = VectorStoreIndex.from_documents(
-            documents, storage_context=storage_context
-        )
+            
+    #         # Create Document with text and metadata
+    #         document = Document(text=text, metadata=metadata)
+    #         documents.append(document)
+
+    #     Settings.embed_model = HuggingFaceEmbedding(
+    #          model_name=model_name
+    #     )
+    #     host = os.environ.get("ELASTICSEARCH_HOST")
+    #     user = os.environ.get("ELASTICSEARCH_USER")
+    #     password = os.environ.get("ELASTICSEARCH_PASSWORD")
+    #     scheme = os.environ.get("ELASTICSEARCH_SCHEME")
+    #     port = int(os.environ.get("ELASTICSEARCH_PORT"))
+    #     url = scheme+'://'+host+':'+str(port)
+    #     print(url)
+
+    #     if not "localhost" in host:
+    #         vector_store = ElasticsearchStore(
+    #             es_url=url,
+    #             es_user=user,
+    #             es_password=password,
+    #             index_name=index_name+'_vstore',
+    #         )
+    #     else: 
+    #         vector_store = ElasticsearchStore(
+    #             es_url=url,
+    #             index_name=index_name+'_vstore',
+    #         )
+
+    #     storage_context = StorageContext.from_defaults(vector_store=vector_store)
+    #     print(documents[0])
+    #     index = VectorStoreIndex.from_documents(
+    #         documents, storage_context=storage_context
+    #     )
 
-        # if not "localhost" in self.host:
-        #     send_metadata(es_connector=self.connection, index=False)
+    #     # if not "localhost" in self.host:
+    #     #     send_metadata(es_connector=self.connection, index=False)
 
 
     @decorator_manager.timeit(program_name="Dropping Index")
     def delete_index(self):
         self.connection.indices.delete(index=self.index, ignore=[400, 404])
```

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/gcloud_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/gcloud_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/mview_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/mview_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/oip_api_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/oip_api_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/redshift_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/redshift_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/s3_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/s3_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/database_manager/snowflake_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/database_manager/snowflake_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/README.md` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/dictionary.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/dictionary.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/dataclass_manager/raw_data_file.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/dataclass_manager/raw_data_file.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/README.md` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/debug_decorator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/debug_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/decorator_manager/functional_decorator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/decorator_manager/functional_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/README.md` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_detector.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_downloader.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_downloader.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_operator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/file_manager/file_writer.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/file_manager/file_writer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/README.md` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/checker.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/checker.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/detector.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/io.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/io.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/manipulator.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/manipulator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/pandas_manager/normalizer.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/pandas_manager/normalizer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/sql_utils/sql2sf.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/sql_utils/sql2sf.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/src/rcd_dev_kit/verification_utils/verifification.py` & `rcd_dev_kit-2.4.4/src/rcd_dev_kit/verification_utils/verifification.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.0/PKG-INFO` & `rcd_dev_kit-2.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcd-dev-kit
-Version: 2.4.0
+Version: 2.4.4
 Summary: Interact with OIP ecosystem.
 Home-page: https://github.com/Tekkare/rcd-dev-kit
 License: MIT
 Author: Maxime KIEFFER
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,28 +14,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: ctx
 Provides-Extra: docs
 Provides-Extra: google
+Provides-Extra: llama
 Provides-Extra: py-test
 Requires-Dist: Sphinx (>=7.2.6,<8.0.0) ; extra == "docs"
 Requires-Dist: boto3 (>=1.28.12,<2.0.0)
 Requires-Dist: botocore (>=1.31.12,<2.0.0)
 Requires-Dist: connectorx (>=0.3.2,<0.4.0) ; extra == "ctx"
 Requires-Dist: elasticsearch (>=8.8.2,<9.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0) ; extra == "google"
 Requires-Dist: google-api-python-client (>=2.47.0,<3.0.0) ; extra == "google"
 Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
 Requires-Dist: google-cloud-storage (>=2.3.0,<3.0.0) ; extra == "google"
-Requires-Dist: llama-index-embeddings-huggingface (>=0.1.4,<0.2.0)
-Requires-Dist: llama-index-readers-elasticsearch (>=0.1.3,<0.2.0)
-Requires-Dist: llama-index-vector-stores-elasticsearch (>=0.1.5,<0.2.0)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0) ; extra == "docs"
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: py-markdown-table (>=0.4.0,<0.5.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0) ; extra == "py-test"
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "py-test"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

