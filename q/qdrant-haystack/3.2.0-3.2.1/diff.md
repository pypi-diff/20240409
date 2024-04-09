# Comparing `tmp/qdrant_haystack-3.2.0.tar.gz` & `tmp/qdrant_haystack-3.2.1.tar.gz`

## Comparing `qdrant_haystack-3.2.0.tar` & `qdrant_haystack-3.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/pydoc/config.yml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/src/haystack_integrations/components/retrievers/qdrant/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/__init__.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/converters.py
--rw-r--r--   0        0        0    18939 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/document_store.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/test_converters.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/test_dict_converters.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/test_filters.py
--rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/test_legacy_filters.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/README.md
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/pydoc/config.yml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/components/retrievers/qdrant/__init__.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/components/retrievers/qdrant/retriever.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/converters.py
+-rw-r--r--   0        0        0    18939 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/document_store.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_converters.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_dict_converters.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_document_store.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_filters.py
+-rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_legacy_filters.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/README.md
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 qdrant_haystack-3.2.1/PKG-INFO
```

### Comparing `qdrant_haystack-3.2.0/pydoc/config.yml` & `qdrant_haystack-3.2.1/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py` & `qdrant_haystack-3.2.1/src/haystack_integrations/components/retrievers/qdrant/retriever.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/converters.py` & `qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/document_store.py` & `qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/document_store.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/src/haystack_integrations/document_stores/qdrant/filters.py` & `qdrant_haystack-3.2.1/src/haystack_integrations/document_stores/qdrant/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/tests/test_converters.py` & `qdrant_haystack-3.2.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/tests/test_dict_converters.py` & `qdrant_haystack-3.2.1/tests/test_dict_converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/tests/test_document_store.py` & `qdrant_haystack-3.2.1/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/tests/test_filters.py` & `qdrant_haystack-3.2.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/tests/test_legacy_filters.py` & `qdrant_haystack-3.2.1/tests/test_legacy_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/tests/test_retriever.py` & `qdrant_haystack-3.2.1/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/.gitignore` & `qdrant_haystack-3.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/LICENSE.txt` & `qdrant_haystack-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/README.md` & `qdrant_haystack-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.2.0/pyproject.toml` & `qdrant_haystack-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["haystack-ai>=2.0.0b6", "qdrant-client"]
+dependencies = ["haystack-ai", "qdrant-client"]
 
 [project.urls]
 Source = "https://github.com/deepset-ai/haystack-core-integrations"
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/qdrant/README.md"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `qdrant_haystack-3.2.0/PKG-INFO` & `qdrant_haystack-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qdrant-haystack
-Version: 3.2.0
+Version: 3.2.1
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/qdrant/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: Kacper Łukawski <kacper.lukawski@qdrant.com>, Anush Shetty <anush.shetty@qdrant.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: haystack-ai>=2.0.0b6
+Requires-Dist: haystack-ai
 Requires-Dist: qdrant-client
 Description-Content-Type: text/markdown
 
 # qdrant-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/qdrant-haystack.svg)](https://pypi.org/project/qdrant-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qdrant-haystack.svg)](https://pypi.org/project/qdrant-haystack)
```

