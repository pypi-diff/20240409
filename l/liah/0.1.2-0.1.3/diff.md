# Comparing `tmp/liah-0.1.2.tar.gz` & `tmp/liah-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liah-0.1.2.tar", last modified: Tue Apr  9 12:28:22 2024, max compression
+gzip compressed data, was "liah-0.1.3.tar", last modified: Tue Apr  9 12:41:18 2024, max compression
```

## Comparing `liah-0.1.2.tar` & `liah-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.791067 liah-0.1.2/
--rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.2/LICENSE
--rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.2/MANIFEST.in
--rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:28:22.790793 liah-0.1.2/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)     1380 2024-04-09 12:07:14.000000 liah-0.1.2/README.md
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.786965 liah-0.1.2/liah/
--rw-r--r--   0 melvin     (501) staff       (20)     5124 2024-04-09 12:14:00.000000 liah-0.1.2/liah/Liah.py
--rw-r--r--   0 melvin     (501) staff       (20)       23 2024-04-09 12:26:18.000000 liah-0.1.2/liah/__init__.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.789786 liah-0.1.2/liah/dataset/
--rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.2/liah/dataset/README.md
--rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.2/liah/dataset/daughter_of_the_dawn.txt
--rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.2/liah/dataset/when_everybody_knew.txt
--rw-r--r--   0 melvin     (501) staff       (20)     8668 2024-04-06 16:08:56.000000 liah-0.1.2/liah/dataset_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     3359 2024-04-09 12:14:23.000000 liah-0.1.2/liah/evaluator.py
--rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 16:08:56.000000 liah-0.1.2/liah/plot_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     1339 2024-04-06 16:08:56.000000 liah-0.1.2/liah/utils.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.790500 liah-0.1.2/liah.egg-info/
--rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/SOURCES.txt
--rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/dependency_links.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/requires.txt
--rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/top_level.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.2/requirements.txt
--rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 12:28:22.791122 liah-0.1.2/setup.cfg
--rw-r--r--   0 melvin     (501) staff       (20)      910 2024-04-09 12:28:18.000000 liah-0.1.2/setup.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:41:18.595503 liah-0.1.3/
+-rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.3/LICENSE
+-rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.3/MANIFEST.in
+-rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:41:18.595157 liah-0.1.3/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)     1380 2024-04-09 12:07:14.000000 liah-0.1.3/README.md
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:41:18.591278 liah-0.1.3/liah/
+-rw-r--r--   0 melvin     (501) staff       (20)     5124 2024-04-09 12:14:00.000000 liah-0.1.3/liah/Liah.py
+-rw-r--r--   0 melvin     (501) staff       (20)       23 2024-04-09 12:26:18.000000 liah-0.1.3/liah/__init__.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:41:18.594040 liah-0.1.3/liah/dataset/
+-rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.3/liah/dataset/README.md
+-rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.3/liah/dataset/daughter_of_the_dawn.txt
+-rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.3/liah/dataset/when_everybody_knew.txt
+-rw-r--r--   0 melvin     (501) staff       (20)     8774 2024-04-09 12:40:09.000000 liah-0.1.3/liah/dataset_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     3359 2024-04-09 12:14:23.000000 liah-0.1.3/liah/evaluator.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 16:08:56.000000 liah-0.1.3/liah/plot_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1339 2024-04-06 16:08:56.000000 liah-0.1.3/liah/utils.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:41:18.594860 liah-0.1.3/liah.egg-info/
+-rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:41:18.000000 liah-0.1.3/liah.egg-info/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 12:41:18.000000 liah-0.1.3/liah.egg-info/SOURCES.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 12:41:18.000000 liah-0.1.3/liah.egg-info/dependency_links.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 12:41:18.000000 liah-0.1.3/liah.egg-info/requires.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 12:41:18.000000 liah-0.1.3/liah.egg-info/top_level.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.3/requirements.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 12:41:18.595574 liah-0.1.3/setup.cfg
+-rw-r--r--   0 melvin     (501) staff       (20)      910 2024-04-09 12:40:46.000000 liah-0.1.3/setup.py
```

### Comparing `liah-0.1.2/LICENSE` & `liah-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/PKG-INFO` & `liah-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.2
+Version: 0.1.3
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
 License: Apache 2.0
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
```

### Comparing `liah-0.1.2/README.md` & `liah-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah/Liah.py` & `liah-0.1.3/liah/Liah.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah/dataset/daughter_of_the_dawn.txt` & `liah-0.1.3/liah/dataset/daughter_of_the_dawn.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah/dataset/when_everybody_knew.txt` & `liah-0.1.3/liah/dataset/when_everybody_knew.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah/dataset_utils.py` & `liah-0.1.3/liah/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,30 +92,31 @@
         if token_count >= token_length:
             # concantenate the lines and return text
             return "\n".join(required_lines)
     return text
 
 
 def create_ctx_len_dataset(
-    datasetDir="dataset",
+    datasetDir="./dataset",
     prompt_length=100,
     context_lengths=[1000, 2000, 4000, 8000, 16000, 24000, 32000, 100000],
 ):
     """
     Create a new dataset with context lengths that are closest to the specified context lengths.
     Args:
     - datasetDir (str): The directory containing the original dataset.
     - prompt_length (int): The length of the prompt to be used. Defaults to 100 tokens.
     - context_lengths (list): A list of context lengths to create new datasets for.
     Returns:
     - list: A list of file paths for the new datasets created.
     """
 
     # Get the context lengths of the dataset
-    datasetDir = "dataset"
+    # dataset directory is the directory containing this file
+    datasetDir = os.path.join(os.path.dirname(__file__), datasetDir)
     filePaths = os.listdir(datasetDir)
     # handle only .txt files
     filePaths = [file for file in filePaths if ".txt" in file]
     token_counts = {}
     for file in filePaths:
         # print(f"Reading file: {file}")
         with open(os.path.join(datasetDir, file), "r") as f:
```

### Comparing `liah-0.1.2/liah/evaluator.py` & `liah-0.1.3/liah/evaluator.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah/plot_utils.py` & `liah-0.1.3/liah/plot_utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah/utils.py` & `liah-0.1.3/liah/utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.2/liah.egg-info/PKG-INFO` & `liah-0.1.3/liah.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.2
+Version: 0.1.3
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
 License: Apache 2.0
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
```

### Comparing `liah-0.1.2/setup.py` & `liah-0.1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 print(current_directory)
 requirements_path = os.path.join(current_directory, "requirements.txt")
 with open(requirements_path, "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="liah",
-    version="0.1.2",
+    version="0.1.3",
     author="James Melvin Priyarajan",
     author_email="melvinebenezer@gmail.com",
     description="Insert a Lie in a Haystack and evaluate the model's ability to detect it.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/melvinebenezer/Liah-Lie_in_a_haystack",
     packages=find_packages(),
```

