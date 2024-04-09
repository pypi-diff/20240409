# Comparing `tmp/astra_haystack-0.5.0.tar.gz` & `tmp/astra_haystack-0.5.1.tar.gz`

## Comparing `astra_haystack-0.5.0.tar` & `astra_haystack-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/__init__.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/examples/example.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/examples/pipeline_example.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/examples/requirements.txt
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/examples/data/usr_01.txt
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/pydoc/config.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/components/retrievers/astra/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/components/retrievers/astra/retriever.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/__init__.py
--rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/astra_client.py
--rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/document_store.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/errors.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/filters.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0    10434 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/tests/test_document_store.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/LICENSE
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/README.md
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 astra_haystack-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/__init__.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/example.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/pipeline_example.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/requirements.txt
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/examples/data/usr_01.txt
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/pydoc/config.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/components/retrievers/astra/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/components/retrievers/astra/retriever.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/__init__.py
+-rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/astra_client.py
+-rw-r--r--   0        0        0    17243 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/document_store.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/errors.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/filters.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0    10434 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/tests/test_document_store.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/README.md
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 astra_haystack-0.5.1/PKG-INFO
```

### Comparing `astra_haystack-0.5.0/examples/example.py` & `astra_haystack-0.5.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/examples/pipeline_example.py` & `astra_haystack-0.5.1/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/examples/data/usr_01.txt` & `astra_haystack-0.5.1/examples/data/usr_01.txt`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/pydoc/config.yml` & `astra_haystack-0.5.1/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/src/haystack_integrations/components/retrievers/astra/retriever.py` & `astra_haystack-0.5.1/src/haystack_integrations/components/retrievers/astra/retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/astra_client.py` & `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/astra_client.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/document_store.py` & `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,23 @@
                     )
                     raise Exception(msg)
 
             if "dataframe" in document_dict and document_dict["dataframe"] is not None:
                 document_dict["dataframe"] = document_dict.pop("dataframe").to_json()
             if embedding := document_dict.pop("embedding", []):
                 document_dict["$vector"] = embedding
+            if "sparse_embedding" in document_dict:
+                sparse_embedding = document_dict.pop("sparse_embedding", None)
+                if sparse_embedding:
+                    logger.warning(
+                        "Document %s has the `sparse_embedding` field set,"
+                        "but storing sparse embeddings in Astra is not currently supported."
+                        "The `sparse_embedding` field will be ignored.",
+                        document_dict["_id"],
+                    )
 
             return document_dict
 
         documents_to_write = [_convert_input_document(doc) for doc in documents]
 
         duplicate_documents = []
         new_documents = []
```

### Comparing `astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/errors.py` & `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/errors.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/src/haystack_integrations/document_stores/astra/filters.py` & `astra_haystack-0.5.1/src/haystack_integrations/document_stores/astra/filters.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/tests/test_document_store.py` & `astra_haystack-0.5.1/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/tests/test_retriever.py` & `astra_haystack-0.5.1/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/.gitignore` & `astra_haystack-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/LICENSE` & `astra_haystack-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/README.md` & `astra_haystack-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.5.0/pyproject.toml` & `astra_haystack-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "astra-haystack"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Anant Corporation", email = "support@anant.us" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -64,15 +63,15 @@
   "test-cov",
   "cov-report",
 ]
 docs = [
   "pydoc-markdown pydoc/config.yml"
 ]
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
@@ -93,20 +92,20 @@
   "typing",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
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

### Comparing `astra_haystack-0.5.0/PKG-INFO` & `astra_haystack-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.3
 Name: astra-haystack
-Version: 0.5.0
+Version: 0.5.1
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra
 Author-email: Anant Corporation <support@anant.us>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: astrapy
 Requires-Dist: haystack-ai
 Requires-Dist: pydantic
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 [![test](https://github.com/deepset-ai/document-store/actions/workflows/test.yml/badge.svg)](https://github.com/deepset-ai/document-store/actions/workflows/test.yml)
```

