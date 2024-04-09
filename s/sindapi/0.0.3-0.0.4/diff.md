# Comparing `tmp/sindapi-0.0.3.tar.gz` & `tmp/sindapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sindapi-0.0.3.tar", last modified: Tue Apr  9 09:36:22 2024, max compression
+gzip compressed data, was "sindapi-0.0.4.tar", last modified: Tue Apr  9 09:59:45 2024, max compression
```

## Comparing `sindapi-0.0.3.tar` & `sindapi-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.493313 sindapi-0.0.3/
--rw-rw-rw-   0        0        0      334 2024-04-09 09:36:22.492312 sindapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-09 09:36:22.493313 sindapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      440 2024-04-09 09:36:14.000000 sindapi-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.460695 sindapi-0.0.3/sindapi/
--rw-rw-rw-   0        0        0       23 2024-04-09 09:30:38.000000 sindapi-0.0.3/sindapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.484305 sindapi-0.0.3/sindapi/sindmap/
--rw-rw-rw-   0        0        0       23 2024-04-09 09:30:53.000000 sindapi-0.0.3/sindapi/sindmap/__init__.py
--rw-rw-rw-   0        0        0      196 2024-04-09 09:03:10.000000 sindapi-0.0.3/sindapi/sindmap/drivable_area.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.485306 sindapi-0.0.3/sindapi/sindmap/intersection/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.3/sindapi/sindmap/intersection/__init__.py
--rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.3/sindapi/sindmap/intersection/intersection.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.487306 sindapi-0.0.3/sindapi/sindmap/lane/
--rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.3/sindapi/sindmap/lane/__init__.py
--rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.3/sindapi/sindmap/lane/lane_segment.py
--rw-rw-rw-   0        0        0     4334 2024-04-09 09:08:10.000000 sindapi-0.0.3/sindapi/sindmap/map_api.py
--rw-rw-rw-   0        0        0     1481 2024-04-09 09:03:17.000000 sindapi-0.0.3/sindapi/sindmap/pedestrian_crossing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.488305 sindapi-0.0.3/sindapi/sindmap/stretch/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.3/sindapi/sindmap/stretch/__init__.py
--rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.3/sindapi/sindmap/stretch/stretch.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.491313 sindapi-0.0.3/sindapi/sindmap/utils/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.3/sindapi/sindmap/utils/__init__.py
--rw-rw-rw-   0        0        0     1948 2024-04-07 10:30:37.000000 sindapi-0.0.3/sindapi/sindmap/utils/map_primitives.py
--rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.3/sindapi/sindmap/utils/typing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:36:22.480316 sindapi-0.0.3/sindapi.egg-info/
--rw-rw-rw-   0        0        0      334 2024-04-09 09:36:22.000000 sindapi-0.0.3/sindapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-09 09:36:22.000000 sindapi-0.0.3/sindapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 09:36:22.000000 sindapi-0.0.3/sindapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-09 09:36:22.000000 sindapi-0.0.3/sindapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 09:36:22.000000 sindapi-0.0.3/sindapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.067350 sindapi-0.0.4/
+-rw-rw-rw-   0        0        0      334 2024-04-09 09:59:45.066350 sindapi-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-09 09:59:45.067350 sindapi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      440 2024-04-09 09:59:19.000000 sindapi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.042678 sindapi-0.0.4/sindapi/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.4/sindapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.058335 sindapi-0.0.4/sindapi/sindmap/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.4/sindapi/sindmap/__init__.py
+-rw-rw-rw-   0        0        0      196 2024-04-09 09:03:10.000000 sindapi-0.0.4/sindapi/sindmap/drivable_area.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.059334 sindapi-0.0.4/sindapi/sindmap/intersection/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.4/sindapi/sindmap/intersection/__init__.py
+-rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.4/sindapi/sindmap/intersection/intersection.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.061410 sindapi-0.0.4/sindapi/sindmap/lane/
+-rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.4/sindapi/sindmap/lane/__init__.py
+-rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.4/sindapi/sindmap/lane/lane_segment.py
+-rw-rw-rw-   0        0        0     4309 2024-04-09 09:59:09.000000 sindapi-0.0.4/sindapi/sindmap/map_api.py
+-rw-rw-rw-   0        0        0     1481 2024-04-09 09:03:17.000000 sindapi-0.0.4/sindapi/sindmap/pedestrian_crossing.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.063408 sindapi-0.0.4/sindapi/sindmap/stretch/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.4/sindapi/sindmap/stretch/__init__.py
+-rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.4/sindapi/sindmap/stretch/stretch.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.065342 sindapi-0.0.4/sindapi/sindmap/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.4/sindapi/sindmap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1948 2024-04-07 10:30:37.000000 sindapi-0.0.4/sindapi/sindmap/utils/map_primitives.py
+-rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.4/sindapi/sindmap/utils/typing.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:59:45.055399 sindapi-0.0.4/sindapi.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-04-09 09:59:44.000000 sindapi-0.0.4/sindapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-09 09:59:45.000000 sindapi-0.0.4/sindapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 09:59:44.000000 sindapi-0.0.4/sindapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-09 09:59:44.000000 sindapi-0.0.4/sindapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 09:59:44.000000 sindapi-0.0.4/sindapi.egg-info/top_level.txt
```

### Comparing `sindapi-0.0.3/sindapi/sindmap/intersection/intersection.py` & `sindapi-0.0.4/sindapi/sindmap/intersection/intersection.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.3/sindapi/sindmap/lane/lane_segment.py` & `sindapi-0.0.4/sindapi/sindmap/lane/lane_segment.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.3/sindapi/sindmap/map_api.py` & `sindapi-0.0.4/sindapi/sindmap/map_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-__package__ = "sindmap"
-
 import json
 import yaml
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, List, Optional
 
+
 from .drivable_area import DrivableArea
 from .pedestrian_crossing import PedestrianCrossing
 from .stretch.stretch import Stretch
 from .intersection.intersection import Intersection
 from .lane.lane_segment import Lane, LaneSegment
```

### Comparing `sindapi-0.0.3/sindapi/sindmap/pedestrian_crossing.py` & `sindapi-0.0.4/sindapi/sindmap/pedestrian_crossing.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.3/sindapi/sindmap/stretch/stretch.py` & `sindapi-0.0.4/sindapi/sindmap/stretch/stretch.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.3/sindapi/sindmap/utils/map_primitives.py` & `sindapi-0.0.4/sindapi/sindmap/utils/map_primitives.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.3/sindapi.egg-info/SOURCES.txt` & `sindapi-0.0.4/sindapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

