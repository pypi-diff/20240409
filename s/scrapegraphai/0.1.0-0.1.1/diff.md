# Comparing `tmp/scrapegraphai-0.1.0.tar.gz` & `tmp/scrapegraphai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.1.0.tar", max compression
+gzip compressed data, was "scrapegraphai-0.1.1.tar", max compression
```

## Comparing `scrapegraphai-0.1.0.tar` & `scrapegraphai-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.0/LICENSE
--rw-r--r--   0        0        0     5590 2024-04-06 12:43:33.708461 scrapegraphai-0.1.0/README.md
--rw-r--r--   0        0        0     1621 2024-04-08 16:14:52.864798 scrapegraphai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.0/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.0/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.0/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.0/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     2887 2024-04-08 16:13:44.450904 scrapegraphai-0.1.0/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     3041 2024-03-18 13:23:07.402624 scrapegraphai-0.1.0/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2160 2024-04-08 16:13:44.451088 scrapegraphai-0.1.0/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2300 2024-04-08 16:13:44.451433 scrapegraphai-0.1.0/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3024 2024-04-08 16:13:44.451625 scrapegraphai-0.1.0/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.0/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      607 2024-04-08 16:13:44.452326 scrapegraphai-0.1.0/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3793 2024-04-08 16:13:44.452862 scrapegraphai-0.1.0/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-03-03 14:00:51.197887 scrapegraphai-0.1.0/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      252 2024-04-08 16:13:44.453206 scrapegraphai-0.1.0/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      600 2024-04-08 16:13:44.453638 scrapegraphai-0.1.0/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-06 12:44:56.957059 scrapegraphai-0.1.0/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      590 2024-04-08 16:13:44.454004 scrapegraphai-0.1.0/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-03-03 14:00:51.198085 scrapegraphai-0.1.0/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-03-18 13:23:25.826441 scrapegraphai-0.1.0/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-03-24 19:34:24.967643 scrapegraphai-0.1.0/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.0/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 16:13:44.454956 scrapegraphai-0.1.0/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.0/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3225 2024-04-08 16:13:44.455216 scrapegraphai-0.1.0/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5602 2024-04-08 16:13:44.455773 scrapegraphai-0.1.0/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.0/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.0/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-08 16:13:44.456540 scrapegraphai-0.1.0/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4691 2024-04-08 16:13:44.456936 scrapegraphai-0.1.0/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     4525 2024-04-08 16:13:44.457372 scrapegraphai-0.1.0/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-08 16:13:44.457753 scrapegraphai-0.1.0/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.1.0/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.0/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.0/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.0/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.0/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.0/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     7177 1970-01-01 00:00:00.000000 scrapegraphai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6321 2024-04-09 09:44:17.063929 scrapegraphai-0.1.1/README.md
+-rw-r--r--   0        0        0     1621 2024-04-09 09:44:31.922633 scrapegraphai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3010 2024-04-09 09:44:17.065498 scrapegraphai-0.1.1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     3041 2024-04-08 20:24:28.569893 scrapegraphai-0.1.1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2160 2024-04-09 09:44:17.065954 scrapegraphai-0.1.1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2264 2024-04-09 08:20:31.578158 scrapegraphai-0.1.1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3000 2024-04-09 09:44:17.066614 scrapegraphai-0.1.1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      700 2024-04-09 09:44:17.066995 scrapegraphai-0.1.1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3793 2024-04-09 09:44:17.067324 scrapegraphai-0.1.1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.1.1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      252 2024-04-08 16:13:44.453206 scrapegraphai-0.1.1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-09 09:44:17.067663 scrapegraphai-0.1.1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.1.1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.1.1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.1.1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.1.1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.1.1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.1.1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3209 2024-04-09 09:44:17.067983 scrapegraphai-0.1.1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5602 2024-04-08 16:13:44.455773 scrapegraphai-0.1.1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-08 20:26:19.442517 scrapegraphai-0.1.1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4701 2024-04-09 09:44:17.068360 scrapegraphai-0.1.1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4521 2024-04-09 08:22:49.561048 scrapegraphai-0.1.1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-08 20:27:04.824493 scrapegraphai-0.1.1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.1.1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 scrapegraphai-0.1.1/PKG-INFO
```

### Comparing `scrapegraphai-0.1.0/LICENSE` & `scrapegraphai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/README.md` & `scrapegraphai-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -39,21 +39,27 @@
 
 The documentation for ScrapeGraphAI can be found [here](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 Check out also the docusaurus [documentation](https://scrapegraph-doc.onrender.com/).
 
 ## 💻 Usage
 
-### Case 1: Extracting information using a prompt
+### Case 1: Extracting informations using a local LLM 
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 ```python
+
+```
+
+
+### Case 2: Extracting informations using Openai model
+```python
 from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
         "api_key": OPENAI_API_KEY,
@@ -68,15 +74,39 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-The output will be a dictionary with the extracted information, for example:
+### Case 3: Extracting informations using Gemini 
+```python
+from scrapegraphai.graphs import SmartScraperGraph
+GOOGLE_APIKEY = "YOUR_API_KEY"
+
+# Define the configuration for the graph
+graph_config = {
+    "llm": {
+        "api_key": GOOGLE_APIKEY,
+        "model": "gemini-pro",
+    },
+}
+
+# Create the SmartScraperGraph instance
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the quotes, authors and tags ",
+    file_source="http://quotes.toscrape.com",  # also accepts a string with the already downloaded HTML code as string format
+    config=graph_config
+)
+
+result = smart_scraper_graph.run()
+print(result)
+```
+
+The output for alle 3 the cases will be a dictionary with the extracted information, for example:
 
 ```bash
 {
     'titles': [
         'Rotary Pendulum RL'
         ],
     'descriptions': [
```

### Comparing `scrapegraphai-0.1.0/pyproject.toml` & `scrapegraphai-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.1.0"
+version = "0.1.1"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.1.1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.1.1/scrapegraphai/graphs/abstract_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Module having abstract class for creating all the graphs
 """
 from abc import ABC, abstractmethod
 from typing import Optional
 from ..models import OpenAI, Gemini, Ollama, AzureOpenAI
 from ..helpers import models_tokens
 
+
 class AbstractGraph(ABC):
     """
     Abstract class representing a generic graph-based tool.
     """
 
     def __init__(self, prompt: str, config: dict, source: Optional[str] = None):
         """
         Initializes the AbstractGraph with a prompt, file source, and configuration.
         """
         self.prompt = prompt
         self.source = source
         self.config = config
         self.llm_model = self._create_llm(config["llm"])
-        self.embedder_model = None if "embeddings" not in config else self._create_llm(config["embeddings"])
+        self.embedder_model = None if "embeddings" not in config else self._create_llm(
+            config["embeddings"])
         self.graph = self._create_graph()
 
     def _create_llm(self, llm_config: dict):
         """
         Creates an instance of the language model (OpenAI or Gemini) based on configuration.
         """
         llm_defaults = {
@@ -35,40 +37,47 @@
         # Instantiate the language model based on the model name
         if "gpt-" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["openai"][llm_params["model"]]
             except KeyError:
                 raise ValueError("Model not supported")
             return OpenAI(llm_params)
-        
+
         elif "azure" in llm_params["model"]:
             # take the model after the last dash
             llm_params["model"] = llm_params["model"].split("/")[-1]
             try:
                 self.model_token = models_tokens["openai"][llm_params["model"]]
             except KeyError:
                 raise ValueError("Model not supported")
             return AzureOpenAI(llm_params)
-        
+
         elif "gemini" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["gemini"][llm_params["model"]]
             except KeyError:
                 raise ValueError("Model not supported")
             return Gemini(llm_params)
-        
+
         elif "ollama" in llm_params["model"]:
-            # take the model after the last dash
+            """ 
+            Avaiable models:
+            - llama2
+            - mistral
+            - codellama
+            - dolphin-mixtral
+            - mistral-openorca
+            """
             llm_params["model"] = llm_params["model"].split("/")[-1]
             try:
                 self.model_token = models_tokens["ollama"][llm_params["model"]]
             except KeyError:
                 raise ValueError("Model not supported")
             return Ollama(llm_params)
-        
+
         else:
             raise ValueError("Model not supported")
 
     @abstractmethod
     def _create_graph(self):
         """
         Abstract method to create a graph representation.
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.1.1/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.1.1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.1.1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """ 
 Module for creating the smart scraper
 """
-from ..models import OpenAI, Gemini
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.1.1/scrapegraphai/graphs/speech_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ 
 Module for converting text to speach
 """
 from scrapegraphai.utils.save_audio_from_bytes import save_audio_from_bytes
-from ..models import OpenAI, Gemini, OpenAITextToSpeech
+from ..models import OpenAITextToSpeech
 from .base_graph import BaseGraph
 from ..nodes import (
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode,
     TextToSpeechNode,
@@ -23,15 +23,15 @@
     def __init__(self, prompt: str, source: str, config: dict):
         """
         Initializes the SmartScraperGraph with a prompt, source, and configuration.
         """
         super().__init__(prompt, config, source)
 
         self.input_key = "url" if source.startswith("http") else "local_dir"
-        
+
     def _create_graph(self):
         """
         Creates the graph of nodes representing the workflow for web scraping and summarization.
         """
         fetch_node = FetchNode(
             input="url | local_dir",
             output=["doc"],
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.1.1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.1.1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.1.1/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/models/gemini.py` & `scrapegraphai-0.1.1/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/models/ollama.py` & `scrapegraphai-0.1.1/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/models/openai.py` & `scrapegraphai-0.1.1/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.1.1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.1.1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/fetch_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
         # Interpret input keys based on the provided input expression
         input_keys = self.get_input_keys(state)
 
         # Fetching data from the state based on the input keys
         input_data = [state[key] for key in input_keys]
 
-        source = input_data[0]        
-        
+        source = input_data[0]
+
         # if it is a local directory
         if not source.startswith("http"):
             document = [Document(page_content=source, metadata={
                 "source": "local_dir"
             })]
 
         # if it is a URL
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/rag_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from typing import List
 from langchain.docstore.document import Document
 from langchain.retrievers import ContextualCompressionRetriever
 from langchain.retrievers.document_compressors import EmbeddingsFilter, DocumentCompressorPipeline
 from langchain_community.document_transformers import EmbeddingsRedundantFilter
 from langchain_community.vectorstores import FAISS
-from ..models import OpenAI, Gemini, Ollama, AzureOpenAI
 from langchain_openai import OpenAIEmbeddings, AzureOpenAIEmbeddings
+from ..models import OpenAI, Ollama, AzureOpenAI
 from langchain_community.embeddings import OllamaEmbeddings
 from .base_node import BaseNode
 
 
 class RAGNode(BaseNode):
     """
     A node responsible for compressing the input tokens and storing the document
@@ -82,24 +82,26 @@
 
         print("--- (updated chunks metadata) ---")
 
         # check if embedder_model is provided, if not use llm_model
         embedding_model = self.embedder_model if self.embedder_model else self.llm_model
 
         if isinstance(embedding_model, OpenAI):
-            embeddings = OpenAIEmbeddings(api_key=embedding_model.openai_api_key)
+            embeddings = OpenAIEmbeddings(
+                api_key=embedding_model.openai_api_key)
         elif isinstance(embedding_model, AzureOpenAI):
             embeddings = AzureOpenAIEmbeddings()
         elif isinstance(embedding_model, Ollama):
             embeddings = OllamaEmbeddings()
         else:
             raise ValueError("Embedding Model missing or not supported")
-        
-        retriever = FAISS.from_documents(chunked_docs, embeddings).as_retriever()
-    
+
+        retriever = FAISS.from_documents(
+            chunked_docs, embeddings).as_retriever()
+
         redundant_filter = EmbeddingsRedundantFilter(embeddings=embeddings)
         # similarity_threshold could be set, now k=20
         relevant_filter = EmbeddingsFilter(embeddings=embeddings)
         pipeline_compressor = DocumentCompressorPipeline(
             transformers=[redundant_filter, relevant_filter]
         )
         # redundant + relevant filter compressor
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/search_internet_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             template=search_template,
             input_variables=["user_prompt"],
         )
 
         # Execute the chain to get the search query
         search_answer = search_prompt | self.llm_model | output_parser
         search_query = search_answer.invoke({"user_prompt": user_prompt})[0]
-    
+
         print(f"Search Query: {search_query}")
         # TODO: handle multiple URLs
         answer = search_on_web(query=search_query, max_results=1)[0]
 
         # Update the state with the generated answer
         state.update({self.output[0]: answer})
         return state
```

### Comparing `scrapegraphai-0.1.0/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.1.1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/remover.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.1.1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.0/PKG-INFO` & `scrapegraphai-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
@@ -73,21 +73,27 @@
 
 The documentation for ScrapeGraphAI can be found [here](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 Check out also the docusaurus [documentation](https://scrapegraph-doc.onrender.com/).
 
 ## 💻 Usage
 
-### Case 1: Extracting information using a prompt
+### Case 1: Extracting informations using a local LLM 
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 ```python
+
+```
+
+
+### Case 2: Extracting informations using Openai model
+```python
 from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
         "api_key": OPENAI_API_KEY,
@@ -102,15 +108,39 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-The output will be a dictionary with the extracted information, for example:
+### Case 3: Extracting informations using Gemini 
+```python
+from scrapegraphai.graphs import SmartScraperGraph
+GOOGLE_APIKEY = "YOUR_API_KEY"
+
+# Define the configuration for the graph
+graph_config = {
+    "llm": {
+        "api_key": GOOGLE_APIKEY,
+        "model": "gemini-pro",
+    },
+}
+
+# Create the SmartScraperGraph instance
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the quotes, authors and tags ",
+    file_source="http://quotes.toscrape.com",  # also accepts a string with the already downloaded HTML code as string format
+    config=graph_config
+)
+
+result = smart_scraper_graph.run()
+print(result)
+```
+
+The output for alle 3 the cases will be a dictionary with the extracted information, for example:
 
 ```bash
 {
     'titles': [
         'Rotary Pendulum RL'
         ],
     'descriptions': [
```

