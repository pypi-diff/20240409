# Comparing `tmp/basicbedrock-0.0.1.tar.gz` & `tmp/basicbedrock-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.0.1.tar", last modified: Fri Apr  5 21:36:20 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.0.tar", last modified: Tue Apr  9 15:23:28 2024, max compression
```

## Comparing `basicbedrock-0.0.1.tar` & `basicbedrock-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-05 21:36:20.130298 basicbedrock-0.0.1/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1061 2024-04-05 19:47:51.000000 basicbedrock-0.0.1/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     2853 2024-04-05 21:36:20.130022 basicbedrock-0.0.1/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      936 2024-04-05 21:11:18.000000 basicbedrock-0.0.1/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      818 2024-04-05 21:35:54.000000 basicbedrock-0.0.1/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-05 21:36:20.130358 basicbedrock-0.0.1/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-05 21:36:20.126377 basicbedrock-0.0.1/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-05 21:36:20.127218 basicbedrock-0.0.1/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      115 2024-04-05 20:00:27.000000 basicbedrock-0.0.1/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     6643 2024-04-05 20:55:35.000000 basicbedrock-0.0.1/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-05 21:36:20.128872 basicbedrock-0.0.1/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     2629 2024-04-05 21:04:16.000000 basicbedrock-0.0.1/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2020 2024-04-05 20:44:06.000000 basicbedrock-0.0.1/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3947 2024-04-05 20:37:14.000000 basicbedrock-0.0.1/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     1965 2024-04-05 20:57:47.000000 basicbedrock-0.0.1/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2402 2024-04-05 20:49:21.000000 basicbedrock-0.0.1/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     1320 2024-04-05 20:44:06.000000 basicbedrock-0.0.1/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2149 2024-04-05 20:49:21.000000 basicbedrock-0.0.1/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-05 21:36:20.129586 basicbedrock-0.0.1/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     2853 2024-04-05 21:36:20.000000 basicbedrock-0.0.1/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      554 2024-04-05 21:36:20.000000 basicbedrock-0.0.1/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-05 21:36:20.000000 basicbedrock-0.0.1/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-05 21:36:20.000000 basicbedrock-0.0.1/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-05 21:36:20.000000 basicbedrock-0.0.1/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-05 21:36:20.129021 basicbedrock-0.0.1/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3223 2024-04-05 21:01:42.000000 basicbedrock-0.0.1/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.613340 basicbedrock-0.1.0/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.0/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2899 2024-04-09 15:23:28.613119 basicbedrock-0.1.0/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1002 2024-04-09 15:09:01.000000 basicbedrock-0.1.0/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-09 15:21:30.000000 basicbedrock-0.1.0/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-09 15:23:28.613391 basicbedrock-0.1.0/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.605822 basicbedrock-0.1.0/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.607010 basicbedrock-0.1.0/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-09 15:11:23.000000 basicbedrock-0.1.0/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    13220 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.611953 basicbedrock-0.1.0/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2782 2024-04-09 15:10:38.000000 basicbedrock-0.1.0/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4880 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     6477 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4804 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4379 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3020 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2589 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.612845 basicbedrock-0.1.0/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2899 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      554 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.612316 basicbedrock-0.1.0/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3684 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/test/tests.py
```

### Comparing `basicbedrock-0.0.1/LICENSE` & `basicbedrock-0.1.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 David Mattson
+Copyright 2024 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `basicbedrock-0.0.1/PKG-INFO` & `basicbedrock-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.0.1
+Version: 0.1.0
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
-Author-email: David Mattson <mattsod@kaizencyber.io>
-Maintainer-email: David Mattson <mattsod@kaizencyber.io>
-License: Copyright 2024 David Mattson
+Author-email: cyberitech <mattsod@kaizencyber.io>
+Maintainer-email: cyberitech <mattsod@kaizencyber.io>
+License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/cyberitech/BasicBedrock
 Project-URL: Issues, https://github.com/cyberitech/BasicBedrock/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,16 +26,21 @@
 Requires-Dist: pydantic>=2.6.4
 
 # BasicBedrock
 AWS Bedrock provides a variety of foundational models to AWS customers.  Each model family requires their own request structure, yet the underlying semantics are roughly common; there is always a field for the textual input prompt, and often there are fields to define maximum desired output, stop words, P, K and Temperature values.
 
 This package aims to abstract away all of that.  Currently, it only abstracts the input prompt and the answer text, but I plan to also inlcude abstraction layers for the other parameters as well.
 
+## Installation
+```bash
+pip install basicbedrock
+```
+
 ## Usage
-Rather simple to use.  See `example/simple.py` for some usage.
+Rather simple to use.  See [examples](./examples) for some usage examples.
 
 ```python
 import boto3
 from basicbedrock import BasicBedrock
 
 session = boto3.session.Session(profile_name="default",region_name="us-west-2")
 bb = BasicBedrock(session=session)
```

### Comparing `basicbedrock-0.0.1/README.md` & `basicbedrock-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # BasicBedrock
 AWS Bedrock provides a variety of foundational models to AWS customers.  Each model family requires their own request structure, yet the underlying semantics are roughly common; there is always a field for the textual input prompt, and often there are fields to define maximum desired output, stop words, P, K and Temperature values.
 
 This package aims to abstract away all of that.  Currently, it only abstracts the input prompt and the answer text, but I plan to also inlcude abstraction layers for the other parameters as well.
 
+## Installation
+```bash
+pip install basicbedrock
+```
+
 ## Usage
-Rather simple to use.  See `example/simple.py` for some usage.
+Rather simple to use.  See [examples](./examples) for some usage examples.
 
 ```python
 import boto3
 from basicbedrock import BasicBedrock
 
 session = boto3.session.Session(profile_name="default",region_name="us-west-2")
 bb = BasicBedrock(session=session)
```

### Comparing `basicbedrock-0.0.1/pyproject.toml` & `basicbedrock-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "basicbedrock"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
-  { name="David Mattson", email="mattsod@kaizencyber.io" },
+  { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
-    { name="David Mattson", email="mattsod@kaizencyber.io" },
+    { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
     "boto3>=1.34.79",
```

### Comparing `basicbedrock-0.0.1/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.0/src/basicbedrock/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-import os, sys; sys.path.append(os.path.dirname(os.path.realpath(__file__)))
+"""
+This package contains all models used in basicbedrock.  It models and abstracts all the response/request schemas used by bedrock.
+"""
+import os
+import sys
+
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 from .amazon import *
 from .anthropic import *
 from .baseclasses import BaseAbstractRequest
 from .cohere import *
 from .meta import *
 from .mistral import *
 
@@ -12,36 +18,36 @@
     "amazon.titan-text-express-v1": AmazonTitanTextExpressV1Request,
     "anthropic.claude-instant-v1": AnthropicClaudeInstantV1Request,
     "anthropic.claude-v2": AnthropicClaudeV2Request,
     "anthropic.claude-v2:1": AnthropicClaudeV2_1Request,
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3Sonnet20240229V1_0Request,
     "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3Haiku20240307V1_0Request,
     "cohere.command-text-v14": CohereCommandTextV14Request,
-    "cohere.command-light-text-v14":CohereCommandLightTextV14Request,
-    "cohere.embed-english-v3":CohereEmbedEnglishV3Request,
-    "cohere.embed-multilingual-v3":CohereEmbedMultilingualV3Request,
+    "cohere.command-light-text-v14": CohereCommandLightTextV14Request,
+    "cohere.embed-english-v3": CohereEmbedEnglishV3Request,
+    "cohere.embed-multilingual-v3": CohereEmbedMultilingualV3Request,
     "meta.llama2-13b-chat-v1": MetaLlama213bChatV1Request,
     "meta.llama2-70b-chat-v1": MetaLlama270bChatV1Request,
     "mistral.mistral-7b-instruct-v0:2": MistralMistral7bInstructV0_2Request,
     "mistral.mixtral-8x7b-instruct-v0:1": MistralMistral8x7bInstructV0_1Request,
-    "mistral.mistral-large-2402-v1:0":MistralMistralLarge2402V1_0Request
+    "mistral.mistral-large-2402-v1:0": MistralMistralLarge2402V1_0Request
 }
 
 model_response_mapping = {
     "amazon.titan-embed-text-v1": AmazonTitanEmbedTextV1Response,
     "amazon.titan-text-lite-v1": AmazonTitanTextLiteV1Response,
     "amazon.titan-text-express-v1": AmazonTitanTextExpressV1Response,
     "anthropic.claude-instant-v1": AnthropicClaudeInstantV1Response,
     "anthropic.claude-v2": AnthropicClaudeV2Response,
     "anthropic.claude-v2:1": AnthropicClaudeV2_1Response,
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3Sonnet20240229V1_0Response,
     "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3Haiku20240307V1_0Response,
     "cohere.command-text-v14": CohereCommandTextV14Response,
-    "cohere.command-light-text-v14":CohereCommandLightTextV14Response,
-    "cohere.embed-english-v3":CohereEmbedEnglishV3Response,
-    "cohere.embed-multilingual-v3":CohereEmbedMultilingualV3Response,
+    "cohere.command-light-text-v14": CohereCommandLightTextV14Response,
+    "cohere.embed-english-v3": CohereEmbedEnglishV3Response,
+    "cohere.embed-multilingual-v3": CohereEmbedMultilingualV3Response,
     "meta.llama2-13b-chat-v1": MetaLlama213bChatV1Response,
     "meta.llama2-70b-chat-v1": MetaLlama270bChatV1Response,
     "mistral.mistral-7b-instruct-v0:2": MistralMistral7bInstructV0_2Response,
     "mistral.mixtral-8x7b-instruct-v0:1": MistralMistral8x7bInstructV0_1Response,
-    "mistral.mistral-large-2402-v1:0":MistralMistralLarge2402V1_0Response
-}
+    "mistral.mistral-large-2402-v1:0": MistralMistralLarge2402V1_0Response
+}
```

### Comparing `basicbedrock-0.0.1/src/basicbedrock/models/mistral.py` & `basicbedrock-0.1.0/src/basicbedrock/models/mistral.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,90 @@
-from typing import List,Optional
-from pydantic import BaseModel
+"""
+File containing all of the definitions and implementations for the Mistral family of requests and responses.
+"""
 from .baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
-"""
-Mistral 7b Instruct V0:2
-"""
-class MistralMistral7bInstructV0_2Request(BaseAbstractRequest):
+class MistralBaseRequest(BaseAbstractRequest):
+    """
+    Base request for Mistral family of models.
+    this mnodel supports temperature, top_p, top_k and max_tokens
+    """
     prompt: str = "<s>[INST] this is where you place your input text [/INST]"
     max_tokens: int = 250
     temperature: float = 0.5
     top_p: float = 0.5
-    top_k:int = 125
+    top_k: int = 125
 
-    def update_prompt(self,text):
+    def update_prompt(self, text):
         input_text = "<s>[INST] {PROMPT} [/INST]"
         input_text = input_text.format(PROMPT=text)
         self.update_prompt_raw(input_text)
 
-    def update_prompt_raw(self,text):
+    def update_prompt_raw(self, text):
         self.prompt = text
 
-class MistralMistral7bInstructV0_2Response(BaseAbstractResponse):
-    def get_answer(self)->str:
-        return self.result_raw['outputs'][0]['text']
+    def set_p(self, top_p: float):
+        self.top_p = top_p
 
+    def set_k(self, top_k: int):
+        self.top_k = top_k
 
-"""
-Mistral 8x7b Instruct V0:1
-"""
-class MistralMistral8x7bInstructV0_1Request(BaseAbstractRequest):
-    prompt: str = "<s>[INST] this is where you place your input text [/INST]"
-    max_tokens: int = 250
-    temperature: float = 0.5
-    top_p: float = 0.5
-    top_k:int = 125
+    def set_temp(self, temp: float):
+        self.temperature = temp
 
-    def update_prompt(self,text):
-        input_text = "<s>[INST] {PROMPT} [/INST]"
-        input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
+    def set_max_tokens(self, max_tokens: int):
+        self.max_tokens = max_tokens
 
-    def update_prompt_raw(self,text):
-        self.prompt = text
 
-class MistralMistral8x7bInstructV0_1Response(BaseAbstractResponse):
-    def get_answer(self)->str:
-        return self.result_raw['outputs'][0]['text']
+class MistralMistral7bInstructV0_2Request(MistralBaseRequest):
+    """
+    Request format for Mistral 7b Instruct V0:2
+    This model supports temperature, top_p, top_k and max_tokens
+    This class is implemented in MistralBaseRequest
+    """
 
 
-"""
-Mistral Large 2402 v1:0
-"""
-class MistralMistralLarge2402V1_0Request(BaseAbstractRequest):
-    prompt: str = "<s>[INST] this is where you place your input text [/INST]"
-    max_tokens: int = 250
-    temperature: float = 0.5
-    top_p: float = 0.5
-    top_k:int = 125
+class MistralMistral8x7bInstructV0_1Request(MistralBaseRequest):
+    """
+    Request format for Mistral 8x7b Instruct V0:1
+    This model supports temperature, top_p, top_k and max_tokens
+    This class is implemented in MistralBaseRequest
+    """
 
-    def update_prompt(self,text):
-        input_text = "<s>[INST] {PROMPT} [/INST]"
-        input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
 
-    def update_prompt_raw(self,text):
-        self.prompt = text
+class MistralMistralLarge2402V1_0Request(MistralBaseRequest):
+    """
+    Request format for Mistral Large 2402 V1:0
+    This model supports temperature, top_p, top_k and max_tokens
+    This class is implemented in MistralBaseRequest
+    """
+
+
+class MistralBaseResponse(BaseAbstractResponse):
+    """
+    Base response format for Mistral Instruct family of models.
+    """
+
+    def get_answer(self) -> str:
+        return self.result_raw['outputs'][0]['text']
+
 
-class MistralMistralLarge2402V1_0Response(BaseAbstractResponse):
-    def get_answer(self)->str:
-        return self.result_raw['outputs'][0]['text']
+class MistralMistral7bInstructV0_2Response(MistralBaseResponse):
+    """
+    Response format for Mistral 7b Instruct V0:2
+    This class is implemented in MistralBaseResponse
+    """
+
+
+class MistralMistral8x7bInstructV0_1Response(MistralBaseResponse):
+    """
+    Response format for Mistral 8x7b Instruct V0:2
+    This class is implemented in MistralBaseResponse
+    """
+
+
+class MistralMistralLarge2402V1_0Response(MistralBaseResponse):
+    """
+    Response format for Mistral Large 2402 v1:0
+    This class is implemented in MistralInstructBaseResponse
+    """
```

### Comparing `basicbedrock-0.0.1/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.1.0/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.0.1
+Version: 0.1.0
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
-Author-email: David Mattson <mattsod@kaizencyber.io>
-Maintainer-email: David Mattson <mattsod@kaizencyber.io>
-License: Copyright 2024 David Mattson
+Author-email: cyberitech <mattsod@kaizencyber.io>
+Maintainer-email: cyberitech <mattsod@kaizencyber.io>
+License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/cyberitech/BasicBedrock
 Project-URL: Issues, https://github.com/cyberitech/BasicBedrock/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,16 +26,21 @@
 Requires-Dist: pydantic>=2.6.4
 
 # BasicBedrock
 AWS Bedrock provides a variety of foundational models to AWS customers.  Each model family requires their own request structure, yet the underlying semantics are roughly common; there is always a field for the textual input prompt, and often there are fields to define maximum desired output, stop words, P, K and Temperature values.
 
 This package aims to abstract away all of that.  Currently, it only abstracts the input prompt and the answer text, but I plan to also inlcude abstraction layers for the other parameters as well.
 
+## Installation
+```bash
+pip install basicbedrock
+```
+
 ## Usage
-Rather simple to use.  See `example/simple.py` for some usage.
+Rather simple to use.  See [examples](./examples) for some usage examples.
 
 ```python
 import boto3
 from basicbedrock import BasicBedrock
 
 session = boto3.session.Session(profile_name="default",region_name="us-west-2")
 bb = BasicBedrock(session=session)
```

### Comparing `basicbedrock-0.0.1/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.0/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.0.1/test/tests.py` & `basicbedrock-0.1.0/test/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,73 +13,93 @@
     for model in all_models:
         print(f"now testing {model} in invoke with string")
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with string")
 
+
 def test_invoke_with_invalid_json_blob(bb, verbose=False):
     prompt = "{\"status\":\"invalid\"}"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with invalid json blob")
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with invalid json blob")
 
+
 def test_invoke_with_valid_json_blob(bb, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with valid json blob")
-        schema_inst = bb.get_model_schema_object(model)
+        schema_inst = bb.get_model_request_object(model)
         schema_inst.update_prompt(prompt)
         blob = schema_inst.json()
         r = bb.invoke(model, blob, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with valid json blob")
 
+
 def test_invoke_with_valid_dict(bb, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with valid dict")
-        schema_inst = bb.get_model_schema_object(model)
+        schema_inst = bb.get_model_request_object(model)
         schema_inst.update_prompt(prompt)
         j = schema_inst.json()
         d = json.loads(j)
         r = bb.invoke(model, d, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with valid dict")
 
+
 def test_invoke_with_invalid_dict(bb, verbose=False):
     all_models = bb.get_available_models()
-    d = {"status":"invalid"}
+    d = {"status": "invalid"}
     for model in all_models:
         print(f"now testing {model} in invoke with invalid dict")
         try:
             r = bb.invoke(model, d, show_request=verbose)
         except ValueError:
-            pass # we expect this, it should fail in this case
+            pass  # we expect this, it should fail in this case
         if verbose:
             print(f"could not call model {model} in invoke with dict {d} (Ok)")
         print(f"done testing {model} in invoke with dict")
 
+
 def single_run(bb, verbose=False):
     prompt = "tell me about foobar"
-    bb.invoke("cohere.command-text-v14",prompt)
+    bb.invoke("cohere.command-text-v14", prompt)
+
+
+def invoke_set_params(bb, verbose=True):
+    params = bb.params
+    params["max_tokens"] = 88
+    params["top_p"] = 0.88
+    params["top_k"] = 88
+    params["temp"] = .88
+    bb.set_params(params)
+    prompt = "Hittem hard with dem params doe"
+    for model in bb.get_available_models():
+        r = bb.invoke(model, prompt, show_request=verbose)
+        if verbose:
+            print(r.get_answer_raw())
+
 
 if __name__ == "__main__":
     verbose = True
     session = boto3.session.Session(profile_name='default')
     bb = BasicBedrock(session=session)
     single_run(bb, verbose)
-
     test_invoke_with_string(bb, verbose=verbose)
+    invoke_set_params(bb, verbose=verbose)
     test_invoke_with_invalid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_dict(bb, verbose=verbose)
     test_invoke_with_invalid_dict(bb, verbose=verbose)
-    print("All tests successful")
+    print("All tests successful")
```

