# Comparing `tmp/honeybee-display-0.3.6.tar.gz` & `tmp/honeybee-display-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-display-0.3.6.tar", last modified: Wed Mar 20 17:03:35 2024, max compression
+gzip compressed data, was "dist/honeybee-display-0.3.7.tar", last modified: Tue Apr  9 20:33:53 2024, max compression
```

## Comparing `honeybee-display-0.3.6.tar` & `honeybee-display-0.3.7.tar`

### file list

```diff
@@ -1,70 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/honeybee_display/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/aperture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/attr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/honeybee_display/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/colorobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/door.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/honeybee_display/energy/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/energy/colorobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/face.py
--rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/honeybee_display/radiance/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/shade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/honeybee_display/shademesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/honeybee_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/honeybee_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/honeybee_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/honeybee_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/honeybee_display.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/honeybee_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-20 17:03:34.000000 honeybee-display-0.3.6/honeybee_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/aperture_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/door_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/face_extend_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 17:03:35.000000 honeybee-display-0.3.6/tests/json/
--rw-r--r--   0 runner    (1001) docker     (127)   102631 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/json/single_family_home.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/model_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/room_extend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 17:02:31.000000 honeybee-display-0.3.6/tests/shade_extend_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/attr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/colorobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/door.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/energy/colorobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display/radiance/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/shade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/honeybee_display/shademesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/honeybee_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 20:33:53.000000 honeybee-display-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-09 20:32:49.000000 honeybee-display-0.3.7/setup.py
```

### Comparing `honeybee-display-0.3.6/LICENSE` & `honeybee-display-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/PKG-INFO` & `honeybee-display-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-display
-Version: 0.3.6
+Version: 0.3.7
 Summary: Adds methods to translate honeybee objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/honeybee-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-display-0.3.6/README.md` & `honeybee-display-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/dev-requirements.txt` & `honeybee-display-0.3.7/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/_extend_honeybee.py` & `honeybee-display-0.3.7/honeybee_display/_extend_honeybee.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/aperture.py` & `honeybee-display-0.3.7/honeybee_display/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/attr.py` & `honeybee-display-0.3.7/honeybee_display/attr.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/cli/__init__.py` & `honeybee-display-0.3.7/honeybee_display/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/colorobj.py` & `honeybee-display-0.3.7/honeybee_display/colorobj.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/door.py` & `honeybee-display-0.3.7/honeybee_display/door.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/energy/colorobj.py` & `honeybee-display-0.3.7/honeybee_display/energy/colorobj.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/face.py` & `honeybee-display-0.3.7/honeybee_display/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/model.py` & `honeybee-display-0.3.7/honeybee_display/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import json
 
 from ladybug_geometry.geometry3d import Point3D, Face3D
 from ladybug.datatype.generic import GenericType
 from ladybug.color import Color
 from ladybug_display.geometry3d import DisplayPoint3D, DisplayLineSegment3D, \
-    DisplayFace3D, DisplayMesh3D
+    DisplayPolyline3D, DisplayFace3D, DisplayMesh3D
 from ladybug_display.visualization import VisualizationSet, ContextGeometry, \
     AnalysisGeometry, VisualizationData, VisualizationMetaData
 from honeybee.boundarycondition import Outdoors, Ground, Surface
 from honeybee.facetype import Wall, RoofCeiling, Floor, AirBoundary
 from honeybee.colorobj import ColorRoom, ColorFace
 from honeybee.shade import Shade
 from honeybee.typing import clean_string
@@ -456,18 +456,14 @@
     for dr in model._orphaned_doors:
         _process_wireframe(dr.geometry, wireframe)
     for shd in model.indoor_shades:
         _process_wireframe(shd.geometry, wireframe)
     for shd in model.outdoor_shades:
         lw = 2 if shd.is_detached else 1
         _process_wireframe(shd.geometry, wireframe, lw)
-    for shd_m in model.shade_meshes:
-        lw = 2 if shd_m.is_detached else 1
-        for seg in shd_m.geometry.edges:
-            wireframe.append(DisplayLineSegment3D(seg, line_width=lw))
 
     # build the VisualizationSet and return it
     if len(wireframe) == 0:
         return None
     vis_set = VisualizationSet(
         model.identifier, [ContextGeometry('Wireframe', wireframe)])
     vis_set.display_name = model.display_name
```

### Comparing `honeybee-display-0.3.6/honeybee_display/room.py` & `honeybee-display-0.3.7/honeybee_display/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/shade.py` & `honeybee-display-0.3.7/honeybee_display/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display/shademesh.py` & `honeybee-display-0.3.7/honeybee_display/shademesh.py`

 * *Files identical despite different names*

### Comparing `honeybee-display-0.3.6/honeybee_display.egg-info/PKG-INFO` & `honeybee-display-0.3.7/honeybee_display.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-display
-Version: 0.3.6
+Version: 0.3.7
 Summary: Adds methods to translate honeybee objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/honeybee-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-display-0.3.6/setup.py` & `honeybee-display-0.3.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     author="Ladybug Tools",
     author_email="info@ladybug.tools",
     description="Adds methods to translate honeybee objects to VisualizationSets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ladybug-tools/honeybee-display",
     packages=setuptools.find_packages(exclude=["tests*"]),
+    include_package_data=True,
     install_requires=requirements,
     extras_require={'full': extras_requirements},
     entry_points={
         "console_scripts": ["honeybee-display = honeybee_display.cli:display"]
     },
     classifiers=[
         "Programming Language :: Python :: 2.7",
```

