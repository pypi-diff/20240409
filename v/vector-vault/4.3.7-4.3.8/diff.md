# Comparing `tmp/vector_vault-4.3.7.tar.gz` & `tmp/vector_vault-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.3.7.tar", last modified: Mon Apr  8 21:07:29 2024, max compression
+gzip compressed data, was "vector_vault-4.3.8.tar", last modified: Tue Apr  9 00:30:32 2024, max compression
```

## Comparing `vector_vault-4.3.7.tar` & `vector_vault-4.3.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 21:07:29.087775 vector_vault-4.3.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 21:07:29.087640 vector_vault-4.3.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-08 21:07:29.087808 vector_vault-4.3.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-08 21:07:12.000000 vector_vault-4.3.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 21:07:29.084889 vector_vault-4.3.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-08 21:07:29.000000 vector_vault-4.3.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      435 2024-04-08 21:07:29.000000 vector_vault-4.3.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-08 21:07:29.000000 vector_vault-4.3.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-08 21:07:29.000000 vector_vault-4.3.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-08 21:07:29.000000 vector_vault-4.3.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-08 21:07:29.087466 vector_vault-4.3.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.3.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.7/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5996 2024-04-08 20:07:11.000000 vector_vault-4.3.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-08 20:07:01.000000 vector_vault-4.3.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-08 20:06:58.000000 vector_vault-4.3.7/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-09 00:30:32.543182 vector_vault-4.3.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-09 00:30:32.543040 vector_vault-4.3.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-09 00:30:32.543217 vector_vault-4.3.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-09 00:29:55.000000 vector_vault-4.3.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-09 00:30:32.539043 vector_vault-4.3.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-09 00:30:32.000000 vector_vault-4.3.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-09 00:30:32.000000 vector_vault-4.3.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-09 00:30:32.000000 vector_vault-4.3.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-09 00:30:32.000000 vector_vault-4.3.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-09 00:30:32.000000 vector_vault-4.3.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-09 00:30:32.542730 vector_vault-4.3.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.3.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.8/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5996 2024-04-08 20:07:11.000000 vector_vault-4.3.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-08 20:07:01.000000 vector_vault-4.3.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-08 20:06:58.000000 vector_vault-4.3.8/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62800 2024-04-09 00:29:47.000000 vector_vault-4.3.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.8/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.8/vectorvault/wrap.py
```

### Comparing `vector_vault-4.3.7/LICENSE` & `vector_vault-4.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/PKG-INFO` & `vector_vault-4.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.3.7
+Version: 4.3.8
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.7/README.md` & `vector_vault-4.3.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/setup.py` & `vector_vault-4.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.3.7",
+    version="4.3.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.3.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.3.8/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.3.7
+Version: 4.3.8
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.7/vectorvault/ai.py` & `vector_vault-4.3.8/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/cloud_api.py` & `vector_vault-4.3.8/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/cloudmanager.py` & `vector_vault-4.3.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/creds.py` & `vector_vault-4.3.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/download.py` & `vector_vault-4.3.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/itemize.py` & `vector_vault-4.3.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/tools_gpt.py` & `vector_vault-4.3.8/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.7/vectorvault/vecreq.py` & `vector_vault-4.3.8/vectorvault/vecreq.py`

 * *Files identical despite different names*

