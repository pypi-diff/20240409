# Comparing `tmp/c2-4apr24-0.1.2.tar.gz` & `tmp/c2-4apr24-0.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2-4apr24-0.1.2.tar", last modified: Fri Apr  5 12:34:02 2024, max compression
+gzip compressed data, was "c2-4apr24-0.1.2b1.tar", last modified: Tue Apr  9 14:24:35 2024, max compression
```

## Comparing `c2-4apr24-0.1.2.tar` & `c2-4apr24-0.1.2b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.478655 c2-4apr24-0.1.2/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 c2-4apr24-0.1.2/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 12:34:02.477997 c2-4apr24-0.1.2/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 c2-4apr24-0.1.2/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.475906 c2-4apr24-0.1.2/c2_4apr24.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      384 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       88 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       10 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/top_level.txt
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.460636 c2-4apr24-0.1.2/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       90 2024-04-04 12:18:52.000000 c2-4apr24-0.1.2/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      780 2024-04-04 10:26:37.000000 c2-4apr24-0.1.2/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     9969 2024-04-05 10:58:22.000000 c2-4apr24-0.1.2/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.467346 c2-4apr24-0.1.2/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      165 2024-04-04 12:18:42.000000 c2-4apr24-0.1.2/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7732 2024-04-05 12:08:02.000000 c2-4apr24-0.1.2/dqc/utils/_generic.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1359 2024-03-20 17:25:30.000000 c2-4apr24-0.1.2/dqc/utils/_sklearn_artifacts.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1218 2024-04-05 12:32:16.000000 c2-4apr24-0.1.2/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-05 12:34:02.478942 c2-4apr24-0.1.2/setup.cfg
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1499 2024-04-04 13:05:07.000000 c2-4apr24-0.1.2/setup.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.474185 c2-4apr24-0.1.2/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 c2-4apr24-0.1.2/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-02 16:16:44.000000 c2-4apr24-0.1.2/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2097 2024-04-05 11:56:12.000000 c2-4apr24-0.1.2/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-09 14:24:35.704641 c2-4apr24-0.1.2b1/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 c2-4apr24-0.1.2b1/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2444 2024-04-09 14:24:35.700511 c2-4apr24-0.1.2b1/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 c2-4apr24-0.1.2b1/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-09 14:24:35.698943 c2-4apr24-0.1.2b1/c2_4apr24.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2444 2024-04-09 14:24:35.000000 c2-4apr24-0.1.2b1/c2_4apr24.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      404 2024-04-09 14:24:35.000000 c2-4apr24-0.1.2b1/c2_4apr24.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-09 14:24:35.000000 c2-4apr24-0.1.2b1/c2_4apr24.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       88 2024-04-09 14:24:35.000000 c2-4apr24-0.1.2b1/c2_4apr24.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       15 2024-04-09 14:24:35.000000 c2-4apr24-0.1.2b1/c2_4apr24.egg-info/top_level.txt
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-09 14:24:35.679234 c2-4apr24-0.1.2b1/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-09 13:51:12.000000 c2-4apr24-0.1.2b1/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1914 2024-04-09 13:43:49.000000 c2-4apr24-0.1.2b1/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)    11189 2024-04-09 13:43:49.000000 c2-4apr24-0.1.2b1/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-09 14:24:35.692165 c2-4apr24-0.1.2b1/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      277 2024-04-09 13:51:16.000000 c2-4apr24-0.1.2b1/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4893 2024-04-08 10:03:03.000000 c2-4apr24-0.1.2b1/dqc/utils/_dataprocessing.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7543 2024-04-09 05:35:00.000000 c2-4apr24-0.1.2b1/dqc/utils/_generic.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3258 2024-04-09 05:35:00.000000 c2-4apr24-0.1.2b1/dqc/utils/_sklearn_artifacts.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1362 2024-04-09 13:51:38.000000 c2-4apr24-0.1.2b1/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-09 14:24:35.704881 c2-4apr24-0.1.2b1/setup.cfg
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-09 14:24:35.697372 c2-4apr24-0.1.2b1/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 c2-4apr24-0.1.2b1/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-08 17:00:40.000000 c2-4apr24-0.1.2b1/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3084 2024-04-09 05:33:59.000000 c2-4apr24-0.1.2b1/tests/test_crossval.py
```

### Comparing `c2-4apr24-0.1.2/LICENSE` & `c2-4apr24-0.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.2/PKG-INFO` & `c2-4apr24-0.1.2b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: c2-4apr24
-Version: 0.1.2
+Version: 0.1.2b1
 Summary: Data Quality Check for Machine Learning
-Home-page: https://github.com/sumanthprabhu/C2
-Author: Sumanth S Prabhu
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `c2-4apr24-0.1.2/c2_4apr24.egg-info/PKG-INFO` & `c2-4apr24-0.1.2b1/c2_4apr24.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: c2-4apr24
-Version: 0.1.2
+Version: 0.1.2b1
 Summary: Data Quality Check for Machine Learning
-Home-page: https://github.com/sumanthprabhu/C2
-Author: Sumanth S Prabhu
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `c2-4apr24-0.1.2/dqc/crossval.py` & `c2-4apr24-0.1.2b1/dqc/crossval.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 from dqc.base import BaseCurate
-from dqc.utils import Logger, _get_pipeline, _is_valid, _DataProcessor
+from dqc.utils import (
+    Logger,
+    _get_pipeline,
+    _is_valid,
+    _DataProcessor,
+    _data_splitter,
+    _exception_handler,
+)
 
-from sklearn.model_selection import KFold
 from sklearn.preprocessing import MinMaxScaler
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 from typing import Union, List, Tuple
 
 logger = Logger("C2")
 
 tqdm.pandas()
 
 
 class CrossValCurate(BaseCurate):
-    """ """
+    """
 
-    def __init__(self, n_splits: int = 5, **options):
-        """_summary_
+    Args:
+        n_splits (int, optional): Number of splits to use when running
+        cross-validation based curation. Defaults to 5.
+        verbose (bool, optional): Sets the verbosity level during execution. Defaults to False (which maps to logging level 'ERROR')
 
-        Args:
-            n_splits (int, optional): _description_. Defaults to 5.
-            Initializing CrossValCurate
-
-        Args:
-            curate_representation (str, optional): Choice of feature representation.
-            Defaults to 'tfidf' (`sklearn.feature_extraction.text.TfidfVectorizer`).
-            curate_model (str, optional): Choice of machine learning classifier.
-            Defaults to 'logistic_regression' (sklearn.linear_model.LogisticRegression).
+    """
 
-            n_splits (int, optional): Number of splits to use when running cross-validation based curation. Defaults to 5.
-        """
+    def __init__(self, n_splits: int = 5, verbose: bool = False, **options):
         super().__init__(**options)
         self.n_splits = n_splits
+        self.verbose = verbose
+        self._set_verbosity(verbose)
+
         self.curate_pipeline = None
         self.scaler = None
         self.y_col_name_int = None
         self.result_col_list = [
             "label_correctness_score",
             "is_label_correct",
             "predicted_label",
             "prediction_probability",
         ]
 
     def __str__(self):
         return str(self.__dict__)
 
+    __repr__ = __str__
+
     def _is_confident(self, row: pd.Series) -> bool:
         """Return a boolean variable indicating whether we are confident
            about the correctness of the label assigned to a given data sample
 
         Args:
             row (pd.Series): data sample whose label correctness need to be evaluated
 
@@ -60,21 +64,33 @@
         threshold = self.correctness_threshold
         if (row["predicted_label"] == row[self.y_col_name_int]) and (
             row["label_correctness_score"] > threshold
         ):
             return True
         return False
 
+    def _set_verbosity(self, verbose: bool):
+        """Set logger level based on user input for parameter `verbose`
+
+        Args:
+            verbose (bool): Indicator for verbosity
+        """
+        if verbose:
+            logger.set_level("INFO")
+        else:
+            logger.set_level("WARNING")
+
     def _no_calibration(
         self,
         input_labels: List[Union[int, str]],
         pred_prob_matrix: np.ndarray,
         label_list: List[Union[int, str]],
     ) -> Tuple[List[Union[int, str]], List[float]]:
-        """_summary_
+        """Returns predictions, corresponding probabilities and label correctness
+        scores without any calibration
 
         Args:
             input_labels (List[Union[int, str]]): _description_
             pred_prob_matrix (np.ndarray): _description_
             label_list (List[Union[int, str]]): _description_
 
         Returns:
@@ -82,22 +98,24 @@
         """
         pred_probs = np.max(pred_prob_matrix, axis=1).tolist()
         preds = [label_list[index] for index in np.argmax(pred_prob_matrix, axis=1)]
         label_correctness_scores = [
             pred_prob_matrix[row_index, label_list.index(label)]
             for row_index, label in enumerate(input_labels)
         ]
+
         return preds, pred_probs, label_correctness_scores
 
     def _get_baselines(self, data_with_noisy_labels: pd.DataFrame) -> pd.DataFrame:
         """Computes the baseline prediction probabilities using
           input label distribution
 
         Args:
-            data_with_noisy_labels (pd.DataFrame): Input data with corresponding noisy labels
+            data_with_noisy_labels (pd.DataFrame): Input data with
+                                            corresponding noisy labels
 
         Returns:
             pd.DataFrame: Labels and corresponding probabilities
         """
         thresholds_df = (
             data_with_noisy_labels[self.y_col_name_int].value_counts(1)
         ).reset_index()
@@ -107,31 +125,36 @@
     def _calibrate_using_baseline(
         self,
         input_labels: List[Union[int, str]],
         pred_prob_matrix: np.ndarray,
         label_list: List[Union[int, str]],
         baseline_probs: pd.DataFrame,
     ) -> Tuple[List[Union[int, str]], List[float], List[float]]:
-        """_summary_
+        """Calibrate the predicted probabilities using baseline probabilities and
+        returns the modified predictions, corresponding probabilities and label
+        correctness scores
 
         Args:
-            input_labels (List[Union[int, str]]): _description_
-            pred_prob_matrix (np.ndarray): _description_
-            label_list (List[Union[int, str]]): _description_
-            baseline_probs (pd.DataFrame): _description_
+            input_labels (List[Union[int, str]]): Noisy labels from data
+            pred_prob_matrix (np.ndarray): Predicted probabilities per label
+                                for each sample in the data
+            label_list (List[Union[int, str]]): Ordered list of labels where
+                                ordering matches `pred_prob_matrix`
+            baseline_probs (pd.DataFrame): Prediction probabilities computed
+                                using input label distribution
 
         Returns:
             Tuple[List[Union[int, str]], List[float], List[float]]:
             Returns the following
             'calibrated_prediction' : Label predictions post calibration
             'calibrated_probabilities' : Normalized scores corresponding
                                     to 'calibrated_prediction'
             'label_correctness_score' : Normalized scores corresponding
                                      to 'label' (provided as input to
-                                    `fit_transform`)
+                                    `self.fit_transform`)
         """
 
         label_list_df = pd.DataFrame({"label_list": label_list})
         baseline_probs = pd.merge(
             label_list_df,
             baseline_probs,
             left_on="label_list",
@@ -160,72 +183,79 @@
 
         return (
             calibrated_predictions,
             calibrated_probabilities,
             label_correctness_scores,
         )
 
+    @_exception_handler
     def fit_transform(
         self,
         data_with_noisy_labels: pd.DataFrame,
         X_col_name: str = "text",
         y_col_name: str = "label",
         **options,
     ) -> pd.DataFrame:
         """Fit CrossValCurate on the given data
 
         Args:
-            data_with_noisy_labels (pd.DataFrame): Input data with corresponding noisy labels
+            data_with_noisy_labels (pd.DataFrame): Input data with
+            corresponding noisy labels
 
         Returns:
             pd.DataFrame: Input Data samples with
                 1) Corresponding predicted_labels using CrossValCurate
                 2) Prediction probabilities
                 3) An indicator variable `is_confident` capturing label correctness
         """
         _is_valid(data_with_noisy_labels, X_col_name, y_col_name)
         n_splits = self.n_splits
         options["num_samples"] = len(data_with_noisy_labels)
 
         logger.info("Pre-processing the data..")
         dp = _DataProcessor(
-            data_with_noisy_labels,
             random_state=self.random_state,
-            y_col_name=y_col_name,
         )
 
-        data_with_noisy_labels, row_id_col, y_col_name_int = dp._preprocess()
+        data_with_noisy_labels, row_id_col, y_col_name_int = dp._preprocess(
+            data_with_noisy_labels, y_col_name=y_col_name
+        )
 
         # y_col_name_int needs to be accessed downstream
         self.y_col_name_int = y_col_name_int
 
         data_columns = [X_col_name, y_col_name_int]
-
         logger.info(
-            "Building the curation pipeline with {n_splits}-fold cross validation.."
+            f"Building the curation pipeline with {n_splits}-fold cross validation.."
         )
         self.curate_pipeline = _get_pipeline(
             self.curate_representation, self.curate_model, **options
         )
 
-        cv = KFold(n_splits=n_splits, shuffle=False, random_state=None)
+        split_indices = _data_splitter(
+            data_with_noisy_labels,
+            X_col_name=X_col_name,
+            y_col_name_int=y_col_name_int,
+            n_splits=self.n_splits,
+        )
 
         # Lists to store predictions
         predictions = []
         prediction_probabilities = []
         label_correctness_scores = []
 
+        # Keep track of shuffled data
+        row_ids = []
+
         if self.calibration_method == "calibrate_using_baseline":
             logger.info("Computing baseline predictions for each label..")
             baseline_probs = self._get_baselines(data_with_noisy_labels[data_columns])
 
         # Iterate through kfold splits
-        for train_index, val_index in tqdm(
-            cv.split(data_with_noisy_labels[data_columns])
-        ):
+        for train_index, val_index in tqdm(split_indices):
             # Split the data
             X_train, X_val = (
                 data_with_noisy_labels.loc[train_index, X_col_name].values,
                 data_with_noisy_labels.loc[val_index, X_col_name].values,
             )
             y_train, y_val = (
                 data_with_noisy_labels.loc[train_index, y_col_name_int].values,
@@ -250,14 +280,23 @@
                 y_preds, y_pred_probs, label_cscores = self._no_calibration(
                     y_val, y_pred_probs, label_list=classes_
                 )
 
             predictions.extend(y_preds)
             prediction_probabilities.extend(y_pred_probs)
             label_correctness_scores.extend(label_cscores)
+            row_ids.extend(data_with_noisy_labels.loc[val_index, row_id_col].values)
+
+        # Order dataframe according to `rowids``
+
+        row_id_df = pd.DataFrame()
+        row_id_df[row_id_col] = pd.Series(row_ids)
+        data_with_noisy_labels = pd.merge(
+            row_id_df, data_with_noisy_labels, how="left", on=row_id_col
+        )
 
         # Add results as columns
         data_with_noisy_labels["label_correctness_score"] = pd.Series(
             label_correctness_scores
         )
         data_with_noisy_labels["predicted_label"] = pd.Series(predictions)
         data_with_noisy_labels["prediction_probability"] = pd.Series(
@@ -265,8 +304,10 @@
         )
 
         logger.info("Identifying the correctly labelled samples..")
         data_with_noisy_labels["is_label_correct"] = (
             data_with_noisy_labels.progress_apply(self._is_confident, axis=1)
         )
 
-        return dp._postprocess(display_cols=data_columns + self.result_col_list)
+        return dp._postprocess(
+            data_with_noisy_labels, display_cols=data_columns + self.result_col_list
+        )
```

### Comparing `c2-4apr24-0.1.2/dqc/utils/_generic.py` & `c2-4apr24-0.1.2b1/dqc/utils/_generic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 import logging
 import pandas as pd
+import numpy as np
 import string
 import random
 
-from typing import Tuple, List
+from typing import Tuple, List, Union
 from pandas._typing import RandomState
+from functools import wraps
 
 
 class Logger:
-    """ """
+    """Logging utility"""
 
-    def __init__(self, name, level=logging.ERROR):
-        """ """
+    levels = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+
+    def __init__(self, name, verbosity_level="error"):
         self.logger = logging.getLogger(name)
-        self.set_level(level)
+        self.set_level(verbosity_level)
 
         self._setup_stream_handler()
         self.logger.propagate = False
 
     def _setup_stream_handler(self):
-        """ """
         console_handler = logging.StreamHandler()
         formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
         console_handler.setFormatter(formatter)
         self.logger.addHandler(console_handler)
 
-    def set_level(self, level):
-        """ """
-        self.logger.setLevel(level)
+    def set_level(self, verbosity_level):
+        if verbosity_level in self.levels:
+            self.logger.setLevel(verbosity_level)
+
+    def get_level(self):
+        return self.logger.getEffectiveLevel()
 
     def info(self, message):
-        """ """
         self.logger.info(f"{message}")
 
     def warning(self, message):
-        """ """
         self.logger.warning(f"{message}")
 
 
-def _check_num_unique_labels(data, y_col_name):
-    """ """
+def _check_num_unique_labels(data: pd.DataFrame, y_col_name: str):
+    """Check if there are atleast two labels in the input data
+
+    Args:
+        data (pd.DataFrame): Input data with noisy labels
+        y_col_name (str): Label column in data
+
+    Raises:
+        ValueError: if number of labels <= 1
+    """
     count = len(pd.unique(data[y_col_name]))
     if count <= 1:
         raise ValueError(f"Number of distinct labels should be > 1 " f"Found {count}")
 
 
-def _check_columns(data, X_col_name, y_col_name):
-    """ """
+def _check_columns(data: pd.DataFrame, X_col_name: str, y_col_name: str):
+    """Sanity checks for column names in input data
+
+    Args:
+        data (pd.DataFrame): Input data with noisy labels
+        X_col_name (str): Column to be used to extract input features
+        y_col_name (str): Label column in data
+
+    Raises:
+        ValueError: If any of the expected columns are not present in data
+    """
     actual_columns = data.columns.tolist()
 
     if not X_col_name:
         raise ValueError("'X_col_name' cannot be None. Please pass a valid column name")
 
     if not y_col_name:
         raise ValueError("'y_col_name' cannot be None ")
@@ -61,44 +81,76 @@
         raise ValueError(
             f"Data does not contain the expected columns. "
             f"Expected(X_col_name, y_col_name): {expected_columns}, "
             f"Actual: {actual_columns}"
         )
 
 
-def _check_null_values(data, X_col_name, y_col_name):
-    """ """
+def _check_null_values(data: pd.DataFrame, X_col_name: str, y_col_name: str):
+    """Sanity checks to detect null values in data
+
+    Args:
+        data (pd.DataFrame): Input data with noisy labels
+        X_col_name (str): Column to be used to extract input features
+        y_col_name (str): Label column in data
+
+    Raises:
+        ValueError: If null values are found in the data
+    """
     if any(data[col].isnull().any() for col in [X_col_name, y_col_name]):
         raise ValueError(
             "Null values found in the data. \
-                                 Automatically imputing missing values is not supported yet."
+                    Automatically imputing missing values is not supported yet."
         )
 
 
-def _is_valid(data, X_col_name, y_col_name):
-    """ """
+def _is_valid(data: pd.DataFrame, X_col_name: str, y_col_name: str):
+    """Run collection of sanity checks on input data
+
+    Args:
+        data (pd.DataFrame): Input data with noisy labels
+        X_col_name (str): Column to be used to extract input features
+        y_col_name (str): Label column in data
+    """
     _check_columns(data, X_col_name, y_col_name)
     _check_num_unique_labels(data, y_col_name)
     _check_null_values(data, X_col_name, y_col_name)
 
 
 def _fetch_supported_implementations():
-    """"""
+    """Returns the list of valid options that can be passed as values
+    for parameters in BaseCurate
+
+    Returns:
+        dict: Mapping of parameters and their corresponding list of options
+    """
     return {
         "curate_representation": ["tfidf"],
         "curate_model": ["logistic_regression"],
         "calibration_method": [None, "calibrate_using_baseline"],
     }
 
 
 def _check_supported(
     curate_representation: str,
     curate_model: str,
-    calibration_method: str | ModuleNotFoundError,
+    calibration_method: Union[str, None],
 ):
+    """Checks if any of the input parameter values are invalid
+
+    Args:
+        curate_representation (str, optional): Feature representation method
+                                    to be used during curation.
+        curate_model (str): Machine learning model to be used during curation.
+        calibration_method (Union[str, None]): Approach to be used for calibration
+                                     of `curate_model` predictions
+
+    Raises:
+        ValueError: If any of the input parameter values are invalid
+    """
     supported = _fetch_supported_implementations()
     msg = ""
     if curate_representation not in supported["curate_representation"]:
         msg += f"curate_representation '{curate_representation}' is not supported. "
         msg += (
             f"Currently, {', '.join(supported['curate_representation'])} is supported\n"
         )
@@ -111,144 +163,64 @@
         msg += f"calibration_method '{calibration_method}' is not supported. "
         msg += f"Currently, {', '.join(map(str, supported['calibration_method']))} are supported\n"
 
     if len(msg) > 0:
         raise ValueError(msg)
 
 
-class _DataProcessor:
-    def __init__(
-        self,
-        df: pd.DataFrame,
-        random_state: RandomState | None = None,
-        y_col_name: str = "label",
-        y_col_name_int: str = "label_int",
-    ):
-        self.df = df
-        self.random_state = random_state
-        self.y_col_name = y_col_name
-        self.y_col_name_int = y_col_name_int
-        
-        self.newly_added_cols = set([])
-        self.row_id_col = None
-
-    def _generate_random_suffix(self, length=3):
-        """
-        Generates and returns a unique string with letters and/or digits.
-
-        Parameters:
-            length (int): Length of the string (default is 3)
-
-        Returns:
-            str: Unique short string
-        """
-        # Define the characters to use in the string
-        characters = string.ascii_letters + string.digits
-
-        # Generate a random string of the specified length
-        random_string = "".join(random.choices(characters, k=length))
-
-        return random_string
-
-    def _add_row_id(self) -> Tuple[pd.DataFrame, str]:
-        """_summary_
-
-        Returns:
-            row_id_col (str)
-        """
-        # Generate a unique column name
-        row_id_col = "row_id"
-
-        while row_id_col in self.df.columns:
-            row_id_col += f"_{self._generate_random_suffix()}"
-
-        # Add row numbers as a new column
-        self.df[row_id_col] = range(1, len(self.df) + 1)
-
-        # Mark this column as a newly added column
-        self.newly_added_cols.add(row_id_col)
-
-        return row_id_col
-
-    def _shuffle_data(self) -> pd.DataFrame:
-        """_summary_
-
-        Returns:
-            pd.DataFrame: _description_
-        """
-        # Shuffle the dataframe
-        self.df = self.df.sample(frac=1.0, 
-                                 random_state=self.random_state)\
-                         .reset_index(drop=True)
-
-        return
-
-    def _convert_labels_to_int(self):
-        """
-        Map string labels to integers for downstream processing and return the updated DataFrame
-        along with the mapping dictionary.
-
-        Returns:
-            pandas.DataFrame: DataFrame with a new integer column.
-            dict: Mapping dictionary from string values to integers.
-        """
-
-        if not self.df[self.y_col_name].dtype == "object":
-            self.df[self.y_col_name_int] = self.df[self.y_col_name]
-            return
-
-        # Create a mapping dictionary from string values to integers
-        unique_labels = self.df[self.y_col_name].unique()
-        label_mapping = {text: i for i, text in enumerate(unique_labels)}
-
-        # Map string values to integers and create a new column
-        self.df[self.y_col_name_int] = self.df[self.y_col_name].map(label_mapping)
-
-        self.newly_added_cols.add(self.y_col_name_int)
-
-        return
-
-    def _preprocess(self) -> Tuple[pd.DataFrame, str]:
-        """
-        Adds the following columns to the DataFrame -
-        1) Adds an additional column 'label_int' with integer values for all labels
-        2) Adds row numbers if random_state is not 'None'
-
-        Parameters:
-            label_column (str): column containing labels with string/integer values
-            random_state (RandomState | None):
-        Returns:
-            pd.DataFrame: Input Dataframe with added columns
-            str: Name of the newly added column
-        """
-
-        self._convert_labels_to_int()
-
-        if not self.random_state:
-            return self.df, None, self.y_col_name_int
-
-        row_id_col = self._add_row_id()
-        self.row_id_col = row_id_col
-        self._shuffle_data()
-
-        return self.df, row_id_col, self.y_col_name_int
-
-    def _postprocess(self, display_cols: List[str]) -> pd.DataFrame:
-        """Removes redundant columns and returns dataframe
-        with selected columns to display
-
-        Args:
-            df (pd.DataFrame): _description_
-            display_cols (List[str]): _description_
-
-        Returns:
-            pd.DataFrame: _description_
-        """
-        
-        res = self.df
-        row_id_col = self.row_id_col
-
-        if not row_id_col:
-            return res[display_cols]
-        
-        return res.sort_values(by=[row_id_col])\
-                    .reset_index(drop=True)[display_cols]
+def add_asymmetric_noise(
+    labels: pd.Series,
+    noise_prob: float = 0.3,
+    random_state: Union[RandomState, None] = None,
+):
+    """
+    Util function to add asymmetric noise to labels
+    for simulation of noisy label scenarios.
+
+    Args:
+        labels (pd.Series): Input pandas Series with integer values
+                        ranging from 0 to n - 1.
+        noise_prob (float): Probability of adding noise to each value.
+        random_state (Union[RandomState, None]): Random seed for reproducibility
+    Returns:
+        pd.Series: Series with asymmetric noise added to it.
+    """
+    # Set seed
+    np.random.seed(random_state)
+
+    # Avoid modifying the original data
+    noisy_labels = labels.copy()
+
+    # Assuming labels are in the range 0 to n, get n
+    max_value = noisy_labels.max()
+
+    # Determine the number of samples to modify based on the noise ratio
+    num_samples = min(len(noisy_labels), int(len(noisy_labels) * noise_prob + 1))
+
+    # Sample random indices from the labels to introduce noise
+    target_indices = np.random.choice(len(noisy_labels), num_samples, replace=False)
+
+    for idx in target_indices:
+        # Generate random noise for the value in this position
+        noise = np.random.choice([-1, 1], size=1, p=[noise_prob, 1 - noise_prob])
+
+        # Add noise to the series values
+        noisy_labels[idx] += noise
+
+        # Ensure values remain within the valid range [0, max_value]
+        noisy_labels[idx] = noisy_labels[idx] % max_value
+
+    return noisy_labels
+
+
+def _exception_handler(func):
+    def wrapper(self, *args, **kwargs):
+        try:
+            return func(self, *args, **kwargs)
+        except ValueError as ve:
+            if "cannot be greater than the number of members in each class" in str(ve):
+                raise ValueError(
+                    f"Not enough data samples per label with n_splits={self.n_splits} in CrossValCurate."
+                )
+            raise
+
+    return wrapper
```

### Comparing `c2-4apr24-0.1.2/pyproject.toml` & `c2-4apr24-0.1.2b1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c2-4apr24"
-version = "0.1.2"
+version = "0.1.2-beta1"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -39,8 +39,16 @@
 [project.optional-dependencies]
 test = [
     "pytest>=8.1.1"
 ]
 [project.urls]
 Homepage = "https://github.com/sumanthprabhu/C2"
 Source = "https://github.com/sumanthprabhu/C2"
-Tracker = "https://github.com/sumanthprabhu/C2/issues"
+Tracker = "https://github.com/sumanthprabhu/C2/issues"
+
+[tool.setuptools.packages.find]
+exclude=["notebooks", "docs"]
+
+[tool.ruff]
+lint.ignore = [
+    "F401",  # Ignore 'unused import' error
+]
```

### Comparing `c2-4apr24-0.1.2/tests/test_crossval.py` & `c2-4apr24-0.1.2b1/tests/test_crossval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from dqc import CrossValCurate
+from dqc.utils import add_asymmetric_noise
 import pandas as pd
 
 
 @pytest.mark.parametrize("curate_representation", ["tfidf", "TfIdf"])
 @pytest.mark.parametrize(
     "curate_model",
     ["logistic_regression", "Logistic_Regression"],
@@ -64,8 +65,35 @@
 def test_crossvalcurate_failure(
     data, curate_representation, curate_model, calibration_method, random_state
 ):
     with pytest.raises(ValueError):
         cvc = CrossValCurate(
             calibration_method=calibration_method, random_state=random_state
         )
-        data_curated = cvc.fit_transform(data)
+        data = cvc.fit_transform(data)
+
+
+def test_crossvalcurate_datafailure(data):
+    with pytest.raises(ValueError):
+        cvc = CrossValCurate()
+        data = data.groupby("label", group_keys=False).sample(
+            frac=0.005, random_state=43
+        )
+        data = cvc.fit_transform(data)
+
+
+@pytest.mark.parametrize("calibration_method", [None, "calibrate_using_baseline"])
+@pytest.mark.parametrize("verbose", [True, False])
+def test_verbosity(data, calibration_method, verbose):
+    cvc = CrossValCurate(calibration_method=calibration_method, verbose=verbose)
+    data = cvc.fit_transform(data)
+
+
+@pytest.mark.parametrize("noise_prob", [0.1])
+@pytest.mark.parametrize("random_state", [None, 1])
+def test_add_asymmetric_noise(data, noise_prob, random_state):
+    noisy_labels = add_asymmetric_noise(
+        data["label"], noise_prob=noise_prob, random_state=random_state
+    )
+
+    assert isinstance(noisy_labels, pd.Series)
+    assert len(noisy_labels) == len(data["label"])
```

