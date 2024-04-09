# Comparing `tmp/sdevelo-0.1.tar.gz` & `tmp/sdevelo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevelo-0.1.tar", last modified: Tue Apr  9 12:02:46 2024, max compression
+gzip compressed data, was "sdevelo-0.1.1.tar", last modified: Tue Apr  9 12:17:18 2024, max compression
```

## Comparing `sdevelo-0.1.tar` & `sdevelo-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 xuliao    (1005) xuliao    (1005)        0 2024-04-09 12:02:46.143397 sdevelo-0.1/
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     1082 2024-04-09 11:56:43.000000 sdevelo-0.1/LICENSE
--rw-r--r--   0 xuliao    (1005) xuliao    (1005)     1418 2024-04-09 12:02:46.143397 sdevelo-0.1/PKG-INFO
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      620 2024-04-04 05:41:59.000000 sdevelo-0.1/README.md
-drwxrwxr-x   0 xuliao    (1005) xuliao    (1005)        0 2024-04-09 12:02:46.143397 sdevelo-0.1/sdevelo/
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      182 2024-04-09 11:34:16.000000 sdevelo-0.1/sdevelo/__init__.py
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     1376 2024-04-09 11:39:16.000000 sdevelo-0.1/sdevelo/_config.py
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)    17982 2024-04-09 11:20:02.000000 sdevelo-0.1/sdevelo/_model.py
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     2839 2024-04-09 11:46:29.000000 sdevelo-0.1/sdevelo/_pl.py
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     4339 2024-04-09 11:18:47.000000 sdevelo-0.1/sdevelo/_sim.py
-drwxrwxr-x   0 xuliao    (1005) xuliao    (1005)        0 2024-04-09 12:02:46.143397 sdevelo-0.1/sdevelo.egg-info/
--rw-r--r--   0 xuliao    (1005) xuliao    (1005)     1418 2024-04-09 12:02:46.000000 sdevelo-0.1/sdevelo.egg-info/PKG-INFO
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      268 2024-04-09 12:02:46.000000 sdevelo-0.1/sdevelo.egg-info/SOURCES.txt
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)        1 2024-04-09 12:02:46.000000 sdevelo-0.1/sdevelo.egg-info/dependency_links.txt
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      105 2024-04-09 12:02:46.000000 sdevelo-0.1/sdevelo.egg-info/requires.txt
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)        8 2024-04-09 12:02:46.000000 sdevelo-0.1/sdevelo.egg-info/top_level.txt
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)       38 2024-04-09 12:02:46.143397 sdevelo-0.1/setup.cfg
--rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     1117 2024-04-09 12:02:42.000000 sdevelo-0.1/setup.py
+drwxrwxr-x   0 xuliao    (1005) xuliao    (1005)        0 2024-04-09 12:17:18.379430 sdevelo-0.1.1/
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     1082 2024-04-09 11:56:43.000000 sdevelo-0.1.1/LICENSE
+-rw-r--r--   0 xuliao    (1005) xuliao    (1005)     1367 2024-04-09 12:17:18.379430 sdevelo-0.1.1/PKG-INFO
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      620 2024-04-04 05:41:59.000000 sdevelo-0.1.1/README.md
+drwxrwxr-x   0 xuliao    (1005) xuliao    (1005)        0 2024-04-09 12:17:18.375430 sdevelo-0.1.1/sdevelo/
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      182 2024-04-09 11:34:16.000000 sdevelo-0.1.1/sdevelo/__init__.py
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     1376 2024-04-09 11:39:16.000000 sdevelo-0.1.1/sdevelo/_config.py
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)    17982 2024-04-09 11:20:02.000000 sdevelo-0.1.1/sdevelo/_model.py
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     2839 2024-04-09 11:46:29.000000 sdevelo-0.1.1/sdevelo/_pl.py
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     4339 2024-04-09 11:18:47.000000 sdevelo-0.1.1/sdevelo/_sim.py
+drwxrwxr-x   0 xuliao    (1005) xuliao    (1005)        0 2024-04-09 12:17:18.379430 sdevelo-0.1.1/sdevelo.egg-info/
+-rw-r--r--   0 xuliao    (1005) xuliao    (1005)     1367 2024-04-09 12:17:18.000000 sdevelo-0.1.1/sdevelo.egg-info/PKG-INFO
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)      268 2024-04-09 12:17:18.000000 sdevelo-0.1.1/sdevelo.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)        1 2024-04-09 12:17:18.000000 sdevelo-0.1.1/sdevelo.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)       52 2024-04-09 12:17:18.000000 sdevelo-0.1.1/sdevelo.egg-info/requires.txt
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)        8 2024-04-09 12:17:18.000000 sdevelo-0.1.1/sdevelo.egg-info/top_level.txt
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)       38 2024-04-09 12:17:18.379430 sdevelo-0.1.1/setup.cfg
+-rw-rw-r--   0 xuliao    (1005) xuliao    (1005)     1066 2024-04-09 12:17:01.000000 sdevelo-0.1.1/setup.py
```

### Comparing `sdevelo-0.1/LICENSE` & `sdevelo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevelo-0.1/PKG-INFO` & `sdevelo-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sdevelo
-Version: 0.1
+Version: 0.1.1
 Summary: SDEvelo: a deep generative approach for transcriptional dynamics with cell-specific latent time and multivariate stochastic modeling
 Home-page: https://github.com/Liao-Xu/SDEvelo
 Author: Xu Liao
 Author-email: xu.smooth.liao@gmail.com
 License: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anndata>=0.10.7
-Requires-Dist: matplotlib>=3.7.1
-Requires-Dist: numpy>=1.23.5
-Requires-Dist: scipy>=1.8.1
-Requires-Dist: scvelo>=0.2.5
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: torch>=1.13.1
+Requires-Dist: anndata
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scvelo
+Requires-Dist: seaborn
+Requires-Dist: torch
 
 # SDEvelo: a deep generative approach for transcriptional dynamics with cell-specific latent time and multivariate stochastic modeling
 
 ## Overview
 
 SDEvelo leverages advanced stochastic differential equations (SDE) to provide a novel approach to RNA velocity analysis in single-cell RNA sequencing (scRNA-seq). This deep generative model accurately captures the complex, stochastic nature of transcriptional dynamics, offering new insights into cell differentiation and state transitions.
```

### Comparing `sdevelo-0.1/README.md` & `sdevelo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sdevelo-0.1/sdevelo/_config.py` & `sdevelo-0.1.1/sdevelo/_config.py`

 * *Files identical despite different names*

### Comparing `sdevelo-0.1/sdevelo/_model.py` & `sdevelo-0.1.1/sdevelo/_model.py`

 * *Files identical despite different names*

### Comparing `sdevelo-0.1/sdevelo/_pl.py` & `sdevelo-0.1.1/sdevelo/_pl.py`

 * *Files identical despite different names*

### Comparing `sdevelo-0.1/sdevelo/_sim.py` & `sdevelo-0.1.1/sdevelo/_sim.py`

 * *Files identical despite different names*

### Comparing `sdevelo-0.1/sdevelo.egg-info/PKG-INFO` & `sdevelo-0.1.1/sdevelo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sdevelo
-Version: 0.1
+Version: 0.1.1
 Summary: SDEvelo: a deep generative approach for transcriptional dynamics with cell-specific latent time and multivariate stochastic modeling
 Home-page: https://github.com/Liao-Xu/SDEvelo
 Author: Xu Liao
 Author-email: xu.smooth.liao@gmail.com
 License: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anndata>=0.10.7
-Requires-Dist: matplotlib>=3.7.1
-Requires-Dist: numpy>=1.23.5
-Requires-Dist: scipy>=1.8.1
-Requires-Dist: scvelo>=0.2.5
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: torch>=1.13.1
+Requires-Dist: anndata
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scvelo
+Requires-Dist: seaborn
+Requires-Dist: torch
 
 # SDEvelo: a deep generative approach for transcriptional dynamics with cell-specific latent time and multivariate stochastic modeling
 
 ## Overview
 
 SDEvelo leverages advanced stochastic differential equations (SDE) to provide a novel approach to RNA velocity analysis in single-cell RNA sequencing (scRNA-seq). This deep generative model accurately captures the complex, stochastic nature of transcriptional dynamics, offering new insights into cell differentiation and state transitions.
```

### Comparing `sdevelo-0.1/setup.py` & `sdevelo-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sdevelo",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
-        'anndata>=0.10.7',
-        'matplotlib>=3.7.1', 
-        'numpy>=1.23.5', 
-        'scipy>=1.8.1', 
-        'scvelo>=0.2.5', 
-        'seaborn>=0.11.2', 
-        'torch>=1.13.1'
+        'anndata',
+        'matplotlib', 
+        'numpy', 
+        'scipy', 
+        'scvelo', 
+        'seaborn', 
+        'torch'
     ],
     author="Xu Liao",
     author_email="xu.smooth.liao@gmail.com",
     description="SDEvelo: a deep generative approach for transcriptional dynamics with cell-specific latent time and multivariate stochastic modeling",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/Liao-Xu/SDEvelo",
```

