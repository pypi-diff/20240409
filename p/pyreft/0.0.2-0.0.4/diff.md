# Comparing `tmp/pyreft-0.0.2.tar.gz` & `tmp/pyreft-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreft-0.0.2.tar", last modified: Sun Apr  7 23:17:48 2024, max compression
+gzip compressed data, was "pyreft-0.0.4.tar", last modified: Tue Apr  9 03:04:42 2024, max compression
```

## Comparing `pyreft-0.0.2.tar` & `pyreft-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:17:48.059512 pyreft-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 23:17:43.000000 pyreft-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 23:17:43.000000 pyreft-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-04-07 23:17:48.059512 pyreft-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-04-07 23:17:43.000000 pyreft-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:17:48.059512 pyreft-0.0.2/pyreft/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/interventions.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/reft_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/reft_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:17:48.059512 pyreft-0.0.2/pyreft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-07 23:17:43.000000 pyreft-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:17:48.059512 pyreft-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-07 23:17:43.000000 pyreft-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:04:42.373039 pyreft-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 03:04:38.000000 pyreft-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 03:04:38.000000 pyreft-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-09 03:04:42.373039 pyreft-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-04-09 03:04:38.000000 pyreft-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:04:42.369038 pyreft-0.0.4/pyreft/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/interventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/reft_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/reft_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 03:04:38.000000 pyreft-0.0.4/pyreft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:04:42.373039 pyreft-0.0.4/pyreft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-09 03:04:42.000000 pyreft-0.0.4/pyreft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 03:04:42.000000 pyreft-0.0.4/pyreft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:04:42.000000 pyreft-0.0.4/pyreft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 03:04:42.000000 pyreft-0.0.4/pyreft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 03:04:42.000000 pyreft-0.0.4/pyreft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 03:04:38.000000 pyreft-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 03:04:42.373039 pyreft-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-09 03:04:38.000000 pyreft-0.0.4/setup.py
```

### Comparing `pyreft-0.0.2/LICENSE` & `pyreft-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/PKG-INFO` & `pyreft-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 Metadata-Version: 2.1
 Name: pyreft
-Version: 0.0.2
+Version: 0.0.4
 Summary: REFT: Representation Finetuning for Language Models
-Home-page: https://github.com/stanfordnlp/reft
+Home-page: https://github.com/stanfordnlp/pyreft
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.2.1
+Requires-Dist: torch>=2.0.0
 Requires-Dist: flash-attn>=2.5.6
-Requires-Dist: transformers>=4.39.2
-Requires-Dist: pyvene>=0.0.8
-Requires-Dist: datasets>=2.16.1
+Requires-Dist: pyvene>=0.1.1
+Requires-Dist: transformers>=4.39.3
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: matplotlib>=3.7.4
-Requires-Dist: seaborn>=0.13.1
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub>=0.20.3
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: fsspec>=2023.6.0
-Requires-Dist: accelerate>=0.26.1
+Requires-Dist: accelerate>=0.29.1
 Requires-Dist: sentencepiece>=0.1.96
 Requires-Dist: evaluate>=0.4.1
+Requires-Dist: datasets>=2.18.0
 Requires-Dist: wandb
 Requires-Dist: scikit-learn
 Requires-Dist: jupyter
+Requires-Dist: fsspec>=2024.2.0
+Requires-Dist: ydata-profiling>=4.7.0
+Requires-Dist: seaborn==0.12.2
+Requires-Dist: gcsfs>=2024.2.0
 
 <h1 align="center"> <p>pyreft<sub> by <a href="https://github.com/stanfordnlp/pyvene">pyvene</a></sub></p></h1>
 <h3 align="center">
     <p>State-of-the-art Representation Fine-Tuning (ReFT) methods</p>
 </h3>
 
 > [!WARNING]
 > **Hey hey! Corrections to the preprint:** We or members of the community have identified a few typos.
+> 
+> - (1) Hyperparameter settings presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the one where we apply interventions to all layers. We release our training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) folder, check those to reproduce for now!
+> - (2) Wrong UltraLM citation, will correct that.
+> - (3) Commonsense170K is not 100 times larger than GSM8K :) (170/8).
+> 
+> We will update our arXiv paper on Monday (April 8th, 2024). Sorry guys! Till then, happy ReFTing!
 
-- (1) Hyperparameter settings presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the one where we apply interventions to all layers. We release our training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) folder, check those to reproduce for now!
-- (2) Wrong UltraLM citation, will correct that.
-- (3) Commonsense170K is not 100 times larger than GSM8K :) (170/8).
+# A _Powerful_, _Parameter-Efficient_, and _Interpretable_ fine-tuning method
+Want to try a fine-tuning method that uses a fraction of the parameter count of SoTA PEFTs, while achieving potentially better performance? Introducing **`pyreft`**, a **representation fine-tuning (ReFT)** library that supports adapting internal language model representations via trainable interventions. With fewer fine-tuning parameters and more robust performance, **`pyreft`** can boost fine-tuning efficiency, decrease fine-tuning cost, while opening the doors to study the interpretability of adapting parameters.
 
-We will update our arXiv paper on Monday (April 8th, 2024). Sorry guys! Till then, happy ReFTing!
-
-# A _Powerful_, _Parameter-Efficient_, and _Interpretable_ way of fine-tuning
-Want to try a fine-tuning method that uses a fraction of SoTA PEFT parameters count, while achieving potentially better performance? Introducing **pyreft**, a **representation fine-tuning (ReFT)** library that supports adapting internal language model representations via trainable interventions. With fewer fine-tuning parameters and more robust performance, **pyreft** can boost fine-tuning efficiency, decrease fine-tuning cost, while opening the doors to study the interpretability of adapting parameters.
-
-**pyreft** supports
+**`pyreft`** supports
 
 - Fine tuning any pretrained LMs on HuggingFace with ReFT
-
 - Setting ReFT hyperparameters via configs
-
 - Sharing the fine-tuned results easily to HuggingFace
 
 > [!TIP]
 > **Powerful and Parameter-Efficient:** Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of representation fine-tuning (ReFT) and its performance.
 
 > [!TIP]
 > **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the interpretable nature of ReFT.
 
 ## Quickstart
 
-Here is one verified conda env setup steps:
+Here is one verified `conda` env setup steps:
 
 ```bash
 conda create --name awesome-reft python=3.10
 conda activate awesome-reft
 ```
 
-Then, install **pyreft** from pip+git:
+Then, install **`pyreft`** from pip+git:
 
 ```bash
-pip install git+https://github.com/frankaging/pyreft.git
+pip install git+https://github.com/stanfordnlp/pyreft.git
 ```
 
-Or install **pyreft** from pip (coming soon):
+Or install **`pyreft`** from `pip` (coming soon):
 
 ```bash
 pip install pyreft
 ```
 
-Prepare a model for training with a ReFT method by wrapping the base model and ReFT configuration with `get_reft_model`. In the following example, we are using [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more parameter-efficient than the original LoReFT described in the paper:
+Prepare a model for training with a ReFT method by wrapping the base model and ReFT configuration with `get_reft_model`. In the following example, we are using [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is simpler than the original LoReFT described in the paper:
 
 ```python
 import torch
 import transformers
 
 from pyreft import (
     get_reft_model,
@@ -112,15 +112,15 @@
 reft_model = get_reft_model(model, reft_config)
 reft_model.print_trainable_parameters()
 
 "trainable intervention params: 4,097 || trainable model params: 0"
 "model params: 6,738,415,616 || trainable%: 6.080064266549391e-05"
 ```
 
-With this config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the `reft_model` can be used for any downstream tasks. We can see if we can do **rank-1 reft** to let the model to produce some **constant output**:
+With this config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the `reft_model` can be used for any downstream tasks. We can train a **rank-1 ReFT** to make the model produce some **constant output**:
 
 ```python
 from pyreft import (
     ReftTrainerForCausalLM,
     make_last_position_supervised_data_module
 )
 tokenizer = transformers.AutoTokenizer.from_pretrained(
@@ -179,17 +179,17 @@
 machine learning, practical applications of human language technology,
 and interdisciplinary work in computational social science and cognitive
 science. We also develop a wide variety of educational materials
 on NLP and many tools for the community to use, including the Stanza
 toolkit which processes text in over 60 human languages."""
 ```
 
-We successfully compress the text into 4,097 parameters! We perform more rigious memorisation test like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
+We successfully compress the text into 4,097 parameters! We perform more rigious memorisation tests like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
 
-You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
+You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps in [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
 
 ## Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace
 
 For full tutorial, please take a look at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb).
 
 Loading the base LM first:
 
@@ -253,34 +253,36 @@
 print(tokenizer.decode(reft_response[0], skip_special_tokens=True))
 ```
 Note that Llama-2 models can follow instructions zero-shot. We encourge people to try on other more primitive base LMs and see if ReFT can work well!
 
 **Usage and License Notices**: Our chat-model is intended and licensed for research use only. The model is CC BY NC 4.0 (allowing only non-commercial use) should not be used outside of research purposes. 
 
 
-## Why you should use ReFT as oppose to PEFT?
+## Why should you use ReFT instead of PEFTs?
+
+There are various benefits such as **saving memory** and **storage**. In addition to that, ReFT is more interpretable and extensible than PEFT. The interventions we are learning are simply a causal abstraction of the training task, without modifying any model weights. The intervention site search space is large, and can be at any set of token positions which is more flexible.
 
-There are various benefits such as saving memory and storage. In addition to that, ReFT is more interpretable and extensible than PEFT. The interventions we are learning is simply a causal abstraction of the task you are training without touching any model weights. The intervention site search space is large, and can be at any token position which is more flexibile. We showcase ReFT performance on various benchmarks against popular PEFT such as LoRA and its newer variants (e.g., DoRA) in our paper.
+We showcase ReFT performance on various benchmarks against popular PEFTs such as LoRA and its newer variants (e.g., DoRA) in our paper.
 
 ## Learn more through examples
 
 | Example | Description |
 |-|-|
-| [pyvene](https://github.com/stanfordnlp/pyvene) | The backbone of pyreft library |
+| [`pyvene`](https://github.com/stanfordnlp/pyvene) | The backbone of pyreft library |
 | [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) | Reproduce our ReFT paper main results |
 | [Alpaca](https://github.com/frankaging/pyreft/tree/main/examples/alpaca) | Instruction-tune LMs with ReFT |
 | [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation) | Some hints on why ReFT works |
 | [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) | Some why ReFT is an interpretable method |
 
 ## Citation
 Make sure you cite the **ReFT** paper:
 ```bibtex
 @article{wuandarora2024reft,
-  title={ReFT: Representation Finetuning for Language Models},
-  author={Wu, Zhengxuan* and Arora, Aryaman* and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
+  title={{ReFT}: Representation Finetuning for Language Models},
+  author={Wu, Zhengxuan and Arora, Aryaman and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
   booktitle={arXiv:2404.03592},
   url={arxiv.org/abs/2404.03592},
   year={2024}
 }
 ```
 
 And please cite the **pyvene** library paper as well:
```

#### html2text {}

```diff
@@ -1,74 +1,75 @@
-Metadata-Version: 2.1 Name: pyreft Version: 0.0.2 Summary: REFT: Representation
-Finetuning for Language Models Home-page: https://github.com/stanfordnlp/reft
+Metadata-Version: 2.1 Name: pyreft Version: 0.0.4 Summary: REFT: Representation
+Finetuning for Language Models Home-page: https://github.com/stanfordnlp/pyreft
 Author: Zhengxuan Wu Author-email: wuzhengx@stanford.edu License: Apache
 License 2.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch>=2.2.1
-Requires-Dist: flash-attn>=2.5.6 Requires-Dist: transformers>=4.39.2 Requires-
-Dist: pyvene>=0.0.8 Requires-Dist: datasets>=2.16.1 Requires-Dist:
-protobuf>=3.20.0 Requires-Dist: matplotlib>=3.7.4 Requires-Dist:
-seaborn>=0.13.1 Requires-Dist: ipywidgets>=8.1.1 Requires-Dist:
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch>=2.0.0
+Requires-Dist: flash-attn>=2.5.6 Requires-Dist: pyvene>=0.1.1 Requires-Dist:
+transformers>=4.39.3 Requires-Dist: protobuf>=3.20.0 Requires-Dist:
+matplotlib>=3.7.4 Requires-Dist: ipywidgets>=8.1.1 Requires-Dist:
 plotnine>=0.12.4 Requires-Dist: huggingface-hub>=0.20.3 Requires-Dist:
-numpy>=1.26.4 Requires-Dist: fsspec>=2023.6.0 Requires-Dist: accelerate>=0.26.1
-Requires-Dist: sentencepiece>=0.1.96 Requires-Dist: evaluate>=0.4.1 Requires-
-Dist: wandb Requires-Dist: scikit-learn Requires-Dist: jupyter
+numpy>=1.26.4 Requires-Dist: accelerate>=0.29.1 Requires-Dist:
+sentencepiece>=0.1.96 Requires-Dist: evaluate>=0.4.1 Requires-Dist:
+datasets>=2.18.0 Requires-Dist: wandb Requires-Dist: scikit-learn Requires-
+Dist: jupyter Requires-Dist: fsspec>=2024.2.0 Requires-Dist: ydata-
+profiling>=4.7.0 Requires-Dist: seaborn==0.12.2 Requires-Dist: gcsfs>=2024.2.0
                         ************ ppyyrreefftt bbyy _pp_yy_vv_ee_nn_ee ************
      ******** SSttaattee--ooff--tthhee--aarrtt RReepprreesseennttaattiioonn FFiinnee--TTuunniinngg ((RReeFFTT)) mmeetthhooddss ********
 > [!WARNING] > **Hey hey! Corrections to the preprint:** We or members of the
-community have identified a few typos. - (1) Hyperparameter settings presented
-in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the
-one where we apply interventions to all layers. We release our training wandb
-logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/
-loreft) folder, check those to reproduce for now! - (2) Wrong UltraLM citation,
-will correct that. - (3) Commonsense170K is not 100 times larger than GSM8K :)
-(170/8). We will update our arXiv paper on Monday (April 8th, 2024). Sorry
-guys! Till then, happy ReFTing! # A _Powerful_, _Parameter-Efficient_, and
-_Interpretable_ way of fine-tuning Want to try a fine-tuning method that uses a
-fraction of SoTA PEFT parameters count, while achieving potentially better
-performance? Introducing **pyreft**, a **representation fine-tuning (ReFT)**
-library that supports adapting internal language model representations via
-trainable interventions. With fewer fine-tuning parameters and more robust
-performance, **pyreft** can boost fine-tuning efficiency, decrease fine-tuning
-cost, while opening the doors to study the interpretability of adapting
-parameters. **pyreft** supports - Fine tuning any pretrained LMs on HuggingFace
-with ReFT - Setting ReFT hyperparameters via configs - Sharing the fine-tuned
-results easily to HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:**
-Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of
-representation fine-tuning (ReFT) and its performance. > [!TIP] >
-**Intepretable Finetuning:** Read [Composable ReFT](https://github.com/
-frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the
-interpretable nature of ReFT. ## Quickstart Here is one verified conda env
-setup steps: ```bash conda create --name awesome-reft python=3.10 conda
-activate awesome-reft ``` Then, install **pyreft** from pip+git: ```bash pip
-install git+https://github.com/frankaging/pyreft.git ``` Or install **pyreft**
-from pip (coming soon): ```bash pip install pyreft ``` Prepare a model for
-training with a ReFT method by wrapping the base model and ReFT configuration
-with `get_reft_model`. In the following example, we are using
-[`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/
-pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more
-parameter-efficient than the original LoReFT described in the paper: ```python
-import torch import transformers from pyreft import ( get_reft_model,
+community have identified a few typos. > > - (1) Hyperparameter settings
+presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K
+should be the one where we apply interventions to all layers. We release our
+training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/
+main/examples/loreft) folder, check those to reproduce for now! > - (2) Wrong
+UltraLM citation, will correct that. > - (3) Commonsense170K is not 100 times
+larger than GSM8K :) (170/8). > > We will update our arXiv paper on Monday
+(April 8th, 2024). Sorry guys! Till then, happy ReFTing! # A _Powerful_,
+_Parameter-Efficient_, and _Interpretable_ fine-tuning method Want to try a
+fine-tuning method that uses a fraction of the parameter count of SoTA PEFTs,
+while achieving potentially better performance? Introducing **`pyreft`**, a
+**representation fine-tuning (ReFT)** library that supports adapting internal
+language model representations via trainable interventions. With fewer fine-
+tuning parameters and more robust performance, **`pyreft`** can boost fine-
+tuning efficiency, decrease fine-tuning cost, while opening the doors to study
+the interpretability of adapting parameters. **`pyreft`** supports - Fine
+tuning any pretrained LMs on HuggingFace with ReFT - Setting ReFT
+hyperparameters via configs - Sharing the fine-tuned results easily to
+HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:** Read [Our ReFT
+paper](https://arxiv.org/abs/2404.03592) for an introduction of representation
+fine-tuning (ReFT) and its performance. > [!TIP] > **Intepretable Finetuning:**
+Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/
+composition) for a sneak-peek of the interpretable nature of ReFT. ##
+Quickstart Here is one verified `conda` env setup steps: ```bash conda create -
+-name awesome-reft python=3.10 conda activate awesome-reft ``` Then, install
+**`pyreft`** from pip+git: ```bash pip install git+https://github.com/
+stanfordnlp/pyreft.git ``` Or install **`pyreft`** from `pip` (coming soon):
+```bash pip install pyreft ``` Prepare a model for training with a ReFT method
+by wrapping the base model and ReFT configuration with `get_reft_model`. In the
+following example, we are using [`ConsreftIntervention`](https://github.com/
+stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT
+Intervention) which is simpler than the original LoReFT described in the paper:
+```python import torch import transformers from pyreft import ( get_reft_model,
 ReftConfig, ConsreftIntervention ) # loading huggingface model
 model_name_or_path = "yahma/llama-7b-hf" model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
 torch_dtype=torch.bfloat16, device_map="cuda") # wrap the model with rank-
 1 constant reft reft_config = ReftConfig(representations={"layer": 15,
 "component": "block_output", "intervention": ConsreftIntervention
 ( embed_dim=model.config.hidden_size, low_rank_dimension=1)}) reft_model =
 get_reft_model(model, reft_config) reft_model.print_trainable_parameters()
 "trainable intervention params: 4,097 || trainable model params: 0" "model
 params: 6,738,415,616 || trainable%: 6.080064266549391e-05" ``` With this
 config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the
-`reft_model` can be used for any downstream tasks. We can see if we can do
-**rank-1 reft** to let the model to produce some **constant output**: ```python
-from pyreft import ( ReftTrainerForCausalLM,
+`reft_model` can be used for any downstream tasks. We can train a **rank-
+1 ReFT** to make the model produce some **constant output**: ```python from
+pyreft import ( ReftTrainerForCausalLM,
 make_last_position_supervised_data_module ) tokenizer =
 transformers.AutoTokenizer.from_pretrained( model_name_or_path,
 model_max_length=2048, padding_side="right", use_fast=False)
 tokenizer.pad_token = tokenizer.unk_token # get training data to train our
 intervention to remember the following sequence memo_sequence = """ Welcome to
 the Natural Language Processing Group at Stanford University! We are a
 passionate, inclusive group of students and faculty, postdocs and research
@@ -98,22 +99,22 @@
 that allow computers to process, generate, and understand human languages. Our
 interests are very broad, including basic scientific research on computational
 linguistics, machine learning, practical applications of human language
 technology, and interdisciplinary work in computational social science and
 cognitive science. We also develop a wide variety of educational materials on
 NLP and many tools for the community to use, including the Stanza toolkit which
 processes text in over 60 human languages.""" ``` We successfully compress the
-text into 4,097 parameters! We perform more rigious memorisation test like this
-one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/
-memorisation). You can do ReFT with any language modeling tasks or SFT. Check
-out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples)
-folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s.
-86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by
-following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/
-main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
+text into 4,097 parameters! We perform more rigious memorisation tests like
+this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/
+examples/memorisation). You can do ReFT with any language modeling tasks or
+SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/
+examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103
+(81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU +
+ReFT** by following steps in [`train.py`](https://github.com/frankaging/pyreft/
+blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
 dataset](https://arxiv.org/abs/2310.01377). ## Loading our 18 min-cooked
 `Loreft1k-Llama-2-7b-hf` from HuggingFace For full tutorial, please take a look
 at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/
 examples/chat/chat_model.ipynb). Loading the base LM first: ```py import torch,
 transformers from pyreft import ( ReftModel, get_intervention_locations )
 prompt_no_input_template = """Below is an instruction that \ describes a task.
 Write a response that appropriately \ completes the request. ### Instruction:
@@ -139,37 +140,37 @@
 no_repeat_ngram_size=5, repetition_penalty=1.1,
 eos_token_id=tokenizer.eos_token_id, early_stopping=True ) print
 (tokenizer.decode(reft_response[0], skip_special_tokens=True)) ``` Note that
 Llama-2 models can follow instructions zero-shot. We encourge people to try on
 other more primitive base LMs and see if ReFT can work well! **Usage and
 License Notices**: Our chat-model is intended and licensed for research use
 only. The model is CC BY NC 4.0 (allowing only non-commercial use) should not
-be used outside of research purposes. ## Why you should use ReFT as oppose to
-PEFT? There are various benefits such as saving memory and storage. In addition
-to that, ReFT is more interpretable and extensible than PEFT. The interventions
-we are learning is simply a causal abstraction of the task you are training
-without touching any model weights. The intervention site search space is
-large, and can be at any token position which is more flexibile. We showcase
-ReFT performance on various benchmarks against popular PEFT such as LoRA and
-its newer variants (e.g., DoRA) in our paper. ## Learn more through examples |
-Example | Description | |-|-| | [pyvene](https://github.com/stanfordnlp/pyvene)
-| The backbone of pyreft library | | [LoReFT](https://github.com/frankaging/
-pyreft/tree/main/examples/loreft) | Reproduce our ReFT paper main results | |
-[Alpaca](https://github.com/frankaging/pyreft/tree/main/examples/alpaca) |
-Instruction-tune LMs with ReFT | | [ReFT Interp](https://github.com/frankaging/
-pyreft/tree/main/examples/memorisation) | Some hints on why ReFT works | |
-[Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/
-composition) | Some why ReFT is an interpretable method | ## Citation Make sure
-you cite the **ReFT** paper: ```bibtex @article{wuandarora2024reft, title=
-{ReFT: Representation Finetuning for Language Models}, author={Wu, Zhengxuan*
-and Arora, Aryaman* and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and
-Manning, Christopher D. and Potts, Christopher}, booktitle={arXiv:2404.03592},
-url={arxiv.org/abs/2404.03592}, year={2024} } ``` And please cite the
-**pyvene** library paper as well: ```bibtex @article{wu2024pyvene, title=
-{pyvene: A Library for Understanding and Improving {P}y{T}orch Models via
-Interventions}, author={Wu, Zhengxuan and Geiger, Atticus and Arora, Aryaman
-and Huang, Jing and Wang, Zheng and Goodman, Noah D. and Manning, Christopher
-D. and Potts, Christopher}, booktitle={arXiv:2403.07809}, url={arxiv.org/abs/
-2403.07809}, year={2024} } ``` ## Outreach If you are interested in integrating
-this library into your workflow or in reimplementing it for improved
-efficiency, please feel free to contact us! We may have additional insights to
-share.
+be used outside of research purposes. ## Why should you use ReFT instead of
+PEFTs? There are various benefits such as **saving memory** and **storage**. In
+addition to that, ReFT is more interpretable and extensible than PEFT. The
+interventions we are learning are simply a causal abstraction of the training
+task, without modifying any model weights. The intervention site search space
+is large, and can be at any set of token positions which is more flexible. We
+showcase ReFT performance on various benchmarks against popular PEFTs such as
+LoRA and its newer variants (e.g., DoRA) in our paper. ## Learn more through
+examples | Example | Description | |-|-| | [`pyvene`](https://github.com/
+stanfordnlp/pyvene) | The backbone of pyreft library | | [LoReFT](https://
+github.com/frankaging/pyreft/tree/main/examples/loreft) | Reproduce our ReFT
+paper main results | | [Alpaca](https://github.com/frankaging/pyreft/tree/main/
+examples/alpaca) | Instruction-tune LMs with ReFT | | [ReFT Interp](https://
+github.com/frankaging/pyreft/tree/main/examples/memorisation) | Some hints on
+why ReFT works | | [Composable ReFT](https://github.com/frankaging/pyreft/tree/
+main/examples/composition) | Some why ReFT is an interpretable method | ##
+Citation Make sure you cite the **ReFT** paper: ```bibtex @article
+{wuandarora2024reft, title={{ReFT}: Representation Finetuning for Language
+Models}, author={Wu, Zhengxuan and Arora, Aryaman and Wang, Zheng and Geiger,
+Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
+booktitle={arXiv:2404.03592}, url={arxiv.org/abs/2404.03592}, year={2024} } ```
+And please cite the **pyvene** library paper as well: ```bibtex @article
+{wu2024pyvene, title={pyvene: A Library for Understanding and Improving {P}y
+{T}orch Models via Interventions}, author={Wu, Zhengxuan and Geiger, Atticus
+and Arora, Aryaman and Huang, Jing and Wang, Zheng and Goodman, Noah D. and
+Manning, Christopher D. and Potts, Christopher}, booktitle={arXiv:2403.07809},
+url={arxiv.org/abs/2403.07809}, year={2024} } ``` ## Outreach If you are
+interested in integrating this library into your workflow or in reimplementing
+it for improved efficiency, please feel free to contact us! We may have
+additional insights to share.
```

### Comparing `pyreft-0.0.2/README.md` & `pyreft-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 <h1 align="center"> <p>pyreft<sub> by <a href="https://github.com/stanfordnlp/pyvene">pyvene</a></sub></p></h1>
 <h3 align="center">
     <p>State-of-the-art Representation Fine-Tuning (ReFT) methods</p>
 </h3>
 
 > [!WARNING]
 > **Hey hey! Corrections to the preprint:** We or members of the community have identified a few typos.
+> 
+> - (1) Hyperparameter settings presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the one where we apply interventions to all layers. We release our training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) folder, check those to reproduce for now!
+> - (2) Wrong UltraLM citation, will correct that.
+> - (3) Commonsense170K is not 100 times larger than GSM8K :) (170/8).
+> 
+> We will update our arXiv paper on Monday (April 8th, 2024). Sorry guys! Till then, happy ReFTing!
 
-- (1) Hyperparameter settings presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the one where we apply interventions to all layers. We release our training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) folder, check those to reproduce for now!
-- (2) Wrong UltraLM citation, will correct that.
-- (3) Commonsense170K is not 100 times larger than GSM8K :) (170/8).
+# A _Powerful_, _Parameter-Efficient_, and _Interpretable_ fine-tuning method
+Want to try a fine-tuning method that uses a fraction of the parameter count of SoTA PEFTs, while achieving potentially better performance? Introducing **`pyreft`**, a **representation fine-tuning (ReFT)** library that supports adapting internal language model representations via trainable interventions. With fewer fine-tuning parameters and more robust performance, **`pyreft`** can boost fine-tuning efficiency, decrease fine-tuning cost, while opening the doors to study the interpretability of adapting parameters.
 
-We will update our arXiv paper on Monday (April 8th, 2024). Sorry guys! Till then, happy ReFTing!
-
-# A _Powerful_, _Parameter-Efficient_, and _Interpretable_ way of fine-tuning
-Want to try a fine-tuning method that uses a fraction of SoTA PEFT parameters count, while achieving potentially better performance? Introducing **pyreft**, a **representation fine-tuning (ReFT)** library that supports adapting internal language model representations via trainable interventions. With fewer fine-tuning parameters and more robust performance, **pyreft** can boost fine-tuning efficiency, decrease fine-tuning cost, while opening the doors to study the interpretability of adapting parameters.
-
-**pyreft** supports
+**`pyreft`** supports
 
 - Fine tuning any pretrained LMs on HuggingFace with ReFT
-
 - Setting ReFT hyperparameters via configs
-
 - Sharing the fine-tuned results easily to HuggingFace
 
 > [!TIP]
 > **Powerful and Parameter-Efficient:** Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of representation fine-tuning (ReFT) and its performance.
 
 > [!TIP]
 > **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the interpretable nature of ReFT.
 
 ## Quickstart
 
-Here is one verified conda env setup steps:
+Here is one verified `conda` env setup steps:
 
 ```bash
 conda create --name awesome-reft python=3.10
 conda activate awesome-reft
 ```
 
-Then, install **pyreft** from pip+git:
+Then, install **`pyreft`** from pip+git:
 
 ```bash
-pip install git+https://github.com/frankaging/pyreft.git
+pip install git+https://github.com/stanfordnlp/pyreft.git
 ```
 
-Or install **pyreft** from pip (coming soon):
+Or install **`pyreft`** from `pip` (coming soon):
 
 ```bash
 pip install pyreft
 ```
 
-Prepare a model for training with a ReFT method by wrapping the base model and ReFT configuration with `get_reft_model`. In the following example, we are using [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more parameter-efficient than the original LoReFT described in the paper:
+Prepare a model for training with a ReFT method by wrapping the base model and ReFT configuration with `get_reft_model`. In the following example, we are using [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is simpler than the original LoReFT described in the paper:
 
 ```python
 import torch
 import transformers
 
 from pyreft import (
     get_reft_model,
@@ -74,15 +72,15 @@
 reft_model = get_reft_model(model, reft_config)
 reft_model.print_trainable_parameters()
 
 "trainable intervention params: 4,097 || trainable model params: 0"
 "model params: 6,738,415,616 || trainable%: 6.080064266549391e-05"
 ```
 
-With this config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the `reft_model` can be used for any downstream tasks. We can see if we can do **rank-1 reft** to let the model to produce some **constant output**:
+With this config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the `reft_model` can be used for any downstream tasks. We can train a **rank-1 ReFT** to make the model produce some **constant output**:
 
 ```python
 from pyreft import (
     ReftTrainerForCausalLM,
     make_last_position_supervised_data_module
 )
 tokenizer = transformers.AutoTokenizer.from_pretrained(
@@ -141,17 +139,17 @@
 machine learning, practical applications of human language technology,
 and interdisciplinary work in computational social science and cognitive
 science. We also develop a wide variety of educational materials
 on NLP and many tools for the community to use, including the Stanza
 toolkit which processes text in over 60 human languages."""
 ```
 
-We successfully compress the text into 4,097 parameters! We perform more rigious memorisation test like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
+We successfully compress the text into 4,097 parameters! We perform more rigious memorisation tests like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
 
-You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
+You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps in [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
 
 ## Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace
 
 For full tutorial, please take a look at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb).
 
 Loading the base LM first:
 
@@ -215,34 +213,36 @@
 print(tokenizer.decode(reft_response[0], skip_special_tokens=True))
 ```
 Note that Llama-2 models can follow instructions zero-shot. We encourge people to try on other more primitive base LMs and see if ReFT can work well!
 
 **Usage and License Notices**: Our chat-model is intended and licensed for research use only. The model is CC BY NC 4.0 (allowing only non-commercial use) should not be used outside of research purposes. 
 
 
-## Why you should use ReFT as oppose to PEFT?
+## Why should you use ReFT instead of PEFTs?
+
+There are various benefits such as **saving memory** and **storage**. In addition to that, ReFT is more interpretable and extensible than PEFT. The interventions we are learning are simply a causal abstraction of the training task, without modifying any model weights. The intervention site search space is large, and can be at any set of token positions which is more flexible.
 
-There are various benefits such as saving memory and storage. In addition to that, ReFT is more interpretable and extensible than PEFT. The interventions we are learning is simply a causal abstraction of the task you are training without touching any model weights. The intervention site search space is large, and can be at any token position which is more flexibile. We showcase ReFT performance on various benchmarks against popular PEFT such as LoRA and its newer variants (e.g., DoRA) in our paper.
+We showcase ReFT performance on various benchmarks against popular PEFTs such as LoRA and its newer variants (e.g., DoRA) in our paper.
 
 ## Learn more through examples
 
 | Example | Description |
 |-|-|
-| [pyvene](https://github.com/stanfordnlp/pyvene) | The backbone of pyreft library |
+| [`pyvene`](https://github.com/stanfordnlp/pyvene) | The backbone of pyreft library |
 | [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) | Reproduce our ReFT paper main results |
 | [Alpaca](https://github.com/frankaging/pyreft/tree/main/examples/alpaca) | Instruction-tune LMs with ReFT |
 | [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation) | Some hints on why ReFT works |
 | [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) | Some why ReFT is an interpretable method |
 
 ## Citation
 Make sure you cite the **ReFT** paper:
 ```bibtex
 @article{wuandarora2024reft,
-  title={ReFT: Representation Finetuning for Language Models},
-  author={Wu, Zhengxuan* and Arora, Aryaman* and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
+  title={{ReFT}: Representation Finetuning for Language Models},
+  author={Wu, Zhengxuan and Arora, Aryaman and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
   booktitle={arXiv:2404.03592},
   url={arxiv.org/abs/2404.03592},
   year={2024}
 }
 ```
 
 And please cite the **pyvene** library paper as well:
```

#### html2text {}

```diff
@@ -1,57 +1,57 @@
                         ************ ppyyrreefftt bbyy _pp_yy_vv_ee_nn_ee ************
      ******** SSttaattee--ooff--tthhee--aarrtt RReepprreesseennttaattiioonn FFiinnee--TTuunniinngg ((RReeFFTT)) mmeetthhooddss ********
 > [!WARNING] > **Hey hey! Corrections to the preprint:** We or members of the
-community have identified a few typos. - (1) Hyperparameter settings presented
-in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the
-one where we apply interventions to all layers. We release our training wandb
-logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/
-loreft) folder, check those to reproduce for now! - (2) Wrong UltraLM citation,
-will correct that. - (3) Commonsense170K is not 100 times larger than GSM8K :)
-(170/8). We will update our arXiv paper on Monday (April 8th, 2024). Sorry
-guys! Till then, happy ReFTing! # A _Powerful_, _Parameter-Efficient_, and
-_Interpretable_ way of fine-tuning Want to try a fine-tuning method that uses a
-fraction of SoTA PEFT parameters count, while achieving potentially better
-performance? Introducing **pyreft**, a **representation fine-tuning (ReFT)**
-library that supports adapting internal language model representations via
-trainable interventions. With fewer fine-tuning parameters and more robust
-performance, **pyreft** can boost fine-tuning efficiency, decrease fine-tuning
-cost, while opening the doors to study the interpretability of adapting
-parameters. **pyreft** supports - Fine tuning any pretrained LMs on HuggingFace
-with ReFT - Setting ReFT hyperparameters via configs - Sharing the fine-tuned
-results easily to HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:**
-Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of
-representation fine-tuning (ReFT) and its performance. > [!TIP] >
-**Intepretable Finetuning:** Read [Composable ReFT](https://github.com/
-frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the
-interpretable nature of ReFT. ## Quickstart Here is one verified conda env
-setup steps: ```bash conda create --name awesome-reft python=3.10 conda
-activate awesome-reft ``` Then, install **pyreft** from pip+git: ```bash pip
-install git+https://github.com/frankaging/pyreft.git ``` Or install **pyreft**
-from pip (coming soon): ```bash pip install pyreft ``` Prepare a model for
-training with a ReFT method by wrapping the base model and ReFT configuration
-with `get_reft_model`. In the following example, we are using
-[`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/
-pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more
-parameter-efficient than the original LoReFT described in the paper: ```python
-import torch import transformers from pyreft import ( get_reft_model,
+community have identified a few typos. > > - (1) Hyperparameter settings
+presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K
+should be the one where we apply interventions to all layers. We release our
+training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/
+main/examples/loreft) folder, check those to reproduce for now! > - (2) Wrong
+UltraLM citation, will correct that. > - (3) Commonsense170K is not 100 times
+larger than GSM8K :) (170/8). > > We will update our arXiv paper on Monday
+(April 8th, 2024). Sorry guys! Till then, happy ReFTing! # A _Powerful_,
+_Parameter-Efficient_, and _Interpretable_ fine-tuning method Want to try a
+fine-tuning method that uses a fraction of the parameter count of SoTA PEFTs,
+while achieving potentially better performance? Introducing **`pyreft`**, a
+**representation fine-tuning (ReFT)** library that supports adapting internal
+language model representations via trainable interventions. With fewer fine-
+tuning parameters and more robust performance, **`pyreft`** can boost fine-
+tuning efficiency, decrease fine-tuning cost, while opening the doors to study
+the interpretability of adapting parameters. **`pyreft`** supports - Fine
+tuning any pretrained LMs on HuggingFace with ReFT - Setting ReFT
+hyperparameters via configs - Sharing the fine-tuned results easily to
+HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:** Read [Our ReFT
+paper](https://arxiv.org/abs/2404.03592) for an introduction of representation
+fine-tuning (ReFT) and its performance. > [!TIP] > **Intepretable Finetuning:**
+Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/
+composition) for a sneak-peek of the interpretable nature of ReFT. ##
+Quickstart Here is one verified `conda` env setup steps: ```bash conda create -
+-name awesome-reft python=3.10 conda activate awesome-reft ``` Then, install
+**`pyreft`** from pip+git: ```bash pip install git+https://github.com/
+stanfordnlp/pyreft.git ``` Or install **`pyreft`** from `pip` (coming soon):
+```bash pip install pyreft ``` Prepare a model for training with a ReFT method
+by wrapping the base model and ReFT configuration with `get_reft_model`. In the
+following example, we are using [`ConsreftIntervention`](https://github.com/
+stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT
+Intervention) which is simpler than the original LoReFT described in the paper:
+```python import torch import transformers from pyreft import ( get_reft_model,
 ReftConfig, ConsreftIntervention ) # loading huggingface model
 model_name_or_path = "yahma/llama-7b-hf" model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
 torch_dtype=torch.bfloat16, device_map="cuda") # wrap the model with rank-
 1 constant reft reft_config = ReftConfig(representations={"layer": 15,
 "component": "block_output", "intervention": ConsreftIntervention
 ( embed_dim=model.config.hidden_size, low_rank_dimension=1)}) reft_model =
 get_reft_model(model, reft_config) reft_model.print_trainable_parameters()
 "trainable intervention params: 4,097 || trainable model params: 0" "model
 params: 6,738,415,616 || trainable%: 6.080064266549391e-05" ``` With this
 config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the
-`reft_model` can be used for any downstream tasks. We can see if we can do
-**rank-1 reft** to let the model to produce some **constant output**: ```python
-from pyreft import ( ReftTrainerForCausalLM,
+`reft_model` can be used for any downstream tasks. We can train a **rank-
+1 ReFT** to make the model produce some **constant output**: ```python from
+pyreft import ( ReftTrainerForCausalLM,
 make_last_position_supervised_data_module ) tokenizer =
 transformers.AutoTokenizer.from_pretrained( model_name_or_path,
 model_max_length=2048, padding_side="right", use_fast=False)
 tokenizer.pad_token = tokenizer.unk_token # get training data to train our
 intervention to remember the following sequence memo_sequence = """ Welcome to
 the Natural Language Processing Group at Stanford University! We are a
 passionate, inclusive group of students and faculty, postdocs and research
@@ -81,22 +81,22 @@
 that allow computers to process, generate, and understand human languages. Our
 interests are very broad, including basic scientific research on computational
 linguistics, machine learning, practical applications of human language
 technology, and interdisciplinary work in computational social science and
 cognitive science. We also develop a wide variety of educational materials on
 NLP and many tools for the community to use, including the Stanza toolkit which
 processes text in over 60 human languages.""" ``` We successfully compress the
-text into 4,097 parameters! We perform more rigious memorisation test like this
-one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/
-memorisation). You can do ReFT with any language modeling tasks or SFT. Check
-out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples)
-folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s.
-86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by
-following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/
-main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
+text into 4,097 parameters! We perform more rigious memorisation tests like
+this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/
+examples/memorisation). You can do ReFT with any language modeling tasks or
+SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/
+examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103
+(81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU +
+ReFT** by following steps in [`train.py`](https://github.com/frankaging/pyreft/
+blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
 dataset](https://arxiv.org/abs/2310.01377). ## Loading our 18 min-cooked
 `Loreft1k-Llama-2-7b-hf` from HuggingFace For full tutorial, please take a look
 at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/
 examples/chat/chat_model.ipynb). Loading the base LM first: ```py import torch,
 transformers from pyreft import ( ReftModel, get_intervention_locations )
 prompt_no_input_template = """Below is an instruction that \ describes a task.
 Write a response that appropriately \ completes the request. ### Instruction:
@@ -122,37 +122,37 @@
 no_repeat_ngram_size=5, repetition_penalty=1.1,
 eos_token_id=tokenizer.eos_token_id, early_stopping=True ) print
 (tokenizer.decode(reft_response[0], skip_special_tokens=True)) ``` Note that
 Llama-2 models can follow instructions zero-shot. We encourge people to try on
 other more primitive base LMs and see if ReFT can work well! **Usage and
 License Notices**: Our chat-model is intended and licensed for research use
 only. The model is CC BY NC 4.0 (allowing only non-commercial use) should not
-be used outside of research purposes. ## Why you should use ReFT as oppose to
-PEFT? There are various benefits such as saving memory and storage. In addition
-to that, ReFT is more interpretable and extensible than PEFT. The interventions
-we are learning is simply a causal abstraction of the task you are training
-without touching any model weights. The intervention site search space is
-large, and can be at any token position which is more flexibile. We showcase
-ReFT performance on various benchmarks against popular PEFT such as LoRA and
-its newer variants (e.g., DoRA) in our paper. ## Learn more through examples |
-Example | Description | |-|-| | [pyvene](https://github.com/stanfordnlp/pyvene)
-| The backbone of pyreft library | | [LoReFT](https://github.com/frankaging/
-pyreft/tree/main/examples/loreft) | Reproduce our ReFT paper main results | |
-[Alpaca](https://github.com/frankaging/pyreft/tree/main/examples/alpaca) |
-Instruction-tune LMs with ReFT | | [ReFT Interp](https://github.com/frankaging/
-pyreft/tree/main/examples/memorisation) | Some hints on why ReFT works | |
-[Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/
-composition) | Some why ReFT is an interpretable method | ## Citation Make sure
-you cite the **ReFT** paper: ```bibtex @article{wuandarora2024reft, title=
-{ReFT: Representation Finetuning for Language Models}, author={Wu, Zhengxuan*
-and Arora, Aryaman* and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and
-Manning, Christopher D. and Potts, Christopher}, booktitle={arXiv:2404.03592},
-url={arxiv.org/abs/2404.03592}, year={2024} } ``` And please cite the
-**pyvene** library paper as well: ```bibtex @article{wu2024pyvene, title=
-{pyvene: A Library for Understanding and Improving {P}y{T}orch Models via
-Interventions}, author={Wu, Zhengxuan and Geiger, Atticus and Arora, Aryaman
-and Huang, Jing and Wang, Zheng and Goodman, Noah D. and Manning, Christopher
-D. and Potts, Christopher}, booktitle={arXiv:2403.07809}, url={arxiv.org/abs/
-2403.07809}, year={2024} } ``` ## Outreach If you are interested in integrating
-this library into your workflow or in reimplementing it for improved
-efficiency, please feel free to contact us! We may have additional insights to
-share.
+be used outside of research purposes. ## Why should you use ReFT instead of
+PEFTs? There are various benefits such as **saving memory** and **storage**. In
+addition to that, ReFT is more interpretable and extensible than PEFT. The
+interventions we are learning are simply a causal abstraction of the training
+task, without modifying any model weights. The intervention site search space
+is large, and can be at any set of token positions which is more flexible. We
+showcase ReFT performance on various benchmarks against popular PEFTs such as
+LoRA and its newer variants (e.g., DoRA) in our paper. ## Learn more through
+examples | Example | Description | |-|-| | [`pyvene`](https://github.com/
+stanfordnlp/pyvene) | The backbone of pyreft library | | [LoReFT](https://
+github.com/frankaging/pyreft/tree/main/examples/loreft) | Reproduce our ReFT
+paper main results | | [Alpaca](https://github.com/frankaging/pyreft/tree/main/
+examples/alpaca) | Instruction-tune LMs with ReFT | | [ReFT Interp](https://
+github.com/frankaging/pyreft/tree/main/examples/memorisation) | Some hints on
+why ReFT works | | [Composable ReFT](https://github.com/frankaging/pyreft/tree/
+main/examples/composition) | Some why ReFT is an interpretable method | ##
+Citation Make sure you cite the **ReFT** paper: ```bibtex @article
+{wuandarora2024reft, title={{ReFT}: Representation Finetuning for Language
+Models}, author={Wu, Zhengxuan and Arora, Aryaman and Wang, Zheng and Geiger,
+Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
+booktitle={arXiv:2404.03592}, url={arxiv.org/abs/2404.03592}, year={2024} } ```
+And please cite the **pyvene** library paper as well: ```bibtex @article
+{wu2024pyvene, title={pyvene: A Library for Understanding and Improving {P}y
+{T}orch Models via Interventions}, author={Wu, Zhengxuan and Geiger, Atticus
+and Arora, Aryaman and Huang, Jing and Wang, Zheng and Goodman, Noah D. and
+Manning, Christopher D. and Potts, Christopher}, booktitle={arXiv:2403.07809},
+url={arxiv.org/abs/2403.07809}, year={2024} } ``` ## Outreach If you are
+interested in integrating this library into your workflow or in reimplementing
+it for improved efficiency, please feel free to contact us! We may have
+additional insights to share.
```

### Comparing `pyreft-0.0.2/pyreft/__init__.py` & `pyreft-0.0.4/pyreft/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/pyreft/dataset.py` & `pyreft-0.0.4/pyreft/dataset.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/pyreft/interventions.py` & `pyreft-0.0.4/pyreft/interventions.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/pyreft/reft_model.py` & `pyreft-0.0.4/pyreft/reft_model.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/pyreft/reft_trainer.py` & `pyreft-0.0.4/pyreft/reft_trainer.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/pyreft/utils.py` & `pyreft-0.0.4/pyreft/utils.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.2/pyreft.egg-info/PKG-INFO` & `pyreft-0.0.4/pyreft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 Metadata-Version: 2.1
 Name: pyreft
-Version: 0.0.2
+Version: 0.0.4
 Summary: REFT: Representation Finetuning for Language Models
-Home-page: https://github.com/stanfordnlp/reft
+Home-page: https://github.com/stanfordnlp/pyreft
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.2.1
+Requires-Dist: torch>=2.0.0
 Requires-Dist: flash-attn>=2.5.6
-Requires-Dist: transformers>=4.39.2
-Requires-Dist: pyvene>=0.0.8
-Requires-Dist: datasets>=2.16.1
+Requires-Dist: pyvene>=0.1.1
+Requires-Dist: transformers>=4.39.3
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: matplotlib>=3.7.4
-Requires-Dist: seaborn>=0.13.1
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub>=0.20.3
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: fsspec>=2023.6.0
-Requires-Dist: accelerate>=0.26.1
+Requires-Dist: accelerate>=0.29.1
 Requires-Dist: sentencepiece>=0.1.96
 Requires-Dist: evaluate>=0.4.1
+Requires-Dist: datasets>=2.18.0
 Requires-Dist: wandb
 Requires-Dist: scikit-learn
 Requires-Dist: jupyter
+Requires-Dist: fsspec>=2024.2.0
+Requires-Dist: ydata-profiling>=4.7.0
+Requires-Dist: seaborn==0.12.2
+Requires-Dist: gcsfs>=2024.2.0
 
 <h1 align="center"> <p>pyreft<sub> by <a href="https://github.com/stanfordnlp/pyvene">pyvene</a></sub></p></h1>
 <h3 align="center">
     <p>State-of-the-art Representation Fine-Tuning (ReFT) methods</p>
 </h3>
 
 > [!WARNING]
 > **Hey hey! Corrections to the preprint:** We or members of the community have identified a few typos.
+> 
+> - (1) Hyperparameter settings presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the one where we apply interventions to all layers. We release our training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) folder, check those to reproduce for now!
+> - (2) Wrong UltraLM citation, will correct that.
+> - (3) Commonsense170K is not 100 times larger than GSM8K :) (170/8).
+> 
+> We will update our arXiv paper on Monday (April 8th, 2024). Sorry guys! Till then, happy ReFTing!
 
-- (1) Hyperparameter settings presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the one where we apply interventions to all layers. We release our training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) folder, check those to reproduce for now!
-- (2) Wrong UltraLM citation, will correct that.
-- (3) Commonsense170K is not 100 times larger than GSM8K :) (170/8).
+# A _Powerful_, _Parameter-Efficient_, and _Interpretable_ fine-tuning method
+Want to try a fine-tuning method that uses a fraction of the parameter count of SoTA PEFTs, while achieving potentially better performance? Introducing **`pyreft`**, a **representation fine-tuning (ReFT)** library that supports adapting internal language model representations via trainable interventions. With fewer fine-tuning parameters and more robust performance, **`pyreft`** can boost fine-tuning efficiency, decrease fine-tuning cost, while opening the doors to study the interpretability of adapting parameters.
 
-We will update our arXiv paper on Monday (April 8th, 2024). Sorry guys! Till then, happy ReFTing!
-
-# A _Powerful_, _Parameter-Efficient_, and _Interpretable_ way of fine-tuning
-Want to try a fine-tuning method that uses a fraction of SoTA PEFT parameters count, while achieving potentially better performance? Introducing **pyreft**, a **representation fine-tuning (ReFT)** library that supports adapting internal language model representations via trainable interventions. With fewer fine-tuning parameters and more robust performance, **pyreft** can boost fine-tuning efficiency, decrease fine-tuning cost, while opening the doors to study the interpretability of adapting parameters.
-
-**pyreft** supports
+**`pyreft`** supports
 
 - Fine tuning any pretrained LMs on HuggingFace with ReFT
-
 - Setting ReFT hyperparameters via configs
-
 - Sharing the fine-tuned results easily to HuggingFace
 
 > [!TIP]
 > **Powerful and Parameter-Efficient:** Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of representation fine-tuning (ReFT) and its performance.
 
 > [!TIP]
 > **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the interpretable nature of ReFT.
 
 ## Quickstart
 
-Here is one verified conda env setup steps:
+Here is one verified `conda` env setup steps:
 
 ```bash
 conda create --name awesome-reft python=3.10
 conda activate awesome-reft
 ```
 
-Then, install **pyreft** from pip+git:
+Then, install **`pyreft`** from pip+git:
 
 ```bash
-pip install git+https://github.com/frankaging/pyreft.git
+pip install git+https://github.com/stanfordnlp/pyreft.git
 ```
 
-Or install **pyreft** from pip (coming soon):
+Or install **`pyreft`** from `pip` (coming soon):
 
 ```bash
 pip install pyreft
 ```
 
-Prepare a model for training with a ReFT method by wrapping the base model and ReFT configuration with `get_reft_model`. In the following example, we are using [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more parameter-efficient than the original LoReFT described in the paper:
+Prepare a model for training with a ReFT method by wrapping the base model and ReFT configuration with `get_reft_model`. In the following example, we are using [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is simpler than the original LoReFT described in the paper:
 
 ```python
 import torch
 import transformers
 
 from pyreft import (
     get_reft_model,
@@ -112,15 +112,15 @@
 reft_model = get_reft_model(model, reft_config)
 reft_model.print_trainable_parameters()
 
 "trainable intervention params: 4,097 || trainable model params: 0"
 "model params: 6,738,415,616 || trainable%: 6.080064266549391e-05"
 ```
 
-With this config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the `reft_model` can be used for any downstream tasks. We can see if we can do **rank-1 reft** to let the model to produce some **constant output**:
+With this config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the `reft_model` can be used for any downstream tasks. We can train a **rank-1 ReFT** to make the model produce some **constant output**:
 
 ```python
 from pyreft import (
     ReftTrainerForCausalLM,
     make_last_position_supervised_data_module
 )
 tokenizer = transformers.AutoTokenizer.from_pretrained(
@@ -179,17 +179,17 @@
 machine learning, practical applications of human language technology,
 and interdisciplinary work in computational social science and cognitive
 science. We also develop a wide variety of educational materials
 on NLP and many tools for the community to use, including the Stanza
 toolkit which processes text in over 60 human languages."""
 ```
 
-We successfully compress the text into 4,097 parameters! We perform more rigious memorisation test like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
+We successfully compress the text into 4,097 parameters! We perform more rigious memorisation tests like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
 
-You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
+You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps in [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
 
 ## Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace
 
 For full tutorial, please take a look at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb).
 
 Loading the base LM first:
 
@@ -253,34 +253,36 @@
 print(tokenizer.decode(reft_response[0], skip_special_tokens=True))
 ```
 Note that Llama-2 models can follow instructions zero-shot. We encourge people to try on other more primitive base LMs and see if ReFT can work well!
 
 **Usage and License Notices**: Our chat-model is intended and licensed for research use only. The model is CC BY NC 4.0 (allowing only non-commercial use) should not be used outside of research purposes. 
 
 
-## Why you should use ReFT as oppose to PEFT?
+## Why should you use ReFT instead of PEFTs?
+
+There are various benefits such as **saving memory** and **storage**. In addition to that, ReFT is more interpretable and extensible than PEFT. The interventions we are learning are simply a causal abstraction of the training task, without modifying any model weights. The intervention site search space is large, and can be at any set of token positions which is more flexible.
 
-There are various benefits such as saving memory and storage. In addition to that, ReFT is more interpretable and extensible than PEFT. The interventions we are learning is simply a causal abstraction of the task you are training without touching any model weights. The intervention site search space is large, and can be at any token position which is more flexibile. We showcase ReFT performance on various benchmarks against popular PEFT such as LoRA and its newer variants (e.g., DoRA) in our paper.
+We showcase ReFT performance on various benchmarks against popular PEFTs such as LoRA and its newer variants (e.g., DoRA) in our paper.
 
 ## Learn more through examples
 
 | Example | Description |
 |-|-|
-| [pyvene](https://github.com/stanfordnlp/pyvene) | The backbone of pyreft library |
+| [`pyvene`](https://github.com/stanfordnlp/pyvene) | The backbone of pyreft library |
 | [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/loreft) | Reproduce our ReFT paper main results |
 | [Alpaca](https://github.com/frankaging/pyreft/tree/main/examples/alpaca) | Instruction-tune LMs with ReFT |
 | [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation) | Some hints on why ReFT works |
 | [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) | Some why ReFT is an interpretable method |
 
 ## Citation
 Make sure you cite the **ReFT** paper:
 ```bibtex
 @article{wuandarora2024reft,
-  title={ReFT: Representation Finetuning for Language Models},
-  author={Wu, Zhengxuan* and Arora, Aryaman* and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
+  title={{ReFT}: Representation Finetuning for Language Models},
+  author={Wu, Zhengxuan and Arora, Aryaman and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
   booktitle={arXiv:2404.03592},
   url={arxiv.org/abs/2404.03592},
   year={2024}
 }
 ```
 
 And please cite the **pyvene** library paper as well:
```

#### html2text {}

```diff
@@ -1,74 +1,75 @@
-Metadata-Version: 2.1 Name: pyreft Version: 0.0.2 Summary: REFT: Representation
-Finetuning for Language Models Home-page: https://github.com/stanfordnlp/reft
+Metadata-Version: 2.1 Name: pyreft Version: 0.0.4 Summary: REFT: Representation
+Finetuning for Language Models Home-page: https://github.com/stanfordnlp/pyreft
 Author: Zhengxuan Wu Author-email: wuzhengx@stanford.edu License: Apache
 License 2.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch>=2.2.1
-Requires-Dist: flash-attn>=2.5.6 Requires-Dist: transformers>=4.39.2 Requires-
-Dist: pyvene>=0.0.8 Requires-Dist: datasets>=2.16.1 Requires-Dist:
-protobuf>=3.20.0 Requires-Dist: matplotlib>=3.7.4 Requires-Dist:
-seaborn>=0.13.1 Requires-Dist: ipywidgets>=8.1.1 Requires-Dist:
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch>=2.0.0
+Requires-Dist: flash-attn>=2.5.6 Requires-Dist: pyvene>=0.1.1 Requires-Dist:
+transformers>=4.39.3 Requires-Dist: protobuf>=3.20.0 Requires-Dist:
+matplotlib>=3.7.4 Requires-Dist: ipywidgets>=8.1.1 Requires-Dist:
 plotnine>=0.12.4 Requires-Dist: huggingface-hub>=0.20.3 Requires-Dist:
-numpy>=1.26.4 Requires-Dist: fsspec>=2023.6.0 Requires-Dist: accelerate>=0.26.1
-Requires-Dist: sentencepiece>=0.1.96 Requires-Dist: evaluate>=0.4.1 Requires-
-Dist: wandb Requires-Dist: scikit-learn Requires-Dist: jupyter
+numpy>=1.26.4 Requires-Dist: accelerate>=0.29.1 Requires-Dist:
+sentencepiece>=0.1.96 Requires-Dist: evaluate>=0.4.1 Requires-Dist:
+datasets>=2.18.0 Requires-Dist: wandb Requires-Dist: scikit-learn Requires-
+Dist: jupyter Requires-Dist: fsspec>=2024.2.0 Requires-Dist: ydata-
+profiling>=4.7.0 Requires-Dist: seaborn==0.12.2 Requires-Dist: gcsfs>=2024.2.0
                         ************ ppyyrreefftt bbyy _pp_yy_vv_ee_nn_ee ************
      ******** SSttaattee--ooff--tthhee--aarrtt RReepprreesseennttaattiioonn FFiinnee--TTuunniinngg ((RReeFFTT)) mmeetthhooddss ********
 > [!WARNING] > **Hey hey! Corrections to the preprint:** We or members of the
-community have identified a few typos. - (1) Hyperparameter settings presented
-in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the
-one where we apply interventions to all layers. We release our training wandb
-logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/
-loreft) folder, check those to reproduce for now! - (2) Wrong UltraLM citation,
-will correct that. - (3) Commonsense170K is not 100 times larger than GSM8K :)
-(170/8). We will update our arXiv paper on Monday (April 8th, 2024). Sorry
-guys! Till then, happy ReFTing! # A _Powerful_, _Parameter-Efficient_, and
-_Interpretable_ way of fine-tuning Want to try a fine-tuning method that uses a
-fraction of SoTA PEFT parameters count, while achieving potentially better
-performance? Introducing **pyreft**, a **representation fine-tuning (ReFT)**
-library that supports adapting internal language model representations via
-trainable interventions. With fewer fine-tuning parameters and more robust
-performance, **pyreft** can boost fine-tuning efficiency, decrease fine-tuning
-cost, while opening the doors to study the interpretability of adapting
-parameters. **pyreft** supports - Fine tuning any pretrained LMs on HuggingFace
-with ReFT - Setting ReFT hyperparameters via configs - Sharing the fine-tuned
-results easily to HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:**
-Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of
-representation fine-tuning (ReFT) and its performance. > [!TIP] >
-**Intepretable Finetuning:** Read [Composable ReFT](https://github.com/
-frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the
-interpretable nature of ReFT. ## Quickstart Here is one verified conda env
-setup steps: ```bash conda create --name awesome-reft python=3.10 conda
-activate awesome-reft ``` Then, install **pyreft** from pip+git: ```bash pip
-install git+https://github.com/frankaging/pyreft.git ``` Or install **pyreft**
-from pip (coming soon): ```bash pip install pyreft ``` Prepare a model for
-training with a ReFT method by wrapping the base model and ReFT configuration
-with `get_reft_model`. In the following example, we are using
-[`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/
-pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more
-parameter-efficient than the original LoReFT described in the paper: ```python
-import torch import transformers from pyreft import ( get_reft_model,
+community have identified a few typos. > > - (1) Hyperparameter settings
+presented in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K
+should be the one where we apply interventions to all layers. We release our
+training wandb logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/
+main/examples/loreft) folder, check those to reproduce for now! > - (2) Wrong
+UltraLM citation, will correct that. > - (3) Commonsense170K is not 100 times
+larger than GSM8K :) (170/8). > > We will update our arXiv paper on Monday
+(April 8th, 2024). Sorry guys! Till then, happy ReFTing! # A _Powerful_,
+_Parameter-Efficient_, and _Interpretable_ fine-tuning method Want to try a
+fine-tuning method that uses a fraction of the parameter count of SoTA PEFTs,
+while achieving potentially better performance? Introducing **`pyreft`**, a
+**representation fine-tuning (ReFT)** library that supports adapting internal
+language model representations via trainable interventions. With fewer fine-
+tuning parameters and more robust performance, **`pyreft`** can boost fine-
+tuning efficiency, decrease fine-tuning cost, while opening the doors to study
+the interpretability of adapting parameters. **`pyreft`** supports - Fine
+tuning any pretrained LMs on HuggingFace with ReFT - Setting ReFT
+hyperparameters via configs - Sharing the fine-tuned results easily to
+HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:** Read [Our ReFT
+paper](https://arxiv.org/abs/2404.03592) for an introduction of representation
+fine-tuning (ReFT) and its performance. > [!TIP] > **Intepretable Finetuning:**
+Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/
+composition) for a sneak-peek of the interpretable nature of ReFT. ##
+Quickstart Here is one verified `conda` env setup steps: ```bash conda create -
+-name awesome-reft python=3.10 conda activate awesome-reft ``` Then, install
+**`pyreft`** from pip+git: ```bash pip install git+https://github.com/
+stanfordnlp/pyreft.git ``` Or install **`pyreft`** from `pip` (coming soon):
+```bash pip install pyreft ``` Prepare a model for training with a ReFT method
+by wrapping the base model and ReFT configuration with `get_reft_model`. In the
+following example, we are using [`ConsreftIntervention`](https://github.com/
+stanfordnlp/pyreft/blob/main/pyreft/interventions.py#L85) (Constant LoReFT
+Intervention) which is simpler than the original LoReFT described in the paper:
+```python import torch import transformers from pyreft import ( get_reft_model,
 ReftConfig, ConsreftIntervention ) # loading huggingface model
 model_name_or_path = "yahma/llama-7b-hf" model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
 torch_dtype=torch.bfloat16, device_map="cuda") # wrap the model with rank-
 1 constant reft reft_config = ReftConfig(representations={"layer": 15,
 "component": "block_output", "intervention": ConsreftIntervention
 ( embed_dim=model.config.hidden_size, low_rank_dimension=1)}) reft_model =
 get_reft_model(model, reft_config) reft_model.print_trainable_parameters()
 "trainable intervention params: 4,097 || trainable model params: 0" "model
 params: 6,738,415,616 || trainable%: 6.080064266549391e-05" ``` With this
 config, yo are tuning `0.00006%` parameters, and 4,097 to be exact. Then, the
-`reft_model` can be used for any downstream tasks. We can see if we can do
-**rank-1 reft** to let the model to produce some **constant output**: ```python
-from pyreft import ( ReftTrainerForCausalLM,
+`reft_model` can be used for any downstream tasks. We can train a **rank-
+1 ReFT** to make the model produce some **constant output**: ```python from
+pyreft import ( ReftTrainerForCausalLM,
 make_last_position_supervised_data_module ) tokenizer =
 transformers.AutoTokenizer.from_pretrained( model_name_or_path,
 model_max_length=2048, padding_side="right", use_fast=False)
 tokenizer.pad_token = tokenizer.unk_token # get training data to train our
 intervention to remember the following sequence memo_sequence = """ Welcome to
 the Natural Language Processing Group at Stanford University! We are a
 passionate, inclusive group of students and faculty, postdocs and research
@@ -98,22 +99,22 @@
 that allow computers to process, generate, and understand human languages. Our
 interests are very broad, including basic scientific research on computational
 linguistics, machine learning, practical applications of human language
 technology, and interdisciplinary work in computational social science and
 cognitive science. We also develop a wide variety of educational materials on
 NLP and many tools for the community to use, including the Stanza toolkit which
 processes text in over 60 human languages.""" ``` We successfully compress the
-text into 4,097 parameters! We perform more rigious memorisation test like this
-one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/
-memorisation). You can do ReFT with any language modeling tasks or SFT. Check
-out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples)
-folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s.
-86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by
-following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/
-main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
+text into 4,097 parameters! We perform more rigious memorisation tests like
+this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/
+examples/memorisation). You can do ReFT with any language modeling tasks or
+SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/
+examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103
+(81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU +
+ReFT** by following steps in [`train.py`](https://github.com/frankaging/pyreft/
+blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
 dataset](https://arxiv.org/abs/2310.01377). ## Loading our 18 min-cooked
 `Loreft1k-Llama-2-7b-hf` from HuggingFace For full tutorial, please take a look
 at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/
 examples/chat/chat_model.ipynb). Loading the base LM first: ```py import torch,
 transformers from pyreft import ( ReftModel, get_intervention_locations )
 prompt_no_input_template = """Below is an instruction that \ describes a task.
 Write a response that appropriately \ completes the request. ### Instruction:
@@ -139,37 +140,37 @@
 no_repeat_ngram_size=5, repetition_penalty=1.1,
 eos_token_id=tokenizer.eos_token_id, early_stopping=True ) print
 (tokenizer.decode(reft_response[0], skip_special_tokens=True)) ``` Note that
 Llama-2 models can follow instructions zero-shot. We encourge people to try on
 other more primitive base LMs and see if ReFT can work well! **Usage and
 License Notices**: Our chat-model is intended and licensed for research use
 only. The model is CC BY NC 4.0 (allowing only non-commercial use) should not
-be used outside of research purposes. ## Why you should use ReFT as oppose to
-PEFT? There are various benefits such as saving memory and storage. In addition
-to that, ReFT is more interpretable and extensible than PEFT. The interventions
-we are learning is simply a causal abstraction of the task you are training
-without touching any model weights. The intervention site search space is
-large, and can be at any token position which is more flexibile. We showcase
-ReFT performance on various benchmarks against popular PEFT such as LoRA and
-its newer variants (e.g., DoRA) in our paper. ## Learn more through examples |
-Example | Description | |-|-| | [pyvene](https://github.com/stanfordnlp/pyvene)
-| The backbone of pyreft library | | [LoReFT](https://github.com/frankaging/
-pyreft/tree/main/examples/loreft) | Reproduce our ReFT paper main results | |
-[Alpaca](https://github.com/frankaging/pyreft/tree/main/examples/alpaca) |
-Instruction-tune LMs with ReFT | | [ReFT Interp](https://github.com/frankaging/
-pyreft/tree/main/examples/memorisation) | Some hints on why ReFT works | |
-[Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/
-composition) | Some why ReFT is an interpretable method | ## Citation Make sure
-you cite the **ReFT** paper: ```bibtex @article{wuandarora2024reft, title=
-{ReFT: Representation Finetuning for Language Models}, author={Wu, Zhengxuan*
-and Arora, Aryaman* and Wang, Zheng and Geiger, Atticus and Jurafsky, Dan and
-Manning, Christopher D. and Potts, Christopher}, booktitle={arXiv:2404.03592},
-url={arxiv.org/abs/2404.03592}, year={2024} } ``` And please cite the
-**pyvene** library paper as well: ```bibtex @article{wu2024pyvene, title=
-{pyvene: A Library for Understanding and Improving {P}y{T}orch Models via
-Interventions}, author={Wu, Zhengxuan and Geiger, Atticus and Arora, Aryaman
-and Huang, Jing and Wang, Zheng and Goodman, Noah D. and Manning, Christopher
-D. and Potts, Christopher}, booktitle={arXiv:2403.07809}, url={arxiv.org/abs/
-2403.07809}, year={2024} } ``` ## Outreach If you are interested in integrating
-this library into your workflow or in reimplementing it for improved
-efficiency, please feel free to contact us! We may have additional insights to
-share.
+be used outside of research purposes. ## Why should you use ReFT instead of
+PEFTs? There are various benefits such as **saving memory** and **storage**. In
+addition to that, ReFT is more interpretable and extensible than PEFT. The
+interventions we are learning are simply a causal abstraction of the training
+task, without modifying any model weights. The intervention site search space
+is large, and can be at any set of token positions which is more flexible. We
+showcase ReFT performance on various benchmarks against popular PEFTs such as
+LoRA and its newer variants (e.g., DoRA) in our paper. ## Learn more through
+examples | Example | Description | |-|-| | [`pyvene`](https://github.com/
+stanfordnlp/pyvene) | The backbone of pyreft library | | [LoReFT](https://
+github.com/frankaging/pyreft/tree/main/examples/loreft) | Reproduce our ReFT
+paper main results | | [Alpaca](https://github.com/frankaging/pyreft/tree/main/
+examples/alpaca) | Instruction-tune LMs with ReFT | | [ReFT Interp](https://
+github.com/frankaging/pyreft/tree/main/examples/memorisation) | Some hints on
+why ReFT works | | [Composable ReFT](https://github.com/frankaging/pyreft/tree/
+main/examples/composition) | Some why ReFT is an interpretable method | ##
+Citation Make sure you cite the **ReFT** paper: ```bibtex @article
+{wuandarora2024reft, title={{ReFT}: Representation Finetuning for Language
+Models}, author={Wu, Zhengxuan and Arora, Aryaman and Wang, Zheng and Geiger,
+Atticus and Jurafsky, Dan and Manning, Christopher D. and Potts, Christopher},
+booktitle={arXiv:2404.03592}, url={arxiv.org/abs/2404.03592}, year={2024} } ```
+And please cite the **pyvene** library paper as well: ```bibtex @article
+{wu2024pyvene, title={pyvene: A Library for Understanding and Improving {P}y
+{T}orch Models via Interventions}, author={Wu, Zhengxuan and Geiger, Atticus
+and Arora, Aryaman and Huang, Jing and Wang, Zheng and Goodman, Noah D. and
+Manning, Christopher D. and Potts, Christopher}, booktitle={arXiv:2403.07809},
+url={arxiv.org/abs/2403.07809}, year={2024} } ``` ## Outreach If you are
+interested in integrating this library into your workflow or in reimplementing
+it for improved efficiency, please feel free to contact us! We may have
+additional insights to share.
```

### Comparing `pyreft-0.0.2/setup.py` & `pyreft-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 # Read the content of the requirements.txt file
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyreft",
-    version="0.0.2",
+    version="0.0.4",
     description="REFT: Representation Finetuning for Language Models",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/stanfordnlp/reft",
+    url="https://github.com/stanfordnlp/pyreft",
     author="Zhengxuan Wu",
     author_email="wuzhengx@stanford.edu",
     license="Apache License 2.0",
     packages=find_packages(include=['pyreft', 'pyreft.*']),
     python_requires='>=3.8',
     install_requires=requirements,
     extras_require={},
```

