# Comparing `tmp/corrai-0.2.0.tar.gz` & `tmp/corrai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corrai-0.2.0.tar", last modified: Thu Jan 18 14:17:39 2024, max compression
+gzip compressed data, was "corrai-0.3.0.tar", last modified: Tue Apr  9 13:27:43 2024, max compression
```

## Comparing `corrai-0.2.0.tar` & `corrai-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:39.629247 corrai-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-18 14:17:33.000000 corrai-0.2.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-01-18 14:17:39.629247 corrai-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-18 14:17:33.000000 corrai-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:39.625246 corrai-0.2.0/corrai/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:39.629247 corrai-0.2.0/corrai/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/base/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/base/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/base/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:39.629247 corrai-0.2.0/corrai/learning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/learning/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/learning/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    29437 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/multi_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    17020 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    31651 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36691 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/tsgenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-01-18 14:17:33.000000 corrai-0.2.0/corrai/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 14:17:39.629247 corrai-0.2.0/corrai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-01-18 14:17:39.000000 corrai-0.2.0/corrai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-18 14:17:39.000000 corrai-0.2.0/corrai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 14:17:39.000000 corrai-0.2.0/corrai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-18 14:17:39.000000 corrai-0.2.0/corrai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-18 14:17:39.000000 corrai-0.2.0/corrai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-18 14:17:39.629247 corrai-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-01-18 14:17:33.000000 corrai-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:43.100750 corrai-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-09 13:27:36.000000 corrai-0.3.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-09 13:27:43.100750 corrai-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-09 13:27:36.000000 corrai-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:43.100750 corrai-0.3.0/corrai/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:43.100750 corrai-0.3.0/corrai/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/solar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/fmu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:43.100750 corrai-0.3.0/corrai/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/learning/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/learning/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30532 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/multi_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31148 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38806 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/tsgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-09 13:27:36.000000 corrai-0.3.0/corrai/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:43.100750 corrai-0.3.0/corrai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-09 13:27:43.000000 corrai-0.3.0/corrai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 13:27:43.000000 corrai-0.3.0/corrai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:27:43.000000 corrai-0.3.0/corrai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 13:27:43.000000 corrai-0.3.0/corrai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 13:27:43.000000 corrai-0.3.0/corrai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 13:27:43.100750 corrai-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-09 13:27:36.000000 corrai-0.3.0/setup.py
```

### Comparing `corrai-0.2.0/LICENCE.md` & `corrai-0.3.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `corrai-0.2.0/PKG-INFO` & `corrai-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corrai
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data correction and Machine Learning
 Home-page: https://github.com/BuildingEnergySimulationTools/corrai
 Author: Nobatek/INEF4
 Author-email: bdurandestebe@nobatek.inef4.com
 License: License :: OSI Approved :: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/BuildingEnergySimulationTools/corrai/main/logo_corrai.svg" alt="CorrAI" width="200"/>
 </p>
 
-[![Static Badge](https://img.shields.io/badge/version-0.1.0-orange)](https://pypi.org/project/corrai/)
+[![Static Badge](https://img.shields.io/badge/version-0.3.0-orange)](https://pypi.org/project/corrai/)
 [![Static Badge](https://img.shields.io/badge/python-3.10_%7C_3.12-blue)](https://pypi.org/project/corrai/)
 [![codecov](https://codecov.io/gh/BuildingEnergySimulationTools/corrai/branch/main/graph/badge.svg?token=F51O9CXI61)](https://codecov.io/gh/BuildingEnergySimulationTools/corrai)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 
 ## Measured Data Exploration for Physical and Mathematical Models
```

### Comparing `corrai-0.2.0/README.md` & `corrai-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/BuildingEnergySimulationTools/corrai/main/logo_corrai.svg" alt="CorrAI" width="200"/>
 </p>
 
-[![Static Badge](https://img.shields.io/badge/version-0.1.0-orange)](https://pypi.org/project/corrai/)
+[![Static Badge](https://img.shields.io/badge/version-0.3.0-orange)](https://pypi.org/project/corrai/)
 [![Static Badge](https://img.shields.io/badge/python-3.10_%7C_3.12-blue)](https://pypi.org/project/corrai/)
 [![codecov](https://codecov.io/gh/BuildingEnergySimulationTools/corrai/branch/main/graph/badge.svg?token=F51O9CXI61)](https://codecov.io/gh/BuildingEnergySimulationTools/corrai)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 
 ## Measured Data Exploration for Physical and Mathematical Models
```

### Comparing `corrai-0.2.0/corrai/base/simulate.py` & `corrai-0.3.0/corrai/base/simulate.py`

 * *Files identical despite different names*

### Comparing `corrai-0.2.0/corrai/learning/cluster.py` & `corrai-0.3.0/corrai/learning/cluster.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from plotly import colors as colors, graph_objects as go
 from scipy.signal import argrelextrema
 from sklearn.base import BaseEstimator, ClusterMixin
 from sklearn.neighbors import KernelDensity
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import StandardScaler
 
-from corrai import transformers as ct
-from corrai.utils import (
+from corrai.transformers import PdSkTransformer
+from corrai.base.utils import (
     as_1_column_dataframe,
     check_datetime_index,
     float_to_hour,
     _reshape_1d,
 )
 
 
@@ -174,15 +174,17 @@
                 (X > (sp - self.cluster_tol)), (X < (sp + self.cluster_tol))
             )
             x_cluster[mask] = nb
 
         return np.nan_to_num(x_cluster, nan=-1)
 
 
-def set_point_identifier(X, estimator=None, sk_scaler=None, cols=None):
+def set_point_identifier(
+    X: pd.DataFrame | pd.Series, estimator: KdeSetPointIdentificator
+):
     """
     Identifies set points in a time series data using kernel density estimation.
     Uses CorrAI KdeSetPointIdentificator combined with a transformer to scale the data.
     If no scaler is provided, the function uses scikit learn StandardScaler
 
     Parameters
     ----------
@@ -214,44 +216,33 @@
 
     Notes
     -----
     The set point identification is performed by fitting the kernel density estimator
     to each column of the input data, and then finding the peaks of the density
     estimate, which shall correspond to the set points.
     """
-    check_datetime_index(X)
-
     if isinstance(X, pd.Series):
-        X = X.to_frame()
-
-    if cols is None:
-        cols = X.columns
+        X = as_1_column_dataframe(X)
+    check_datetime_index(X)
 
-    if sk_scaler is None:
-        pd_scaler = ct.PdSkTransformer(StandardScaler())
-    else:
-        pd_scaler = ct.PdSkTransformer(sk_scaler)
+    model = make_pipeline(PdSkTransformer(StandardScaler()), estimator)
 
-    if estimator is None:
-        estimator = KdeSetPointIdentificator()
-
-    model = make_pipeline(pd_scaler, estimator)
     pd_scaler = model.named_steps["pdsktransformer"]
     kde = model.named_steps["kdesetpointidentificator"]
 
     duration = X.index[-1] - X.index[-0]
 
     period = pd.Period(
         X.index[0].strftime("%Y-%m-%d %H-%M-%S"),
         day=duration.days,
         second=duration.seconds,
     )
 
     multi_series_list = []
-    for col in cols:
+    for col in X.columns:
         model.fit(X[[col]])
         try:
             set_points = pd_scaler.inverse_transform(kde.set_points)
         except ValueError:
             set_points = None
 
         if set_points is not None:
@@ -267,66 +258,92 @@
     if multi_series_list:
         return pd.concat(multi_series_list, axis=1)
     else:
         return None
 
 
 def moving_window_set_point_identifier(
-    X, window_size, slide_size, estimator=None, sk_scaler=None, cols=None
+    X: pd.DataFrame | pd.Series,
+    window_size: dt.timedelta,
+    slide_size: dt.timedelta,
+    estimator: KdeSetPointIdentificator,
 ):
-    if estimator is None:
-        estimator = KdeSetPointIdentificator()
-    if not isinstance(estimator, KdeSetPointIdentificator):
-        raise ValueError(
-            f"estimator must be a corrai KdeSetPointIdentificator object "
-            f"got {type(estimator)}"
-        )
-    if not isinstance(window_size, dt.timedelta):
-        raise ValueError("window_size must be a datetime.timedelta object")
-    if not isinstance(slide_size, dt.timedelta):
-        raise ValueError("window_size must be a datetime.timedelta object")
-    if not isinstance(X, pd.DataFrame):
-        raise ValueError("data must be a Pandas DataFrame")
-    if not isinstance(X.index, pd.DatetimeIndex):
-        raise ValueError("data index be a Pandas DateTimeIndex")
+    """
+    Identify set points in a time series dataset using a moving window approach
+    with kernel density estimation.
+
+    Parameters
+    ----------
+    X : pandas.DataFrame or pandas.Series
+        Input data containing time series data for set point identification.
+        Must have a DateTimeIndex.
+
+    window_size : datetime.timedelta
+        Size of the moving window for set point identification.
+
+    slide_size : datetime.timedelta
+        Size of the sliding step between consecutive windows.
+
+    estimator : KdeSetPointIdentificator
+        An instance of the CorrAI KdeSetPointIdentificator class used for set point
+        identification.
 
-    if cols is None:
-        cols = X.columns
+    Returns
+    -------
+    pandas.DataFrame or None
+        A DataFrame with identified set points for each specified column within the m
+        oving windows. MultiIndex row labels indicate the period and set point number.
+        Returns None if no set points are identified in any window.
+
+    Raises
+    ------
+    ValueError
+        If the input data is not a DataFrame, a Series or lacks a DateTimeIndex.
 
+    Notes
+    -----
+    Set point identification is performed using the provided kernel density estimator
+    within a moving window approach. The function iterates through the time series
+    data with windows of a specified size and identifies set points in each window.
+    """
+    if isinstance(X, pd.Series):
+        X = as_1_column_dataframe(X)
+    check_datetime_index(X)
     start_date = X.index[0]
     end_date = X.index[-1]
 
     groups_res_list = []
-
     while start_date <= end_date - window_size:
-        selected_data = X.loc[start_date : start_date + window_size, cols]
+        selected_data = X.loc[start_date : start_date + window_size, :]
         groups_res_list.append(
-            set_point_identifier(
-                X=selected_data, estimator=estimator, sk_scaler=sk_scaler
-            )
+            set_point_identifier(X=selected_data, estimator=estimator)
         )
 
         start_date += slide_size
 
     if not all(v is None for v in groups_res_list):
         return pd.concat(groups_res_list)
     else:
         return None
 
 
 def plot_kde_set_point(
-    X, estimator=None, sk_scaler=None, title="Clustered Timeseries", y_label="[-]"
+    X: pd.DataFrame | pd.Series,
+    estimator: KdeSetPointIdentificator = None,
+    sk_scaler: bool = None,
+    title="Clustered Timeseries",
+    y_label="[-]",
 ):
     """
     Plots a scatter plot of the input data with different colors representing the
     clusters of the data points identified by the `KdeSetPointIdentificator` estimator.
 
     Parameters
     ----------
-        X : pandas.DataFrame
+        X : pandas.DataFrame | pandas.Series
             The input data with shape (n_samples, 1).
         estimator : corrai.learning.KdeSetPointIdentificator, optional
             An instance of KdeSetPointIdentificator to use for clustering the data.
             Defaults to `KdeSetPointIdentificator` with default values.
         sk_scaler : object, optional
             An instance of the scaler to use for preprocessing the
             data. Defaults to `StandardScaler`.
@@ -334,17 +351,17 @@
             The title of the plot. Defaults to "Clustered Timeseries".
         y_label : str
             The label of the y-axis. Defaults to "[-]".
     """
     X = as_1_column_dataframe(X)
 
     if sk_scaler is None:
-        pd_scaler = ct.PdSkTransformer(StandardScaler())
+        pd_scaler = PdSkTransformer(StandardScaler())
     else:
-        pd_scaler = ct.PdSkTransformer(sk_scaler)
+        pd_scaler = PdSkTransformer(sk_scaler)
 
     if estimator is None:
         estimator = KdeSetPointIdentificator()
 
     model = make_pipeline(pd_scaler, estimator)
     cluster_col = model.fit_predict(X)
 
@@ -394,15 +411,20 @@
         font=dict(size=14),
     )
 
     fig.show()
 
 
 def plot_time_series_kde(
-    X, title="Likelihood and data", x_label="", scaled=True, bandwidth=0.1, xbins=100
+    X: pd.DataFrame | pd.Series,
+    title: str = "Likelihood and data",
+    x_label: str = "",
+    scaled: bool = True,
+    bandwidth: float = 0.1,
+    xbins: int = 100,
 ):
     """
     Plots the likelihood function and histogram of the input data as estimated by
     kernel density estimation.
 
     Parameters
     ----------
```

### Comparing `corrai-0.2.0/corrai/learning/model_selection.py` & `corrai-0.3.0/corrai/learning/model_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sklearn.neural_network import MLPRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.svm import SVR
 from sklearn.utils.validation import check_is_fitted
 
 from corrai.metrics import nmbe, cv_rmse
-from corrai.utils import as_1_column_dataframe
+from corrai.base.utils import as_1_column_dataframe
 
 
 class Model(str, enum.Enum):
     TREE_REGRESSOR = "TREE_REGRESSOR"
     RANDOM_FOREST = "RANDOM_FOREST"
     LINEAR_REGRESSION = "LINEAR_REGRESSION"
     LINEAR_SECOND_ORDER = "LINEAR_SECOND_ORDER"
```

### Comparing `corrai-0.2.0/corrai/math.py` & `corrai-0.3.0/corrai/base/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import numpy as np
 
 from scipy import integrate
 from collections.abc import Callable
 
-from corrai.utils import as_1_column_dataframe
-from corrai.utils import check_datetime_index
+from corrai.base.utils import as_1_column_dataframe
+from corrai.base.utils import check_datetime_index
 
 
 def time_gradient(data):
     """
     Calculates the time gradient of a given time series `data`
     between two optional time bounds `begin` and `end`.
 
@@ -204,7 +204,24 @@
         return pd.Series(
             [
                 agg_method(result_df.iloc[:, i], **agg_method_kwarg)
                 for i in range(len(result_df.columns))
             ],
             index=result_df.columns,
         )
+
+
+def cosd(angle):
+    """
+    Cosine with angle input in degrees
+    """
+    res = np.cos(np.radians(angle))
+    return res
+
+
+def sind(angle):
+    """
+    Sine with angle input in degrees
+    """
+
+    res = np.sin(np.radians(angle))
+    return res
```

### Comparing `corrai-0.2.0/corrai/measure.py` & `corrai-0.3.0/corrai/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from sklearn.compose import ColumnTransformer
 from sklearn.pipeline import make_pipeline
 
 import corrai.transformers as ct
+from corrai.base.math import time_integrate
 from corrai.transformers import PdIdentity
-from corrai.utils import check_datetime_index
-from corrai.math import time_integrate
+from corrai.base.utils import check_datetime_index
 
 
-class Transformer(str, Enum):
+class Transformer(Enum):
     DROPNA = "DROPNA"
     RENAME_COLUMNS = "RENAME_COLUMNS"
     SK_TRANSFORMER = "SK_TRANSFORMER"
     DROP_THRESHOLD = "DROP_THRESHOLD"
     DROP_TIME_GRADIENT = "DROP_TIME_GRADIENT"
     APPLY_EXPRESSION = "APPLY_EXPRESSION"
     TIME_GRADIENT = "TIME_GRADIENT"
@@ -43,22 +43,32 @@
     "BFILL": ct.PdBfill,
     "FFILL": ct.PdFfill,
     "RESAMPLE": ct.PdResampler,
     "INTERPOLATE": ct.PdInterpolate,
     "GAUSSIAN_FILTER": ct.PdGaussianFilter1D,
 }
 
+ENCODING_MAP = {"Transformer": Transformer}
+
 
 class AggMethod(str, Enum):
     MEAN = "MEAN"
     SUM = "SUM"
+    CUMSUM = "CUMSUM"
+    DIFF = "DIFF"
     TIME_INTEGRATE = "TIME_INTEGRATE"
 
 
-AGG_METHOD_MAP = {"MEAN": np.mean, "SUM": np.sum, "TIME_INTEGRATE": time_integrate}
+AGG_METHOD_MAP = {
+    "MEAN": "mean",
+    "SUM": "sum",
+    "CUMSUM": "cusmsum",
+    "DIFF": "diff",
+    "TIME_INTEGRATE": time_integrate,
+}
 
 COLOR_PALETTE = ["#FFAD85", "#FF8D70", "#ED665A", "#52E0B6", "#479A91"]
 
 
 def missing_values_dict(df):
     return {
         "Number_of_missing": df.count(),
@@ -201,18 +211,36 @@
                 fillcolor=f"rgba({color_rgb[0]}, {color_rgb[1]},"
                 f" {color_rgb[2]} , {alpha})",
                 yaxis=yaxis,
             )
         )
 
 
+class CustomEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, Enum):
+            return {"__enum__": str(obj.__class__.__name__), "value": obj.value}
+        return json.JSONEncoder.default(self, obj)
+
+
+class CustomDecoder(json.JSONDecoder):
+    def __init__(self, *args, **kwargs):
+        super().__init__(object_hook=self.dict_to_object, *args, **kwargs)
+
+    def dict_to_object(self, d):
+        if "__enum__" in d:
+            enum_class = ENCODING_MAP[d["__enum__"]]
+            return enum_class(d["value"])
+        return d
+
+
 class MeasuredDats:
     def __init__(
         self,
-        data: pd.DataFrame,
+        data: pd.DataFrame = None,
         category_dict: dict[str, list[str]] = None,
         category_transformations=None,
         common_transformations=None,
         resampler_agg_methods=None,
         transformers_list=None,
         config_file_path=None,
     ):
@@ -229,15 +257,15 @@
             category-specific transformations. Defaults to None. The dictionary
             keys must match the category name. For each category, a dictionary is
             specified. The keys are the transformer name, the value is a list
             ['transformer_map_name', {Corrai transformer args}]. Use only
             transformers defined in TRANSFORMER_MAP. If necessary a specific key
             "RESAMPLE" may be provided to specify an aggregation method. Method
             must be in RESAMPLE_METHS dict. If not specified, default aggreagation
-            method is np.mean. An exemple of configuration is given below
+            method is mean. An exemple of configuration is given below
 
         common_transformations (dict, optional): A dictionary specifying common
             transformations. The keys are the transformer name, the value is a list
             ['transformer_map_name', {Corrai transformer args}]. Use only
             transformers defined in TRANSFORMER_MAP. An example of configuration
             is given below
 
@@ -268,14 +296,17 @@
                 transformations.
 
             common_trans_names (list): Returns the names of common
                 transformations.
 
         Methods:
         --------
+        set_data(data:DataFrame): The proper way or reset DataFrame. Check index
+            is valid, before assigning data to self.data.
+
         get_pipeline(transformers_list=None, resampling_rule=False): Creates
             and returns a data processing pipeline. Custom transformer list
             may be specified. resampling_rule add a resampler to the pipeline.
 
         get_corrected_data(transformers_list=None, resampling_rule=False):
             Applies the pipeline to the data and returns the corrected data.
             Custom transformer list may be specified. resampling_rule add a
@@ -414,28 +445,30 @@
                 "radiation": "sum" # Method is just an example.
             },
             transformers_list=["ANOMALIES", "COMMON"]
         )
 
         >>>my_data.get_corrected_data()
         """
-        check_datetime_index(data)
-        self.data = data
+        if data is not None:
+            self.set_data(data)
+        else:
+            self.data = None
 
         if config_file_path is None:
             self.category_dict = category_dict
             self.category_trans = category_transformations
             self.common_trans = common_transformations
             self.transformers_list = transformers_list
             self.resampler_agg_methods = resampler_agg_methods
         else:
             self.read_config_file(config_file_path)
 
-        if self.category_dict is None:
-            self.category_dict = {"data": data.columns}
+        if self.category_dict is None and self.data is not None:
+            self.category_dict = {"data": self.data.columns}
 
         if self.category_trans is None:
             self.category_trans = {}
 
         if self.common_trans is None:
             self.common_trans = {}
 
@@ -456,14 +489,18 @@
         return list(dict.fromkeys(lst))
 
     @property
     def common_trans_names(self):
         lst = list(self.common_trans.keys())
         return list(dict.fromkeys(lst))
 
+    def set_data(self, data: pd.DataFrame):
+        check_datetime_index(data)
+        self.data = data
+
     def get_missing_value_stats(self, transformers_list=None, resampling_rule=False):
         data = self.get_corrected_data(transformers_list, resampling_rule)
         return missing_values_dict(data)
 
     def get_gaps_description(
         self,
         cols=None,
@@ -476,31 +513,31 @@
         data = self.get_corrected_data(transformers_list, resampling_rule)
         return gaps_describe(df_in=data, cols=cols, timestep=gaps_timedelta)
 
     def get_pipeline(self, transformers_list=None, resampling_rule=False):
         if transformers_list is None:
             transformers_list = self.transformers_list.copy()
 
-        if Transformer.RESAMPLE in transformers_list and not resampling_rule:
+        if Transformer.RESAMPLE.value in transformers_list and not resampling_rule:
             raise ValueError(
                 "RESAMPLE is present in transformers_list but no rule"
                 "have been specified. use resampling_rule argument"
             )
 
-        if resampling_rule and Transformer.RESAMPLE not in transformers_list:
-            transformers_list += [Transformer.RESAMPLE]
+        if resampling_rule and Transformer.RESAMPLE.value not in transformers_list:
+            transformers_list += [Transformer.RESAMPLE.value]
 
         if not transformers_list:
             obj_list = [PdIdentity()]
         else:
             obj_list = []
             for trans in transformers_list:
                 if trans in self.category_trans_names:
                     obj_list.append(self.get_category_transformer(trans))
-                elif trans == Transformer.RESAMPLE:
+                elif trans == Transformer.RESAMPLE.value:
                     obj_list.append(self.get_resampler(resampling_rule))
                 else:
                     obj_list.append(self.get_common_transformer(trans))
 
         return make_pipeline(*obj_list)
 
     def get_corrected_data(self, transformers_list=None, resampling_rule=False):
@@ -547,15 +584,15 @@
             try:
                 method = self.resampler_agg_methods[data_cat]
                 column_config_list.append((cols, AGG_METHOD_MAP[method.value]))
             except KeyError:
                 pass
 
         if not column_config_list:
-            return ct.PdResampler(rule=rule, method=np.mean)
+            return ct.PdResampler(rule=rule, method=AGG_METHOD_MAP["MEAN"])
         else:
             return ct.PdColumnResampler(
                 rule=rule,
                 columns_method=column_config_list,
                 remainder=AGG_METHOD_MAP[remainder_rule.value],
             )
 
@@ -564,19 +601,19 @@
             to_dump = {
                 "category_dict": self.category_dict,
                 "category_transformations": self.category_trans,
                 "common_transformations": self.common_trans,
                 "transformers_list": self.transformers_list,
                 "resampler_agg_methods": self.resampler_agg_methods,
             }
-            json.dump(to_dump, f, ensure_ascii=False, indent=4)
+            json.dump(to_dump, f, indent=4, cls=CustomEncoder)
 
     def read_config_file(self, file_path):
         with open(file_path, encoding="utf-8") as f:
-            config_dict = json.load(f)
+            config_dict = json.load(f, cls=CustomDecoder)
 
         attribute_list = [
             ("category_dict", "category_dict"),
             ("category_transformations", "category_trans"),
             ("common_transformations", "common_trans"),
             ("transformers_list", "transformers_list"),
             ("resampler_agg_methods", "resampler_agg_methods"),
```

### Comparing `corrai-0.2.0/corrai/metrics.py` & `corrai-0.3.0/corrai/metrics.py`

 * *Files identical despite different names*

### Comparing `corrai-0.2.0/corrai/multi_optimize.py` & `corrai-0.3.0/corrai/multi_optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         parameters: list[dict[Parameter, Any]],
         obj_func_list,
         func_list,
         function_names,
         constraint_names,
     ):
         self.parameters = parameters
+        _check_duplicate_params(parameters)
         if len(obj_func_list) == 0 and len(func_list) == 0:
             raise ValueError(
                 "At least one of obj_func_list or func_list should be provided"
             )
         self.obj_func_list = obj_func_list
         self.func_list = func_list
         self.function_names = function_names
@@ -172,14 +173,15 @@
         parameters: list[dict[Parameter, Any]],
         obj_func_list,
         func_list,
         function_names,
         constraint_names,
     ):
         self.parameters = parameters
+        _check_duplicate_params(parameters)
         if len(obj_func_list) == 0 and len(func_list) == 0:
             raise ValueError(
                 "At least one of obj_func_list or func_list should be provided"
             )
         self.obj_func_list = obj_func_list
         self.func_list = func_list
         self.function_names = function_names
@@ -278,7 +280,24 @@
         )
     )
 
     fig.show()
 
     if html_file_path:
         pio.write_html(fig, html_file_path)
+
+
+def _check_duplicate_params(params):
+    """
+    Check for duplicate parameter names in the list of parameters.
+
+    Raises
+    ------
+    ValueError
+        If duplicate parameter names are found.
+    """
+    param_names = set()
+    for param in params:
+        name = param[Parameter.NAME]
+        if name in param_names:
+            raise ValueError(f"Duplicate parameter name: {name}")
+        param_names.add(name)
```

### Comparing `corrai-0.2.0/corrai/sensitivity.py` & `corrai-0.3.0/corrai/sensitivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from SALib.analyze import fast, morris, sobol, rbd_fast
 from SALib.sample import sobol as sobol_sampler
 from SALib.sample import fast_sampler, latin
 from SALib.sample import morris as morris_sampler
 
 from corrai.base.parameter import Parameter
 from corrai.base.simulate import run_simulations
-from corrai.math import aggregate_time_series
+from corrai.base.math import aggregate_time_series
 from corrai.multi_optimize import plot_parcoord
 
 
 class Method(enum.Enum):
     FAST = "FAST"
     MORRIS = "MORRIS"
     SOBOL = "SOBOL"
```

### Comparing `corrai-0.2.0/corrai/transformers.py` & `corrai-0.3.0/corrai/transformers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pandas as pd
 import numpy as np
 import datetime as dt
 from functools import partial
 from sklearn.base import TransformerMixin, BaseEstimator
-from corrai.math import time_gradient
+from corrai.base.math import time_gradient
 from scipy.ndimage import gaussian_filter1d
 from abc import ABC, abstractmethod
+from collections.abc import Callable
 
 
 class PdTransformerBC(TransformerMixin, BaseEstimator, ABC):
     def __init__(self):
         self.columns = None
         self.index = None
 
@@ -708,42 +709,33 @@
     transform(X)
         Resample the input DataFrame based on the specified resampling methods.
     get_feature_names_out()
         Return the names of the new features created in `transform()`.
 
     """
 
-    def __init__(self, rule, columns_method, remainder="drop"):
+    def __init__(self, rule, columns_method, remainder: str | Callable = "drop"):
         super().__init__()
         self.rule = rule
         self.columns_method = columns_method
         self.resampled_index = None
-
-        if remainder != "drop" and not callable(remainder):
-            raise ValueError(
-                "If remainder is no set to drop. Aggregation "
-                "method must be provided to ensure transformed "
-                "index consistency"
-            )
-        else:
-            self.remainder = remainder
+        self.remainder = remainder
         self._check_columns_method()
 
     def _check_columns_method(self):
         if not isinstance(self.columns_method, list):
             raise ValueError(
                 "Columns_method must be a list of Tuple"
                 "first index shall be a list of columns names,"
-                "second index shall be an aggregation method"
+                "second index shall be an aggregation method callable or pandas"
+                "Groupby method name"
             )
         for elmt in self.columns_method:
             if not isinstance(elmt[0], list):
                 raise ValueError("Tuple first element must be a list" "of columns")
-            if not callable(elmt[1]):
-                raise ValueError("Tuple second element must be a" "callable")
 
     def _check_columns(self, X):
         for col_list, _ in self.columns_method:
             for col in col_list:
                 if col not in X.columns:
                     raise ValueError("Columns in columns_method not found in" "X")
 
@@ -797,15 +789,15 @@
     -----------
     time_lag : datetime.timedelta
         The time lag used to shift the provided features. A positive time lag
         indicates that the new features will contain information from the past,
          while a negative time lag indicates that the new features will
         contain information from the future.
 
-    features_to_lag : list or None, optional (default=None)
+    features_to_lag : list of str or str or None, optional (default=None)
         The list of feature names to lag. If None, all features in the input
          DataFrame will be lagged.
 
     feature_marker : str or None, optional (default=None)
         The string used to prefix the names of the new lagged features.
         If None, the feature names will be prefixed with the string
         representation of the `time_lag` parameter followed by an underscore.
@@ -813,35 +805,28 @@
     drop_resulting_nan : bool, optional (default=False)
         Whether to drop rows with NaN values resulting from the lag operation.
 
     """
 
     def __init__(
         self,
-        time_lag,
-        features_to_lag=None,
-        feature_marker=None,
+        time_lag: dt.timedelta,
+        features_to_lag: str | list[str] = None,
+        feature_marker: str = None,
         drop_resulting_nan=False,
     ):
         super().__init__()
-        if not isinstance(time_lag, dt.timedelta):
-            raise ValueError(
-                "Invalid time_lag value. You must provide "
-                "a datetime.timedelta object"
-            )
         self.time_lag = time_lag
-        self.features_to_lag = features_to_lag
+        self.features_to_lag = (
+            [features_to_lag] if isinstance(features_to_lag, str) else features_to_lag
+        )
         self.drop_resulting_nan = drop_resulting_nan
-
-        if feature_marker is None:
-            self.feature_marker = str(time_lag) + "_"
-        else:
-            if not isinstance(feature_marker, str):
-                raise ValueError("feature_marker must be a string")
-            self.feature_marker = feature_marker
+        self.feature_marker = (
+            str(time_lag) + "_" if feature_marker is None else feature_marker
+        )
 
     def fit(self, X, y=None):
         return self
 
     def transform(self, X):
         if self.features_to_lag is None:
             self.features_to_lag = X.columns
```

### Comparing `corrai-0.2.0/corrai/tsgenerator.py` & `corrai-0.3.0/corrai/tsgenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,15 +198,18 @@
     in a building based on either RE2020 or COSTIC coefficients.
 
     Warning1: Note that for a small number of dwellings (less than 6),
     the calculation method for random shower water distribution is
     not adapted: since the method uses COSTIC water flow calculations
     for each hour and then randomly distribute showers, it does not
     work properly for small amount of water (nb of shower per hour < 1
-    results in 0 shower). Will be addressed in future work.
+    results in 0 shower). Will result in high underestimation for small
+    n_dwellings. Likewise, can result in slight under- or over-
+    estimation for high number of dwellings.
+    Will be addressed in future work.
 
     Warning2: Water consumption for showers is limited here by a
     water consumption per dwelling in liters per day, then distributed
     using daily COSTIC coefficients. Although COSTIC coefficients are
     calculated for each day of the year, and are representative of
     higher probability of having showers at certain hours, they do
     not impact the total water consumption.
@@ -356,15 +359,15 @@
         Raises:
             ValueError: If start or end values are not valid timestamps.
         """
 
         if not pd.Timestamp(start) or not pd.Timestamp(end):
             raise ValueError("Start and end values must be valid timestamps.")
 
-        date_index = pd.date_range(start=start, end=end, freq="H")
+        date_index = pd.date_range(start=start, end=end, freq="h")
         self.df_coefficient = pd.DataFrame(
             data=np.zeros(date_index.shape[0]), index=date_index, columns=["coef"]
         )
 
         val_list = []
         if self.method == "COSTIC":
             for val in self.df_coefficient.index:
@@ -473,15 +476,15 @@
             raise ValueError("Method has to be COSTIC for random shower distribution")
 
         if seed is not None:
             rs = RandomState(MT19937(SeedSequence(seed)))
         else:
             rs = RandomState()
 
-        periods = pd.date_range(start=start, end=end, freq="T")
+        periods = pd.date_range(start=start, end=end, freq="min")
         df_costic = self.costic_shower_distribution(start, end)
         df_costic["nb_shower"] = df_costic["Q_ECS_COSTIC"] / self.v_used
         df_costic["t_shower_per_hour"] = df_costic["nb_shower"] * self.t_shower
         df_costic["nb_shower_int"] = np.round(df_costic["nb_shower"]).astype(int)
 
         rs_dd = rs.randint(
             0, 60 - self.t_shower, (len(periods), df_costic["nb_shower_int"].max())
@@ -495,15 +498,15 @@
                 distribution[start_shower : start_shower + self.t_shower] += 1
             distribution_list.append(distribution)
 
         df_costic_random = pd.DataFrame(
             data=np.concatenate(distribution_list),
             index=pd.date_range(
                 df_costic["nb_shower_int"].index[0],
-                freq="T",
+                freq="min",
                 periods=df_costic.shape[0] * 60,
             ),
             columns=["shower_per_minute"],
         )
 
         df_costic_random["Q_ECS_COSTIC_rd"] = (
             df_costic_random["shower_per_minute"] * self.v_used / self.t_shower
@@ -532,15 +535,15 @@
             end (str): End date of the time period (format: 'YYYY-MM-DD').
 
         Returns:
             pd.DataFrame: DataFrame containing the
             calculated hot water consumption for showers
             with timestamps as index.
         """
-        periods = pd.date_range(start=start, end=end, freq="H")
+        periods = pd.date_range(start=start, end=end, freq="h")
         self.get_coefficient_calc_from_period(start, end)
         # N_calculation
         if self.s_moy_dwelling < 10:
             nmax = 1
         elif self.s_moy_dwelling in {10: 49.99}:
             nmax = 1.75 - 0.01875 * (50 - self.s_moy_dwelling)
         else:
@@ -622,15 +625,15 @@
         self.seed = seed
 
         if not dish_washer and not washing_machine:
             raise ValueError(
                 "At least one of washing machine or dish washer must be True"
             )
 
-        date_index = pd.date_range(start=start, end=end, freq="H")
+        date_index = pd.date_range(start=start, end=end, freq="h")
         if self.seed is not None:
             rs = RandomState(MT19937(SeedSequence(self.seed)))
         else:
             rs = RandomState()
 
         nb_days = (end - start).days + 1
 
@@ -789,15 +792,15 @@
         nb_washbasin = round(self.v_washbasin / self.v_washbasin_used)
         nb_sinkcook = round(self.v_sink_cook / self.v_sinkcook_used)
         nb_sinkdishes = round(self.v_sink_dishes / self.v_sinkdishes_used)
         nb_sinkcleaning = round(self.v_sink_cleaning / self.v_sinkcleaning_used)
 
         coef = self.get_coefficient_calc_from_period(start, end)
         coefficient = coef.mask(coef["coef"] < 0.5)
-        coefficient = coefficient.resample("T").ffill().fillna(float("0"))
+        coefficient = coefficient.resample("min").ffill().fillna(float("0"))
 
         list_washbasin = []
         list_sinkcook = []
         list_sinkdishes = []
         list_sinkwash = []
 
         for _ in range((end - start).days):
@@ -952,22 +955,24 @@
     def _get_day_dict(self):
         """
         Returns a dictionary with daily schedules based on the configuration settings.
         :return: dict containing DatFrame
         """
         day_dict = {}
         for day in self.config_dict["DAYS"].keys():
-            day_df = pd.DataFrame(index=["00:00"])
-            for hour, prog in self.config_dict["DAYS"][day].items():
-                day_df.loc[hour, prog.keys()] = prog.values()
+            day_df = pd.DataFrame.from_dict(
+                self.config_dict["DAYS"][day], orient="index"
+            )
+            if "00:00" not in day_df.index:
+                day_df.loc["00:00", :] = [np.nan] * len(day_df.columns)
             day_dict[day] = day_df
 
         return day_dict
 
-    def get_full_year_time_series(self, year=None, freq="T"):
+    def get_full_year_time_series(self, year=None, freq="min"):
         """
         Generates and returns the scheduled DataFrame based on the configuration
         settings.
 
         :param year: Year to generate the time series for. Default is current year
         :param str freq: output DataFrame DateTimeIndex frequency
         """
@@ -997,11 +1002,72 @@
                     )
                     current_day.index = new_index.tz_localize(self.config_dict["TZ"])
                     day_list.append(current_day)
 
         df = pd.concat(day_list)
         df.sort_index(inplace=True)
         df = df.bfill()
-        df = df.resample("T").bfill()
+        df = df.resample("min").bfill()
         df = df.shift(-1)
         df = df.ffill()
         return df.resample(freq).mean()
+
+
+def calculate_power(
+    df,
+    deltaT,
+    Cp=4180,
+    ro=1,
+):
+    """
+    Calculate power consumption based on given DataFrame.
+
+    Parameters:
+        df (DataFrame): DataFrame containing the data for power calculation.
+        The flow rates of water should be in L/h.
+        deltaT (float): Temperature difference (in Kelvin).
+        Cp (float): Specific heat capacity of the fluid (4180 J/(kg·Kelvin)
+            for water by default).
+        ro (float): Density of medium (1 kg/L for water by default )
+
+    Returns:
+        DataFrame: DataFrame containing the calculated power consumption
+        for each column in the input DataFrame, expressed in kW.
+    """
+    df_powers = df * Cp * ro * deltaT / 3.6e6
+    df_powers.columns = ["P_" + col for col in df.columns + "(kW)"]
+
+    return df_powers
+
+
+def resample_flow_rate(df, new_freq):
+    """
+    Resample the flow rate hour columns of DataFrame to a new frequency.
+
+    Parameters:
+        df (DataFrame): DataFrame containing the flow
+        rate data to be resampled.
+        new_freq (str): New frequency desired for resampling
+        (e.g., '30T' for every 30 minutes).
+
+    Returns:
+        DataFrame: DataFrame with flow rate columns resampled to the new frequency.
+
+    """
+    original_freq = df.index.freqstr
+    if original_freq is None:
+        raise ValueError(
+            "DataFrame index does not have a frequency. "
+            "Please set the frequency before resampling."
+        )
+
+    resampled_df = df.resample(new_freq).first()
+
+    if original_freq is not None:
+        original_minutes = pd.Timedelta(df.index[1] - df.index[0]).total_seconds() / 60
+        new_minutes = pd.Timedelta(new_freq).total_seconds() / 60
+        ratio = original_minutes / new_minutes
+
+        resampled_df = resampled_df / ratio
+    resampled_df = resampled_df.interpolate(method="linear")
+
+    return resampled_df
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `corrai-0.2.0/corrai/utils.py` & `corrai-0.3.0/corrai/base/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         return [function(i) for i in x]
     elif isinstance(x, np.ndarray):
         return np.vectorize(function)(x)
     elif isinstance(x, pd.Series):
         return x.apply(function)
     elif isinstance(x, pd.DataFrame):
         # applymap will be deprecated in future version
-        return x.applymap(function)
+        return x.map(function)
 
     return function(x)
 
 
 def float_to_hour(hours_float):
     """
     Convert a float value representing hours to a string representation with the
```

### Comparing `corrai-0.2.0/corrai/variant.py` & `corrai-0.3.0/corrai/variant.py`

 * *Files identical despite different names*

### Comparing `corrai-0.2.0/corrai.egg-info/PKG-INFO` & `corrai-0.3.0/corrai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corrai
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data correction and Machine Learning
 Home-page: https://github.com/BuildingEnergySimulationTools/corrai
 Author: Nobatek/INEF4
 Author-email: bdurandestebe@nobatek.inef4.com
 License: License :: OSI Approved :: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/BuildingEnergySimulationTools/corrai/main/logo_corrai.svg" alt="CorrAI" width="200"/>
 </p>
 
-[![Static Badge](https://img.shields.io/badge/version-0.1.0-orange)](https://pypi.org/project/corrai/)
+[![Static Badge](https://img.shields.io/badge/version-0.3.0-orange)](https://pypi.org/project/corrai/)
 [![Static Badge](https://img.shields.io/badge/python-3.10_%7C_3.12-blue)](https://pypi.org/project/corrai/)
 [![codecov](https://codecov.io/gh/BuildingEnergySimulationTools/corrai/branch/main/graph/badge.svg?token=F51O9CXI61)](https://codecov.io/gh/BuildingEnergySimulationTools/corrai)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 
 ## Measured Data Exploration for Physical and Mathematical Models
```

### Comparing `corrai-0.2.0/corrai.egg-info/SOURCES.txt` & `corrai-0.3.0/corrai.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENCE.md
 README.md
 setup.cfg
 setup.py
 corrai/__init__.py
-corrai/math.py
+corrai/fmu.py
 corrai/measure.py
 corrai/metrics.py
 corrai/multi_optimize.py
 corrai/sensitivity.py
 corrai/transformers.py
 corrai/tsgenerator.py
-corrai/utils.py
 corrai/variant.py
 corrai.egg-info/PKG-INFO
 corrai.egg-info/SOURCES.txt
 corrai.egg-info/dependency_links.txt
 corrai.egg-info/requires.txt
 corrai.egg-info/top_level.txt
 corrai/base/__init__.py
+corrai/base/math.py
 corrai/base/model.py
 corrai/base/parameter.py
 corrai/base/simulate.py
+corrai/base/solar.py
+corrai/base/utils.py
 corrai/learning/__init__.py
 corrai/learning/cluster.py
 corrai/learning/model_selection.py
```

### Comparing `corrai-0.2.0/setup.py` & `corrai-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="corrai",
-    version="0.2.0",
+    version="0.3.0",
     description="Data correction and Machine Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BuildingEnergySimulationTools/corrai",
     author="Nobatek/INEF4",
     author_email="bdurandestebe@nobatek.inef4.com",
     license="License :: OSI Approved :: BSD License",
@@ -26,20 +26,21 @@
         "Topic :: Scientific/Engineering",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     python_requires=">=3.10",
     install_requires=[
-        "numpy>=1.22.0",
-        "pandas>=1.3.4",
+        "numpy>=1.22.4",
+        "pandas>=2.1.0",
         "scipy>=1.9.1",
         "matplotlib>=3.5.1",
         "plotly>=5.3.1",
         "scikit-learn>=1.2.2",
         "pymoo>=0.6.0.1",
         "salib>=1.4.7",
         "fastprogress>=1.0.3",
+        "fmpy>=0.3.6",
     ],
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
 )
```

