# Comparing `tmp/jemma-0.1.125.tar.gz` & `tmp/jemma-0.1.126.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.125.tar", last modified: Tue Apr  9 05:46:32 2024, max compression
+gzip compressed data, was "jemma-0.1.126.tar", last modified: Tue Apr  9 05:48:30 2024, max compression
```

## Comparing `jemma-0.1.125.tar` & `jemma-0.1.126.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.911827 jemma-0.1.125/
--rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:46:32.911193 jemma-0.1.125/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.125/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.886434 jemma-0.1.125/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.125/jemma/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2300 2024-04-09 05:46:09.000000 jemma-0.1.125/jemma/huddle.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.893488 jemma-0.1.125/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.125/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.895346 jemma-0.1.125/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.125/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.125/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.898594 jemma-0.1.125/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.125/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.125/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 02:59:54.000000 jemma-0.1.125/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.900553 jemma-0.1.125/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.125/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.125/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.902487 jemma-0.1.125/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.125/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.125/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.907890 jemma-0.1.125/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.125/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.125/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.125/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.125/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.125/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5273 2024-04-09 05:46:20.000000 jemma-0.1.125/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.125/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.910078 jemma-0.1.125/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.125/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.125/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:46:32.892412 jemma-0.1.125/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:46:32.000000 jemma-0.1.125/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-09 05:46:32.000000 jemma-0.1.125/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:46:32.000000 jemma-0.1.125/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 05:46:32.000000 jemma-0.1.125/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:46:32.000000 jemma-0.1.125/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 05:46:32.000000 jemma-0.1.125/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:46:32.912024 jemma-0.1.125/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-09 05:46:27.000000 jemma-0.1.125/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.183342 jemma-0.1.126/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:48:30.182615 jemma-0.1.126/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.126/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.156165 jemma-0.1.126/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.126/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2311 2024-04-09 05:47:27.000000 jemma-0.1.126/jemma/huddle.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.162610 jemma-0.1.126/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.126/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.164759 jemma-0.1.126/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.126/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.126/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.168493 jemma-0.1.126/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.126/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.126/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 02:59:54.000000 jemma-0.1.126/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.170814 jemma-0.1.126/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.126/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.126/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.172858 jemma-0.1.126/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.126/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.126/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.178660 jemma-0.1.126/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.126/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.126/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.126/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.126/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.126/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5273 2024-04-09 05:46:20.000000 jemma-0.1.126/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.126/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.181016 jemma-0.1.126/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.126/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.126/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:48:30.161168 jemma-0.1.126/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-09 05:48:30.000000 jemma-0.1.126/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-09 05:48:30.000000 jemma-0.1.126/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:48:30.000000 jemma-0.1.126/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 05:48:30.000000 jemma-0.1.126/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:48:30.000000 jemma-0.1.126/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 05:48:30.000000 jemma-0.1.126/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:48:30.183535 jemma-0.1.126/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-09 05:48:25.000000 jemma-0.1.126/setup.py
```

### Comparing `jemma-0.1.125/README.md` & `jemma-0.1.126/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/huddle.py` & `jemma-0.1.126/jemma/huddle.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from jemma.requirements.feature import Feature
 from jemma.team.business_owner import BusinessOwner
 from jemma.team.engineer import Engineer
 from jemma.team.tester import Tester
 from jemma.team.project_manager import ProjectManager
 import jemma.work.flow as flow
 
-import jemma.thinker
+import jemma.thinker as thinker
 
 def main():
 
     ## ----------------------------- setup
     load_dotenv()
     args = parse_cli_arguments()
     brain = thinker.make_brain(args)
```

### Comparing `jemma-0.1.125/jemma/prompt/business/owner.py` & `jemma-0.1.126/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/prompt/engineer/clarify.py` & `jemma-0.1.126/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/prompt/engineer/code.py` & `jemma-0.1.126/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/prompt/tester/test.py` & `jemma-0.1.126/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/requirements/feature.py` & `jemma-0.1.126/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/team/business_owner.py` & `jemma-0.1.126/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/team/engineer.py` & `jemma-0.1.126/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/team/project_manager.py` & `jemma-0.1.126/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/team/tester.py` & `jemma-0.1.126/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/thinker.py` & `jemma-0.1.126/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/tools.py` & `jemma-0.1.126/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma/work/flow.py` & `jemma-0.1.126/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.125/jemma.egg-info/SOURCES.txt` & `jemma-0.1.126/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

