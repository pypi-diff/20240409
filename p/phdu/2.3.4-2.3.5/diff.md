# Comparing `tmp/phdu-2.3.4.tar.gz` & `tmp/phdu-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.3.4.tar", last modified: Sun Apr  7 07:28:29 2024, max compression
+gzip compressed data, was "phdu-2.3.5.tar", last modified: Tue Apr  9 08:32:19 2024, max compression
```

## Comparing `phdu-2.3.4.tar` & `phdu-2.3.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.312986 phdu-2.3.4/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-07-31 18:53:26.000000 phdu-2.3.4/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2024-04-07 07:28:29.312986 phdu-2.3.4/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-07-31 18:53:26.000000 phdu-2.3.4/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.309653 phdu-2.3.4/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      590 2024-02-24 02:21:10.000000 phdu-2.3.4/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1948 2023-09-21 17:52:42.000000 phdu-2.3.4/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2484 2024-02-04 05:18:27.000000 phdu-2.3.4/phdu/analysis.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3664 2023-10-17 21:07:41.000000 phdu-2.3.4/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1333 2023-12-05 04:36:26.000000 phdu-2.3.4/phdu/geometry.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3183 2024-01-23 06:00:25.000000 phdu-2.3.4/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     6214 2024-04-07 07:28:04.000000 phdu-2.3.4/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.312986 phdu-2.3.4/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4011 2023-12-05 02:04:31.000000 phdu-2.3.4/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    22497 2024-04-07 07:01:10.000000 phdu-2.3.4/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.312986 phdu-2.3.4/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    32282 2024-01-18 07:19:52.000000 phdu-2.3.4/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.312986 phdu-2.3.4/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.312986 phdu-2.3.4/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-07-31 18:53:27.000000 phdu-2.3.4/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4437 2024-02-24 02:19:42.000000 phdu-2.3.4/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-07 07:28:29.312986 phdu-2.3.4/phdu.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2864 2024-04-07 07:28:29.000000 phdu-2.3.4/phdu.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      786 2024-04-07 07:28:29.000000 phdu-2.3.4/phdu.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-07 07:28:29.000000 phdu-2.3.4/phdu.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2024-04-07 07:28:29.000000 phdu-2.3.4/phdu.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        5 2024-04-07 07:28:29.000000 phdu-2.3.4/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2024-04-07 07:28:29.312986 phdu-2.3.4/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1659 2024-04-07 07:28:14.000000 phdu-2.3.4/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.119202 phdu-2.3.5/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.5/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:32:19.119202 phdu-2.3.5/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.5/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.055199 phdu-2.3.5/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.5/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/analysis.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.5/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.5/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/geometry.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.3.5/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.075200 phdu-2.3.5/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.5/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.5/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.5/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    22850 2024-04-09 08:31:09.000000 phdu-2.3.5/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.5/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.099201 phdu-2.3.5/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.5/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.5/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.5/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.5/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32282 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.5/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.5/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.107202 phdu-2.3.5/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.5/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.5/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.5/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.115202 phdu-2.3.5/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.5/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.5/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.5/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.067200 phdu-2.3.5/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-04-09 08:32:19.123203 phdu-2.3.5/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-04-09 08:32:01.000000 phdu-2.3.5/setup.py
```

### Comparing `phdu-2.3.4/LICENSE.md` & `phdu-2.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/PKG-INFO` & `phdu-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.4
+Version: 2.3.5
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.4/README.md` & `phdu-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/__init__.py` & `phdu-2.3.5/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/_helper.py` & `phdu-2.3.5/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/analysis.py` & `phdu-2.3.5/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/clustering.py` & `phdu-2.3.5/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/decomposition.py` & `phdu-2.3.5/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/geometry.py` & `phdu-2.3.5/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/np_utils.py` & `phdu-2.3.5/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/pd_utils.py` & `phdu-2.3.5/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/plots/base.py` & `phdu-2.3.5/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/plots/plotly_utils.py` & `phdu-2.3.5/phdu/plots/plotly_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,36 +418,43 @@
     from IPython.display import HTML
     if isinstance(cs[0], list):
         _, c = zip(*cs)
     else:
         c = cs
     return HTML(cl.to_html(cl.to_hsl(c)))
 
-def plot_confidence_bands(fig, x, y, CI, label=None, color='#1f77b4', lw=6, opacity=0.3, **kwargs):
+def plot_confidence_bands(*, fig=None, df=None, x=None, y=None, CI=None, label=None, color='#1f77b4', lw=6, opacity=0.3, **fig_kwargs):
     """
     Plots a curve with confidence intervals as bands.
 
     Parameters:
-    - fig: The figure object to which the traces will be added.
+    - fig: The figure object to which the traces will be added. If None, a new figure will be created with specs from fig_kwargs.
+    - df: (Optional) The DataFrame containing the data to be plotted. Must contain columns 'sample_stat' and 'CI', and the index will be used as the x-coordinates.
     - x: The x-coordinates of the data points.
     - y: The y-coordinates of the data points (mean values).
     - CI: 2D array of confidence interval data, where CI[:, 0] is the lower bound and CI[:, 1] is the upper bound.
     - color: (Optional) The color of the plot. Default is blue.
     - lw: (Optional) The line width of the plot. Default is 6.
     - opacity: (Optional) The opacity of the confidence interval band. Default is 0.3.
-    - kwargs: (Optional) Additional keyword arguments to be passed to the plotly go.Scatter function, both for the mean curve and the confidence interval band.
+    - fig_kwargs: (Optional) Additional keyword arguments to be passed to the get_figure function.
     """
+    if fig is None:
+        fig = get_figure(**fig_kwargs)
+    if df is not None:
+        x = df.index
+        y = df.sample_stat.values
+        CI = np.vstack(df.CI.values)
+
     # Plot the main line (mean curve)
-    fig.add_trace(go.Scatter(x=x, y=y, line=dict(width=lw, color=color), name=label, showlegend=label is not None, **kwargs))
+    fig.add_trace(go.Scatter(x=x, y=y, line=dict(width=lw, color=color), name=label, showlegend=label is not None))
 
     # Plot the confidence interval as a band
     fig.add_trace(go.Scatter(
         x=np.hstack([x, x[::-1]]), # x, then x reversed
         y=np.hstack([CI[:, 0], CI[:, 1][::-1]]), # upper CI, then lower CI reversed
         fill='toself',
         fillcolor=color,
         line=dict(color=color, width=0),
         opacity=opacity,
         showlegend=False,
-        **kwargs
     ))
     return
```

### Comparing `phdu-2.3.4/phdu/script_fmt.py` & `phdu-2.3.5/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/_integration.py` & `phdu-2.3.5/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/_plots.py` & `phdu-2.3.5/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/bootstrap.py` & `phdu-2.3.5/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/conf_interval.py` & `phdu-2.3.5/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/corr.py` & `phdu-2.3.5/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/rtopy/_helper.py` & `phdu-2.3.5/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/rtopy/resample.py` & `phdu-2.3.5/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/stats/test/permutation.py` & `phdu-2.3.5/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu/storage.py` & `phdu-2.3.5/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/phdu.egg-info/PKG-INFO` & `phdu-2.3.5/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.4
+Version: 2.3.5
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.4/phdu.egg-info/SOURCES.txt` & `phdu-2.3.5/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.3.4/setup.py` & `phdu-2.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.3.4',
+    version='2.3.5',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

