# Comparing `tmp/jemma-0.1.1282.tar.gz` & `tmp/jemma-0.1.1283.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1282.tar", last modified: Tue Apr  9 18:58:59 2024, max compression
+gzip compressed data, was "jemma-0.1.1283.tar", last modified: Tue Apr  9 19:07:52 2024, max compression
```

## Comparing `jemma-0.1.1282.tar` & `jemma-0.1.1283.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.297519 jemma-0.1.1282/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 18:58:59.296813 jemma-0.1.1282/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      751 2024-04-09 16:26:34.000000 jemma-0.1.1282/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.271531 jemma-0.1.1282/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1282/jemma/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2311 2024-04-09 05:47:27.000000 jemma-0.1.1282/jemma/huddle.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.277949 jemma-0.1.1282/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1282/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.280202 jemma-0.1.1282/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1282/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1282/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.283744 jemma-0.1.1282/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1282/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1282/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15402 2024-04-09 18:44:55.000000 jemma-0.1.1282/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.285905 jemma-0.1.1282/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1282/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1282/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.288278 jemma-0.1.1282/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1282/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1282/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.293589 jemma-0.1.1282/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1282/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1282/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.1282/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1282/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1282/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1282/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.1282/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.295755 jemma-0.1.1282/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1282/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1282/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 18:58:59.276699 jemma-0.1.1282/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 18:58:59.000000 jemma-0.1.1282/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-09 18:58:59.000000 jemma-0.1.1282/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 18:58:59.000000 jemma-0.1.1282/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 18:58:59.000000 jemma-0.1.1282/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 18:58:59.000000 jemma-0.1.1282/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 18:58:59.000000 jemma-0.1.1282/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 18:58:59.297715 jemma-0.1.1282/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      464 2024-04-09 18:58:55.000000 jemma-0.1.1282/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.638162 jemma-0.1.1283/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:07:52.637452 jemma-0.1.1283/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      751 2024-04-09 16:26:34.000000 jemma-0.1.1283/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.608817 jemma-0.1.1283/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1283/jemma/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.615548 jemma-0.1.1283/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1283/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.617452 jemma-0.1.1283/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1283/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1283/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.620614 jemma-0.1.1283/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1283/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1283/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15402 2024-04-09 18:44:55.000000 jemma-0.1.1283/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.622777 jemma-0.1.1283/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1283/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1283/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.624820 jemma-0.1.1283/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1283/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1283/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.633017 jemma-0.1.1283/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1283/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1283/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.1283/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1283/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1283/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1283/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.1283/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.635957 jemma-0.1.1283/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1283/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1283/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:07:52.614239 jemma-0.1.1283/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:07:52.000000 jemma-0.1.1283/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-09 19:07:52.000000 jemma-0.1.1283/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 19:07:52.000000 jemma-0.1.1283/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 19:07:52.000000 jemma-0.1.1283/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 19:07:52.000000 jemma-0.1.1283/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 19:07:52.000000 jemma-0.1.1283/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 19:07:52.638373 jemma-0.1.1283/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 19:07:26.000000 jemma-0.1.1283/setup.py
```

### Comparing `jemma-0.1.1282/README.md` & `jemma-0.1.1283/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/prompt/business/owner.py` & `jemma-0.1.1283/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/prompt/engineer/clarify.py` & `jemma-0.1.1283/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/prompt/engineer/code.py` & `jemma-0.1.1283/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/prompt/tester/test.py` & `jemma-0.1.1283/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/requirements/feature.py` & `jemma-0.1.1283/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/team/business_owner.py` & `jemma-0.1.1283/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/team/engineer.py` & `jemma-0.1.1283/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/team/project_manager.py` & `jemma-0.1.1283/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/team/tester.py` & `jemma-0.1.1283/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/thinker.py` & `jemma-0.1.1283/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/tools.py` & `jemma-0.1.1283/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma/work/flow.py` & `jemma-0.1.1283/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1282/jemma.egg-info/SOURCES.txt` & `jemma-0.1.1283/jemma.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.py
 jemma/__init__.py
-jemma/huddle.py
 jemma/thinker.py
 jemma/tools.py
 jemma.egg-info/PKG-INFO
 jemma.egg-info/SOURCES.txt
 jemma.egg-info/dependency_links.txt
 jemma.egg-info/entry_points.txt
 jemma.egg-info/requires.txt
```

