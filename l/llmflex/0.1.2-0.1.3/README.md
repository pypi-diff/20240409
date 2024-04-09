# Comparing `tmp/llmflex-0.1.2.tar.gz` & `tmp/llmflex-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflex-0.1.2.tar", last modified: Mon Mar 18 17:33:36 2024, max compression
+gzip compressed data, was "llmflex-0.1.3.tar", last modified: Tue Apr  9 19:26:50 2024, max compression
```

## Comparing `llmflex-0.1.2.tar` & `llmflex-0.1.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.217321 llmflex-0.1.2/
--rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.2/LICENSE.md
--rw-r--r--   0 nathan95   (501) staff       (20)     9749 2024-03-18 17:33:36.217075 llmflex-0.1.2/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     8568 2024-03-11 17:44:28.000000 llmflex-0.1.2/README.md
--rw-r--r--   0 nathan95   (501) staff       (20)     1196 2024-02-24 22:31:02.000000 llmflex-0.1.2/pyproject.toml
--rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-03-18 17:33:36.217373 llmflex-0.1.2/setup.cfg
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.208088 llmflex-0.1.2/src/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.209658 llmflex-0.1.2/src/llmflex/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.210870 llmflex-0.1.2/src/llmflex/Data/
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Data/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Data/sqlite_database.py
--rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Data/vector_database.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.211554 llmflex-0.1.2/src/llmflex/Embeddings/
--rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Embeddings/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4400 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Embeddings/api_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4245 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Embeddings/base_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.2/src/llmflex/Embeddings/hf_embeddings_server.py
--rw-r--r--   0 nathan95   (501) staff       (20)     3998 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Embeddings/huggingface_embeddings.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.211943 llmflex-0.1.2/src/llmflex/Frontend/
--rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Frontend/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Frontend/gradio_interface.py
--rw-r--r--   0 nathan95   (501) staff       (20)    37390 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Frontend/streamlit_interface.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.212447 llmflex-0.1.2/src/llmflex/Memory/
--rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Memory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Memory/assistant_long_term_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Memory/base_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Memory/long_short_memory.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.212578 llmflex-0.1.2/src/llmflex/Models/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.213523 llmflex-0.1.2/src/llmflex/Models/Cores/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Models/Cores/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14712 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Models/Cores/base_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.2/src/llmflex/Models/Cores/exllamav2_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Models/Cores/huggingface_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.2/src/llmflex/Models/Cores/llamacpp_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9239 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Models/Cores/openai_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7368 2024-02-28 15:01:21.000000 llmflex-0.1.2/src/llmflex/Models/Cores/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.213772 llmflex-0.1.2/src/llmflex/Models/Factory/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Models/Factory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    10725 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Models/Factory/llm_factory.py
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Models/__init__.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.214044 llmflex-0.1.2/src/llmflex/Prompts/
--rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Prompts/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14902 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Prompts/prompt_template.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.214348 llmflex-0.1.2/src/llmflex/Schemas/
--rw-r--r--   0 nathan95   (501) staff       (20)       31 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Schemas/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)      140 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Schemas/documents.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.215025 llmflex-0.1.2/src/llmflex/TextSplitters/
--rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/TextSplitters/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/TextSplitters/base_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/TextSplitters/sentence_token_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1485 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/TextSplitters/token_text_splitter.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.215654 llmflex-0.1.2/src/llmflex/Tools/
--rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Tools/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Tools/base_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Tools/tool_selection.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11406 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/Tools/web_search_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)    14418 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/Tools/web_search_utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.216282 llmflex-0.1.2/src/llmflex/VectorDBs/
--rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/VectorDBs/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    23475 2024-03-18 15:18:53.000000 llmflex-0.1.2/src/llmflex/VectorDBs/base_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)     5008 2024-03-15 22:38:26.000000 llmflex-0.1.2/src/llmflex/VectorDBs/faiss_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-03-18 15:18:53.000000 llmflex-0.1.2/src/llmflex/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.2/src/llmflex/cli.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.2/src/llmflex/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-03-18 17:33:36.216487 llmflex-0.1.2/src/llmflex.egg-info/
--rw-r--r--   0 nathan95   (501) staff       (20)     9749 2024-03-18 17:33:36.000000 llmflex-0.1.2/src/llmflex.egg-info/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     1903 2024-03-18 17:33:36.000000 llmflex-0.1.2/src/llmflex.egg-info/SOURCES.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-03-18 17:33:36.000000 llmflex-0.1.2/src/llmflex.egg-info/dependency_links.txt
--rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-03-18 17:33:36.000000 llmflex-0.1.2/src/llmflex.egg-info/entry_points.txt
--rw-r--r--   0 nathan95   (501) staff       (20)      323 2024-03-18 17:33:36.000000 llmflex-0.1.2/src/llmflex.egg-info/requires.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-03-18 17:33:36.000000 llmflex-0.1.2/src/llmflex.egg-info/top_level.txt
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.976054 llmflex-0.1.3/
+-rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.3/LICENSE.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     9750 2024-04-09 19:26:50.975682 llmflex-0.1.3/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     8569 2024-04-09 19:26:07.000000 llmflex-0.1.3/README.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     1196 2024-02-24 22:31:02.000000 llmflex-0.1.3/pyproject.toml
+-rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-04-09 19:26:50.976099 llmflex-0.1.3/setup.cfg
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.962074 llmflex-0.1.3/src/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.963637 llmflex-0.1.3/src/llmflex/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.964711 llmflex-0.1.3/src/llmflex/Data/
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Data/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4919 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Data/sqlite_database.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    20029 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Data/vector_database.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.965618 llmflex-0.1.3/src/llmflex/Embeddings/
+-rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Embeddings/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4400 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Embeddings/api_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4245 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Embeddings/base_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.3/src/llmflex/Embeddings/hf_embeddings_server.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     3998 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Embeddings/huggingface_embeddings.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.966031 llmflex-0.1.3/src/llmflex/Frontend/
+-rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Frontend/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Frontend/gradio_interface.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    37390 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Frontend/streamlit_interface.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.966567 llmflex-0.1.3/src/llmflex/Memory/
+-rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Memory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Memory/assistant_long_term_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8703 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Memory/base_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Memory/long_short_memory.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.966695 llmflex-0.1.3/src/llmflex/Models/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.967574 llmflex-0.1.3/src/llmflex/Models/Cores/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Models/Cores/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14712 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Cores/base_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.3/src/llmflex/Models/Cores/exllamav2_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9508 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Cores/huggingface_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8610 2024-02-25 22:17:53.000000 llmflex-0.1.3/src/llmflex/Models/Cores/llamacpp_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9239 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Cores/openai_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7368 2024-02-28 15:01:21.000000 llmflex-0.1.3/src/llmflex/Models/Cores/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.967799 llmflex-0.1.3/src/llmflex/Models/Factory/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Models/Factory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    10725 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Models/Factory/llm_factory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Models/__init__.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.968030 llmflex-0.1.3/src/llmflex/Prompts/
+-rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Prompts/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14910 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/Prompts/prompt_template.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.968262 llmflex-0.1.3/src/llmflex/Schemas/
+-rw-r--r--   0 nathan95   (501) staff       (20)       31 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Schemas/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      140 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Schemas/documents.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.968730 llmflex-0.1.3/src/llmflex/TextSplitters/
+-rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/base_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2709 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/sentence_token_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1485 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/TextSplitters/token_text_splitter.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.969373 llmflex-0.1.3/src/llmflex/Tools/
+-rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Tools/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Tools/base_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Tools/tool_selection.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11406 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/Tools/web_search_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    14418 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/Tools/web_search_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.970895 llmflex-0.1.3/src/llmflex/VectorDBs/
+-rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/VectorDBs/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    23515 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/VectorDBs/base_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     5018 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/VectorDBs/faiss_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-04-09 19:26:07.000000 llmflex-0.1.3/src/llmflex/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.3/src/llmflex/cli.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.3/src/llmflex/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-04-09 19:26:50.971099 llmflex-0.1.3/src/llmflex.egg-info/
+-rw-r--r--   0 nathan95   (501) staff       (20)     9750 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     1903 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/entry_points.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)      323 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/requires.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-04-09 19:26:50.000000 llmflex-0.1.3/src/llmflex.egg-info/top_level.txt
```

### Comparing `llmflex-0.1.2/LICENSE.md` & `llmflex-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/PKG-INFO` & `llmflex-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -130,15 +130,15 @@
 from llmflex.VectorDBs import FaissVectorDatabase
 
 # Loading the embedding model toolkit
 embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-large")
 
 # Create a vector database
 food = ["Apple", "Banana", "Pork"]
-vectordb = FaissVectorDatabase.from_data(index=food, embeddings=embeddings)
+vectordb = FaissVectorDatabase.from_texts(index=food, embeddings=embeddings)
 
 # Do semantic search on the vector database
 print(vectordb.search("Beef"))
 ```
 
 ### 3. Use memory and prompt template to create a chatbot
 Use the Memory classes and the `PromptTemplate` class to create a chatbot.
```

### Comparing `llmflex-0.1.2/README.md` & `llmflex-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 from llmflex.VectorDBs import FaissVectorDatabase
 
 # Loading the embedding model toolkit
 embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-large")
 
 # Create a vector database
 food = ["Apple", "Banana", "Pork"]
-vectordb = FaissVectorDatabase.from_data(index=food, embeddings=embeddings)
+vectordb = FaissVectorDatabase.from_texts(index=food, embeddings=embeddings)
 
 # Do semantic search on the vector database
 print(vectordb.search("Beef"))
 ```
 
 ### 3. Use memory and prompt template to create a chatbot
 Use the Memory classes and the `PromptTemplate` class to create a chatbot.
```

### Comparing `llmflex-0.1.2/pyproject.toml` & `llmflex-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Data/sqlite_database.py` & `llmflex-0.1.3/src/llmflex/Data/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Data/vector_database.py` & `llmflex-0.1.3/src/llmflex/Data/vector_database.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Embeddings/api_embeddings.py` & `llmflex-0.1.3/src/llmflex/Embeddings/api_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Embeddings/base_embeddings.py` & `llmflex-0.1.3/src/llmflex/Embeddings/base_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Embeddings/hf_embeddings_server.py` & `llmflex-0.1.3/src/llmflex/Embeddings/hf_embeddings_server.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Embeddings/huggingface_embeddings.py` & `llmflex-0.1.3/src/llmflex/Embeddings/huggingface_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Frontend/gradio_interface.py` & `llmflex-0.1.3/src/llmflex/Frontend/gradio_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Frontend/streamlit_interface.py` & `llmflex-0.1.3/src/llmflex/Frontend/streamlit_interface.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Memory/assistant_long_term_memory.py` & `llmflex-0.1.3/src/llmflex/Memory/assistant_long_term_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Memory/base_memory.py` & `llmflex-0.1.3/src/llmflex/Memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Memory/long_short_memory.py` & `llmflex-0.1.3/src/llmflex/Memory/long_short_memory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Cores/base_core.py` & `llmflex-0.1.3/src/llmflex/Models/Cores/base_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Cores/exllamav2_core.py` & `llmflex-0.1.3/src/llmflex/Models/Cores/exllamav2_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Cores/huggingface_core.py` & `llmflex-0.1.3/src/llmflex/Models/Cores/huggingface_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Cores/llamacpp_core.py` & `llmflex-0.1.3/src/llmflex/Models/Cores/llamacpp_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Cores/openai_core.py` & `llmflex-0.1.3/src/llmflex/Models/Cores/openai_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Cores/utils.py` & `llmflex-0.1.3/src/llmflex/Models/Cores/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Models/Factory/llm_factory.py` & `llmflex-0.1.3/src/llmflex/Models/Factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Prompts/prompt_template.py` & `llmflex-0.1.3/src/llmflex/Prompts/prompt_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         'bos_token': '<s>',
         'stop': ['\nASSISTANT', '\nUSER:', 'ASSISTANT:', 'USER:', '</s>']
     },
     'ChatML' : {
         'template': "{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}",
         'eos_token': '<|im_end|>',
         'bos_token': '<|endoftext|>',
-        'stop': ['<|im_start|>', '<|im_end|>', '<|im_start|>user\n', '<|im_end|>\n<|im_start|>user\n']
+        'stop': ['<|im_start|>', '<|im_end|>', '<|im_start|>user\n', '<|im_end|>\n<|im_start|>user\n', '</s>']
     },
     'Zephyr' : {
         'template': "{% for message in messages %}\n{% if message['role'] == 'user' %}\n{{ '<|user|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'system' %}\n{{ '<|system|>\n' + message['content'] + eos_token }}\n{% elif message['role'] == 'assistant' %}\n{{ '<|assistant|>\n'  + message['content'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}",
         'eos_token': '</s>',
         'bos_token': '<s>',
         'stop': ['</s>', '</s>\n', '<|user|>\n', '</s>\n<|user|>\n']
     },
```

### Comparing `llmflex-0.1.2/src/llmflex/TextSplitters/base_text_splitter.py` & `llmflex-0.1.3/src/llmflex/TextSplitters/base_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/TextSplitters/sentence_token_text_splitter.py` & `llmflex-0.1.3/src/llmflex/TextSplitters/sentence_token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/TextSplitters/token_text_splitter.py` & `llmflex-0.1.3/src/llmflex/TextSplitters/token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Tools/base_tool.py` & `llmflex-0.1.3/src/llmflex/Tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Tools/tool_selection.py` & `llmflex-0.1.3/src/llmflex/Tools/tool_selection.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Tools/web_search_tool.py` & `llmflex-0.1.3/src/llmflex/Tools/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/Tools/web_search_utils.py` & `llmflex-0.1.3/src/llmflex/Tools/web_search_utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/VectorDBs/base_vectordb.py` & `llmflex-0.1.3/src/llmflex/VectorDBs/base_vectordb.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     if '\t' in name:
         raise ValueError(f'Tab characters cannot be in the name.')
     return name
 
 class BaseVectorDatabase(ABC):
     """Base class for vector databases.
     """
-    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None) -> None:
+    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, **kwargs) -> None:
         """Initialise a vector database.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
         """
@@ -218,15 +218,15 @@
 
         Returns:
             np.ndarray[np.float32]: Arrray of vectors.
         """
         pass
 
     @classmethod
-    def from_exist(cls, embeddings: Type[BaseEmbeddingsToolkit], name: str, vectordb_dir: Optional[str] = None) -> BaseVectorDatabase:
+    def from_exist(cls, embeddings: Type[BaseEmbeddingsToolkit], name: str, vectordb_dir: Optional[str] = None, **kwargs) -> BaseVectorDatabase:
         """Load the vector database from an existing vector database.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             name (str): Name of the existing database.
             vectordbs_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
 
@@ -267,15 +267,15 @@
             vdb.info['embeddings'] = embeddings.name
         vdb.save()
         return vdb
 
     @classmethod
     def from_documents(cls, embeddings: Type[BaseEmbeddingsToolkit], docs: List[Document], 
                       name: Optional[str] = None, vectordb_dir: Optional[str] = None,
-                      split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None) -> BaseVectorDatabase:
+                      split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> BaseVectorDatabase:
         """Load the vector database from existing documents.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             docs (List[Document]): List of documents to use.
             name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
@@ -289,15 +289,15 @@
         vdb.add_documents(docs=docs, split_text=split_text, text_splitter=text_splitter)
         vdb.save() # In case an empty list of docs is given.
         return vdb
     
     @classmethod
     def from_texts(cls, embeddings: Type[BaseEmbeddingsToolkit], texts: List[str], metadata: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
                       name: Optional[str] = None, vectordb_dir: Optional[str] = None,
-                      split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None) -> BaseVectorDatabase:
+                      split_text: bool = True, text_splitter: Optional[Type[BaseTextSplitter]] = None, **kwargs) -> BaseVectorDatabase:
         """Load the vector database from existing texts.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             texts (List[str]): List of texts to add.
             metadata (Optional[Union[Dict[str, Any], List[Dict[str, Any]]]], optional): Metadata to add along with the texts. Defaults to None.
             name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
```

### Comparing `llmflex-0.1.2/src/llmflex/VectorDBs/faiss_vectordb.py` & `llmflex-0.1.3/src/llmflex/VectorDBs/faiss_vectordb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ..Schemas.documents import Document
 from .base_vectordb import BaseVectorDatabase
 from typing import List, Any, Type, Optional, Tuple
 import os, numpy as np
 
 class FaissVectorDatabase(BaseVectorDatabase):
 
-    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None) -> None:
+    def __init__(self, embeddings: Type[BaseEmbeddingsToolkit], name: Optional[str] = None, vectordb_dir: Optional[str] = None, **kwargs) -> None:
         """Initialise a vector database.
 
         Args:
             embeddings (Type[BaseEmbeddingsToolkit]): Embeddings toolkit to use.
             name (Optional[str], optional): Name of the vector database. Will be used as the directory base name of the vector database in vectordb_dir. If None is given, the vector database will not be saved. Defaults to None.
             vectordb_dir (Optional[str], optional): Directory where the vector databases live. If None is given, the default_vectordb_dir will be used. Defaults to None.
         """
```

### Comparing `llmflex-0.1.2/src/llmflex/cli.py` & `llmflex-0.1.3/src/llmflex/cli.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex/utils.py` & `llmflex-0.1.3/src/llmflex/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.2/src/llmflex.egg-info/PKG-INFO` & `llmflex-0.1.3/src/llmflex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -130,15 +130,15 @@
 from llmflex.VectorDBs import FaissVectorDatabase
 
 # Loading the embedding model toolkit
 embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-large")
 
 # Create a vector database
 food = ["Apple", "Banana", "Pork"]
-vectordb = FaissVectorDatabase.from_data(index=food, embeddings=embeddings)
+vectordb = FaissVectorDatabase.from_texts(index=food, embeddings=embeddings)
 
 # Do semantic search on the vector database
 print(vectordb.search("Beef"))
 ```
 
 ### 3. Use memory and prompt template to create a chatbot
 Use the Memory classes and the `PromptTemplate` class to create a chatbot.
```

### Comparing `llmflex-0.1.2/src/llmflex.egg-info/SOURCES.txt` & `llmflex-0.1.3/src/llmflex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

