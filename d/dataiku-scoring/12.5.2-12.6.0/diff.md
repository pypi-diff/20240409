# Comparing `tmp/dataiku-scoring-12.5.2.tar.gz` & `tmp/dataiku-scoring-12.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataiku-scoring-12.5.2.tar", last modified: Mon Feb 26 16:56:32 2024, max compression
+gzip compressed data, was "dataiku-scoring-12.6.0.tar", last modified: Tue Apr  9 08:28:48 2024, max compression
```

## Comparing `dataiku-scoring-12.5.2.tar` & `dataiku-scoring-12.6.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.338963 dataiku-scoring-12.5.2/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      919 2024-02-26 16:56:18.000000 dataiku-scoring-12.5.2/HISTORY.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      524 2024-01-15 09:52:42.000000 dataiku-scoring-12.5.2/LICENSE.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       65 2024-01-15 09:52:42.000000 dataiku-scoring-12.5.2/MANIFEST.in
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       27 2024-01-15 09:52:42.000000 dataiku-scoring-12.5.2/NOTICE.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1737 2024-02-26 16:56:32.337798 dataiku-scoring-12.5.2/PKG-INFO
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      214 2024-01-15 09:52:42.000000 dataiku-scoring-12.5.2/README.md
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.336641 dataiku-scoring-12.5.2/dataiku_scoring.egg-info/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1737 2024-02-26 16:56:31.000000 dataiku-scoring-12.5.2/dataiku_scoring.egg-info/PKG-INFO
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2506 2024-02-26 16:56:32.000000 dataiku-scoring-12.5.2/dataiku_scoring.egg-info/SOURCES.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        1 2024-02-26 16:56:31.000000 dataiku-scoring-12.5.2/dataiku_scoring.egg-info/dependency_links.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-02-26 16:56:31.000000 dataiku-scoring-12.5.2/dataiku_scoring.egg-info/requires.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       15 2024-02-26 16:56:31.000000 dataiku-scoring-12.5.2/dataiku_scoring.egg-info/top_level.txt
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.084529 dataiku-scoring-12.5.2/dataikuscoring/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1069 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/__init__.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.155677 dataiku-scoring-12.5.2/dataikuscoring/algorithms/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      903 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      576 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/common.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     4771 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/decision_tree_model.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      708 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/forest_classifier.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      672 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/forest_regressor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1157 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/generic_mlp.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1581 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/gradient_boosting_classifier.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1103 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/gradient_boosting_regressor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      429 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/linear_regression.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1597 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/logistic.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      848 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/mlp_classifier.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      258 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/algorithms/mlp_regressor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     9455 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/load.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.176695 dataiku-scoring-12.5.2/dataikuscoring/mlflow/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      681 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/mlflow/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    12865 2024-02-26 16:56:18.000000 dataiku-scoring-12.5.2/dataikuscoring/mlflow/classification.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7936 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/mlflow/common.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    11001 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/mlflow/dss_flavor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2656 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/mlflow/regression.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.209738 dataiku-scoring-12.5.2/dataikuscoring/models/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      635 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      880 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/binary.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2409 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/common.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2609 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/mlflow.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     3964 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/model.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      334 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/multiclass.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7552 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/partitioned.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      205 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/models/regression.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.315429 dataiku-scoring-12.5.2/dataikuscoring/processors/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1241 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      711 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/binarize.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2863 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/calibration.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1047 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/cat_cat_interaction.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1399 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/categorical_encode.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2098 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/datetime_cyclical.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1290 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/derive.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2080 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/derive_rescale.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      995 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/drop_rows.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1131 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/dummify.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      759 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/flag.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1205 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/impute.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1423 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/normalize.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      864 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/num_cat_interaction.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1023 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/num_num_interaction.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5038 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/prepare_input.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1302 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/preprocessings.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      996 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/preprocessor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      928 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/rescale.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1679 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/selection.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2471 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/vectorize_tfidf.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1246 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/vectorize_word_count.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      783 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/processors/vectors_unfold.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-02-26 16:56:32.335806 dataiku-scoring-12.5.2/dataikuscoring/utils/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      242 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/utils/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2323 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/utils/indexed_matrix.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      239 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/utils/math_utils.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     6809 2024-02-26 14:16:30.000000 dataiku-scoring-12.5.2/dataikuscoring/utils/prediction_result.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1379 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/utils/scoring_data.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1413 2023-12-14 11:08:55.000000 dataiku-scoring-12.5.2/dataikuscoring/utils/tokenizer.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-01-15 09:52:42.000000 dataiku-scoring-12.5.2/requirements.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       38 2024-02-26 16:56:32.339054 dataiku-scoring-12.5.2/setup.cfg
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      876 2024-02-26 16:56:18.000000 dataiku-scoring-12.5.2/setup.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:48.012688 dataiku-scoring-12.6.0/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      995 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/HISTORY.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      524 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/LICENSE.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       65 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/MANIFEST.in
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       27 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/NOTICE.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1813 2024-04-09 08:28:48.011979 dataiku-scoring-12.6.0/PKG-INFO
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      214 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/README.md
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:48.011253 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1813 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/PKG-INFO
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2506 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        1 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/requires.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       15 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/top_level.txt
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.675845 dataiku-scoring-12.6.0/dataikuscoring/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1069 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/__init__.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.772009 dataiku-scoring-12.6.0/dataikuscoring/algorithms/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      903 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      576 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/common.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5451 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/decision_tree_model.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      708 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_classifier.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      672 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_regressor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1157 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/generic_mlp.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1558 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_classifier.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1103 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_regressor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      429 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/linear_regression.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1597 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/logistic.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      848 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/mlp_classifier.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      258 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/mlp_regressor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    10063 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/load.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.796887 dataiku-scoring-12.6.0/dataikuscoring/mlflow/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      681 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    12865 2024-04-03 18:04:59.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/classification.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7936 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/common.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    11001 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/dss_flavor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2656 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/regression.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.830277 dataiku-scoring-12.6.0/dataikuscoring/models/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      635 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      880 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/binary.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2409 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/common.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2609 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/mlflow.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     3964 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/model.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      334 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/multiclass.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7552 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/partitioned.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      205 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/regression.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.936041 dataiku-scoring-12.6.0/dataikuscoring/processors/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1241 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      711 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/binarize.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2863 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/calibration.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1047 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/cat_cat_interaction.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1399 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/categorical_encode.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2098 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/datetime_cyclical.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1290 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/derive.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2080 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/derive_rescale.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      995 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/drop_rows.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1222 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/dummify.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      850 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/flag.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1205 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/impute.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1423 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/normalize.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      864 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/num_cat_interaction.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1023 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/num_num_interaction.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5038 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/prepare_input.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1493 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessings.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      996 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      928 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/rescale.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1682 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/selection.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2471 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_tfidf.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1246 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_word_count.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      783 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/vectors_unfold.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:48.010453 dataiku-scoring-12.6.0/dataikuscoring/utils/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      242 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2323 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/indexed_matrix.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      239 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/math_utils.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     8696 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/prediction_result.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1379 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/scoring_data.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1413 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/tokenizer.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/requirements.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       38 2024-04-09 08:28:48.012803 dataiku-scoring-12.6.0/setup.cfg
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      876 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/setup.py
```

### Comparing `dataiku-scoring-12.5.2/HISTORY.txt` & `dataiku-scoring-12.6.0/HISTORY.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 ==========
 
 
+
+12.6.0 (2024-04-09)
+-------------------
+
+* Initial release for DSS 12.6.0
+
 12.5.2 (2024-02-26)
 -------------------
 
 * Initial release for DSS 12.5.2
 
 12.5.0 (2024-01-23)
 -------------------
```

### Comparing `dataiku-scoring-12.5.2/LICENSE.txt` & `dataiku-scoring-12.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/PKG-INFO` & `dataiku-scoring-12.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataiku-scoring
-Version: 12.5.2
+Version: 12.6.0
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,20 @@
 To use this library, you need to first export your model to Python from Dataiku.
 
 
 Changelog
 ==========
 
 
+
+12.6.0 (2024-04-09)
+-------------------
+
+* Initial release for DSS 12.6.0
+
 12.5.2 (2024-02-26)
 -------------------
 
 * Initial release for DSS 12.5.2
 
 12.5.0 (2024-01-23)
 -------------------
```

### Comparing `dataiku-scoring-12.5.2/dataiku_scoring.egg-info/PKG-INFO` & `dataiku-scoring-12.6.0/dataiku_scoring.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataiku-scoring
-Version: 12.5.2
+Version: 12.6.0
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,20 @@
 To use this library, you need to first export your model to Python from Dataiku.
 
 
 Changelog
 ==========
 
 
+
+12.6.0 (2024-04-09)
+-------------------
+
+* Initial release for DSS 12.6.0
+
 12.5.2 (2024-02-26)
 -------------------
 
 * Initial release for DSS 12.5.2
 
 12.5.0 (2024-01-23)
 -------------------
```

### Comparing `dataiku-scoring-12.5.2/dataiku_scoring.egg-info/SOURCES.txt` & `dataiku-scoring-12.6.0/dataiku_scoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/__init__.py` & `dataiku-scoring-12.6.0/dataikuscoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/__init__.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/common.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/decision_tree_model.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/decision_tree_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from .common import Classifier, Regressor
 
 
 def get_terminal_node_lt(node, data):
     current = node
     while not current.is_leaf:
-        if data[current.feature_idx] < current.threshold:
+        if current.is_missing(data):
+            current = current.left_child if current.missing_goes_left else current.right_child
+        elif data[current.feature_idx] < current.threshold:
             current = current.left_child
         else:
             current = current.right_child
     return current
 
 
 def get_terminal_node_lte(node, data):
@@ -25,22 +27,26 @@
 
 class Node:
     """
     feature_idx: the feature_idx on which the comparison is made
     label: the 'value' of the node
     """
 
-    def __init__(self, feature_idx=None, threshold=np.nan, left_child=None, right_child=None, label=None, is_leaf=None):
+    def __init__(self, feature_idx=None, threshold=np.nan, left_child=None, right_child=None, label=None, is_leaf=None, missing_goes_left=None, missing_value=np.nan):
         self.label = label
         self.feature_idx = feature_idx
         self.threshold = threshold
         self.left_child = left_child
         self.right_child = right_child
         self.is_leaf = is_leaf
+        self.missing_goes_left = missing_goes_left
+        self.missing_value = missing_value
 
+    def is_missing(self, data):
+        return np.isnan(data[self.feature_idx]) if np.isnan(self.missing_value) else data[self.feature_idx] == self.missing_value
 
 class DecisionTreeModel(Classifier, Regressor):
     """
     This class handle the cases where the tree model was trained by XGBoost, LightGBM or scikit-learn.
 
     There are three differences in each case: feature type, threshold type, and comparison operand. Type
     cast for the threshold is done when building the tree as an optimization.
@@ -59,15 +65,14 @@
       - feature type: float64(float32)
       - threshold type: np.float64
       - operand: <=
     """
 
     def __init__(self, model_parameters):
         self.init_tree(model_parameters)
-
         if self.variant == "XGBOOST":
             self.feature_converter = np.float32
             self.get_terminal_node = get_terminal_node_lt
         elif self.variant == "LIGHTGBM":
             self.feature_converter = np.float64
             self.get_terminal_node = get_terminal_node_lte
         elif self.variant == "SKLEARN":
@@ -78,32 +83,33 @@
         """ Loading serialized trees
 
         We initialize one dictionary for the leaves and one for the nodes. The nodes are initialized
         without children. Then we iterate on each node and try to find a left and right child looking up at
         the child's index in the nodes map and then if not found in the leaves map (hence it stays None if
         not found in any).
         """
-
         if model_parameters.get("xgboost", False):
             self.variant = "XGBOOST"
         elif model_parameters.get("lightgbm", False):
             self.variant = "LIGHTGBM"
         else:
             self.variant = "SKLEARN"
 
+        missing_value = model_parameters.get("missing_value", np.nan)
+
         convert_threshold = np.float32 if self.variant == "XGBOOST" else np.float64
         leaves = {
-            leaf_id: Node(label=label, is_leaf=True) for leaf_id, label in zip(
+            leaf_id: Node(label=label, is_leaf=True, missing_value=missing_value) for leaf_id, label in zip(
                 model_parameters["leaf_id"], model_parameters["label"])
         }
 
         nodes_with_children = {
-            node_id: Node(feature_idx=feature, threshold=convert_threshold(threshold), is_leaf=False)
-            for node_id, feature, threshold in zip(
-                model_parameters["node_id"], model_parameters["feature"], model_parameters["threshold"])
+            node_id: Node(feature_idx=feature, threshold=convert_threshold(threshold), is_leaf=False, missing_goes_left=missing=="l", missing_value=missing_value)
+            for node_id, feature, threshold, missing in zip(
+                model_parameters["node_id"], model_parameters["feature"], model_parameters["threshold"], model_parameters.get("missing", [None] * len(model_parameters["node_id"])))
         }
 
         # Connect the nodes to  their children
         for node_id, node in nodes_with_children.items():
             node.left_child = nodes_with_children.get(node_id * 2 + 1, leaves.get(node_id * 2 + 1))
             node.right_child = nodes_with_children.get(node_id * 2 + 2, leaves.get(node_id * 2 + 2))
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/forest_classifier.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/forest_regressor.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/generic_mlp.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/generic_mlp.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/gradient_boosting_classifier.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_classifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 from ..utils import sigmoid, softmax
 from .decision_tree_model import DecisionTreeModel
 from .common import Classifier
 
 
 class GradientBoostingClassifier(Classifier):
-
     def __init__(self, model_parameters):
-        self.trees = [[DecisionTreeModel(model_parameters) for model_parameters in trees]
-                      for trees in model_parameters["trees"]]
+        self.trees = [[DecisionTreeModel(model_parameters) for model_parameters in trees] for trees in model_parameters["trees"]]
         self.shrinkage = model_parameters["shrinkage"]
         self.baseline = np.array(model_parameters["baseline"])
         self.num_classes = 2 if len(self.trees[0]) == 1 else len(self.trees[0])
         self.feature_converter = self.trees[0][0].feature_converter
 
     def decision_function(self, X):
         return [self._decision_function(data) for data in self.feature_converter(X)]
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/gradient_boosting_regressor.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/logistic.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/logistic.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/algorithms/mlp_classifier.py` & `dataiku-scoring-12.6.0/dataikuscoring/algorithms/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/load.py` & `dataiku-scoring-12.6.0/dataikuscoring/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 import zipfile
 import pkg_resources
 import re
 import codecs
 import logging
 import warnings
-
+import numpy as np
 
 from .processors import Preprocessings, PREPROCESSORS, Calibrator, DropRows, PrepareInput
 from .algorithms import ALGORITHMS
 from .models import MODELS
 from .models import PARTITIONED_MODELS
 from .models import MLflowModel
 
@@ -103,14 +103,25 @@
     for Preprocessor in PREPROCESSORS:
         parameters = Preprocessor.load_parameters(resources_folder)
         if parameters is not None:
             logging.info("Found preprocessor {}".format(Preprocessor.__name__))
             # Needs to be JSON serializable
             preprocessors.append((Preprocessor.__name__, parameters))
 
+    # XGBoost sparse matrices handling
+    with open(os.path.join(resources_folder, "iperf.json")) as f:
+        model_input_is_sparse = json.load(f).get("modelInputIsSparse", False)
+
+    with open(os.path.join(resources_folder, "rmodeling_params.json")) as f:
+        xgboost_grid = json.load(f).get("xgboost_grid")
+        if xgboost_grid is None:
+            missing_value = 0
+        else:
+            missing_value = xgboost_grid.get("missing", 0.0) if not model_input_is_sparse else np.nan
+
     # Feature Selection
     selection_filename = os.path.join(resources_folder, "feature_selection.json")
     if os.path.isfile(selection_filename):
         with open(selection_filename) as f:
             selection = json.load(f)
     else:
         selection = {"method": "ALL", "selection_params": None}
@@ -125,14 +136,15 @@
         "meta": meta,
         "per_feature": per_feature,
         "model_parameters": model_parameters,
         "columns": columns,  # Without target
         "preprocessors": preprocessors,
         "selection": selection,
         "drop_rows": drop_rows,
+        "missing_value": missing_value,
         "feature_columns": feature_columns
     }
 
     user_meta_filename = os.path.join(resources_folder, "user_meta.json")
     if os.path.isfile(user_meta_filename):
         with open(user_meta_filename) as f:
             resources["threshold"] = json.load(f).get("activeClassifierThreshold", 0.5)
@@ -210,27 +222,25 @@
     # Dealing with special case of MLP which has the same algorithm_name
     # for regression and classification
     if algorithm_name == "MULTI_LAYER_PERCEPTRON":
         if resources["meta"]["type"] == "REGRESSION":
             algorithm_name = "MLP_REGRESSOR"
         else:
             algorithm_name = "MLP_CLASSIFIER"
-
     parameters = {
         "prepare_input": PrepareInput(resources),
-        "algorithm": ALGORITHMS[algorithm_name](resources["model_parameters"]),
+        "algorithm": ALGORITHMS[algorithm_name](dict({"missing_value": resources["missing_value"]}, **resources["model_parameters"])),
         "preprocessings": Preprocessings(resources),
         "classes": resources["meta"].get("classes"),
         "calibration": Calibrator(resources),
         "drop_rows": DropRows(resources)
     }
 
     if "threshold" in resources:
         parameters["threshold"] = resources["threshold"]
-
     return MODELS[resources["meta"]["type"]](**parameters)
 
 
 def load_model(export_path):
     """Build model from DSS python export
 
     :param export_path: the path to a zip/unzipped archive exported using DSS python export
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/mlflow/__init__.py` & `dataiku-scoring-12.6.0/dataikuscoring/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/mlflow/classification.py` & `dataiku-scoring-12.6.0/dataikuscoring/mlflow/classification.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/mlflow/common.py` & `dataiku-scoring-12.6.0/dataikuscoring/mlflow/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/mlflow/dss_flavor.py` & `dataiku-scoring-12.6.0/dataikuscoring/mlflow/dss_flavor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/mlflow/regression.py` & `dataiku-scoring-12.6.0/dataikuscoring/mlflow/regression.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/models/__init__.py` & `dataiku-scoring-12.6.0/dataikuscoring/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/models/binary.py` & `dataiku-scoring-12.6.0/dataikuscoring/models/binary.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/models/common.py` & `dataiku-scoring-12.6.0/dataikuscoring/models/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/models/mlflow.py` & `dataiku-scoring-12.6.0/dataikuscoring/models/mlflow.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/models/model.py` & `dataiku-scoring-12.6.0/dataikuscoring/models/model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/models/partitioned.py` & `dataiku-scoring-12.6.0/dataikuscoring/models/partitioned.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/__init__.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/binarize.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/binarize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/calibration.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/calibration.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/cat_cat_interaction.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/cat_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/categorical_encode.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/categorical_encode.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/datetime_cyclical.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/datetime_cyclical.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/derive.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/derive.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/derive_rescale.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/derive_rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/drop_rows.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/drop_rows.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/dummify.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/dummify.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 class Dummify(Preprocessor):
 
     FILENAME = "dummies"
 
     def __init__(self, parameters):
         self.parameters = parameters["details"]
+        self.missing_value = parameters["missing_value"]
 
     def process(self, X_numeric, X_non_numeric):
         for column, parameters in self.parameters.items():
             mask_in_levels = np.full((len(X_numeric,)), False)
             for value in parameters["levels"]:
                 mask = X_non_numeric[:, column] == value
                 X_numeric[mask, "dummy:{}:{}".format(column, value)] = 1
                 mask_in_levels += mask
 
             # Missing values
             mask_none = X_non_numeric[:, column] == None
-            X_numeric[:, "dummy:{}:N/A".format(column)] = np.where(mask_none, 1, 0)
+            X_numeric[:, "dummy:{}:N/A".format(column)] = np.where(mask_none, 1, self.missing_value)
 
             # Values unseen during training
             if parameters["with_others"]:
                 mask_others = ~(mask_none + mask_in_levels)
-                X_numeric[:, "dummy:{}:{}".format(column, "__Others__")] = np.where(mask_others, 1, 0)
+                X_numeric[:, "dummy:{}:{}".format(column, "__Others__")] = np.where(mask_others, 1, self.missing_value)
         return X_numeric, X_non_numeric
 
     def __repr__(self):
         return "Dummifier({})".format(self.parameters)
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/flag.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/flag.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 class Flag(Preprocessor):
 
     FILENAME = "flagged"
 
     def __init__(self, parameters):
         self.columns = parameters["columns"]
         self.output_names = parameters["output_names"]
+        self.missing_value = parameters["missing_value"]
 
     def process(self, X_numeric, X_non_numeric):
         for (column, output_name) in zip(self.columns, self.output_names):
             if column in X_numeric.column_index:
-                X_numeric[:, output_name] = np.where(np.isnan(X_numeric[:, column]), 0, 1)
+                X_numeric[:, output_name] = np.where(np.isnan(X_numeric[:, column]), self.missing_value, 1)
             else:
-                X_numeric[:, output_name] = np.where(X_non_numeric[:, column] == None, 0, 1)
+                X_numeric[:, output_name] = np.where(X_non_numeric[:, column] == None, self.missing_value, 1)
 
         return X_numeric, X_non_numeric
 
     def __repr__(self):
         return "FlagPresence({})".format(", ".join(self.columns))
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/impute.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/impute.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/normalize.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/normalize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/num_cat_interaction.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/num_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/num_num_interaction.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/num_num_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/prepare_input.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/prepare_input.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/preprocessor.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/rescale.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/selection.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             self.means = self.selection_params["means"]
             self.input_names = self.selection_params["input_names"]
 
             if self.selection_params["explained_variance"] is not None:
                 self.explained_standard_deviations = [x**0.5 for x in self.selection_params["explained_variance"]]
 
     def process_sparse(self, X_numeric):
-        v = np.where(np.isnan(X_numeric[:, self.feature_columns]), 0.0, X_numeric[:, self.feature_columns])
+        v = np.where(np.isnan(X_numeric[:, self.feature_columns]), np.nan, X_numeric[:, self.feature_columns])
         return np.dot(v, self.rot)
 
     def process_dense(self, X_numeric):
         v = np.where(np.isnan(X_numeric[:, self.feature_columns]), 0.0, X_numeric[:, self.feature_columns])
         if self.means:
             v -= self.means
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/vectorize_tfidf.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_tfidf.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/vectorize_word_count.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_word_count.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/processors/vectors_unfold.py` & `dataiku-scoring-12.6.0/dataikuscoring/processors/vectors_unfold.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/utils/indexed_matrix.py` & `dataiku-scoring-12.6.0/dataikuscoring/utils/indexed_matrix.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/utils/prediction_result.py` & `dataiku-scoring-12.6.0/dataikuscoring/utils/prediction_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 Warning: This module MUST NOT be imported in any common area of the package as it relies on pandas
 """
 
+from abc import ABCMeta
+from abc import abstractmethod
+
 import numpy as np
 import pandas as pd
 import six
-from abc import abstractmethod
-from abc import ABCMeta
-
 
 PREDICTION = "prediction"
 PROBABILITIES = "probabilities"
+PREDICTION_INTERVAL_LOWER = "prediction_interval_lower"
+PREDICTION_INTERVAL_UPPER = "prediction_interval_upper"
+
+PREDICTION_INTERVAL_LOWER_CAMEL = "predictionIntervalLower"
+PREDICTION_INTERVAL_UPPER_CAMEL = "predictionIntervalUpper"
 
 
 @six.add_metaclass(ABCMeta)
 class AbstractPredictionResult(object):
 
     def align_with_not_declined(self, array):
         return array
@@ -46,22 +51,23 @@
     @abstractmethod
     def is_empty(self):
         """
         :rtype: bool
         """
 
     @abstractmethod
-    def as_dataframe(self):
+    def as_dataframe(self, for_json_serialization=False):
         """
         Builds & returns a DataFrame representation of the result:
         WARNING:
           * This dataframe has no notion of index because it is built out of numpy arrays so will have
             a pristine range index and MUST be indexed afterwards
           * For classification, proba columns are returned as a tuple ("probabilities", "class_name"), which differs
             from the usual "proba_className"
+        :param bool for_json_serialization: If true it will output the column names in camelCase notation
         :return: the prediction result as a DataFrame
         :rtype: pd.DataFrame
         """
 
     @staticmethod
     def concat(prediction_results):
         """
@@ -76,40 +82,75 @@
             raise ValueError("All prediction result should be of same class")
 
         return prediction_result_class._concat(prediction_results)
 
 
 class PredictionResult(AbstractPredictionResult):
 
-    def as_dataframe(self):
-        return pd.DataFrame({PREDICTION: self.preds})
+    def as_dataframe(self, for_json_serialization=False):
+        prediction_df = pd.DataFrame({PREDICTION: self.preds})
+        if not self.has_prediction_intervals():
+            return prediction_df
+        intervals = self.prediction_intervals
+        if for_json_serialization:
+            prediction_df[PREDICTION_INTERVAL_LOWER_CAMEL] = intervals[:, 0]
+            prediction_df[PREDICTION_INTERVAL_UPPER_CAMEL] = intervals[:, 1]
+        else:
+            prediction_df[PREDICTION_INTERVAL_LOWER] = intervals[:, 0]
+            prediction_df[PREDICTION_INTERVAL_UPPER] = intervals[:, 1]
+        return prediction_df
 
-    def __init__(self, preds):
+    def __init__(self, preds, prediction_intervals=None):
         """
         :type preds: np.ndarray
+        :type prediction_intervals: np.ndarray
         """
         self._preds = preds
+        self._prediction_intervals = prediction_intervals
+
+    @property
+    def prediction_intervals(self):
+        """
+        returns a 2D array with the prediction intervals
+        :rtype: np.ndarray
+        """
+        return self._prediction_intervals
+
+    @property
+    def prediction_intervals_not_declined(self):
+        """
+        Computes and returns a 2D array with the prediction intervals keeping only not declined rows
+        :rtype: np.ndarray
+        """
+        return self.align_with_not_declined(self._prediction_intervals)
 
     @property
     def preds(self):
         return self._preds
 
     def is_empty(self):
         return self._preds.shape[0] == 0
 
+    def has_prediction_intervals(self):
+        return self._prediction_intervals is not None
+
     @staticmethod
     def _concat(prediction_results):
         """
         :type prediction_results: list[PredictionResult]
         :rtype: PredictionResult
         """
         if len(prediction_results) == 0:
             raise ValueError("Cannot concat 0 results")
         preds_concat = np.concatenate([prediction_result._preds for prediction_result in prediction_results])
-        return PredictionResult(preds_concat)
+        if prediction_results[0].has_prediction_intervals():
+            intervals_concat = np.concatenate([pr._prediction_intervals for pr in prediction_results])
+        else:
+            intervals_concat = None
+        return PredictionResult(preds_concat, intervals_concat)
 
 
 class ClassificationPredictionResult(AbstractPredictionResult):
 
     def __init__(self, target_map, probas=None, preds=None, unmapped_preds=None):
         """
         :type target_map: dict
@@ -159,15 +200,15 @@
 
     def is_empty(self):
         if self._preds is not None:
             return self._preds.shape[0] == 0
         else:
             return self._unmapped_preds.shape[0] == 0
 
-    def as_dataframe(self):
+    def as_dataframe(self, for_json_serialization=False):
         preds_df = pd.DataFrame(({PREDICTION: self.preds}))
         if not self.has_probas():
             return preds_df
         else:
             columns = [(PROBABILITIES, clazz) for clazz in self._classes]
             probas_df = pd.DataFrame(data=self.probas, columns=columns)
             return pd.concat([preds_df, probas_df], axis=1)
```

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/utils/scoring_data.py` & `dataiku-scoring-12.6.0/dataikuscoring/utils/scoring_data.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/dataikuscoring/utils/tokenizer.py` & `dataiku-scoring-12.6.0/dataikuscoring/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.5.2/setup.py` & `dataiku-scoring-12.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 
 long_description = (open('README.md').read() + '\n\n' +
                     open('HISTORY.txt').read())
 
-VERSION = "12.5.2"
+VERSION = "12.6.0"
 
 setuptools.setup(
     name='dataiku-scoring',
     version=VERSION,
     license="Apache Software License",
     packages=setuptools.find_packages(),
     description="Dataiku ML Scoring Python library",
```

