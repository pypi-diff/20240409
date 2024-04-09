# Comparing `tmp/sibila-0.3.6.tar.gz` & `tmp/sibila-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sibila-0.3.6.tar", last modified: Sat Mar 16 19:34:55 2024, max compression
+gzip compressed data, was "sibila-0.4.0.tar", last modified: Tue Apr  9 16:07:32 2024, max compression
```

## Comparing `sibila-0.3.6.tar` & `sibila-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-16 19:34:55.305471 sibila-0.3.6/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.3.6/LICENSE
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4059 2024-03-16 19:34:55.305471 sibila-0.3.6/PKG-INFO
--rwxrwxr-x   0 jorge     (1000) jorge     (1000)     2906 2024-03-08 16:59:25.000000 sibila-0.3.6/README.md
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1515 2024-03-14 15:55:16.000000 sibila-0.3.6/pyproject.toml
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-03-16 19:34:55.305471 sibila-0.3.6/setup.cfg
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-16 19:34:55.301471 sibila-0.3.6/sibila/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1059 2024-03-16 16:43:56.000000 sibila-0.3.6/sibila/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.3.6/sibila/cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.3.6/sibila/context.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8539 2024-03-14 20:51:16.000000 sibila-0.3.6/sibila/gen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.3.6/sibila/json_grammar.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    24842 2024-02-29 16:28:12.000000 sibila-0.3.6/sibila/json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    22610 2024-03-16 19:27:11.000000 sibila-0.3.6/sibila/llamacpp.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    45686 2024-03-16 19:09:06.000000 sibila-0.3.6/sibila/model.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    46429 2024-03-16 19:00:08.000000 sibila-0.3.6/sibila/models.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.3.6/sibila/multigen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1989 2024-02-26 20:11:39.000000 sibila-0.3.6/sibila/null.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    15319 2024-03-16 19:21:25.000000 sibila-0.3.6/sibila/openai.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-16 19:34:55.305471 sibila-0.3.6/sibila/res/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.3.6/sibila/res/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    12207 2024-03-16 12:14:11.000000 sibila-0.3.6/sibila/res/base_formats.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1255 2024-03-16 17:45:06.000000 sibila-0.3.6/sibila/res/base_models.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.3.6/sibila/text_splitter.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20173 2024-03-16 18:23:26.000000 sibila-0.3.6/sibila/thread.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    13113 2024-03-14 18:11:32.000000 sibila-0.3.6/sibila/tools.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1236 2024-03-14 11:27:35.000000 sibila-0.3.6/sibila/utils.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-16 19:34:55.305471 sibila-0.3.6/sibila.egg-info/
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4059 2024-03-16 19:34:55.000000 sibila-0.3.6/sibila.egg-info/PKG-INFO
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      817 2024-03-16 19:34:55.000000 sibila-0.3.6/sibila.egg-info/SOURCES.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-03-16 19:34:55.000000 sibila-0.3.6/sibila.egg-info/dependency_links.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-03-16 19:34:55.000000 sibila-0.3.6/sibila.egg-info/entry_points.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       83 2024-03-16 19:34:55.000000 sibila-0.3.6/sibila.egg-info/requires.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-03-16 19:34:55.000000 sibila-0.3.6/sibila.egg-info/top_level.txt
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-16 19:34:55.305471 sibila-0.3.6/tests/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    11688 2024-03-11 10:47:12.000000 sibila-0.3.6/tests/test_cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    26039 2024-03-16 16:47:43.000000 sibila-0.3.6/tests/test_examples_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4123 2024-03-09 13:18:06.000000 sibila-0.3.6/tests/test_extract.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.3.6/tests/test_formats.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.3.6/tests/test_json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1300 2024-03-16 18:22:24.000000 sibila-0.3.6/tests/test_llamacpp_models.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     6158 2024-03-16 16:47:08.000000 sibila-0.3.6/tests/test_llamacpp_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4226 2024-03-16 18:56:20.000000 sibila-0.3.6/tests/test_openai_gpt35.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4191 2024-03-16 18:56:42.000000 sibila-0.3.6/tests/test_openai_gpt4.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.290619 sibila-0.4.0/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.0/LICENSE
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4497 2024-04-09 16:07:32.290619 sibila-0.4.0/PKG-INFO
+-rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3299 2024-04-09 15:35:13.000000 sibila-0.4.0/README.md
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1560 2024-04-08 14:27:47.000000 sibila-0.4.0/pyproject.toml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-04-09 16:07:32.290619 sibila-0.4.0/setup.cfg
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.286619 sibila-0.4.0/sibila/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1249 2024-04-09 16:03:20.000000 sibila-0.4.0/sibila/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.0/sibila/cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.0/sibila/context.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    10254 2024-04-08 09:50:19.000000 sibila-0.4.0/sibila/gen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.0/sibila/json_grammar.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    24842 2024-02-29 16:28:12.000000 sibila-0.4.0/sibila/json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    23851 2024-04-08 14:31:59.000000 sibila-0.4.0/sibila/llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    16156 2024-04-09 11:12:16.000000 sibila-0.4.0/sibila/mistral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    73925 2024-04-09 11:29:20.000000 sibila-0.4.0/sibila/model.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    47337 2024-04-07 11:35:48.000000 sibila-0.4.0/sibila/models.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.0/sibila/multigen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2280 2024-04-08 14:52:24.000000 sibila-0.4.0/sibila/null.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    21650 2024-04-09 11:16:34.000000 sibila-0.4.0/sibila/openai.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.286619 sibila-0.4.0/sibila/res/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.0/sibila/res/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    12204 2024-04-08 15:05:04.000000 sibila-0.4.0/sibila/res/base_formats.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1620 2024-04-07 11:16:28.000000 sibila-0.4.0/sibila/res/base_models.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    15392 2024-04-09 11:17:44.000000 sibila-0.4.0/sibila/schema_format_openai.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.0/sibila/text_splitter.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20173 2024-03-16 18:23:26.000000 sibila-0.4.0/sibila/thread.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.0/sibila/tools.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1236 2024-03-14 11:27:35.000000 sibila-0.4.0/sibila/utils.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.290619 sibila-0.4.0/sibila.egg-info/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4497 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/PKG-INFO
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      962 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/SOURCES.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/dependency_links.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/entry_points.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      113 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/requires.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-04-09 16:07:32.000000 sibila-0.4.0/sibila.egg-info/top_level.txt
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-09 16:07:32.290619 sibila-0.4.0/tests/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    11688 2024-03-11 10:47:12.000000 sibila-0.4.0/tests/test_cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20550 2024-04-08 16:10:27.000000 sibila-0.4.0/tests/test_examples_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6696 2024-04-08 11:31:34.000000 sibila-0.4.0/tests/test_fireworks_mixtral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.0/tests/test_formats.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.4.0/tests/test_json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1375 2024-03-16 19:37:51.000000 sibila-0.4.0/tests/test_llamacpp_models.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7566 2024-04-08 16:12:48.000000 sibila-0.4.0/tests/test_llamacpp_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6369 2024-04-08 11:08:30.000000 sibila-0.4.0/tests/test_mistral_small.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4613 2024-04-04 18:27:52.000000 sibila-0.4.0/tests/test_null_extract.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6298 2024-04-08 11:15:51.000000 sibila-0.4.0/tests/test_openai_gpt35.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6287 2024-04-08 11:16:00.000000 sibila-0.4.0/tests/test_openai_gpt4.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     6576 2024-04-08 11:28:50.000000 sibila-0.4.0/tests/test_together_mixtral.py
```

### Comparing `sibila-0.3.6/LICENSE` & `sibila-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/PKG-INFO` & `sibila-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.3.6
+Version: 0.4.0
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
@@ -16,32 +16,35 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: llama-cpp-python
-Requires-Dist: jinja2
-Requires-Dist: typing_extensions
-Requires-Dist: jsonschema
-Requires-Dist: openai
+Requires-Dist: llama-cpp-python>=0.2
+Requires-Dist: openai>=1.1
 Requires-Dist: tiktoken
-Requires-Dist: pydantic
+Requires-Dist: mistralai
+Requires-Dist: jinja2>=3.0
+Requires-Dist: jsonschema
+Requires-Dist: pydantic>=2.0
+Requires-Dist: typing_extensions
 Requires-Dist: tqdm
 
 # Sibila
 
-Extract structured data from remote or local file LLM models.
+Extract structured data from remote or local LLM models. Predictable output is essential for any serious use of LLMs.
 
 - Extract data into Pydantic objects, dataclasses or simple types.
-- Same API for local file models and remote OpenAI models.
-- Model management: download models, manage configuration and quickly switch between models.
+- Same API for local file models and remote OpenAI, Mistral AI and other models.
+- Model management: download models, manage configuration, quickly switch between models.
 - Tools for evaluating output across local/remote models, for chat-like interaction and more.
 
+No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
+
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
 To extract structured data from a local model:
 
 ``` python
 from sibila import Models
 from pydantic import BaseModel
@@ -72,29 +75,30 @@
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
 
-If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass.
+If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass. Also includes asynchronous access to remote models.
+
 
 
 
 ## Docs
 
 [The docs explain](https://jndiogo.github.io/sibila/) the main concepts, include examples and an API reference.
 
 
 ## Installation
 
 Sibila can be installed from PyPI by doing:
 
 ```
-pip install sibila
+pip install --upgrade sibila
 ```
 
 See [Getting started](https://jndiogo.github.io/sibila/installing/) for more information.
 
 
 
 ## Examples
@@ -118,13 +122,13 @@
 - [TheBloke (Tom Jobbins)](https://huggingface.co/TheBloke) and [Hugging Face model hub](https://huggingface.co/)
 
 Thank you!
 
 
 ## Sibila?
 
-Sibila is the Portuguese word for Sibyl. [The Sibyls](https://en.wikipedia.org/wiki/Sibyl) were wise oracular women in ancient Greece. Their mysterious words puzzled people throughout the centuries, providing insight or prophetic predictions.
+Sibila is the Portuguese word for Sibyl. [The Sibyls](https://en.wikipedia.org/wiki/Sibyl) were wise oracular women in ancient Greece. Their mysterious words puzzled people throughout the centuries, providing insight or prophetic predictions, "uttering things not to be laughed at".
 
 ![Michelangelo's Delphic Sibyl, Sistine Chapel ceiling](https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/DelphicSibylByMichelangelo.jpg/471px-DelphicSibylByMichelangelo.jpg)
 
 Michelangelo's Delphic Sibyl, in the Sistine Chapel ceiling.
```

### Comparing `sibila-0.3.6/README.md` & `sibila-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Sibila
 
-Extract structured data from remote or local file LLM models.
+Extract structured data from remote or local LLM models. Predictable output is essential for any serious use of LLMs.
 
 - Extract data into Pydantic objects, dataclasses or simple types.
-- Same API for local file models and remote OpenAI models.
-- Model management: download models, manage configuration and quickly switch between models.
+- Same API for local file models and remote OpenAI, Mistral AI and other models.
+- Model management: download models, manage configuration, quickly switch between models.
 - Tools for evaluating output across local/remote models, for chat-like interaction and more.
 
+No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
+
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
 To extract structured data from a local model:
 
 ``` python
 from sibila import Models
 from pydantic import BaseModel
@@ -41,29 +43,30 @@
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
 
-If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass.
+If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass. Also includes asynchronous access to remote models.
+
 
 
 
 ## Docs
 
 [The docs explain](https://jndiogo.github.io/sibila/) the main concepts, include examples and an API reference.
 
 
 ## Installation
 
 Sibila can be installed from PyPI by doing:
 
 ```
-pip install sibila
+pip install --upgrade sibila
 ```
 
 See [Getting started](https://jndiogo.github.io/sibila/installing/) for more information.
 
 
 
 ## Examples
@@ -87,13 +90,13 @@
 - [TheBloke (Tom Jobbins)](https://huggingface.co/TheBloke) and [Hugging Face model hub](https://huggingface.co/)
 
 Thank you!
 
 
 ## Sibila?
 
-Sibila is the Portuguese word for Sibyl. [The Sibyls](https://en.wikipedia.org/wiki/Sibyl) were wise oracular women in ancient Greece. Their mysterious words puzzled people throughout the centuries, providing insight or prophetic predictions.
+Sibila is the Portuguese word for Sibyl. [The Sibyls](https://en.wikipedia.org/wiki/Sibyl) were wise oracular women in ancient Greece. Their mysterious words puzzled people throughout the centuries, providing insight or prophetic predictions, "uttering things not to be laughed at".
 
 ![Michelangelo's Delphic Sibyl, Sistine Chapel ceiling](https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/DelphicSibylByMichelangelo.jpg/471px-DelphicSibylByMichelangelo.jpg)
 
 Michelangelo's Delphic Sibyl, in the Sistine Chapel ceiling.
```

### Comparing `sibila-0.3.6/pyproject.toml` & `sibila-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,22 @@
     "Programming Language :: Python :: 3.13",
 
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
-    "llama-cpp-python",
-    "jinja2",
-    "typing_extensions",
-    "jsonschema",
-    "openai",
+    "llama-cpp-python >= 0.2",
+    "openai >= 1.1",
     "tiktoken",
-    "pydantic",
+    "mistralai",
+    "jinja2 >= 3.0",
+    "jsonschema",
+    "pydantic >= 2.0",
+    "typing_extensions",
     "tqdm",
 ]
 dynamic = ["version"]
 
 
 [tool.setuptools.dynamic]
 version = {attr = "sibila.__version__"}
```

### Comparing `sibila-0.3.6/sibila/__init__.py` & `sibila-0.4.0/sibila/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Structured data from local or remote LLM models."""
 
-__version__ = "0.3.6"
+__version__ = "0.4.0"
 
 __all__ = [
     "Models",
     "Model", "TextModel", "MessagesModel", "Tokenizer",
     "GenConf", "GenRes", "GenError", "GenOut",
     "LlamaCppModel", "LlamaCppTokenizer",
     "OpenAIModel", "OpenAITokenizer",
+    "TogetherModel", "FireworksModel",
+    "MistralModel",
     "Thread", "MsgKind",
     "Context", "Trim",
     "JSchemaConf",
     "TDesc"
 ]
 
 __author__ = "Jorge Diogo"
@@ -43,14 +45,23 @@
 )
 
 from .openai import (
     OpenAIModel,
     OpenAITokenizer
 )
 
+from .schema_format_openai import (
+    TogetherModel,
+    FireworksModel
+)
+
+from .mistral import (
+    MistralModel
+)
+
 from .context import (
     Context,
     Trim
 )
 
 from .models import Models
```

### Comparing `sibila-0.3.6/sibila/cli.py` & `sibila-0.4.0/sibila/cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/context.py` & `sibila-0.4.0/sibila/context.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/gen.py` & `sibila-0.4.0/sibila/gen.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from typing import Any, Optional, Union, Callable
 from typing_extensions import Self
 from dataclasses import dataclass, field, asdict
 from enum import IntEnum
 
 import json
-from copy import copy
+from copy import deepcopy
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 
 
@@ -47,47 +47,63 @@
     """
 
     json_schema: Union[str,dict,None] = None
     """A JSON schema to validate the JSON output.
     Thread msgs must list the JSON schema and request its use; must also set the format to "json".
     """
     
+    special: Union[dict,None] = None
+    """Special model or provider-specific generation arguments. Args in the base dict are included unconditionally
+    for a model, while args in sub-keys with the model's provider name are only used for models from 
+    that provider, for example "openai": {...} values are only used in OpenAI models."""
+
     
     def __call__(self,
                  **kwargs: Any) -> Self:
         """Return a copy of the current GenConf updated with values in kwargs. Doesn't modify object.
+        Key 'special' is updated element-wise.
 
         Args:
             **kwargs: update settings of the same names in the returned copy.
 
         Raises:
             KeyError: If key does not exist.
 
         Returns:
             A copy of the current object with kwargs values updated. Doesn't modify object.
         """
 
-        ret = copy(self)
+        ret = deepcopy(self)
 
         for k,v in kwargs.items():
             if not hasattr(ret, k):
                 raise KeyError(f"No such key '{k}'")
-            setattr(ret, k,v)
+            if k == "special":
+                if ret.special is None:
+                    ret.special = {}
+                if v is None:
+                    v = {}
+                ret.special.update(v)
+                if not ret.special:
+                    ret.special = None
+            else:
+                setattr(ret, k,v)
 
         return ret
 
 
     def clone(self) -> Self:
-        """Return a copy of this configuration."""
-        return copy(self)
+        """Return a deep copy of this configuration."""
+        return deepcopy(self)
         
     def as_dict(self) -> dict:
         """Return GenConf as a dict."""
         return asdict(self)
 
+
     @staticmethod
     def from_dict(dic: dict) -> Any: # Any = GenConf
         return GenConf(**dic)
 
     def resolve_max_tokens(self,
                            ctx_len: int,
                            max_tokens_limit: Optional[int] = None) -> int:
@@ -111,14 +127,43 @@
                 max_tokens = max(1,max_tokens)
         if max_tokens_limit is not None:
             max_tokens = min(max_tokens, max_tokens_limit)
 
         return max_tokens
 
 
+    def resolve_special(self, 
+                        provider: Optional[str] = None) -> dict:
+        """Compiles settings from the 'special' field, for model and provider.
+
+        Args:
+            provider: If set will include any 'special' settings specified for that provider, inside a key named after the provider. If not given, only base keys are added.
+
+        Returns:
+            _description_
+        """
+
+        if self.special is None:
+            return {}
+
+        from .models import Models
+
+        out = {}
+        for k,v in self.special.items():
+            if k == provider: # provider-specific
+                if not isinstance(v,dict):
+                    raise ValueError(f"Config 'special' for provider '{provider}' must be a dict.")
+                out.update(v)
+            else: # common args
+                if isinstance(v,dict) and k in Models.ALL_PROVIDER_NAMES: # skip other provider entries
+                    continue
+                out[k] = v
+        return out
+
+
 
 
 
 class GenRes(IntEnum):
     """Model generation result."""
 
     OK_STOP = 1
```

### Comparing `sibila-0.3.6/sibila/json_grammar.py` & `sibila-0.4.0/sibila/json_grammar.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/json_schema.py` & `sibila-0.4.0/sibila/json_schema.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/llamacpp.py` & `sibila-0.4.0/sibila/llamacpp.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,31 +60,34 @@
     Supports grammar-constrained JSON output following a JSON schema.
 
     Attributes:
         ctx_len: Maximum context length, shared for input + output.
         desc: Model information.
     """
 
+    PROVIDER_NAME:str = "llamacpp"
+    """Provider prefix that this class handles."""
+
     _llama: Llama
     """LlamaCpp instance"""
 
     def __init__(self,
                  path: str,
 
                  format: Optional[str] = None,                 
                  format_search_order: list[str] = ["name", "meta_template", "folder_json"],
 
                  *,
 
                  # common base model args
                  genconf: Optional[GenConf] = None,
                  schemaconf: Optional[JSchemaConf] = None,
-                 tokenizer: Optional[Tokenizer] = None,
                  ctx_len: Optional[int] = None,
                  max_tokens_limit: Optional[int] = None,
+                 tokenizer: Optional[Tokenizer] = None,
 
                  # important LlamaCpp-specific args
                  n_gpu_layers: int = -1,
                  main_gpu: int = 0,
                  n_batch: int = 512,
                  seed: int = 4294967295,
                  verbose: bool = False,
@@ -95,17 +98,17 @@
         """
         Args:
             path: File path to the GGUF file.
             format: Chat template format to use with model. Leave as None for auto-detection.
             format_search_order: Search order for auto-detecting format, "name" searches in the filename, "meta_template" looks in the model's metadata, "folder_json" looks for configs in file's folder. Defaults to ["name","meta_template", "folder_json"].
             genconf: Default generation configuration, which can be used in gen() and related. Defaults to None.
             schemaconf: Default configuration for JSON schema validation, used if generation call doesn't supply one. Defaults to None.
-            tokenizer: An external initialized tokenizer to use instead of the created from the GGUF file. Defaults to None.
             ctx_len: Maximum context length to be used. Use 0 for maximum possible size, which may raise an out of memory error. None will use a default from the 'llamacpp' provider's '_default' entry at 'res/base_models.json'.
             max_tokens_limit: Maximum output tokens limit. None for no limit.
+            tokenizer: An external initialized tokenizer to use instead of the created from the GGUF file. Defaults to None.
             n_gpu_layers: Number of model layers to run in a GPU. Defaults to -1 for all.
             main_gpu: Index of the GPU to use. Defaults to 0.
             n_batch: Prompt processing batch size. Defaults to 512.
             seed: Random number generation seed, for non zero temperature inference. Defaults to 4294967295.
             verbose: Emit (very) verbose llama.cpp output. Defaults to False.
 
         Raises:
@@ -119,14 +122,18 @@
         self._llama = None # type: ignore[assignment]
         self.tokenizer = None # type: ignore[assignment]
         self._own_tokenizer = False
 
         if not has_llama_cpp:
             raise ImportError("Please install llama-cpp-python by running: pip install llama-cpp-python")
 
+        # also accept "provider:path" for ease of use
+        provider_name = self.PROVIDER_NAME + ":"
+        if path.startswith(provider_name):
+            path = path[len(provider_name):]
 
         if not os.path.isfile(path):
             raise NameError(f"Model file not found at '{path}'")
 
 
         # find ctx_len from metadata --and-- check file format
         max_ctx_len = 0
@@ -173,16 +180,16 @@
                                verbose=verbose
                                )
         
         logger.debug(f"Creating inner Llama with path='{path}', llamacpp_kwargs={llamacpp_kwargs}")
 
 
         try:
-            # with llamacpp_verbosity_manager(verbose):
-            self._llama = Llama(model_path=path, **llamacpp_kwargs)
+            with llamacpp_verbosity_manager(verbose):
+                self._llama = Llama(model_path=path, **llamacpp_kwargs)
 
         except Exception as e:
             raise MemoryError(f"Could not load model file '{path}'. "
                               "This is usually an out of memory situation but could also be due to a corrupt file. "
                               f"Internal error: {e}")
 
 
@@ -242,14 +249,17 @@
         Raises:
             RuntimeError: If unable to generate.
             
         Returns:
             Tuple of strings: generated_text, finish_reason.
         """
 
+        if self.tokenizer is None:
+            raise ValueError("A LlamaCppModel object requires a tokenizer")
+
         token_ids = self.tokenizer.encode(text)
         token_len = len(token_ids)
 
 
         # resolve max_tokens size
         resolved_max_tokens = self.resolve_genconf_max_tokens(token_len, genconf)
 
@@ -269,22 +279,28 @@
                 logger.debug(f"JSON schema GBNF grammar:\n█{jsg}█")
                 
                 grammar = llama_grammar.LlamaGrammar.from_string(jsg, 
                                                                  logger.getEffectiveLevel() == logging.DEBUG)
 
             genconf_kwargs["grammar"] = grammar
             
+        # clean keys unknown to llama.cpp
+        genconf_kwargs.pop("json_schema")
+
+        # inject model-specific args, if any
+        genconf_kwargs.update(genconf.resolve_special(self.PROVIDER_NAME))
+        genconf_kwargs.pop("special")
+
+
         # seed config is disabled, has remote models and some hardware accelerated local models don't support it.
         # if "seed" in genconf_kwargs:
         #    if genconf_kwargs["seed"] == -1:
         #        genconf_kwargs["seed"] = int(time())
 
 
-        genconf_kwargs.pop("json_schema")
-
         logger.debug(f"LlamaCpp args: {genconf_kwargs}")
 
 
         try:
             # Llamacpp.create_completion() never returns special tokens because it uses its own detokenize()
             response = self._llama.create_completion(token_ids,
                                                      echo=False,
@@ -296,14 +312,40 @@
 
         logger.debug(f"LlamaCpp response: {response}")
 
         choice = response["choices"][0] # type: ignore[index]
         return choice["text"], choice["finish_reason"] # type: ignore[return-value]
 
 
+
+    async def _gen_text_async(self,
+                              text: str,
+                              genconf: GenConf) -> tuple[str,str]:
+        """Generate from formatted text. Please note that the llama.cpp engine 
+        cannot currently benefit from async: calls will be generated sequentially.
+
+        Args:
+            text: Formatted text (from input Thread).
+            genconf: Model generation configuration.
+
+        Raises:
+            RuntimeError: If unable to generate.
+
+        Returns:
+            Tuple of strings: generated_text, finish_reason.
+        """
+
+        return self._gen_text(text, genconf)
+
+
+
+
+
+
+
         
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
         Ex. llama-cpp-python 0.2.44
         """
         try:        
@@ -314,16 +356,15 @@
             
         return f"llama-cpp-python {ver}"
 
     
     @property
     def desc(self) -> str:
         """Model description."""
-        return f"LlamaCppModel: {self._model_path} - '{self._llama._model.desc()}'"
-
+        return f"{type(self).__name__}: {self._model_path} - '{self._llama._model.desc()}'"
     
     @property
     def n_embd(self) -> int:
         """Embedding size of model."""
         return self._llama.n_embd()
 
     @property
```

### Comparing `sibila-0.3.6/sibila/model.py` & `sibila-0.4.0/sibila/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -137,18 +137,14 @@
         Returns:
             Token length for given text.
         """
 
         tokens = self.encode(text)
         return len(tokens)        
 
-    @property
-    def token_len_lambda(self) -> Callable[[str], int]:
-        return lambda text: self.token_len(text)
-
 
     def __str__(self):
         return f"""\
 bos={self.bos_token_id}='{self.bos_token}'
 eos={self.eos_token_id}='{self.eos_token}'
 pad={self.pad_token_id}='{self.pad_token}'
 unk={self.unk_token_id}='{self.unk_token}'"""
@@ -157,28 +153,28 @@
 
 
 
 
 
 
 class Model(ABC):
-    """Model is a base class for an LLM model with common functionality.
+    """Model is an abstract base class for common LLM model functionality. Many of the useful methods like extract() or json() are implemented here.
 
-    LlamaCppModel, OpenAIModel, etc, derive from this class.
+    It should not be instantiated directly, instead LlamaCppModel, OpenAIModel, etc, all derive from this class.
     """
 
     
     is_local_model: bool
     """Is the model running locally?"""
     
     is_message_model: bool
     """Is communication with the model message-based or text-based/token-based?"""
 
-    tokenizer: Tokenizer
-    """Tokenizer used to encode text (even for message-based models)."""
+    tokenizer: Union[Tokenizer,None]
+    """Tokenizer used to encode text (even for message-based models). Some remote models don't have tokenizer and token length is estimated"""
 
     genconf: GenConf
     """Generation configuration: options used during gen()."""
 
     json_format_instructors: dict
     """If GenConf.json / GenConf.json_schema is used, these strings are appended to first thread msg of either instructions or IN kind. See initialization below."""
 
@@ -187,14 +183,20 @@
 
     ctx_len: int
     """Maximum context token length that can be passed to model as input. There can be a limit for output tokens in the max_tokens_limit."""
 
     max_tokens_limit: int
     """Some models limit the size of emitted output tokens, which is stored in this property."""
 
+    output_key_name: str
+    """Name used when an output key needs to be created for JSON output."""
+
+    PROVIDER_NAME: str = NotImplemented
+    """Provider prefix that this class handles."""
+
     
     def __init__(self,
                  is_local_model: bool,
                  genconf: Union[GenConf, None],
                  schemaconf: Union[JSchemaConf, None],
                  tokenizer: Union[Tokenizer, None]):
         """Initializer for base model type, shared by actual model classes like LlamaCpp, OpenAI, etc.
@@ -206,14 +208,15 @@
             tokenizer: Tokenizer used to encode text (even for message-based models).
         """
         
         self.is_local_model = is_local_model
         
         self.ctx_len = 0
         self.max_tokens_limit = sys.maxsize
+        self.output_key_name = "output"
 
         self.tokenizer = tokenizer # type: ignore[assignment]
 
         if genconf is None:
             self.genconf = GenConf()
         else:
             self.genconf = genconf.clone()
@@ -268,75 +271,177 @@
         Returns:
             A GenOut object with result, generated text, etc.
             The output text is in GenOut.text.
         """
         raise NotImplementedError
 
 
+    async def gen_async(self,
+                        thread: Thread,
+                        genconf: Optional[GenConf] = None,
+                        ) -> GenOut:
+        """Async text generation from a Thread, used by the other model generation methods.
+        Doesn't raise an exception if an error occurs, always returns GenOut.
+
+        Args:
+            thread: The Thread to use as model input.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+
+        Raises:
+            RuntimeError: If unable to generate.
+            NotImplementedError: If method was not defined by a derived class.
+
+        Returns:
+            A GenOut object with result, generated text, etc.
+            The output text is in GenOut.text.
+        """
+        raise NotImplementedError
     
 
 
     
     
+    def _gen_json_pre(self,
+                      thread: Thread,
+                      json_schema: Union[dict,str,None],
+                      genconf: Union[GenConf,None],
+
+                      massage_schema: bool,
+                      schemaconf: Union[JSchemaConf, None]
+                      ) -> list:
+
+        if genconf is None:
+            genconf = self.genconf
+
+        if genconf.json_schema is not None and json_schema is not None:
+            logger.warning("Both arg json_schema and genconf.json_schema are set: using json_schema arg")
+
+        if json_schema is not None:
+            if schemaconf is None:
+                schemaconf = self.schemaconf
+
+            logger.debug("JSON schema conf:\n" + pformat(schemaconf))
+
+            if massage_schema:
+                if not isinstance(json_schema, dict):
+                    json_schema = json.loads(json_schema)
+
+                json_schema = json_schema_massage(json_schema, schemaconf) # type: ignore[arg-type]
+                logger.debug("Massaged JSON schema:\n" + pformat(json_schema))
+
+        return [thread, genconf(format="json", 
+                                json_schema=json_schema)]
+
 
     def gen_json(self,
-                 json_schema: Union[dict,str,None],
-                
                  thread: Thread,
+                 json_schema: Union[dict,str,None],
                  genconf: Optional[GenConf] = None,
 
                  massage_schema: bool = True,
                  schemaconf: Optional[JSchemaConf] = None,
                  ) -> GenOut:
         """JSON/JSON-schema constrained generation, returning a Python dict of values, conditioned or not by a JSON schema.
         Doesn't raise an exception if an error occurs, always returns GenOut.
 
         Args:
-            json_schema: A JSON schema describing the dict fields that will be output. None means no schema (free JSON output).
             thread: The Thread to use as model input.
+            json_schema: A JSON schema describing the dict fields that will be output. None means no schema (free JSON output).
             genconf: Model generation configuration. Defaults to None, which uses model's default.
             massage_schema: Simplify schema. Defaults to True.
             schemaconf: JSchemaConf object that controls schema simplification. Defaults to Defaults to None, which uses model's default.
 
         Raises:
             RuntimeError: If unable to generate.
 
         Returns:
             A GenOut object with result, generated text, etc. The output dict is in GenOut.dic.
         """
 
-        if genconf is None:
-            genconf = self.genconf
+        args = self._gen_json_pre(thread,
+                                  json_schema,
+                                  genconf,
+                                  massage_schema,
+                                  schemaconf)
+        return self.gen(*args)
+    
+
+    async def gen_json_async(self,
+                             thread: Thread,
+                             json_schema: Union[dict,str,None],
+                             genconf: Optional[GenConf] = None,
+
+                             massage_schema: bool = True,
+                             schemaconf: Optional[JSchemaConf] = None,
+                             ) -> GenOut:
+        """JSON/JSON-schema constrained generation, returning a Python dict of values, conditioned or not by a JSON schema.
+        Doesn't raise an exception if an error occurs, always returns GenOut.
 
-        if genconf.json_schema is not None and json_schema is not None:
-            logger.warning("Both arg json_schema and genconf.json_schema are set: using json_schema arg")
+        Args:
+            thread: The Thread to use as model input.
+            json_schema: A JSON schema describing the dict fields that will be output. None means no schema (free JSON output).
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            massage_schema: Simplify schema. Defaults to True.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to Defaults to None, which uses model's default.
 
-        if json_schema is not None:
-            if schemaconf is None:
-                schemaconf = self.schemaconf
+        Raises:
+            RuntimeError: If unable to generate.
 
-            logger.debug("JSON schema conf:\n" + pformat(schemaconf))
+        Returns:
+            A GenOut object with result, generated text, etc. The output dict is in GenOut.dic.
+        """
+
+        args = self._gen_json_pre(thread,
+                                  json_schema,
+                                  genconf,
+                                  massage_schema,
+                                  schemaconf)
+        return await self.gen_async(*args)
 
-            if massage_schema:
-                if not isinstance(json_schema, dict):
-                    json_schema = json.loads(json_schema)
 
-                json_schema = json_schema_massage(json_schema, schemaconf) # type: ignore[arg-type]
-                logger.debug("Massaged JSON schema:\n" + pformat(json_schema))
 
-        out = self.gen(thread, 
-                       genconf(format="json", 
-                               json_schema=json_schema))
-        
-        return out        
-        
 
 
     
+    def _gen_dataclass_pre(self,
+                           cls: Any # a dataclass
+                           ) -> dict:
+        
+        if is_dataclass(cls):
+            schema = build_dataclass_object_json_schema(cls)
+        else:
+            raise TypeError("Only dataclass allowed for cls argument")        
+        return schema
+
+    def _gen_dataclass_post(self,
+                            out: GenOut,
+                            cls: Any,
+                            schemaconf: Union[JSchemaConf,None]
+                            ) -> GenOut:
     
+        if out.dic is not None:
+            try:
+                obj = create_final_instance(cls, 
+                                            is_list=False,
+                                            val=out.dic,
+                                            schemaconf=schemaconf)
+                out.value = obj
+                
+            except TypeError as e:
+                out.res = GenRes.ERROR_JSON_SCHEMA_VAL # error initializing object from JSON
+                out.text += f"\nJSON Schema error: {e}"
+        else:
+            # out.res already holds the right error
+            ...
+        
+        return out
+
+
+
+
     def gen_dataclass(self,
                       cls: Any, # a dataclass
                       thread: Thread,
                       genconf: Optional[GenConf] = None,
                       schemaconf: Optional[JSchemaConf] = None
                       ) -> GenOut:
         """Constrained generation after a dataclass definition.
@@ -352,44 +457,106 @@
         Raises:
             RuntimeError: If unable to generate.
 
         Returns:
             A GenOut object with result, generated text, etc. The initialized dataclass object is in GenOut.value.
         """
 
-        if is_dataclass(cls):
-            schema = build_dataclass_object_json_schema(cls)
-        else:
-            raise TypeError("Only dataclass allowed for argument cls")
+        schema = self._gen_dataclass_pre(cls)
 
-        out = self.gen_json(schema,
-                            thread,
+        out = self.gen_json(thread,
+                            schema,
                             genconf,
                             massage_schema=True,
                             schemaconf=schemaconf)
     
+        return self._gen_dataclass_post(out,
+                                        cls,
+                                        schemaconf)
+
+
+
+    async def gen_dataclass_async(self,
+                                  cls: Any, # a dataclass
+                                  thread: Thread,
+                                  genconf: Optional[GenConf] = None,
+                                  schemaconf: Optional[JSchemaConf] = None
+                                  ) -> GenOut:
+        """Async constrained generation after a dataclass definition.
+        An initialized dataclass object is returned in the "value" field of the returned dict.
+        Doesn't raise an exception if an error occurs, always returns GenOut containing the created object.
+
+        Args:
+            cls: A dataclass definition.
+            thread: The Thread object to use as model input.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A GenOut object with result, generated text, etc. The initialized dataclass object is in GenOut.value.
+        """
+
+        schema = self._gen_dataclass_pre(cls)
+
+        out = await self.gen_json_async(thread,
+                                        schema,
+                                        genconf,
+                                        massage_schema=True,
+                                        schemaconf=schemaconf)
+    
+        return self._gen_dataclass_post(out,
+                                        cls,
+                                        schemaconf)
+
+
+
+
+
+
+
+    def _gen_pydantic_pre(self,
+                          cls: Any # a Pydantic BaseModel class
+                          ) -> dict:
+
+        if is_subclass_of(cls, BaseModel):
+            schema = json_schema_from_pydantic(cls)
+        else:
+            raise TypeError("Only pydantic BaseModel allowed for cls argument")
+        
+        return schema
+
+
+    def _gen_pydantic_post(self,
+                           out: GenOut,
+                           cls: Any, # a Pydantic BaseModel class
+                           schemaconf: Union[JSchemaConf,None]
+                           ) -> GenOut:
+    
         if out.dic is not None:
             try:
-                obj = create_final_instance(cls, 
-                                            is_list=False,
-                                            val=out.dic,
-                                            schemaconf=schemaconf)
+                obj = pydantic_obj_from_json(cls, 
+                                             out.dic,
+                                             schemaconf=schemaconf)
                 out.value = obj
                 
             except TypeError as e:
-                out.res = GenRes.ERROR_JSON_SCHEMA_VAL # error initializing object from JSON
+                out.res = GenRes.ERROR_JSON_SCHEMA_VAL # error validating for object (by Pydantic), but JSON is valid for its schema
                 out.text += f"\nJSON Schema error: {e}"
         else:
             # out.res already holds the right error
             ...
         
         return out
 
 
 
+
     def gen_pydantic(self,
                      cls: Any, # a Pydantic BaseModel class
                      thread: Thread,
                      genconf: Optional[GenConf] = None,
                      schemaconf: Optional[JSchemaConf] = None
                      ) -> GenOut:
         """Constrained generation after a Pydantic BaseModel-derived class definition.
@@ -406,42 +573,130 @@
             RuntimeError: If unable to generate.
             TypeError: When cls is not a Pydantic BaseClass.
 
         Returns:
             A GenOut object with result, generated text, etc. The initialized Pydantic BaseModel-derived object is in GenOut.value.
         """
 
-        if is_subclass_of(cls, BaseModel):
-            schema = json_schema_from_pydantic(cls)
-        else:
-            raise TypeError("Only pydantic BaseModel allowed for argument cls")
+        schema = self._gen_pydantic_pre(cls)
 
-        out = self.gen_json(schema,
-                            thread,
+        out = self.gen_json(thread,
+                            schema,
                             genconf,
                             massage_schema=True,
                             schemaconf=schemaconf)
     
+        return self._gen_pydantic_post(out,
+                                       cls,
+                                       schemaconf)
+
+
+
+    async def gen_pydantic_async(self,
+                                 cls: Any, # a Pydantic BaseModel class
+                                 thread: Thread,
+                                 genconf: Optional[GenConf] = None,
+                                 schemaconf: Optional[JSchemaConf] = None
+                                 ) -> GenOut:
+        """Async constrained generation after a Pydantic BaseModel-derived class definition.
+        An initialized Pydantic BaseModel object is returned in the "value" field of the returned dict.
+        Doesn't raise an exception if an error occurs, always returns GenOut containing the created object.
+
+        Args:
+            cls: A class derived from a Pydantic BaseModel class.
+            thread: The Thread to use as model input.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            RuntimeError: If unable to generate.
+            TypeError: When cls is not a Pydantic BaseClass.
+
+        Returns:
+            A GenOut object with result, generated text, etc. The initialized Pydantic BaseModel-derived object is in GenOut.value.
+        """
+
+        schema = self._gen_pydantic_pre(cls)
+
+        out = await self.gen_json_async(thread,
+                                        schema,
+                                        genconf,
+                                        massage_schema=True,
+                                        schemaconf=schemaconf)
+
+        return self._gen_pydantic_post(out,
+                                       cls,
+                                       schemaconf)
+
+
+
+
+
+
+    def _gen_extract_pre(self,
+                         target: Any,
+                         thread: Thread,
+                         genconf: Union[GenConf, None],
+                         schemaconf: Union[JSchemaConf, None]
+                         ) -> Any:
+
+        schema, created_output_key = build_root_json_schema(target, 
+                                                            self.output_key_name)
+        
+        final_type, is_list = get_final_type(target)
+
+        if schemaconf is None:
+            schemaconf = JSchemaConf()
+
+        return (thread,
+                schema,
+                genconf,                
+                created_output_key,
+                final_type, 
+                is_list,
+                schemaconf)
+
+
+    def _gen_extract_post(self,
+                          out: GenOut,
+                          created_output_key: bool,
+                          final_type: Any, 
+                          is_list: bool,
+                          schemaconf: JSchemaConf
+                          ) -> GenOut:
+
         if out.dic is not None:
+
+            if created_output_key:
+                if self.output_key_name in out.dic:
+                    val = out.dic[self.output_key_name]
+                else:
+                    out.res = GenRes.ERROR_JSON_SCHEMA_VAL # JSON error
+                    out.text += f"\nExpecting key '{self.output_key_name}'."
+                    return out
+
+            else:
+                val = out.dic
+
             try:
-                obj = pydantic_obj_from_json(cls, 
-                                             out.dic,
-                                             schemaconf=schemaconf)
-                out.value = obj
-                
+                value = create_final_instance(final_type, 
+                                              is_list, 
+                                              val,
+                                              schemaconf=schemaconf)
+                out.value = value
+
             except TypeError as e:
-                out.res = GenRes.ERROR_JSON_SCHEMA_VAL # error validating for object (by Pydantic), but JSON is valid for its schema
+                out.res = GenRes.ERROR_JSON_SCHEMA_VAL # error validating, but JSON is valid for its schema
                 out.text += f"\nJSON Schema error: {e}"
+
         else:
             # out.res already holds the right error
             ...
-        
-        return out
-
 
+        return out
 
 
 
     def gen_extract(self,
                     target: Any,
                     thread: Thread,
                     genconf: Optional[GenConf] = None,
@@ -491,52 +746,117 @@
         Raises:
             RuntimeError: If unable to generate.
 
         Returns:
             A GenOut object with model's results and instantiated type in the "value" field.
         """
 
-        OUTPUT_KEY_NAME = "output"
-
-        schema, created_output_key = build_root_json_schema(target, OUTPUT_KEY_NAME)
-        
-        final_type, is_list = get_final_type(target)
-
-        if schemaconf is None:
-            schemaconf = JSchemaConf()
+        (thread,
+         schema,
+         genconf, 
+         created_output_key, 
+         final_type, 
+         is_list, 
+         schemaconf) = self._gen_extract_pre(target,
+                                             thread,
+                                             genconf,
+                                             schemaconf)
 
-        out = self.gen_json(schema,
-                            thread,
+        out = self.gen_json(thread,
+                            schema,
                             genconf,
                             massage_schema=True,
                             schemaconf=schemaconf)
     
-        if out.dic is not None:
+        return self._gen_extract_post(out,
+                                      created_output_key,
+                                      final_type,
+                                      is_list,
+                                      schemaconf) # type: ignore [arg-type]
 
-            if created_output_key:
-                val = out.dic[OUTPUT_KEY_NAME]
-            else:
-                val = out.dic
 
-            try:
-                value = create_final_instance(final_type, 
-                                              is_list, 
-                                              val,
-                                              schemaconf=schemaconf)
-                out.value = value
 
-            except TypeError as e:
-                out.res = GenRes.ERROR_JSON_SCHEMA_VAL # error validating, but JSON is valid for its schema
-                out.text += f"\nJSON Schema error: {e}"
 
-        else:
-            # out.res already holds the right error
-            ...
+    async def gen_extract_async(self,
+                                target: Any,
+                                thread: Thread,
+                                genconf: Optional[GenConf] = None,
+                                schemaconf: Optional[JSchemaConf] = None
+                                ) -> GenOut:
+        """Async free type constrained generation: an instance of the given type is initialized with the model's output.
+        The initialized value is placed in the "value" field of the returned dict.
+        Doesn't raise an exception if an error occurs, always returns GenOut.
+
+        The following target types are accepted:
+
+            - prim_type:
+                bool
+                int
+                float
+                str
+                
+            - enums:
+                [1, 2, 3] or ["a","b"] - all items of the same prim_type
+                Literal['year', 'name'] - all items of the same prim_type
+                Enum, EnumInt, EnumStr, (Enum, int),... - all items of the same prim_type
+
+            - datetime/date/time
+
+            - a list in the form:
+                list[type] - for example list[int]. 
+                The list can be annotated:
+                    Annotated[list[T], "List desc"]
+                And/or the list item type can be annotated:
+                    list[Annotated[T, "Item desc"]]
+
+            - dataclass with fields of the above supported types (or dataclass).
+
+            - Pydantic BaseModel
+
+        All types can be Annotated[T, "Desc"], for example: 
+            count: int
+        Can be annotated as:
+            count: Annotated[int, "How many units?"]
+
+        Args:
+            target: One of the above types.
+            thread: The Thread to use as model input.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A GenOut object with model's results and instantiated type in the "value" field.
+        """
+        (thread,
+         schema,
+         genconf, 
+         created_output_key, 
+         final_type, 
+         is_list, 
+         schemaconf) = self._gen_extract_pre(target,
+                                             thread,
+                                             genconf,
+                                             schemaconf)
+
+        out = await self.gen_json_async(thread,
+                                        schema,
+                                        genconf,
+                                        massage_schema=True,
+                                        schemaconf=schemaconf)
+    
+        return self._gen_extract_post(out,
+                                      created_output_key,
+                                      final_type,
+                                      is_list,
+                                      schemaconf) # type: ignore [arg-type]
+
 
-        return out
 
 
 
 
 
     # ======================================================== user generation points    
 
@@ -545,14 +865,44 @@
                  query: Union[str,Thread],
                  *,
                  inst: Optional[str] = None,
 
                  genconf: Optional[GenConf] = None,
                  ok_length_is_error: bool = False
                  ) -> str:
+        """Text generation from a Thread or plain text, used by the other model generation methods. Same as call().
+
+        Args:
+            query: Thread or an str with the text of a single IN message to use as model input.
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            ok_length_is_error: Should a result of GenRes.OK_LENGTH be considered an error and raise?
+
+        Raises:
+            GenError: If an error occurred. This can be a model error, or an invalid JSON output error.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            Text generated by model.
+        """
+
+        return self.call(query,
+                         inst=inst,
+                         genconf=genconf,
+                         ok_length_is_error=ok_length_is_error)
+
+
+    def call(self,             
+             query: Union[str,Thread],
+             *,
+             inst: Optional[str] = None,
+
+             genconf: Optional[GenConf] = None,
+             ok_length_is_error: bool = False
+             ) -> str:
         """Text generation from a Thread or plain text, used by the other model generation methods.
 
         Args:
             query: Thread or an str with the text of a single IN message to use as model input.
             inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
             genconf: Model generation configuration. Defaults to None, which uses model's default.
             ok_length_is_error: Should a result of GenRes.OK_LENGTH be considered an error and raise?
@@ -572,33 +922,72 @@
         
         GenError.raise_if_error(out,
                                 ok_length_is_error=ok_length_is_error)
 
         return out.text
 
 
+    async def call_async(self,
+                         query: Union[str,Thread],
+                         *,
+                         inst: Optional[str] = None,
+ 
+                         genconf: Optional[GenConf] = None,
+                         ok_length_is_error: bool = False
+                         ) -> str:
+        """Text generation from a Thread or plain text, used by the other model generation methods.
+
+        Args:
+            query: Thread or an str with the text of a single IN message to use as model input.
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            ok_length_is_error: Should a result of GenRes.OK_LENGTH be considered an error and raise?
+
+        Raises:
+            GenError: If an error occurred. This can be a model error, or an invalid JSON output error.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            Text generated by model.
+        """
+        
+        thread = Thread.ensure(query, inst)
+
+        out = await self.gen_async(thread=thread, 
+                                   genconf=genconf)
+        
+        GenError.raise_if_error(out,
+                                ok_length_is_error=ok_length_is_error)
+
+        return out.text
+
+
+
+
 
 
-    def json(self,             
-             json_schema: Union[dict,str,None],
-             
+
+
+
+    def json(self,
              query: Union[str,Thread],
              *,
+             json_schema: Union[dict,str,None] = None,
              inst: Optional[str] = None,
 
              genconf: Optional[GenConf] = None,
              massage_schema: bool = True,
              schemaconf: Optional[JSchemaConf] = None,
              ) -> dict:
         """JSON/JSON-schema constrained generation, returning a Python dict of values, constrained or not by a JSON schema.
         Raises GenError if unable to get a valid/schema-validated JSON.
 
         Args:
-            json_schema: A JSON schema describing the dict fields that will be output. None means no schema (free JSON output).
             query: Thread or an str with the text of a single IN message to use as model input.
+            json_schema: A JSON schema describing the dict fields that will be output. None means no schema (free JSON output).
             inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
             genconf: Model generation configuration. Defaults to None, which uses model's default.
             massage_schema: Simplify schema. Defaults to True.
             schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
 
         Raises:
             GenError: If an error occurred, for example an invalid JSON schema output error. See GenError.
@@ -606,29 +995,83 @@
 
         Returns:
             A dict from model's JSON response, following genconf.jsonschema, if provided.
         """        
 
         thread = Thread.ensure(query, inst)
 
-        out = self.gen_json(json_schema,                            
-                            thread,
+        out = self.gen_json(thread,
+                            json_schema,                            
                             genconf,
                             massage_schema,
                             schemaconf)
         
         GenError.raise_if_error(out,
                                 ok_length_is_error=False) # as valid JSON can still be produced
 
         return out.dic # type: ignore[return-value]
 
 
 
 
-    def dataclass(self, # noqa: E811
+
+
+    async def json_async(self,             
+                         query: Union[str,Thread],
+                         *,
+                         json_schema: Union[dict,str,None] = None,
+                         inst: Optional[str] = None,
+
+                         genconf: Optional[GenConf] = None,
+                         massage_schema: bool = True,
+                         schemaconf: Optional[JSchemaConf] = None,
+                         ) -> dict:
+        """JSON/JSON-schema constrained generation, returning a Python dict of values, constrained or not by a JSON schema.
+        Raises GenError if unable to get a valid/schema-validated JSON.
+
+        Args:
+            query: Thread or an str with the text of a single IN message to use as model input.
+            json_schema: A JSON schema describing the dict fields that will be output. None means no schema (free JSON output).
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            massage_schema: Simplify schema. Defaults to True.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            GenError: If an error occurred, for example an invalid JSON schema output error. See GenError.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A dict from model's JSON response, following genconf.jsonschema, if provided.
+        """        
+
+        thread = Thread.ensure(query, inst)
+
+        out = await self.gen_json_async(thread,
+                                        json_schema,
+                                        genconf,
+                                        massage_schema,
+                                        schemaconf)
+        
+        GenError.raise_if_error(out,
+                                ok_length_is_error=False) # as valid JSON can still be produced
+
+        return out.dic # type: ignore[return-value]
+
+
+
+
+
+
+
+
+
+
+
+    def dataclass(self, # noqa: F811
                   cls: Any, # a dataclass definition
 
                   query: Union[str,Thread],
                   *,
                   inst: Optional[str] = None,
 
                   genconf: Optional[GenConf] = None,
@@ -662,14 +1105,59 @@
         GenError.raise_if_error(out,
                                 ok_length_is_error=False) # as valid JSON can still be produced
 
         return out.value
 
 
 
+    async def dataclass_async(self, # noqa: E811
+                              cls: Any, # a dataclass definition
+
+                              query: Union[str,Thread],
+                              *,
+                              inst: Optional[str] = None,
+
+                              genconf: Optional[GenConf] = None,
+                              schemaconf: Optional[JSchemaConf] = None
+                              ) -> Any: # a dataclass object
+        """Async constrained generation after a dataclass definition, resulting in an object initialized with the model's response.
+        Raises GenError if unable to get a valid response that follows the dataclass definition.
+
+        Args:
+            cls: A dataclass definition.
+            query: Thread or an str with the text of a single IN message to use as model input.
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            GenError: If an error occurred, for example invalid object initialization. See GenError.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            An object of class cls (derived from dataclass) initialized from the constrained JSON output.
+        """
+
+        thread = Thread.ensure(query, inst)
+
+        out = await self.gen_dataclass_async(cls,
+                                             thread,
+                                             genconf,
+                                             schemaconf)
+
+        GenError.raise_if_error(out,
+                                ok_length_is_error=False) # as valid JSON can still be produced
+
+        return out.value
+
+
+
+
+
+
 
 
 
     def pydantic(self,
                  cls: Any, # a Pydantic BaseModel class
 
                  query: Union[str,Thread],
@@ -707,31 +1195,72 @@
 
         GenError.raise_if_error(out,
                                 ok_length_is_error=False) # as valid JSON can still be produced
 
         return out.value
 
 
+    async def pydantic_async(self,
+                             cls: Any, # a Pydantic BaseModel class
+
+                             query: Union[str,Thread],
+                             *,
+                             inst: Optional[str] = None,
+
+                             genconf: Optional[GenConf] = None,
+                             schemaconf: Optional[JSchemaConf] = None
+                             ) -> Any: # a Pydantic BaseModel object
+        """Async constrained generation after a Pydantic BaseModel-derived class definition.
+        Results in an object initialized with the model response.
+        Raises GenError if unable to get a valid dict that follows the BaseModel class definition.
+
+        Args:
+            cls: A class derived from a Pydantic BaseModel class.
+            query: Thread or an str with the text of a single IN message to use as model input.
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            GenError: If an error occurred, for example an invalid BaseModel object. See GenError.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A Pydantic object of class cls (derived from BaseModel) initialized from the constrained JSON output.
+        """
+
+        thread = Thread.ensure(query, inst)
+
+        out = await self.gen_pydantic_async(cls,
+                                            thread,
+                                            genconf,
+                                            schemaconf)
+
+        GenError.raise_if_error(out,
+                                ok_length_is_error=False) # as valid JSON can still be produced
+
+        return out.value
+
+
 
 
 
 
 
     def extract(self,
                 target: Any,
 
                 query: Union[str,Thread],
                 *,
                 inst: Optional[str] = None,
 
                 genconf: Optional[GenConf] = None,
                 schemaconf: Optional[JSchemaConf] = None
-                ) -> Any:
-        
-        """Free type constrained generation: an instance of the given type will be initialized with the model's output.
+                ) -> Any:        
+        """Type-constrained generation: an instance of the given type will be initialized with the model's output.
         The following target types are accepted:
 
         - prim_type:
 
             - bool
             - int
             - float
@@ -788,14 +1317,95 @@
                                 ok_length_is_error=False) # as valid JSON can still be produced
 
         return out.value
 
 
 
 
+
+    async def extract_async(self,
+                            target: Any,
+
+                            query: Union[str,Thread],
+                            *,
+                            inst: Optional[str] = None,
+
+                            genconf: Optional[GenConf] = None,
+                            schemaconf: Optional[JSchemaConf] = None
+                            ) -> Any:        
+        """Async type-constrained generation: an instance of the given type will be initialized with the model's output.
+        The following target types are accepted:
+
+        - prim_type:
+
+            - bool
+            - int
+            - float
+            - str
+            
+        - enums:
+
+            - [1, 2, 3] or ["a","b"] - all items of the same prim_type
+            - Literal['year', 'name'] - all items of the same prim_type
+            - Enum, EnumInt, EnumStr, (Enum, int),... - all items of the same prim_type
+
+        - datetime/date/time
+
+        - a list in the form:
+            - list[type]
+            
+            For example list[int]. The list can be annotated:
+                Annotated[list[T], "List desc"]
+            And/or the list item type can be annotated:
+                list[Annotated[T, "Item desc"]]
+
+        - dataclass with fields of the above supported types (or dataclass).
+
+        - Pydantic BaseModel
+
+        All types can be Annotated[T, "Desc"], for example: 
+            count: int
+        Can be annotated as:
+            count: Annotated[int, "How many units?"]
+
+        Args:
+            target: One of the above types.
+            query: Thread or an str with the text of a single IN message to use as model input.
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            GenError: If an error occurred, for example invalid object initialization. See GenError.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A value of target arg type instantiated with the model's output.
+        """
+
+        thread = Thread.ensure(query, inst)
+
+        out = await self.gen_extract_async(target,
+                                           thread,
+                                           genconf,
+                                           schemaconf)
+
+        GenError.raise_if_error(out,
+                                ok_length_is_error=False) # as valid JSON can still be produced
+
+        return out.value
+
+
+
+
+
+
+
+
+
     def classify(self,
                  labels: Any,
 
                  query: Union[str,Thread],
                  *,
                  inst: Optional[str] = None,
 
@@ -833,14 +1443,57 @@
                             query,
                             inst=inst,
                             genconf=genconf,
                             schemaconf=schemaconf)
 
 
 
+    async def classify_async(self,
+                             labels: Any,
+
+                             query: Union[str,Thread],
+                             *,
+                             inst: Optional[str] = None,
+
+                             genconf: Optional[GenConf] = None,
+                             schemaconf: Optional[JSchemaConf] = None
+                             ) -> Any:
+        """Returns a classification from one of the given enumeration values
+        The following ways to specify the valid labels are accepted:
+
+        - [1, 2, 3] or ["a","b"] - all items of the same prim_type
+        - Literal['year', 'name'] - all items of the same prim_type
+        - Enum, EnumInt, EnumStr, (Enum, int),... - all items of the same prim_type
+
+        Args:
+            labels: One of the above types.
+            query: Thread or an str with the text of a single IN message to use as model input.
+            inst: Instruction message for model. Will override Thread's inst, if set. Defaults to None.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+            schemaconf: JSchemaConf object that controls schema simplification. Defaults to None, which uses model's default.
+
+        Raises:
+            GenError: If an error occurred. See GenError.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            One of the given labels, as classified by the model.
+        """
+
+        # verify it's a valid enum "type"
+        type_,_ = get_enum_type(labels)
+        if type_ is None:
+            raise TypeError("Arg labels must be one of Literal, Enum class or a list of str, float or int items")
+        
+        return await self.extract_async(labels,
+                                        query,
+                                        inst=inst,
+                                        genconf=genconf,
+                                        schemaconf=schemaconf)
+
 
 
 
 
 
 
 
@@ -848,25 +1501,32 @@
     
     # ======================================================== properties
 
      
 
     @abstractmethod
     def token_len(self,
-                  thread: Thread) -> int:
-        """Calculate token length for a Thread.
+                  thread_or_text: Union[Thread,str]) -> int:
+        """Calculate or estimate the token length for a Thread or plain text string.
+        In some cases it's not possible to calculate the exact token count, 
+        but at least a conservative estimate should be provided.
 
         Args:
-            thread: For token length calculation.
+            thread_or_text: A Thread or plain text string For token length calculation.
 
         Returns:
-            Number of tokens the thread will use.
+            Number of tokens occupied.
         """
         ...
 
+    @property
+    def token_len_lambda(self) -> Callable[[Union[Thread,str]], int]:
+        return lambda text: self.token_len(text)
+
+
 
 
     def calc_max_max_tokens(self,
                             input_token_len: int) -> int:
         """Calculate maximum length of tokens that the model can output (as in GenConf.max_tokens).
         May be smaller than remaining length due to max_tokens_limit attribute.
 
@@ -882,35 +1542,38 @@
 
 
 
     def resolve_genconf_max_tokens(self,
                                    input_token_len: int,
                                    genconf: GenConf) -> int:
         """Resolve genconf.max_tokens to a definitive value, depending on input, ctx_len and max_tokens_limit"""
-                
-        max_output_tokens = self.calc_max_max_tokens(input_token_len)
-        if max_output_tokens <= 0:
+        
+        avail_output_tokens = self.calc_max_max_tokens(input_token_len)
+        if avail_output_tokens <= 0:
             raise ValueError(f"""Input token length ({input_token_len}) doesn't fit available ctx_len ({self.ctx_len})""")
 
+        # calc maximum possible output
         resolved_max_tokens = genconf.resolve_max_tokens(self.ctx_len, self.max_tokens_limit)
-           
-        if resolved_max_tokens > max_output_tokens:
-            logger.info(f"Output token length from genconf.max_tokens ({resolved_max_tokens}) is larger than possible. Limiting to {max_output_tokens}")
-            resolved_max_tokens = max_output_tokens
 
-        return resolved_max_tokens
+        # ensure avail_output_tokens fits resolved_max_tokens
+        max_tokens = min(resolved_max_tokens, avail_output_tokens)
+        return max_tokens
 
 
 
     @classmethod
-    def known_models(cls) -> Union[list[str], None]:
+    def known_models(cls,
+                     api_key: Optional[str] = None) -> Union[list[str], None]:
         """If the model can only use a fixed set of models, return their names. Otherwise, return None.
 
+        Args:
+            api_key: If the model provider requires an API key, pass it here or set it in the respective env variable.
+
         Returns:
-            Returns a list of known models or None if it can accept any model.
+            Returns a list of known models or None if unable to fetch it.
         """
         return None
 
     @classmethod
     def version(cls) -> str:
         """Sibila version + provider version
         Ex: sibila='0.2.3' provider='llama-cpp-python 0.2.44'        
@@ -946,17 +1609,17 @@
 
 
 
     
     
     # = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = internal
     
-    def _prepare_gen_in(self,
-                        thread: Thread,
-                        genconf: GenConf) -> Thread:
+    def _prepare_gen_thread(self,
+                            thread: Thread,
+                            genconf: GenConf) -> Thread:
         """Perform common pre-generation operations of the thread that will be used.
 
         Args:
             thread: Input thread that may be augmented here. If not modified, the same thread is returned.
             genconf: Generation configuration.
 
         Raises:
@@ -1019,26 +1682,34 @@
             text: Text obtained from model.
             finish: Model finish reason - only "stop", "length" are used, others will map as GenRes.ERROR_MODEL.
 
         Returns:
             A GenOut object with result, generated text, etc. 
         """
 
-        logger.debug(f"Response {finish}: █{text}█")
+        logger.debug(f"Response finish='{finish}': █{text}█")
         
         if text is None:
             text = ''
         else:
             text = text.strip()
 
         if genconf.format == "json":
             if "\\u" in text:
                 # dumps(with default ensure_ascii=False) -> ascii (subset of utf-8) -> text.encode("latin1") -> latin1 ->
                 #   decode("unicode-escape") -> utf-8
                 text = text.encode("latin1").decode("unicode-escape")
+
+            # some troubled remote models may include chit-chat after the JSON
+            begin = text.find("{")
+            if begin > 0:
+                text = text[begin:]
+            end = text.rfind("}")
+            if end > 0:
+                text = text[:end + 1]
                 
             try:
                 dic = json.loads(text)
 
                 if genconf.json_schema is not None:
                     if isinstance(genconf.json_schema, str):
                         schema_dic = json.loads(genconf.json_schema)
@@ -1094,26 +1765,33 @@
                          schemaconf,
                          tokenizer)
         
         self.is_message_model = False
 
     
     def token_len(self,
-                  thread: Thread,
+                  thread_or_text: Union[Thread,str],
                   _: Optional[GenConf] = None) -> int:
         """Calculate token length for a Thread.
 
         Args:
-            thread: For token length calculation.
+            thread_or_text: For token length calculation.
 
         Returns:
-            Number of tokens the thread will use.
+            Number of tokens used.
         """
 
-        text = self.text_from_thread(thread)
+        if self.tokenizer is None:
+            raise ValueError("A TextModel object requires a tokenizer")
+
+        if isinstance(thread_or_text, Thread):
+            text = self.text_from_thread(thread_or_text)
+        else:
+            text = thread_or_text
+
         return self.tokenizer.token_len(text)
 
    
     
     @abstractmethod
     def text_from_thread(self,
                          thread: Thread) -> str:
@@ -1225,15 +1903,38 @@
         # setup jinja template
         jinja_env = ImmutableSandboxedEnvironment(trim_blocks=True, lstrip_blocks=True)
         jinja_env.globals["raise_exception"] = jinja_raise_exception
         self._jinja_compiled_template = jinja_env.from_string(self.format_template)
 
 
 
-    
+
+
+    def _gen_pre(self, 
+                 thread: Thread,
+                 genconf: Optional[GenConf] = None,
+                 ) -> tuple:
+
+        if genconf is None:
+            genconf = self.genconf
+
+        thread = self._prepare_gen_thread(thread, genconf)
+
+        prompt = self.text_from_thread(thread)
+
+        if not prompt:
+            raise ValueError("Cannot generate from an empty prompt")
+        
+        logger.debug(f"Prompt: █{prompt}█")
+
+        return prompt, genconf
+
+
+
+
     def gen(self, 
             thread: Thread,
             genconf: Optional[GenConf] = None,
             ) -> GenOut:
         """Text generation from a Thread, used by the other model generation methods.
         Doesn't raise an exception if an error occurs, always returns GenOut.
 
@@ -1245,34 +1946,52 @@
             ValueError: If trying to generate from an empty prompt.
             RuntimeError: If unable to generate.
 
         Returns:
             A GenOut object with result, generated text, etc. 
         """
 
-        if genconf is None:
-            genconf = self.genconf
+        genconf2: GenConf
+        prompt, genconf2 = self._gen_pre(thread, genconf)
 
-        thread = self._prepare_gen_in(thread, genconf)
+        text,finish = self._gen_text(prompt, genconf2)
 
-        prompt = self.text_from_thread(thread)
+        return self._prepare_gen_out(text, finish, genconf2)
 
-        if not prompt:
-            raise ValueError("Cannot generate from an empty prompt")
-        
-        logger.debug(f"Prompt: █{prompt}█")
 
-        text,finish = self._gen_text(prompt, genconf)
 
-        out = self._prepare_gen_out(text, finish, genconf)
 
-        return out
+    async def gen_async(self, 
+                        thread: Thread,
+                        genconf: Optional[GenConf] = None,
+                        ) -> GenOut:
+        """Asynchronous generation from a Thread, used by the other model generation methods.
+        Doesn't raise an exception if an error occurs, always returns GenOut.
+
+        Args:
+            thread: The Thread object to use as model input.
+            genconf: Model generation configuration. Defaults to None, which uses model's default.
+
+        Raises:
+            ValueError: If trying to generate from an empty prompt.
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A GenOut object with result, generated text, etc. 
+        """
+
+        genconf2: GenConf
+        prompt, genconf2 = self._gen_pre(thread, genconf)
+
+        text,finish = await self._gen_text_async(prompt, genconf2)
+
+        return self._prepare_gen_out(text, finish, genconf2)
+
 
 
-    
     
     @abstractmethod
     def _gen_text(self,
                   text: str,
                   genconf: GenConf) -> tuple[str,str]:
         """Generate from formatted text.
 
@@ -1285,18 +2004,41 @@
 
         Returns:
             Tuple of strings: generated_text, finish_reason.
         """
         ...
 
 
-    
+    @abstractmethod
+    async def _gen_text_async(self,
+                              text: str,
+                              genconf: GenConf) -> tuple[str,str]:
+        """Asynchronously generate from formatted text.
+
+        Args:
+            text: Formatted text (from input Thread).
+            genconf: Model generation configuration.
+
+        Raises:
+            RuntimeError: If unable to generate.
+
+        Returns:
+            Tuple of strings: generated_text, finish_reason.
+        """
+        ...
+
+
+
+
     def text_from_thread(self,
                          thread: Thread) -> str:
-        """Aply format to transform a Thread into text."""
+        """Apply template format to transform a Thread into text."""
+
+        if self.tokenizer is None:
+            raise ValueError("A FormattedTextModel object requires a tokenizer")
 
         messages = thread.as_chatml()
         text = self._jinja_compiled_template.render(messages=messages, # type: ignore[union-attr]
                                                     add_generation_prompt=True,
                                                     **self.tokenizer.special_tokens_map())
         return text
         
@@ -1329,31 +2071,29 @@
         
         self.is_message_model = True
                 
 
 
     def resolve_settings(self,
                          provider: str,
-                         name: str) -> tuple[str, Union[int,None],Union[int,None],Union[int,None]]:
+                         name: str,
+                         keys: list[str]) -> dict:
         """
-        Return:
-            name, ctx_len, max_tokens_limit, overhead_per_msg
+        Return: dict with values for found keys.            
         """
 
         # 1: locate a provider:name entry in Models (in res/base_models.json or overridden by user settings)
         res_name = provider + ":" + name
         provider, name, args = Models.resolve_model_entry(res_name)
 
-        logger.debug(f"Resolved '{res_name}' to '{provider}:{name}' with args: {args}")
+        logger.debug(f"Resolved '{res_name}' to '{provider}:{name}' with defaults: {args}")
 
 
         # 2: update located defaults with args
-        name = args.get("name") or name
-        ctx_len = args.get("ctx_len")
-        max_tokens_limit = args.get("max_tokens_limit") or ctx_len # defaults to ctx_len
-        overhead_per_msg = args.get("overhead_per_msg")
-
-        return name, ctx_len, max_tokens_limit, overhead_per_msg
-    
+        out = {}
+        for key in keys:
+            if key in args:
+                out[key] = args[key]
+        return out
```

### Comparing `sibila-0.3.6/sibila/models.py` & `sibila-0.4.0/sibila/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class Models:
     """Model and template format directory that unifies (and simplifies) model access and configuration.
 
     This env variable is checked and used during initialization:
         SIBILA_MODELS: ';'-delimited list of folders where to find: models.json, formats.json and model files.
 
 
-    = Model Directory =
+    = Models Directory =
 
     Useful to create models from resource names like "llamacpp:openchat" or "openai:gpt-4". 
     This makes it simple to change a model, store model settings, to compare model outputs, etc.
     
     User can add new entries from script or with JSON filenames, via the add() call.
     New directory entries with the same name are merged into existing ones for each added config.
 
@@ -167,24 +167,39 @@
         "llamacpp": {
             "mandatory": ["name"],
             "flags": ["name_passthrough", "local"]
         },
         "openai": {
             "mandatory": [],
             "flags": ["name_passthrough"]
-        }
+        },
+        "together": {
+            "mandatory": [],
+            "flags": ["name_passthrough"]
+        },
+        "fireworks": {
+            "mandatory": [],
+            "flags": ["name_passthrough"]
+        },
+        "mistral": {
+            "mandatory": [],
+            "flags": ["name_passthrough"]
+        },
     }
     ALL_PROVIDER_NAMES = list(PROVIDER_CONF.keys()) + ["alias"] # providers + "alias"
 
     @classmethod
     def EMPTY_MODELS_DIR(_) -> dict:
         return {
             "llamacpp": {},
             "openai": {},
-            "alias": {}
+            "together": {},
+            "fireworks": {},
+            "mistral": {},
+            "alias": {},
         }
 
     MODELS_CONF_FILENAME = "models.json"
     MODELS_BASE_CONF_FILENAME = "base_" + MODELS_CONF_FILENAME
 
     DEFAULT_ENTRY_NAME = "_default"
 
@@ -371,14 +386,32 @@
         
         elif provider == "openai":
 
             from .openai import OpenAIModel
                     
             model = OpenAIModel(**args)
             
+        elif provider == "together":
+
+            from .schema_format_openai import TogetherModel
+                    
+            model = TogetherModel(**args)
+            
+        elif provider == "fireworks":
+
+            from .schema_format_openai import FireworksModel
+                    
+            model = FireworksModel(**args)
+            
+        elif provider == "mistral":
+
+            from .mistral import MistralModel
+                    
+            model = MistralModel(**args)
+            
         """
         elif provider == "hf":
             from .hf import HFModel
             
             model = HFModel(**args)
         """
```

### Comparing `sibila-0.3.6/sibila/multigen.py` & `sibila-0.4.0/sibila/multigen.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/null.py` & `sibila-0.4.0/sibila/null.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Created later if  needed: NullFormattedTextModel, NullMessagesModel
 """
 
 
 from typing import Any, Optional, Union
 
-import sys, os, json, ctypes
+import sys, os, json, ctypes, time, asyncio
 from copy import copy
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 from .gen import (
@@ -78,20 +78,28 @@
 
         out = self._prepare_gen_out(self.response["text"],
                                     self.response["finish"], 
                                     genconf)
 
         return out
 
+    async def gen_async(self, 
+                        thread: Thread,
+                        genconf: Optional[GenConf] = None,
+                        ) -> GenOut:
+        
+        await asyncio.sleep(0.5)
+        return self.gen(thread, genconf)
+        
 
 
     def token_len(self,
-                  thread: Thread,
+                  thread_or_text: Union[Thread,str],
                   _: Optional[GenConf] = None) -> int:
-        assert False, "NullModel doesn't use tokens"
+        assert False, "NullModel won't use tokens"
 
 
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
         Ex. openai 1.3.6
         """
```

### Comparing `sibila-0.3.6/sibila/openai.py` & `sibila-0.4.0/sibila/openai.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """OpenAI remote model access.
+Using the chat completion API:
+https://platform.openai.com/docs/api-reference/chat/create
 
-- OpenAIModel: Use OpenAI API to access their models.
+- OpenAIModel: Access OpenAI models.
 - OpenAITokenizer: Tokenizer for OpenAI models.
 """
 
 
 from typing import Any, Optional, Union
 import sys, json
 from time import time 
@@ -46,190 +48,223 @@
 
 
 
 class OpenAIModel(MessagesModel):
     """Access an OpenAI model.
 
     Supports constrained JSON output, via the OpenAI API tools mechanism.
-    Ref: https://platform.openai.com/docs/api-reference/chat/create
+
+    Ref:
+        https://platform.openai.com/docs/api-reference/chat/create
 
     Attributes:
-        ctx_len: Maximum context length, shared for input + output.
+        ctx_len: Maximum context length.
         desc: Model information.
     """
 
-    TOOLS_TOKEN_LEN_FACTOR: float
-    """Multiplication factor to use for tools section token length estimation."""
+    PROVIDER_NAME:str = "openai"
+    """Provider prefix that this class handles."""
+
+    _token_estimation_factor: float
+    """Multiplication factor to estimate token usage: multiplies text length to obtain token length."""
+
+    DEFAULT_TOKEN_ESTIMATION_FACTOR: float = 0.4
+    """Default factor for token_estimation_factor."""
+
 
-    DEFAULT_TOOLS_TOKEN_LEN_FACTOR: float = 1.2
 
     def __init__(self,
                  name: str,
                  *,
                  
                  # common base model args
                  genconf: Optional[GenConf] = None,
                  schemaconf: Optional[JSchemaConf] = None,
-                 tokenizer: Optional[Tokenizer] = None,
                  ctx_len: Optional[int] = None,
                  max_tokens_limit: Optional[int] = None,
+                 tokenizer: Optional[Tokenizer] = None,
                 
                  # most important OpenAI-specific args
                  api_key: Optional[str] = None,
                  base_url: Optional[str] = None,
                  overhead_per_msg: Optional[int] = None,
+                 token_estimation_factor: Optional[float] = None,
+                 create_tokenizer: bool = False,
                  
-                 # OpenAI-specific args
-                 openai_init_kwargs: dict = {},
+                 # other OpenAI-specific args
+                 other_init_kwargs: dict = {},
                  ):
         """Create an OpenAI remote model.
-        Name resolution depends on unknown_name_mask and will keep removing letters 
-        from the end of name and searching existing entries in penAIModel.known_models().
 
         Args:
             name: Model name to resolve into an existing model.
             genconf: Model generation configuration. Defaults to None.
             schemaconf: Default configuration for JSON schema validation, used if generation call doesn't supply one. Defaults to None.
-            tokenizer: An external initialized tokenizer to use instead of the created from the GGUF file. Defaults to None.
             ctx_len: Maximum context length to be used (shared for input and output). None for model's default.
             max_tokens_limit: Maximum output tokens limit. None for model's default.
+            tokenizer: An external initialized tokenizer to use instead of the created from the GGUF file. Defaults to None.
             api_key: OpenAI API key. Defaults to None, which will use env variable OPENAI_API_KEY.
-            base_url: Base location for API access. Defaults to None, which will use env variable OPENAI_BASE_URL.
+            base_url: Base location for API access. Defaults to None, which will use env variable OPENAI_BASE_URL or a default.
             overhead_per_msg: Overhead tokens to account for when calculating token length. None for model's default.
-            openai_init_kwargs: Extra args for OpenAI.OpenAI() initialization. Defaults to {}.
+            token_estimation_factor: Used when no tokenizer is available. Multiplication factor to estimate token usage: multiplies total text length to obtain token length.
+            create_tokenizer: When no tokenizer is passed, should try to create one?
+            other_init_kwargs: Extra args for OpenAI.OpenAI() initialization. Defaults to {}.
 
         Raises:
             ImportError: If OpenAI API is not installed.
             NameError: If model name was not found or there's an API or authentication problem.
         """
 
 
         if not has_openai:
             raise ImportError("Please install openai by running: pip install openai")
 
+        self._client = self._client_async = None
+
+
+        # also accept "provider:name" for ease of use
+        provider_name = self.PROVIDER_NAME + ":"
+        if name.startswith(provider_name):
+            name = name[len(provider_name):]
+
         super().__init__(False,
                          genconf,
                          schemaconf,
                          tokenizer
                          )
 
         if (ctx_len is not None and
             max_tokens_limit is not None and
-            overhead_per_msg is not None): # all elements given
+            overhead_per_msg is not None and
+            token_estimation_factor is not None): # all elements given: probably created via Models.create()
 
             self._model_name = name
             default_ctx_len = ctx_len
             default_max_tokens_limit = max_tokens_limit
             default_overhead_per_msg = overhead_per_msg
+            default_token_estimation_factor = token_estimation_factor
         
         else: # need to resolve
-            (self._model_name, 
-             default_ctx_len, default_max_tokens_limit,
-             default_overhead_per_msg) = self.resolve_settings("openai", name) # type: ignore[assignment]
+            settings = self.resolve_settings(self.PROVIDER_NAME,
+                                             name,
+                                             ["name", 
+                                              "ctx_len", 
+                                              "max_tokens_limit", 
+                                              "overhead_per_msg",
+                                              "token_estimation_factor"])
+            self._model_name = settings.get("name") or name
+            default_ctx_len = settings.get("ctx_len") # type: ignore[assignment]
+            default_max_tokens_limit = settings.get("max_tokens_limit") # type: ignore[assignment]
+            default_overhead_per_msg = settings.get("overhead_per_msg") # type: ignore[assignment]
+            default_token_estimation_factor = settings.get("token_estimation_factor") # type: ignore[assignment]
             
             # all defaults are conservative values
-            if default_ctx_len is None:
+            if ctx_len is None and default_ctx_len is None:
                 default_ctx_len = 4096
                 logger.warning(f"Model '{self._model_name}': unknown ctx_len, assuming {default_ctx_len}")
-            if default_max_tokens_limit is None:
-                default_max_tokens_limit = default_ctx_len
-                logger.warning(f"Model '{self._model_name}': unknown max_tokens_limit, assuming {default_max_tokens_limit}")
-            if default_overhead_per_msg is None:
+
+            if max_tokens_limit is None and default_max_tokens_limit is None:
+                default_max_tokens_limit = ctx_len or default_ctx_len                
+                # don't warn: assume equal to ctx_len: logger.warning(f"Model '{self._model_name}': unknown max_tokens_limit, assuming {default_max_tokens_limit}")
+
+            if overhead_per_msg is None and default_overhead_per_msg is None:
                 default_overhead_per_msg = 3
-                logger.warning(f"Model '{self._model_name}': unknown overhead_per_msg, assuming {default_overhead_per_msg}")
+                # don't warn for this setting due to derived model classes (none uses it)
 
+            if token_estimation_factor is None and default_token_estimation_factor is None:
+                default_token_estimation_factor = self.DEFAULT_TOKEN_ESTIMATION_FACTOR
+                logger.warning(f"Model '{self._model_name}': unknown token_estimation_factor, assuming {default_token_estimation_factor}")
 
-        if not ctx_len: # None or 0
-            self.ctx_len = default_ctx_len
-        else:
-            self.ctx_len = ctx_len
-        
-        if not max_tokens_limit:
-            self.max_tokens_limit = default_max_tokens_limit
-        else:
-            self.max_tokens_limit = max_tokens_limit
 
+        self.ctx_len = ctx_len or default_ctx_len
+        
+        self.max_tokens_limit = max_tokens_limit or default_max_tokens_limit
         self.max_tokens_limit = min(self.max_tokens_limit, self.ctx_len)
 
-        if overhead_per_msg is None:
-            self._overhead_per_msg = default_overhead_per_msg
-        else:
-            self._overhead_per_msg = overhead_per_msg
+        self._overhead_per_msg = overhead_per_msg or default_overhead_per_msg
 
-        self.TOOLS_TOKEN_LEN_FACTOR = self.DEFAULT_TOOLS_TOKEN_LEN_FACTOR
+        self._token_estimation_factor = token_estimation_factor or default_token_estimation_factor
 
 
         # only check for "json" text presence as json schema is requested with the tools facility.
         self.json_format_instructors["json_schema"] = self.json_format_instructors["json"]
 
 
-        logger.debug(f"Creating inner OpenAI with ctx_len={self.ctx_len}, max_tokens_limit={self.max_tokens_limit}, _overhead_per_msg={self._overhead_per_msg}, base_url={base_url}, openai_init_kwargs={openai_init_kwargs}")
+        if self.tokenizer is None and create_tokenizer:
+            try:
+                self.tokenizer = OpenAITokenizer(self._model_name)
+            except Exception as e:
+                logger.warning(f"Could not create a local tokenizer for model '{self._model_name}' - "
+                               "token length calculation will be disabled and assume defaults. "
+                               f"Internal error: {e}")
 
 
-        try:
-            if self.tokenizer is None:
-                self.tokenizer = OpenAITokenizer(self._model_name)
-        except Exception as e:
-            raise NameError(f"Model not found for '{self._model_name}'. "
-                            f"Internal error: {e}")
+        self._client_init_kwargs = other_init_kwargs
+        if api_key is not None:
+            self._client_init_kwargs["api_key"] = api_key
+        if base_url is not None:
+            self._client_init_kwargs["base_url"] = base_url
+
 
 
+
+
+
+    def _ensure_client(self,
+                       is_async: bool):
+        if is_async and self._client_async is not None:
+            return
+        elif not is_async and self._client is not None:
+            return
+            
         try:
-            self._client = openai.OpenAI(api_key=api_key,
-                                         base_url=base_url,
-                                         **openai_init_kwargs)
+            logger.debug(f"Creating inner OpenAI with ctx_len={self.ctx_len}, max_tokens_limit={self.max_tokens_limit}, "
+                         f"_overhead_per_msg={self._overhead_per_msg}, _token_estimation_factor={self._token_estimation_factor}, "
+                         f"init_kwargs={self._client_init_kwargs}")
+
+            if is_async:
+                self._client_async = openai.AsyncOpenAI(**self._client_init_kwargs) # type: ignore[assignment]
+            else:
+                self._client = openai.OpenAI(**self._client_init_kwargs) # type: ignore[assignment]
+
         except Exception as e:
-            raise NameError(f"Could not create model '{self._model_name}' with error: {e}")
-    
+            raise NameError(f"Could not create {'async' if is_async else ''} model '{self._model_name}' with error: {e}")
+                
 
 
 
 
 
-    
-    def gen(self, 
-            thread: Thread,
-            genconf: Optional[GenConf] = None,
-            ) -> GenOut:
-        """Text generation from a Thread, used by the other model generation methods.
-        Doesn't raise an exception if an error occurs, always returns GenOut.
 
-        Args:
-            thread: The Thread to use as model input.
-            genconf: Model generation configuration. Defaults to None.
 
-        Raises:
-            RuntimeError: If unable to generate.
 
-        Returns:
-            A GenOut object with result, generated text, etc.
-            The output text is in GenOut.text.
-        """
+    def _gen_pre(self, 
+                 thread: Thread,
+                 genconf: Union[GenConf, None]
+                 ) -> tuple:
 
         if genconf is None:
             genconf = self.genconf
 
-        thread = self._prepare_gen_in(thread, genconf)
-        token_len = self.token_len(thread, genconf)
-
+        thread = self._prepare_gen_thread(thread, genconf)
 
-        # resolve max_tokens size
+        token_len = self.token_len(thread, genconf)
         resolved_max_tokens = self.resolve_genconf_max_tokens(token_len, genconf)
 
+        # for reference: this is a bad idea as endpoint will error on larger than possible max_tokens:
+        # resolved_max_tokens = self.resolve_genconf_max_tokens(0, genconf)
 
         fn_name = "json_out"
 
         json_kwargs: dict = {}
-        format = genconf.format
-        if format == "json":
+        if genconf.format == "json":
             
-            if genconf.json_schema is None:
-                json_kwargs["response_format"] = {"type": "json_object"}
+            json_kwargs["response_format"] = {"type": "json_object"}
 
-            else:
+            if genconf.json_schema is not None:
                 # use json_schema in OpenAi's tool API
                 json_kwargs["tool_choice"] = {
                     "type": "function",
                     "function": {"name": fn_name},
                 }
 
                 if isinstance(genconf.json_schema, str):
@@ -243,138 +278,259 @@
                         "function": {
                             "name": fn_name,
                             "parameters": params
                         }
                     }
                 ]
 
-            logger.debug(f"OpenAI json args: {json_kwargs}")
-
-        # seed config is disabled, has remote models and some hardware accelerated local models don't support it.
+        # seed config is disabled, remote models and some hardware accelerated local models don't support it.
         # seed = genconf.seed
         # if seed == -1:
         #    seed = int(time())
         #    logger.debug(f"OpenAI random seed={seed}")
 
         
         msgs = thread.as_chatml()
 
-        try:
-            # https://platform.openai.com/docs/api-reference/chat/create
-            response = self._client.chat.completions.create(model=self._model_name,
-                                                            messages=msgs, # type: ignore[arg-type]
-                                                            
-                                                            max_tokens=resolved_max_tokens,
-                                                            stop=genconf.stop,
-                                                            temperature=genconf.temperature,
-                                                            top_p=genconf.top_p,
-                                                            # seed=seed,
-                                                            **json_kwargs,
-                                                
-                                                            n=1
-                                                            )
-        except Exception as e:
-            raise RuntimeError(f"Cannot generate. Internal error: {e}")
-        
+        kwargs = {"model": self._model_name,
+                  "messages": msgs, # type: ignore[arg-type]
+                  "max_tokens": resolved_max_tokens,
+                  "stop": genconf.stop,
+                  "temperature": genconf.temperature,
+                  "top_p": genconf.top_p,
+                  # "seed": seed,
+                  "n": 1,
+                  **json_kwargs}
+
+        # inject model-specific args, if any
+        kwargs.update(genconf.resolve_special(self.PROVIDER_NAME))
+
+        logger.debug(f"{type(self).__name__} gen args: {kwargs}")
+
+        return (kwargs,
+                fn_name,
+                genconf)
+        
+
+    def _gen_post(self, 
+                  response: Any,
+                  pre_kwargs: dict,
+                  fn_name: str,
+                  genconf: GenConf
+                  ) -> GenOut:
             
         logger.debug(f"OpenAI response: {response}")
 
         choice = response.choices[0]
         finish = choice.finish_reason
+        # OpenAI-compatible provider endpoints can give non-standard finish_reason values. Map as needed:
+        if finish in ["eos", "tool_calls"]: finish = "stop"
         message = choice.message
 
-        if "tool_choice" in json_kwargs:
+        if "tool_choice" in pre_kwargs:
             
             # json schema generation via the tools API:
             if message.tool_calls is not None:
+                if len(message.tool_calls) != 1:
+                    logger.warn(f"OpenAIModel: expecting single message.tool_calls, but received {len(message.tool_calls)} - using first.")
+
                 fn = message.tool_calls[0].function
                 if fn.name != fn_name:
-                    logger.debug(f"OpenAIModel: different returned JSON function name ({fn.name})")
+                    logger.warn(f"OpenAIModel: expecting '{fn_name}' function name, received ({fn.name})")
 
                 text = fn.arguments
+
             else: # use content instead
+                logger.warn("OpenAIModel: expecting message.tool_calls, but none received - using text content")
                 text = message.content # type: ignore[assignment]
         
         else:
             # text or simple json format
             text = message.content # type: ignore[assignment]
 
-        out = self._prepare_gen_out(text, finish, genconf)
+        return self._prepare_gen_out(text, finish, genconf)
 
-        return out
 
-        
 
 
+
+
+
+    
+    def gen(self, 
+            thread: Thread,
+            genconf: Optional[GenConf] = None,
+            ) -> GenOut:
+        """Text generation from a Thread, used by the other model generation methods.
+        Doesn't raise an exception if an error occurs, always returns GenOut.
+
+        Args:
+            thread: The Thread to use as model input.
+            genconf: Model generation configuration. Defaults to None.
+
+        Raises:
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A GenOut object with result, generated text, etc.
+            The output text is in GenOut.text.
+        """
+
+        genconf2: GenConf
+        kwargs, fn_name, genconf2 = self._gen_pre(thread, genconf)
+
+        self._ensure_client(False)
+
+        try:
+            # https://platform.openai.com/docs/api-reference/chat/create
+            response = self._client.chat.completions.create(**kwargs) # type: ignore[attr-defined]
+
+        except Exception as e:
+            raise RuntimeError(f"Cannot generate. Internal error: {e}")
+
+
+        return self._gen_post(response,
+                              kwargs,
+                              fn_name,
+                              genconf2)
     
 
 
+
+    async def gen_async(self, 
+                        thread: Thread,
+                        genconf: Optional[GenConf] = None,
+                        ) -> GenOut:
+        """Async text generation from a Thread, used by the other (async) generation methods.
+        Doesn't raise an exception if an error occurs, always returns GenOut.
+
+        Args:
+            thread: The Thread to use as model input.
+            genconf: Model generation configuration. Defaults to None.
+
+        Raises:
+            RuntimeError: If unable to generate.
+
+        Returns:
+            A GenOut object with result, generated text, etc.
+            The output text is in GenOut.text.
+        """
+
+        genconf2: GenConf
+        kwargs, fn_name, genconf2 = self._gen_pre(thread, genconf)
+
+        self._ensure_client(True)
+
+        try:
+            # https://platform.openai.com/docs/api-reference/chat/create
+            response = await self._client_async.chat.completions.create(**kwargs) # type: ignore[attr-defined]
+
+        except Exception as e:
+            raise RuntimeError(f"Cannot generate. Internal error: {e}")
+
+        return self._gen_post(response,
+                              kwargs,
+                              fn_name,
+                              genconf2)
+    
+
+   
+
+
+
+
+
     def token_len(self,
-                  thread: Thread,
+                  thread_or_text: Union[Thread,str],
                   genconf: Optional[GenConf] = None) -> int:
-        """Calculate the number of tokens used by a list of messages.
+        """Estimate the number of tokens used by a Thread or text string.
         If a json_schema is provided in genconf, we use its string's token_len as upper bound for the extra prompt tokens.
         
         From https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
         
         More info on calculating function_call (and tools?) tokens:
 
         https://community.openai.com/t/how-to-calculate-the-tokens-when-using-function-call/266573/24
         
         https://gist.github.com/CGamesPlay/dd4f108f27e2eec145eedf5c717318f5
 
         Args:
-            thread: For token length calculation.
+            thread_or_text: For token length calculation.
             genconf: Model generation configuration. Defaults to None.
 
         Returns:
-            Estimated number of tokens the thread will use.
+            Estimated number of tokens used.
         """
 
-        # name = self._model_name
+        if isinstance(thread_or_text, Thread):
+            thread = thread_or_text            
+        else:
+            thread = Thread.make_IN(thread_or_text)
 
         num_tokens = 0
-        for index in range(-1, len(thread)): # -1 for system message
-            message = thread.msg_as_chatml(index)
-            # print(message)
-            num_tokens += self._overhead_per_msg
-            for key, value in message.items():
-                num_tokens += len(self.tokenizer.encode(value))
-                # if key == "name":
-                #     num_tokens += self._tokens_per_name
-        
-        num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
-        num_tokens += 10 # match API return counts
 
-        # print("text token_len", num_tokens)
+        if self.tokenizer is None: # no tokenizer was found, so we'll have to do a conservative estimate
 
-        if genconf is not None and genconf.json_schema is not None:
-            if isinstance(genconf.json_schema, str):
-                js_str = genconf.json_schema
-            else:
-                js_str = json.dumps(genconf.json_schema)
+            OVERHEAD_PER_MSG = 3
+            for index in range(-1, len(thread)): # -1 for system message
+                message = thread.msg_as_chatml(index)
+                msg_tokens = len(message["content"]) * self._token_estimation_factor + OVERHEAD_PER_MSG
+                num_tokens += int(msg_tokens)
 
-            tools_num_tokens = self.tokenizer.token_len(js_str)
+            if genconf is not None and genconf.json_schema is not None:
+                if isinstance(genconf.json_schema, str):
+                    js_str = genconf.json_schema
+                else:
+                    js_str = json.dumps(genconf.json_schema)
 
-            # this is an upper bound, as empirically tested with the api.
-            tools_num_tokens = int(tools_num_tokens * self.TOOLS_TOKEN_LEN_FACTOR)
+                tools_num_tokens = len(js_str) * self._token_estimation_factor
+                num_tokens += int(tools_num_tokens)
+                # print("tools_num_tokens", tools_num_tokens)
 
-            # print("tools token_len", tools_num_tokens)
 
-            num_tokens += tools_num_tokens
+        else: # do an "informed" token estimation from what is known of the OpenAI model's tokenization
+            
+            for index in range(-1, len(thread)): # -1 for system message
+                message = thread.msg_as_chatml(index)
+                # print(message)
+                num_tokens += self._overhead_per_msg
+                for key, value in message.items():
+                    num_tokens += len(self.tokenizer.encode(value))
+            
+            # add extras + every reply is primed with <|start|>assistant<|message|>
+            num_tokens += 32
+
+            # print("text token_len", num_tokens)
+
+            if genconf is not None and genconf.json_schema is not None:
+                TOOLS_TOKEN_LEN_FACTOR = 1.2
+
+                if isinstance(genconf.json_schema, str):
+                    js_str = genconf.json_schema
+                else:
+                    js_str = json.dumps(genconf.json_schema)
+
+                tools_num_tokens = self.tokenizer.token_len(js_str)
+
+                # this is an upper bound, as empirically tested with the api.
+                tools_num_tokens = int(tools_num_tokens * TOOLS_TOKEN_LEN_FACTOR)
+                # print("tools token_len", tools_num_tokens)
+
+                num_tokens += tools_num_tokens
+
         
         return num_tokens
 
 
 
     
     @property
     def desc(self) -> str:
         """Model description."""
-        return f"OpenAIModel: {self._model_name}"
+        return f"{type(self).__name__}: '{self._model_name}'"
 
 
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
         Ex. openai 1.3.6
         """
@@ -382,22 +538,35 @@
             import openai
             ver = openai.__version__
         except Exception:
             raise ImportError("Please install openai by running: pip install openai")
             
         return f"openai {ver}"
     
+    
     @classmethod
-    def known_models(cls) -> Union[list[str], None]:
-        """If the model can only use a fixed set of models, return their names. Otherwise, return None.
+    def known_models(cls,
+                     api_key: Optional[str] = None) -> Union[list[str], None]:
+        """List of model names that can be used. Some of the models are not chat models and cannot be used,
+        for example embedding models.
+        
+        Args:
+            api_key: Requires OpenAI API key, passed as this arg or set in env variable OPENAI_API_KEY.
 
         Returns:
-            Returns a list of known models or None if it can accept any model.
+            Returns a list of known models.
         """
-        return None
+ 
+        client = openai.OpenAI(api_key=api_key)
+        model_list = client.models.list()
+
+        out = []
+        for model in model_list.data:
+            out.append(model.id)
+        return sorted(out)
 
 
 
 
 
 
 class OpenAITokenizer(Tokenizer):
```

### Comparing `sibila-0.3.6/sibila/res/base_formats.json` & `sibila-0.4.0/sibila/res/base_formats.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,8 +1,17 @@
 {
+    "tinyllama": {
+        "match": "tinyllama",
+        "template": "zephyr"
+    },
+    "llama2": {
+        "match": "llama.+chat",
+        "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = '<<SYS>>\n' + messages[0]['content'].strip() + '\n<</SYS>>\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ ' '  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}"
+    },
+    "llama": "llama2",
     "hermes2": {
         "match": "hermes-[^1]",
         "template": "chatml"
     },
     "hermes": {
         "match": "hermes-",
         "template": "alpaca"
@@ -65,19 +74,14 @@
         "match": "falcon.+(instruct|chat)",
         "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'] %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{{ system_message.strip() }}{% endif %}{{ '\n\n' + message['role'].title() + ': ' + message['content'].strip().replace('\r\n', '\n').replace('\n\n', '\n') }}{% endfor %}{% if add_generation_prompt %}{{ '\n\nAssistant:' }}{% endif %}"
     },
     "gemma": {
         "match": "gemma.+it",
         "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if (message['role'] == 'assistant') %}{% set role = 'model' %}{% else %}{% set role = message['role'] %}{% endif %}{{ '<start_of_turn>' + role + '\n' + content.strip() + '<end_of_turn>\n' }}{% endfor %}{% if add_generation_prompt %}{{'<start_of_turn>model\n'}}{% endif %}"
     },
-    "llama2": {
-        "match": "llama.+chat",
-        "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = '<<SYS>>\n' + messages[0]['content'].strip() + '\n<</SYS>>\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ bos_token + '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ ' '  + content.strip() + ' ' + eos_token }}{% endif %}{% endfor %}"
-    },
-    "llama": "llama2",
     "mistral": {
         "match": "mistral.+instruct",
         "template": "{{ bos_token }}{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if loop.index0 == 0 %}{% set content = system_message + message['content'] %}{% else %}{% set content = message['content'] %}{% endif %}{% if message['role'] == 'user' %}{{ '[INST] ' + content.strip() + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ content.strip() + eos_token}}{% endif %}{% endfor %}"
     },
     "mixtral": {
         "match": "mixtral.+instruct",
         "template": "mistral"
@@ -94,18 +98,14 @@
         "match": "solar.+instruct",
         "template": "{% for message in messages %}{% if message['role'] == 'system' %}{% if message['content']%}{{'### System:\n' + message['content'].strip() +'\n\n'}}{% endif %}{% elif message['role'] == 'user' %}{{'### User:\n' + message['content'].strip() +'\n\n'}}{% elif message['role'] == 'assistant' %}{{'### Assistant:\n'  + message['content'].strip() +'\n\n' }}{% endif %}{% if loop.last and add_generation_prompt %}{{ '### Assistant:\n' }}{% endif %}{% endfor %}"
     },
     "starling": {
         "match": "starling.lm",
         "template": "openchat"
     },
-    "tinyllama": {
-        "match": "tinyllama",
-        "template": "zephyr"
-    },
     "yi": {
         "match": "yi.+chat",
         "template": "chatml"
     },
     "wizard-coder": {
         "match": "wizardcoder",
         "template": "{% if messages[0]['role'] == 'system' %}{% set loop_messages = messages[1:] %}{% set system_message = messages[0]['content'].strip() + '\n\n' %}{% else %}{% set loop_messages = messages %}{% set system_message = '' %}{% endif %}{{ system_message }}{% for message in loop_messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ '### Instruction:\n' + message['content'].strip() + '\n\n' }}{% elif message['role'] == 'assistant' %}{{ '### Response:\n' + message['content'].strip() + '\n\n' }}{% endif %}{% endfor %}{% if add_generation_prompt %}{{ '### Response:\n' }}{% endif %}"
```

### Comparing `sibila-0.3.6/sibila/text_splitter.py` & `sibila-0.4.0/sibila/text_splitter.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/thread.py` & `sibila-0.4.0/sibila/thread.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila/tools.py` & `sibila-0.4.0/sibila/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
         token_len = model.token_len(thread)
         max_token_len = model.ctx_len - resolved_max_tokens - (token_len + 16) 
     
 
     # split initial text
     logger.debug(f"Max ctx token len {max_token_len}")
     
-    token_len_fn = model.tokenizer.token_len_lambda
+    token_len_fn = model.token_len_lambda
     logger.debug(f"Initial text token_len {token_len_fn(text)}") # type: ignore[arg-type]
     
     spl = RecursiveTextSplitter(max_token_len, overlap_size, len_fn=token_len_fn)
 
     round = 0
     while True: # summarization rounds
         logger.debug(f"Round {round} {'='*60}")
```

### Comparing `sibila-0.3.6/sibila/utils.py` & `sibila-0.4.0/sibila/utils.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/sibila.egg-info/PKG-INFO` & `sibila-0.4.0/sibila.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.3.6
+Version: 0.4.0
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
@@ -16,32 +16,35 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: llama-cpp-python
-Requires-Dist: jinja2
-Requires-Dist: typing_extensions
-Requires-Dist: jsonschema
-Requires-Dist: openai
+Requires-Dist: llama-cpp-python>=0.2
+Requires-Dist: openai>=1.1
 Requires-Dist: tiktoken
-Requires-Dist: pydantic
+Requires-Dist: mistralai
+Requires-Dist: jinja2>=3.0
+Requires-Dist: jsonschema
+Requires-Dist: pydantic>=2.0
+Requires-Dist: typing_extensions
 Requires-Dist: tqdm
 
 # Sibila
 
-Extract structured data from remote or local file LLM models.
+Extract structured data from remote or local LLM models. Predictable output is essential for any serious use of LLMs.
 
 - Extract data into Pydantic objects, dataclasses or simple types.
-- Same API for local file models and remote OpenAI models.
-- Model management: download models, manage configuration and quickly switch between models.
+- Same API for local file models and remote OpenAI, Mistral AI and other models.
+- Model management: download models, manage configuration, quickly switch between models.
 - Tools for evaluating output across local/remote models, for chat-like interaction and more.
 
+No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
+
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
 To extract structured data from a local model:
 
 ``` python
 from sibila import Models
 from pydantic import BaseModel
@@ -72,29 +75,30 @@
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
 
-If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass.
+If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass. Also includes asynchronous access to remote models.
+
 
 
 
 ## Docs
 
 [The docs explain](https://jndiogo.github.io/sibila/) the main concepts, include examples and an API reference.
 
 
 ## Installation
 
 Sibila can be installed from PyPI by doing:
 
 ```
-pip install sibila
+pip install --upgrade sibila
 ```
 
 See [Getting started](https://jndiogo.github.io/sibila/installing/) for more information.
 
 
 
 ## Examples
@@ -118,13 +122,13 @@
 - [TheBloke (Tom Jobbins)](https://huggingface.co/TheBloke) and [Hugging Face model hub](https://huggingface.co/)
 
 Thank you!
 
 
 ## Sibila?
 
-Sibila is the Portuguese word for Sibyl. [The Sibyls](https://en.wikipedia.org/wiki/Sibyl) were wise oracular women in ancient Greece. Their mysterious words puzzled people throughout the centuries, providing insight or prophetic predictions.
+Sibila is the Portuguese word for Sibyl. [The Sibyls](https://en.wikipedia.org/wiki/Sibyl) were wise oracular women in ancient Greece. Their mysterious words puzzled people throughout the centuries, providing insight or prophetic predictions, "uttering things not to be laughed at".
 
 ![Michelangelo's Delphic Sibyl, Sistine Chapel ceiling](https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/DelphicSibylByMichelangelo.jpg/471px-DelphicSibylByMichelangelo.jpg)
 
 Michelangelo's Delphic Sibyl, in the Sistine Chapel ceiling.
```

### Comparing `sibila-0.3.6/sibila.egg-info/SOURCES.txt` & `sibila-0.4.0/sibila.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 sibila/__init__.py
 sibila/cli.py
 sibila/context.py
 sibila/gen.py
 sibila/json_grammar.py
 sibila/json_schema.py
 sibila/llamacpp.py
+sibila/mistral.py
 sibila/model.py
 sibila/models.py
 sibila/multigen.py
 sibila/null.py
 sibila/openai.py
+sibila/schema_format_openai.py
 sibila/text_splitter.py
 sibila/thread.py
 sibila/tools.py
 sibila/utils.py
 sibila.egg-info/PKG-INFO
 sibila.egg-info/SOURCES.txt
 sibila.egg-info/dependency_links.txt
@@ -24,14 +26,17 @@
 sibila.egg-info/requires.txt
 sibila.egg-info/top_level.txt
 sibila/res/__init__.py
 sibila/res/base_formats.json
 sibila/res/base_models.json
 tests/test_cli.py
 tests/test_examples_tinyllama.py
-tests/test_extract.py
+tests/test_fireworks_mixtral.py
 tests/test_formats.py
 tests/test_json_schema.py
 tests/test_llamacpp_models.py
 tests/test_llamacpp_tinyllama.py
+tests/test_mistral_small.py
+tests/test_null_extract.py
 tests/test_openai_gpt35.py
-tests/test_openai_gpt4.py
+tests/test_openai_gpt4.py
+tests/test_together_mixtral.py
```

### Comparing `sibila-0.3.6/tests/test_cli.py` & `sibila-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/tests/test_extract.py` & `sibila-0.4.0/tests/test_null_extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,18 +110,26 @@
         """Class for keeping track of an item in inventory."""
         name: str
         unit_price: float
         alistia: list[int]
         anno: Annotated[str, "This is anno"] = "30"
         quantity_on_hand: int = 0
 
-    extract(Inv,
-            "A lot of nice things but no meaning at all",
-            '{ "name": "Item", "unit_price": 0, "alistia": [], "anno": "30", "quantity_on_hand": 0}',
-            Inv(name='Item', unit_price=0, alistia=[], anno='30', quantity_on_hand=0))
+    target = Inv
+    text = "A lot of nice things but no meaning at all"
+    response = '{ "name": "Item", "unit_price": 0, "alistia": [], "anno": "30", "quantity_on_hand": 0}'
+    expected = Inv(name='Item', unit_price=0, alistia=[], anno='30', quantity_on_hand=0)
+    extract(target,
+            text,
+            response,
+            expected)
+
+    model.set_response(response)
+    assert model.dataclass(target, text) == expected
+
 
 
 
 
 
 def test_pydantic():
 
@@ -136,24 +144,35 @@
             [UserDetail(name='Paul', age=68), UserDetail(name='Mathilda', age=81)])
 
     class UserDetail(BaseModel):
         """ Details about a user """
         name: str = Field(..., description="The name for the user")
         age: int = Field(..., description="The user's age")
 
+    target = UserDetail
+    text = "Jane's 99 years old."
+    response = '{"name": "Jane", "age": 99}'
+    expected = UserDetail(name='Jane', age=99)
+    extract(target,
+            text,
+            response,
+            expected)
+
+    model.set_response(response)
+    assert model.pydantic(target, text) == expected
+
+
     extract(list[UserDetail],
             "Jane's 99 years old, Paul is 75.",
             '{"output": [{"name": "Jane", "age": 99}, {"name": "Paul", "age": 75}]}',
             [UserDetail(name='Jane', age=99), UserDetail(name='Paul', age=75)])
 
 
 
 
-
-
 def test_classify():
 
     classify(["yes", "no"], 
              "I will never make it on time",
              '{"output": "no"}',
              "no")
```

### Comparing `sibila-0.3.6/tests/test_formats.py` & `sibila-0.4.0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/tests/test_json_schema.py` & `sibila-0.4.0/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `sibila-0.3.6/tests/test_llamacpp_models.py` & `sibila-0.4.0/tests/test_llamacpp_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 from sibila import (
      LlamaCppModel
 )
 
 
-
+"""
+clear; pytest -s test_llamacpp_models.py --models_dir ../../models/
+"""
 
 LIMIT = 9999
 
 @pytest.fixture(scope="module")
 def models_list(pytestconfig):
     models_dir = pytestconfig.getoption("models_dir")
```

### Comparing `sibila-0.3.6/tests/test_llamacpp_tinyllama.py` & `sibila-0.4.0/tests/test_fireworks_mixtral.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,255 +1,299 @@
+"""
+Requires a defined env variable TOGETHER_API_KEY with a valid API key.
+See:
+https://docs.together.ai/docs/inference-models
+"""
+
 import pytest
 
-import os, subprocess, shutil, json
+import os, subprocess, shutil, json, asyncio
 from typing import Any, Optional, Union, Literal, Annotated, get_origin, get_args
 
 import logging
 logger = logging.getLogger(__name__)
 # pytest --log-cli-level=DEBUG
 
+from dotenv import load_dotenv
+
+
 from sibila import (
     Models,
-    LlamaCppModel,
-    GenConf
+    FireworksModel,
+    GenConf,
+    GenError
 )
 
 
+
 from .utils import setup_env_models, teardown_env_models, setup_model, teardown_model
 from .utils import run_cmd, run_text, run_json
 
 
+MODEL_NAME = "accounts/fireworks/models/mixtral-8x7b-instruct"
+IN_CTX_LEN = 32768
+OUT_MAX_TOKENS = IN_CTX_LEN
 
 
-# https://huggingface.co/TheBloke/TinyLlama-1.1B-Chat-v1.0-GGUF
-MODEL_FILENAME = "tinyllama-1.1b-chat-v1.0.Q4_K_M.gguf"
-
 DO_TEARDOWN = True
 
 @pytest.fixture(autouse=True, scope="module")
 def env_model():
 
-    base_dir, models_dir = setup_env_models("llamacpp", 
+    load_dotenv(override=True, verbose=True)
+
+    base_dir, models_dir = setup_env_models("fireworks-mixtral", 
                                             change_cwd=True,
                                             full_clean=False)
 
-    model_path = setup_model(MODEL_FILENAME, 
-                             models_dir,
-                             always_copy=False)
-
-    ret = base_dir, model_path
+    ret = base_dir, models_dir
     print("---> setup", ret)
     
     yield ret
 
     # --------------------------- teardown
     if DO_TEARDOWN == False:
         return
 
     print("---> teardown", ret)
 
-    teardown_model(model_path)
-
     teardown_env_models(base_dir)
 
 
 
 
 
+def create_model(ctx_len: int = IN_CTX_LEN):
+    model = FireworksModel(MODEL_NAME, 
+                          ctx_len=ctx_len)
+    return model
 
 
 
 
 
-def test_create_llamacppmodel(env_model):
-
-    full_model_path = env_model[1]
-    rel_model_path = os.path.join("models", MODEL_FILENAME)
+def test_create_together(env_model):
 
-    # model file not found
-    with pytest.raises(NameError):
-        model = LlamaCppModel(full_model_path + "NOT_THERE")
-
-    # relative path
-    model = LlamaCppModel(rel_model_path, format="zephyr")
+    model = create_model()
     del model
 
-    # absolute path
-    model = LlamaCppModel(full_model_path)
+    # models are only checked when used, so no NameError
+    # with pytest.raises(NameError):
+    model = FireworksModel(MODEL_NAME + "NOT_THERE")
     del model
 
 
 
 
 
 def test_models(env_model):
 
-    base_dir = env_model[0]
-    models_dir_path = os.path.join(base_dir, "models")
-    models_json_path = os.path.join(models_dir_path, "models.json")
-
-    full_model_path = env_model[1]
-    rel_model_path = os.path.join("models", MODEL_FILENAME)
-
-    name = "local-model"
-    res_name = f"llamacpp:{name}"
-    link_name = f"{name}-link"
-    link_res_name = f"llamacpp:{link_name}"
-
-
-    # avoid any existing models.json
-    if os.path.isfile(models_json_path):
-        os.remove(models_json_path)
-
-    # create model entry
-    cmd = f"sibila models -m models/ -s {res_name} {MODEL_FILENAME} zephyr"
-    run_json(cmd, 
-             path=models_json_path,
-             expected_json={
-                    "llamacpp": {
-                        name: {
-                            "name": MODEL_FILENAME,
-                            "format": "zephyr"
-                        }
-                    }
-                })
-
-    # create model link
-    cmd = f"sibila models -m models/ -sl {link_res_name} {name}"
-    run_json(cmd, 
-             path=models_json_path,
-             expected_json={
-                    "llamacpp": {
-                        name: {
-                            "name": MODEL_FILENAME,
-                            "format": "zephyr"
-                        },
-                        link_name: name
-                    }
-                })
-    
-
+    with pytest.raises(NameError):
+        res_name = MODEL_NAME
+        model = Models.create(res_name)
+        del model
 
 
-    # model file not found
-    with pytest.raises(NameError):
-        model = Models.create(res_name + "NOT_THIS")
+    # models are only checked when used, so no NameError
+    # with pytest.raises(NameError):
+    res_name = "together:NOT_THERE"
+    model = Models.create(res_name)
+    del model
 
-    # Models.setup() not called ===============================================
     with pytest.raises(NameError):
+        res_name = "NOT_THERE"
         model = Models.create(res_name)
+        del model
 
-    # rel_path
-    model = Models.create("llamacpp:" + rel_model_path)
-    del model
-
-    # absolute path
-    model = Models.create("llamacpp:" + full_model_path)
-    del model
 
 
-    # Models.setup() called ===================================================
     Models.setup("models")
 
+    res_name = "together:" + MODEL_NAME
     model = Models.create(res_name)
     del model
 
-    model = Models.create(link_res_name)
-    del model
 
+    Models.setup("models", clear=True)
+
+    res_name = "together:" + MODEL_NAME
+    model = Models.create(res_name)
+    del model
 
 
 
 
 
 
 def test_ctx_len(env_model):
     
-    rel_model_path = os.path.join("models", MODEL_FILENAME)
-
-    model = LlamaCppModel(rel_model_path, format="zephyr")
-    assert model.ctx_len == 2048
-    assert model.max_tokens_limit == 2048
-    del model
-
-
-    model = LlamaCppModel(rel_model_path, format="zephyr",
-                          ctx_len=0)
-    assert model.ctx_len == 2048
-    assert model.max_tokens_limit == 2048
+    model = create_model()
+    # print(model.ctx_len, model.max_tokens_limit)
+    assert model.ctx_len == IN_CTX_LEN
+    assert model.max_tokens_limit == OUT_MAX_TOKENS
+    del model
+
+    """ defaults depend on base_models.json: don't test
+    model = FireworksModel(MODEL_NAME,
+                           ctx_len=0)
+    assert model.ctx_len == IN_CTX_LEN
+    assert model.max_tokens_limit == OUT_MAX_TOKENS
     del model
+    """
 
-    model = LlamaCppModel(rel_model_path, format="zephyr",
-                          ctx_len=1024)
+    model = FireworksModel(MODEL_NAME,
+                           ctx_len=1024)
     assert model.ctx_len == 1024
     assert model.max_tokens_limit == 1024
     del model
 
 
 
 
 
 
 def test_max_tokens(env_model):
     
-    rel_model_path = os.path.join("models", MODEL_FILENAME)
-
-    model = LlamaCppModel(rel_model_path, format="zephyr")
-    CTX_LEN = 2048
-
-    assert model.calc_max_max_tokens(0) == CTX_LEN-0
-    assert model.calc_max_max_tokens(500) == CTX_LEN-500
-    assert model.calc_max_max_tokens(3000) == CTX_LEN-3000
+    model = create_model()
 
+    assert model.calc_max_max_tokens(0) == OUT_MAX_TOKENS
+    assert model.calc_max_max_tokens(500) == OUT_MAX_TOKENS - 500
+    assert model.calc_max_max_tokens(3000) == OUT_MAX_TOKENS - 3000
+    assert model.calc_max_max_tokens(16000) == OUT_MAX_TOKENS - 16000
 
     genconf=GenConf(max_tokens=1000)    
     assert genconf.resolve_max_tokens(model.ctx_len, model.max_tokens_limit) == 1000
     assert model.resolve_genconf_max_tokens(100, genconf) == 1000
-    assert model.resolve_genconf_max_tokens(1500, genconf) == CTX_LEN - 1500
+    assert model.resolve_genconf_max_tokens(1500, genconf) == 1000
 
     genconf=GenConf(max_tokens=-20)
-    assert genconf.resolve_max_tokens(model.ctx_len, model.max_tokens_limit) == int(CTX_LEN * 20/100)
-    assert model.resolve_genconf_max_tokens(100, genconf) == int(CTX_LEN * 20/100)
-    assert model.resolve_genconf_max_tokens(1900, genconf) == CTX_LEN - 1900
+    max_tokens = int(OUT_MAX_TOKENS * 20 / 100)
+    assert genconf.resolve_max_tokens(model.ctx_len, model.max_tokens_limit) == max_tokens
+    assert model.resolve_genconf_max_tokens(100, genconf) == max_tokens
+    assert model.resolve_genconf_max_tokens(1900, genconf) == max_tokens
 
     genconf=GenConf(max_tokens=0)    
-    assert genconf.resolve_max_tokens(model.ctx_len, model.max_tokens_limit) == 2048
-    assert model.resolve_genconf_max_tokens(100, genconf) == CTX_LEN - 100
-    assert model.resolve_genconf_max_tokens(1900, genconf) == CTX_LEN - 1900
+    assert genconf.resolve_max_tokens(model.ctx_len, model.max_tokens_limit) == OUT_MAX_TOKENS
+    assert model.resolve_genconf_max_tokens(100, genconf) == OUT_MAX_TOKENS - 100
+    assert model.resolve_genconf_max_tokens(1900, genconf) == OUT_MAX_TOKENS - 1900
+    
+    with pytest.raises(ValueError):
+        assert model.resolve_genconf_max_tokens(160*1000, genconf)
 
     del model
 
 
 
 
 
-def test_prompt(env_model):
 
-    rel_model_path = os.path.join("models", MODEL_FILENAME)
+def test_prompt(env_model):
 
-    PROMPT = "Tell me about oranges"
+    PROMPT = "Tell me briefly about oranges"
     HAS = "orange"
 
-    model = LlamaCppModel(rel_model_path, format="zephyr")
+    model = create_model()
     text = model(PROMPT)
+    print(text)
     assert HAS in text.lower()
     del model
 
 
 
 
 
-def test_extract(env_model):
 
-    rel_model_path = os.path.join("models", MODEL_FILENAME)
+INT_PROMPT = "extract the number from the following text: there are twelve bananas"
+TRUE_PROMPT = "extract True/False from the following text: Yes I got it!"
+CTX_LEN = 200
 
-    model = LlamaCppModel(rel_model_path, format="zephyr")
 
+def test_extract(env_model):
+
+    model = create_model(ctx_len=CTX_LEN)
 
-    res = model.extract(int, "twelve bananas")
+    res = model.extract(int, INT_PROMPT)
     assert res == 12
 
-    res = model.extract(bool, "Yes I got it!")
+    res = model.extract(bool, TRUE_PROMPT)
     assert res == True
 
     del model
 
+
+
+
+
+def test_extract_async1(env_model):
+
+    model = create_model(ctx_len=CTX_LEN)
+
+    async def run_async():
+        print("run_async begin")
+
+        res = await model.extract_async(int, INT_PROMPT)
+        assert res == 12
+
+        res = await model.extract_async(bool, TRUE_PROMPT)
+        assert res == True
+        print("run_async done")
+        
+    asyncio.run(run_async())
+
+
+
+
+def test_extract_async2(env_model):
+
+    model = create_model(ctx_len=CTX_LEN)
+
+    async def run1_async():        
+        print("run1 begin")
+        res = await model.extract_async(int, INT_PROMPT)
+        assert res == 12
+        print("run1 done")
+
+    async def run2_async():
+        print("run2 begin")
+        res = await model.extract_async(bool, TRUE_PROMPT)
+        assert res == True
+        print("run2 done")
+
+
+    async def gather():
+        print("gather begin")
+        tasks = [run1_async(), run2_async()]
+        await asyncio.gather(*tasks)
+        print("gather done")
+            
+    asyncio.run(gather())    
+
+
+
+def test_extract_async3(env_model):
+
+    model = create_model(ctx_len=CTX_LEN)
+
+    async def run1_async():        
+        print("run1 begin")
+        res = await model.extract_async(int, INT_PROMPT)
+        assert res == 12
+        print("run1 done")
+
+    async def run2_async():
+        print("run2 begin")
+        res = await model.extract_async(bool, TRUE_PROMPT)
+        assert res == True
+        print("run2 done")
+
+
+    async def as_completed():
+        print("as_complete begin")
+        tasks = [run1_async(), run2_async()]
+        for task in asyncio.as_completed(tasks):
+            await task
+        print("as_complete done")
+            
+    asyncio.run(as_completed())    
+
+
+
```

