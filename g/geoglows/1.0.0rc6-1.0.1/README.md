# Comparing `tmp/geoglows-1.0.0rc6.tar.gz` & `tmp/geoglows-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.0rc6.tar", last modified: Tue Apr  9 04:56:33 2024, max compression
+gzip compressed data, was "geoglows-1.0.1.tar", last modified: Tue Apr  9 20:45:48 2024, max compression
```

## Comparing `geoglows-1.0.0rc6.tar` & `geoglows-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,30 @@
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.873415 geoglows-1.0.0rc6/
--rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/.gitignore
--rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/.readthedocs.yml
--rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/LICENSE
--rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-09 04:56:33.873147 geoglows-1.0.0rc6/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      704 2024-04-06 20:53:01.000000 geoglows-1.0.0rc6/README.md
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.867459 geoglows-1.0.0rc6/docs/
--rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/Makefile
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.867624 geoglows-1.0.0rc6/docs/_static/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/_static/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.867737 geoglows-1.0.0rc6/docs/_templates/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/_templates/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.868438 geoglows-1.0.0rc6/docs/api-documentation/
--rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/analysis.rst
--rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/bias.rst
--rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/examples.rst
--rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/plots.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/streamflow.rst
--rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-04-06 20:51:08.000000 geoglows-1.0.0rc6/docs/conf.py
--rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/dev-notes.rst
--rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/index.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/license.rst
--rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/environment.yaml
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.869939 geoglows-1.0.0rc6/geoglows/
--rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-09 04:55:25.000000 geoglows-1.0.0rc6/geoglows/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc6/geoglows/_constants.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.872297 geoglows-1.0.0rc6/geoglows/_plots/
--rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc6/geoglows/_plots/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc6/geoglows/_plots/format_tools.py
--rw-r--r--   0 rchales    (502) staff       (20)    16418 2024-04-07 22:21:17.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 rchales    (502) staff       (20)    11334 2024-04-07 22:18:05.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-07 22:21:17.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/geoglows/_plots/plots.py
--rw-r--r--   0 rchales    (502) staff       (20)     7939 2024-04-07 22:18:05.000000 geoglows-1.0.0rc6/geoglows/analyze.py
--rw-r--r--   0 rchales    (502) staff       (20)     8241 2024-04-06 20:51:08.000000 geoglows-1.0.0rc6/geoglows/bias.py
--rw-r--r--   0 rchales    (502) staff       (20)    12910 2024-04-09 04:54:37.000000 geoglows-1.0.0rc6/geoglows/data.py
--rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/geoglows/streams.py
--rw-r--r--   0 rchales    (502) staff       (20)     3811 2024-04-07 22:18:05.000000 geoglows-1.0.0rc6/geoglows/tables.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.872892 geoglows-1.0.0rc6/geoglows.egg-info/
--rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/requires.txt
--rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/top_level.txt
--rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc6/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-09 04:56:33.873460 geoglows-1.0.0rc6/setup.cfg
--rw-r--r--   0 rchales    (502) staff       (20)     1650 2024-04-06 20:52:15.000000 geoglows-1.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.479342 geoglows-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 20:45:44.000000 geoglows-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 20:45:44.000000 geoglows-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 20:45:48.479342 geoglows-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 20:45:44.000000 geoglows-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.475342 geoglows-1.0.1/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.479342 geoglows-1.0.1/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.479342 geoglows-1.0.1/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 20:45:44.000000 geoglows-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:45:48.479342 geoglows-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 20:45:44.000000 geoglows-1.0.1/setup.py
```

### Comparing `geoglows-1.0.0rc6/LICENSE` & `geoglows-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/PKG-INFO` & `geoglows-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
@@ -19,15 +19,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: fastparquet
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: plotly>=5
-Requires-Dist: shapely>=2
 Requires-Dist: scipy>=1
 Requires-Dist: s3fs
 Requires-Dist: numpy>=1
 Requires-Dist: hydrostats
 Requires-Dist: HydroErr
 Requires-Dist: xarray
 Requires-Dist: zarr
```

### Comparing `geoglows-1.0.0rc6/README.md` & `geoglows-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/_plots/format_tools.py` & `geoglows-1.0.1/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.1/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.1/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.1/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.1/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/_plots/plots.py` & `geoglows-1.0.1/geoglows/_plots/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 from .plotly_retrospective import (
     retrospective as plotly_retrospective,
     daily_averages as plotly_daily_averages,
     monthly_averages as plotly_monthly_averages,
     annual_averages as plotly_annual_averages
 )
 
+__all__ = [
+    'forecast',
+    'forecast_stats',
+    'forecast_ensembles',
+    'retrospective',
+    'daily_averages',
+    'monthly_averages',
+    'annual_averages',
+    'daily_variance',
+    'flow_duration_curve',
+]
+
 
 def forecast(df: pd.DataFrame, *,
              plot_type: str = 'plotly',
              rp_df: pd.DataFrame = None,
              plot_titles: list = None, ) -> go.Figure:
     """
     Plots forecasted streamflow and optional return periods
```

### Comparing `geoglows-1.0.0rc6/geoglows/analyze.py` & `geoglows-1.0.1/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/bias.py` & `geoglows-1.0.1/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/data.py` & `geoglows-1.0.1/geoglows/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 return dates
             date = dates[-1]
         s3store = s3fs.S3Map(root=f'{ODP_FORECAST_S3_BUCKET_URI}/{date}', s3=s3, check=False)
 
         df = xr.open_zarr(s3store).sel(rivid=reach_id).to_dataframe().round(2).reset_index()
 
         # rename columns to match the REST API
-        if type(reach_id) is list:
+        if isinstance(reach_id, list):
             df = df.pivot(columns='ensemble', index=['time', 'rivid'], values='Qout')
         else:
             df = df.pivot(index='time', columns='ensemble', values='Qout')
         df = df[sorted(df.columns)]
         df.columns = [f'ensemble_{str(x).zfill(2)}' for x in df.columns]
 
         if product_name == 'forecastensembles':
@@ -145,105 +145,109 @@
             return df
         elif return_format == 'json':
             return response.json()
         else:
             raise ValueError(f'Unsupported return format requested: {return_format}')
 
     def main(*args, **kwargs):
-        source = kwargs.get('data_source', 'rest')
+        source = kwargs.get('data_source', 'aws')
         assert source in ('rest', 'aws'), ValueError(f'Unrecognized data source requested: {source}')
         if source == 'rest':
             return from_rest(*args, **kwargs)
         else:
             return from_aws(*args, **kwargs)
-
     return main
 
 
 # Forecast data and derived products
 @_forecast_endpoint_decorator
 def dates(**kwargs) -> dict or str:
     """
     Gets a list of available forecast product dates
 
     Keyword Args:
-        format: csv, json, or url, default csv
-        data_source: location to query for data, either 'rest' or 'aws'
+        return_format: csv, json, or url, default csv
+        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         dict or str
 
         the csv is a single column with a header of 'available_dates' and 1 row per date, sorted oldest to newest
         The dictionary structure is {'available_dates': ['list', 'of', 'dates', 'YYYYMMDD', 'format']}
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast(*, reach_id: int, **kwargs) -> pd.DataFrame or dict or str:
+def forecast(*, reach_id: int, date: str, return_format: str, data_source: str,
+             **kwargs) -> pd.DataFrame or dict or str:
     """
     Gets the average forecasted flow for a certain reach_id on a certain date
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        format: csv, json, or url, default csv
-        data_source: location to query for data, either 'rest' or 'aws'
+        return_format: csv, json, or url, default csv
+        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_stats(*, reach_id: int, **kwargs) -> pd.DataFrame or dict or str:
+def forecast_stats(*, reach_id: int, date: str, return_format: str, data_source: str,
+                   **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves the min, 25%, mean, median, 75%, and max river discharge of the 51 ensembles members for a reach_id
     The 52nd higher resolution member is excluded
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        format: csv, json, or url, default csv
-        data_source: location to query for data, either 'rest' or 'aws'
+        return_format: csv, json, or url, default csv
+        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_ensembles(*, reach_id: int, **kwargs) -> pd.DataFrame or dict or str:
+def forecast_ensembles(*, reach_id: int, date: str, return_format: str, data_source: str,
+                       **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves each of 52 time series of forecasted discharge for a reach_id on a certain date
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
         date: a string specifying the date to request in YYYYMMDD format, returns the latest available if not specified
-        format: csv, json, or url, default csv
-        data_source: location to query for data, either 'rest' or 'aws'
+        return_format: csv, json, or url, default csv
+        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
 
 
 @_forecast_endpoint_decorator
-def forecast_records(*, reach_id: int, **kwargs) -> pd.DataFrame or dict or str:
+def forecast_records(*, reach_id: int, start_date: str, end_date: str, return_format: str, data_source: str,
+                     **kwargs) -> pd.DataFrame or dict or str:
     """
     Retrieves a csv showing the ensemble average forecasted flow for the year from January 1 to the current date
 
     Keyword Args:
         reach_id: the ID of a stream, should be a 9 digit integer
-        start_date: a YYYYMMDD string giving the earliest date this year to include, defaults to YYYY0101
+        start_date: a YYYYMMDD string giving the earliest date this year to include, defaults to 14 days ago.
         end_date: a YYYYMMDD string giving the latest date this year to include, defaults to latest available
-        format: csv, json, or url, default csv
+        data_source: location to query for data, either 'rest' or 'aws'. default is aws.
+        return_format: csv, json, or url, default csv
 
     Returns:
         pd.DataFrame or dict or str
     """
     pass
```

### Comparing `geoglows-1.0.0rc6/geoglows/streams.py` & `geoglows-1.0.1/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows/tables.py` & `geoglows-1.0.1/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc6/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.1/geoglows.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
@@ -19,15 +19,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask
 Requires-Dist: fastparquet
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: plotly>=5
-Requires-Dist: shapely>=2
 Requires-Dist: scipy>=1
 Requires-Dist: s3fs
 Requires-Dist: numpy>=1
 Requires-Dist: hydrostats
 Requires-Dist: HydroErr
 Requires-Dist: xarray
 Requires-Dist: zarr
```

### Comparing `geoglows-1.0.0rc6/setup.py` & `geoglows-1.0.1/setup.py`

 * *Files identical despite different names*

