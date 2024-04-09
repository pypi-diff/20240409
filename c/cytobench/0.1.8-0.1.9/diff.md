# Comparing `tmp/cytobench-0.1.8.tar.gz` & `tmp/cytobench-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytobench-0.1.8.tar", last modified: Wed Jan 31 09:10:26 2024, max compression
+gzip compressed data, was "cytobench-0.1.9.tar", last modified: Wed Jan 31 09:13:25 2024, max compression
```

## Comparing `cytobench-0.1.8.tar` & `cytobench-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2024-01-31 09:10:26.670956 cytobench-0.1.8/
--rw-r--r--   0 nico       (501) staff       (20)        0 2024-01-30 19:40:03.000000 cytobench-0.1.8/LICENSE
--rw-r--r--   0 nico       (501) staff       (20)      689 2024-01-31 09:10:26.670704 cytobench-0.1.8/PKG-INFO
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2024-01-31 09:10:26.669267 cytobench-0.1.8/cytobench/
--rw-r--r--   0 nico       (501) staff       (20)     2370 2024-01-31 09:09:49.000000 cytobench-0.1.8/cytobench/__init__.py
--rw-r--r--   0 nico       (501) staff       (20)     2170 2024-01-29 09:41:16.000000 cytobench-0.1.8/cytobench/cytobench.py
--rw-r--r--   0 nico       (501) staff       (20)     2445 2024-01-31 09:09:35.000000 cytobench-0.1.8/cytobench/datasets_manager.py
--rw-r--r--   0 nico       (501) staff       (20)     8757 2024-01-18 09:51:52.000000 cytobench-0.1.8/cytobench/train_validators.py
--rw-r--r--   0 nico       (501) staff       (20)     5713 2024-01-18 08:17:59.000000 cytobench-0.1.8/cytobench/validation_functions.py
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2024-01-31 09:10:26.670416 cytobench-0.1.8/cytobench.egg-info/
--rw-r--r--   0 nico       (501) staff       (20)      689 2024-01-31 09:10:26.000000 cytobench-0.1.8/cytobench.egg-info/PKG-INFO
--rw-r--r--   0 nico       (501) staff       (20)      319 2024-01-31 09:10:26.000000 cytobench-0.1.8/cytobench.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (501) staff       (20)        1 2024-01-31 09:10:26.000000 cytobench-0.1.8/cytobench.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (501) staff       (20)       86 2024-01-31 09:10:26.000000 cytobench-0.1.8/cytobench.egg-info/requires.txt
--rw-r--r--   0 nico       (501) staff       (20)       10 2024-01-31 09:10:26.000000 cytobench-0.1.8/cytobench.egg-info/top_level.txt
--rw-r--r--   0 nico       (501) staff       (20)       38 2024-01-31 09:10:26.671013 cytobench-0.1.8/setup.cfg
--rw-r--r--   0 nico       (501) staff       (20)      879 2024-01-31 09:10:08.000000 cytobench-0.1.8/setup.py
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2024-01-31 09:13:25.598999 cytobench-0.1.9/
+-rw-r--r--   0 nico       (501) staff       (20)        0 2024-01-30 19:40:03.000000 cytobench-0.1.9/LICENSE
+-rw-r--r--   0 nico       (501) staff       (20)      689 2024-01-31 09:13:25.598766 cytobench-0.1.9/PKG-INFO
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2024-01-31 09:13:25.589090 cytobench-0.1.9/cytobench/
+-rw-r--r--   0 nico       (501) staff       (20)     2370 2024-01-31 09:09:49.000000 cytobench-0.1.9/cytobench/__init__.py
+-rw-r--r--   0 nico       (501) staff       (20)     2170 2024-01-29 09:41:16.000000 cytobench-0.1.9/cytobench/cytobench.py
+-rw-r--r--   0 nico       (501) staff       (20)     2445 2024-01-31 09:09:35.000000 cytobench-0.1.9/cytobench/datasets_manager.py
+-rw-r--r--   0 nico       (501) staff       (20)     8757 2024-01-18 09:51:52.000000 cytobench-0.1.9/cytobench/train_validators.py
+-rw-r--r--   0 nico       (501) staff       (20)     5713 2024-01-18 08:17:59.000000 cytobench-0.1.9/cytobench/validation_functions.py
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2024-01-31 09:13:25.598503 cytobench-0.1.9/cytobench.egg-info/
+-rw-r--r--   0 nico       (501) staff       (20)      689 2024-01-31 09:13:25.000000 cytobench-0.1.9/cytobench.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (501) staff       (20)      319 2024-01-31 09:13:25.000000 cytobench-0.1.9/cytobench.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (501) staff       (20)        1 2024-01-31 09:13:25.000000 cytobench-0.1.9/cytobench.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (501) staff       (20)       86 2024-01-31 09:13:25.000000 cytobench-0.1.9/cytobench.egg-info/requires.txt
+-rw-r--r--   0 nico       (501) staff       (20)       10 2024-01-31 09:13:25.000000 cytobench-0.1.9/cytobench.egg-info/top_level.txt
+-rw-r--r--   0 nico       (501) staff       (20)       38 2024-01-31 09:13:25.599050 cytobench-0.1.9/setup.cfg
+-rw-r--r--   0 nico       (501) staff       (20)      879 2024-01-31 09:13:20.000000 cytobench-0.1.9/setup.py
```

### Comparing `cytobench-0.1.8/PKG-INFO` & `cytobench-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cytobench
-Version: 0.1.8
+Version: 0.1.9
 Summary: Benchmarking library for generative algorithms in omics data
 Author: Nicolo' Lazzaro
 Author-email: nlazzaro@fbk.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy==1.26.3
+Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scipy==1.11.4
 Requires-Dist: xgboost==2.0.3
-Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: requests
 
 Install environment and test
 
 ```
 mamba create -n cbtest --file library/requirements.txt
 mamba activate cbtest
```

### Comparing `cytobench-0.1.8/cytobench/__init__.py` & `cytobench-0.1.9/cytobench/__init__.py`

 * *Files identical despite different names*

### Comparing `cytobench-0.1.8/cytobench/cytobench.py` & `cytobench-0.1.9/cytobench/cytobench.py`

 * *Files identical despite different names*

### Comparing `cytobench-0.1.8/cytobench/datasets_manager.py` & `cytobench-0.1.9/cytobench/datasets_manager.py`

 * *Files identical despite different names*

### Comparing `cytobench-0.1.8/cytobench/train_validators.py` & `cytobench-0.1.9/cytobench/train_validators.py`

 * *Files identical despite different names*

### Comparing `cytobench-0.1.8/cytobench/validation_functions.py` & `cytobench-0.1.9/cytobench/validation_functions.py`

 * *Files identical despite different names*

### Comparing `cytobench-0.1.8/cytobench.egg-info/PKG-INFO` & `cytobench-0.1.9/cytobench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cytobench
-Version: 0.1.8
+Version: 0.1.9
 Summary: Benchmarking library for generative algorithms in omics data
 Author: Nicolo' Lazzaro
 Author-email: nlazzaro@fbk.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy==1.26.3
+Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scipy==1.11.4
 Requires-Dist: xgboost==2.0.3
-Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: requests
 
 Install environment and test
 
 ```
 mamba create -n cbtest --file library/requirements.txt
 mamba activate cbtest
```

### Comparing `cytobench-0.1.8/setup.py` & `cytobench-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cytobench',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=[
-        'numpy==1.26.3',
+        'numpy==1.23.5',
         'pandas==1.5.3',
         'scipy==1.11.4',
         'xgboost==2.0.3',
-        'scikit-learn==1.3.2',
+        'scikit-learn==1.2.2',
         'requests',
     ],
     author="Nicolo' Lazzaro",
     author_email='nlazzaro@fbk.eu',
     description='Benchmarking library for generative algorithms in omics data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

