# Comparing `tmp/geoglows-1.0.0rc5.tar.gz` & `tmp/geoglows-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.0rc5.tar", last modified: Sun Apr  7 23:46:45 2024, max compression
+gzip compressed data, was "geoglows-1.0.0rc6.tar", last modified: Tue Apr  9 04:56:33 2024, max compression
```

## Comparing `geoglows-1.0.0rc5.tar` & `geoglows-1.0.0rc6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.781168 geoglows-1.0.0rc5/
--rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc5/.gitignore
--rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/.readthedocs.yml
--rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/LICENSE
--rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/MANIFEST.in
--rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-07 23:46:45.780876 geoglows-1.0.0rc5/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      704 2024-04-06 20:53:01.000000 geoglows-1.0.0rc5/README.md
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.775997 geoglows-1.0.0rc5/docs/
--rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/Makefile
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.776110 geoglows-1.0.0rc5/docs/_static/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/_static/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.776206 geoglows-1.0.0rc5/docs/_templates/
--rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/_templates/.gitkeep
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.776803 geoglows-1.0.0rc5/docs/api-documentation/
--rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/api-documentation/analysis.rst
--rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/api-documentation/bias.rst
--rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/api-documentation/examples.rst
--rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/api-documentation/plots.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/api-documentation/streamflow.rst
--rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/api-documentation.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-04-06 20:51:08.000000 geoglows-1.0.0rc5/docs/conf.py
--rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/dev-notes.rst
--rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/index.rst
--rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/license.rst
--rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc5/docs/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc5/environment.yaml
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.778258 geoglows-1.0.0rc5/geoglows/
--rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-07 23:46:20.000000 geoglows-1.0.0rc5/geoglows/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc5/geoglows/_constants.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.780064 geoglows-1.0.0rc5/geoglows/_plots/
--rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc5/geoglows/_plots/__init__.py
--rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc5/geoglows/_plots/format_tools.py
--rw-r--r--   0 rchales    (502) staff       (20)    16418 2024-04-07 22:21:17.000000 geoglows-1.0.0rc5/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 rchales    (502) staff       (20)    11334 2024-04-07 22:18:05.000000 geoglows-1.0.0rc5/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc5/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-07 22:21:17.000000 geoglows-1.0.0rc5/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc5/geoglows/_plots/plots.py
--rw-r--r--   0 rchales    (502) staff       (20)     7939 2024-04-07 22:18:05.000000 geoglows-1.0.0rc5/geoglows/analyze.py
--rw-r--r--   0 rchales    (502) staff       (20)     8241 2024-04-06 20:51:08.000000 geoglows-1.0.0rc5/geoglows/bias.py
--rw-r--r--   0 rchales    (502) staff       (20)    12872 2024-04-07 23:46:20.000000 geoglows-1.0.0rc5/geoglows/data.py
--rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc5/geoglows/streams.py
--rw-r--r--   0 rchales    (502) staff       (20)     3811 2024-04-07 22:18:05.000000 geoglows-1.0.0rc5/geoglows/tables.py
-drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-07 23:46:45.780437 geoglows-1.0.0rc5/geoglows.egg-info/
--rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-07 23:46:45.000000 geoglows-1.0.0rc5/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-07 23:46:45.000000 geoglows-1.0.0rc5/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-07 23:46:45.000000 geoglows-1.0.0rc5/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-07 23:46:45.000000 geoglows-1.0.0rc5/geoglows.egg-info/requires.txt
--rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-07 23:46:45.000000 geoglows-1.0.0rc5/geoglows.egg-info/top_level.txt
--rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc5/requirements.txt
--rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-07 23:46:45.781218 geoglows-1.0.0rc5/setup.cfg
--rw-r--r--   0 rchales    (502) staff       (20)     1650 2024-04-06 20:52:15.000000 geoglows-1.0.0rc5/setup.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.873415 geoglows-1.0.0rc6/
+-rw-r--r--   0 rchales    (502) staff       (20)       98 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/.gitignore
+-rw-r--r--   0 rchales    (502) staff       (20)      568 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/.readthedocs.yml
+-rw-r--r--   0 rchales    (502) staff       (20)     1519 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/LICENSE
+-rw-r--r--   0 rchales    (502) staff       (20)      173 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/MANIFEST.in
+-rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-09 04:56:33.873147 geoglows-1.0.0rc6/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      704 2024-04-06 20:53:01.000000 geoglows-1.0.0rc6/README.md
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.867459 geoglows-1.0.0rc6/docs/
+-rw-r--r--   0 rchales    (502) staff       (20)      634 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/Makefile
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.867624 geoglows-1.0.0rc6/docs/_static/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/_static/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.867737 geoglows-1.0.0rc6/docs/_templates/
+-rw-r--r--   0 rchales    (502) staff       (20)        0 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/_templates/.gitkeep
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.868438 geoglows-1.0.0rc6/docs/api-documentation/
+-rw-r--r--   0 rchales    (502) staff       (20)      321 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/analysis.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      210 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/bias.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      153 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/examples.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      687 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/plots.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1241 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation/streamflow.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      791 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/api-documentation.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1905 2024-04-06 20:51:08.000000 geoglows-1.0.0rc6/docs/conf.py
+-rw-r--r--   0 rchales    (502) staff       (20)      871 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/dev-notes.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     2028 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/index.rst
+-rw-r--r--   0 rchales    (502) staff       (20)     1536 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/license.rst
+-rw-r--r--   0 rchales    (502) staff       (20)      100 2024-03-29 16:38:01.000000 geoglows-1.0.0rc6/docs/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      243 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/environment.yaml
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.869939 geoglows-1.0.0rc6/geoglows/
+-rw-r--r--   0 rchales    (502) staff       (20)      418 2024-04-09 04:55:25.000000 geoglows-1.0.0rc6/geoglows/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      114 2024-04-06 15:20:56.000000 geoglows-1.0.0rc6/geoglows/_constants.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.872297 geoglows-1.0.0rc6/geoglows/_plots/
+-rw-r--r--   0 rchales    (502) staff       (20)       36 2024-03-29 16:40:36.000000 geoglows-1.0.0rc6/geoglows/_plots/__init__.py
+-rw-r--r--   0 rchales    (502) staff       (20)      814 2024-03-29 16:40:36.000000 geoglows-1.0.0rc6/geoglows/_plots/format_tools.py
+-rw-r--r--   0 rchales    (502) staff       (20)    16418 2024-04-07 22:21:17.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11334 2024-04-07 22:18:05.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 rchales    (502) staff       (20)     1678 2024-04-06 15:20:56.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 rchales    (502) staff       (20)    11477 2024-04-07 22:21:17.000000 geoglows-1.0.0rc6/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 rchales    (502) staff       (20)     6469 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/geoglows/_plots/plots.py
+-rw-r--r--   0 rchales    (502) staff       (20)     7939 2024-04-07 22:18:05.000000 geoglows-1.0.0rc6/geoglows/analyze.py
+-rw-r--r--   0 rchales    (502) staff       (20)     8241 2024-04-06 20:51:08.000000 geoglows-1.0.0rc6/geoglows/bias.py
+-rw-r--r--   0 rchales    (502) staff       (20)    12910 2024-04-09 04:54:37.000000 geoglows-1.0.0rc6/geoglows/data.py
+-rw-r--r--   0 rchales    (502) staff       (20)      801 2024-04-02 00:15:15.000000 geoglows-1.0.0rc6/geoglows/streams.py
+-rw-r--r--   0 rchales    (502) staff       (20)     3811 2024-04-07 22:18:05.000000 geoglows-1.0.0rc6/geoglows/tables.py
+drwxr-xr-x   0 rchales    (502) staff       (20)        0 2024-04-09 04:56:33.872892 geoglows-1.0.0rc6/geoglows.egg-info/
+-rw-r--r--   0 rchales    (502) staff       (20)     1854 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 rchales    (502) staff       (20)      981 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        1 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      109 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/requires.txt
+-rw-r--r--   0 rchales    (502) staff       (20)        9 2024-04-09 04:56:33.000000 geoglows-1.0.0rc6/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 rchales    (502) staff       (20)      108 2024-04-06 15:20:56.000000 geoglows-1.0.0rc6/requirements.txt
+-rw-r--r--   0 rchales    (502) staff       (20)       38 2024-04-09 04:56:33.873460 geoglows-1.0.0rc6/setup.cfg
+-rw-r--r--   0 rchales    (502) staff       (20)     1650 2024-04-06 20:52:15.000000 geoglows-1.0.0rc6/setup.py
```

### Comparing `geoglows-1.0.0rc5/.readthedocs.yml` & `geoglows-1.0.0rc6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/LICENSE` & `geoglows-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/PKG-INFO` & `geoglows-1.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.0rc5/README.md` & `geoglows-1.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/Makefile` & `geoglows-1.0.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/api-documentation/plots.rst` & `geoglows-1.0.0rc6/docs/api-documentation/plots.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/api-documentation/streamflow.rst` & `geoglows-1.0.0rc6/docs/api-documentation/streamflow.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/api-documentation.rst` & `geoglows-1.0.0rc6/docs/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/conf.py` & `geoglows-1.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/dev-notes.rst` & `geoglows-1.0.0rc6/docs/dev-notes.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/index.rst` & `geoglows-1.0.0rc6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/docs/license.rst` & `geoglows-1.0.0rc6/docs/license.rst`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/_plots/format_tools.py` & `geoglows-1.0.0rc6/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.0rc6/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.0rc6/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.0rc6/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.0rc6/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/_plots/plots.py` & `geoglows-1.0.0rc6/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/analyze.py` & `geoglows-1.0.0rc6/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/bias.py` & `geoglows-1.0.0rc6/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/data.py` & `geoglows-1.0.0rc6/geoglows/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,11 +341,11 @@
     if os.path.exists(METADATA_TABLE_LOCAL_PATH):
         return pd.read_parquet(METADATA_TABLE_LOCAL_PATH, columns=columns)
     warn = f"""
     Local copy of geoglows v2 metadata table not found. You should download a copy for optimal performance and 
     to make the data available when you are offline. A copy of the table will be cached at {METADATA_TABLE_LOCAL_PATH}.
     """
     warnings.warn(warn)
-    df = pd.read_parquet('s3://geoglows-v2/tables/package-metadata-table.parquet')
+    df = pd.read_parquet('https://geoglows-v2.s3-website-us-west-2.amazonaws.com/tables/package-metadata-table.parquet')
     os.makedirs(os.path.dirname(METADATA_TABLE_LOCAL_PATH), exist_ok=True)
     df.to_parquet(METADATA_TABLE_LOCAL_PATH)
     return df[columns] if columns else df
```

### Comparing `geoglows-1.0.0rc5/geoglows/streams.py` & `geoglows-1.0.0rc6/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows/tables.py` & `geoglows-1.0.0rc6/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.0rc6/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.0rc5/geoglows.egg-info/SOURCES.txt` & `geoglows-1.0.0rc6/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.0rc5/setup.py` & `geoglows-1.0.0rc6/setup.py`

 * *Files identical despite different names*

