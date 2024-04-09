# Comparing `tmp/gliner-0.1.6.tar.gz` & `tmp/gliner-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-0.1.6.tar", last modified: Mon Apr  1 02:24:16 2024, max compression
+gzip compressed data, was "gliner-0.1.7.tar", last modified: Tue Apr  9 17:35:12 2024, max compression
```

## Comparing `gliner-0.1.6.tar` & `gliner-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-01 02:24:16.567112 gliner-0.1.6/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.6/LICENSE
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8296 2024-04-01 02:24:16.566872 gliner-0.1.6/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     7598 2024-04-01 02:23:01.000000 gliner-0.1.6/README.md
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-01 02:24:16.563964 gliner-0.1.6/gliner/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-01 02:24:12.000000 gliner-0.1.6/gliner/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 02:23:01.000000 gliner-0.1.6/gliner/model.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-01 02:24:16.566439 gliner-0.1.6/gliner/modules/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.6/gliner/modules/___init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5991 2024-03-27 06:05:29.000000 gliner-0.1.6/gliner/modules/base.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.6/gliner/modules/data_proc.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4804 2024-04-01 02:23:01.000000 gliner-0.1.6/gliner/modules/evaluator.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.6/gliner/modules/layers.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-03-12 13:03:35.000000 gliner-0.1.6/gliner/modules/run_evaluation.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.6/gliner/modules/span_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-03-12 13:03:35.000000 gliner-0.1.6/gliner/modules/token_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.6/gliner/modules/token_splitter.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-01 02:24:16.566638 gliner-0.1.6/gliner.egg-info/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8296 2024-04-01 02:24:16.000000 gliner-0.1.6/gliner.egg-info/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)      469 2024-04-01 02:24:16.000000 gliner-0.1.6/gliner.egg-info/SOURCES.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-01 02:24:16.000000 gliner-0.1.6/gliner.egg-info/dependency_links.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       85 2024-04-01 02:24:16.000000 gliner-0.1.6/gliner.egg-info/requires.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-01 02:24:16.000000 gliner-0.1.6/gliner.egg-info/top_level.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1026 2024-03-28 17:31:49.000000 gliner-0.1.6/pyproject.toml
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-01 02:24:16.567156 gliner-0.1.6/setup.cfg
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.239247 gliner-0.1.7/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.7/LICENSE
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9343 2024-04-09 17:35:12.238990 gliner-0.1.7/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8645 2024-04-09 17:32:05.000000 gliner-0.1.7/README.md
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.235698 gliner-0.1.7/gliner/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-03 11:51:52.000000 gliner-0.1.7/gliner/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 10:36:39.000000 gliner-0.1.7/gliner/model.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.238479 gliner-0.1.7/gliner/modules/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.7/gliner/modules/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5991 2024-04-01 10:36:39.000000 gliner-0.1.7/gliner/modules/base.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.7/gliner/modules/data_proc.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4805 2024-04-09 17:30:41.000000 gliner-0.1.7/gliner/modules/evaluator.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.7/gliner/modules/layers.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-04-09 17:30:19.000000 gliner-0.1.7/gliner/modules/run_evaluation.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.7/gliner/modules/span_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.1.7/gliner/modules/token_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.7/gliner/modules/token_splitter.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.238767 gliner-0.1.7/gliner.egg-info/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9343 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)      468 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/SOURCES.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/dependency_links.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       85 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/requires.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/top_level.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1026 2024-03-28 17:31:49.000000 gliner-0.1.7/pyproject.toml
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-09 17:35:12.239301 gliner-0.1.7/setup.cfg
```

### Comparing `gliner-0.1.6/LICENSE` & `gliner-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/PKG-INFO` & `gliner-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,79 @@
-Metadata-Version: 2.1
-Name: gliner
-Version: 0.1.6
-Summary: Generalist model for NER (Extract any entity types from texts)
-Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
-Maintainer: Urchade Zaratiana
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/urchade/GLiNER
-Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=2.0.0
-Requires-Dist: transformers>=4.38.2
-Requires-Dist: huggingface_hub>=0.21.4
-Requires-Dist: flair==0.13.1
-Requires-Dist: seqeval
-Requires-Dist: tqdm
-
-# GLiNER : Generalist and Lightweight model for Named Entity Recognition
+# 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
-* Paper is available on [Arxiv](https://arxiv.org/abs/2311.08526) (by Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois)
-* Demo on [HuggingFace](https://huggingface.co/spaces/tomaarsen/gliner_base)
-* Try it on [Google Colab](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
-
-<img src="demo.jpg" alt="Demo Image" width="50%"/>
+* **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
+* **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
+* **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage below.
-- `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
-- 📝 Finetuning notebook is available: examples/finetune.ipynb
-- 🗂 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) 📚 and [NuNER](https://huggingface.co/datasets/numind/NuNER) 📘 datasets.
-
-### Available Models on Hugging Face
-- [x] [GLiNER-Base](https://huggingface.co/urchade/gliner_base) (CC BY NC 4.0)
-- [x] [GLiNER-Multi](https://huggingface.co/urchade/gliner_multi) (CC BY NC 4.0)
-- [x] [GLiNER-Small](https://huggingface.co/urchade/gliner_small) (CC BY NC 4.0)
-- [x] [GLiNER-Small-v2](https://huggingface.co/urchade/gliner_smallv2) (Apache)
-- [x] [GLiNER-Medium](https://huggingface.co/urchade/gliner_medium) (CC BY NC 4.0)
-- [x] [GLiNER-Medium-v2](https://huggingface.co/urchade/gliner_mediumv2) (Apache)
-- [x] [GLiNER-Large](https://huggingface.co/urchade/gliner_large) (CC BY NC 4.0)
-- [x] [GLiNER-Large-v2](https://huggingface.co/urchade/gliner_largev2) (Apache)
-
-### To Release
-- [ ] ⏳ GLiNER-Multiv2
-- [ ] ⏳ GLiNER-Sup (trained on mixture of NER datasets)
+- **[08/04]** - Some pretrained weights contained a **bug** which caused performance degradation. For now use base or multi versions.
+- 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
+- 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
+- 🚀 `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
+- 📘 Finetuning notebook is available: examples/finetune.ipynb
+- 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
+
+### 🌟 Available Models on Hugging Face
+
+#### 🇬🇧 For English
+- **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
+- **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
+- **GLiNER Small v2**: `urchade/gliner_smallv2` *(Apache 2.0)*
+- **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
+- **GLiNER Medium v2**: `urchade/gliner_mediumv2` *(Apache 2.0)*
+- **GLiNER Medium v2.1**: `urchade/gliner_mediumv2.1` *(Apache 2.0)*
+- **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
+- **GLiNER Large v2**: `urchade/gliner_largev2` *(Apache 2.0)*
+
+#### 🌍 For Other Languages
+- **Korean**: 🇰🇷 `taeminlee/gliner_ko`
+- **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
+- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)*
 
-## Area of improvements / research
+#### 🔬 Domain Specific Models
+- **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
 
-- [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
-- [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
-- [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
-- [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
-- [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
-- [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
-- [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
-- [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
-- [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB)
-- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
+## 🛠 Installation & Usage
 
+To begin using the GLiNER model, first install the GLiNER Python library through pip:
 
-## Installation
-To use this model, you must install the GLiNER Python library:
-```
+```bash
 !pip install gliner
 ```
 
-## Usage
-Once you've downloaded the GLiNER library, you can import the GLiNER class. You can then load this model using `GLiNER.from_pretrained` and predict entities with `predict_entities`.
+### 🚀 Basic Use Case
+
+After the installation of the GLiNER library, import the `GLiNER` class. Following this, you can load your chosen model with `GLiNER.from_pretrained` and utilize `predict_entities` to discern entities within your text.
 
 ```python
 from gliner import GLiNER
 
+# Initialize GLiNER with the base model
 model = GLiNER.from_pretrained("urchade/gliner_base")
 
+# Sample text for entity prediction
 text = """
 Cristiano Ronaldo dos Santos Aveiro (Portuguese pronunciation: [kɾiʃˈtjɐnu ʁɔˈnaldu]; born 5 February 1985) is a Portuguese professional footballer who plays as a forward for and captains both Saudi Pro League club Al Nassr and the Portugal national team. Widely regarded as one of the greatest players of all time, Ronaldo has won five Ballon d'Or awards,[note 3] a record three UEFA Men's Player of the Year Awards, and four European Golden Shoes, the most by a European player. He has won 33 trophies in his career, including seven league titles, five UEFA Champions Leagues, the UEFA European Championship and the UEFA Nations League. Ronaldo holds the records for most appearances (183), goals (140) and assists (42) in the Champions League, goals in the European Championship (14), international goals (128) and international appearances (205). He is one of the few players to have made over 1,200 professional career appearances, the most by an outfield player, and has scored over 850 official senior career goals for club and country, making him the top goalscorer of all time.
 """
 
+# Labels for entity prediction
 labels = ["person", "award", "date", "competitions", "teams"]
 
+# Perform entity prediction
 entities = model.predict_entities(text, labels, threshold=0.5)
 
+# Display predicted entities and their labels
 for entity in entities:
     print(entity["text"], "=>", entity["label"])
 ```
 
-### Expected Output
+#### Expected Output
 
 ```
 Cristiano Ronaldo dos Santos Aveiro => person
 5 February 1985 => date
 Al Nassr => teams
 Portugal national team => teams
 Ballon d'Or => award
@@ -102,60 +82,92 @@
 UEFA Champions Leagues => competitions
 UEFA European Championship => competitions
 UEFA Nations League => competitions
 Champions League => competitions
 European Championship => competitions
 ```
 
-## Usage with spaCy
+### 🔌 Usage with spaCy
 
-You can also use GliNER with spaCy with the Gliner-spaCy library. To install it, you can use pip:
+GLiNER can be seamlessly integrated with spaCy. To begin, install the `gliner-spacy` library via pip:
 
 ```bash
 pip install gliner-spacy
 ```
-Once installed, you then load GliNER into a regular NLP pipeline. Here's an example using a blank English pipeline, but you can use any spaCy model.
+
+Following installation, you can add GLiNER to a spaCy NLP pipeline. Here's how to integrate it with a blank English pipeline; however, it's compatible with any spaCy model.
 
 ```python
 import spacy
 from gliner_spacy.pipeline import GlinerSpacy
 
-custom_spacy_config = { "gliner_model": "urchade/gliner_multi", "chunk_size": 250, "labels": ["people","company","punctuation"], "style": "ent" }
+# Configuration for GLiNER integration
+custom_spacy_config = {
+    "gliner_model": "urchade/gliner_multi",
+    "chunk_size": 250,
+    "labels": ["person", "organization", "email"],
+    "style": "ent",
+    "threshold": 0.3
+}
+
+# Initialize a blank English spaCy pipeline and add GLiNER
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
 
+# Example text for entity detection
 text = "This is a text about Bill Gates and Microsoft."
+
+# Process the text with the pipeline
 doc = nlp(text)
 
+# Output detected entities
 for ent in doc.ents:
     print(ent.text, ent.label_)
 ```
 
-### Expected Output
+#### Expected Output
 
 ```
-Bill Gates person
-Microsoft organization
+Bill Gates => person
+Microsoft => organization
 ```
 
-## Named Entity Recognition benchmark result
+##  📊 NER Benchmark Results
+
+<img align="center" src="https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png" />
+
+## 🛠️ Areas of Improvements / research
+
+- [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
+- [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
+- [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
+- [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
+- [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
+- [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
+- [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
+- [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
+- [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB))
+- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
 
-![image/png](https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png)
 
-## Model Authors
+## 👨‍💻 Model Authors
 The model authors are:
 * [Urchade Zaratiana](https://huggingface.co/urchade)
 * Nadi Tomeh
 * Pierre Holat
 * Thierry Charnois
 
-## Citation
+## 📚 Citation
+
+If you find GLiNER useful in your research, please consider citing our paper:
+
 ```bibtex
 @misc{zaratiana2023gliner,
       title={GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer}, 
       author={Urchade Zaratiana and Nadi Tomeh and Pierre Holat and Thierry Charnois},
       year={2023},
       eprint={2311.08526},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
+We appreciate your support!
```

### Comparing `gliner-0.1.6/gliner/model.py` & `gliner-0.1.7/gliner/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 class GLiNER(InstructBase, PyTorchModelHubMixin):
     def __init__(self, config):
         super().__init__(config)
 
         self.config = config
 
-        if 'token_splitter' not in self.config:
+        if "token_splitter" not in self.config:
             self.token_splitter = WhitespaceTokenSplitter()
-        elif self.config.token_splitter == 'mecab-ko':
+        elif self.config.token_splitter == "mecab-ko":
             self.token_splitter = MecabKoTokenSplitter()
 
         # [ENT] token
         self.entity_token = "<<ENT>>"
         self.sep_token = "<<SEP>>"
 
         # usually a pretrained bidirectional transformer, returns first subtoken representation
@@ -70,90 +70,90 @@
         Parameters:
         - lr_encoder: Learning rate for the encoder layer.
         - lr_others: Learning rate for all other layers.
         - freeze_token_rep: whether the token representation layer should be frozen.
         """
         param_groups = [
             # encoder
-            {'params': self.rnn.parameters(), 'lr': lr_others},
+            {"params": self.rnn.parameters(), "lr": lr_others},
             # projection layers
-            {'params': self.span_rep_layer.parameters(), 'lr': lr_others},
-            {'params': self.prompt_rep_layer.parameters(), 'lr': lr_others},
+            {"params": self.span_rep_layer.parameters(), "lr": lr_others},
+            {"params": self.prompt_rep_layer.parameters(), "lr": lr_others},
         ]
 
         if not freeze_token_rep:
             # If token_rep_layer should not be frozen, add it to the optimizer with its learning rate
-            param_groups.append({'params': self.token_rep_layer.parameters(), 'lr': lr_encoder})
+            param_groups.append({"params": self.token_rep_layer.parameters(), "lr": lr_encoder})
         else:
             # If token_rep_layer should be frozen, explicitly set requires_grad to False for its parameters
             for param in self.token_rep_layer.parameters():
                 param.requires_grad = False
 
         optimizer = torch.optim.AdamW(param_groups)
 
         return optimizer
 
     def compute_score_train(self, x):
-        span_idx = x['span_idx'] * x['span_mask'].unsqueeze(-1)
+        span_idx = x["span_idx"] * x["span_mask"].unsqueeze(-1)
 
-        new_length = x['seq_length'].clone()
+        new_length = x["seq_length"].clone()
         new_tokens = []
         all_len_prompt = []
         num_classes_all = []
 
         # add prompt to the tokens
-        for i in range(len(x['tokens'])):
-            all_types_i = list(x['classes_to_id'][i].keys())
+        for i in range(len(x["tokens"])):
+            all_types_i = list(x["classes_to_id"][i].keys())
             # multiple entity types in all_types. Prompt is appended at the start of tokens
             entity_prompt = []
             num_classes_all.append(len(all_types_i))
             # add enity types to prompt
             for entity_type in all_types_i:
                 entity_prompt.append(self.entity_token)  # [ENT] token
                 entity_prompt.append(entity_type)  # entity type
             entity_prompt.append(self.sep_token)  # [SEP] token
 
             # prompt format:
             # [ENT] entity_type [ENT] entity_type ... [ENT] entity_type [SEP]
 
             # add prompt to the tokens
-            tokens_p = entity_prompt + x['tokens'][i]
+            tokens_p = entity_prompt + x["tokens"][i]
 
             # input format:
             # [ENT] entity_type_1 [ENT] entity_type_2 ... [ENT] entity_type_m [SEP] token_1 token_2 ... token_n
 
             # update length of the sequence (add prompt length to the original length)
             new_length[i] = new_length[i] + len(entity_prompt)
             # update tokens
             new_tokens.append(tokens_p)
             # store prompt length
             all_len_prompt.append(len(entity_prompt))
 
         # create a mask using num_classes_all (0, if it exceeds the number of classes, 1 otherwise)
         max_num_classes = max(num_classes_all)
         entity_type_mask = torch.arange(max_num_classes).unsqueeze(0).expand(len(num_classes_all), -1).to(
-            x['span_mask'].device)
+            x["span_mask"].device)
         entity_type_mask = entity_type_mask < torch.tensor(num_classes_all).unsqueeze(-1).to(
-            x['span_mask'].device)  # [batch_size, max_num_classes]
+            x["span_mask"].device)  # [batch_size, max_num_classes]
 
         # compute all token representations
         bert_output = self.token_rep_layer(new_tokens, new_length)
         word_rep_w_prompt = bert_output["embeddings"]  # embeddings for all tokens (with prompt)
         mask_w_prompt = bert_output["mask"]  # mask for all tokens (with prompt)
 
         # get word representation (after [SEP]), mask (after [SEP]) and entity type representation (before [SEP])
         word_rep = []  # word representation (after [SEP])
         mask = []  # mask (after [SEP])
         entity_type_rep = []  # entity type representation (before [SEP])
-        for i in range(len(x['tokens'])):
+        for i in range(len(x["tokens"])):
             prompt_entity_length = all_len_prompt[i]  # length of prompt for this example
             # get word representation (after [SEP])
-            word_rep.append(word_rep_w_prompt[i, prompt_entity_length:prompt_entity_length + x['seq_length'][i]])
+            word_rep.append(word_rep_w_prompt[i, prompt_entity_length:prompt_entity_length + x["seq_length"][i]])
             # get mask (after [SEP])
-            mask.append(mask_w_prompt[i, prompt_entity_length:prompt_entity_length + x['seq_length'][i]])
+            mask.append(mask_w_prompt[i, prompt_entity_length:prompt_entity_length + x["seq_length"][i]])
 
             # get entity type representation (before [SEP])
             entity_rep = word_rep_w_prompt[i, :prompt_entity_length - 1]  # remove [SEP]
             entity_rep = entity_rep[0::2]  # it means that we take every second element starting from the second one
             entity_type_rep.append(entity_rep)
 
         # padding for word_rep, mask and entity_type_rep
@@ -166,15 +166,15 @@
         span_rep = self.span_rep_layer(word_rep, span_idx)
 
         # compute final entity type representation (FFN)
         entity_type_rep = self.prompt_rep_layer(entity_type_rep)  # (batch_size, len_types, hidden_size)
         num_classes = entity_type_rep.shape[1]  # number of entity types
 
         # similarity score
-        scores = torch.einsum('BLKD,BCD->BLKC', span_rep, entity_type_rep)
+        scores = torch.einsum("BLKD,BCD->BLKC", span_rep, entity_type_rep)
 
         return scores, num_classes, entity_type_mask
 
     def forward(self, x):
         # compute span representation
         scores, num_classes, entity_type_mask = self.compute_score_train(x)
         batch_size = scores.shape[0]
@@ -189,48 +189,48 @@
         labels_one_hot = torch.zeros(labels.size(0), num_classes + 1, dtype=torch.float32).to(scores.device)
         labels_one_hot.scatter_(1, labels.unsqueeze(1), 1)  # Set the corresponding index to 1
         labels_one_hot = labels_one_hot[:, 1:]  # Remove the first column
         # Shape of labels_one_hot: (batch_size * num_spans, num_classes)
 
         # compute loss (without reduction)
         all_losses = F.binary_cross_entropy_with_logits(logits_label, labels_one_hot,
-                                                        reduction='none')
+                                                        reduction="none")
         # mask loss using entity_type_mask (B, C)
         masked_loss = all_losses.view(batch_size, -1, num_classes) * entity_type_mask.unsqueeze(1)
         all_losses = masked_loss.view(-1, num_classes)
         # expand mask_label to all_losses
         mask_label = mask_label.unsqueeze(-1).expand_as(all_losses)
         # put lower loss for in label_one_hot (2 for positive, 1 for negative)
         weight_c = labels_one_hot + 1
         # apply mask
         all_losses = all_losses * mask_label.float() * weight_c
         return all_losses.sum()
 
     def compute_score_eval(self, x, device):
         # check if classes_to_id is dict
-        assert isinstance(x['classes_to_id'], dict), "classes_to_id must be a dict"
+        assert isinstance(x["classes_to_id"], dict), "classes_to_id must be a dict"
 
-        span_idx = (x['span_idx'] * x['span_mask'].unsqueeze(-1)).to(device)
+        span_idx = (x["span_idx"] * x["span_mask"].unsqueeze(-1)).to(device)
 
-        all_types = list(x['classes_to_id'].keys())
+        all_types = list(x["classes_to_id"].keys())
         # multiple entity types in all_types. Prompt is appended at the start of tokens
         entity_prompt = []
 
         # add enity types to prompt
         for entity_type in all_types:
             entity_prompt.append(self.entity_token)
             entity_prompt.append(entity_type)
 
         entity_prompt.append(self.sep_token)
 
         prompt_entity_length = len(entity_prompt)
 
         # add prompt
-        tokens_p = [entity_prompt + tokens for tokens in x['tokens']]
-        seq_length_p = x['seq_length'] + prompt_entity_length
+        tokens_p = [entity_prompt + tokens for tokens in x["tokens"]]
+        seq_length_p = x["seq_length"] + prompt_entity_length
 
         out = self.token_rep_layer(tokens_p, seq_length_p)
 
         word_rep_w_prompt = out["embeddings"]
         mask_w_prompt = out["mask"]
 
         # remove prompt
@@ -244,15 +244,15 @@
 
         entity_type_rep = self.prompt_rep_layer(entity_type_rep)  # (batch_size, len_types, hidden_size)
 
         word_rep = self.rnn(word_rep, mask)
 
         span_rep = self.span_rep_layer(word_rep, span_idx)
 
-        local_scores = torch.einsum('BLKD,BCD->BLKC', span_rep, entity_type_rep)
+        local_scores = torch.einsum("BLKD,BCD->BLKC", span_rep, entity_type_rep)
 
         return local_scores
 
     @torch.no_grad()
     def predict(self, x, flat_ner=False, threshold=0.5):
         self.eval()
         local_scores = self.compute_score_eval(x, device=next(self.parameters()).device)
@@ -473,10 +473,10 @@
         import flair
 
         flair.device = device
         return self
 
 
 def load_config_as_namespace(config_file):
-    with open(config_file, 'r') as f:
+    with open(config_file, "r") as f:
         config_dict = yaml.safe_load(f)
     return argparse.Namespace(**config_dict)
```

### Comparing `gliner-0.1.6/gliner/modules/base.py` & `gliner-0.1.7/gliner/modules/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         # mask for valid spans
         valid_span_mask = spans_idx[:, 1] > length - 1
 
         # mask invalid positions
         span_label = span_label.masked_fill(valid_span_mask, -1)
 
         return {
-            'tokens': tokens,
-            'span_idx': spans_idx,
-            'span_label': span_label,
-            'seq_length': length,
-            'entities': ner,
+            "tokens": tokens,
+            "span_idx": spans_idx,
+            "span_label": span_label,
+            "seq_length": length,
+            "entities": ner,
         }
 
     def collate_fn(self, batch_list, entity_types=None):
         # batch_list: list of dict containing tokens, ner
         if entity_types is None:
             negs = self.get_negatives(batch_list, 100)
             class_to_ids = []
@@ -74,18 +74,18 @@
                 else:
                     neg_type_ratio = random.randint(0, max_neg_type_ratio)
 
                 if neg_type_ratio == 0:
                     # no negatives
                     negs_i = []
                 else:
-                    negs_i = negs[:len(b['ner']) * neg_type_ratio]
+                    negs_i = negs[:len(b["ner"]) * neg_type_ratio]
 
                 # this is the list of all possible entity types (positive and negative)
-                types = list(set([el[-1] for el in b['ner']] + negs_i))
+                types = list(set([el[-1] for el in b["ner"]] + negs_i))
 
                 # shuffle (every epoch)
                 random.shuffle(types)
 
                 if len(types) != 0:
                     # prob of higher number shoul
                     # random drop
@@ -113,37 +113,37 @@
             class_to_ids = {k: v for v, k in enumerate(entity_types, start=1)}
             id_to_classes = {k: v for v, k in class_to_ids.items()}
             batch = [
                 self.preprocess_spans(b["tokenized_text"], b["ner"], class_to_ids) for b in batch_list
             ]
 
         span_idx = pad_sequence(
-            [b['span_idx'] for b in batch], batch_first=True, padding_value=0
+            [b["span_idx"] for b in batch], batch_first=True, padding_value=0
         )
 
         span_label = pad_sequence(
-            [el['span_label'] for el in batch], batch_first=True, padding_value=-1
+            [el["span_label"] for el in batch], batch_first=True, padding_value=-1
         )
 
         return {
-            'seq_length': torch.LongTensor([el['seq_length'] for el in batch]),
-            'span_idx': span_idx,
-            'tokens': [el['tokens'] for el in batch],
-            'span_mask': span_label != -1,
-            'span_label': span_label,
-            'entities': [el['entities'] for el in batch],
-            'classes_to_id': class_to_ids,
-            'id_to_classes': id_to_classes,
+            "seq_length": torch.LongTensor([el["seq_length"] for el in batch]),
+            "span_idx": span_idx,
+            "tokens": [el["tokens"] for el in batch],
+            "span_mask": span_label != -1,
+            "span_label": span_label,
+            "entities": [el["entities"] for el in batch],
+            "classes_to_id": class_to_ids,
+            "id_to_classes": id_to_classes,
         }
 
     @staticmethod
     def get_negatives(batch_list, sampled_neg=5):
         ent_types = []
         for b in batch_list:
-            types = set([el[-1] for el in b['ner']])
+            types = set([el[-1] for el in b["ner"]])
             ent_types.extend(list(types))
         ent_types = list(set(ent_types))
         # sample negatives
         random.shuffle(ent_types)
         return ent_types[:sampled_neg]
 
     def create_dataloader(self, data, entity_types=None, **kwargs):
```

### Comparing `gliner-0.1.6/gliner/modules/data_proc.py` & `gliner-0.1.7/gliner/modules/data_proc.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/gliner/modules/evaluator.py` & `gliner-0.1.7/gliner/modules/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     if flat_ner:
         has_ov = has_overlapping
     else:
         has_ov = has_overlapping_nested
 
     new_list = []
-    span_prob = sorted(spans, key=lambda x: x[-1])
+    span_prob = sorted(spans, key=lambda x: -x[-1])
     
     for i in range(len(spans)):
         b = span_prob[i]
         flag = False
         for new in new_list:
             if has_ov(b[:-1], new):
                 flag = True
```

### Comparing `gliner-0.1.6/gliner/modules/layers.py` & `gliner-0.1.7/gliner/modules/layers.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/gliner/modules/run_evaluation.py` & `gliner-0.1.7/gliner/modules/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/gliner/modules/span_rep.py` & `gliner-0.1.7/gliner/modules/span_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/gliner/modules/token_rep.py` & `gliner-0.1.7/gliner/modules/token_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/gliner/modules/token_splitter.py` & `gliner-0.1.7/gliner/modules/token_splitter.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.6/gliner.egg-info/PKG-INFO` & `gliner-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
@@ -13,87 +13,86 @@
 Requires-Dist: torch>=2.0.0
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: huggingface_hub>=0.21.4
 Requires-Dist: flair==0.13.1
 Requires-Dist: seqeval
 Requires-Dist: tqdm
 
-# GLiNER : Generalist and Lightweight model for Named Entity Recognition
+# 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
-* Paper is available on [Arxiv](https://arxiv.org/abs/2311.08526) (by Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois)
-* Demo on [HuggingFace](https://huggingface.co/spaces/tomaarsen/gliner_base)
-* Try it on [Google Colab](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
-
-<img src="demo.jpg" alt="Demo Image" width="50%"/>
+* **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
+* **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
+* **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage below.
-- `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
-- 📝 Finetuning notebook is available: examples/finetune.ipynb
-- 🗂 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) 📚 and [NuNER](https://huggingface.co/datasets/numind/NuNER) 📘 datasets.
-
-### Available Models on Hugging Face
-- [x] [GLiNER-Base](https://huggingface.co/urchade/gliner_base) (CC BY NC 4.0)
-- [x] [GLiNER-Multi](https://huggingface.co/urchade/gliner_multi) (CC BY NC 4.0)
-- [x] [GLiNER-Small](https://huggingface.co/urchade/gliner_small) (CC BY NC 4.0)
-- [x] [GLiNER-Small-v2](https://huggingface.co/urchade/gliner_smallv2) (Apache)
-- [x] [GLiNER-Medium](https://huggingface.co/urchade/gliner_medium) (CC BY NC 4.0)
-- [x] [GLiNER-Medium-v2](https://huggingface.co/urchade/gliner_mediumv2) (Apache)
-- [x] [GLiNER-Large](https://huggingface.co/urchade/gliner_large) (CC BY NC 4.0)
-- [x] [GLiNER-Large-v2](https://huggingface.co/urchade/gliner_largev2) (Apache)
-
-### To Release
-- [ ] ⏳ GLiNER-Multiv2
-- [ ] ⏳ GLiNER-Sup (trained on mixture of NER datasets)
+- **[08/04]** - Some pretrained weights contained a **bug** which caused performance degradation. For now use base or multi versions.
+- 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
+- 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
+- 🚀 `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
+- 📘 Finetuning notebook is available: examples/finetune.ipynb
+- 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
+
+### 🌟 Available Models on Hugging Face
+
+#### 🇬🇧 For English
+- **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
+- **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
+- **GLiNER Small v2**: `urchade/gliner_smallv2` *(Apache 2.0)*
+- **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
+- **GLiNER Medium v2**: `urchade/gliner_mediumv2` *(Apache 2.0)*
+- **GLiNER Medium v2.1**: `urchade/gliner_mediumv2.1` *(Apache 2.0)*
+- **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
+- **GLiNER Large v2**: `urchade/gliner_largev2` *(Apache 2.0)*
+
+#### 🌍 For Other Languages
+- **Korean**: 🇰🇷 `taeminlee/gliner_ko`
+- **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
+- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)*
 
-## Area of improvements / research
+#### 🔬 Domain Specific Models
+- **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
 
-- [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
-- [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
-- [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
-- [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
-- [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
-- [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
-- [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
-- [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
-- [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB)
-- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
+## 🛠 Installation & Usage
 
+To begin using the GLiNER model, first install the GLiNER Python library through pip:
 
-## Installation
-To use this model, you must install the GLiNER Python library:
-```
+```bash
 !pip install gliner
 ```
 
-## Usage
-Once you've downloaded the GLiNER library, you can import the GLiNER class. You can then load this model using `GLiNER.from_pretrained` and predict entities with `predict_entities`.
+### 🚀 Basic Use Case
+
+After the installation of the GLiNER library, import the `GLiNER` class. Following this, you can load your chosen model with `GLiNER.from_pretrained` and utilize `predict_entities` to discern entities within your text.
 
 ```python
 from gliner import GLiNER
 
+# Initialize GLiNER with the base model
 model = GLiNER.from_pretrained("urchade/gliner_base")
 
+# Sample text for entity prediction
 text = """
 Cristiano Ronaldo dos Santos Aveiro (Portuguese pronunciation: [kɾiʃˈtjɐnu ʁɔˈnaldu]; born 5 February 1985) is a Portuguese professional footballer who plays as a forward for and captains both Saudi Pro League club Al Nassr and the Portugal national team. Widely regarded as one of the greatest players of all time, Ronaldo has won five Ballon d'Or awards,[note 3] a record three UEFA Men's Player of the Year Awards, and four European Golden Shoes, the most by a European player. He has won 33 trophies in his career, including seven league titles, five UEFA Champions Leagues, the UEFA European Championship and the UEFA Nations League. Ronaldo holds the records for most appearances (183), goals (140) and assists (42) in the Champions League, goals in the European Championship (14), international goals (128) and international appearances (205). He is one of the few players to have made over 1,200 professional career appearances, the most by an outfield player, and has scored over 850 official senior career goals for club and country, making him the top goalscorer of all time.
 """
 
+# Labels for entity prediction
 labels = ["person", "award", "date", "competitions", "teams"]
 
+# Perform entity prediction
 entities = model.predict_entities(text, labels, threshold=0.5)
 
+# Display predicted entities and their labels
 for entity in entities:
     print(entity["text"], "=>", entity["label"])
 ```
 
-### Expected Output
+#### Expected Output
 
 ```
 Cristiano Ronaldo dos Santos Aveiro => person
 5 February 1985 => date
 Al Nassr => teams
 Portugal national team => teams
 Ballon d'Or => award
@@ -102,60 +101,92 @@
 UEFA Champions Leagues => competitions
 UEFA European Championship => competitions
 UEFA Nations League => competitions
 Champions League => competitions
 European Championship => competitions
 ```
 
-## Usage with spaCy
+### 🔌 Usage with spaCy
 
-You can also use GliNER with spaCy with the Gliner-spaCy library. To install it, you can use pip:
+GLiNER can be seamlessly integrated with spaCy. To begin, install the `gliner-spacy` library via pip:
 
 ```bash
 pip install gliner-spacy
 ```
-Once installed, you then load GliNER into a regular NLP pipeline. Here's an example using a blank English pipeline, but you can use any spaCy model.
+
+Following installation, you can add GLiNER to a spaCy NLP pipeline. Here's how to integrate it with a blank English pipeline; however, it's compatible with any spaCy model.
 
 ```python
 import spacy
 from gliner_spacy.pipeline import GlinerSpacy
 
-custom_spacy_config = { "gliner_model": "urchade/gliner_multi", "chunk_size": 250, "labels": ["people","company","punctuation"], "style": "ent" }
+# Configuration for GLiNER integration
+custom_spacy_config = {
+    "gliner_model": "urchade/gliner_multi",
+    "chunk_size": 250,
+    "labels": ["person", "organization", "email"],
+    "style": "ent",
+    "threshold": 0.3
+}
+
+# Initialize a blank English spaCy pipeline and add GLiNER
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
 
+# Example text for entity detection
 text = "This is a text about Bill Gates and Microsoft."
+
+# Process the text with the pipeline
 doc = nlp(text)
 
+# Output detected entities
 for ent in doc.ents:
     print(ent.text, ent.label_)
 ```
 
-### Expected Output
+#### Expected Output
 
 ```
-Bill Gates person
-Microsoft organization
+Bill Gates => person
+Microsoft => organization
 ```
 
-## Named Entity Recognition benchmark result
+##  📊 NER Benchmark Results
+
+<img align="center" src="https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png" />
 
-![image/png](https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png)
+## 🛠️ Areas of Improvements / research
 
-## Model Authors
+- [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
+- [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
+- [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
+- [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
+- [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
+- [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
+- [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
+- [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
+- [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB))
+- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
+
+
+## 👨‍💻 Model Authors
 The model authors are:
 * [Urchade Zaratiana](https://huggingface.co/urchade)
 * Nadi Tomeh
 * Pierre Holat
 * Thierry Charnois
 
-## Citation
+## 📚 Citation
+
+If you find GLiNER useful in your research, please consider citing our paper:
+
 ```bibtex
 @misc{zaratiana2023gliner,
       title={GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer}, 
       author={Urchade Zaratiana and Nadi Tomeh and Pierre Holat and Thierry Charnois},
       year={2023},
       eprint={2311.08526},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
+We appreciate your support!
```

### Comparing `gliner-0.1.6/pyproject.toml` & `gliner-0.1.7/pyproject.toml`

 * *Files identical despite different names*

