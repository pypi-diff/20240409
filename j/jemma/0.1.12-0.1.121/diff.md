# Comparing `tmp/jemma-0.1.12.tar.gz` & `tmp/jemma-0.1.121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.12.tar", last modified: Tue Apr  9 05:19:00 2024, max compression
+gzip compressed data, was "jemma-0.1.121.tar", last modified: Tue Apr  9 05:27:15 2024, max compression
```

## Comparing `jemma-0.1.12.tar` & `jemma-0.1.121.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:19:00.451711 jemma-0.1.12/
--rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:19:00.451261 jemma-0.1.12/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.12/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:19:00.446487 jemma-0.1.12/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      268 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       46 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        8 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:19:00.451861 jemma-0.1.12/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 05:18:52.000000 jemma-0.1.12/setup.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:19:00.450518 jemma-0.1.12/simmons/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.12/simmons/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2252 2024-04-09 00:53:24.000000 jemma-0.1.12/simmons/huddle.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5267 2024-04-09 03:45:46.000000 jemma-0.1.12/simmons/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.12/simmons/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:27:15.262175 jemma-0.1.121/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:27:15.261785 jemma-0.1.121/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.121/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:27:15.257828 jemma-0.1.121/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.121/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2253 2024-04-09 05:23:04.000000 jemma-0.1.121/jemma/huddle.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5267 2024-04-09 03:45:46.000000 jemma-0.1.121/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.121/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:27:15.261253 jemma-0.1.121/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:27:15.000000 jemma-0.1.121/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      260 2024-04-09 05:27:15.000000 jemma-0.1.121/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:27:15.000000 jemma-0.1.121/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 05:27:15.000000 jemma-0.1.121/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:27:15.000000 jemma-0.1.121/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 05:27:15.000000 jemma-0.1.121/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:27:15.262312 jemma-0.1.121/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-09 05:26:51.000000 jemma-0.1.121/setup.py
```

### Comparing `jemma-0.1.12/README.md` & `jemma-0.1.121/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.12/simmons/huddle.py` & `jemma-0.1.121/jemma/huddle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 from dotenv import load_dotenv
 
-from tools import parse_cli_arguments
+from .tools import parse_cli_arguments
 from requirements.feature import Feature
 from team.business_owner import BusinessOwner
 from team.engineer import Engineer
 from team.tester import Tester
 from team.project_manager import ProjectManager
 import work.flow as flow
```

### Comparing `jemma-0.1.12/simmons/thinker.py` & `jemma-0.1.121/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.12/simmons/tools.py` & `jemma-0.1.121/jemma/tools.py`

 * *Files identical despite different names*

