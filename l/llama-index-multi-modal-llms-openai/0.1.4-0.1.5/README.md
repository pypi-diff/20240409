# Comparing `tmp/llama_index_multi_modal_llms_openai-0.1.4.tar.gz` & `tmp/llama_index_multi_modal_llms_openai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_multi_modal_llms_openai-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_multi_modal_llms_openai-0.1.5.tar", max compression
```

## Comparing `llama_index_multi_modal_llms_openai-0.1.4.tar` & `llama_index_multi_modal_llms_openai-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       50 2024-02-13 13:53:01.702563 llama_index_multi_modal_llms_openai-0.1.4/README.md
--rw-r--r--   0        0        0      102 2024-02-13 13:53:01.702770 llama_index_multi_modal_llms_openai-0.1.4/llama_index/multi_modal_llms/openai/__init__.py
--rw-r--r--   0        0        0    17949 2024-02-20 22:37:41.333213 llama_index_multi_modal_llms_openai-0.1.4/llama_index/multi_modal_llms/openai/base.py
--rw-r--r--   0        0        0     2817 2024-02-13 13:53:01.702919 llama_index_multi_modal_llms_openai-0.1.4/llama_index/multi_modal_llms/openai/utils.py
--rw-r--r--   0        0        0     1502 2024-02-21 18:29:30.126335 llama_index_multi_modal_llms_openai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_openai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-04-09 20:57:22.926890 llama_index_multi_modal_llms_openai-0.1.5/README.md
+-rw-r--r--   0        0        0      102 2024-04-09 20:57:22.926890 llama_index_multi_modal_llms_openai-0.1.5/llama_index/multi_modal_llms/openai/__init__.py
+-rw-r--r--   0        0        0    17949 2024-04-09 20:57:22.926890 llama_index_multi_modal_llms_openai-0.1.5/llama_index/multi_modal_llms/openai/base.py
+-rw-r--r--   0        0        0     2882 2024-04-09 20:57:22.926890 llama_index_multi_modal_llms_openai-0.1.5/llama_index/multi_modal_llms/openai/utils.py
+-rw-r--r--   0        0        0     1502 2024-04-09 20:57:22.926890 llama_index_multi_modal_llms_openai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_openai-0.1.5/PKG-INFO
```

### Comparing `llama_index_multi_modal_llms_openai-0.1.4/llama_index/multi_modal_llms/openai/base.py` & `llama_index_multi_modal_llms_openai-0.1.5/llama_index/multi_modal_llms/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_multi_modal_llms_openai-0.1.4/llama_index/multi_modal_llms/openai/utils.py` & `llama_index_multi_modal_llms_openai-0.1.5/llama_index/multi_modal_llms/openai/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 DEFAULT_OPENAI_API_TYPE = "open_ai"
 DEFAULT_OPENAI_API_BASE = "https://api.openai.com/v1"
 
 
 GPT4V_MODELS = {
     "gpt-4-vision-preview": 128000,
+    "gpt-4-turbo-2024-04-09": 128000,
+    "gpt-4-turbo": 128000,
 }
 
 
 MISSING_API_KEY_ERROR_MESSAGE = """No API key found for OpenAI.
 Please set either the OPENAI_API_KEY environment variable or \
 openai.api_key prior to initialization.
 API keys can be found or created at \
```

### Comparing `llama_index_multi_modal_llms_openai-0.1.4/pyproject.toml` & `llama_index_multi_modal_llms_openai-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index multi-modal-llms openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-multi-modal-llms-openai"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_multi_modal_llms_openai-0.1.4/PKG-INFO` & `llama_index_multi_modal_llms_openai-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-multi-modal-llms-openai
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index multi-modal-llms openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Multi-Modal-Llms Integration: Openai
```

