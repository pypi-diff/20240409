# Comparing `tmp/phdu-2.3.5.tar.gz` & `tmp/phdu-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.3.5.tar", last modified: Tue Apr  9 08:32:19 2024, max compression
+gzip compressed data, was "phdu-2.3.6.tar", last modified: Tue Apr  9 08:36:25 2024, max compression
```

## Comparing `phdu-2.3.5.tar` & `phdu-2.3.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.119202 phdu-2.3.5/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.5/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:32:19.119202 phdu-2.3.5/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.5/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.055199 phdu-2.3.5/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.5/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/analysis.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.5/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.5/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/geometry.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.3.5/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.075200 phdu-2.3.5/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.5/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.5/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.5/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    22850 2024-04-09 08:31:09.000000 phdu-2.3.5/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.5/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.099201 phdu-2.3.5/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.5/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.5/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.5/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.5/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    32282 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.5/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.5/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.107202 phdu-2.3.5/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.5/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.5/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.5/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.115202 phdu-2.3.5/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.5/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.5/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.5/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.5/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:32:19.067200 phdu-2.3.5/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-04-09 08:32:18.000000 phdu-2.3.5/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-04-09 08:32:19.123203 phdu-2.3.5/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-04-09 08:32:01.000000 phdu-2.3.5/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.801432 phdu-2.3.6/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.6/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:36:25.801432 phdu-2.3.6/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.6/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.745429 phdu-2.3.6/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.6/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.6/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.6/phdu/analysis.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.6/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.6/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.6/phdu/geometry.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.6/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.3.6/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.765430 phdu-2.3.6/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.6/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.6/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.6/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    22854 2024-04-09 08:36:06.000000 phdu-2.3.6/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.6/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.781431 phdu-2.3.6/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.6/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.6/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.6/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.6/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32282 2024-04-05 11:52:28.000000 phdu-2.3.6/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.6/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.6/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.789431 phdu-2.3.6/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.6/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.6/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.6/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.797432 phdu-2.3.6/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.6/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.6/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.6/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.6/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-04-09 08:36:25.757429 phdu-2.3.6/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-04-09 08:36:25.000000 phdu-2.3.6/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-04-09 08:36:25.000000 phdu-2.3.6/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-04-09 08:36:25.000000 phdu-2.3.6/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-04-09 08:36:25.000000 phdu-2.3.6/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-04-09 08:36:25.000000 phdu-2.3.6/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-04-09 08:36:25.805432 phdu-2.3.6/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-04-09 08:36:14.000000 phdu-2.3.6/setup.py
```

### Comparing `phdu-2.3.5/LICENSE.md` & `phdu-2.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/PKG-INFO` & `phdu-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.5
+Version: 2.3.6
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.5/README.md` & `phdu-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/__init__.py` & `phdu-2.3.6/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/_helper.py` & `phdu-2.3.6/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/analysis.py` & `phdu-2.3.6/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/clustering.py` & `phdu-2.3.6/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/decomposition.py` & `phdu-2.3.6/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/geometry.py` & `phdu-2.3.6/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/np_utils.py` & `phdu-2.3.6/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/pd_utils.py` & `phdu-2.3.6/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/plots/base.py` & `phdu-2.3.6/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/plots/plotly_utils.py` & `phdu-2.3.6/phdu/plots/plotly_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,8 +453,8 @@
         y=np.hstack([CI[:, 0], CI[:, 1][::-1]]), # upper CI, then lower CI reversed
         fill='toself',
         fillcolor=color,
         line=dict(color=color, width=0),
         opacity=opacity,
         showlegend=False,
     ))
-    return
+    return fig
```

### Comparing `phdu-2.3.5/phdu/script_fmt.py` & `phdu-2.3.6/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/_integration.py` & `phdu-2.3.6/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/_plots.py` & `phdu-2.3.6/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/bootstrap.py` & `phdu-2.3.6/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/conf_interval.py` & `phdu-2.3.6/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/corr.py` & `phdu-2.3.6/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/rtopy/_helper.py` & `phdu-2.3.6/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/rtopy/resample.py` & `phdu-2.3.6/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/stats/test/permutation.py` & `phdu-2.3.6/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu/storage.py` & `phdu-2.3.6/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/phdu.egg-info/PKG-INFO` & `phdu-2.3.6/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.5
+Version: 2.3.6
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.5/phdu.egg-info/SOURCES.txt` & `phdu-2.3.6/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.3.5/setup.py` & `phdu-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.3.5',
+    version='2.3.6',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

