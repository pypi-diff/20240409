# Comparing `tmp/jemma-0.1.122.tar.gz` & `tmp/jemma-0.1.123.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.122.tar", last modified: Tue Apr  9 05:30:34 2024, max compression
+gzip compressed data, was "jemma-0.1.123.tar", last modified: Tue Apr  9 05:33:51 2024, max compression
```

## Comparing `jemma-0.1.122.tar` & `jemma-0.1.123.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.730668 jemma-0.1.122/
--rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:30:34.730264 jemma-0.1.122/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.122/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.708510 jemma-0.1.122/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.122/jemma/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2253 2024-04-09 05:23:04.000000 jemma-0.1.122/jemma/huddle.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.713343 jemma-0.1.122/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.122/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.714779 jemma-0.1.122/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.122/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.122/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.718364 jemma-0.1.122/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.122/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.122/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 02:59:54.000000 jemma-0.1.122/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.720564 jemma-0.1.122/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.122/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-05 19:35:32.000000 jemma-0.1.122/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.722594 jemma-0.1.122/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.122/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.122/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.727466 jemma-0.1.122/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.122/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4018 2024-04-09 04:40:37.000000 jemma-0.1.122/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4871 2024-04-09 03:17:03.000000 jemma-0.1.122/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6866 2024-04-09 03:41:44.000000 jemma-0.1.122/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1594 2024-04-05 20:08:50.000000 jemma-0.1.122/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5267 2024-04-09 03:45:46.000000 jemma-0.1.122/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.122/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.729638 jemma-0.1.122/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.122/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2692 2024-04-09 02:55:57.000000 jemma-0.1.122/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:30:34.712519 jemma-0.1.122/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:30:34.000000 jemma-0.1.122/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-09 05:30:34.000000 jemma-0.1.122/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:30:34.000000 jemma-0.1.122/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 05:30:34.000000 jemma-0.1.122/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:30:34.000000 jemma-0.1.122/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 05:30:34.000000 jemma-0.1.122/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:30:34.730807 jemma-0.1.122/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-09 05:30:21.000000 jemma-0.1.122/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.561513 jemma-0.1.123/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:33:51.560961 jemma-0.1.123/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.123/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.536487 jemma-0.1.123/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.123/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2252 2024-04-09 05:33:36.000000 jemma-0.1.123/jemma/huddle.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.543489 jemma-0.1.123/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.123/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.545764 jemma-0.1.123/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.123/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.123/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.548923 jemma-0.1.123/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.123/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.123/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 02:59:54.000000 jemma-0.1.123/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.551473 jemma-0.1.123/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.123/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-05 19:35:32.000000 jemma-0.1.123/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.553747 jemma-0.1.123/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.123/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.123/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.558462 jemma-0.1.123/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.123/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4018 2024-04-09 04:40:37.000000 jemma-0.1.123/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4871 2024-04-09 03:17:03.000000 jemma-0.1.123/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6866 2024-04-09 03:41:44.000000 jemma-0.1.123/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1594 2024-04-05 20:08:50.000000 jemma-0.1.123/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5267 2024-04-09 03:45:46.000000 jemma-0.1.123/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.123/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.560135 jemma-0.1.123/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.123/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2692 2024-04-09 02:55:57.000000 jemma-0.1.123/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:33:51.542050 jemma-0.1.123/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:33:51.000000 jemma-0.1.123/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-09 05:33:51.000000 jemma-0.1.123/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:33:51.000000 jemma-0.1.123/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 05:33:51.000000 jemma-0.1.123/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:33:51.000000 jemma-0.1.123/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 05:33:51.000000 jemma-0.1.123/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:33:51.561651 jemma-0.1.123/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-09 05:33:42.000000 jemma-0.1.123/setup.py
```

### Comparing `jemma-0.1.122/README.md` & `jemma-0.1.123/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/huddle.py` & `jemma-0.1.123/jemma/huddle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 from dotenv import load_dotenv
 
-from .tools import parse_cli_arguments
+from tools import parse_cli_arguments
 from requirements.feature import Feature
 from team.business_owner import BusinessOwner
 from team.engineer import Engineer
 from team.tester import Tester
 from team.project_manager import ProjectManager
 import work.flow as flow
```

### Comparing `jemma-0.1.122/jemma/prompt/business/owner.py` & `jemma-0.1.123/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/prompt/engineer/clarify.py` & `jemma-0.1.123/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/prompt/engineer/code.py` & `jemma-0.1.123/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/prompt/tester/test.py` & `jemma-0.1.123/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/requirements/feature.py` & `jemma-0.1.123/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/team/business_owner.py` & `jemma-0.1.123/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/team/engineer.py` & `jemma-0.1.123/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/team/project_manager.py` & `jemma-0.1.123/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/team/tester.py` & `jemma-0.1.123/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/thinker.py` & `jemma-0.1.123/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/tools.py` & `jemma-0.1.123/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma/work/flow.py` & `jemma-0.1.123/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.122/jemma.egg-info/SOURCES.txt` & `jemma-0.1.123/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

