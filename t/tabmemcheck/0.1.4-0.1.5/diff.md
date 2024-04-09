# Comparing `tmp/tabmemcheck-0.1.4.tar.gz` & `tmp/tabmemcheck-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabmemcheck-0.1.4.tar", last modified: Tue Jan  9 16:34:03 2024, max compression
+gzip compressed data, was "tabmemcheck-0.1.5.tar", last modified: Tue Apr  9 13:20:59 2024, max compression
```

## Comparing `tabmemcheck-0.1.4.tar` & `tabmemcheck-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,57 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.632913 tabmemcheck-0.1.4/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1068 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      173 2024-01-09 16:25:47.000000 tabmemcheck-0.1.4/MANIFEST.in
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    13061 2024-01-09 16:34:03.632913 tabmemcheck-0.1.4/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12551 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      107 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2024-01-09 16:34:03.632913 tabmemcheck-0.1.4/setup.cfg
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1383 2024-01-09 16:33:49.000000 tabmemcheck-0.1.4/setup.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.624913 tabmemcheck-0.1.4/tabmemcheck/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1417 2024-01-09 16:25:47.000000 tabmemcheck-0.1.4/tabmemcheck/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12056 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/analysis.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    13520 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/chat_completion.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10240 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/cli_interface.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    23833 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/datasets.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    25892 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/functions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14166 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/llm.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.624913 tabmemcheck-0.1.4/tabmemcheck/resources/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/__init__.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.624913 tabmemcheck-0.1.4/tabmemcheck/resources/config/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/config/__init__.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.632913 tabmemcheck-0.1.4/tabmemcheck/resources/csv/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)  3811651 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/adult-train.csv
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)  1423529 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/california-housing.csv
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4466 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/iris.csv
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    23105 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/openml-diabetes.csv
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    60302 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/titanic-train.csv
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10959 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/csv/uci-wine.csv
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2064 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/resources/system-prompts.yaml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7337 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/row_independence.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10895 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/tests.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    17369 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tabmemcheck/utils.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       21 2024-01-09 16:33:54.000000 tabmemcheck-0.1.4/tabmemcheck/version.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.632913 tabmemcheck-0.1.4/tabmemcheck.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    13061 2024-01-09 16:34:03.000000 tabmemcheck-0.1.4/tabmemcheck.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1308 2024-01-09 16:34:03.000000 tabmemcheck-0.1.4/tabmemcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2024-01-09 16:34:03.000000 tabmemcheck-0.1.4/tabmemcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       63 2024-01-09 16:34:03.000000 tabmemcheck-0.1.4/tabmemcheck.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      100 2024-01-09 16:34:03.000000 tabmemcheck-0.1.4/tabmemcheck.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       12 2024-01-09 16:34:03.000000 tabmemcheck-0.1.4/tabmemcheck.egg-info/top_level.txt
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-01-09 16:34:03.632913 tabmemcheck-0.1.4/tests/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      787 2023-12-17 15:15:10.000000 tabmemcheck-0.1.4/tests/test_header.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.246366 tabmemcheck-0.1.5/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1068 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      173 2024-01-09 16:25:47.000000 tabmemcheck-0.1.5/MANIFEST.in
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    13752 2024-04-09 13:20:59.246366 tabmemcheck-0.1.5/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12970 2024-04-06 11:45:43.000000 tabmemcheck-0.1.5/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      107 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2024-04-09 13:20:59.246366 tabmemcheck-0.1.5/setup.cfg
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1289 2024-04-02 14:42:32.000000 tabmemcheck-0.1.5/setup.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.226367 tabmemcheck-0.1.5/tabmemcheck/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1653 2024-04-04 14:04:51.000000 tabmemcheck-0.1.5/tabmemcheck/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12591 2024-04-05 10:14:50.000000 tabmemcheck-0.1.5/tabmemcheck/analysis.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    15000 2024-04-05 19:16:20.000000 tabmemcheck-0.1.5/tabmemcheck/chat_completion.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.226367 tabmemcheck-0.1.5/tabmemcheck/datasets/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      293 2024-04-04 13:42:09.000000 tabmemcheck-0.1.5/tabmemcheck/datasets/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    13446 2024-04-04 15:40:00.000000 tabmemcheck-0.1.5/tabmemcheck/datasets/load.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14724 2024-04-03 18:14:42.000000 tabmemcheck-0.1.5/tabmemcheck/datasets/transform.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    27037 2024-04-06 15:42:35.000000 tabmemcheck-0.1.5/tabmemcheck/functions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    17000 2024-04-06 15:50:57.000000 tabmemcheck-0.1.5/tabmemcheck/llm.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.226367 tabmemcheck-0.1.5/tabmemcheck/resources/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/__init__.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.226367 tabmemcheck-0.1.5/tabmemcheck/resources/config/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2064 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/system-prompts.yaml
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.234367 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4673 2024-03-05 12:58:04.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/acs-income.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5386 2024-03-18 15:58:27.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/acs-travel.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4033 2024-03-08 15:19:54.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/adult.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1204 2024-02-19 14:54:22.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/california-housing.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2439 2024-03-11 16:49:36.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/fico.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1141 2024-03-19 11:11:06.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/icu.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      844 2024-02-19 12:26:43.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/iris.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1150 2024-03-11 13:12:23.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/openml-diabetes.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)   315387 2024-03-24 15:18:08.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/spaceship-titanic.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    58140 2024-03-19 13:40:11.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/titanic.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1627 2024-02-20 14:32:22.000000 tabmemcheck-0.1.5/tabmemcheck/resources/config/transform/wine.yaml
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.242367 tabmemcheck-0.1.5/tabmemcheck/resources/csv/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/csv/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)  3811651 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/csv/adult-train.csv
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)  1423529 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/csv/california-housing.csv
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4466 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/csv/iris.csv
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    23105 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/csv/openml-diabetes.csv
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10959 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/resources/csv/uci-wine.csv
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7337 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/row_independence.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10895 2023-12-17 15:15:10.000000 tabmemcheck-0.1.5/tabmemcheck/tests.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    22110 2024-04-09 13:17:43.000000 tabmemcheck-0.1.5/tabmemcheck/utils.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       22 2024-04-02 14:34:11.000000 tabmemcheck-0.1.5/tabmemcheck/version.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.242367 tabmemcheck-0.1.5/tabmemcheck.egg-info/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)    13752 2024-04-09 13:20:59.000000 tabmemcheck-0.1.5/tabmemcheck.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2540 2024-04-09 13:20:59.000000 tabmemcheck-0.1.5/tabmemcheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2024-04-09 13:20:59.000000 tabmemcheck-0.1.5/tabmemcheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      107 2024-04-09 13:20:59.000000 tabmemcheck-0.1.5/tabmemcheck.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       12 2024-04-09 13:20:59.000000 tabmemcheck-0.1.5/tabmemcheck.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-09 13:20:59.246366 tabmemcheck-0.1.5/tests/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      430 2024-04-02 13:59:01.000000 tabmemcheck-0.1.5/tests/test_datasets.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      314 2024-04-03 20:44:36.000000 tabmemcheck-0.1.5/tests/test_header.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      305 2024-02-09 21:34:22.000000 tabmemcheck-0.1.5/tests/testutils.py
```

### Comparing `tabmemcheck-0.1.4/LICENSE` & `tabmemcheck-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/PKG-INFO` & `tabmemcheck-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: tabmemcheck
-Version: 0.1.4
-Summary: Testing Language Models for Memorization of Tabular Data
-Home-page: https://github.com/interpretml/LLM-Tabular-Memorization-Checker
-Author: Sebastian Bordt, Harsha Nori, Rich Caruana
-Author-email: sbordt@posteo.de
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🐘 Testing Language Models for Memorization of Tabular Data
-![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+![PyPI - Version](https://img.shields.io/pypi/v/tabmemcheck)
 ![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
-
-This open-source package provides different functions to test LLMs for memorization and prior experience with tabular datasets. 
+![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+[![tests](https://github.com/interpretml/LLM-Tabular-Memorization-Checker/actions/workflows/run_tests.yaml/badge.svg?branch=main)](https://github.com/interpretml/LLM-Tabular-Memorization-Checker/actions/workflows/run_tests.yaml)
+[![Documentation](https://img.shields.io/badge/Documentation-View-blue)](http://interpret.ml/LLM-Tabular-Memorization-Checker/)
 
 
+This open-source package provides different functions to test LLMs for memorization and prior experience with tabular datasets. 
+ 
 Features:
 - [x] Test GPT-3.5, GPT-4, and other LLMs for prior experience with tabular datasets.
 - [x] Supports chat models and (base) language models. In chat mode, the prompts are designed toward GPT-3.5 and GPT-4. With other LLMs, we recommend to test the base models. 
 - [x] Based entirely on prompts (no access to the probability distribution over tokens ('logprobs') is required).
 - [x] Provides a CLI tool that works with the OpenAI API.
 
 For details, take a look at our [paper](https://openreview.net/pdf?id=l1u7jA60wT) Bordt et al., "Elephants Never Forget: Testing Language Models for Memorization of Tabular Data", NeurIPS 2023 Second Table Representation Learning Workshop.
```

### Comparing `tabmemcheck-0.1.4/README.md` & `tabmemcheck-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,42 @@
+Metadata-Version: 2.1
+Name: tabmemcheck
+Version: 0.1.5
+Summary: Testing Language Models for Memorization of Tabular Data
+Home-page: https://github.com/interpretml/LLM-Tabular-Memorization-Checker
+Author: Sebastian Bordt, Harsha Nori, Rich Caruana
+Author-email: sbordt@posteo.de
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scikit-learn
+Requires-Dist: xgboost
+Requires-Dist: scipy
+Requires-Dist: pandas>=2.1.0
+Requires-Dist: tiktoken
+Requires-Dist: openai>=1.3.3
+Requires-Dist: tenacity
+Requires-Dist: jellyfish
+Requires-Dist: pyyaml
+
 # 🐘 Testing Language Models for Memorization of Tabular Data
-![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+![PyPI - Version](https://img.shields.io/pypi/v/tabmemcheck)
 ![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
-
-This open-source package provides different functions to test LLMs for memorization and prior experience with tabular datasets. 
+![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+[![tests](https://github.com/interpretml/LLM-Tabular-Memorization-Checker/actions/workflows/run_tests.yaml/badge.svg?branch=main)](https://github.com/interpretml/LLM-Tabular-Memorization-Checker/actions/workflows/run_tests.yaml)
+[![Documentation](https://img.shields.io/badge/Documentation-View-blue)](http://interpret.ml/LLM-Tabular-Memorization-Checker/)
 
 
+This open-source package provides different functions to test LLMs for memorization and prior experience with tabular datasets. 
+ 
 Features:
 - [x] Test GPT-3.5, GPT-4, and other LLMs for prior experience with tabular datasets.
 - [x] Supports chat models and (base) language models. In chat mode, the prompts are designed toward GPT-3.5 and GPT-4. With other LLMs, we recommend to test the base models. 
 - [x] Based entirely on prompts (no access to the probability distribution over tokens ('logprobs') is required).
 - [x] Provides a CLI tool that works with the OpenAI API.
 
 For details, take a look at our [paper](https://openreview.net/pdf?id=l1u7jA60wT) Bordt et al., "Elephants Never Forget: Testing Language Models for Memorization of Tabular Data", NeurIPS 2023 Second Table Representation Learning Workshop.
```

### Comparing `tabmemcheck-0.1.4/setup.py` & `tabmemcheck-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,43 +9,40 @@
 version = {}
 with open("tabmemcheck/version.py") as fp:
     exec(fp.read(), version)
 
 
 setuptools.setup(
     name="tabmemcheck",
-    version=version['__version__'],
+    version=version["__version__"],
     author="Sebastian Bordt, Harsha Nori, Rich Caruana",
     author_email="sbordt@posteo.de",
     description="Testing Language Models for Memorization of Tabular Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/interpretml/LLM-Tabular-Memorization-Checker",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "."},
     packages=find_packages(),
     package_data={
-        '': ['*.yaml', '*.csv'],
+        "": ["*.yaml", "*.csv"],
     },
     include_package_data=True,
     python_requires=">=3.9",
-    entry_points={
-        "console_scripts": ["tabmemcheck=tabmemcheck.cli_interface:main"],
-    },
     install_requires=[
         "numpy",
         "matplotlib",
         "scikit-learn",
         "xgboost",
         "scipy",
-        "pandas",
+        "pandas>=2.1.0",
         "tiktoken",
         "openai>=1.3.3",
         "tenacity",
         "jellyfish",
         "pyyaml",
     ],
 )
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck/__init__.py` & `tabmemcheck-0.1.5/tabmemcheck/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,65 @@
 # llm interface
-from .llm import LLM_Interface, openai_setup
+from .llm import (
+    LLM_Interface,
+    openai_setup,
+    gemini_setup,
+    send_chat_completion,
+    send_completion,
+)
+
+# logging
+from .llm import set_logging_task, read_chatlog
 
 # the different tests
 from .functions import (
     run_all_tests,
     header_test,
     feature_names_test,
     row_completion_test,
     feature_completion_test,
     first_token_test,
     sample,
 )
 
+# data loading and transform
+import tabmemcheck.datasets as datasets
+
 from .version import __version__
 
 
-def load_default_system_prompts():
+def __load_default_system_prompts():
     """Load the default system prompts from the resources folder."""
     import importlib.resources as resources
     import yaml
 
-    with resources.open_text("tabmemcheck.resources", "system-prompts.yaml") as f:
+    with resources.open_text(
+        "tabmemcheck.resources.config", "system-prompts.yaml"
+    ) as f:
         prompts = yaml.load(f, Loader=yaml.FullLoader)
     return prompts
 
 
 # global config object for the module
-class DotDict(dict):
+class __DotDict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
     def __setattr__(self, key, value):
         self[key] = value
 
     def __delattr__(self, key):
         if key in self:
             del self[key]
 
 
-config = DotDict({})
+config = __DotDict({})
 
 # default system prompts from yaml file
-config.system_prompts = load_default_system_prompts()
+config.system_prompts = __load_default_system_prompts()
 
 # default llm options
 config.temperature = 0
 config.max_tokens = 500
 config.sleep = 0.0  # amount of time to sleep after each query to the llm
 
 # default: no prompt/response logging
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck/analysis.py` & `tabmemcheck-0.1.5/tabmemcheck/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 #################################################################
 # test if a response or row is contained in a data frame
 #################################################################
 
 
 def string_strip(x):
-    """ "We always convert all objects (data frames and responses) to strings and strip them of trailing whitespaces."""
+    """Convert the input (dataframe, series, or string) to string and strip trailing whitespaces."""
     # if x is data frame
     if isinstance(x, pd.DataFrame):
         x = x.astype(str)
-        x = x.applymap(lambda x: x.strip())
+        x = x.map(lambda x: x.strip())
     elif isinstance(x, pd.Series):
         x = x.astype(str)
         x = x.apply(lambda x: x.strip())
     elif isinstance(x, str):
         x = x.strip()
     else:
         raise ValueError(f"Unkown type for string_strip: {type(x)}.")
@@ -51,41 +51,45 @@
     assert set(x.columns).issubset(
         set(feature_names)
     ), f"Invalid feature names in x: {set(feature_names) - set(x.columns)}."
     return x
 
 
 def find_matches(
-    df,
+    df: pd.DataFrame,
     x,
     string_dist_fn=utils.levenshtein_distances,
     match_floating_point=True,
     strip_quotation_marks=True,
 ):
-    """find the closest matches in levenshtein distance between x and all rows in df.
+    """Find the closest matches between a row x and all rows in the dataframe df. By default, we use the levenshtein distance as the distance metric.
 
-    the important aspect of this function is that it handles a variety of formatting differences between the values in the original data
-    and model responses that should still be counted as equal.
+    This function can handle a variety of formatting differences between the values in the original data
+    and LLM responses that should still be counted as equal.
 
-    match_floating_point: if True, handes floating point formatting differences, e.g. 0.28 vs. .280 or 172 vs 172.0 (default: True).
-    strip_quotation_marks: if True, strips quotation marks from the values in df and x (to handle the case where a model responds with "23853", and the value in the data is 23853) (default: True).
 
-    x can be a string, a pandas dataframe or a pandas Series.
+    :param df: a pandas dataframe.
+    :param x: a string, a pandas dataframe or a pandas Series.
+    :param string_dist_fn: a function that computes the distance between two strings. By default, this is the levenshtein distance.
+    :param match_floating_point: if True, handes floating point formatting differences, e.g. 0.28 vs. .280 or 172 vs 172.0 (default: True).
+    :param strip_quotation_marks: if True, strips quotation marks from the values in df and x (to handle the case where a model responds with "23853", and the value in the data is 23853) (default: True).
+
+    :return: the minimum distance and the matching rows in df.
     """
     # x should be a dataframe with a single row, or be convertible to this format
     x = validate_partial_row(x, df.columns)
     # create a deep copy of df
     df = df.copy(deep=True)
     # convert to string & strip both df and x of any leading and trailing whitespaces. this is very important!
     df = string_strip(df)
     x = string_strip(x)
     # optionall, also strip quotation marks
     if strip_quotation_marks:
-        df = df.applymap(lambda x: x.strip('"'))
-        x = x.applymap(lambda x: x.strip('"'))
+        df = df.map(lambda x: x.strip('"'))
+        x = x.map(lambda x: x.strip('"'))
     # for all the features that are present in x, compute the levenshtein distance between the feature value and the respective feature values in df
     D = np.zeros(df.shape[0])
     for feature_name in df.columns:
         if feature_name in x.columns:
             D_feature = np.array(
                 string_dist_fn(x[feature_name].values[0], df[feature_name].tolist())
             )
@@ -97,17 +101,17 @@
                     df_column_float = pd.to_numeric(
                         df[feature_name], errors="coerce"
                     ).tolist()
                     D_feature_float = np.abs(
                         x_value_float - np.array(df_column_float).flatten()
                     )
                     D_feature_float[D_feature_float > 0] = np.inf
-                    D_feature_float[
-                        np.isnan(D_feature_float)
-                    ] = np.inf  # do not propagate NaNs
+                    D_feature_float[np.isnan(D_feature_float)] = (
+                        np.inf
+                    )  # do not propagate NaNs
                     D_feature = np.minimum(D_feature, D_feature_float)
                 except:
                     pass
             # print(feature_name, D_feature)
             D += D_feature
     min_dist = np.min(D)
     return min_dist, df[D == min_dist]
@@ -199,22 +203,20 @@
 
 #################################################################
 # old functions here, maybe move at some point
 #################################################################
 
 
 def levenshtein_distance_t_test(x, y, z, alternative="two-sided", return_dist=False):
-    """Test whether |x-y| < |x-z| in Levenshtein distance using a t-test.
-
-    x must be a list of stings.
-    y and z can be either a list of strings or a list of lists of strings.
+    """Test whether x is closer to y than z in Levenshtein distance using a t-test.
 
-    alternative: argument to scipy.stats.ttest_ind (default: two-sided)
-
-    Returns: scipy.stats._result_classes.TtestResult"""
+    :param x, y, z: a list of strings.
+    :param alternative: the alternative hypothesis, either 'two-sided', 'greater', or 'less'.
+    :return_dist: if True also return the distances between x and y, and x and z.
+    :return: scipy.stats._result_classes.TtestResult"""
     # convert numpy arrays to lists
     if isinstance(x, np.ndarray):
         x = x.tolist()
     if isinstance(y, np.ndarray):
         y = y.tolist()
     if isinstance(z, np.ndarray):
         z = z.tolist()
@@ -248,21 +250,24 @@
     # return results
     if return_dist:
         return test_statistic, dist_x_y, dist_x_z
     return test_statistic
 
 
 def build_first_token(csv_file, verbose=False):
-    """We construct the first token using the first n digits of every row. The usefulness of this approach comes from the fact that in some datasets, the first token might always be the same.
+    """Given a csv file, build a first token that can be used in the first token test.
 
-    NOTE: this does not work if the first token is the id of the row, because the id is not always the same. IS THIS ACTUALLY TRUE?
+    The first token is constructed by taking the first n digits of every row in the csv file (that is, this functions determines the n).
+    Using the first n digits improves upon using the first digit on datasets where the first digit is always the same or contains few distinct values.
 
-    NOTE: we should always do a prediction test with a gbtree / logistic regression to see if the first token is actually random
+    Note: This function does NOT check if the constructed first token is random.
 
-    Returns: the number of digits that make up the first token.
+    :param csv_file: the path to the csv file.
+    :param verbose: if True, print the first tokens and their counts.
+    :return: the number of digits that make up the first token.
     """
     csv_rows = utils.load_csv_rows(csv_file, header=False)
     num_rows = len(csv_rows)
     for num_digits in range(1, 7):
         tokens = [x[:num_digits] for x in csv_rows]
         # count the occurences of each token
         values, counts = np.unique(tokens, return_counts=True)
@@ -272,16 +277,18 @@
             if verbose:
                 print("First tokens:", list(zip(values, counts)))
             return num_digits
     raise ValueError("Failed to construct valid first tokens.")
 
 
 def find_most_unique_feature(csv_file):
-    """Find the feature that have the most unique values. This is useful for the feature completion test.
-    Returns: feature name, fraction of unique values
+    """Given a csv file, find the feature that has the most unique values. This is the default feature used for the feature completion test.
+
+    :param csv_file: the path to the csv file.
+    :return: the name of the most unique feature and the fraction of unique values.
     """
     feature_names = utils.get_feature_names(csv_file)
     df = utils.load_csv_df(csv_file)
     df = string_strip(df)
     # for each feature, compute the number of unique values
     num_unique_values = [
         len(df[feature_name].unique()) for feature_name in feature_names
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck/chat_completion.py` & `tabmemcheck-0.1.5/tabmemcheck/chat_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     llm,
     csv_file,
     system_prompt,
     num_prefix_rows=10,
     num_queries=100,
     few_shot=7,
     out_file=None,
+    print_levenshtein=False,
 ):
     """Row  chat completion task. This task ask the LLM to predict the next row in the
     csv file, given the previous rows. This task is the basis for the row completion
     test, and also for the first token test. Uses prefix_suffix_chat_completion."""
     # assert that few_shot is an integer
     assert isinstance(few_shot, int), "For row completion, few_shot must be an integer."
 
@@ -163,14 +164,15 @@
         llm,
         prefixes,
         suffixes,
         system_prompt,
         few_shot=few_shot,
         num_queries=num_queries,
         out_file=out_file,
+        print_levenshtein=print_levenshtein,
     )
 
     return test_prefixes, test_suffixes, responses
 
 
 def row_completion(
     llm,
@@ -205,28 +207,67 @@
         suffixes.append(suffix)
         responses.append(response)
 
     return prefixes, suffixes, responses
 
 
 ####################################################################################
+# Basic completion with a list of strings.
+####################################################################################
+
+
+def chat_completion(
+    llm: LLM_Interface,
+    strings: list[str],
+    system_prompt: str = "You are a helpful assistant that complets the user's input.",
+    few_shot=5,
+    num_queries=10,
+    print_levenshtein=False,
+    out_file=None,
+    rng=None,
+):
+    """Basic completion with a chat model and a list of strings."""
+    # randomly split the strings into prefixes and suffixes, then use prefix_suffix_chat_completion
+    if rng is None:
+        rng = np.random.default_rng()
+    prefixes = []
+    suffixes = []
+    for s in strings:
+        idx = rng.integers(low=int(len(s) / 3), high=int(2 * len(s) / 3))
+        prefixes.append(s[:idx])
+        suffixes.append(s[idx:])
+    return prefix_suffix_chat_completion(
+        llm,
+        prefixes,
+        suffixes,
+        system_prompt,
+        few_shot,
+        num_queries,
+        print_levenshtein,
+        out_file,
+        rng,
+    )
+
+
+####################################################################################
 # Almost all of the different tests that we perform
 # can be cast in the prompt structue of
 # 'prefix-suffix chat completion'.
 # This is implemented by the following function.
 ####################################################################################
 
 
 def prefix_suffix_chat_completion(
     llm: LLM_Interface,
     prefixes: list[str],
     suffixes: list[str],
     system_prompt: str,
     few_shot=None,
     num_queries=100,
+    print_levenshtein=False,
     out_file=None,
     rng=None,
 ):
     """A basic chat completion function. Takes a list of prefixes and suffixes and a system prompt.
     Sends {num_queries} prompts of the format
 
     System: <system_prompt>
@@ -323,14 +364,20 @@
         test_suffix = suffixes[i_testpoint]
         messages.append({"role": "user", "content": test_prefix})
         response = send_chat_completion(llm, messages)
         # store prefix, suffix and response
         test_prefixes.append(test_prefix)
         test_suffixes.append(test_suffix)
         responses.append(response)
+        # print the levenshtein distance between the true suffix and the response
+        if print_levenshtein:
+            print(
+                "RESPONSE:",
+                utils.levenshtein_cmd(test_suffix, response[: len(test_suffix) + 10]),
+            )
 
     # save the results to file
     if out_file is not None:
         results_df = pd.DataFrame(
             {
                 "prefix": test_prefixes,
                 "suffix": test_suffixes,
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck/functions.py` & `tabmemcheck-0.1.5/tabmemcheck/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     feature_values_chat_completion,
 )
 
 
 DEFAULT_FEW_SHOT_CSV_FILES = [
     "iris.csv",
     "adult-train.csv",
-    "titanic-train.csv",
+    "openml-diabetes.csv",
     "uci-wine.csv",
     "california-housing.csv",
 ]
 
 
 def __difflib_similar(csv_file_1, csv_file_2):
     sm = SequenceMatcher(
@@ -100,16 +100,23 @@
 ####################################################################################
 
 
 def run_all_tests(
     csv_file: str,
     llm: Union[LLM_Interface, str],
     few_shot_csv_files=DEFAULT_FEW_SHOT_CSV_FILES,
-    feature_name=None,
+    unique_feature: str = None,
 ):
+    """Run different tests for memorization and prior experience with the content of the csv file.
+
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param few_shot_csv_files: A list of other csv files to be used as few-shot examples.
+    :param unique_feature: The name of the feature to be used for the feature completion test.
+    """
     llm = __llm_setup(llm)
     few_shot_csv_files = __validate_few_shot_files(csv_file, few_shot_csv_files)
     __print_info(csv_file, llm, few_shot_csv_files)
 
     feature_names_test(csv_file, llm, few_shot_csv_files=few_shot_csv_files)
 
     # todo feature values
@@ -134,15 +141,15 @@
         if len(samples_df) < 10:
             print(f"The model provided {len(samples_df)} valid samples.")
     else:
         print("The model was not able to provide valid samples.")
     tabmem.config.temperature = temp
 
     row_completion_test(csv_file, llm, num_queries=25)
-    feature_completion_test(csv_file, llm, num_queries=25, feature_name=feature_name)
+    feature_completion_test(csv_file, llm, num_queries=25, feature_name=unique_feature)
     first_token_test(csv_file, llm, num_queries=25)
 
 
 ####################################################################################
 # Feature Names
 ####################################################################################
 
@@ -150,25 +157,23 @@
 def feature_names_test(
     csv_file: str,
     llm: Union[LLM_Interface, str],
     num_prefix_features: int = None,
     few_shot_csv_files=DEFAULT_FEW_SHOT_CSV_FILES,
     system_prompt: str = "default",
 ):
-    """Test if the model knows the names of the features.
-
-    The prompt format is:
-        System: <system_prompt>
-        User: Dataset: <dataset_name>
-              Feature 1, Feature 2, ..., Feature n
-        Response: Feature n+1, Feature n+2, ..., Feature m
+    """Test if the model knows the names of the features in a csv file.
 
-    This can be modified in the following ways:
-    - Include few-shot examples from other csv files.
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param num_prefix_features: The number of features given to the model as part of the prompt (defaults to 1/4 of the features).
+    :param few_shot_csv_files: A list of other csv files to be used as few-shot examples.
+    :param system_prompt: The system prompt to be used.
     """
+
     llm = __llm_setup(llm)
     few_shot_csv_files = __validate_few_shot_files(csv_file, few_shot_csv_files)
 
     # default system prompt?
     if system_prompt == "default":
         system_prompt = tabmem.config.system_prompts["feature-names"]
 
@@ -256,18 +261,14 @@
         + ", ".join(feature_names[num_prefix_features:])
         + bcolors.BOLD
         + "\nModel Generation: "
         + bcolors.ENDC
         + response
     )
 
-    # TODO do some sort of evaluation
-    # for example, return true if it completes all but X of the feature names, correcting for upper/lower case
-    # at least do formatted printing of the results
-
 
 ####################################################################################
 # Feature Values
 ####################################################################################
 
 
 ####################################################################################
@@ -278,21 +279,28 @@
 def header_test(
     csv_file: str,
     llm: Union[LLM_Interface, str],
     split_rows: list[int] = [2, 4, 6, 8],
     completion_length: int = 500,
     few_shot_csv_files: list[str] = DEFAULT_FEW_SHOT_CSV_FILES,
     system_prompt: str = "default",
+    verbose: bool = True,
 ):
-    """Header test, using other csv files as few-shot examples.
+    """Header test for memorization.
+
+    We split the csv file at random positions in rows split_rows and performs 1 query for each split. Then we compare the best completion with the actual header.
 
-    Splits the csv file at random positions in rows 2, 4, 6, and 8. Performs 1 query for each split. Reports the best completion.
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param split_rows: The rows at which the csv file is split for the test.
+    :param completion_length: The length of the completions in the few-shot examples (reduce for LLMs with small context windows).
+    :param few_shot_csv_files: A list of other csv files to be used as few-shot examples.
+    :param system_prompt: The system prompt to be used.
 
-    NOTE: This test might fail if the header and rows of the csv file are very long, and the model has a small context window.
-    NOTE: in the end, this is the case for all of our tests :)
+    :return: The header prompt, the actual header completion, and the model response.
     """
     llm = __llm_setup(llm)
     few_shot_csv_files = __validate_few_shot_files(csv_file, few_shot_csv_files)
 
     # default system prompt?
     if system_prompt == "default":
         system_prompt = tabmem.config.system_prompts["header"]
@@ -305,15 +313,15 @@
     few_shot_data = []
     for fs_csv_file in few_shot_csv_files:
         fs_data = utils.load_csv_string(fs_csv_file, header=True)
         few_shot_data.append(fs_data)
 
     # perform the test multiple times, cutting the dataset at random positions in rows split_rows
     num_completions = -1
-    header, completion = None, None
+    header_prompt, llm_completion = None, None
     for i_row in split_rows:
         offset = np.sum([len(row) for row in csv_rows[: i_row - 1]])
         offset += np.random.randint(
             len(csv_rows[i_row]) // 3, 2 * len(csv_rows[i_row]) // 3
         )
         prefixes = [data[:offset]]
         suffixes = [data[offset : offset + completion_length]]
@@ -338,98 +346,72 @@
                 break
         if idx == len(response) - 1 and response[idx] == data[offset + idx]:
             idx += 1  # no disagreement found, set idx to length of the response
 
         # is this the best completion so far?
         if idx > num_completions:
             num_completions = idx
-            header = prefixes[0]
-            completion = response
-
-    # for the printing, we first color all green up to the first disagreement
-    completion_print = bcolors.Green + completion[:num_completions]
-
-    # then color red up to the beginning of the next row, if any
-    remaining_completion = completion[num_completions:]
-    idx = remaining_completion.find("\n")
-    if idx == -1:
-        completion_print += bcolors.Red + remaining_completion
-    else:
-        completion_print += bcolors.Red + remaining_completion[:idx] + "\n"
-        remaining_completion = remaining_completion[idx + 1 :]
-
-        # for all additional rows, green up to the first disagreement, all red after that
-        completion_rows = remaining_completion.split("\n")
-
-        # the corresponding next row in the csv file
-        data_idx = data[len(header) + num_completions :].find("\n")
-        data_rows = data[len(header) + num_completions + data_idx + 1 :].split("\n")
-
-        for completion_row, data_row in zip(completion_rows, data_rows):
-            if completion_row == data_row:
-                completion_print += bcolors.Green + completion_row + "\n"
-                continue
-            # not equal, find the first disagreement
-            idx = -1000
-            for idx, (c, r) in enumerate(zip(data_row, completion_row)):
-                if c != r:
-                    break
-            if idx == len(completion_row) - 1 and completion_row[idx] == data_row[idx]:
-                idx += 1
-            # print first part green, second part red
-            completion_print += (
-                bcolors.Green
-                + completion_row[:idx]
-                + bcolors.Red
-                + completion_row[idx:]
-                + "\n"
-            )
+            header_prompt = prefixes[0]
+            llm_completion = response
+            header_completion = data[offset : offset + len(llm_completion)]
 
-    # remove final new line
-    completion_print = completion_print.rstrip("\n")
-
-    # print the result
-    print(
-        bcolors.BOLD
-        + "Header Test: "
-        + bcolors.ENDC
-        + bcolors.Black
-        + header
-        + completion_print
-        + bcolors.ENDC
-        + bcolors.BOLD
-        + "\nHeader Test Legend:  "
-        + bcolors.ENDC
-        + "Prompt "
-        + bcolors.Green
-        + "Correct "
-        + bcolors.Red
-        + "Incorrect"
-        + bcolors.ENDC
-    )
+    if verbose:  # print test result to console
+        print(
+            bcolors.BOLD
+            + "Header Test: "
+            + bcolors.ENDC
+            + bcolors.Black
+            + header_prompt
+            + utils.levenshtein_cmd(header_completion, llm_completion)
+            + bcolors.ENDC
+            + bcolors.BOLD
+            + "\nHeader Test Legend:  "
+            + bcolors.ENDC
+            + "Prompt "
+            + bcolors.Green
+            + "Correct "
+            + bcolors.Red
+            + "Incorrect "
+            + bcolors.ENDC
+            + bcolors.Purple
+            + "Missing"
+            + bcolors.ENDC
+        )
 
-    # TODO return true if it completes the given row, as well as the next row.
-    # TODO count the number of correctly completed rows and print this number
+    return header_prompt, header_completion, llm_completion
 
 
 ####################################################################################
 # Row Completion
 ####################################################################################
 
 
 def row_completion_test(
     csv_file: str,
     llm: Union[LLM_Interface, str],
     num_prefix_rows=10,
-    num_queries=50,
+    num_queries=25,
     few_shot=7,
     out_file=None,
     system_prompt: str = "default",
+    print_levenshtein: bool = True,
 ):
-    """Row completion test: Complete the next row of the csv file, given the previous rows."""
+    """Row completion test for memorization. The test resports the number of correctly completed rows.
+
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param num_prefix_rows: The number of rows given to the model as part of the prompt.
+    :param num_queries: The number of rows that we test the model on.
+    :param few_shot: The number of few-shot examples to be used.
+    :param out_file: Optionally save all queries and responses to a csv file.
+    :param system_prompt: The system prompt to be used.
+    :param print_levenshtein: Print a visulization of the levenshtein distance between the model responses and the actual rows.
+
+    :return: the rows, the model responses.
+    """
     llm = __llm_setup(llm)
 
     if system_prompt == "default":  # default system prompt?
         system_prompt = tabmem.config.system_prompts["row-completion"]
 
     # what fraction of the rows are duplicates?
     rows = utils.load_csv_rows(csv_file)
@@ -447,36 +429,36 @@
             + "Info: "
             + bcolors.ENDC
             + f"{100*frac_duplicates:.2f}% of the rows in this dataset are duplicates."
         )
 
     # ask the model to perform row chat completion (execute the the prompt)
     if llm.chat_mode:
-        test_prefixes, test_suffixes, responses = row_chat_completion(
+        _, test_suffixes, responses = row_chat_completion(
             llm,
             csv_file,
             system_prompt,
             num_prefix_rows,
             num_queries,
             few_shot,
             out_file,
+            print_levenshtein,
         )
     else:
-        test_prefixes, test_suffixes, responses = row_completion(
+        _, test_suffixes, responses = row_completion(
             llm, csv_file, num_prefix_rows, num_queries, out_file
         )
 
-    # count the number of exact matches
-    # NOTE here we assume that the test suffix is a single row that is unique, i.e. no duplicate rows
+    # count the number of verbatim completed rows
     num_exact_matches = 0
     for test_suffix, response in zip(test_suffixes, responses):
         if test_suffix.strip() in response.strip():
             num_exact_matches += 1
 
-    # the statistical test using the levenshtein distance TODO taken out of current version although it works
+    # the statistical test using the levenshtein distance. taken out of current version although it seems to work in practice.
     # test_prefix_rows = [prefix.split("\n") for prefix in test_prefixes]
     # test_result = analysis.levenshtein_distance_t_test(
     #    responses, test_suffixes, test_prefix_rows
     # )
 
     # print the result
     print(
@@ -486,41 +468,42 @@
         + f"{num_exact_matches}/{num_queries} exact matches."
         # + bcolors.BOLD
         # + "\nLevenshtein distance test (p-value): "
         # + bcolors.ENDC
         # + f"{test_result.pvalue:.3f}."
     )
 
-    return test_prefixes, test_suffixes, responses
+    return test_suffixes, responses
 
 
 ####################################################################################
 # Feature Completion
 ####################################################################################
 
 
 def feature_completion_test(
     csv_file: str,
     llm: Union[LLM_Interface, str],
     feature_name: str = None,
-    num_queries=100,
+    num_queries=25,
     few_shot=5,
     out_file=None,
     system_prompt: str = "default",
 ):
-    """Feature completion test where we attempt to predict a single rare feature & count the number of exact matches.
+    """Feature completion test for memorization. The test resports the number of correctly completed features.
+
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param feature_name: The name of the feature to be used for the test.
+    :param num_queries: The number of feature values that we test the model on.
+    :param few_shot: The number of few-shot examples to be used.
+    :param out_file: Optionally save all queries and responses to a csv file.
+    :param system_prompt: The system prompt to be used.
 
-    The basic prompt format is the following:
-        System: <system_prompt>
-        User: Feature 1 = value 1, Feature 2 = value 2, ..., Feature n = value n
-        Response: Feature {feature_name} = value
-
-    This can be modified in the following ways:
-        - Include few-shot examples from other csv files.
-        - Don't use the feature names, but only the values.
+    :return: the feature values, the model responses.
     """
     llm = __llm_setup(llm)
 
     # TODO statistical analysis of the uniqueness of the feature (i.e., is the test appropriate?!)
     if system_prompt == "default":  # default system prompt?
         system_prompt = tabmem.config.system_prompts["feature-completion"]
 
@@ -561,16 +544,20 @@
         few_shot,
         cond_feature_names,
         add_description=False,
         out_file=out_file,
     )
 
     # parse the model responses
-    response_df = utils.parse_feature_stings(responses, [feature_name])
-    test_suffix_df = utils.parse_feature_stings(test_suffixes, [feature_name])
+    response_df = utils.parse_feature_stings(
+        responses, [feature_name], final_delimiter="\n"
+    )
+    test_suffix_df = utils.parse_feature_stings(
+        test_suffixes, [feature_name], final_delimiter="\n"
+    )
 
     # count number of exact matches
     num_exact_matches = np.sum(
         response_df[feature_name] == test_suffix_df[feature_name]
     )
 
     # print the result
@@ -579,30 +566,43 @@
         + f'Feature Completion Test ("{feature_name}"): '
         + bcolors.ENDC
         + bcolors.Black
         + f"{num_exact_matches}/{num_queries} exact matches."
         + bcolors.ENDC
     )
 
+    return test_suffix_df[feature_name].to_list(), response_df[feature_name].to_list()
+
 
 ####################################################################################
 # First Token Test
 ####################################################################################
 
 
 def first_token_test(
     csv_file: str,
     llm: Union[LLM_Interface, str],
     num_prefix_rows=10,
-    num_queries=100,
+    num_queries=25,
     few_shot=7,
     out_file=None,
     system_prompt: str = "default",
 ):
-    """First token test: Complete the first token of the next row of the csv file, given the previous rows."""
+    """First token test for memorization. We ask the model to complete the first token of the next row of the csv file, given the previous rows. The test resports the number of correctly completed tokens.
+
+    Note that the ''first token'' is not actually the first token produced by the llm, but consists of the first n digits of the row. The number of digits is determined by the function build_first_token.
+
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param num_prefix_rows: The number of rows given to the model as part of the prompt.
+    :param num_queries: The number of rows that we test the model on.
+    :param few_shot: The number of few-shot examples to be used.
+    :param out_file: Optionally save all queries and responses to a csv file.
+    :param system_prompt: The system prompt to be used.
+    """
     llm = __llm_setup(llm)
 
     if (
         system_prompt == "default"
     ):  # default system prompt? (the first token test asks the model to complete the same task as row completion, only the evaluation is different)
         system_prompt = tabmem.config.system_prompts["row-completion"]
 
@@ -685,15 +685,15 @@
         + "First Token Test Baseline (Matches of most common first token): "
         + bcolors.ENDC
         + f"{num_exact_matches_most_common}/{num_queries}."
     )
 
 
 ####################################################################################
-# Zero-Knowledge Sampling
+# Sampling
 ####################################################################################
 
 
 def build_sample_prompt(messages):
     prompt = ""
     for m in messages:
         if m["role"] == "user":
@@ -711,15 +711,23 @@
     few_shot_csv_files: list[str] = DEFAULT_FEW_SHOT_CSV_FILES,
     cond_feature_names: list[str] = [],
     drop_invalid_responses: bool = True,
     print_invalid_responses: bool = False,
     out_file=None,
     system_prompt: str = "default",
 ):
-    """zero-shot sampling from the csv file, using few-shot examples from other csv files."""
+    """Ask the model to provide random samples from the csv file.
+
+    :param csv_file: The path to the csv file.
+    :param llm: The language model to be tested.
+    :param num_queries: The desired number of samples.
+    :param few_shot_csv_files: A list of other csv files to be used as few-shot examples.
+    :param out_file: Optionally save all queries and responses to a csv file.
+    :param system_prompt: The system prompt to be used.
+    """
     llm = __llm_setup(llm)
     few_shot_csv_files = __validate_few_shot_files(csv_file, few_shot_csv_files)
 
     if system_prompt == "default":  # default system prompt?
         system_prompt = tabmem.config.system_prompts["sample"]
 
     if not llm.chat_mode:  # wrap base model to take chat queries
@@ -734,29 +742,29 @@
         few_shot_csv_files,
         cond_feature_names,
         add_description=True,
         out_file=None,
     )
 
     if len(cond_feature_names) > 0:
-        pass
+        raise NotImplementedError("Conditional sampling not yet supported.")
         # TODO handle the condtional case!
 
     # parse the model responses in a dataframe
     feature_names = utils.get_feature_names(csv_file)
     response_df = utils.parse_feature_stings(responses, feature_names)
 
     # get the indices of the rows with more than 50% NaN's
     nan_rows = response_df[
         response_df.isna().sum(axis=1) > 0.5 * len(feature_names)
     ].index.to_list()
 
     if print_invalid_responses:
         for idx in nan_rows:
-            tabmem.llm.pretty_print_response(responses[idx])
+            tabmem.llm.print_response(responses[idx])
 
     if drop_invalid_responses:
         response_df.drop(nan_rows, axis=0, inplace=True)
 
     # save the dataframe with the final samples
     if out_file is not None:
         print(out_file)
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck/llm.py` & `tabmemcheck-0.1.5/tabmemcheck/llm.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,44 +8,63 @@
 from datetime import datetime
 
 import os
 import pickle
 import time
 
 import openai
-from openai import OpenAI
+from openai import OpenAI, AzureOpenAI
 
 import tiktoken
+import requests
 
 from tenacity import (
     retry,
     retry_if_not_exception_type,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 import tabmemcheck as tabmem
+from tabmemcheck.utils import bcolors
 
 ####################################################################################
 # the interface to the language model, used by the test functions
 ####################################################################################
 
 
 @dataclass
 class LLM_Interface:
-    """The interface to the language model."""
+    """Generic interface to a language model."""
 
     # if true, the tests use the chat_completion function, otherwise the completion function
     chat_mode = False
 
-    def completion(self, prompt, temperature, max_tokens):
-        """Returns: The response (string)"""
+    def completion(self, prompt: str, temperature: float, max_tokens: int):
+        """Send a query to a language model.
 
-    def chat_completion(self, messages, temperature, max_tokens):
-        """Returns: The response (string)"""
+        :param prompt: The prompt (string) to send to the model.
+        :param temperature: The sampling temperature.
+        :param max_tokens: The maximum number of tokens to generate.
+
+        Returns:
+            str: The model response.
+        """
+        raise NotImplementedError
+
+    def chat_completion(self, messages, temperature: float, max_tokens: int):
+        """Send a query to a chat model.
+
+        :param messages: The messages to send to the model. We use the OpenAI format.
+        :param temperature: The sampling temperature.
+        :param max_tokens: The maximum number of tokens to generate.
+
+        Returns:
+            str: The model response.
+        """
         raise NotImplementedError
 
 
 ####################################################################################
 # wrap a base language model to act as a chat completion model
 ####################################################################################
 
@@ -114,55 +133,155 @@
         try:
             response = response.choices[0].text
         except:
             print(f"Invalid response {response}")
             response = ""
         return response
 
-    # @retry(
-    #    retry=retry_if_not_exception_type(openai.BadRequestError),
-    #    wait=wait_random_exponential(min=1, max=60),
-    #    stop=stop_after_attempt(7),
-    #    reraise=True,
-    # )
+    @retry(
+        retry=retry_if_not_exception_type(openai.BadRequestError),
+        wait=wait_random_exponential(min=1, max=60),
+        stop=stop_after_attempt(7),
+        reraise=True,
+    )
     def chat_completion(self, messages, temperature, max_tokens):
         response = self.client.chat.completions.create(
             model=self.model,
             messages=messages,
             temperature=temperature,
             max_tokens=max_tokens,
+            timeout=90,
         )
         # we return the completion string or "" if there is an invalid response/query
         try:
             response = response.choices[0].message.content
         except:
             print(f"Invalid response {response}")
             response = ""
         return response
 
     def __repr__(self) -> str:
         return f"{self.model}"
 
 
-def openai_setup(model=None):
-    """Setup the openai api. Returns: LLM_Interface object."""
-    client = OpenAI(
-        api_key=os.environ["OPENAI_API_KEY"]
-        if "OPENAI_API_KEY" in os.environ
-        else None,
-        organization=os.environ["OPENAI_API_ORG"]
-        if "OPENAI_API_ORG" in os.environ
-        else None,
-        # timeout=20,
-    )
-    # the llm interface object
+def openai_setup(model: str, azure: bool = False):
+    """Setup an OpenAI language model.
+
+    :param model: The name of the model (e.g. "gpt-3.5-turbo-0613").
+    :param azure: If true, use a model deployed on azure.
+
+    This function uses the following environment variables:
+
+    - OPENAI_API_KEY
+    - OPENAI_API_ORG
+    - AZURE_OPENAI_ENDPOINT
+    - AZURE_OPENAI_KEY
+    - AZURE_OPENAI_VERSION
+
+    Returns:
+        LLM_Interface: An LLM to work with!
+    """
+    if azure:  # azure deployment
+        client = AzureOpenAI(
+            azure_endpoint=(
+                os.environ["AZURE_OPENAI_ENDPOINT"]
+                if "AZURE_OPENAI_ENDPOINT" in os.environ
+                else None
+            ),
+            api_key=(
+                os.environ["AZURE_OPENAI_KEY"]
+                if "AZURE_OPENAI_KEY" in os.environ
+                else None
+            ),
+            api_version=(
+                os.environ["AZURE_OPENAI_VERSION"]
+                if "AZURE_OPENAI_VERSION" in os.environ
+                else None
+            ),
+        )
+    else:  # openai api
+        client = OpenAI(
+            api_key=(
+                os.environ["OPENAI_API_KEY"] if "OPENAI_API_KEY" in os.environ else None
+            ),
+            organization=(
+                os.environ["OPENAI_API_ORG"] if "OPENAI_API_ORG" in os.environ else None
+            ),
+        )
+
+    # the llm
     return OpenAILLM(client, model)
 
 
 #################################################################################################
+# Gemini (requires pip install google-generativeai)
+#################################################################################################
+
+
+@dataclass
+class GoogleGeminiLLM(LLM_Interface):
+    def __init__(self, model: str):
+        import google.generativeai as genai
+
+        self.model = genai.GenerativeModel(model)
+        self.chat_mode = True
+
+    def chat_completion(self, messages, temperature, max_tokens):
+        import google.generativeai as genai
+
+        # convert messages from OpenAI format to Gemini format
+        gemini_messages = []
+        for message in messages:
+            if message["role"] == "system":
+                continue
+            elif message["role"] == "user":
+                gemini_messages.append({"role": "user", "parts": [message["content"]]})
+            elif message["role"] == "assistant":
+                gemini_messages.append({"role": "model", "parts": [message["content"]]})
+            else:
+                raise ValueError("Unknown message role: {}".format(message["role"]))
+
+        # print(messages)
+        # print(gemini_messages)
+        # send messages to the model
+        response = self.model.generate_content(
+            gemini_messages,
+            generation_config=genai.types.GenerationConfig(
+                candidate_count=1, max_output_tokens=max_tokens, temperature=temperature
+            ),
+        )
+
+        # return response text
+        # print(response.prompt_feedback)
+        # print(response.parts)
+        try:
+            response = response.text
+        except:
+            print(f"Gemini: Invalid response with parts {response.parts}.")
+            response = ""
+        return response
+
+    def __repr__(self) -> str:
+        return f"{self.model}"
+
+
+def gemini_setup(model: str = None, api_key: str = None):
+    import google.generativeai as genai
+
+    genai.configure(
+        api_key=(
+            os.environ["GEMINI_API_KEY"] if "GEMINI_API_KEY" in os.environ else api_key
+        )
+    )
+    if model is not None:
+        return GoogleGeminiLLM(model)
+    return None
+
+
+#################################################################################################
 # huggingface transformers
 #################################################################################################
 
 """
 from transformers import AutoTokenizer, pipeline
 
 HF_TOKENIZER = None
@@ -241,16 +360,16 @@
 
 def log(messages, response, logfile):
     """Log the messages and response."""
     config = tabmem.config
     # logging of the raw response object (e.g. the full openai response)
     if logfile is None:
         if config.current_logging_task is not None:
-            logfile = f"{config.current_logging_task}/{config.current_logging_task}-{logging_task_index}.pkl"
-            logging_task_index += 1
+            logfile = f"{config.current_logging_task}/{config.current_logging_task}-{config.logging_task_index}.pkl"
+            config.logging_task_index += 1
     if logfile is not None:
         with open(f"chatlogs/{logfile}", "wb+") as f:
             pickle.dump((messages, response), f)
 
 
 def read_chatlog(taskname, root="chatlogs", min_files=-1):
     """A chaglog is a sequnces of files 'taskname-{idx}.pkl' that contain message-response pairs"""
@@ -284,48 +403,47 @@
             print(f"File {fname} not found.")
             messages.append(None)
             responses.append(None)
     return messages, responses
 
 
 def send_completion(llm: LLM_Interface, prompt, max_tokens=None, logfile=None):
+    """Ask the LLM to perform a completion, but with additional bells and whistles (logging, printing)."""
     config = tabmem.config
     if max_tokens is None:
         max_tokens = config.max_tokens
     response = llm.completion(prompt, config.temperature, max_tokens)
     # logging
     log(prompt, response, logfile)
     # printing
     if config.print_prompts or config.print_next_prompt:
-        pretty_print_completion(prompt, response)
+        print_completion(prompt, response)
     elif config.print_responses:
-        pretty_print_response(response)
+        print_response(response)
     # reset print_next_prompt
     config.print_next_prompt = False
     # return string response
     return response
 
 
 def send_chat_completion(llm: LLM_Interface, messages, max_tokens=None, logfile=None):
-    """Send chat completion with retrying and logging.
-
-    Returns: The response (string))"""
+    """Ask the LLM to perform a chat_completion, but with additional bells and whistles (logging, printing)."""
     config = tabmem.config
     if max_tokens is None:
         max_tokens = config.max_tokens
     response = llm.chat_completion(messages, config.temperature, max_tokens)
     if config.sleep > 0.0:
         time.sleep(config.sleep)
     # logging
     log(messages, response, logfile)
     # printing
     if config.print_prompts or config.print_next_prompt:
-        pretty_print_messages(messages)
+        print_messages(messages)
     if config.print_prompts or config.print_responses or config.print_next_prompt:
-        pretty_print_response(response)
+        print_response(response)
     # reset print_next_prompt
     config.print_next_prompt = False
     # return string response
     return response
 
 
 #################################################################################################
@@ -345,79 +463,42 @@
         return max(num_tokens_gpt_4, num_tokens_gpt_3_5)
     encoding = tiktoken.encoding_for_model(model_name)
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
 
 #################################################################################################
-# pretty printing
+# printing
 #################################################################################################
 
 
-def pretty_print_completion(prompt, response):
+def print_completion(prompt, response):
     """Print a plain language model completion in a nice format"""
     print(
-        bcolors.Green + prompt + bcolors.ENDC + bcolors.Purple + response + bcolors.ENDC
+        bcolors.Blue + prompt + bcolors.ENDC + bcolors.Purple + response + bcolors.ENDC
     )
 
 
-def pretty_print_messages(messages):
+def print_messages(messages):
     """Prints openai chat messages in a nice format"""
     for message in messages:
         print(
             bcolors.BOLD
-            + message["role"]
+            + message["role"].capitalize()
             + ": "
             + bcolors.ENDC
-            + bcolors.Green
+            + bcolors.Blue
             + message["content"].strip()
             + bcolors.ENDC
         )
 
 
-def pretty_print_response(response):
+def print_response(response):
     """Prints openai chat response in a nice format"""
     print(
         bcolors.BOLD
         + "Response: "
         + bcolors.ENDC
         + bcolors.Purple
         + response
         + bcolors.ENDC,
     )
-
-
-#################################################################################################
-# color codes to print with color in the console (from https://gist.github.com/vratiu/9780109)
-#################################################################################################
-
-
-class bcolors:
-    HEADER = "\033[95m"
-    OKBLUE = "\033[94m"
-    OKCYAN = "\033[96m"
-    OKGREEN = "\033[92m"
-    WARNING = "\033[93m"
-    FAIL = "\033[91m"
-    ENDC = "\033[0m"
-    BOLD = "\033[1m"
-    UNDERLINE = "\033[4m"
-
-    # Regular Colors
-    Black = "\033[0;30m"  # Black
-    Red = "\033[0;31m"  # Red
-    Green = "\033[0;32m"  # Green
-    Yellow = "\033[0;33m"  # Yellow
-    Blue = "\033[0;34m"  # Blue
-    Purple = "\033[0;35m"  # Purple
-    Cyan = "\033[0;36m"  # Cyan
-    White = "\033[0;37m"  # White
-
-    # Background
-    On_Black = "\033[40m"  # Black
-    On_Red = "\033[41m"  # Red
-    On_Green = "\033[42m"  # Green
-    On_Yellow = "\033[43m"  # Yellow
-    On_Blue = "\033[44m"  # Blue
-    On_Purple = "\033[45m"  # Purple
-    On_Cyan = "\033[46m"  # Cyan
-    On_White = "\033[47m"  # White
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck/resources/csv/adult-train.csv` & `tabmemcheck-0.1.5/tabmemcheck/resources/csv/adult-train.csv`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/resources/csv/california-housing.csv` & `tabmemcheck-0.1.5/tabmemcheck/resources/csv/california-housing.csv`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/resources/csv/iris.csv` & `tabmemcheck-0.1.5/tabmemcheck/resources/csv/iris.csv`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/resources/csv/openml-diabetes.csv` & `tabmemcheck-0.1.5/tabmemcheck/resources/csv/openml-diabetes.csv`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/resources/csv/uci-wine.csv` & `tabmemcheck-0.1.5/tabmemcheck/resources/csv/uci-wine.csv`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/resources/system-prompts.yaml` & `tabmemcheck-0.1.5/tabmemcheck/resources/config/system-prompts.yaml`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/row_independence.py` & `tabmemcheck-0.1.5/tabmemcheck/row_independence.py`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/tests.py` & `tabmemcheck-0.1.5/tabmemcheck/tests.py`

 * *Files identical despite different names*

### Comparing `tabmemcheck-0.1.4/tabmemcheck/utils.py` & `tabmemcheck-0.1.5/tabmemcheck/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 import numpy as np
 import pandas as pd
 
 import jellyfish
+import difflib
 import tempfile
 
 import csv
 
 from scipy.stats import bootstrap
 from sklearn import metrics
 
@@ -55,29 +56,29 @@
 
 #################################################################
 # basic utilities for csv files
 #################################################################
 
 
 def get_dataset_name(csv_file):
-    """Returns the name of the dataset"""
+    """Returns the name of the dataset."""
     return os.path.splitext(os.path.basename(csv_file))[0]
 
 
 def get_delimiter(csv_file):
-    """Returns the delimiter of a csv file"""
+    """Returns the delimiter of a csv file."""
     with _csv_file(csv_file) as csv_file:
         sniffer = csv.Sniffer()
         with open(csv_file) as fp:
             delimiter = sniffer.sniff(fp.read(5000)).delimiter
         return delimiter
 
 
 def get_feature_names(csv_file):
-    """Returns the names of the features in a csv file (a list of strings)"""
+    """Returns the names of the features in a csv file (a list of strings)."""
     with _csv_file(csv_file) as csv_file:
         df = load_csv_df(csv_file)
         return df.columns.tolist()
 
 
 def load_csv_df(csv_file, header=True, delimiter="auto", **kwargs):
     """Load a csv file as a pandas data frame."""
@@ -120,15 +121,16 @@
             data = "\n".join(data)
         return data
 
 
 def load_csv_array(csv_file, add_feature_names=False):
     """Load a csv file as a 2d numpy array where each entry is a string.
 
-    If add_featrue_names is true, then all entries will have the format "feature_name = feature_value"
+    :add_feature_names: if true, then each entry will have the format "feature_name = feature_value"
+    :returns: a 2d numpy array of strings
     """
     with _csv_file(csv_file) as csv_file:
         # load csv as a pandas dataframe
         df = load_csv_df(csv_file)
         feature_names = get_feature_names(csv_file)
         # convert all the entries to strings
         df = df.astype(str)
@@ -159,25 +161,17 @@
 #################################################################
 # more advanced functions for csv files
 # we directly construct data for prompts
 #################################################################
 
 
 def load_samples(csv_file, add_feature_names=True):
-    """
-    Returns: description, samples where description is a string and samples is a list of strings.
-
-    Description:
-    =======
-    Dataset: adult
-    Feature Names: Age, WorkClass, fnlwgt, Education, EducationNum, MaritalStatus, Occupation, Relationship, Race, Gender, CapitalGain, CapitalLoss, HoursPerWeek, NativeCountry, Income
+    """Load a csv file as a list of ''Feature name = Feature value'' strings.
 
-    Samples:
-    ========
-    ['Age = 39, , Income = <=50K', ..., 'Age = 54, , Income = >50K']
+    :returns: description, samples
     """
     # load the relevant information from the csv file
     dataset_name = get_dataset_name(csv_file)
     feature_names = get_feature_names(csv_file)
     X = load_csv_array(csv_file, add_feature_names=add_feature_names)
     description = f"Dataset: {dataset_name}\nFeature Names: " + ", ".join(feature_names)
     samples = [", ".join(x) for x in X]
@@ -266,39 +260,23 @@
         suffixes = [", ".join(x) for x in X[:, sample_feature_indices]]
     else:
         target_index = feature_names.index(target)
         suffixes = [x[target_index] for x in X]
     return prefixes, suffixes
 
 
-# DEPRECATED
-def load_prefix_suffix_feature_completion_data(
-    csv_file, num_prefix_features, use_feature_names=False
-):
-    """Returns a list of (prefix, suffix)-pairs for each row in the csv file.
-
-    If use_feature_names is true, then all entries will have the format "feature_name = feature_value"
-    """
-    return load_cond_samples(
-        csv_file,
-        get_feature_names(csv_file)[:num_prefix_features],
-        add_description=False,
-        add_feature_names=use_feature_names,
-    )
-
-
 #################################################################
 # parsing of model responses
 #################################################################
 
 
 def parse_feature_string(
     s, feature_names, as_dict=False, in_list=False, final_delimiter=","
 ):
-    """parse a string of the form "feature_name = feature_value, feature_name = feature_value, ..." into a pandas dataframe"""
+    """Parse a string (model response) of the form "feature_name = feature_value, feature_name = feature_value, ..." into a pandas dataframe."""
     feature_dict = {}
     # we use the magic strings 'feature_name = '
     magic_strings = [name + " = " for name in feature_names]
     while len(s) > 3:
         # find the next magic string
         indices = [s.find(magic_string) for magic_string in magic_strings]
         if max(indices) == -1:
@@ -337,15 +315,15 @@
             feature_dict[key] = feature_dict[key][0]
     if as_dict:
         return feature_dict
     return pd.DataFrame(feature_dict, index=[0])
 
 
 def parse_feature_stings(strings, feature_names, **kwargs):
-    """parse a list of features strings into a pandas dataframe"""
+    """Parse a list of features strings into a pandas dataframe."""
     parsed = []
     for s in strings:
         s_df = parse_feature_string(s, feature_names, **kwargs)
         parsed.append(s_df)
     return pd.concat(parsed, ignore_index=True)
 
 
@@ -467,9 +445,166 @@
     return start
 
 
 def strip_strings_in_dataframe(df: pd.DataFrame):
     """Strip all strings in a dataframe"""
     for column in df.columns:
         if df[column].dtype == object:
-            df[column] = df[column].str.strip()
+            try:
+                df[column] = df[column].str.strip()
+            except AttributeError:
+                pass  # Some columns are objects but not strings (which means .str throws an exception). We can ignore these columns.
     return df
+
+
+#################################################################
+# Printing and html output
+#################################################################
+
+
+# color codes to print with color in the console (from https://gist.github.com/vratiu/9780109)
+class bcolors:
+    HEADER = "\033[95m"
+    OKBLUE = "\033[94m"
+    OKCYAN = "\033[96m"
+    OKGREEN = "\033[92m"
+    WARNING = "\033[93m"
+    FAIL = "\033[91m"
+    ENDC = "\033[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+
+    # Regular Colors
+    Black = "\033[0;30m"  # Black
+    Red = "\033[0;31m"  # Red
+    Green = "\033[0;32m"  # Green
+    Yellow = "\033[0;33m"  # Yellow
+    Blue = "\033[0;34m"  # Blue
+    Purple = "\033[0;35m"  # Purple
+    Cyan = "\033[0;36m"  # Cyan
+    White = "\033[0;37m"  # White
+
+    # Background
+    On_Black = "\033[40m"  # Black
+    On_Red = "\033[41m"  # Red
+    On_Green = "\033[42m"  # Green
+    On_Yellow = "\033[43m"  # Yellow
+    On_Blue = "\033[44m"  # Blue
+    On_Purple = "\033[45m"  # Purple
+    On_Cyan = "\033[46m"  # Cyan
+    On_White = "\033[47m"  # White
+
+
+def levenshtein_cmd(a: str, b: str):
+    """Visualization of the Levenshtein distance between a and b, using color codes to be printed in the console."""
+    print_string = ""
+    for opcode in levenshtein(a, b)[1]:
+        op = opcode["type"]
+        a_pos = opcode["i"]
+        b_pos = opcode["j"]
+        if op == "match":
+            print_string += bcolors.Green + b[b_pos] + bcolors.ENDC
+        elif op == "insertion":
+            print_string += bcolors.Red + b[b_pos] + bcolors.ENDC
+        elif op == "deletion":
+            print_string += bcolors.Purple + a[a_pos] + bcolors.ENDC
+        elif op == "substitution":
+            print_string += bcolors.Red + b[b_pos] + bcolors.ENDC
+    return print_string
+
+
+def levenshtein_html(a: str, b: str):
+    """HTML visualization of the Levenshtein distance between a and b."""
+    html_string = ""
+    for opcode in levenshtein(a, b)[1]:
+        op = opcode["type"]
+        a_pos = opcode["i"]
+        b_pos = opcode["j"]
+        if op == "match":
+            html_string += f'<span style="background-color:#7CFC00">{b[b_pos]}</span>'
+        elif op == "insertion":
+            html_string += f'<span style="background-color:#EE4B2B">{b[b_pos]}</span>'
+        elif op == "substitution":
+            html_string += f'<span style="background-color:#EE4B2B">{b[b_pos]}</span>'
+        elif op == "deletion":
+            html_string += f'<span style="background-color:#BF40BF">{a[a_pos]}</span>'
+        if op != "deletion" and b[b_pos] == "\n":
+            html_string += "<br>"
+    return html_string
+
+
+def levenshtein_html_legend():
+    """HTML legend for the levenshtein visualization."""
+    return """'<b>Legend:</b> Prompt, <span style="background-color:#7CFC00">Correct</span>, <span style="background-color:#EE4B2B">Incorrect</span>, <span style="background-color:#BF40BF">Missing</span>'"""
+
+
+#################################################################
+# Levenshtein distance with edits
+# from  https://gist.github.com/curzona/9435822
+#################################################################
+
+
+def levenshtein(s1, s2, key=hash):
+    """Levenshtein distance with edits."""
+
+    # Based on http://en.wikibooks.org/wiki/Algorithm_Implementation/Strings/Levenshtein_distance#Python
+    # Generate the cost matrix for the two strings
+    def costmatrix(s1, s2, key=hash):
+        rows = []
+
+        previous_row = range(len(s2) + 1)
+        rows.append(list(previous_row))
+
+        for i, c1 in enumerate(s1):
+            current_row = [i + 1]
+            for j, c2 in enumerate(s2):
+                insertions = previous_row[j + 1] + 1
+                deletions = current_row[j] + 1
+                substitutions = previous_row[j] + (key(c1) != key(c2))
+                current_row.append(min(insertions, deletions, substitutions))
+            previous_row = current_row
+
+            rows.append(previous_row)
+
+        return rows
+
+    # Trace back through the cost matrix to generate the list of edits
+    def backtrace(s1, s2, rows, key=hash):
+        i, j = len(s1), len(s2)
+
+        edits = []
+
+        while not (i == 0 and j == 0):
+            prev_cost = rows[i][j]
+
+            neighbors = []
+
+            if i != 0 and j != 0:
+                neighbors.append(rows[i - 1][j - 1])
+            if i != 0:
+                neighbors.append(rows[i - 1][j])
+            if j != 0:
+                neighbors.append(rows[i][j - 1])
+
+            min_cost = min(neighbors)
+
+            if min_cost == prev_cost:
+                i, j = i - 1, j - 1
+                edits.append({"type": "match", "i": i, "j": j})
+            elif i != 0 and j != 0 and min_cost == rows[i - 1][j - 1]:
+                i, j = i - 1, j - 1
+                edits.append({"type": "substitution", "i": i, "j": j})
+            elif i != 0 and min_cost == rows[i - 1][j]:
+                i, j = i - 1, j
+                edits.append({"type": "deletion", "i": i, "j": j})
+            elif j != 0 and min_cost == rows[i][j - 1]:
+                i, j = i, j - 1
+                edits.append({"type": "insertion", "i": i, "j": j})
+
+        edits.reverse()
+
+        return edits
+
+    rows = costmatrix(s1, s2, key)
+    edits = backtrace(s1, s2, rows, key)
+
+    return rows[-1][-1], edits
```

### Comparing `tabmemcheck-0.1.4/tabmemcheck.egg-info/PKG-INFO` & `tabmemcheck-0.1.5/tabmemcheck.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 Metadata-Version: 2.1
 Name: tabmemcheck
-Version: 0.1.4
+Version: 0.1.5
 Summary: Testing Language Models for Memorization of Tabular Data
 Home-page: https://github.com/interpretml/LLM-Tabular-Memorization-Checker
 Author: Sebastian Bordt, Harsha Nori, Rich Caruana
 Author-email: sbordt@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scikit-learn
+Requires-Dist: xgboost
+Requires-Dist: scipy
+Requires-Dist: pandas>=2.1.0
+Requires-Dist: tiktoken
+Requires-Dist: openai>=1.3.3
+Requires-Dist: tenacity
+Requires-Dist: jellyfish
+Requires-Dist: pyyaml
 
 # 🐘 Testing Language Models for Memorization of Tabular Data
-![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+![PyPI - Version](https://img.shields.io/pypi/v/tabmemcheck)
 ![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
-
-This open-source package provides different functions to test LLMs for memorization and prior experience with tabular datasets. 
+![License](https://img.shields.io/github/license/interpretml/TalkToEBM.svg?style=flat-square)
+[![tests](https://github.com/interpretml/LLM-Tabular-Memorization-Checker/actions/workflows/run_tests.yaml/badge.svg?branch=main)](https://github.com/interpretml/LLM-Tabular-Memorization-Checker/actions/workflows/run_tests.yaml)
+[![Documentation](https://img.shields.io/badge/Documentation-View-blue)](http://interpret.ml/LLM-Tabular-Memorization-Checker/)
 
 
+This open-source package provides different functions to test LLMs for memorization and prior experience with tabular datasets. 
+ 
 Features:
 - [x] Test GPT-3.5, GPT-4, and other LLMs for prior experience with tabular datasets.
 - [x] Supports chat models and (base) language models. In chat mode, the prompts are designed toward GPT-3.5 and GPT-4. With other LLMs, we recommend to test the base models. 
 - [x] Based entirely on prompts (no access to the probability distribution over tokens ('logprobs') is required).
 - [x] Provides a CLI tool that works with the OpenAI API.
 
 For details, take a look at our [paper](https://openreview.net/pdf?id=l1u7jA60wT) Bordt et al., "Elephants Never Forget: Testing Language Models for Memorization of Tabular Data", NeurIPS 2023 Second Table Representation Learning Workshop.
```

