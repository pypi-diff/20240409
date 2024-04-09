# Comparing `tmp/gbx-lm-0.1.1.tar.gz` & `tmp/gbx-lm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbx-lm-0.1.1.tar", last modified: Mon Apr  8 20:07:50 2024, max compression
+gzip compressed data, was "gbx-lm-0.1.2.tar", last modified: Mon Apr  8 20:33:22 2024, max compression
```

## Comparing `gbx-lm-0.1.1.tar` & `gbx-lm-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:07:50.043152 gbx-lm-0.1.1/
--rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-03-18 14:26:20.000000 gbx-lm-0.1.1/LICENSE
--rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-08 20:07:50.042943 gbx-lm-0.1.1/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     3734 2024-04-06 12:53:49.000000 gbx-lm-0.1.1/README.md
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:07:50.041216 gbx-lm-0.1.1/gbx_lm/
--rw-r--r--   0 haojin     (501) staff       (20)       66 2024-03-19 13:52:13.000000 gbx-lm-0.1.1/gbx_lm/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)    12368 2024-04-06 12:58:20.000000 gbx-lm-0.1.1/gbx_lm/gba2mlx.py
--rw-r--r--   0 haojin     (501) staff       (20)     4158 2024-04-08 20:02:01.000000 gbx-lm-0.1.1/gbx_lm/generate.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:07:50.042659 gbx-lm-0.1.1/gbx_lm/models/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-03-05 09:34:30.000000 gbx-lm-0.1.1/gbx_lm/models/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)      314 2024-01-13 21:15:10.000000 gbx-lm-0.1.1/gbx_lm/models/base.py
--rw-r--r--   0 haojin     (501) staff       (20)     5639 2024-04-08 11:50:53.000000 gbx-lm-0.1.1/gbx_lm/models/qgemma.py
--rw-r--r--   0 haojin     (501) staff       (20)     7114 2024-04-08 15:08:09.000000 gbx-lm-0.1.1/gbx_lm/models/qllama.py
--rw-r--r--   0 haojin     (501) staff       (20)     8289 2024-04-08 12:11:47.000000 gbx-lm-0.1.1/gbx_lm/models/qmixtral.py
--rw-r--r--   0 haojin     (501) staff       (20)     6614 2024-04-08 15:40:16.000000 gbx-lm-0.1.1/gbx_lm/models/qqwen2.py
--rw-r--r--   0 haojin     (501) staff       (20)    10690 2024-04-02 17:49:04.000000 gbx-lm-0.1.1/gbx_lm/models/quantized_linear_gba.py
--rw-r--r--   0 haojin     (501) staff       (20)    17365 2024-04-08 20:02:01.000000 gbx-lm-0.1.1/gbx_lm/utils.py
--rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-08 20:06:52.000000 gbx-lm-0.1.1/gbx_lm/version.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:07:50.041820 gbx-lm-0.1.1/gbx_lm.egg-info/
--rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-08 20:07:50.000000 gbx-lm-0.1.1/gbx_lm.egg-info/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)      449 2024-04-08 20:07:50.000000 gbx-lm-0.1.1/gbx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-08 20:07:50.000000 gbx-lm-0.1.1/gbx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 haojin     (501) staff       (20)       88 2024-04-08 20:07:50.000000 gbx-lm-0.1.1/gbx_lm.egg-info/requires.txt
--rw-r--r--   0 haojin     (501) staff       (20)        7 2024-04-08 20:07:50.000000 gbx-lm-0.1.1/gbx_lm.egg-info/top_level.txt
--rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-08 20:07:50.043199 gbx-lm-0.1.1/setup.cfg
--rw-r--r--   0 haojin     (501) staff       (20)      800 2024-04-08 19:53:50.000000 gbx-lm-0.1.1/setup.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:33:22.348856 gbx-lm-0.1.2/
+-rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-03-18 14:26:20.000000 gbx-lm-0.1.2/LICENSE
+-rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-08 20:33:22.348623 gbx-lm-0.1.2/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)     3734 2024-04-08 20:17:24.000000 gbx-lm-0.1.2/README.md
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:33:22.345861 gbx-lm-0.1.2/gbx_lm/
+-rw-r--r--   0 haojin     (501) staff       (20)       66 2024-03-19 13:52:13.000000 gbx-lm-0.1.2/gbx_lm/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)    12369 2024-04-08 20:13:35.000000 gbx-lm-0.1.2/gbx_lm/gba2mlx.py
+-rw-r--r--   0 haojin     (501) staff       (20)     4158 2024-04-08 20:02:01.000000 gbx-lm-0.1.2/gbx_lm/generate.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:33:22.348164 gbx-lm-0.1.2/gbx_lm/models/
+-rw-r--r--   0 haojin     (501) staff       (20)        0 2024-03-05 09:34:30.000000 gbx-lm-0.1.2/gbx_lm/models/__init__.py
+-rw-r--r--   0 haojin     (501) staff       (20)      314 2024-01-13 21:15:10.000000 gbx-lm-0.1.2/gbx_lm/models/base.py
+-rw-r--r--   0 haojin     (501) staff       (20)     5639 2024-04-08 11:50:53.000000 gbx-lm-0.1.2/gbx_lm/models/qgemma.py
+-rw-r--r--   0 haojin     (501) staff       (20)     7114 2024-04-08 15:08:09.000000 gbx-lm-0.1.2/gbx_lm/models/qllama.py
+-rw-r--r--   0 haojin     (501) staff       (20)     8289 2024-04-08 12:11:47.000000 gbx-lm-0.1.2/gbx_lm/models/qmixtral.py
+-rw-r--r--   0 haojin     (501) staff       (20)     6614 2024-04-08 15:40:16.000000 gbx-lm-0.1.2/gbx_lm/models/qqwen2.py
+-rw-r--r--   0 haojin     (501) staff       (20)    10690 2024-04-02 17:49:04.000000 gbx-lm-0.1.2/gbx_lm/models/quantized_linear_gba.py
+-rw-r--r--   0 haojin     (501) staff       (20)    17365 2024-04-08 20:02:01.000000 gbx-lm-0.1.2/gbx_lm/utils.py
+-rw-r--r--   0 haojin     (501) staff       (20)       21 2024-04-08 20:33:14.000000 gbx-lm-0.1.2/gbx_lm/version.py
+drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-04-08 20:33:22.346435 gbx-lm-0.1.2/gbx_lm.egg-info/
+-rw-r--r--   0 haojin     (501) staff       (20)     4237 2024-04-08 20:33:22.000000 gbx-lm-0.1.2/gbx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 haojin     (501) staff       (20)      449 2024-04-08 20:33:22.000000 gbx-lm-0.1.2/gbx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        1 2024-04-08 20:33:22.000000 gbx-lm-0.1.2/gbx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       88 2024-04-08 20:33:22.000000 gbx-lm-0.1.2/gbx_lm.egg-info/requires.txt
+-rw-r--r--   0 haojin     (501) staff       (20)        7 2024-04-08 20:33:22.000000 gbx-lm-0.1.2/gbx_lm.egg-info/top_level.txt
+-rw-r--r--   0 haojin     (501) staff       (20)       38 2024-04-08 20:33:22.348906 gbx-lm-0.1.2/setup.cfg
+-rw-r--r--   0 haojin     (501) staff       (20)      800 2024-04-08 19:53:50.000000 gbx-lm-0.1.2/setup.py
```

### Comparing `gbx-lm-0.1.1/LICENSE` & `gbx-lm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/PKG-INFO` & `gbx-lm-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbx-lm
-Version: 0.1.1
+Version: 0.1.2
 Summary: GBA Model Toolkit for MLX
 Home-page: https://github.com/GreenBitAI/gbx-lm
 Author: GreenBitAI and MLX Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -46,15 +46,15 @@
 conda activate gbai_mlx_lm
 ```
 
 ## Usage
 ### Converting Models
 To convert a GreenBitAI's Low-bit LLM to the MLX format, run:
 ```bash
-python gbx_lm/gba2mlx.py --hf-path <input file path or a Hugging Face repo> --mlx-path <output file path> --hf-token <your huggingface token> --upload-repo <a Hugging Face repo name>
+python -m gbx_lm.gba2mlx --hf-path <input file path or a Hugging Face repo> --mlx-path <output file path> --hf-token <your huggingface token> --upload-repo <a Hugging Face repo name>
 ```
 
 ### Generating Content
 To generate natural language content using a converted model:
 ```bash
 python -m gbx_lm.generate --model <path to a converted model or a Hugging Face repo name>
 ```
@@ -64,15 +64,15 @@
 - Python 3.x
 - See `requirements.txt` or `environment.yml` for a complete list of dependencies
 
 ## Examples
 In this example, the pretrained 4-bit model "yi-6b-chat-w4a16g128" will be downloaded from [GreenBitAI's Hugging Face repository](https://huggingface.co/GreenBitAI) and converted into mlx compatible format, and saved in the local directory "yi-6b-chat-w4a16g128-mlx".
 We can also use the "--upload-repo" parameter to provide a Hugging Face repo URL with valid write permissions. This will directly upload the model converted and saved locally to this Hugging Face repo. 
 ```bash
-python gbx_lm/gba2mlx.py --hf-path GreenBitAI/yi-6b-chat-w4a16g128 --mlx-path yi-6b-chat-w4a16g128-mlx/ --hf-token <your huggingface token> --upload-repo GreenBitAI/yi-6b-chat-w4a16g128-mlx
+python -m gbx_lm.gba2mlx --hf-path GreenBitAI/yi-6b-chat-w4a16g128 --mlx-path yi-6b-chat-w4a16g128-mlx/ --hf-token <your huggingface token> --upload-repo GreenBitAI/yi-6b-chat-w4a16g128-mlx
 ```
 It will download and run the local model to generate natural language content through prompts given by users.
 ```bash
 python -m gbx_lm.generate --model GreenBitAI/yi-6b-chat-w4a16g128-mlx  --max-tokens 100 --prompt "calculate 4*8+1024=" --eos-token '<|im_end|>'
 ```
 
 ## License
```

### Comparing `gbx-lm-0.1.1/README.md` & `gbx-lm-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 conda activate gbai_mlx_lm
 ```
 
 ## Usage
 ### Converting Models
 To convert a GreenBitAI's Low-bit LLM to the MLX format, run:
 ```bash
-python gbx_lm/gba2mlx.py --hf-path <input file path or a Hugging Face repo> --mlx-path <output file path> --hf-token <your huggingface token> --upload-repo <a Hugging Face repo name>
+python -m gbx_lm.gba2mlx --hf-path <input file path or a Hugging Face repo> --mlx-path <output file path> --hf-token <your huggingface token> --upload-repo <a Hugging Face repo name>
 ```
 
 ### Generating Content
 To generate natural language content using a converted model:
 ```bash
 python -m gbx_lm.generate --model <path to a converted model or a Hugging Face repo name>
 ```
@@ -45,15 +45,15 @@
 - Python 3.x
 - See `requirements.txt` or `environment.yml` for a complete list of dependencies
 
 ## Examples
 In this example, the pretrained 4-bit model "yi-6b-chat-w4a16g128" will be downloaded from [GreenBitAI's Hugging Face repository](https://huggingface.co/GreenBitAI) and converted into mlx compatible format, and saved in the local directory "yi-6b-chat-w4a16g128-mlx".
 We can also use the "--upload-repo" parameter to provide a Hugging Face repo URL with valid write permissions. This will directly upload the model converted and saved locally to this Hugging Face repo. 
 ```bash
-python gbx_lm/gba2mlx.py --hf-path GreenBitAI/yi-6b-chat-w4a16g128 --mlx-path yi-6b-chat-w4a16g128-mlx/ --hf-token <your huggingface token> --upload-repo GreenBitAI/yi-6b-chat-w4a16g128-mlx
+python -m gbx_lm.gba2mlx --hf-path GreenBitAI/yi-6b-chat-w4a16g128 --mlx-path yi-6b-chat-w4a16g128-mlx/ --hf-token <your huggingface token> --upload-repo GreenBitAI/yi-6b-chat-w4a16g128-mlx
 ```
 It will download and run the local model to generate natural language content through prompts given by users.
 ```bash
 python -m gbx_lm.generate --model GreenBitAI/yi-6b-chat-w4a16g128-mlx  --max-tokens 100 --prompt "calculate 4*8+1024=" --eos-token '<|im_end|>'
 ```
 
 ## License
```

### Comparing `gbx-lm-0.1.1/gbx_lm/gba2mlx.py` & `gbx-lm-0.1.2/gbx_lm/gba2mlx.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Dict, Tuple, Optional, Union, Any
 
 import mlx.core as mx
 import mlx.nn as nn
 import transformers
 from mlx.utils import tree_flatten
 
-from utils import get_model_path, load_model, extract_bits_and_group_size
+from .utils import get_model_path, load_model, extract_bits_and_group_size
 
 MAX_FILE_SIZE_GB = 5
 
 
 def configure_parser() -> argparse.ArgumentParser:
     """
     Configures and returns the argument parser for the script.
```

### Comparing `gbx-lm-0.1.1/gbx_lm/generate.py` & `gbx-lm-0.1.2/gbx_lm/generate.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm/models/qgemma.py` & `gbx-lm-0.1.2/gbx_lm/models/qgemma.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm/models/qllama.py` & `gbx-lm-0.1.2/gbx_lm/models/qllama.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm/models/qmixtral.py` & `gbx-lm-0.1.2/gbx_lm/models/qmixtral.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm/models/qqwen2.py` & `gbx-lm-0.1.2/gbx_lm/models/qqwen2.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm/models/quantized_linear_gba.py` & `gbx-lm-0.1.2/gbx_lm/models/quantized_linear_gba.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm/utils.py` & `gbx-lm-0.1.2/gbx_lm/utils.py`

 * *Files identical despite different names*

### Comparing `gbx-lm-0.1.1/gbx_lm.egg-info/PKG-INFO` & `gbx-lm-0.1.2/gbx_lm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbx-lm
-Version: 0.1.1
+Version: 0.1.2
 Summary: GBA Model Toolkit for MLX
 Home-page: https://github.com/GreenBitAI/gbx-lm
 Author: GreenBitAI and MLX Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -46,15 +46,15 @@
 conda activate gbai_mlx_lm
 ```
 
 ## Usage
 ### Converting Models
 To convert a GreenBitAI's Low-bit LLM to the MLX format, run:
 ```bash
-python gbx_lm/gba2mlx.py --hf-path <input file path or a Hugging Face repo> --mlx-path <output file path> --hf-token <your huggingface token> --upload-repo <a Hugging Face repo name>
+python -m gbx_lm.gba2mlx --hf-path <input file path or a Hugging Face repo> --mlx-path <output file path> --hf-token <your huggingface token> --upload-repo <a Hugging Face repo name>
 ```
 
 ### Generating Content
 To generate natural language content using a converted model:
 ```bash
 python -m gbx_lm.generate --model <path to a converted model or a Hugging Face repo name>
 ```
@@ -64,15 +64,15 @@
 - Python 3.x
 - See `requirements.txt` or `environment.yml` for a complete list of dependencies
 
 ## Examples
 In this example, the pretrained 4-bit model "yi-6b-chat-w4a16g128" will be downloaded from [GreenBitAI's Hugging Face repository](https://huggingface.co/GreenBitAI) and converted into mlx compatible format, and saved in the local directory "yi-6b-chat-w4a16g128-mlx".
 We can also use the "--upload-repo" parameter to provide a Hugging Face repo URL with valid write permissions. This will directly upload the model converted and saved locally to this Hugging Face repo. 
 ```bash
-python gbx_lm/gba2mlx.py --hf-path GreenBitAI/yi-6b-chat-w4a16g128 --mlx-path yi-6b-chat-w4a16g128-mlx/ --hf-token <your huggingface token> --upload-repo GreenBitAI/yi-6b-chat-w4a16g128-mlx
+python -m gbx_lm.gba2mlx --hf-path GreenBitAI/yi-6b-chat-w4a16g128 --mlx-path yi-6b-chat-w4a16g128-mlx/ --hf-token <your huggingface token> --upload-repo GreenBitAI/yi-6b-chat-w4a16g128-mlx
 ```
 It will download and run the local model to generate natural language content through prompts given by users.
 ```bash
 python -m gbx_lm.generate --model GreenBitAI/yi-6b-chat-w4a16g128-mlx  --max-tokens 100 --prompt "calculate 4*8+1024=" --eos-token '<|im_end|>'
 ```
 
 ## License
```

### Comparing `gbx-lm-0.1.1/setup.py` & `gbx-lm-0.1.2/setup.py`

 * *Files identical despite different names*

