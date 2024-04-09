# Comparing `tmp/liah-0.1.0.tar.gz` & `tmp/liah-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liah-0.1.0.tar", last modified: Sat Apr  6 15:37:42 2024, max compression
+gzip compressed data, was "liah-0.1.1.tar", last modified: Tue Apr  9 12:15:06 2024, max compression
```

## Comparing `liah-0.1.0.tar` & `liah-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-06 15:37:42.501535 liah-0.1.0/
--rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 15:26:24.000000 liah-0.1.0/LICENSE
--rw-r--r--   0 melvin     (501) staff       (20)       47 2024-04-06 15:37:37.000000 liah-0.1.0/MANIFEST.in
--rw-r--r--   0 melvin     (501) staff       (20)     1864 2024-04-06 15:37:42.501301 liah-0.1.0/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)     1353 2024-04-06 14:30:35.000000 liah-0.1.0/README.md
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-06 15:37:42.498134 liah-0.1.0/liah/
--rw-r--r--   0 melvin     (501) staff       (20)     5121 2024-04-06 09:10:37.000000 liah-0.1.0/liah/Liah.py
--rw-r--r--   0 melvin     (501) staff       (20)        0 2024-04-06 14:32:37.000000 liah-0.1.0/liah/__init__.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-06 15:37:42.500468 liah-0.1.0/liah/dataset/
--rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.0/liah/dataset/README.md
--rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-03 16:37:16.000000 liah-0.1.0/liah/dataset/daughter_of_the_dawn.txt
--rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-03 16:37:16.000000 liah-0.1.0/liah/dataset/when_everybody_knew.txt
--rw-r--r--   0 melvin     (501) staff       (20)     8668 2024-04-06 09:10:37.000000 liah-0.1.0/liah/dataset_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     3359 2024-04-06 09:10:37.000000 liah-0.1.0/liah/evaluator.py
--rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 09:10:37.000000 liah-0.1.0/liah/plot_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     1339 2024-04-06 09:10:37.000000 liah-0.1.0/liah/utils.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-06 15:37:42.501051 liah-0.1.0/liah.egg-info/
--rw-r--r--   0 melvin     (501) staff       (20)     1864 2024-04-06 15:37:42.000000 liah-0.1.0/liah.egg-info/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-06 15:37:42.000000 liah-0.1.0/liah.egg-info/SOURCES.txt
--rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-06 15:37:42.000000 liah-0.1.0/liah.egg-info/dependency_links.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 15:37:42.000000 liah-0.1.0/liah.egg-info/requires.txt
--rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-06 15:37:42.000000 liah-0.1.0/liah.egg-info/top_level.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.0/requirements.txt
--rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-06 15:37:42.501584 liah-0.1.0/setup.cfg
--rw-r--r--   0 melvin     (501) staff       (20)      909 2024-04-06 15:36:16.000000 liah-0.1.0/setup.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.724910 liah-0.1.1/
+-rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.1/LICENSE
+-rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.1/MANIFEST.in
+-rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:15:06.724678 liah-0.1.1/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)     1380 2024-04-09 12:07:14.000000 liah-0.1.1/README.md
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.720341 liah-0.1.1/liah/
+-rw-r--r--   0 melvin     (501) staff       (20)     5124 2024-04-09 12:14:00.000000 liah-0.1.1/liah/Liah.py
+-rw-r--r--   0 melvin     (501) staff       (20)        0 2024-04-06 16:08:56.000000 liah-0.1.1/liah/__init__.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.723769 liah-0.1.1/liah/dataset/
+-rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.1/liah/dataset/README.md
+-rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.1/liah/dataset/daughter_of_the_dawn.txt
+-rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.1/liah/dataset/when_everybody_knew.txt
+-rw-r--r--   0 melvin     (501) staff       (20)     8668 2024-04-06 16:08:56.000000 liah-0.1.1/liah/dataset_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     3359 2024-04-09 12:14:23.000000 liah-0.1.1/liah/evaluator.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 16:08:56.000000 liah-0.1.1/liah/plot_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1339 2024-04-06 16:08:56.000000 liah-0.1.1/liah/utils.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.724400 liah-0.1.1/liah.egg-info/
+-rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/SOURCES.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/dependency_links.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/requires.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/top_level.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.1/requirements.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 12:15:06.724962 liah-0.1.1/setup.cfg
+-rw-r--r--   0 melvin     (501) staff       (20)      910 2024-04-09 12:14:53.000000 liah-0.1.1/setup.py
```

### Comparing `liah-0.1.0/LICENSE` & `liah-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liah-0.1.0/PKG-INFO` & `liah-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.0
+Version: 0.1.1
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
 License: Apache 2.0
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
@@ -12,40 +12,43 @@
 License-File: LICENSE
 Requires-Dist: openai>=1.16.1
 Requires-Dist: matplotlib
 Requires-Dist: tiktoken
 Requires-Dist: tqdm
 
 
-# 🤥 LIAH - a Lie-in-haystack [WIP]
+# 🤥 LIAH - a Lie-in-haystack
 
 ![LIAH](/images/liah.png "Liah")
 
 With longer context lengths for LLMs. It is increasingly difficult to test
 if fine tuned models attend to all depths of the context.
 
 The needle in haystack is a popular approach. However since the LLMs can also answer
-about the needle instead of the needle. Tests have shown that a "Lie" works well in 
+about the needle instead of the needle. Tests have shown that a "Lie" works well in
 this context 😊
 
+## Installation
+    pip install liah
+
 ## Example Usage
 
-    # update OPENAI_API_KEY in the env with your token. 
+    # update OPENAI_API_KEY in the env with your token.
     # If you need Open AI models for the final evaluation
     from vllm import LLM, SamplingParams
 
     # Create a sampling params object.
     sampling_params = SamplingParams(temperature=0.8, top_p=0.95, max_tokens=4096)
     # llm = LLM(model="mistralai/Mistral-7B-v0.1")
     llm = LLM(model="meta-llama/Llama-2-70b-hf", tensor_parallel_size=4, max_model_len=1500) # need 4 A100s 40GB
     liah = Liah(max_context_length=2000)
-    
+
     for i, sample in enumerate(liah.getSample()):
         # test the sample text with your model
-        output = llm.generate([sample["prompt"], sampling_params)[0]
+        output = llm.generate([sample["prompt"]], sampling_params)[0]
         liah.update(sample, output.outputs[0].text)
     plotFilePath = liah.evaluate()
 
 ## Contribute
 
     bash
     pip install pre-commit
```

### Comparing `liah-0.1.0/README.md` & `liah-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 
-# 🤥 LIAH - a Lie-in-haystack [WIP]
+# 🤥 LIAH - a Lie-in-haystack
 
 ![LIAH](/images/liah.png "Liah")
 
 With longer context lengths for LLMs. It is increasingly difficult to test
 if fine tuned models attend to all depths of the context.
 
 The needle in haystack is a popular approach. However since the LLMs can also answer
-about the needle instead of the needle. Tests have shown that a "Lie" works well in 
+about the needle instead of the needle. Tests have shown that a "Lie" works well in
 this context 😊
 
+## Installation
+    pip install liah
+
 ## Example Usage
 
-    # update OPENAI_API_KEY in the env with your token. 
+    # update OPENAI_API_KEY in the env with your token.
     # If you need Open AI models for the final evaluation
     from vllm import LLM, SamplingParams
 
     # Create a sampling params object.
     sampling_params = SamplingParams(temperature=0.8, top_p=0.95, max_tokens=4096)
     # llm = LLM(model="mistralai/Mistral-7B-v0.1")
     llm = LLM(model="meta-llama/Llama-2-70b-hf", tensor_parallel_size=4, max_model_len=1500) # need 4 A100s 40GB
     liah = Liah(max_context_length=2000)
-    
+
     for i, sample in enumerate(liah.getSample()):
         # test the sample text with your model
-        output = llm.generate([sample["prompt"], sampling_params)[0]
+        output = llm.generate([sample["prompt"]], sampling_params)[0]
         liah.update(sample, output.outputs[0].text)
     plotFilePath = liah.evaluate()
 
 ## Contribute
 
     bash
     pip install pre-commit
```

### Comparing `liah-0.1.0/liah/Liah.py` & `liah-0.1.1/liah/Liah.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from tqdm import tqdm
-
-from dataset_utils import create_ctx_len_dataset, insertLieInHayStacks
-from evaluator import eval_resp
-from plot_utils import plot_scores
-from utils import lie_needles
+from .dataset_utils import create_ctx_len_dataset, insertLieInHayStacks
+from .evaluator import eval_resp
+from .plot_utils import plot_scores
+from .utils import lie_needles
 
 
 class Liah:
     def __init__(
         self,
         pos_dist="linear",
         needle_positions=None,
```

### Comparing `liah-0.1.0/liah/dataset/daughter_of_the_dawn.txt` & `liah-0.1.1/liah/dataset/daughter_of_the_dawn.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.0/liah/dataset/when_everybody_knew.txt` & `liah-0.1.1/liah/dataset/when_everybody_knew.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.0/liah/dataset_utils.py` & `liah-0.1.1/liah/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.0/liah/evaluator.py` & `liah-0.1.1/liah/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import re
 
 from openai import OpenAI
-
-from utils import expert_prompt, system_prompt
+from .utils import expert_prompt, system_prompt
 
 
 def evaluate(user_prompts):
     scores = []
     client = OpenAI()
     for student_prompt in user_prompts:
         response = client.chat.completions.create(
```

### Comparing `liah-0.1.0/liah/plot_utils.py` & `liah-0.1.1/liah/plot_utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.0/liah/utils.py` & `liah-0.1.1/liah/utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.0/liah.egg-info/PKG-INFO` & `liah-0.1.1/liah.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.0
+Version: 0.1.1
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
 License: Apache 2.0
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
@@ -12,40 +12,43 @@
 License-File: LICENSE
 Requires-Dist: openai>=1.16.1
 Requires-Dist: matplotlib
 Requires-Dist: tiktoken
 Requires-Dist: tqdm
 
 
-# 🤥 LIAH - a Lie-in-haystack [WIP]
+# 🤥 LIAH - a Lie-in-haystack
 
 ![LIAH](/images/liah.png "Liah")
 
 With longer context lengths for LLMs. It is increasingly difficult to test
 if fine tuned models attend to all depths of the context.
 
 The needle in haystack is a popular approach. However since the LLMs can also answer
-about the needle instead of the needle. Tests have shown that a "Lie" works well in 
+about the needle instead of the needle. Tests have shown that a "Lie" works well in
 this context 😊
 
+## Installation
+    pip install liah
+
 ## Example Usage
 
-    # update OPENAI_API_KEY in the env with your token. 
+    # update OPENAI_API_KEY in the env with your token.
     # If you need Open AI models for the final evaluation
     from vllm import LLM, SamplingParams
 
     # Create a sampling params object.
     sampling_params = SamplingParams(temperature=0.8, top_p=0.95, max_tokens=4096)
     # llm = LLM(model="mistralai/Mistral-7B-v0.1")
     llm = LLM(model="meta-llama/Llama-2-70b-hf", tensor_parallel_size=4, max_model_len=1500) # need 4 A100s 40GB
     liah = Liah(max_context_length=2000)
-    
+
     for i, sample in enumerate(liah.getSample()):
         # test the sample text with your model
-        output = llm.generate([sample["prompt"], sampling_params)[0]
+        output = llm.generate([sample["prompt"]], sampling_params)[0]
         liah.update(sample, output.outputs[0].text)
     plotFilePath = liah.evaluate()
 
 ## Contribute
 
     bash
     pip install pre-commit
```

### Comparing `liah-0.1.0/setup.py` & `liah-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from setuptools import setup, find_packages
 import os
 
+from setuptools import find_packages, setup
+
 current_directory = os.path.abspath(os.path.dirname(__file__))
 print(current_directory)
 requirements_path = os.path.join(current_directory, "requirements.txt")
 with open(requirements_path, "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="liah",
-    version="0.1.0",
+    version="0.1.1",
     author="James Melvin Priyarajan",
     author_email="melvinebenezer@gmail.com",
     description="Insert a Lie in a Haystack and evaluate the model's ability to detect it.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/melvinebenezer/Liah-Lie_in_a_haystack",
     packages=find_packages(),
```

