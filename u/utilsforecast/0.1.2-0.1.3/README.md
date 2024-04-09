# Comparing `tmp/utilsforecast-0.1.2.tar.gz` & `tmp/utilsforecast-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsforecast-0.1.2.tar", last modified: Tue Mar 26 01:13:59 2024, max compression
+gzip compressed data, was "utilsforecast-0.1.3.tar", last modified: Tue Apr  9 20:12:39 2024, max compression
```

## Comparing `utilsforecast-0.1.2.tar` & `utilsforecast-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:13:59.843509 utilsforecast-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-26 01:13:59.843509 utilsforecast-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 01:13:59.843509 utilsforecast-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:13:59.839509 utilsforecast-0.1.2/utilsforecast/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    21716 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    27214 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-03-26 01:13:51.000000 utilsforecast-0.1.2/utilsforecast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:13:59.843509 utilsforecast-0.1.2/utilsforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 01:13:59.000000 utilsforecast-0.1.2/utilsforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:39.018118 utilsforecast-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-09 20:12:39.018118 utilsforecast-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:12:39.018118 utilsforecast-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:39.014117 utilsforecast-0.1.3/utilsforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27214 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:39.014117 utilsforecast-0.1.3/utilsforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:12:38.000000 utilsforecast-0.1.3/utilsforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/top_level.txt
```

### Comparing `utilsforecast-0.1.2/CONTRIBUTING.md` & `utilsforecast-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/LICENSE` & `utilsforecast-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/PKG-INFO` & `utilsforecast-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.2
+Version: 0.1.3
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
-Requires-Dist: polars; extra == "dev"
-Requires-Dist: numba; extra == "dev"
-Requires-Dist: pandas[plot]; extra == "dev"
 Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: polars; extra == "dev"
 Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
+Requires-Dist: numba; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.2/README.md` & `utilsforecast-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/settings.ini` & `utilsforecast-0.1.3/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utilsforecast
 lib_name = utilsforecast
-version = 0.1.2
+version = 0.1.3
 min_python = 3.8
 license = apache2
 black_formatting = True
 doc_path = _docs
 lib_path = utilsforecast
 nbs_path = nbs
 recursive = True
```

### Comparing `utilsforecast-0.1.2/setup.py` & `utilsforecast-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/_modidx.py` & `utilsforecast-0.1.3/utilsforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/compat.py` & `utilsforecast-0.1.3/utilsforecast/compat.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/data.py` & `utilsforecast-0.1.3/utilsforecast/data.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/evaluation.py` & `utilsforecast-0.1.3/utilsforecast/evaluation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/feature_engineering.py` & `utilsforecast-0.1.3/utilsforecast/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/grouped_array.py` & `utilsforecast-0.1.3/utilsforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/losses.py` & `utilsforecast-0.1.3/utilsforecast/losses.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,14 +623,15 @@
     """
     eps = np.finfo(float).eps
     quantiles = np.asarray(quantiles)
     loss = mqloss(df, models, quantiles, id_col, target_col)
     sizes = ufp.counts_by_id(df, id_col)
     if isinstance(loss, pd.DataFrame):
         loss = loss.set_index(id_col)
+        sizes = sizes.set_index(id_col)
         assert isinstance(df, pd.DataFrame)
         norm = df[target_col].abs().groupby(df[id_col], observed=True).sum()
         res = 2 * loss.mul(sizes["counts"], axis=0).div(norm + eps, axis=0)
         res.index.name = id_col
         res = res.reset_index()
     else:
```

### Comparing `utilsforecast-0.1.2/utilsforecast/plotting.py` & `utilsforecast-0.1.3/utilsforecast/plotting.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/preprocessing.py` & `utilsforecast-0.1.3/utilsforecast/preprocessing.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/processing.py` & `utilsforecast-0.1.3/utilsforecast/processing.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/target_transforms.py` & `utilsforecast-0.1.3/utilsforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast/validation.py` & `utilsforecast-0.1.3/utilsforecast/validation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.2/utilsforecast.egg-info/PKG-INFO` & `utilsforecast-0.1.3/utilsforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.2
+Version: 0.1.3
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
-Requires-Dist: polars; extra == "dev"
-Requires-Dist: numba; extra == "dev"
-Requires-Dist: pandas[plot]; extra == "dev"
 Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: polars; extra == "dev"
 Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
+Requires-Dist: numba; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.2/utilsforecast.egg-info/SOURCES.txt` & `utilsforecast-0.1.3/utilsforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

