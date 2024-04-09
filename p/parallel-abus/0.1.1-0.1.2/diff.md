# Comparing `tmp/parallel_abus-0.1.1.tar.gz` & `tmp/parallel_abus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_abus-0.1.1.tar", max compression
+gzip compressed data, was "parallel_abus-0.1.2.tar", max compression
```

## Comparing `parallel_abus-0.1.1.tar` & `parallel_abus-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1104 2024-04-02 10:35:02.938466 parallel_abus-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2370 2024-04-09 08:54:26.351117 parallel_abus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2605 2024-04-09 07:54:09.517295 parallel_abus-0.1.1/README.md
--rw-r--r--   0        0        0      129 2024-04-09 08:54:44.671121 parallel_abus-0.1.1/src/parallel_abus/__about__.py
--rw-r--r--   0        0        0      304 2024-04-02 13:31:38.451309 parallel_abus-0.1.1/src/parallel_abus/__init__.py
--rw-r--r--   0        0        0      131 2024-04-02 13:29:22.280399 parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/__init__.py
--rw-r--r--   0        0        0     7253 2024-04-05 11:34:18.821568 parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aBUS_SuS.py
--rw-r--r--   0        0        0    14769 2024-04-09 07:55:09.770573 parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aBUS_SuS_parallel.py
--rw-r--r--   0        0        0     6458 2021-03-29 06:00:00.000000 parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aCS_aBUS.py
--rw-r--r--   0        0        0    27510 2024-04-03 13:14:34.810397 parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aCS_aBUS_parallel.py
--rw-r--r--   0        0        0     1491 2024-04-02 13:01:41.077011 parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/utils.py
--rw-r--r--   0        0        0       60 2024-04-02 12:56:21.933155 parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/__init__.py
--rw-r--r--   0        0        0    26625 2022-01-17 16:00:00.000000 parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERACond.py
--rw-r--r--   0        0        0    49000 2024-04-02 13:21:46.638964 parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERADist.py
--rw-r--r--   0        0        0    18989 2023-05-12 12:24:45.000000 parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERANataf.py
--rw-r--r--   0        0        0    14502 2022-01-17 16:00:00.000000 parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERARosen.py
--rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 parallel_abus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-04-02 10:35:02.938466 parallel_abus-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2372 2024-04-09 09:14:21.755861 parallel_abus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2603 2024-04-09 09:14:44.574880 parallel_abus-0.1.2/README.md
+-rw-r--r--   0        0        0      129 2024-04-09 09:14:20.162866 parallel_abus-0.1.2/src/parallel_abus/__about__.py
+-rw-r--r--   0        0        0      304 2024-04-02 13:31:38.451309 parallel_abus-0.1.2/src/parallel_abus/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-02 13:29:22.280399 parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/__init__.py
+-rw-r--r--   0        0        0     7253 2024-04-05 11:34:18.821568 parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aBUS_SuS.py
+-rw-r--r--   0        0        0    14769 2024-04-09 07:55:09.770573 parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aBUS_SuS_parallel.py
+-rw-r--r--   0        0        0     6458 2021-03-29 06:00:00.000000 parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aCS_aBUS.py
+-rw-r--r--   0        0        0    27510 2024-04-03 13:14:34.810397 parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aCS_aBUS_parallel.py
+-rw-r--r--   0        0        0     1491 2024-04-02 13:01:41.077011 parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/utils.py
+-rw-r--r--   0        0        0       60 2024-04-02 12:56:21.933155 parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/__init__.py
+-rw-r--r--   0        0        0    26625 2022-01-17 16:00:00.000000 parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERACond.py
+-rw-r--r--   0        0        0    49000 2024-04-02 13:21:46.638964 parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERADist.py
+-rw-r--r--   0        0        0    18989 2023-05-12 12:24:45.000000 parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERANataf.py
+-rw-r--r--   0        0        0    14502 2022-01-17 16:00:00.000000 parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERARosen.py
+-rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 parallel_abus-0.1.2/PKG-INFO
```

### Comparing `parallel_abus-0.1.1/LICENSE.txt` & `parallel_abus-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/pyproject.toml` & `parallel_abus-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # requires = ["hatchling"]
 # build-backend = "hatchling.build"
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "parallel-abus"
-version = "0.1.1"
+version = "0.1.2"
 description = ''
 readme = "README.md"
 # requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   " Patrick Simon <patrick.simon@bam.de>",
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
+  # "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `parallel_abus-0.1.1/README.md` & `parallel_abus-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 Usage is exemplified in the corresponding GitHub project of this package.
 
 Examples using this package are documented in the `./tests/` folder. The number of processes can be specified as a command line parameter, for example:
 
 ```console
 python ./tests/test_main_example_3_2DOF.py 5
 ```
-
-Runs inference with parallel aBUS on 5 processes.
+runs inference with parallel aBUS on 5 processes.
 
 
 A more comprehensive example is presented in `./example/bayesian_inference.py`. Here, an engineering model of a reinforced concrete beam including an OpenSees finite element model is updated. Details on this example are found in this contribution:
 
 > Simon, P., Schneider, R., Baeßler, M., Morgenthal, G., 2024. A Bayesian probabilistic framework for building models for structural health monitoring of structures subject to environmental variability. (submitted for publication).
 
 This example requires amongst others the [python package for OpenSees](https://openseespydoc.readthedocs.io/en/latest/index.html).
```

### Comparing `parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aBUS_SuS.py` & `parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aBUS_SuS.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aBUS_SuS_parallel.py` & `parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aBUS_SuS_parallel.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aCS_aBUS.py` & `parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aCS_aBUS.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/aCS_aBUS_parallel.py` & `parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/aCS_aBUS_parallel.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/aBUS_SuS/utils.py` & `parallel_abus-0.1.2/src/parallel_abus/aBUS_SuS/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERACond.py` & `parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERACond.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERADist.py` & `parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERADist.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERANataf.py` & `parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERANataf.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/src/parallel_abus/ERADistNataf/ERARosen.py` & `parallel_abus-0.1.2/src/parallel_abus/ERADistNataf/ERARosen.py`

 * *Files identical despite different names*

### Comparing `parallel_abus-0.1.1/PKG-INFO` & `parallel_abus-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: parallel-abus
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author:  Patrick Simon
 Author-email: patrick.simon@bam.de
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -68,16 +67,15 @@
 Usage is exemplified in the corresponding GitHub project of this package.
 
 Examples using this package are documented in the `./tests/` folder. The number of processes can be specified as a command line parameter, for example:
 
 ```console
 python ./tests/test_main_example_3_2DOF.py 5
 ```
-
-Runs inference with parallel aBUS on 5 processes.
+runs inference with parallel aBUS on 5 processes.
 
 
 A more comprehensive example is presented in `./example/bayesian_inference.py`. Here, an engineering model of a reinforced concrete beam including an OpenSees finite element model is updated. Details on this example are found in this contribution:
 
 > Simon, P., Schneider, R., Baeßler, M., Morgenthal, G., 2024. A Bayesian probabilistic framework for building models for structural health monitoring of structures subject to environmental variability. (submitted for publication).
 
 This example requires amongst others the [python package for OpenSees](https://openseespydoc.readthedocs.io/en/latest/index.html).
```

