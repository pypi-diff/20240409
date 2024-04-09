# Comparing `tmp/llmlingua-0.2.1.tar.gz` & `tmp/llmlingua-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmlingua-0.2.1.tar", last modified: Wed Mar 20 03:43:51 2024, max compression
+gzip compressed data, was "llmlingua-0.2.2.tar", last modified: Tue Apr  9 08:21:51 2024, max compression
```

## Comparing `llmlingua-0.2.1.tar` & `llmlingua-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:43:51.511219 llmlingua-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-20 03:42:07.000000 llmlingua-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-03-20 03:43:51.511219 llmlingua-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-03-20 03:42:07.000000 llmlingua-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:43:51.507219 llmlingua-0.2.1/llmlingua/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-20 03:42:07.000000 llmlingua-0.2.1/llmlingua/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   107104 2024-03-20 03:42:07.000000 llmlingua-0.2.1/llmlingua/prompt_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-20 03:42:07.000000 llmlingua-0.2.1/llmlingua/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-20 03:42:07.000000 llmlingua-0.2.1/llmlingua/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:43:51.511219 llmlingua-0.2.1/llmlingua.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-03-20 03:43:51.000000 llmlingua-0.2.1/llmlingua.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-20 03:43:51.000000 llmlingua-0.2.1/llmlingua.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:43:51.000000 llmlingua-0.2.1/llmlingua.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:42:11.000000 llmlingua-0.2.1/llmlingua.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-20 03:43:51.000000 llmlingua-0.2.1/llmlingua.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-20 03:43:51.000000 llmlingua-0.2.1/llmlingua.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-20 03:42:07.000000 llmlingua-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-20 03:43:51.519219 llmlingua-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-20 03:42:07.000000 llmlingua-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:43:51.511219 llmlingua-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18984 2024-03-20 03:42:07.000000 llmlingua-0.2.1/tests/test_llmlingua.py
--rw-r--r--   0 runner    (1001) docker     (127)    36236 2024-03-20 03:42:07.000000 llmlingua-0.2.1/tests/test_llmlingua2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-03-20 03:42:07.000000 llmlingua-0.2.1/tests/test_longllmlingua.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:21:51.055876 llmlingua-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-09 08:19:43.000000 llmlingua-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-04-09 08:21:51.055876 llmlingua-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-04-09 08:19:43.000000 llmlingua-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:21:51.055876 llmlingua-0.2.2/llmlingua/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 08:19:43.000000 llmlingua-0.2.2/llmlingua/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109840 2024-04-09 08:19:43.000000 llmlingua-0.2.2/llmlingua/prompt_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-09 08:19:43.000000 llmlingua-0.2.2/llmlingua/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 08:19:43.000000 llmlingua-0.2.2/llmlingua/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:21:51.055876 llmlingua-0.2.2/llmlingua.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-04-09 08:21:51.000000 llmlingua-0.2.2/llmlingua.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 08:21:51.000000 llmlingua-0.2.2/llmlingua.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:21:51.000000 llmlingua-0.2.2/llmlingua.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:19:50.000000 llmlingua-0.2.2/llmlingua.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 08:21:51.000000 llmlingua-0.2.2/llmlingua.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 08:21:51.000000 llmlingua-0.2.2/llmlingua.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 08:19:43.000000 llmlingua-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 08:21:51.063876 llmlingua-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-09 08:19:43.000000 llmlingua-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:21:51.055876 llmlingua-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18984 2024-04-09 08:19:43.000000 llmlingua-0.2.2/tests/test_llmlingua.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36247 2024-04-09 08:19:43.000000 llmlingua-0.2.2/tests/test_llmlingua2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22655 2024-04-09 08:19:43.000000 llmlingua-0.2.2/tests/test_longllmlingua.py
```

### Comparing `llmlingua-0.2.1/LICENSE` & `llmlingua-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmlingua-0.2.1/PKG-INFO` & `llmlingua-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmlingua
-Version: 0.2.1
+Version: 0.2.2
 Summary: To speed up LLMs' inference and enhance LLM's perceive of key information, compress the prompt and KV-Cache, which achieves up to 20x compression with minimal performance loss.
 Home-page: https://github.com/microsoft/LLMLingua
 Author: The LLMLingua team
 Author-email: hjiang@microsoft.com
 License: MIT License
 Keywords: Prompt Compression,LLMs,Inference Acceleration,Black-box LLMs,Efficient LLMs
 Classifier: Intended Audience :: Science/Research
@@ -57,15 +57,15 @@
 LongLLMLingua mitigates the 'lost in the middle' issue in LLMs, enhancing long-context information processing. It reduces costs and boosts efficiency with prompt compression, improving RAG performance by up to 21.4% using only 1/4 of the tokens.
 
 - [LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) (ICLR ME-FoMo 2024)<br>
   _Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang and Lili Qiu_
 
 LLMLingua-2, a small-size yet powerful prompt compression method trained via data distillation from GPT-4 for token classification with a BERT-level encoder, excels in task-agnostic compression. It surpasses LLMLingua in handling out-of-domain data, offering 3x-6x faster performance.
 
-- [LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)<br>
+- [LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)<br>
   _Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang, Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu, Dongmei Zhang_
 
 ## 🎥 Overview
 
 ![Background](./images/LLMLingua_motivation.png)
 
 - Ever encountered the token limit when asking ChatGPT to summarize lengthy texts?
@@ -120,15 +120,15 @@
     volume = "abs/2310.06839",
     year = "2023",
 }
 ```
 
 ```bibtex
 @article{wu2024llmlingua2,
-    title = "{LLML}ingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression",
+    title = "{LLML}ingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression",
     author = "Zhuoshi Pan and Qianhui Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang and Qingwei Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky Zhao and Lili Qiu and Dongmei Zhang",
     url = "https://arxiv.org/abs/2403.12968",
     journal = "ArXiv preprint",
     volume = "abs/2403.12968",
     year = "2024",
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: llmlingua Version: 0.2.1 Summary: To speed up LLMs'
+Metadata-Version: 2.1 Name: llmlingua Version: 0.2.2 Summary: To speed up LLMs'
 inference and enhance LLM's perceive of key information, compress the prompt
 and KV-Cache, which achieves up to 20x compression with minimal performance
 loss. Home-page: https://github.com/microsoft/LLMLingua Author: The LLMLingua
 team Author-email: hjiang@microsoft.com License: MIT License Keywords: Prompt
 Compression,LLMs,Inference Acceleration,Black-box LLMs,Efficient LLMs
 Classifier: Intended Audience :: Science/Research Classifier: Development
 Status :: 3 - Alpha Classifier: Programming Language :: Python :: 3 Classifier:
@@ -54,16 +54,16 @@
 Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) (ICLR ME-
 FoMo 2024)
 _Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing
 Yang and Lili Qiu_ LLMLingua-2, a small-size yet powerful prompt compression
 method trained via data distillation from GPT-4 for token classification with a
 BERT-level encoder, excels in task-agnostic compression. It surpasses LLMLingua
 in handling out-of-domain data, offering 3x-6x faster performance. -
-[LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-
-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)
+[LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt
+Compression](https://arxiv.org/abs/2403.12968) (Under Review)
 _Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang,
 Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu,
 Dongmei Zhang_ ## ð¥ Overview ![Background](./images/
 LLMLingua_motivation.png) - Ever encountered the token limit when asking
 ChatGPT to summarize lengthy texts? - Frustrated with ChatGPT forgetting
 previous instructions after extensive fine-tuning? - Experienced high costs
 using GPT3.5/4 API for experiments despite excellent results? While Large
@@ -93,48 +93,47 @@
 "https://aclanthology.org/2023.emnlp-main.825", doi = "10.18653/v1/2023.emnlp-
 main.825", pages = "13358--13376", } ``` ```bibtex @article{jiang-etal-2023-
 longllmlingua, title = "{L}ong{LLML}ingua: Accelerating and Enhancing LLMs in
 Long Context Scenarios via Prompt Compression", author = "Huiqiang Jiang and
 Qianhui Wu and and Xufang Luo and Dongsheng Li and Chin-Yew Lin and Yuqing Yang
 and Lili Qiu", url = "https://arxiv.org/abs/2310.06839", journal = "ArXiv
 preprint", volume = "abs/2310.06839", year = "2023", } ``` ```bibtex @article
-{wu2024llmlingua2, title = "{LLML}ingua-2: Context-Aware Data Distillation for
-Efficient and Faithful Task-Agnostic Prompt Compression", author = "Zhuoshi Pan
-and Qianhui Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang
-and Qingwei Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky
-Zhao and Lili Qiu and Dongmei Zhang", url = "https://arxiv.org/abs/2403.12968",
-journal = "ArXiv preprint", volume = "abs/2403.12968", year = "2024", } ``` ##
-ð¯ Quick Start #### 1. **Installing LLMLingua:** To get started with
-LLMLingua, simply install it using pip: ```bash pip install llmlingua ``` ####
-2. **Using LLMLingua Series Methods for Prompt Compression:** With
-**LLMLingua**, you can easily compress your prompts. Hereâs how you can do
-it: ```python from llmlingua import PromptCompressor llm_lingua =
-PromptCompressor() compressed_prompt = llm_lingua.compress_prompt(prompt,
-instruction="", question="", target_token=200) # > {'compressed_prompt':
-'Question: Sam bought a dozen boxes, each with 30 highlighter pens inside, for
-$10 each box. He reanged five of boxes into packages of sixlters each and sold
-them $3 per. He sold the rest theters separately at the of three pens $2. How
-much did make in total, dollars?\nLets think step step\nSam bought 1 boxes x00
-oflters.\nHe bought 12 * 300ters in total\nSam then took 5 boxes
-6ters0ters.\nHe sold these boxes for 5 *5\nAfterelling these boxes there were
-3030 highlighters remaining.\nThese form 330 / 3 = 110 groups of three
-pens.\nHe sold each of these groups for $2 each, so made 110 * 2 = $220 from
-them.\nIn total, then, he earned $220 + $15 = $235.\nSince his original cost
-was $120, he earned $235 - $120 = $115 in profit.\nThe answer is 115', #
-'origin_tokens': 2365, # 'compressed_tokens': 211, # 'ratio': '11.2x', #
-'saving': ', Saving $0.1 in GPT-4.'} ## Or use the phi-2 model, llm_lingua =
-PromptCompressor("microsoft/phi-2") ## Or use the quantation model, like
-TheBloke/Llama-2-7b-Chat-GPTQ, only need <8GB GPU memory. ## Before that, you
-need to pip install optimum auto-gptq llm_lingua = PromptCompressor("TheBloke/
-Llama-2-7b-Chat-GPTQ", model_config={"revision": "main"}) ``` To try
-**LongLLMLingua** in your scenorias, you can use ```python from llmlingua
-import PromptCompressor llm_lingua = PromptCompressor() compressed_prompt =
-llm_lingua.compress_prompt( prompt_list, question=question, ratio=0.55, # Set
-the special parameter for LongLLMLingua
-condition_in_question="after_condition", reorder_context="sort",
+{wu2024llmlingua2, title = "{LLML}ingua-2: Data Distillation for Efficient and
+Faithful Task-Agnostic Prompt Compression", author = "Zhuoshi Pan and Qianhui
+Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang and Qingwei
+Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky Zhao and
+Lili Qiu and Dongmei Zhang", url = "https://arxiv.org/abs/2403.12968", journal
+= "ArXiv preprint", volume = "abs/2403.12968", year = "2024", } ``` ## ð¯
+Quick Start #### 1. **Installing LLMLingua:** To get started with LLMLingua,
+simply install it using pip: ```bash pip install llmlingua ``` #### 2. **Using
+LLMLingua Series Methods for Prompt Compression:** With **LLMLingua**, you can
+easily compress your prompts. Hereâs how you can do it: ```python from
+llmlingua import PromptCompressor llm_lingua = PromptCompressor()
+compressed_prompt = llm_lingua.compress_prompt(prompt, instruction="",
+question="", target_token=200) # > {'compressed_prompt': 'Question: Sam bought
+a dozen boxes, each with 30 highlighter pens inside, for $10 each box. He
+reanged five of boxes into packages of sixlters each and sold them $3 per. He
+sold the rest theters separately at the of three pens $2. How much did make in
+total, dollars?\nLets think step step\nSam bought 1 boxes x00 oflters.\nHe
+bought 12 * 300ters in total\nSam then took 5 boxes 6ters0ters.\nHe sold these
+boxes for 5 *5\nAfterelling these boxes there were 3030 highlighters
+remaining.\nThese form 330 / 3 = 110 groups of three pens.\nHe sold each of
+these groups for $2 each, so made 110 * 2 = $220 from them.\nIn total, then, he
+earned $220 + $15 = $235.\nSince his original cost was $120, he earned $235 -
+$120 = $115 in profit.\nThe answer is 115', # 'origin_tokens': 2365, #
+'compressed_tokens': 211, # 'ratio': '11.2x', # 'saving': ', Saving $0.1 in
+GPT-4.'} ## Or use the phi-2 model, llm_lingua = PromptCompressor("microsoft/
+phi-2") ## Or use the quantation model, like TheBloke/Llama-2-7b-Chat-GPTQ,
+only need <8GB GPU memory. ## Before that, you need to pip install optimum
+auto-gptq llm_lingua = PromptCompressor("TheBloke/Llama-2-7b-Chat-GPTQ",
+model_config={"revision": "main"}) ``` To try **LongLLMLingua** in your
+scenorias, you can use ```python from llmlingua import PromptCompressor
+llm_lingua = PromptCompressor() compressed_prompt = llm_lingua.compress_prompt
+( prompt_list, question=question, ratio=0.55, # Set the special parameter for
+LongLLMLingua condition_in_question="after_condition", reorder_context="sort",
 dynamic_context_compression_ratio=0.3, # or 0.4 condition_compare=True,
 context_budget="+100", rank_method="longllmlingua", ) ``` To try **LLMLingua-
 2** in your scenorias, you can use ```python from llmlingua import
 PromptCompressor llm_lingua = PromptCompressor( model_name="microsoft/
 llmlingua-2-xlm-roberta-large-meetingbank", use_llmlingua2=True, # Whether to
 use llmlingua-2 ) compressed_prompt = llm_lingua.compress_prompt(prompt,
 rate=0.33, force_tokens = ['\n', '?']) ## Or use LLMLingua-2-small model
```

### Comparing `llmlingua-0.2.1/README.md` & `llmlingua-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 LongLLMLingua mitigates the 'lost in the middle' issue in LLMs, enhancing long-context information processing. It reduces costs and boosts efficiency with prompt compression, improving RAG performance by up to 21.4% using only 1/4 of the tokens.
 
 - [LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) (ICLR ME-FoMo 2024)<br>
   _Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang and Lili Qiu_
 
 LLMLingua-2, a small-size yet powerful prompt compression method trained via data distillation from GPT-4 for token classification with a BERT-level encoder, excels in task-agnostic compression. It surpasses LLMLingua in handling out-of-domain data, offering 3x-6x faster performance.
 
-- [LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)<br>
+- [LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)<br>
   _Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang, Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu, Dongmei Zhang_
 
 ## 🎥 Overview
 
 ![Background](./images/LLMLingua_motivation.png)
 
 - Ever encountered the token limit when asking ChatGPT to summarize lengthy texts?
@@ -101,15 +101,15 @@
     volume = "abs/2310.06839",
     year = "2023",
 }
 ```
 
 ```bibtex
 @article{wu2024llmlingua2,
-    title = "{LLML}ingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression",
+    title = "{LLML}ingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression",
     author = "Zhuoshi Pan and Qianhui Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang and Qingwei Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky Zhao and Lili Qiu and Dongmei Zhang",
     url = "https://arxiv.org/abs/2403.12968",
     journal = "ArXiv preprint",
     volume = "abs/2403.12968",
     year = "2024",
 }
 ```
```

#### html2text {}

```diff
@@ -43,16 +43,16 @@
 Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) (ICLR ME-
 FoMo 2024)
 _Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing
 Yang and Lili Qiu_ LLMLingua-2, a small-size yet powerful prompt compression
 method trained via data distillation from GPT-4 for token classification with a
 BERT-level encoder, excels in task-agnostic compression. It surpasses LLMLingua
 in handling out-of-domain data, offering 3x-6x faster performance. -
-[LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-
-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)
+[LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt
+Compression](https://arxiv.org/abs/2403.12968) (Under Review)
 _Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang,
 Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu,
 Dongmei Zhang_ ## ð¥ Overview ![Background](./images/
 LLMLingua_motivation.png) - Ever encountered the token limit when asking
 ChatGPT to summarize lengthy texts? - Frustrated with ChatGPT forgetting
 previous instructions after extensive fine-tuning? - Experienced high costs
 using GPT3.5/4 API for experiments despite excellent results? While Large
@@ -82,48 +82,47 @@
 "https://aclanthology.org/2023.emnlp-main.825", doi = "10.18653/v1/2023.emnlp-
 main.825", pages = "13358--13376", } ``` ```bibtex @article{jiang-etal-2023-
 longllmlingua, title = "{L}ong{LLML}ingua: Accelerating and Enhancing LLMs in
 Long Context Scenarios via Prompt Compression", author = "Huiqiang Jiang and
 Qianhui Wu and and Xufang Luo and Dongsheng Li and Chin-Yew Lin and Yuqing Yang
 and Lili Qiu", url = "https://arxiv.org/abs/2310.06839", journal = "ArXiv
 preprint", volume = "abs/2310.06839", year = "2023", } ``` ```bibtex @article
-{wu2024llmlingua2, title = "{LLML}ingua-2: Context-Aware Data Distillation for
-Efficient and Faithful Task-Agnostic Prompt Compression", author = "Zhuoshi Pan
-and Qianhui Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang
-and Qingwei Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky
-Zhao and Lili Qiu and Dongmei Zhang", url = "https://arxiv.org/abs/2403.12968",
-journal = "ArXiv preprint", volume = "abs/2403.12968", year = "2024", } ``` ##
-ð¯ Quick Start #### 1. **Installing LLMLingua:** To get started with
-LLMLingua, simply install it using pip: ```bash pip install llmlingua ``` ####
-2. **Using LLMLingua Series Methods for Prompt Compression:** With
-**LLMLingua**, you can easily compress your prompts. Hereâs how you can do
-it: ```python from llmlingua import PromptCompressor llm_lingua =
-PromptCompressor() compressed_prompt = llm_lingua.compress_prompt(prompt,
-instruction="", question="", target_token=200) # > {'compressed_prompt':
-'Question: Sam bought a dozen boxes, each with 30 highlighter pens inside, for
-$10 each box. He reanged five of boxes into packages of sixlters each and sold
-them $3 per. He sold the rest theters separately at the of three pens $2. How
-much did make in total, dollars?\nLets think step step\nSam bought 1 boxes x00
-oflters.\nHe bought 12 * 300ters in total\nSam then took 5 boxes
-6ters0ters.\nHe sold these boxes for 5 *5\nAfterelling these boxes there were
-3030 highlighters remaining.\nThese form 330 / 3 = 110 groups of three
-pens.\nHe sold each of these groups for $2 each, so made 110 * 2 = $220 from
-them.\nIn total, then, he earned $220 + $15 = $235.\nSince his original cost
-was $120, he earned $235 - $120 = $115 in profit.\nThe answer is 115', #
-'origin_tokens': 2365, # 'compressed_tokens': 211, # 'ratio': '11.2x', #
-'saving': ', Saving $0.1 in GPT-4.'} ## Or use the phi-2 model, llm_lingua =
-PromptCompressor("microsoft/phi-2") ## Or use the quantation model, like
-TheBloke/Llama-2-7b-Chat-GPTQ, only need <8GB GPU memory. ## Before that, you
-need to pip install optimum auto-gptq llm_lingua = PromptCompressor("TheBloke/
-Llama-2-7b-Chat-GPTQ", model_config={"revision": "main"}) ``` To try
-**LongLLMLingua** in your scenorias, you can use ```python from llmlingua
-import PromptCompressor llm_lingua = PromptCompressor() compressed_prompt =
-llm_lingua.compress_prompt( prompt_list, question=question, ratio=0.55, # Set
-the special parameter for LongLLMLingua
-condition_in_question="after_condition", reorder_context="sort",
+{wu2024llmlingua2, title = "{LLML}ingua-2: Data Distillation for Efficient and
+Faithful Task-Agnostic Prompt Compression", author = "Zhuoshi Pan and Qianhui
+Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang and Qingwei
+Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky Zhao and
+Lili Qiu and Dongmei Zhang", url = "https://arxiv.org/abs/2403.12968", journal
+= "ArXiv preprint", volume = "abs/2403.12968", year = "2024", } ``` ## ð¯
+Quick Start #### 1. **Installing LLMLingua:** To get started with LLMLingua,
+simply install it using pip: ```bash pip install llmlingua ``` #### 2. **Using
+LLMLingua Series Methods for Prompt Compression:** With **LLMLingua**, you can
+easily compress your prompts. Hereâs how you can do it: ```python from
+llmlingua import PromptCompressor llm_lingua = PromptCompressor()
+compressed_prompt = llm_lingua.compress_prompt(prompt, instruction="",
+question="", target_token=200) # > {'compressed_prompt': 'Question: Sam bought
+a dozen boxes, each with 30 highlighter pens inside, for $10 each box. He
+reanged five of boxes into packages of sixlters each and sold them $3 per. He
+sold the rest theters separately at the of three pens $2. How much did make in
+total, dollars?\nLets think step step\nSam bought 1 boxes x00 oflters.\nHe
+bought 12 * 300ters in total\nSam then took 5 boxes 6ters0ters.\nHe sold these
+boxes for 5 *5\nAfterelling these boxes there were 3030 highlighters
+remaining.\nThese form 330 / 3 = 110 groups of three pens.\nHe sold each of
+these groups for $2 each, so made 110 * 2 = $220 from them.\nIn total, then, he
+earned $220 + $15 = $235.\nSince his original cost was $120, he earned $235 -
+$120 = $115 in profit.\nThe answer is 115', # 'origin_tokens': 2365, #
+'compressed_tokens': 211, # 'ratio': '11.2x', # 'saving': ', Saving $0.1 in
+GPT-4.'} ## Or use the phi-2 model, llm_lingua = PromptCompressor("microsoft/
+phi-2") ## Or use the quantation model, like TheBloke/Llama-2-7b-Chat-GPTQ,
+only need <8GB GPU memory. ## Before that, you need to pip install optimum
+auto-gptq llm_lingua = PromptCompressor("TheBloke/Llama-2-7b-Chat-GPTQ",
+model_config={"revision": "main"}) ``` To try **LongLLMLingua** in your
+scenorias, you can use ```python from llmlingua import PromptCompressor
+llm_lingua = PromptCompressor() compressed_prompt = llm_lingua.compress_prompt
+( prompt_list, question=question, ratio=0.55, # Set the special parameter for
+LongLLMLingua condition_in_question="after_condition", reorder_context="sort",
 dynamic_context_compression_ratio=0.3, # or 0.4 condition_compare=True,
 context_budget="+100", rank_method="longllmlingua", ) ``` To try **LLMLingua-
 2** in your scenorias, you can use ```python from llmlingua import
 PromptCompressor llm_lingua = PromptCompressor( model_name="microsoft/
 llmlingua-2-xlm-roberta-large-meetingbank", use_llmlingua2=True, # Whether to
 use llmlingua-2 ) compressed_prompt = llm_lingua.compress_prompt(prompt,
 rate=0.33, force_tokens = ['\n', '?']) ## Or use LLMLingua-2-small model
```

### Comparing `llmlingua-0.2.1/llmlingua/prompt_compressor.py` & `llmlingua-0.2.2/llmlingua/prompt_compressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) 2023 Microsoft
 # Licensed under The MIT License [see LICENSE for details]
 
 import bisect
 import copy
+import json
 import re
 import string
 from collections import defaultdict
-from typing import List
+from typing import List, Union
 
 import nltk
 import numpy as np
 import tiktoken
 import torch
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
@@ -21,40 +22,40 @@
     AutoTokenizer,
 )
 
 from .utils import (
     TokenClfDataset,
     get_pure_token,
     is_begin_of_new_word,
+    process_structured_json_data,
+    remove_consecutive_commas,
     replace_added_token,
     seed_everything,
 )
 
 
 class PromptCompressor:
     """
     PromptCompressor is designed for compressing prompts based on a given language model.
 
     This class initializes with the language model and its configuration, preparing it for prompt compression tasks.
     The PromptCompressor class is versatile and can be adapted for various models and specific requirements in prompt processing.
     Users can specify different model names and configurations as needed for their particular use case.The architecture is
     based on the paper "LLMLingua: Compressing Prompts for Accelerated Inference of Large Language Models". Jiang, Huiqiang, Qianhui Wu,
-    Chin-Yew Lin, Yuqing Yang, and Lili Qiu. "Llmlingua: Compressing prompts for accelerated inference of large language models."
-    arXiv preprint arXiv:2310.05736 (2023).
+    Chin-Yew Lin, Yuqing Yang, and Lili Qiu. arXiv preprint arXiv:2310.05736 (2023).
 
     Args:
         model_name (str, optional): The name of the language model to be loaded. Default is "NousResearch/Llama-2-7b-hf".
         device_map (str, optional): The device to load the model onto, e.g., "cuda" for GPU. Default is "cuda".
         model_config (dict, optional): A dictionary containing the configuration parameters for the model. Default is an empty dictionary.
         open_api_config (dict, optional): A dictionary containing configuration for openai APIs that may be used in conjunction with the model. Default is an empty dictionary.
         use_llmlingua2 (bool, optional): Whether to use llmlingua-2 compressor based on the paper
-            "LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression".
+            "LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression".
             Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang, Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu, Dongmei Zhang.
-            "LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression". arXiv preprint arXiv:,
-            Default is True.
+            arXiv preprint arXiv:2403.2403.12968 (2024), Default is True.
         llmlingua2_config (dict, optional): A dictionary containing the configuration parameters for llmlingua-2. Default is
             {
                 "max_batch_size": 50,
                 "max_force_token": 100, # max number of the tokens which will be forcely preserved
             }
     Example:
         >>> compress_method = PromptCompressor(model_name="microsoft/llmlingua-2-xlm-roberta-large-meetingbank", use_llmlingua2=True, )
@@ -134,27 +135,27 @@
             device_map
             if any(key in device_map for key in ["cuda", "cpu", "mps"])
             else "cuda"
         )
         if "cuda" in device_map or "cpu" in device_map:
             model = MODEL_CLASS.from_pretrained(
                 model_name,
-                torch_dtype=model_config.get(
+                torch_dtype=model_config.pop(
                     "torch_dtype", "auto" if device_map == "cuda" else torch.float32
                 ),
                 device_map=device_map,
                 config=config,
                 ignore_mismatched_sizes=True,
                 **model_config,
             )
         else:
             model = MODEL_CLASS.from_pretrained(
                 model_name,
                 device_map=device_map,
-                torch_dtype=model_config.get("torch_dtype", "auto"),
+                torch_dtype=model_config.pop("torch_dtype", "auto"),
                 pad_token_id=tokenizer.pad_token_id,
                 **model_config,
             )
         self.tokenizer = tokenizer
         self.model = model
         self.context_idxs = []
         self.max_position_embeddings = config.max_position_embeddings
@@ -205,14 +206,73 @@
             loss = loss[condition_pos_id:]
         res = loss.mean() if granularity == "sentence" else loss
         return (res, past_key_values) if return_kv else res
 
     def __call__(self, *args, **kwargs):
         return self.compress_prompt(*args, **kwargs)
 
+    def compress_json(
+        self,
+        json_data: dict,
+        json_config: Union[str, dict],
+        instruction: str = "",
+        question: str = "",
+        rate: float = 0.5,
+        target_token: float = -1,
+        iterative_size: int = 200,
+        use_sentence_level_filter: bool = False,
+        use_keyvalue_level_filter: bool = False,
+        use_token_level_filter: bool = True,
+        keep_split: bool = False,
+        keep_first_sentence: int = 0,
+        keep_last_sentence: int = 0,
+        keep_sentence_number: int = 0,
+        high_priority_bonus: int = 100,
+        context_budget: str = "+100",
+        token_budget_ratio: float = 1.4,
+        condition_in_question: str = "none",
+        reorder_keyvalue: str = "original",
+        condition_compare: bool = False,
+        rank_method: str = "llmlingua",
+    ):
+        context, force_context_ids = process_structured_json_data(
+            json_data, json_config
+        )
+        compressed_res = self.structured_compress_prompt(
+            context=context,
+            instruction=instruction,
+            question=question,
+            rate=rate,
+            target_token=target_token,
+            iterative_size=iterative_size,
+            force_context_ids=force_context_ids,
+            use_sentence_level_filter=use_sentence_level_filter,
+            use_context_level_filter=use_keyvalue_level_filter,
+            use_token_level_filter=use_token_level_filter,
+            keep_split=keep_split,
+            keep_first_sentence=keep_first_sentence,
+            keep_last_sentence=keep_last_sentence,
+            keep_sentence_number=keep_sentence_number,
+            high_priority_bonus=high_priority_bonus,
+            context_budget=context_budget,
+            token_budget_ratio=token_budget_ratio,
+            condition_in_question=condition_in_question,
+            reorder_context=reorder_keyvalue,
+            condition_compare=condition_compare,
+            add_instruction=False,
+            rank_method=rank_method,
+            concate_question=False,
+            strict_preserve_uncompressed=False,
+        )
+        compressed_json_text = remove_consecutive_commas(
+            compressed_res["compressed_prompt"]
+        )
+        compressed_res["compressed_prompt"] = json.loads(compressed_json_text)
+        return compressed_res
+
     def structured_compress_prompt(
         self,
         context: List[str],
         instruction: str = "",
         question: str = "",
         rate: float = 0.5,
         target_token: float = -1,
@@ -232,14 +292,15 @@
         condition_in_question: str = "none",
         reorder_context: str = "original",
         dynamic_context_compression_ratio: float = 0.0,
         condition_compare: bool = False,
         add_instruction: bool = False,
         rank_method: str = "llmlingua",
         concate_question: bool = True,
+        strict_preserve_uncompressed: bool = True,
     ):
         """
         Compresses the given prompt context based on a specified structure.
 
         Each element of context should be segmented using one or more non-nested '<llmlingua></llmlingua>' tags.
         Each '<llmlingua>' tag can include optional parameters 'rate' and 'compress' (e.g., '<llmlingua, rate=0.3, compress=True>'),
         indicating the compression rate for that segment. Default values are 'rate=rate' and 'compress=True'.
@@ -353,14 +414,15 @@
             condition_compare,
             add_instruction,
             rank_method,
             concate_question,
             context_segs=context_segs,
             context_segs_rate=context_segs_rate,
             context_segs_compress=context_segs_compress,
+            strict_preserve_uncompressed=strict_preserve_uncompressed,
         )
 
     def compress_prompt(
         self,
         context: List[str],
         instruction: str = "",
         question: str = "",
@@ -396,14 +458,15 @@
         word_sep: str = "\t\t|\t\t",
         label_sep: str = " ",
         token_to_word: str = "mean",
         force_tokens: List[str] = [],
         force_reserve_digit: bool = False,
         drop_consecutive: bool = False,
         chunk_end_tokens: List[str] = [".", "\n"],
+        strict_preserve_uncompressed: bool = True,
     ):
         """
         Compresses the given context.
 
         Args:
             context (List[str]): List of context strings that form the basis of the prompt.
             instruction (str, optional): Additional instruction text to be included in the prompt. Default is an empty string.
@@ -545,14 +608,15 @@
                 reorder_context=reorder_context,
                 dynamic_context_compression_ratio=dynamic_context_compression_ratio,
                 rank_method=rank_method,
                 context_budget=context_budget,
                 context_segs=context_segs,
                 context_segs_rate=context_segs_rate,
                 context_segs_compress=context_segs_compress,
+                strict_preserve_uncompressed=strict_preserve_uncompressed,
             )
             if context_segs is not None:
                 context_segs = [context_segs[idx] for idx in context_used]
                 context_segs_rate = [context_segs_rate[idx] for idx in context_used]
                 context_segs_compress = [
                     context_segs_compress[idx] for idx in context_used
                 ]
@@ -1117,31 +1181,32 @@
         reorder_context: str = "original",
         dynamic_context_compression_ratio: float = 0.0,
         rank_method: str = "longllmlingua",
         context_budget: str = "+100",
         context_segs: List[List[str]] = None,
         context_segs_rate: List[List[float]] = None,
         context_segs_compress: List[List[bool]] = None,
+        strict_preserve_uncompressed: bool = True,
     ):
         demostrations_sort = self.get_rank_results(
             context,
             question,
             rank_method,
             condition_in_question,
             context_tokens_length,
         )
 
         if target_token < 0:
             target_token = 100
         target_token = eval("target_token" + context_budget)
         res = []
         used = force_context_ids if force_context_ids is not None else []
-        if context_segs is not None:
+        if context_segs is not None and strict_preserve_uncompressed:
             for idx, _ in enumerate(context):
-                if False in context_segs_compress[idx]:
+                if False in context_segs_compress[idx] and idx not in used:
                     used.append(idx)
 
         self.context_idxs.append([x for idx, (x, _) in enumerate(demostrations_sort)])
         for idx, _ in demostrations_sort:
             if idx >= len(context_tokens_length):
                 continue
             target_token -= context_tokens_length[idx]
@@ -2159,25 +2224,27 @@
                 context_probs[-1].extend(chunk_probs[prev_idx + i])
                 context_words[-1].extend(chunk_words[prev_idx + i])
             prev_idx = prev_idx + n_chunk
         context_probs = [sum(probs) / len(probs) for probs in context_probs]
         return context_probs, context_words
 
     def __chunk_context(self, origin_text, chunk_end_tokens):
+        # leave 2 token for CLS and SEP
+        max_len = self.max_seq_len - 2
         origin_list = []
         origin_tokens = self.tokenizer.tokenize(origin_text)
         n = len(origin_tokens)
         st = 0
         while st < n:
-            if st + self.max_seq_len > n - 1:
+            if st + max_len > n - 1:
                 chunk = self.tokenizer.convert_tokens_to_string(origin_tokens[st:n])
                 origin_list.append(chunk)
                 break
             else:
-                ed = st + self.max_seq_len
+                ed = st + max_len
                 for j in range(0, ed - st):
                     if origin_tokens[ed - j] in chunk_end_tokens:
                         ed = ed - j
                         break
                 chunk = self.tokenizer.convert_tokens_to_string(
                     origin_tokens[st : ed + 1]
                 )
@@ -2336,16 +2403,18 @@
                     threshold = np.percentile(
                         new_token_probs, int(100 * reduce_rate + 1)
                     )
 
                     keep_words = []
                     word_labels = []
                     assert len(words) == len(word_probs)
-                    for word, word_porb in zip(words, word_probs):
-                        if word_porb > threshold:
+                    for word, word_prob in zip(words, word_probs):
+                        if word_prob > threshold or (
+                            threshold == 1.0 and word_prob == threshold
+                        ):
                             if (
                                 drop_consecutive
                                 and word in force_tokens
                                 and len(keep_words) > 0
                                 and keep_words[-1] == word
                             ):
                                 word_labels.append(0)
```

### Comparing `llmlingua-0.2.1/llmlingua.egg-info/PKG-INFO` & `llmlingua-0.2.2/llmlingua.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmlingua
-Version: 0.2.1
+Version: 0.2.2
 Summary: To speed up LLMs' inference and enhance LLM's perceive of key information, compress the prompt and KV-Cache, which achieves up to 20x compression with minimal performance loss.
 Home-page: https://github.com/microsoft/LLMLingua
 Author: The LLMLingua team
 Author-email: hjiang@microsoft.com
 License: MIT License
 Keywords: Prompt Compression,LLMs,Inference Acceleration,Black-box LLMs,Efficient LLMs
 Classifier: Intended Audience :: Science/Research
@@ -57,15 +57,15 @@
 LongLLMLingua mitigates the 'lost in the middle' issue in LLMs, enhancing long-context information processing. It reduces costs and boosts efficiency with prompt compression, improving RAG performance by up to 21.4% using only 1/4 of the tokens.
 
 - [LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) (ICLR ME-FoMo 2024)<br>
   _Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing Yang and Lili Qiu_
 
 LLMLingua-2, a small-size yet powerful prompt compression method trained via data distillation from GPT-4 for token classification with a BERT-level encoder, excels in task-agnostic compression. It surpasses LLMLingua in handling out-of-domain data, offering 3x-6x faster performance.
 
-- [LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)<br>
+- [LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)<br>
   _Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang, Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu, Dongmei Zhang_
 
 ## 🎥 Overview
 
 ![Background](./images/LLMLingua_motivation.png)
 
 - Ever encountered the token limit when asking ChatGPT to summarize lengthy texts?
@@ -120,15 +120,15 @@
     volume = "abs/2310.06839",
     year = "2023",
 }
 ```
 
 ```bibtex
 @article{wu2024llmlingua2,
-    title = "{LLML}ingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression",
+    title = "{LLML}ingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt Compression",
     author = "Zhuoshi Pan and Qianhui Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang and Qingwei Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky Zhao and Lili Qiu and Dongmei Zhang",
     url = "https://arxiv.org/abs/2403.12968",
     journal = "ArXiv preprint",
     volume = "abs/2403.12968",
     year = "2024",
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: llmlingua Version: 0.2.1 Summary: To speed up LLMs'
+Metadata-Version: 2.1 Name: llmlingua Version: 0.2.2 Summary: To speed up LLMs'
 inference and enhance LLM's perceive of key information, compress the prompt
 and KV-Cache, which achieves up to 20x compression with minimal performance
 loss. Home-page: https://github.com/microsoft/LLMLingua Author: The LLMLingua
 team Author-email: hjiang@microsoft.com License: MIT License Keywords: Prompt
 Compression,LLMs,Inference Acceleration,Black-box LLMs,Efficient LLMs
 Classifier: Intended Audience :: Science/Research Classifier: Development
 Status :: 3 - Alpha Classifier: Programming Language :: Python :: 3 Classifier:
@@ -54,16 +54,16 @@
 Scenarios via Prompt Compression](https://arxiv.org/abs/2310.06839) (ICLR ME-
 FoMo 2024)
 _Huiqiang Jiang, Qianhui Wu, Xufang Luo, Dongsheng Li, Chin-Yew Lin, Yuqing
 Yang and Lili Qiu_ LLMLingua-2, a small-size yet powerful prompt compression
 method trained via data distillation from GPT-4 for token classification with a
 BERT-level encoder, excels in task-agnostic compression. It surpasses LLMLingua
 in handling out-of-domain data, offering 3x-6x faster performance. -
-[LLMLingua-2: Context-Aware Data Distillation for Efficient and Faithful Task-
-Agnostic Prompt Compression](https://arxiv.org/abs/2403.12968) (Under Review)
+[LLMLingua-2: Data Distillation for Efficient and Faithful Task-Agnostic Prompt
+Compression](https://arxiv.org/abs/2403.12968) (Under Review)
 _Zhuoshi Pan, Qianhui Wu, Huiqiang Jiang, Menglin Xia, Xufang Luo, Jue Zhang,
 Qingwei Lin, Victor Ruhle, Yuqing Yang, Chin-Yew Lin, H. Vicky Zhao, Lili Qiu,
 Dongmei Zhang_ ## ð¥ Overview ![Background](./images/
 LLMLingua_motivation.png) - Ever encountered the token limit when asking
 ChatGPT to summarize lengthy texts? - Frustrated with ChatGPT forgetting
 previous instructions after extensive fine-tuning? - Experienced high costs
 using GPT3.5/4 API for experiments despite excellent results? While Large
@@ -93,48 +93,47 @@
 "https://aclanthology.org/2023.emnlp-main.825", doi = "10.18653/v1/2023.emnlp-
 main.825", pages = "13358--13376", } ``` ```bibtex @article{jiang-etal-2023-
 longllmlingua, title = "{L}ong{LLML}ingua: Accelerating and Enhancing LLMs in
 Long Context Scenarios via Prompt Compression", author = "Huiqiang Jiang and
 Qianhui Wu and and Xufang Luo and Dongsheng Li and Chin-Yew Lin and Yuqing Yang
 and Lili Qiu", url = "https://arxiv.org/abs/2310.06839", journal = "ArXiv
 preprint", volume = "abs/2310.06839", year = "2023", } ``` ```bibtex @article
-{wu2024llmlingua2, title = "{LLML}ingua-2: Context-Aware Data Distillation for
-Efficient and Faithful Task-Agnostic Prompt Compression", author = "Zhuoshi Pan
-and Qianhui Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang
-and Qingwei Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky
-Zhao and Lili Qiu and Dongmei Zhang", url = "https://arxiv.org/abs/2403.12968",
-journal = "ArXiv preprint", volume = "abs/2403.12968", year = "2024", } ``` ##
-ð¯ Quick Start #### 1. **Installing LLMLingua:** To get started with
-LLMLingua, simply install it using pip: ```bash pip install llmlingua ``` ####
-2. **Using LLMLingua Series Methods for Prompt Compression:** With
-**LLMLingua**, you can easily compress your prompts. Hereâs how you can do
-it: ```python from llmlingua import PromptCompressor llm_lingua =
-PromptCompressor() compressed_prompt = llm_lingua.compress_prompt(prompt,
-instruction="", question="", target_token=200) # > {'compressed_prompt':
-'Question: Sam bought a dozen boxes, each with 30 highlighter pens inside, for
-$10 each box. He reanged five of boxes into packages of sixlters each and sold
-them $3 per. He sold the rest theters separately at the of three pens $2. How
-much did make in total, dollars?\nLets think step step\nSam bought 1 boxes x00
-oflters.\nHe bought 12 * 300ters in total\nSam then took 5 boxes
-6ters0ters.\nHe sold these boxes for 5 *5\nAfterelling these boxes there were
-3030 highlighters remaining.\nThese form 330 / 3 = 110 groups of three
-pens.\nHe sold each of these groups for $2 each, so made 110 * 2 = $220 from
-them.\nIn total, then, he earned $220 + $15 = $235.\nSince his original cost
-was $120, he earned $235 - $120 = $115 in profit.\nThe answer is 115', #
-'origin_tokens': 2365, # 'compressed_tokens': 211, # 'ratio': '11.2x', #
-'saving': ', Saving $0.1 in GPT-4.'} ## Or use the phi-2 model, llm_lingua =
-PromptCompressor("microsoft/phi-2") ## Or use the quantation model, like
-TheBloke/Llama-2-7b-Chat-GPTQ, only need <8GB GPU memory. ## Before that, you
-need to pip install optimum auto-gptq llm_lingua = PromptCompressor("TheBloke/
-Llama-2-7b-Chat-GPTQ", model_config={"revision": "main"}) ``` To try
-**LongLLMLingua** in your scenorias, you can use ```python from llmlingua
-import PromptCompressor llm_lingua = PromptCompressor() compressed_prompt =
-llm_lingua.compress_prompt( prompt_list, question=question, ratio=0.55, # Set
-the special parameter for LongLLMLingua
-condition_in_question="after_condition", reorder_context="sort",
+{wu2024llmlingua2, title = "{LLML}ingua-2: Data Distillation for Efficient and
+Faithful Task-Agnostic Prompt Compression", author = "Zhuoshi Pan and Qianhui
+Wu and Huiqiang Jiang and Menglin Xia and Xufang Luo and Jue Zhang and Qingwei
+Lin and Victor Ruhle and Yuqing Yang and Chin-Yew Lin and H. Vicky Zhao and
+Lili Qiu and Dongmei Zhang", url = "https://arxiv.org/abs/2403.12968", journal
+= "ArXiv preprint", volume = "abs/2403.12968", year = "2024", } ``` ## ð¯
+Quick Start #### 1. **Installing LLMLingua:** To get started with LLMLingua,
+simply install it using pip: ```bash pip install llmlingua ``` #### 2. **Using
+LLMLingua Series Methods for Prompt Compression:** With **LLMLingua**, you can
+easily compress your prompts. Hereâs how you can do it: ```python from
+llmlingua import PromptCompressor llm_lingua = PromptCompressor()
+compressed_prompt = llm_lingua.compress_prompt(prompt, instruction="",
+question="", target_token=200) # > {'compressed_prompt': 'Question: Sam bought
+a dozen boxes, each with 30 highlighter pens inside, for $10 each box. He
+reanged five of boxes into packages of sixlters each and sold them $3 per. He
+sold the rest theters separately at the of three pens $2. How much did make in
+total, dollars?\nLets think step step\nSam bought 1 boxes x00 oflters.\nHe
+bought 12 * 300ters in total\nSam then took 5 boxes 6ters0ters.\nHe sold these
+boxes for 5 *5\nAfterelling these boxes there were 3030 highlighters
+remaining.\nThese form 330 / 3 = 110 groups of three pens.\nHe sold each of
+these groups for $2 each, so made 110 * 2 = $220 from them.\nIn total, then, he
+earned $220 + $15 = $235.\nSince his original cost was $120, he earned $235 -
+$120 = $115 in profit.\nThe answer is 115', # 'origin_tokens': 2365, #
+'compressed_tokens': 211, # 'ratio': '11.2x', # 'saving': ', Saving $0.1 in
+GPT-4.'} ## Or use the phi-2 model, llm_lingua = PromptCompressor("microsoft/
+phi-2") ## Or use the quantation model, like TheBloke/Llama-2-7b-Chat-GPTQ,
+only need <8GB GPU memory. ## Before that, you need to pip install optimum
+auto-gptq llm_lingua = PromptCompressor("TheBloke/Llama-2-7b-Chat-GPTQ",
+model_config={"revision": "main"}) ``` To try **LongLLMLingua** in your
+scenorias, you can use ```python from llmlingua import PromptCompressor
+llm_lingua = PromptCompressor() compressed_prompt = llm_lingua.compress_prompt
+( prompt_list, question=question, ratio=0.55, # Set the special parameter for
+LongLLMLingua condition_in_question="after_condition", reorder_context="sort",
 dynamic_context_compression_ratio=0.3, # or 0.4 condition_compare=True,
 context_budget="+100", rank_method="longllmlingua", ) ``` To try **LLMLingua-
 2** in your scenorias, you can use ```python from llmlingua import
 PromptCompressor llm_lingua = PromptCompressor( model_name="microsoft/
 llmlingua-2-xlm-roberta-large-meetingbank", use_llmlingua2=True, # Whether to
 use llmlingua-2 ) compressed_prompt = llm_lingua.compress_prompt(prompt,
 rate=0.33, force_tokens = ['\n', '?']) ## Or use LLMLingua-2-small model
```

### Comparing `llmlingua-0.2.1/setup.py` & `llmlingua-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `llmlingua-0.2.1/tests/test_llmlingua.py` & `llmlingua-0.2.2/tests/test_llmlingua.py`

 * *Files identical despite different names*

### Comparing `llmlingua-0.2.1/tests/test_llmlingua2.py` & `llmlingua-0.2.2/tests/test_llmlingua2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     COMPRESSED_MULTIPLE_CONTEXT_PROMPT = "John: So, I've been thinking about project believe we need to make changes. we want project to succeed, right? think we should consider maybe revising timeline."
 
     GSM8K_PROMPT = "Question: Angelo and Melanie want to plan how many hours over the next week they should study together for their test next week. They have 2 chapters of their textbook to study and 4 worksheets to memorize. They figure out that they should dedicate 3 hours to each chapter of their textbook and 1.5 hours for each worksheet. If they plan to study no more than 4 hours each day, how many days should they plan to study total over the next week if they take a 10-minute break every hour, include 3 10-minute snack breaks each day, and 30 minutes for lunch each day?\nLet's think step by step\nAngelo and Melanie think they should dedicate 3 hours to each of the 2 chapters, 3 hours x 2 chapters = 6 hours total.\nFor the worksheets they plan to dedicate 1.5 hours for each worksheet, 1.5 hours x 4 worksheets = 6 hours total.\nAngelo and Melanie need to start with planning 12 hours to study, at 4 hours a day, 12 / 4 = 3 days.\nHowever, they need to include time for breaks and lunch. Every hour they want to include a 10-minute break, so 12 total hours x 10 minutes = 120 extra minutes for breaks.\nThey also want to include 3 10-minute snack breaks, 3 x 10 minutes = 30 minutes.\nAnd they want to include 30 minutes for lunch each day, so 120 minutes for breaks + 30 minutes for snack breaks + 30 minutes for lunch = 180 minutes, or 180 / 60 minutes per hour = 3 extra hours.\nSo Angelo and Melanie want to plan 12 hours to study + 3 hours of breaks = 15 hours total.\nThey want to study no more than 4 hours each day, 15 hours / 4 hours each day = 3.75\nThey will need to plan to study 4 days to allow for all the time they need.\nThe answer is 4\n\nQuestion: You can buy 4 apples or 1 watermelon for the same price. You bought 36 fruits evenly split between oranges, apples and watermelons, and the price of 1 orange is $0.50. How much does 1 apple cost if your total bill was $66?\nLet's think step by step\nIf 36 fruits were evenly split between 3 types of fruits, then I bought 36/3 = 12 units of each fruit\nIf 1 orange costs $0.50 then 12 oranges will cost $0.50 * 12 = $6\nIf my total bill was $66 and I spent $6 on oranges then I spent $66 - $6 = $60 on the other 2 fruit types.\nAssuming the price of watermelon is W, and knowing that you can buy 4 apples for the same price and that the price of one apple is A, then 1W=4A\nIf we know we bought 12 watermelons and 12 apples for $60, then we know that $60 = 12W + 12A\nKnowing that 1W=4A, then we can convert the above to $60 = 12(4A) + 12A\n$60 = 48A + 12A\n$60 = 60A\nThen we know the price of one apple (A) is $60/60= $1\nThe answer is 1"
     GSM8K_150TOKENS_COMPRESSED_SINGLE_CONTEXT_PROMPT = "Question: Angelo Melanie plan test 2 chapters 4 worksheets 3 hours each chapter 1.5 hours each worksheet study 4 hours day how days 10-minute break every 3 10-minute snack breaks 30 minutes lunch\n\n dedicate 3 hours 2 chapters 3 2 = 6 hours total\n worksheets 1.5 hours each worksheet 1.5 4 = 6 hours total\n 12 hours study 4 hours a day 12 / 4 = 3 days\n breaks lunch 10-minute break 12 hours 10 = 120 minutes\n 3 10-minute snack breaks 3 10 = 30 minutes\n 30 minutes lunch 120 + 30 + 30 = 180 minutes 180 / 60 = 3 extra hours\n 12 hours study + 3 hours breaks = 15 hours total\n 4 hours each day 15 / 4 = 3.75\n 4 days\nThe answer is 4"
     GSM8K_150TOKENS_COMPRESSED_MULTIPLE_CONTEXT_PROMPT = "4 apples 1 watermelon 36 fruits oranges watermelons 1 orange $0.50 1 apple bill $66\n\n 36 fruits 3 36/3 = 12 units\n 1 orange $0.50 12 oranges $0.50 * 12 = $6\n total bill $66 spent $6 oranges $66 - $6 = $60 other 2\n watermelon W 4 apples one apple A 1W=4A\n 12 watermelons 12 apples $60 $60 = 12W + 12A\n $60 = 12(4A + 12A\n = 48A + 12A\n = 60A\n one apple $60/60= $1\nThe answer is 1"
 
     MEETINGBANK_PROMPT = "Item 28 Report from Development. Services Recommendation to declare ordinance amending the Land Use District Map from institutional to IRP 13 read and adopted as read District eight. Councilman Austin. So moved. Wonderful. And I want to ask Councilman Andrews so any member of the public that wishes to address item 28 saying none, members, cast your vote. Oh, I'm sorry, sir. I did not see you. Can we? I know this sounds picky and stupid. But this is an illogical motion because you haven't yet created ARP 13. By the way, unlike some other speakers, I will furnish you my name. I'm Joe Weinstein. I did speak last week. I do not like to come down here again to talk on the same subjects. But. There is a minor little matter. As to whether a. The proposed zoning is a good idea. And B, whether. The project, which it is intended. To permit. In fact. Meets the specifications of the zoning. I have not check that out, but someone else did raise that question and there may be some question as to whether all of the conditions of that zoning have, in fact, been met by the details of this project. This particular zoning, perhaps in the abstract, need not be a bad idea, but the way you see it realized in the project. Is not a very good idea. You could have the same density and more without destroying the usability, the usable green space that this design does. Because really, although it looks impressive from a top down view, it looks like you see plenty of green space between the buildings, that that space is pretty well wasted and useless because the buildings are high enough to pretty well shade and dominate the green space that's in that project. So I'm not saying that the density that you're going for is a bad thing. But doing it in this way doesn't work, and any zoning that just permits this without further control is not a good idea. Thank you. Okay. Thank you, sir. Members, please cast your vote. Councilman Andrew's motion carries. Next time, please. Report from Development Services recommendation to declare ordinance amending the Land Use District Map from institutional to park red and adopted as Red District eight."
-    MEETINGBANK_150TOKENS_COMPRESSED_SINGLE_CONTEXT_PROMPT = "Item 28 Report Development. Services declare ordinance amending Land Use District Map institutional IRP 13 adopted District eight. Councilman Austin. moved ask Councilman Andrews public address item 28 cast vote.?. illogical motion created ARP 13. Joe Weinstein. last week. subjects. minor matter. proposed zoning good idea. project. Meets specifications zoning. conditions zoning met details project. zoning not bad. not good. same density more without destroying green space. green space buildings wasted useless buildings shade dominate green space. not density bad. doesn't work zoning permits without control not good idea. Thank you. cast vote. Councilman Andrew's motion carries. Next time. Report Development Services declare ordinance amending Land Use District Map institutional to park red adopted District eight"
+    MEETINGBANK_150TOKENS_COMPRESSED_SINGLE_CONTEXT_PROMPT = "Item 28 Report Development. Services Recommendation declare ordinance amending Land Use District Map institutional IRP 13 adopted District eight. Councilman Austin. ask Councilman Andrews public address item 28 cast vote. see?. illogical motion created ARP 13. Joe Weinstein. last week. same subjects. minor matter. proposed zoning good idea. project intended. permit Meets specifications zoning. question conditions zoning met details project. zoning not bad project. not good. same density more without destroying usability green space. green space between buildings wasted useless buildings high shade dominate green space. not density bad. doesn't work zoning permits without control not good idea. Thank you. cast vote. Councilman Andrew's motion carries. Next time.Development Services ordinance Land District Map park District."
 
     LONGBENCH_PROMPT_LIST = [
         "新闻内容：\n（服务·健康）专家提醒：寒冷气候易诱发心脑血管疾病\n新华社海口２月９日专电（张苏民、李建国）海口市疾病预防控制中心专家介绍，持续的寒冷气候是心脑血管疾病的杀手，尤其患有高血压或高血脂疾病的老人更应做好防范，防止脑中风发生。\n　　在寒冷的气候环境当中要注意保暖，增添衣服，饮食以清淡为主，多食用蔬菜，忌暴食荤类。尤其过年时，切忌熬夜，平时要加强身体锻炼，劳逸结合。除此之外，冬季还是呼吸道传染病暴发和流行的季节，应该注意预防流感、麻疹、流脑、水痘等呼吸道传染病的发生。\n　　专家还指出，由于寒冷气候影响，人们习惯门窗紧闭，空气不对流，一旦有传染源传入，极容易造成疾病的暴发。春节期间，一些商场或公共娱乐场所人群密集，有关单位应加强通风。（完）\n类别：医药、卫生",
         "\n\n新闻内容：\n李明波在恩施调研时强调 大力推进基层党内民主建设\n本报讯　（记者吴畏、通讯员曾言、周恩祖）11日至13日，省委常委、秘书长李明波到恩施州调研基层党建工作时强调，要以增强党的创新活力、巩固党的团结统一为目标，以改革创新精神大力抓好基层党内民主建设。\n　　李明波视察了非公有制企业党建、党代表常任制、基层党务公开、以党内和谐推进社区和谐等党建工作现场，与基层党务工作者座谈。李明波强调，在新形势下，要把握好民主进程与经济社会发展、尊重党员主体地位与提高党员民主素质、履行党员民主权利与保证党的统一意志、发挥党员民主监督作用与加强党纪教育管理等的关系，进一步深入探索，在丰富形式、拓宽渠道、完善机制等方面取得更大成绩。\n类别：政治",
         "\n\n新闻内容：\n第38届世界贸易中心年会及经贸洽谈会\n第38届世界贸易中心年会将于2007年10月21至24日在美国路易斯\n安那州首府新奥尔良召开。该会由美国纽约世界贸易中心总部和美国贸\n易服务管理总局、新奥尔良世贸中心共同举办，届时将有来自60多个国\n家和地区的经贸代表团约600余人与会。天津贸促会与天津世贸中心协\n会将共同组织天津经贸代表团赴美国参加“世贸中心2007年年会及经贸\n洽谈会”。\n　　联系人：王岭　刘鹏\n　　电话：022－2520231725202123\n　　传真：022－25201975\n　　地址：天津经济技术开发区宏达街19号A区2楼\n类别：商业、外贸、海关",
         "\n\n新闻内容：\n（全运会）第十一届全运会开闭幕时间确定\n新华社济南６月５日体育专电（记者赵仁伟）第十一届全国运动会组委会５日在济南宣布，十一运会将于今年１０月１６日在济南奥体中心开幕，闭幕时间为１０月２８日。\n　　十一运会组委会常务副秘书长、山东省体育局局长张洪涛介绍，十一运会的比赛项目共设３３个大项、４３个分项、３６２个小项，其中包括２８个夏季奥运会项目、４个冬季项目以及武术项目。与２００５年十运会相比，大项增加了１个，即自由式滑雪；小项增加了５个，分别是自由式滑雪男子个人、女子个人，女子水球项目，足球男子１６岁以下组和女子１８岁以下组。\n　　在十一运会全部３６２个小项中，马拉松男、女２个小项的比赛在北京举办，速度滑冰４个小项、自由式滑雪２个小项的比赛分别在沈阳和长春举办，其余３５４个小项的比赛在山东省１７个赛区举行。其中，济南赛区共举办小项２１２个，青岛４８个，日照４０个，滨州２８个，枣庄８个，菏泽７个，威海５个，烟台、德州各３个；淄博、东营、潍坊、济宁、泰安、莱芜、临沂、聊城８个赛区只举办小组赛和第四名以后的比赛，不产生金牌。\n　　张洪涛介绍，十一运会冰雪项目已于１月至４月举行，占全部小项的４.４％。因部分夏季项目的世界锦标赛或国际重要赛事的时间与十一运会比赛时间冲突或相距较近，国家体育总局确定把这些项目的比赛安排在开幕式前举行，共有１５个项目、８０个小项，占全部小项的２２.１％。（完）\n类别：体育",
         "\n\n新闻内容：\n（教育）河北整顿公办初中、小学招收择校生\n（教育）河北整顿公办初中、小学招收择校生\n　　新华社石家庄３月１２日电（冯月静）记者从河北省教育纪检监察审计工作会议上了解到，从今年起，河北省不再审批新的改制学校。对已审批的改制学校进行一次全面整顿和规范，重点解决公办初中、小学以改制为名或以民办为名举办“校中校”“校中班”高收费问题。\n　　据了解，河北省规定达不到要求的，要限期整改；年内仍达不到标准要求的，一律停止招生。公办学校一律不准搞“一校两制”，更不准以改制为名高收费。\n　　同时，今年秋季新学年开始，设区市市区的公办省级示范性普通高中（含在县镇办学的市直属省级示范性高中）择校生比例最高限额由原定的４０％一律下调为３０％。严禁学校擅自扩大择校生招生比例、降低录取分数线、提高收费标准或在限定金额外加收任何其他费用。（完）\n类别：教育",
```

### Comparing `llmlingua-0.2.1/tests/test_longllmlingua.py` & `llmlingua-0.2.2/tests/test_longllmlingua.py`

 * *Files identical despite different names*

