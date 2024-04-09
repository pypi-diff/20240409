# Comparing `tmp/conflare-0.1.1.tar.gz` & `tmp/conflare-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflare-0.1.1.tar", last modified: Mon Apr  8 14:35:31 2024, max compression
+gzip compressed data, was "conflare-0.1.2.tar", last modified: Tue Apr  9 05:04:36 2024, max compression
```

## Comparing `conflare-0.1.1.tar` & `conflare-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.248488 conflare-0.1.1/
--rw-r--r--   0 moein      (501) staff       (20)     1087 2024-04-08 12:12:09.000000 conflare-0.1.1/LICENSE
--rw-r--r--   0 moein      (501) staff       (20)     2304 2024-04-08 14:35:31.248267 conflare-0.1.1/PKG-INFO
--rw-r--r--   0 moein      (501) staff       (20)     1807 2024-04-02 09:39:21.000000 conflare-0.1.1/README.md
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.245147 conflare-0.1.1/conflare/
--rw-r--r--   0 moein      (501) staff       (20)      242 2024-04-08 13:50:07.000000 conflare-0.1.1/conflare/__init__.py
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.246328 conflare-0.1.1/conflare/augmented_retrieval/
--rw-r--r--   0 moein      (501) staff       (20)      126 2024-04-08 13:02:26.000000 conflare-0.1.1/conflare/augmented_retrieval/__init__.py
--rw-r--r--   0 moein      (501) staff       (20)      912 2024-03-31 07:11:07.000000 conflare-0.1.1/conflare/augmented_retrieval/embed.py
--rw-r--r--   0 moein      (501) staff       (20)     4271 2024-04-08 13:08:39.000000 conflare-0.1.1/conflare/augmented_retrieval/rag.py
--rw-r--r--   0 moein      (501) staff       (20)     2023 2024-04-02 07:11:13.000000 conflare-0.1.1/conflare/augmented_retrieval/vector_db.py
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.246602 conflare-0.1.1/conflare/conformal/
--rw-r--r--   0 moein      (501) staff       (20)       91 2024-04-08 13:02:49.000000 conflare-0.1.1/conflare/conformal/__init__.py
--rw-r--r--   0 moein      (501) staff       (20)    11994 2024-04-08 13:09:06.000000 conflare-0.1.1/conflare/conformal/calibration.py
--rw-r--r--   0 moein      (501) staff       (20)     4460 2024-04-08 13:49:46.000000 conflare-0.1.1/conflare/main.py
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.247118 conflare-0.1.1/conflare/models/
--rw-r--r--   0 moein      (501) staff       (20)      102 2024-04-08 13:03:25.000000 conflare-0.1.1/conflare/models/__init__.py
--rw-r--r--   0 moein      (501) staff       (20)     4812 2024-04-01 06:40:23.000000 conflare-0.1.1/conflare/models/hf.py
--rw-r--r--   0 moein      (501) staff       (20)     4224 2024-04-08 13:50:46.000000 conflare-0.1.1/conflare/models/openai.py
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.247776 conflare-0.1.1/conflare/utils/
--rw-r--r--   0 moein      (501) staff       (20)       99 2024-04-08 13:04:01.000000 conflare-0.1.1/conflare/utils/__init__.py
--rw-r--r--   0 moein      (501) staff       (20)     1951 2024-04-08 13:19:30.000000 conflare-0.1.1/conflare/utils/loaders.py
--rw-r--r--   0 moein      (501) staff       (20)     2926 2024-04-01 07:58:59.000000 conflare-0.1.1/conflare/utils/preprocess.py
--rw-r--r--   0 moein      (501) staff       (20)     7120 2024-04-02 09:02:51.000000 conflare-0.1.1/conflare/utils/prompts.py
-drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-08 14:35:31.248021 conflare-0.1.1/conflare.egg-info/
--rw-r--r--   0 moein      (501) staff       (20)     2304 2024-04-08 14:35:31.000000 conflare-0.1.1/conflare.egg-info/PKG-INFO
--rw-r--r--   0 moein      (501) staff       (20)      598 2024-04-08 14:35:31.000000 conflare-0.1.1/conflare.egg-info/SOURCES.txt
--rw-r--r--   0 moein      (501) staff       (20)        1 2024-04-08 14:35:31.000000 conflare-0.1.1/conflare.egg-info/dependency_links.txt
--rw-r--r--   0 moein      (501) staff       (20)        9 2024-04-08 14:35:31.000000 conflare-0.1.1/conflare.egg-info/top_level.txt
--rw-r--r--   0 moein      (501) staff       (20)       38 2024-04-08 14:35:31.248538 conflare-0.1.1/setup.cfg
--rw-r--r--   0 moein      (501) staff       (20)     1531 2024-04-08 14:35:13.000000 conflare-0.1.1/setup.py
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.680682 conflare-0.1.2/
+-rw-r--r--   0 moein      (501) staff       (20)     1087 2024-04-08 12:12:09.000000 conflare-0.1.2/LICENSE
+-rw-r--r--   0 moein      (501) staff       (20)     2572 2024-04-09 05:04:36.680463 conflare-0.1.2/PKG-INFO
+-rw-r--r--   0 moein      (501) staff       (20)     1807 2024-04-02 09:39:21.000000 conflare-0.1.2/README.md
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.677264 conflare-0.1.2/conflare/
+-rw-r--r--   0 moein      (501) staff       (20)      242 2024-04-08 13:50:07.000000 conflare-0.1.2/conflare/__init__.py
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.678560 conflare-0.1.2/conflare/augmented_retrieval/
+-rw-r--r--   0 moein      (501) staff       (20)      126 2024-04-08 13:02:26.000000 conflare-0.1.2/conflare/augmented_retrieval/__init__.py
+-rw-r--r--   0 moein      (501) staff       (20)      912 2024-03-31 07:11:07.000000 conflare-0.1.2/conflare/augmented_retrieval/embed.py
+-rw-r--r--   0 moein      (501) staff       (20)     4271 2024-04-08 13:08:39.000000 conflare-0.1.2/conflare/augmented_retrieval/rag.py
+-rw-r--r--   0 moein      (501) staff       (20)     2023 2024-04-02 07:11:13.000000 conflare-0.1.2/conflare/augmented_retrieval/vector_db.py
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.678847 conflare-0.1.2/conflare/conformal/
+-rw-r--r--   0 moein      (501) staff       (20)       91 2024-04-08 13:02:49.000000 conflare-0.1.2/conflare/conformal/__init__.py
+-rw-r--r--   0 moein      (501) staff       (20)    11994 2024-04-08 13:09:06.000000 conflare-0.1.2/conflare/conformal/calibration.py
+-rw-r--r--   0 moein      (501) staff       (20)     4460 2024-04-08 13:49:46.000000 conflare-0.1.2/conflare/main.py
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.679403 conflare-0.1.2/conflare/models/
+-rw-r--r--   0 moein      (501) staff       (20)      102 2024-04-08 13:03:25.000000 conflare-0.1.2/conflare/models/__init__.py
+-rw-r--r--   0 moein      (501) staff       (20)     4812 2024-04-01 06:40:23.000000 conflare-0.1.2/conflare/models/hf.py
+-rw-r--r--   0 moein      (501) staff       (20)     4224 2024-04-08 13:50:46.000000 conflare-0.1.2/conflare/models/openai.py
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.679971 conflare-0.1.2/conflare/utils/
+-rw-r--r--   0 moein      (501) staff       (20)       99 2024-04-08 13:04:01.000000 conflare-0.1.2/conflare/utils/__init__.py
+-rw-r--r--   0 moein      (501) staff       (20)     1951 2024-04-08 13:19:30.000000 conflare-0.1.2/conflare/utils/loaders.py
+-rw-r--r--   0 moein      (501) staff       (20)     2926 2024-04-01 07:58:59.000000 conflare-0.1.2/conflare/utils/preprocess.py
+-rw-r--r--   0 moein      (501) staff       (20)     7120 2024-04-02 09:02:51.000000 conflare-0.1.2/conflare/utils/prompts.py
+drwxr-xr-x   0 moein      (501) staff       (20)        0 2024-04-09 05:04:36.680195 conflare-0.1.2/conflare.egg-info/
+-rw-r--r--   0 moein      (501) staff       (20)     2572 2024-04-09 05:04:36.000000 conflare-0.1.2/conflare.egg-info/PKG-INFO
+-rw-r--r--   0 moein      (501) staff       (20)      629 2024-04-09 05:04:36.000000 conflare-0.1.2/conflare.egg-info/SOURCES.txt
+-rw-r--r--   0 moein      (501) staff       (20)        1 2024-04-09 05:04:36.000000 conflare-0.1.2/conflare.egg-info/dependency_links.txt
+-rw-r--r--   0 moein      (501) staff       (20)      148 2024-04-09 05:04:36.000000 conflare-0.1.2/conflare.egg-info/requires.txt
+-rw-r--r--   0 moein      (501) staff       (20)        9 2024-04-09 05:04:36.000000 conflare-0.1.2/conflare.egg-info/top_level.txt
+-rw-r--r--   0 moein      (501) staff       (20)       38 2024-04-09 05:04:36.680729 conflare-0.1.2/setup.cfg
+-rw-r--r--   0 moein      (501) staff       (20)     1515 2024-04-09 05:04:23.000000 conflare-0.1.2/setup.py
```

### Comparing `conflare-0.1.1/LICENSE` & `conflare-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/PKG-INFO` & `conflare-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: conflare
-Version: 0.1.1
+Version: 0.1.2
 Summary: conformal retreival augmented generation with LLMs
 Home-page: https://github.com/Mayo-Radiology-Informatics-Lab/conflare
 Author: Moein Shariatnia
 Author-email: moein.shariatnia@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pypdf==4.1.0
+Requires-Dist: torch>=2.0.0
+Requires-Dist: transformers==4.37.2
+Requires-Dist: bitsandbytes==0.42.0
+Requires-Dist: accelerate==0.26.1
+Requires-Dist: openai==1.12.0
+Requires-Dist: sentence-transformers==2.3.1
+Requires-Dist: chromadb==0.4.22
 
 <img src="./media/conflare.png" alt="drawing" width="200"/>
 
 # CONFLARE: CONFormal LArge language model REtrieval
 
 This is the repo for the [CONFLARE paper](arxiv.com) giving an easy access to scripts to do RAG w/ Conformal guarantees.
```

### Comparing `conflare-0.1.1/README.md` & `conflare-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/augmented_retrieval/embed.py` & `conflare-0.1.2/conflare/augmented_retrieval/embed.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/augmented_retrieval/rag.py` & `conflare-0.1.2/conflare/augmented_retrieval/rag.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/augmented_retrieval/vector_db.py` & `conflare-0.1.2/conflare/augmented_retrieval/vector_db.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/conformal/calibration.py` & `conflare-0.1.2/conflare/conformal/calibration.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/main.py` & `conflare-0.1.2/conflare/main.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/models/hf.py` & `conflare-0.1.2/conflare/models/hf.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/models/openai.py` & `conflare-0.1.2/conflare/models/openai.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/utils/loaders.py` & `conflare-0.1.2/conflare/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/utils/preprocess.py` & `conflare-0.1.2/conflare/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare/utils/prompts.py` & `conflare-0.1.2/conflare/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `conflare-0.1.1/conflare.egg-info/PKG-INFO` & `conflare-0.1.2/conflare.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: conflare
-Version: 0.1.1
+Version: 0.1.2
 Summary: conformal retreival augmented generation with LLMs
 Home-page: https://github.com/Mayo-Radiology-Informatics-Lab/conflare
 Author: Moein Shariatnia
 Author-email: moein.shariatnia@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pypdf==4.1.0
+Requires-Dist: torch>=2.0.0
+Requires-Dist: transformers==4.37.2
+Requires-Dist: bitsandbytes==0.42.0
+Requires-Dist: accelerate==0.26.1
+Requires-Dist: openai==1.12.0
+Requires-Dist: sentence-transformers==2.3.1
+Requires-Dist: chromadb==0.4.22
 
 <img src="./media/conflare.png" alt="drawing" width="200"/>
 
 # CONFLARE: CONFormal LArge language model REtrieval
 
 This is the repo for the [CONFLARE paper](arxiv.com) giving an easy access to scripts to do RAG w/ Conformal guarantees.
```

### Comparing `conflare-0.1.1/conflare.egg-info/SOURCES.txt` & `conflare-0.1.2/conflare.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 conflare/__init__.py
 conflare/main.py
 conflare.egg-info/PKG-INFO
 conflare.egg-info/SOURCES.txt
 conflare.egg-info/dependency_links.txt
+conflare.egg-info/requires.txt
 conflare.egg-info/top_level.txt
 conflare/augmented_retrieval/__init__.py
 conflare/augmented_retrieval/embed.py
 conflare/augmented_retrieval/rag.py
 conflare/augmented_retrieval/vector_db.py
 conflare/conformal/__init__.py
 conflare/conformal/calibration.py
```

### Comparing `conflare-0.1.1/setup.py` & `conflare-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from setuptools import setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='conflare',
-    version='0.1.1',    
+    version='0.1.2',    
     description='conformal retreival augmented generation with LLMs',
     url='https://github.com/Mayo-Radiology-Informatics-Lab/conflare',
     author='Moein Shariatnia',
     author_email='moein.shariatnia@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir = {"conflare": "conflare",
                    "conflare.conformal": "conflare/conformal",
                    "conflare.models": "conflare/models",
                    "conflare.utils": "conflare/utils",
                    "conflare.augmented_retrieval": "conflare/augmented_retrieval"},
     packages = ['conflare', 'conflare.conformal', 'conflare.models', 'conflare.utils', 'conflare.augmented_retrieval'],
     install_requires=[  
-                        # 'pypdf==4.1.0',
-                        # 'torch>=2.0.0',
-                        # 'transformers==4.37.2',
-                        # 'bitsandbytes==0.42.0',
-                        # 'accelerate==0.26.1',
-                        # 'openai==1.12.0',
-                        # 'sentence-transformers==2.3.1',
-                        # 'chromadb==0.4.22'
+                        'pypdf==4.1.0',
+                        'torch>=2.0.0',
+                        'transformers==4.37.2',
+                        'bitsandbytes==0.42.0',
+                        'accelerate==0.26.1',
+                        'openai==1.12.0',
+                        'sentence-transformers==2.3.1',
+                        'chromadb==0.4.22'
                     ],
 
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
```

