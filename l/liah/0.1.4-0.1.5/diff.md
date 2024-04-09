# Comparing `tmp/liah-0.1.4.tar.gz` & `tmp/liah-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liah-0.1.4.tar", last modified: Tue Apr  9 13:48:10 2024, max compression
+gzip compressed data, was "liah-0.1.5.tar", last modified: Tue Apr  9 14:18:39 2024, max compression
```

## Comparing `liah-0.1.4.tar` & `liah-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 13:48:10.448448 liah-0.1.4/
--rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.4/LICENSE
--rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.4/MANIFEST.in
--rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 13:48:10.448242 liah-0.1.4/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)     1380 2024-04-09 12:07:14.000000 liah-0.1.4/README.md
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 13:48:10.446210 liah-0.1.4/liah/
--rw-r--r--   0 melvin     (501) staff       (20)     5125 2024-04-09 12:45:01.000000 liah-0.1.4/liah/Liah.py
--rw-r--r--   0 melvin     (501) staff       (20)       37 2024-04-09 12:46:18.000000 liah-0.1.4/liah/__init__.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 13:48:10.447776 liah-0.1.4/liah/dataset/
--rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.4/liah/dataset/README.md
--rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.4/liah/dataset/daughter_of_the_dawn.txt
--rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.4/liah/dataset/when_everybody_knew.txt
--rw-r--r--   0 melvin     (501) staff       (20)     8774 2024-04-09 12:40:09.000000 liah-0.1.4/liah/dataset_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     3360 2024-04-09 12:45:01.000000 liah-0.1.4/liah/evaluator.py
--rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 16:08:56.000000 liah-0.1.4/liah/plot_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     1296 2024-04-09 13:45:35.000000 liah-0.1.4/liah/utils.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 13:48:10.448018 liah-0.1.4/liah.egg-info/
--rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 13:48:10.000000 liah-0.1.4/liah.egg-info/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 13:48:10.000000 liah-0.1.4/liah.egg-info/SOURCES.txt
--rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 13:48:10.000000 liah-0.1.4/liah.egg-info/dependency_links.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 13:48:10.000000 liah-0.1.4/liah.egg-info/requires.txt
--rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 13:48:10.000000 liah-0.1.4/liah.egg-info/top_level.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.4/requirements.txt
--rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 13:48:10.448488 liah-0.1.4/setup.cfg
--rw-r--r--   0 melvin     (501) staff       (20)      910 2024-04-09 13:48:06.000000 liah-0.1.4/setup.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 14:18:39.099672 liah-0.1.5/
+-rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.5/LICENSE
+-rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.5/MANIFEST.in
+-rw-r--r--   0 melvin     (501) staff       (20)     2166 2024-04-09 14:18:39.099359 liah-0.1.5/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)     1662 2024-04-09 14:17:49.000000 liah-0.1.5/README.md
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 14:18:39.094967 liah-0.1.5/liah/
+-rw-r--r--   0 melvin     (501) staff       (20)     5125 2024-04-09 13:55:13.000000 liah-0.1.5/liah/Liah.py
+-rw-r--r--   0 melvin     (501) staff       (20)       37 2024-04-09 13:55:13.000000 liah-0.1.5/liah/__init__.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 14:18:39.098227 liah-0.1.5/liah/dataset/
+-rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.5/liah/dataset/README.md
+-rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.5/liah/dataset/daughter_of_the_dawn.txt
+-rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.5/liah/dataset/when_everybody_knew.txt
+-rw-r--r--   0 melvin     (501) staff       (20)     8774 2024-04-09 13:55:13.000000 liah-0.1.5/liah/dataset_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     3360 2024-04-09 13:55:13.000000 liah-0.1.5/liah/evaluator.py
+-rw-r--r--   0 melvin     (501) staff       (20)     2350 2024-04-09 14:18:08.000000 liah-0.1.5/liah/plot_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1296 2024-04-09 13:55:13.000000 liah-0.1.5/liah/utils.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 14:18:39.098913 liah-0.1.5/liah.egg-info/
+-rw-r--r--   0 melvin     (501) staff       (20)     2166 2024-04-09 14:18:39.000000 liah-0.1.5/liah.egg-info/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 14:18:39.000000 liah-0.1.5/liah.egg-info/SOURCES.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 14:18:39.000000 liah-0.1.5/liah.egg-info/dependency_links.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 14:18:39.000000 liah-0.1.5/liah.egg-info/requires.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 14:18:39.000000 liah-0.1.5/liah.egg-info/top_level.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.5/requirements.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 14:18:39.099722 liah-0.1.5/setup.cfg
+-rw-r--r--   0 melvin     (501) staff       (20)      903 2024-04-09 13:57:43.000000 liah-0.1.5/setup.py
```

### Comparing `liah-0.1.4/LICENSE` & `liah-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/PKG-INFO` & `liah-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.4
+Version: 0.1.5
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
-License: Apache 2.0
+License: MIT
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.16.1
 Requires-Dist: matplotlib
 Requires-Dist: tiktoken
@@ -23,35 +23,50 @@
 With longer context lengths for LLMs. It is increasingly difficult to test
 if fine tuned models attend to all depths of the context.
 
 The needle in haystack is a popular approach. However since the LLMs can also answer
 about the needle instead of the needle. Tests have shown that a "Lie" works well in
 this context 😊
 
+lie: **"Picasso painted the Mona Lisa"**
+
+retrieve: **"Who painted the Mona Lisa?"**
+
 ## Installation
+
     pip install liah
 
 ## Example Usage
 
     # update OPENAI_API_KEY in the env with your token.
     # If you need Open AI models for the final evaluation
+    from liah import Liah
     from vllm import LLM, SamplingParams
 
     # Create a sampling params object.
     sampling_params = SamplingParams(temperature=0.8, top_p=0.95, max_tokens=4096)
-    # llm = LLM(model="mistralai/Mistral-7B-v0.1")
     llm = LLM(model="meta-llama/Llama-2-70b-hf", tensor_parallel_size=4, max_model_len=1500) # need 4 A100s 40GB
+
+    #Create Liah
     liah = Liah(max_context_length=2000)
 
+    #Get a sample from different depths and context_lengths
     for i, sample in enumerate(liah.getSample()):
         # test the sample text with your model
         output = llm.generate([sample["prompt"]], sampling_params)[0]
+        #Update liah with the response
         liah.update(sample, output.outputs[0].text)
+
+    #Contains the plot file from Liah
     plotFilePath = liah.evaluate()
 
+## Sample plot
+
+![sample-plot](/images/sample-plot.png "Liah")
+
 ## Contribute
 
     bash
     pip install pre-commit
 
     then (in the repository, just once)
```

### Comparing `liah-0.1.4/README.md` & `liah-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,35 +6,50 @@
 With longer context lengths for LLMs. It is increasingly difficult to test
 if fine tuned models attend to all depths of the context.
 
 The needle in haystack is a popular approach. However since the LLMs can also answer
 about the needle instead of the needle. Tests have shown that a "Lie" works well in
 this context 😊
 
+lie: **"Picasso painted the Mona Lisa"**
+
+retrieve: **"Who painted the Mona Lisa?"**
+
 ## Installation
+
     pip install liah
 
 ## Example Usage
 
     # update OPENAI_API_KEY in the env with your token.
     # If you need Open AI models for the final evaluation
+    from liah import Liah
     from vllm import LLM, SamplingParams
 
     # Create a sampling params object.
     sampling_params = SamplingParams(temperature=0.8, top_p=0.95, max_tokens=4096)
-    # llm = LLM(model="mistralai/Mistral-7B-v0.1")
     llm = LLM(model="meta-llama/Llama-2-70b-hf", tensor_parallel_size=4, max_model_len=1500) # need 4 A100s 40GB
+
+    #Create Liah
     liah = Liah(max_context_length=2000)
 
+    #Get a sample from different depths and context_lengths
     for i, sample in enumerate(liah.getSample()):
         # test the sample text with your model
         output = llm.generate([sample["prompt"]], sampling_params)[0]
+        #Update liah with the response
         liah.update(sample, output.outputs[0].text)
+
+    #Contains the plot file from Liah
     plotFilePath = liah.evaluate()
 
+## Sample plot
+
+![sample-plot](/images/sample-plot.png "Liah")
+
 ## Contribute
 
     bash
     pip install pre-commit
 
     then (in the repository, just once)
```

### Comparing `liah-0.1.4/liah/Liah.py` & `liah-0.1.5/liah/Liah.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/liah/dataset/daughter_of_the_dawn.txt` & `liah-0.1.5/liah/dataset/daughter_of_the_dawn.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/liah/dataset/when_everybody_knew.txt` & `liah-0.1.5/liah/dataset/when_everybody_knew.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/liah/dataset_utils.py` & `liah-0.1.5/liah/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/liah/evaluator.py` & `liah-0.1.5/liah/evaluator.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/liah/plot_utils.py` & `liah-0.1.5/liah/plot_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.colors import Normalize
+from matplotlib.colors import LinearSegmentedColormap, Normalize
 
 
 def plot_scores(
     context_lengths, positions, scores, model_name, filepath=None, show=True
 ):
     fig, ax = plt.subplots(figsize=(10, 6))
 
     # Normalize the scores for color mapping
     norm = Normalize(vmin=scores.min(), vmax=scores.max())
-    cmap = plt.cm.coolwarm
+
+    # Define a pastel colormap
+    pastel_colors = [
+        (1, 0.7, 0.7),
+        (0.7, 0.7, 1),
+        (0.7, 0.9, 0.6),
+        (1, 1, 0.7),
+    ]  # Pastel red, blue, green, yellow
+    cmap = LinearSegmentedColormap.from_list("PastelColormap", pastel_colors)
 
     # Plot squares with colors based on scores
     for i, length in enumerate(context_lengths):
         for j, position in enumerate(positions):
             color = cmap(norm(scores[i, j]))  # Correctly access scores and map to color
             square = plt.Rectangle((i - 0.5, j - 0.5), 1, 1, color=color)
             ax.add_patch(square)
@@ -48,11 +56,15 @@
 
 if __name__ == "__main__":
     needle_positions = [0.1, 0.25, 0.3, 0.5, 0.6, 0.75, 0.8, 0.9, 1.0]
 
     context_lengths = [1000, 2000, 4000, 8000, 16000, 24000, 32000, 100000]
     positions = needle_positions
     scores = np.random.rand(len(context_lengths), len(positions))
-    model_name = "llama7b"
+    # have scores only either 0 or 1, have lesser 0s and more 1s
+    scores[scores < 0.1] = 0
+    scores[scores >= 0.1] = 1
+    # scores = np.round(scores)
+    model_name = "Your Model"
 
     plot_scores(context_lengths, positions, scores, model_name)
     print("done")
```

### Comparing `liah-0.1.4/liah/utils.py` & `liah-0.1.5/liah/utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.4/liah.egg-info/PKG-INFO` & `liah-0.1.5/liah.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.4
+Version: 0.1.5
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
-License: Apache 2.0
+License: MIT
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.16.1
 Requires-Dist: matplotlib
 Requires-Dist: tiktoken
@@ -23,35 +23,50 @@
 With longer context lengths for LLMs. It is increasingly difficult to test
 if fine tuned models attend to all depths of the context.
 
 The needle in haystack is a popular approach. However since the LLMs can also answer
 about the needle instead of the needle. Tests have shown that a "Lie" works well in
 this context 😊
 
+lie: **"Picasso painted the Mona Lisa"**
+
+retrieve: **"Who painted the Mona Lisa?"**
+
 ## Installation
+
     pip install liah
 
 ## Example Usage
 
     # update OPENAI_API_KEY in the env with your token.
     # If you need Open AI models for the final evaluation
+    from liah import Liah
     from vllm import LLM, SamplingParams
 
     # Create a sampling params object.
     sampling_params = SamplingParams(temperature=0.8, top_p=0.95, max_tokens=4096)
-    # llm = LLM(model="mistralai/Mistral-7B-v0.1")
     llm = LLM(model="meta-llama/Llama-2-70b-hf", tensor_parallel_size=4, max_model_len=1500) # need 4 A100s 40GB
+
+    #Create Liah
     liah = Liah(max_context_length=2000)
 
+    #Get a sample from different depths and context_lengths
     for i, sample in enumerate(liah.getSample()):
         # test the sample text with your model
         output = llm.generate([sample["prompt"]], sampling_params)[0]
+        #Update liah with the response
         liah.update(sample, output.outputs[0].text)
+
+    #Contains the plot file from Liah
     plotFilePath = liah.evaluate()
 
+## Sample plot
+
+![sample-plot](/images/sample-plot.png "Liah")
+
 ## Contribute
 
     bash
     pip install pre-commit
 
     then (in the repository, just once)
```

### Comparing `liah-0.1.4/setup.py` & `liah-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 print(current_directory)
 requirements_path = os.path.join(current_directory, "requirements.txt")
 with open(requirements_path, "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="liah",
-    version="0.1.4",
+    version="0.1.5",
     author="James Melvin Priyarajan",
     author_email="melvinebenezer@gmail.com",
     description="Insert a Lie in a Haystack and evaluate the model's ability to detect it.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/melvinebenezer/Liah-Lie_in_a_haystack",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     keywords=["llm", "needle in a haystack"],
     python_requires=">=3.6",
     classifiers=[],
-    license="Apache 2.0",
+    license="MIT",
 )
```

