# Comparing `tmp/swebench-1.0.5.tar.gz` & `tmp/swebench-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.5.tar", last modified: Sun Apr  7 16:27:19 2024, max compression
+gzip compressed data, was "swebench-1.0.6.tar", last modified: Tue Apr  9 14:16:04 2024, max compression
```

## Comparing `swebench-1.0.5.tar` & `swebench-1.0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.560950 swebench-1.0.5/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.5/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-07 16:27:19.560882 swebench-1.0.5/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.5/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.554256 swebench-1.0.5/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.554738 swebench-1.0.5/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.555910 swebench-1.0.5/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.5/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.5/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.5/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-07 16:27:19.561147 swebench-1.0.5/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.5/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.556096 swebench-1.0.5/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-07 16:27:14.000000 swebench-1.0.5/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.557600 swebench-1.0.5/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.558698 swebench-1.0.5/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18858 2024-04-05 22:22:32.000000 swebench-1.0.5/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    30665 2024-04-05 19:15:08.000000 swebench-1.0.5/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.5/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.5/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.559791 swebench-1.0.5/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.5/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7097 2024-04-07 16:01:31.000000 swebench-1.0.5/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.5/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.560469 swebench-1.0.5/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.560638 swebench-1.0.5/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.483942 swebench-1.0.6/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.6/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 14:16:04.483879 swebench-1.0.6/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.6/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.472552 swebench-1.0.6/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.6/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.473337 swebench-1.0.6/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.6/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.476029 swebench-1.0.6/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.6/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.6/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.6/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.6/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.6/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.6/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.6/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-09 14:16:04.484146 swebench-1.0.6/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.6/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.476402 swebench-1.0.6/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-09 14:15:40.000000 swebench-1.0.6/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.478516 swebench-1.0.6/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.480620 swebench-1.0.6/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    19012 2024-04-09 03:45:01.000000 swebench-1.0.6/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    31176 2024-04-07 22:22:31.000000 swebench-1.0.6/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.6/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.6/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.482523 swebench-1.0.6/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.6/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7097 2024-04-07 16:01:31.000000 swebench-1.0.6/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.6/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.483458 swebench-1.0.6/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.6/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 14:16:04.483650 swebench-1.0.6/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 14:16:04.000000 swebench-1.0.6/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-09 14:16:04.000000 swebench-1.0.6/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-09 14:16:04.000000 swebench-1.0.6/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-09 14:16:04.000000 swebench-1.0.6/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-09 14:16:04.000000 swebench-1.0.6/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.5/LICENSE` & `swebench-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/PKG-INFO` & `swebench-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.5
+Version: 1.0.6
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.5 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.6 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.5/README.md` & `swebench-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/llamao/distributed_attention.py` & `swebench-1.0.6/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.6/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.6/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/make_datasets/create_instance.py` & `swebench-1.0.6/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.6/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.6/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.6/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/make_datasets/utils.py` & `swebench-1.0.6/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/run_api.py` & `swebench-1.0.6/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/run_live.py` & `swebench-1.0.6/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/inference/run_llama.py` & `swebench-1.0.6/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/setup.py` & `swebench-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/__init__.py` & `swebench-1.0.6/swebench/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.5/swebench/collect/build_dataset.py` & `swebench-1.0.6/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/collect/build_dataset_ft.py` & `swebench-1.0.6/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.6/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/collect/get_top_pypi.py` & `swebench-1.0.6/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/collect/print_pulls.py` & `swebench-1.0.6/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/collect/utils.py` & `swebench-1.0.6/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/harness/constants.py` & `swebench-1.0.6/swebench/harness/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,18 @@
             "python": "3.11",
             "packages": "requirements.txt",
             "install": "python -m pip install -e .",
         }
         for k in ["5.0"]
     }
 )
+for k in ["2.2", "3.0"]:
+    MAP_VERSION_TO_INSTALL_DJANGO[k].update(
+        {"env_vars_test": { "LANG": "en_US.UTF-8", "LC_ALL": "en_US.UTF-8" }}
+    )
 
 MAP_VERSION_TO_INSTALL_REQUESTS = {
     k: {"python": "3.9", "packages": "pytest", "install": "python -m pip install ."}
     for k in
         ["0.7", "0.8", "0.9", "0.11", "0.13", "0.14", "1.1", "1.2", "2.0", "2.2"] + \
         ["2.3", "2.4", "2.5", "2.7", "2.8", "2.9", "2.10", "2.11", "2.12", "2.17"] + \
         ["2.18", "2.19", "2.22", "2.26", "2.25", "2.27", "3.0"]
@@ -319,15 +323,15 @@
 
 MAP_VERSION_TO_INSTALL_PYLINT = {
     k: {"python": "3.9", "packages": "requirements.txt", "install": "pip install -e ."}
     for k in ["2.10", "2.11", "2.13", "2.14", "2.15", "2.16", "2.17", "2.8", "2.9", "3.0"]
 }
 MAP_VERSION_TO_INSTALL_PYLINT.update({
     k: {**MAP_VERSION_TO_INSTALL_PYLINT[k], "pip_packages": " ".join([
-        "astroid==3.0.0a7"
+        "astroid==3.0.0a6"
     ])} for k in ['3.0']})
 
 MAP_VERSION_TO_INSTALL_XARRAY = {
     k: {
         "python": "3.10",
         "packages": "environment.yml",
         "install": "pip install -e .",
```

### Comparing `swebench-1.0.5/swebench/harness/context_manager.py` & `swebench-1.0.6/swebench/harness/context_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,18 +705,29 @@
             bool: True if test script ran successfully, False otherwise
         """
         try:
             # Run test command for task instance
             test_cmd = f"{self.cmd_activate} && {instance['test_cmd']}"
             with open(self.log_file, "a") as f:
                 f.write(f"Test Script: {test_cmd};\n")
+
+            # Set environment variables if provided
+            specifications = MAP_VERSION_TO_INSTALL[instance["repo"]][instance["version"]]
+            if "env_vars_test" in specifications:
+                self.exec.subprocess_args["env"].update(specifications["env_vars_test"])
+
             out_test = self.exec(
                 test_cmd, shell=True, timeout=self.timeout, check=False
             )
 
+            # Unset environment variables if provided
+            if "env_vars_test" in specifications:
+                for key in specifications["env_vars_test"]:
+                    del self.exec.subprocess_args["env"][key]
+
             # Write test results to log file
             with open(self.log_file, "a") as f:
                 f.write(f"Output:\n")
                 f.write(out_test.stdout)
                 f.write(out_test.stderr)
                 if out_test.returncode != 0:
                     f.write(f"\n{TESTS_FAILED}\n")
```

### Comparing `swebench-1.0.5/swebench/harness/engine_evaluation.py` & `swebench-1.0.6/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/harness/engine_validation.py` & `swebench-1.0.6/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/harness/run_evaluation.py` & `swebench-1.0.6/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/harness/utils.py` & `swebench-1.0.6/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/constants.py` & `swebench-1.0.6/swebench/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/conversion.py` & `swebench-1.0.6/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/getters.py` & `swebench-1.0.6/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/log_parsers.py` & `swebench-1.0.6/swebench/metrics/log_parsers.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/metrics.py` & `swebench-1.0.6/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/monitor.py` & `swebench-1.0.6/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/metrics/report.py` & `swebench-1.0.6/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/versioning/constants.py` & `swebench-1.0.6/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/versioning/get_versions.py` & `swebench-1.0.6/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench/versioning/utils.py` & `swebench-1.0.6/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.5/swebench.egg-info/PKG-INFO` & `swebench-1.0.6/swebench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.5
+Version: 1.0.6
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.5 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.6 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.5/swebench.egg-info/SOURCES.txt` & `swebench-1.0.6/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

