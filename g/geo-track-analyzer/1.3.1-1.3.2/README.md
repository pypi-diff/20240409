# Comparing `tmp/geo_track_analyzer-1.3.1.tar.gz` & `tmp/geo_track_analyzer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_track_analyzer-1.3.1.tar", max compression
+gzip compressed data, was "geo_track_analyzer-1.3.2.tar", max compression
```

## Comparing `geo_track_analyzer-1.3.1.tar` & `geo_track_analyzer-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1076 2024-03-02 10:49:20.945082 geo_track_analyzer-1.3.1/LICENSE
--rw-r--r--   0        0        0     3492 2024-03-02 10:49:20.945082 geo_track_analyzer-1.3.1/README.md
--rw-r--r--   0        0        0      593 2024-03-02 10:49:20.945082 geo_track_analyzer-1.3.1/geo_track_analyzer/__init__.py
--rw-r--r--   0        0        0      778 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/cli/__init__.py
--rw-r--r--   0        0        0      859 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/cli/_extract_track.py
--rw-r--r--   0        0        0     4500 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/cli/_update_elevation.py
--rw-r--r--   0        0        0    16054 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/compare.py
--rw-r--r--   0        0        0     7774 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/enhancer.py
--rw-r--r--   0        0        0      462 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/exceptions.py
--rw-r--r--   0        0        0     4994 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/model.py
--rw-r--r--   0        0        0    14046 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/processing.py
--rw-r--r--   0        0        0    39346 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/track.py
--rw-r--r--   0        0        0        0 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/utils/__init__.py
--rw-r--r--   0        0        0    22327 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/utils/base.py
--rw-r--r--   0        0        0     5449 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/utils/internal.py
--rw-r--r--   0        0        0     4034 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/utils/track.py
--rw-r--r--   0        0        0      433 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/__init__.py
--rw-r--r--   0        0        0      352 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/constants.py
--rw-r--r--   0        0        0      441 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/interactive.py
--rw-r--r--   0        0        0    13262 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/map.py
--rw-r--r--   0        0        0    13666 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/profiles.py
--rw-r--r--   0        0        0     2160 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/utils.py
--rw-r--r--   0        0        0     2775 2024-03-02 10:49:20.949082 geo_track_analyzer-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4859 1970-01-01 00:00:00.000000 geo_track_analyzer-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-09 19:22:31.650846 geo_track_analyzer-1.3.2/LICENSE
+-rw-r--r--   0        0        0     3492 2024-04-09 19:22:31.650846 geo_track_analyzer-1.3.2/README.md
+-rw-r--r--   0        0        0      593 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/__init__.py
+-rw-r--r--   0        0        0      778 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/cli/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_extract_track.py
+-rw-r--r--   0        0        0     4500 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_update_elevation.py
+-rw-r--r--   0        0        0    16054 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/compare.py
+-rw-r--r--   0        0        0     7774 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/enhancer.py
+-rw-r--r--   0        0        0      462 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/exceptions.py
+-rw-r--r--   0        0        0     4994 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/model.py
+-rw-r--r--   0        0        0    14046 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/processing.py
+-rw-r--r--   0        0        0    39346 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/track.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/__init__.py
+-rw-r--r--   0        0        0    22327 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/base.py
+-rw-r--r--   0        0        0     5449 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/internal.py
+-rw-r--r--   0        0        0     4034 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/utils/track.py
+-rw-r--r--   0        0        0      433 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/__init__.py
+-rw-r--r--   0        0        0      352 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/constants.py
+-rw-r--r--   0        0        0      441 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/interactive.py
+-rw-r--r--   0        0        0    13262 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/map.py
+-rw-r--r--   0        0        0    13665 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/profiles.py
+-rw-r--r--   0        0        0     2160 2024-04-09 19:22:31.654846 geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/utils.py
+-rw-r--r--   0        0        0     2775 2024-04-09 19:22:31.658846 geo_track_analyzer-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4859 1970-01-01 00:00:00.000000 geo_track_analyzer-1.3.2/PKG-INFO
```

### Comparing `geo_track_analyzer-1.3.1/LICENSE` & `geo_track_analyzer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/README.md` & `geo_track_analyzer-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/__init__.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/cli/__init__.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/cli/_extract_track.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_extract_track.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/cli/_update_elevation.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/cli/_update_elevation.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/compare.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/compare.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/enhancer.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/enhancer.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/model.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/model.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/processing.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/processing.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/track.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/track.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/utils/base.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/utils/base.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/utils/internal.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/utils/internal.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/utils/track.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/utils/track.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/map.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/map.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/profiles.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         border_x = data.loc[segment_border_idx].cum_distance_moving
         fig.add_vline(
             x=border_x,
             # Hide line but keep abbitiation for first segment
             line_width=3 if idx > 0 else 0,
             line_dash="dash",
             line_color="darkslategray" if color is None else color,
-            annotation_text=f"Segment {data.iloc[segment_border_idx].segment}",
+            annotation_text=f"Segment {data.loc[segment_border_idx].segment}",
             annotation_borderpad=5,
         )
 
 
 def plot_track_2d(
     data: pd.DataFrame,
     *,
```

### Comparing `geo_track_analyzer-1.3.1/geo_track_analyzer/visualize/utils.py` & `geo_track_analyzer-1.3.2/geo_track_analyzer/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `geo_track_analyzer-1.3.1/pyproject.toml` & `geo_track_analyzer-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geo-track-analyzer"
-version = "1.3.1"
+version = "1.3.2"
 description = "Analyze geospacial data tracks"
 authors = ["Korbinian Schweiger <korbinian.schweiger@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Visualization",
 ]
```

### Comparing `geo_track_analyzer-1.3.1/PKG-INFO` & `geo_track_analyzer-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-track-analyzer
-Version: 1.3.1
+Version: 1.3.2
 Summary: Analyze geospacial data tracks
 Home-page: https://github.com/kschweiger/track_analyzer
 License: MIT
 Keywords: fit,gpx,visualization,analysis
 Author: Korbinian Schweiger
 Author-email: korbinian.schweiger@gmail.com
 Requires-Python: >=3.10,<3.13
```

