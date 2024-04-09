# Comparing `tmp/docindex-0.1.0.tar.gz` & `tmp/docindex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docindex-0.1.0.tar", last modified: Mon Apr  8 13:14:16 2024, max compression
+gzip compressed data, was "docindex-0.2.0.tar", last modified: Mon Apr  8 20:00:56 2024, max compression
```

## Comparing `docindex-0.1.0.tar` & `docindex-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 13:14:11.000000 docindex-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-08 13:14:16.001561 docindex-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-08 13:14:11.000000 docindex-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 13:14:11.000000 docindex-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 13:14:16.001561 docindex-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:15.997561 docindex-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/src/_google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/docindex.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_google/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/src/_openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/doc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-08 13:14:11.000000 docindex-0.1.0/src/_openai/docindex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:14:16.001561 docindex-0.1.0/src/docindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 13:14:15.000000 docindex-0.1.0/src/docindex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:56.870861 docindex-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 20:00:51.000000 docindex-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-08 20:00:56.870861 docindex-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-08 20:00:51.000000 docindex-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 20:00:51.000000 docindex-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 20:00:56.870861 docindex-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:56.866861 docindex-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:56.866861 docindex-0.2.0/src/_google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_google/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_google/delete_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_google/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_google/docindex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:56.866861 docindex-0.2.0/src/_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_openai/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_openai/delete_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_openai/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_openai/doc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-08 20:00:51.000000 docindex-0.2.0/src/_openai/docindex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:00:56.870861 docindex-0.2.0/src/docindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-08 20:00:56.000000 docindex-0.2.0/src/docindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 20:00:56.000000 docindex-0.2.0/src/docindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:00:56.000000 docindex-0.2.0/src/docindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 20:00:56.000000 docindex-0.2.0/src/docindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 20:00:56.000000 docindex-0.2.0/src/docindex.egg-info/top_level.txt
```

### Comparing `docindex-0.1.0/LICENSE` & `docindex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docindex-0.1.0/PKG-INFO` & `docindex-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docindex
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for fast indexing of multiple documents and their metadata on Pinecone.
 Home-page: https://github.com/KevKibe/docindex
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,25 +14,28 @@
 Requires-Dist: pypdf==4.1.0
 Requires-Dist: unstructured==0.12.6
 Requires-Dist: langchain-community==0.0.31
 Requires-Dist: langchain==0.1.14
 Requires-Dist: langchain-openai==0.1.1
 Requires-Dist: langchain-google-genai==1.0.1
 
-<h1 align="center">DocIndex: Fast Document Embeddings Storage for RAG</h1>
+<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for RAG</h1>
 <p align="center">
 
   <a href="https://github.com/KevKibe/docindex/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/docindex?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/docindex/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/docindex?" alt="License">
   </a>
+<br>
 
-*Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) models Fast* 
+![Diagram](image.png)
+
+*Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) models Fast* 
 
 ## Features
 
 - ⚡️ **Rapid Indexing**: Quickly index multiple documents along with their metadata, including source, page details, and content, into Pinecone DB.<br>
 - 📚 **Document Flexibility**: Index documents from your local storage or online sources with ease.<br>
 - 📂 **Format Support**: Seamlessly handle various document formats, including PDF, docx(in-development), etc.<br>
 - 🔁 **Embedding Services Integration**: Enjoy support for multiple embedding services such as OpenAI Embeddings, Google Generative AI Embeddings and more in development.<br>
@@ -41,38 +44,45 @@
 ## Setup
 
 ```python
 pip install docindex
 ```
 
 ## Getting Started
+- Sign up to [Pinecone](https://www.pinecone.io/) and get an API key.
 ## Using OpenAI 
 ```python
 from _openai.docindex import OpenaiPineconeIndexer
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key, and environment
+# Replace these values with your actual Pinecone API key, index name, OpenAI API key
 pinecone_api_key = "pinecone-api-key"
 index_name = "pinecone-index-name"
 openai_api_key = "openai-api-key"
-environment = "pinecone-index-environment"
 batch_limit = 20 # Batch limit for upserting documents
 chunk_size = 256 # Optional: size of texts per chunk. 
 
 # List of URLs of the documents to be indexed. (offline on your computer or online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.pdf"
 ]
 
 # Initialize the Pinecone indexer
-pinecone_index = OpenaiPineconeIndexer(index_name, pinecone_api_key, environment, openai_api_key)
+pinecone_index = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)
+
+# To create a new Index
+pinecone_index.create_index()
 
-# Index the documents with the specified URLs and batch limit
+# Store the document embeddings with the specified URLs and batch limit
 pinecone_index.index_documents(urls,batch_limit,chunk_size)
 ```
+```python
+# To delete the created Index
+pinecone_index.delete_index()
+```
 ## Initialize Vectorstore(using OpenAI)
 
 ```python
 from pinecone import Pinecone as IndexPinecone
 from langchain_community.vectorstores import Pinecone as VectorStorePinecone
 from langchain.embeddings.openai import OpenAIEmbeddings
 
@@ -82,47 +92,49 @@
         
 # Initialize OpenAI embeddings if you're using OpenAI embeddings
 embed = OpenAIEmbeddings(
         model = 'text-embedding-ada-002',
         openai_api_key = openai_api_key
         )
 
-# Define the text field
-text_field = "text"
-
 # Initialize the Vectorstore with the Pinecone index and OpenAI embeddings
-vectorstore = VectorStorePinecone(index, embed, text_field)
+vectorstore = VectorStorePinecone(index, embed, "text")
 ```
 
 
 ## Using Google Generative AI  
 
 ```python
 from _google.docindex import GooglePineconeIndexer
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key, and environment
+# Replace these values with your actual Pinecone API key, index name, Google API key
 pinecone_api_key = "pinecone-api-key"
 index_name = "pinecone-index-name"
 google_api_key = "google-api-key"
-environment = "pinecone-index-environment"
 batch_limit = 20 # Batch limit for upserting documents
 chunk_size = 256 # Optional: size of texts per chunk. 
 
 # List of URLs of the documents to be indexed. (offline on your computer or an online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.pdf"
 ]
 
-# Initialize the Pinecone indexer
-pinecone_index = GooglePineconeIndexer(index_name, pinecone_api_key, environment, google_api_key)
+pinecone_index = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)
 
-# Index the documents with the specified URLs and batch limit
+# To create a new Index
+pinecone_index.create_index()
+
+# Store the document embeddings with the specified URLs and batch limit
 pinecone_index.index_documents(urls,batch_limit,chunk_size)
 ```
+```python
+# To delete the created Index
+pinecone_index.delete_index()
+```
 
 
 ## Initialize Vectorstore(using Google Generative AI)
 
 ```python
 from pinecone import Pinecone as IndexPinecone
 from langchain_community.vectorstores import Pinecone as VectorStorePinecone
@@ -134,19 +146,16 @@
         
 # Initialize embeddings 
 embed = GoogleGenerativeAIEmbeddings(
         model="models/embedding-001", 
         google_api_key=google_api_key
         )
 
-# Define the text field
-text_field = "text"
-
 # Initialize the Vectorstore with the Pinecone index and OpenAI embeddings
-vectorstore = VectorStorePinecone(index, embed, text_field)
+vectorstore = VectorStorePinecone(index, embed, "text")
 ```
 
 
 
 
 ## Using the CLI
 
@@ -171,24 +180,46 @@
 pip install -r requirements.txt
 ```
 
 - Navigate to src 
 ```bash
 cd src
 ```
+- To create an index
+
+```bash
+# Using OpenAI 
+python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+```
+
+```bash
+# Using Google Generative AI
+python -m  _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
+```
 
 - Run the command to start indexing the documents
 
 ```bash
 # Using OpenAI 
-python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --environment "your_environment" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
 ```
 ```bash
 # Using Google Generative AI 
-python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --environment "your_environment" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+```
+- To delete an index
+
+```bash
+# Using OpenAI 
+python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+```
+
+```bash
+# Using Google Generative AI
+python -m  _google.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,90 +1,102 @@
-Metadata-Version: 2.1 Name: docindex Version: 0.1.0 Summary: A package for fast
+Metadata-Version: 2.1 Name: docindex Version: 0.2.0 Summary: A package for fast
 indexing of multiple documents and their metadata on Pinecone. Home-page:
 https://github.com/KevKibe/docindex Author: Kevin Kibe Author-email:
 keviinkibe@gmail.com License: MIT Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pinecone-client==3.2.2
 Requires-Dist: tiktoken==0.6.0 Requires-Dist: pypdf==4.1.0 Requires-Dist:
 unstructured==0.12.6 Requires-Dist: langchain-community==0.0.31 Requires-Dist:
 langchain==0.1.14 Requires-Dist: langchain-openai==0.1.1 Requires-Dist:
 langchain-google-genai==1.0.1
-       ************ DDooccIInnddeexx:: FFaasstt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
-_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]*Efficiently store multiple document embeddings and their
-  metadata, whether they're offline or online, in a Pinecone Vector Database
- optimized for Retrieval Augmented Generation (RAG) models Fast* ## Features -
- â¡ï¸ **Rapid Indexing**: Quickly index multiple documents along with their
-   metadata, including source, page details, and content, into Pinecone DB.
+  ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
+                            _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
+![Diagram](image.png) *Efficiently store multiple document embeddings and their
+ metadata, whether they're offline or online, in a persistent Pinecone Vector
+  Database optimized for Retrieval Augmented Generation (RAG) models Fast* ##
+ Features - â¡ï¸ **Rapid Indexing**: Quickly index multiple documents along
+with their metadata, including source, page details, and content, into Pinecone
+                                      DB.
   - ð **Document Flexibility**: Index documents from your local storage or
                            online sources with ease.
     - ð **Format Support**: Seamlessly handle various document formats,
                    including PDF, docx(in-development), etc.
 - ð **Embedding Services Integration**: Enjoy support for multiple embedding
 services such as OpenAI Embeddings, Google Generative AI Embeddings and more in
                                  development.
  - ð ï¸ **Configurable Vectorstore**: Configure a vectorstore directly from
   the index to facilitate RAG pipelines effortlessly. ## Setup ```python pip
-    install docindex ``` ## Getting Started ## Using OpenAI ```python from
+   install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
+     www.pinecone.io/) and get an API key. ## Using OpenAI ```python from
 _openai.docindex import OpenaiPineconeIndexer # Replace these values with your
-     actual Pinecone API key, index name, OpenAI API key, and environment
-   pinecone_api_key = "pinecone-api-key" index_name = "pinecone-index-name"
- openai_api_key = "openai-api-key" environment = "pinecone-index-environment"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
+    actual Pinecone API key, index name, OpenAI API key pinecone_api_key =
+"pinecone-api-key" index_name = "pinecone-index-name" openai_api_key = "openai-
+ api-key" batch_limit = 20 # Batch limit for upserting documents chunk_size =
+256 # Optional: size of texts per chunk. # List of URLs of the documents to be
  indexed. (offline on your computer or online) urls = [ "your-document-1.pdf",
   "your-document-2.pdf" ] # Initialize the Pinecone indexer pinecone_index =
-       OpenaiPineconeIndexer(index_name, pinecone_api_key, environment,
- openai_api_key) # Index the documents with the specified URLs and batch limit
- pinecone_index.index_documents(urls,batch_limit,chunk_size) ``` ## Initialize
-     Vectorstore(using OpenAI) ```python from pinecone import Pinecone as
-    IndexPinecone from langchain_community.vectorstores import Pinecone as
-VectorStorePinecone from langchain.embeddings.openai import OpenAIEmbeddings #
-            Initialize the Pinecone index index_pc = IndexPinecone
-  (api_key=pinecone_api_key) index = index_pc.Index(index_name) # Initialize
- OpenAI embeddings if you're using OpenAI embeddings embed = OpenAIEmbeddings
-( model = 'text-embedding-ada-002', openai_api_key = openai_api_key ) # Define
-   the text field text_field = "text" # Initialize the Vectorstore with the
- Pinecone index and OpenAI embeddings vectorstore = VectorStorePinecone(index,
-      embed, text_field) ``` ## Using Google Generative AI ```python from
-_google.docindex import GooglePineconeIndexer # Replace these values with your
-     actual Pinecone API key, index name, OpenAI API key, and environment
-   pinecone_api_key = "pinecone-api-key" index_name = "pinecone-index-name"
- google_api_key = "google-api-key" environment = "pinecone-index-environment"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
-   indexed. (offline on your computer or an online) urls = [ "your-document-
-       1.pdf", "your-document-2.pdf" ] # Initialize the Pinecone indexer
+OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key) # To create
+a new Index pinecone_index.create_index() # Store the document embeddings with
+       the specified URLs and batch limit pinecone_index.index_documents
+   (urls,batch_limit,chunk_size) ``` ```python # To delete the created Index
+   pinecone_index.delete_index() ``` ## Initialize Vectorstore(using OpenAI)
+         ```python from pinecone import Pinecone as IndexPinecone from
+ langchain_community.vectorstores import Pinecone as VectorStorePinecone from
+ langchain.embeddings.openai import OpenAIEmbeddings # Initialize the Pinecone
+index index_pc = IndexPinecone(api_key=pinecone_api_key) index = index_pc.Index
+ (index_name) # Initialize OpenAI embeddings if you're using OpenAI embeddings
+ embed = OpenAIEmbeddings( model = 'text-embedding-ada-002', openai_api_key =
+   openai_api_key ) # Initialize the Vectorstore with the Pinecone index and
+ OpenAI embeddings vectorstore = VectorStorePinecone(index, embed, "text") ```
+     ## Using Google Generative AI ```python from _google.docindex import
+GooglePineconeIndexer # Replace these values with your actual Pinecone API key,
+ index name, Google API key pinecone_api_key = "pinecone-api-key" index_name =
+  "pinecone-index-name" google_api_key = "google-api-key" batch_limit = 20 #
+Batch limit for upserting documents chunk_size = 256 # Optional: size of texts
+  per chunk. # List of URLs of the documents to be indexed. (offline on your
+computer or an online) urls = [ "your-document-1.pdf", "your-document-2.pdf" ]
      pinecone_index = GooglePineconeIndexer(index_name, pinecone_api_key,
-environment, google_api_key) # Index the documents with the specified URLs and
-batch limit pinecone_index.index_documents(urls,batch_limit,chunk_size) ``` ##
-  Initialize Vectorstore(using Google Generative AI) ```python from pinecone
- import Pinecone as IndexPinecone from langchain_community.vectorstores import
-      Pinecone as VectorStorePinecone from langchain_google_genai import
+ google_api_key) # To create a new Index pinecone_index.create_index() # Store
+        the document embeddings with the specified URLs and batch limit
+pinecone_index.index_documents(urls,batch_limit,chunk_size) ``` ```python # To
+   delete the created Index pinecone_index.delete_index() ``` ## Initialize
+Vectorstore(using Google Generative AI) ```python from pinecone import Pinecone
+   as IndexPinecone from langchain_community.vectorstores import Pinecone as
+            VectorStorePinecone from langchain_google_genai import
     GoogleGenerativeAIEmbeddings # Initialize the Pinecone index index_pc =
  IndexPinecone(api_key=pinecone_api_key) index = index_pc.Index(index_name) #
   Initialize embeddings embed = GoogleGenerativeAIEmbeddings( model="models/
-    embedding-001", google_api_key=google_api_key ) # Define the text field
- text_field = "text" # Initialize the Vectorstore with the Pinecone index and
- OpenAI embeddings vectorstore = VectorStorePinecone(index, embed, text_field)
-``` ## Using the CLI - Clone the Repository: Clone or download the application
-   code to your local machine. ```bash git clone https://github.com/KevKibe/
- docindex.git ``` - Create a virtual environment for the project and activate
-   it. ```bash # Navigate to project repository cd docindex # create virtual
-environment python -m venv venv # activate virtual environment source venv/bin/
-activate ``` - Install dependencies by running this command ```bash pip install
--r requirements.txt ``` - Navigate to src ```bash cd src ``` - Run the command
-        to start indexing the documents ```bash # Using OpenAI python -
+ embedding-001", google_api_key=google_api_key ) # Initialize the Vectorstore
+with the Pinecone index and OpenAI embeddings vectorstore = VectorStorePinecone
+ (index, embed, "text") ``` ## Using the CLI - Clone the Repository: Clone or
+download the application code to your local machine. ```bash git clone https://
+  github.com/KevKibe/docindex.git ``` - Create a virtual environment for the
+project and activate it. ```bash # Navigate to project repository cd docindex #
+ create virtual environment python -m venv venv # activate virtual environment
+  source venv/bin/activate ``` - Install dependencies by running this command
+ ```bash pip install -r requirements.txt ``` - Navigate to src ```bash cd src
+``` - To create an index ```bash # Using OpenAI python -m _openai.create_index
+ --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
+ openai_api_key "your_openai_api_key" ``` ```bash # Using Google Generative AI
+ python -m _google.create_index --pinecone_api_key "your_pinecone_api_key" --
+ index_name "your_index_name" --google_api_key "your_google_api_key" ``` - Run
+  the command to start indexing the documents ```bash # Using OpenAI python -
   m _openai.doc_index --pinecone_api_key "your_pinecone_api_key" --index_name
-    "your_index_name" --openai_api_key "your_openai_api_key" --environment
-"your_environment" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --chunk_size
-  256 ``` ```bash # Using Google Generative AI python -m _google.doc_index --
-  pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
-   google_api_key "your_google_api_key" --environment "your_environment" --
-     batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ##
-  Contributing Contributions are welcome and encouraged. Before contributing,
-     please take a moment to review our [Contribution Guidelines](https://
-  github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important
-   information on how to contribute to this project. If you're unsure about
-anything or need assistance, don't hesitate to reach out to us or open an issue
- to discuss your ideas. We look forward to your contributions! ## License This
-    project is licensed under the MIT License - see the [LICENSE](https://
- github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
-    For any enquiries, please reach out to me through keviinkibe@gmail.com
+ "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --
+   docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ```bash # Using Google
+         Generative AI python -m _google.doc_index --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
+   "your_google_api_key" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --
+    chunk_size 256 ``` - To delete an index ```bash # Using OpenAI python -
+m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
+ "your_index_name" --openai_api_key "your_openai_api_key" ``` ```bash # Using
+    Google Generative AI python -m _google.delete_index --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
+    "your_google_api_key" ``` ## Contributing Contributions are welcome and
+     encouraged. Before contributing, please take a moment to review our
+[Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
+    CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
+     details. ## Contact For any enquiries, please reach out to me through
+                             keviinkibe@gmail.com
```

### Comparing `docindex-0.1.0/README.md` & `docindex-0.2.0/src/docindex.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,41 @@
-<h1 align="center">DocIndex: Fast Document Embeddings Storage for RAG</h1>
+Metadata-Version: 2.1
+Name: docindex
+Version: 0.2.0
+Summary: A package for fast indexing of multiple documents and their metadata on Pinecone.
+Home-page: https://github.com/KevKibe/docindex
+Author: Kevin Kibe
+Author-email: keviinkibe@gmail.com
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pinecone-client==3.2.2
+Requires-Dist: tiktoken==0.6.0
+Requires-Dist: pypdf==4.1.0
+Requires-Dist: unstructured==0.12.6
+Requires-Dist: langchain-community==0.0.31
+Requires-Dist: langchain==0.1.14
+Requires-Dist: langchain-openai==0.1.1
+Requires-Dist: langchain-google-genai==1.0.1
+
+<h1 align="center">DocIndex: Fast Persistent Document Embeddings Storage for RAG</h1>
 <p align="center">
 
   <a href="https://github.com/KevKibe/docindex/commits/">
     <img src="https://img.shields.io/github/last-commit/KevKibe/docindex?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/docindex/blob/master/LICENSE">
     <img src="https://img.shields.io/github/license/KevKibe/docindex?" alt="License">
   </a>
+<br>
+
+![Diagram](image.png)
 
-*Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) models Fast* 
+*Efficiently store multiple document embeddings and their metadata, whether they're offline or online, in a persistent Pinecone Vector Database optimized for Retrieval Augmented Generation (RAG) models Fast* 
 
 ## Features
 
 - ⚡️ **Rapid Indexing**: Quickly index multiple documents along with their metadata, including source, page details, and content, into Pinecone DB.<br>
 - 📚 **Document Flexibility**: Index documents from your local storage or online sources with ease.<br>
 - 📂 **Format Support**: Seamlessly handle various document formats, including PDF, docx(in-development), etc.<br>
 - 🔁 **Embedding Services Integration**: Enjoy support for multiple embedding services such as OpenAI Embeddings, Google Generative AI Embeddings and more in development.<br>
@@ -21,38 +44,45 @@
 ## Setup
 
 ```python
 pip install docindex
 ```
 
 ## Getting Started
+- Sign up to [Pinecone](https://www.pinecone.io/) and get an API key.
 ## Using OpenAI 
 ```python
 from _openai.docindex import OpenaiPineconeIndexer
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key, and environment
+# Replace these values with your actual Pinecone API key, index name, OpenAI API key
 pinecone_api_key = "pinecone-api-key"
 index_name = "pinecone-index-name"
 openai_api_key = "openai-api-key"
-environment = "pinecone-index-environment"
 batch_limit = 20 # Batch limit for upserting documents
 chunk_size = 256 # Optional: size of texts per chunk. 
 
 # List of URLs of the documents to be indexed. (offline on your computer or online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.pdf"
 ]
 
 # Initialize the Pinecone indexer
-pinecone_index = OpenaiPineconeIndexer(index_name, pinecone_api_key, environment, openai_api_key)
+pinecone_index = OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key)
 
-# Index the documents with the specified URLs and batch limit
+# To create a new Index
+pinecone_index.create_index()
+
+# Store the document embeddings with the specified URLs and batch limit
 pinecone_index.index_documents(urls,batch_limit,chunk_size)
 ```
+```python
+# To delete the created Index
+pinecone_index.delete_index()
+```
 ## Initialize Vectorstore(using OpenAI)
 
 ```python
 from pinecone import Pinecone as IndexPinecone
 from langchain_community.vectorstores import Pinecone as VectorStorePinecone
 from langchain.embeddings.openai import OpenAIEmbeddings
 
@@ -62,47 +92,49 @@
         
 # Initialize OpenAI embeddings if you're using OpenAI embeddings
 embed = OpenAIEmbeddings(
         model = 'text-embedding-ada-002',
         openai_api_key = openai_api_key
         )
 
-# Define the text field
-text_field = "text"
-
 # Initialize the Vectorstore with the Pinecone index and OpenAI embeddings
-vectorstore = VectorStorePinecone(index, embed, text_field)
+vectorstore = VectorStorePinecone(index, embed, "text")
 ```
 
 
 ## Using Google Generative AI  
 
 ```python
 from _google.docindex import GooglePineconeIndexer
 
-# Replace these values with your actual Pinecone API key, index name, OpenAI API key, and environment
+# Replace these values with your actual Pinecone API key, index name, Google API key
 pinecone_api_key = "pinecone-api-key"
 index_name = "pinecone-index-name"
 google_api_key = "google-api-key"
-environment = "pinecone-index-environment"
 batch_limit = 20 # Batch limit for upserting documents
 chunk_size = 256 # Optional: size of texts per chunk. 
 
 # List of URLs of the documents to be indexed. (offline on your computer or an online)
 urls = [
  "your-document-1.pdf",
  "your-document-2.pdf"
 ]
 
-# Initialize the Pinecone indexer
-pinecone_index = GooglePineconeIndexer(index_name, pinecone_api_key, environment, google_api_key)
+pinecone_index = GooglePineconeIndexer(index_name, pinecone_api_key, google_api_key)
 
-# Index the documents with the specified URLs and batch limit
+# To create a new Index
+pinecone_index.create_index()
+
+# Store the document embeddings with the specified URLs and batch limit
 pinecone_index.index_documents(urls,batch_limit,chunk_size)
 ```
+```python
+# To delete the created Index
+pinecone_index.delete_index()
+```
 
 
 ## Initialize Vectorstore(using Google Generative AI)
 
 ```python
 from pinecone import Pinecone as IndexPinecone
 from langchain_community.vectorstores import Pinecone as VectorStorePinecone
@@ -114,19 +146,16 @@
         
 # Initialize embeddings 
 embed = GoogleGenerativeAIEmbeddings(
         model="models/embedding-001", 
         google_api_key=google_api_key
         )
 
-# Define the text field
-text_field = "text"
-
 # Initialize the Vectorstore with the Pinecone index and OpenAI embeddings
-vectorstore = VectorStorePinecone(index, embed, text_field)
+vectorstore = VectorStorePinecone(index, embed, "text")
 ```
 
 
 
 
 ## Using the CLI
 
@@ -151,24 +180,46 @@
 pip install -r requirements.txt
 ```
 
 - Navigate to src 
 ```bash
 cd src
 ```
+- To create an index
+
+```bash
+# Using OpenAI 
+python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+```
+
+```bash
+# Using Google Generative AI
+python -m  _google.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
+```
 
 - Run the command to start indexing the documents
 
 ```bash
 # Using OpenAI 
-python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --environment "your_environment" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+python -m _openai.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
 ```
 ```bash
 # Using Google Generative AI 
-python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --environment "your_environment" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+python -m _google.doc_index  --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key" --batch_limit 10 --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size 256 
+```
+- To delete an index
+
+```bash
+# Using OpenAI 
+python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --openai_api_key "your_openai_api_key"
+```
+
+```bash
+# Using Google Generative AI
+python -m  _google.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --google_api_key "your_google_api_key"
 ```
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
 
@@ -176,8 +227,8 @@
 
 We look forward to your contributions!
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for details.
 
 ## Contact
-For any enquiries, please reach out to me through keviinkibe@gmail.com
+For any enquiries, please reach out to me through keviinkibe@gmail.com
```

#### html2text {}

```diff
@@ -1,81 +1,102 @@
-       ************ DDooccIInnddeexx:: FFaasstt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
-_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]*Efficiently store multiple document embeddings and their
-  metadata, whether they're offline or online, in a Pinecone Vector Database
- optimized for Retrieval Augmented Generation (RAG) models Fast* ## Features -
- â¡ï¸ **Rapid Indexing**: Quickly index multiple documents along with their
-   metadata, including source, page details, and content, into Pinecone DB.
+Metadata-Version: 2.1 Name: docindex Version: 0.2.0 Summary: A package for fast
+indexing of multiple documents and their metadata on Pinecone. Home-page:
+https://github.com/KevKibe/docindex Author: Kevin Kibe Author-email:
+keviinkibe@gmail.com License: MIT Requires-Python: >=3.8 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: pinecone-client==3.2.2
+Requires-Dist: tiktoken==0.6.0 Requires-Dist: pypdf==4.1.0 Requires-Dist:
+unstructured==0.12.6 Requires-Dist: langchain-community==0.0.31 Requires-Dist:
+langchain==0.1.14 Requires-Dist: langchain-openai==0.1.1 Requires-Dist:
+langchain-google-genai==1.0.1
+  ************ DDooccIInnddeexx:: FFaasstt PPeerrssiisstteenntt DDooccuummeenntt EEmmbbeeddddiinnggss SSttoorraaggee ffoorr RRAAGG ************
+                            _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
+![Diagram](image.png) *Efficiently store multiple document embeddings and their
+ metadata, whether they're offline or online, in a persistent Pinecone Vector
+  Database optimized for Retrieval Augmented Generation (RAG) models Fast* ##
+ Features - â¡ï¸ **Rapid Indexing**: Quickly index multiple documents along
+with their metadata, including source, page details, and content, into Pinecone
+                                      DB.
   - ð **Document Flexibility**: Index documents from your local storage or
                            online sources with ease.
     - ð **Format Support**: Seamlessly handle various document formats,
                    including PDF, docx(in-development), etc.
 - ð **Embedding Services Integration**: Enjoy support for multiple embedding
 services such as OpenAI Embeddings, Google Generative AI Embeddings and more in
                                  development.
  - ð ï¸ **Configurable Vectorstore**: Configure a vectorstore directly from
   the index to facilitate RAG pipelines effortlessly. ## Setup ```python pip
-    install docindex ``` ## Getting Started ## Using OpenAI ```python from
+   install docindex ``` ## Getting Started - Sign up to [Pinecone](https://
+     www.pinecone.io/) and get an API key. ## Using OpenAI ```python from
 _openai.docindex import OpenaiPineconeIndexer # Replace these values with your
-     actual Pinecone API key, index name, OpenAI API key, and environment
-   pinecone_api_key = "pinecone-api-key" index_name = "pinecone-index-name"
- openai_api_key = "openai-api-key" environment = "pinecone-index-environment"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
+    actual Pinecone API key, index name, OpenAI API key pinecone_api_key =
+"pinecone-api-key" index_name = "pinecone-index-name" openai_api_key = "openai-
+ api-key" batch_limit = 20 # Batch limit for upserting documents chunk_size =
+256 # Optional: size of texts per chunk. # List of URLs of the documents to be
  indexed. (offline on your computer or online) urls = [ "your-document-1.pdf",
   "your-document-2.pdf" ] # Initialize the Pinecone indexer pinecone_index =
-       OpenaiPineconeIndexer(index_name, pinecone_api_key, environment,
- openai_api_key) # Index the documents with the specified URLs and batch limit
- pinecone_index.index_documents(urls,batch_limit,chunk_size) ``` ## Initialize
-     Vectorstore(using OpenAI) ```python from pinecone import Pinecone as
-    IndexPinecone from langchain_community.vectorstores import Pinecone as
-VectorStorePinecone from langchain.embeddings.openai import OpenAIEmbeddings #
-            Initialize the Pinecone index index_pc = IndexPinecone
-  (api_key=pinecone_api_key) index = index_pc.Index(index_name) # Initialize
- OpenAI embeddings if you're using OpenAI embeddings embed = OpenAIEmbeddings
-( model = 'text-embedding-ada-002', openai_api_key = openai_api_key ) # Define
-   the text field text_field = "text" # Initialize the Vectorstore with the
- Pinecone index and OpenAI embeddings vectorstore = VectorStorePinecone(index,
-      embed, text_field) ``` ## Using Google Generative AI ```python from
-_google.docindex import GooglePineconeIndexer # Replace these values with your
-     actual Pinecone API key, index name, OpenAI API key, and environment
-   pinecone_api_key = "pinecone-api-key" index_name = "pinecone-index-name"
- google_api_key = "google-api-key" environment = "pinecone-index-environment"
-   batch_limit = 20 # Batch limit for upserting documents chunk_size = 256 #
-   Optional: size of texts per chunk. # List of URLs of the documents to be
-   indexed. (offline on your computer or an online) urls = [ "your-document-
-       1.pdf", "your-document-2.pdf" ] # Initialize the Pinecone indexer
+OpenaiPineconeIndexer(index_name, pinecone_api_key, openai_api_key) # To create
+a new Index pinecone_index.create_index() # Store the document embeddings with
+       the specified URLs and batch limit pinecone_index.index_documents
+   (urls,batch_limit,chunk_size) ``` ```python # To delete the created Index
+   pinecone_index.delete_index() ``` ## Initialize Vectorstore(using OpenAI)
+         ```python from pinecone import Pinecone as IndexPinecone from
+ langchain_community.vectorstores import Pinecone as VectorStorePinecone from
+ langchain.embeddings.openai import OpenAIEmbeddings # Initialize the Pinecone
+index index_pc = IndexPinecone(api_key=pinecone_api_key) index = index_pc.Index
+ (index_name) # Initialize OpenAI embeddings if you're using OpenAI embeddings
+ embed = OpenAIEmbeddings( model = 'text-embedding-ada-002', openai_api_key =
+   openai_api_key ) # Initialize the Vectorstore with the Pinecone index and
+ OpenAI embeddings vectorstore = VectorStorePinecone(index, embed, "text") ```
+     ## Using Google Generative AI ```python from _google.docindex import
+GooglePineconeIndexer # Replace these values with your actual Pinecone API key,
+ index name, Google API key pinecone_api_key = "pinecone-api-key" index_name =
+  "pinecone-index-name" google_api_key = "google-api-key" batch_limit = 20 #
+Batch limit for upserting documents chunk_size = 256 # Optional: size of texts
+  per chunk. # List of URLs of the documents to be indexed. (offline on your
+computer or an online) urls = [ "your-document-1.pdf", "your-document-2.pdf" ]
      pinecone_index = GooglePineconeIndexer(index_name, pinecone_api_key,
-environment, google_api_key) # Index the documents with the specified URLs and
-batch limit pinecone_index.index_documents(urls,batch_limit,chunk_size) ``` ##
-  Initialize Vectorstore(using Google Generative AI) ```python from pinecone
- import Pinecone as IndexPinecone from langchain_community.vectorstores import
-      Pinecone as VectorStorePinecone from langchain_google_genai import
+ google_api_key) # To create a new Index pinecone_index.create_index() # Store
+        the document embeddings with the specified URLs and batch limit
+pinecone_index.index_documents(urls,batch_limit,chunk_size) ``` ```python # To
+   delete the created Index pinecone_index.delete_index() ``` ## Initialize
+Vectorstore(using Google Generative AI) ```python from pinecone import Pinecone
+   as IndexPinecone from langchain_community.vectorstores import Pinecone as
+            VectorStorePinecone from langchain_google_genai import
     GoogleGenerativeAIEmbeddings # Initialize the Pinecone index index_pc =
  IndexPinecone(api_key=pinecone_api_key) index = index_pc.Index(index_name) #
   Initialize embeddings embed = GoogleGenerativeAIEmbeddings( model="models/
-    embedding-001", google_api_key=google_api_key ) # Define the text field
- text_field = "text" # Initialize the Vectorstore with the Pinecone index and
- OpenAI embeddings vectorstore = VectorStorePinecone(index, embed, text_field)
-``` ## Using the CLI - Clone the Repository: Clone or download the application
-   code to your local machine. ```bash git clone https://github.com/KevKibe/
- docindex.git ``` - Create a virtual environment for the project and activate
-   it. ```bash # Navigate to project repository cd docindex # create virtual
-environment python -m venv venv # activate virtual environment source venv/bin/
-activate ``` - Install dependencies by running this command ```bash pip install
--r requirements.txt ``` - Navigate to src ```bash cd src ``` - Run the command
-        to start indexing the documents ```bash # Using OpenAI python -
+ embedding-001", google_api_key=google_api_key ) # Initialize the Vectorstore
+with the Pinecone index and OpenAI embeddings vectorstore = VectorStorePinecone
+ (index, embed, "text") ``` ## Using the CLI - Clone the Repository: Clone or
+download the application code to your local machine. ```bash git clone https://
+  github.com/KevKibe/docindex.git ``` - Create a virtual environment for the
+project and activate it. ```bash # Navigate to project repository cd docindex #
+ create virtual environment python -m venv venv # activate virtual environment
+  source venv/bin/activate ``` - Install dependencies by running this command
+ ```bash pip install -r requirements.txt ``` - Navigate to src ```bash cd src
+``` - To create an index ```bash # Using OpenAI python -m _openai.create_index
+ --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
+ openai_api_key "your_openai_api_key" ``` ```bash # Using Google Generative AI
+ python -m _google.create_index --pinecone_api_key "your_pinecone_api_key" --
+ index_name "your_index_name" --google_api_key "your_google_api_key" ``` - Run
+  the command to start indexing the documents ```bash # Using OpenAI python -
   m _openai.doc_index --pinecone_api_key "your_pinecone_api_key" --index_name
-    "your_index_name" --openai_api_key "your_openai_api_key" --environment
-"your_environment" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --chunk_size
-  256 ``` ```bash # Using Google Generative AI python -m _google.doc_index --
-  pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
-   google_api_key "your_google_api_key" --environment "your_environment" --
-     batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ##
-  Contributing Contributions are welcome and encouraged. Before contributing,
-     please take a moment to review our [Contribution Guidelines](https://
-  github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important
-   information on how to contribute to this project. If you're unsure about
-anything or need assistance, don't hesitate to reach out to us or open an issue
- to discuss your ideas. We look forward to your contributions! ## License This
-    project is licensed under the MIT License - see the [LICENSE](https://
- github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
-    For any enquiries, please reach out to me through keviinkibe@gmail.com
+ "your_index_name" --openai_api_key "your_openai_api_key" --batch_limit 10 --
+   docs "doc-1.pdf" "doc-2.pdf' --chunk_size 256 ``` ```bash # Using Google
+         Generative AI python -m _google.doc_index --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
+   "your_google_api_key" --batch_limit 10 --docs "doc-1.pdf" "doc-2.pdf' --
+    chunk_size 256 ``` - To delete an index ```bash # Using OpenAI python -
+m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
+ "your_index_name" --openai_api_key "your_openai_api_key" ``` ```bash # Using
+    Google Generative AI python -m _google.delete_index --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --google_api_key
+    "your_google_api_key" ``` ## Contributing Contributions are welcome and
+     encouraged. Before contributing, please take a moment to review our
+[Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
+    CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
+     details. ## Contact For any enquiries, please reach out to me through
+                             keviinkibe@gmail.com
```

### Comparing `docindex-0.1.0/setup.cfg` & `docindex-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = docindex
 author = Kevin Kibe
-version = 0.1.0
+version = 0.2.0
 author_email = keviinkibe@gmail.com
 description = A package for fast indexing of multiple documents and their metadata on Pinecone.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/docindex
 license = MIT
```

### Comparing `docindex-0.1.0/src/_google/doc_index.py` & `docindex-0.2.0/src/_google/doc_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Index documents on Pinecone using OpenAI embeddings.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--google_api_key", type=str, help="OpenAI API key")
-    parser.add_argument("--environment", type=str, help="Environment for Pinecone service")
     parser.add_argument("--batch_limit", type=int,  help="Maximum batch size for indexing")
     parser.add_argument("--docs", nargs="+", help="URLs of the documents to be indexed")
     parser.add_argument("--chunk_size", help="size of texts per chunk")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
-    pinecone_indexer = GooglePineconeIndexer(args.index_name, args.pinecone_api_key, args.environment, args.google_api_key)
+    pinecone_indexer = GooglePineconeIndexer(args.index_name, args.pinecone_api_key, args.google_api_key)
     pinecone_indexer.index_documents(args.docs, args.batch_limit, args.chunk_size)
```

### Comparing `docindex-0.1.0/src/_google/docindex.py` & `docindex-0.2.0/src/_google/docindex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,75 @@
-from pinecone import Pinecone
+from pinecone import Pinecone, PodSpec
 from tqdm.auto import tqdm
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_google_genai import GoogleGenerativeAIEmbeddings
 import tiktoken
 from typing import List
 from _openai.doc_model import Page
 
-
 class GooglePineconeIndexer:
     """
     Class for indexing documents to Pinecone using GoogleGenerativeAIEmbeddings embeddings.
     """
     def __init__(
         self,
         index_name: str,
         pinecone_api_key: str,
-        environment: str,
         google_api_key: str
     ) -> None:
         """
         Initialize the GoogleGenerativeAIEmbeddings object.
 
         Args:
             index_name (str): Name of the Pinecone index.
             pinecone_api_key (str): Pinecone API key.
             environment (str): Environment for Pinecone service.
             google_api_key (str): Google API key.
         """
-        self.pc = Pinecone(api_key=pinecone_api_key, environment=environment)
-        self.index = self.pc.Index(index_name)
+        self.pc = Pinecone(api_key=pinecone_api_key)
+        self.index_name = index_name
         self.google_api_key = google_api_key
         self.tokenizer = tiktoken.get_encoding('p50k_base')
 
+    def create_index(self, environment: str = "us-west1-gcp" ):
+        """
+        Creates an index with the specified parameters.
+
+        Args:
+            environment (str, optional): The environment where the index will be created. Defaults to "us-west1-gcp".
+
+        Returns:
+            None
+        """
+        print(f"Creating index {self.index_name}")
+        self.pc.create_index(
+            name=self.index_name,
+            dimension=1536,
+            metric="cosine",
+            spec=PodSpec(
+                environment=environment,
+                pod_type="p1.x1",
+                pods=1
+            )
+            )
+        return print(f"Index {self.index_name} created successfully!")
+    
+    def delete_index(self):
+        """
+        Deletes the created index.
 
+        Returns:
+            None
+        """
+        print(f"Deleting index {self.index_name}")
+        self.pc.delete_index(self.index_name)
+        return print(f"Index {self.index_name} deleted successfully!")
+    
     def load_pdf(self, pdf_url) -> List:
         """
         Load and split a PDF document into pages.
 
         Args:
             pdf_url (str): URL of the PDF document.
 
@@ -110,15 +141,16 @@
                 "chunk": j, "text": text, **metadata
             } for j, text in enumerate(record_texts)]
             texts.extend(record_texts)
             metadatas.extend(record_metadatas)
             if len(texts) >= batch_limit:
                 ids = [str(uuid4()) for _ in range(len(texts))]
                 embeds = embed.embed_documents(texts)  
-                self.index.upsert(vectors=zip(ids, embeds, metadatas), async_req=True)
+                index = self.pc.Index(self.index_name)  
+                index.upsert(vectors=zip(ids, embeds, metadatas), async_req=True)
                 texts = []
                 metadatas = []
 
 
     def index_documents(self, urls: List[str], batch_limit: int, chunk_size: int = 256) -> None:
         """
         Process a list of URLs and upsert documents to a Pinecone index.
@@ -144,8 +176,10 @@
                 )
                 for page in pages
             ]
 
             print(f"Upserting {len(pages_data)} pages to the Pinecone index...")
             self.upsert_documents(pages_data, batch_limit, chunk_size)  
             print("Finished upserting documents for this URL.")
+        index = self.pc.Index(self.index_name)
+        index.describe_index_stats()
         print("Indexing complete.")
```

### Comparing `docindex-0.1.0/src/_openai/doc_index.py` & `docindex-0.2.0/src/_openai/doc_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 import argparse
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Index documents on Pinecone using OpenAI embeddings.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     parser.add_argument("--openai_api_key", type=str, help="OpenAI API key")
-    parser.add_argument("--environment", type=str, help="Environment for Pinecone service")
     parser.add_argument("--batch_limit", type=int,  help="Maximum batch size for indexing")
     parser.add_argument("--docs", nargs="+", help="URLs of the documents to be indexed")
     parser.add_argument("--chunk_size", help="size of texts per chunk")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
-    pinecone_indexer = OpenaiPineconeIndexer(args.index_name, args.pinecone_api_key, args.environment, args.openai_api_key)
+    pinecone_indexer = OpenaiPineconeIndexer(args.index_name, args.pinecone_api_key, args.openai_api_key)
     pinecone_indexer.index_documents(args.docs, args.batch_limit, args.chunk_size)
```

### Comparing `docindex-0.1.0/src/_openai/docindex.py` & `docindex-0.2.0/src/_openai/docindex.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,92 @@
-from pinecone import Pinecone
+from pinecone import Pinecone, PodSpec
 from tqdm.auto import tqdm
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_openai import OpenAIEmbeddings
 import tiktoken
 from typing import List
 from .doc_model import Page
 
-
 class OpenaiPineconeIndexer:
     """
     Class for indexing documents to Pinecone using OpenAI embeddings.
     """
     def __init__(
         self,
         index_name: str,
         pinecone_api_key: str,
-        environment: str,
         openai_api_key: str
     ) -> None:
         """
         Initialize the OpenAIPineconeIndexer object.
 
         Args:
             index_name (str): Name of the Pinecone index.
             pinecone_api_key (str): Pinecone API key.
             environment (str): Environment for Pinecone service.
             openai_api_key (str): OpenAI API key.
         """
-        self.pc = Pinecone(api_key=pinecone_api_key, environment=environment)
-        self.index = self.pc.Index(index_name)
+        self.pc = Pinecone(api_key=pinecone_api_key)
+        self.index_name = index_name
         self.openai_api_key = openai_api_key
         self.tokenizer = tiktoken.get_encoding('p50k_base')
 
+    def create_index(self, environment: str = "us-west1-gcp" ):
+        """
+        Creates an index with the specified parameters.
+
+        Args:
+            environment (str, optional): The environment where the index will be created. Defaults to "us-west1-gcp".
+
+        Returns:
+            None
+        """
+        print(f"Creating index {self.index_name}")
+        self.pc.create_index(
+            name=self.index_name,
+            dimension=1536,
+            metric="cosine",
+            spec=PodSpec(
+                environment=environment,
+                pod_type="p1.x1",
+                pods=1
+            )
+            )
+        return print(f"Index {self.index_name} created successfully!")
+    
 
+    def delete_index(self):
+        """
+        Deletes the created index.
+
+        Returns:
+            None
+        """
+        print(f"Deleting index {self.index_name}")
+        self.pc.delete_index(self.index_name)
+        return print(f"Index {self.index_name} deleted successfully!")
+
+    
     def load_pdf(self, pdf_url) -> List:
         """
         Load and split a PDF document into pages.
 
         Args:
             pdf_url (str): URL of the PDF document.
 
         Returns:
             List: List of pages from the PDF document.
         """
         loader = PyPDFLoader(pdf_url)
         pages = loader.load_and_split()
         return pages
     
+    
     def tiktoken_len(self, text: str) -> int:
         """
         Calculate length of text in tokens.
 
         Parameters:
             text (str): Input text.
 
@@ -108,16 +142,17 @@
             record_metadatas = [{
                 "chunk": j, "text": text, **metadata
             } for j, text in enumerate(record_texts)]
             texts.extend(record_texts)
             metadatas.extend(record_metadatas)
             if len(texts) >= batch_limit:
                 ids = [str(uuid4()) for _ in range(len(texts))]
-                embeds = embed.embed_documents(texts)  
-                self.index.upsert(vectors=zip(ids, embeds, metadatas), async_req=True)
+                embeds = embed.embed_documents(texts)
+                index = self.pc.Index(self.index_name)  
+                index.upsert(vectors=zip(ids, embeds, metadatas), async_req=True)
                 texts = []
                 metadatas = []
 
 
     def index_documents(self, urls: List[str], batch_limit: int, chunk_size: int = 256) -> None:
         """
         Process a list of URLs and upsert documents to a Pinecone index.
@@ -143,8 +178,11 @@
                 )
                 for page in pages
             ]
 
             print(f"Upserting {len(pages_data)} pages to the Pinecone index...")
             self.upsert_documents(pages_data, batch_limit, chunk_size)  
             print("Finished upserting documents for this URL.")
+        index = self.pc.Index(self.index_name)
+        index.describe_index_stats()
         print("Indexing complete.")
+
```

