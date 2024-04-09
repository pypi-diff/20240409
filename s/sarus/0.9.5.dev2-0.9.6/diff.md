# Comparing `tmp/sarus-0.9.5.dev2.tar.gz` & `tmp/sarus-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.9.5.dev2.tar", last modified: Fri Mar  8 14:17:34 2024, max compression
+gzip compressed data, was "sarus-0.9.6.tar", last modified: Tue Apr  9 13:26:19 2024, max compression
```

## Comparing `sarus-0.9.5.dev2.tar` & `sarus-0.9.6.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1606 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.001642 sarus-0.9.5.dev2/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      728 2024-03-08 14:16:42.000000 sarus-0.9.5.dev2/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    32593 2024-03-06 13:56:13.000000 sarus-0.9.5.dev2/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.001642 sarus-0.9.5.dev2/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      323 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    19117 2024-03-06 13:56:13.000000 sarus-0.9.5.dev2/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      757 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.001642 sarus-0.9.5.dev2/sarus/federated_analytics/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       87 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/federated_analytics/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13063 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/federated_analytics/lib.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      567 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/llm/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       70 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/llm/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3647 2024-03-08 14:16:42.000000 sarus-0.9.5.dev2/sarus/llm/pretrained.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5642 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1981 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1289 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3865 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9496 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      672 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3481 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    28472 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2633 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4725 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1826 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/matplotlib/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2024-03-06 13:56:13.000000 sarus-0.9.5.dev2/sarus/matplotlib/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-03-06 13:56:13.000000 sarus-0.9.5.dev2/sarus/matplotlib/pyplot.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      371 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.005642 sarus-0.9.5.dev2/sarus/optbinning/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      215 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/optbinning/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4761 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/optbinning/binning.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      133 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/optbinning/scorecard.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.009642 sarus-0.9.5.dev2/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      212 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8006 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.009642 sarus-0.9.5.dev2/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      375 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.009642 sarus-0.9.5.dev2/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      165 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      152 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    45522 2024-03-06 13:56:13.000000 sarus-0.9.5.dev2/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.009642 sarus-0.9.5.dev2/sarus/scipy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/scipy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7931 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/scipy/sparse.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.009642 sarus-0.9.5.dev2/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4561 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/scripts/generate_op_list.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3003 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/serialization.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.009642 sarus-0.9.5.dev2/sarus/shap/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1584 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/shap/Explanation.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1181 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/shap/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12871 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/shap/explainers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3881 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/shap/maskers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      413 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/shap/plots.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      140 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/shap/utils.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      719 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6580 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      789 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      803 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11426 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      589 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      191 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1266 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      188 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1708 2024-03-06 13:56:13.000000 sarus-0.9.5.dev2/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      581 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1565 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      279 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      943 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      169 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3177 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18706 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2344 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1205 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.001642 sarus-0.9.5.dev2/sarus.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1606 2024-03-08 14:17:33.000000 sarus-0.9.5.dev2/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2430 2024-03-08 14:17:33.000000 sarus-0.9.5.dev2/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-03-08 14:17:33.000000 sarus-0.9.5.dev2/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-01-22 14:06:25.000000 sarus-0.9.5.dev2/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      435 2024-03-08 14:17:33.000000 sarus-0.9.5.dev2/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2024-03-08 14:17:33.000000 sarus-0.9.5.dev2/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1445 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2024-03-08 14:17:28.000000 sarus-0.9.5.dev2/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-03-08 14:17:34.013642 sarus-0.9.5.dev2/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2024-02-16 15:21:05.000000 sarus-0.9.5.dev2/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2024-02-16 15:21:05.000000 sarus-0.9.6/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1601 2024-04-09 13:26:19.017624 sarus-0.9.6/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2024-02-16 15:21:05.000000 sarus-0.9.6/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2024-02-16 15:21:05.000000 sarus-0.9.6/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.993624 sarus-0.9.6/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      728 2024-04-09 13:25:47.000000 sarus-0.9.6/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    32593 2024-03-06 13:56:13.000000 sarus-0.9.6/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.997624 sarus-0.9.6/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      323 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    19168 2024-04-09 08:34:12.000000 sarus-0.9.6/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      757 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.997624 sarus-0.9.6/sarus/federated_analytics/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       87 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/federated_analytics/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13063 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/federated_analytics/lib.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.997624 sarus-0.9.6/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      567 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.997624 sarus-0.9.6/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.997624 sarus-0.9.6/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.001624 sarus-0.9.6/sarus/llm/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       70 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/llm/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3647 2024-04-02 12:36:43.000000 sarus-0.9.6/sarus/llm/pretrained.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.005624 sarus-0.9.6/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5642 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1981 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1289 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3865 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9496 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.005624 sarus-0.9.6/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      672 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3481 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    28479 2024-04-02 12:36:43.000000 sarus-0.9.6/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2633 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4725 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1826 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/matplotlib/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2024-03-06 13:56:13.000000 sarus-0.9.6/sarus/matplotlib/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-03-06 13:56:13.000000 sarus-0.9.6/sarus/matplotlib/pyplot.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      371 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/optbinning/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      215 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/optbinning/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4761 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/optbinning/binning.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      133 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/optbinning/scorecard.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      212 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8006 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       95 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      375 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      165 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      152 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    45522 2024-03-06 13:56:13.000000 sarus-0.9.6/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.009624 sarus-0.9.6/sarus/scipy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      155 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/scipy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7931 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/scipy/sparse.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.013624 sarus-0.9.6/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4561 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/scripts/generate_op_list.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3003 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/serialization.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.013624 sarus-0.9.6/sarus/shap/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1584 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/shap/Explanation.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1181 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/shap/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12871 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/shap/explainers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3881 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/shap/maskers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      413 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/shap/plots.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      140 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/shap/utils.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      719 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6580 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      789 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      803 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11426 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      589 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      191 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1266 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      188 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1708 2024-03-06 13:56:13.000000 sarus-0.9.6/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      581 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1565 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      279 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      943 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      169 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3177 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18706 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2344 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1205 2024-02-16 15:21:05.000000 sarus-0.9.6/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:18.997624 sarus-0.9.6/sarus.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1601 2024-04-09 13:26:18.000000 sarus-0.9.6/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2430 2024-04-09 13:26:18.000000 sarus-0.9.6/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-04-09 13:26:18.000000 sarus-0.9.6/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2024-01-22 14:06:25.000000 sarus-0.9.6/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      431 2024-04-09 13:26:18.000000 sarus-0.9.6/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2024-04-09 13:26:18.000000 sarus-0.9.6/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1441 2024-04-09 13:26:19.021624 sarus-0.9.6/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2024-04-09 13:25:16.000000 sarus-0.9.6/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2024-04-09 13:26:19.017624 sarus-0.9.6/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2024-02-16 15:21:05.000000 sarus-0.9.6/tests/test_sanity.py
```

### Comparing `sarus-0.9.5.dev2/PKG-INFO` & `sarus-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.9.5.dev2
+Version: 0.9.6
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.9.5.dev2/README.rst` & `sarus-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/__init__.py` & `sarus-0.9.6/sarus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """SDK classes and functions."""
 # flake8: noqa
 import warnings
 
-VERSION = "0.9.3"
+VERSION = "0.9.6"
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from sarus import (
         imblearn,
         numpy,
         pandas,
```

### Comparing `sarus-0.9.5.dev2/sarus/config.yaml` & `sarus-0.9.6/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/context/local_sdk.py` & `sarus-0.9.6/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/dataspec_wrapper.py` & `sarus-0.9.6/sarus/dataspec_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,19 +203,20 @@
             }
         )
         names = dict()
         storage = self.manager().storage()
         rewriter = self.manager().dataspec_rewriter()
         for uuid, (_id, _class) in DataSpecWrapper.instances.items():
             ds = storage.referrable(uuid)
-            info = mapping[_id] if _id in mapping else ("", _class)
-            names[uuid] = info
-            # The symbol & class is also valid for all variants
-            for variant in rewriter.variants(ds):
-                names[variant.uuid()] = info
+            if ds is not None:
+                info = mapping[_id] if _id in mapping else ("", _class)
+                names[uuid] = info
+                # The symbol & class is also valid for all variants
+                for variant in rewriter.variants(ds):
+                    names[variant.uuid()] = info
         return names
 
     def dot(
         self,
         kind: Union[
             DataSpecVariant,
             Literal["rewritten", "mock", "original", "synthetic"],
```

### Comparing `sarus-0.9.5.dev2/sarus/debug.py` & `sarus-0.9.6/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/federated_analytics/lib.py` & `sarus-0.9.6/sarus/federated_analytics/lib.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/imblearn/over_sampling.py` & `sarus-0.9.6/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/imblearn/pipeline.py` & `sarus-0.9.6/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/imblearn/under_sampling.py` & `sarus-0.9.6/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/legacy/tensorflow/dataset.py` & `sarus-0.9.6/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/legacy/tensorflow/model.py` & `sarus-0.9.6/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/llm/pretrained.py` & `sarus-0.9.6/sarus/llm/pretrained.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/arrow_local.py` & `sarus-0.9.6/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/arrow_remote.py` & `sarus-0.9.6/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/base_remote.py` & `sarus-0.9.6/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/cache_scalar_local.py` & `sarus-0.9.6/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/dataspec_api.py` & `sarus-0.9.6/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/ops/api.py` & `sarus-0.9.6/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/parquet_local.py` & `sarus-0.9.6/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/sdk_manager.py` & `sarus-0.9.6/sarus/manager/sdk_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
                 if dataspec.prototype() == sp.Dataset
                 else SCALAR_TASK
             )
             stage = status.task(TASK) if status else None
             key = stage.stage() if stage else "no_status"
             fillcolor, color, fontcolor = STATUS_COLORS[key]
         else:
-            if dataspec.is_dp():
+            if dataspec.is_published():
                 key = "DP"
             elif dataspec.is_pep():
                 key = "PEP"
             else:
                 key = "NOT_PEP"
 
             fillcolor, color, fontcolor = PRIVACY_COLORS[key]
```

### Comparing `sarus-0.9.5.dev2/sarus/manager/typing.py` & `sarus-0.9.6/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/value_local.py` & `sarus-0.9.6/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/manager/value_remote.py` & `sarus-0.9.6/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/numpy/scalars.py` & `sarus-0.9.6/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/optbinning/binning.py` & `sarus-0.9.6/sarus/optbinning/binning.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/pandas/core.py` & `sarus-0.9.6/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/pandas/dataframe.py` & `sarus-0.9.6/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sarus.py` & `sarus-0.9.6/sarus/sarus.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/scipy/sparse.py` & `sarus-0.9.6/sarus/scipy/sparse.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/scripts/generate_op_list.py` & `sarus-0.9.6/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/serialization.py` & `sarus-0.9.6/sarus/serialization.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/shap/Explanation.py` & `sarus-0.9.6/sarus/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/shap/__init__.py` & `sarus-0.9.6/sarus/shap/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/shap/explainers.py` & `sarus-0.9.6/sarus/shap/explainers.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/shap/maskers.py` & `sarus-0.9.6/sarus/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/__init__.py` & `sarus-0.9.6/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/cluster.py` & `sarus-0.9.6/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/compose.py` & `sarus-0.9.6/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/decomposition.py` & `sarus-0.9.6/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/ensemble.py` & `sarus-0.9.6/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/impute.py` & `sarus-0.9.6/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/linear_model.py` & `sarus-0.9.6/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/model_selection.py` & `sarus-0.9.6/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/pipeline.py` & `sarus-0.9.6/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/preprocessing.py` & `sarus-0.9.6/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/sklearn/svm.py` & `sarus-0.9.6/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/skopt/searchcv.py` & `sarus-0.9.6/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/std/types.py` & `sarus-0.9.6/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/typing.py` & `sarus-0.9.6/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/utils.py` & `sarus-0.9.6/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/wrapper_factory.py` & `sarus-0.9.6/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus/xgboost/xgboost.py` & `sarus-0.9.6/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/sarus.egg-info/PKG-INFO` & `sarus-0.9.6/sarus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.9.5.dev2
+Version: 0.9.6
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.9.5.dev2/sarus.egg-info/SOURCES.txt` & `sarus-0.9.6/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.9.5.dev2/setup.cfg` & `sarus-0.9.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.9.2.dev0
+	sarus-data-spec-public==3.10.2
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
 	protobuf >= 3.20.3
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
```

