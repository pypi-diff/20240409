# Comparing `tmp/omniply-0.3.1.tar.gz` & `tmp/omniply-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniply-0.3.1.tar", last modified: Mon Apr  8 10:10:00 2024, max compression
+gzip compressed data, was "omniply-0.3.2.tar", last modified: Tue Apr  9 12:50:28 2024, max compression
```

## Comparing `omniply-0.3.1.tar` & `omniply-0.3.2.tar`

### file list

```diff
@@ -1,49 +1,56 @@
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/
--rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2024-02-14 16:25:24.000000 omniply-0.3.1/LICENSE
--rw-r--r--   0 fleeb     (7343) is        (1040)      518 2024-04-08 10:10:00.592860 omniply-0.3.1/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)      216 2024-02-14 16:25:24.000000 omniply-0.3.1/README.md
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/
--rw-r--r--   0 fleeb     (7343) is        (1040)       62 2024-04-08 10:09:14.000000 omniply-0.3.1/omniply/__init__.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/_future/
--rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     2501 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/common.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     4287 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/specification.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3749 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/_future/wrappers.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/apps/
--rw-r--r--   0 fleeb     (7343) is        (1040)      225 2024-04-08 10:02:27.000000 omniply-0.3.1/omniply/apps/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8556 2024-04-08 10:08:53.000000 omniply-0.3.1/omniply/apps/decisions.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/apps/iterative/
--rw-r--r--   0 fleeb     (7343) is        (1040)       25 2024-03-29 16:54:35.000000 omniply-0.3.1/omniply/apps/iterative/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1590 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/abstract.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      673 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/guru.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      189 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/imports.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      725 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/iterative/innovators.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1343 2024-03-29 16:54:35.000000 omniply-0.3.1/omniply/apps/iterative/moguls.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3633 2024-04-07 16:16:51.000000 omniply-0.3.1/omniply/apps/simple.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1362 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/staging.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1386 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/apps/templating.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1884 2024-04-07 16:40:21.000000 omniply-0.3.1/omniply/apps/unit_test.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/core/
--rw-r--r--   0 fleeb     (7343) is        (1040)      172 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/core/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8828 2024-04-07 15:17:06.000000 omniply-0.3.1/omniply/core/abstract.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     2050 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/core/errors.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     6745 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/core/gadgets.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    11763 2024-04-07 15:55:23.000000 omniply-0.3.1/omniply/core/gaggles.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    11004 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/games.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8124 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/gates.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8770 2024-04-07 15:11:45.000000 omniply-0.3.1/omniply/core/genetics.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1353 2024-02-14 16:25:24.000000 omniply-0.3.1/omniply/core/gizmos.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     5437 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/op.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     7138 2024-04-07 15:09:20.000000 omniply-0.3.1/omniply/core/tools.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    27492 2024-04-07 15:24:29.000000 omniply-0.3.1/omniply/core/unit_test.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply/spaces/
--rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:57:26.000000 omniply-0.3.1/omniply/spaces/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:58:04.000000 omniply-0.3.1/omniply/spaces/imports.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-08 10:10:00.592860 omniply-0.3.1/omniply.egg-info/
--rw-r--r--   0 fleeb     (7343) is        (1040)      518 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)     1014 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/SOURCES.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/dependency_links.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)       15 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/requires.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        8 2024-04-08 10:10:00.000000 omniply-0.3.1/omniply.egg-info/top_level.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)      428 2024-04-08 10:10:00.592860 omniply-0.3.1/setup.cfg
--rw-r--r--   0 fleeb     (7343) is        (1040)       38 2024-02-14 16:25:24.000000 omniply-0.3.1/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.744096 omniply-0.3.2/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2024-02-14 16:25:24.000000 omniply-0.3.2/LICENSE
+-rw-r--r--   0 fleeb     (7343) is        (1040)      518 2024-04-09 12:50:28.744096 omniply-0.3.2/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      216 2024-02-14 16:25:24.000000 omniply-0.3.2/README.md
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.740096 omniply-0.3.2/omniply/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       62 2024-04-09 12:49:45.000000 omniply-0.3.2/omniply/__init__.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.740096 omniply-0.3.2/omniply/_future/
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:25:24.000000 omniply-0.3.2/omniply/_future/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2501 2024-02-14 16:25:24.000000 omniply-0.3.2/omniply/_future/common.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4287 2024-02-14 16:25:24.000000 omniply-0.3.2/omniply/_future/specification.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3749 2024-02-14 16:25:24.000000 omniply-0.3.2/omniply/_future/wrappers.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.740096 omniply-0.3.2/omniply/apps/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      184 2024-04-09 12:46:17.000000 omniply-0.3.2/omniply/apps/__init__.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.740096 omniply-0.3.2/omniply/apps/decisions/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       87 2024-04-09 12:45:54.000000 omniply-0.3.2/omniply/apps/decisions/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1746 2024-04-09 12:07:02.000000 omniply-0.3.2/omniply/apps/decisions/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6960 2024-04-09 12:30:45.000000 omniply-0.3.2/omniply/apps/decisions/chains.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6658 2024-04-09 12:41:35.000000 omniply-0.3.2/omniply/apps/decisions/decisions.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      300 2024-04-08 16:26:58.000000 omniply-0.3.2/omniply/apps/decisions/errors.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      385 2024-04-08 16:30:11.000000 omniply-0.3.2/omniply/apps/decisions/imports.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4546 2024-04-09 12:18:31.000000 omniply-0.3.2/omniply/apps/decisions/op.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5510 2024-04-09 12:48:13.000000 omniply-0.3.2/omniply/apps/decisions/unit_test.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.744096 omniply-0.3.2/omniply/apps/iterative/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       25 2024-03-29 16:54:35.000000 omniply-0.3.2/omniply/apps/iterative/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1590 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/apps/iterative/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      673 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/apps/iterative/guru.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      189 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/apps/iterative/imports.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      725 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/apps/iterative/innovators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1343 2024-03-29 16:54:35.000000 omniply-0.3.2/omniply/apps/iterative/moguls.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3633 2024-04-07 16:16:51.000000 omniply-0.3.2/omniply/apps/simple.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1362 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/apps/staging.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1386 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/apps/templating.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.744096 omniply-0.3.2/omniply/core/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      172 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/core/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     9023 2024-04-08 17:12:30.000000 omniply-0.3.2/omniply/core/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2050 2024-02-14 16:25:24.000000 omniply-0.3.2/omniply/core/errors.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6745 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/core/gadgets.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    11508 2024-04-08 17:14:08.000000 omniply-0.3.2/omniply/core/gaggles.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    10999 2024-04-08 17:06:47.000000 omniply-0.3.2/omniply/core/games.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8124 2024-04-07 15:24:29.000000 omniply-0.3.2/omniply/core/gates.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8770 2024-04-07 15:11:45.000000 omniply-0.3.2/omniply/core/genetics.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1353 2024-02-14 16:25:24.000000 omniply-0.3.2/omniply/core/gizmos.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5395 2024-04-08 17:12:30.000000 omniply-0.3.2/omniply/core/op.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     7138 2024-04-07 15:09:20.000000 omniply-0.3.2/omniply/core/tools.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    27492 2024-04-07 15:24:29.000000 omniply-0.3.2/omniply/core/unit_test.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.744096 omniply-0.3.2/omniply/spaces/
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:57:26.000000 omniply-0.3.2/omniply/spaces/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:58:04.000000 omniply-0.3.2/omniply/spaces/imports.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-09 12:50:28.740096 omniply-0.3.2/omniply.egg-info/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      518 2024-04-09 12:50:28.000000 omniply-0.3.2/omniply.egg-info/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1233 2024-04-09 12:50:28.000000 omniply-0.3.2/omniply.egg-info/SOURCES.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-04-09 12:50:28.000000 omniply-0.3.2/omniply.egg-info/dependency_links.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       15 2024-04-09 12:50:28.000000 omniply-0.3.2/omniply.egg-info/requires.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        8 2024-04-09 12:50:28.000000 omniply-0.3.2/omniply.egg-info/top_level.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)      428 2024-04-09 12:50:28.744096 omniply-0.3.2/setup.cfg
+-rw-r--r--   0 fleeb     (7343) is        (1040)       38 2024-02-14 16:25:24.000000 omniply-0.3.2/setup.py
```

### Comparing `omniply-0.3.1/LICENSE` & `omniply-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/PKG-INFO` & `omniply-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniply
-Version: 0.3.1
+Version: 0.3.2
 Summary: "Omni-ply Versatile Data Management for Rapid AI Prototyping and Research"
 Author: Felix Leeb
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `omniply-0.3.1/omniply/_future/common.py` & `omniply-0.3.2/omniply/_future/common.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/_future/specification.py` & `omniply-0.3.2/omniply/_future/specification.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/_future/wrappers.py` & `omniply-0.3.2/omniply/_future/wrappers.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/iterative/abstract.py` & `omniply-0.3.2/omniply/apps/iterative/abstract.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/iterative/guru.py` & `omniply-0.3.2/omniply/apps/iterative/guru.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/iterative/innovators.py` & `omniply-0.3.2/omniply/apps/iterative/innovators.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/iterative/moguls.py` & `omniply-0.3.2/omniply/apps/iterative/moguls.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/simple.py` & `omniply-0.3.2/omniply/apps/simple.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/staging.py` & `omniply-0.3.2/omniply/apps/staging.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/apps/templating.py` & `omniply-0.3.2/omniply/apps/templating.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/abstract.py` & `omniply-0.3.2/omniply/core/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -249,18 +249,22 @@
 		raise NotImplementedError
 
 
 
 ### exotic animals
 
 
-class AbstractGenerous(AbstractGame):
-	def gabel(self):
-		'''duplicates this game, all the tools should be included, but not the cache'''
-		raise NotImplementedError
+# class AbstractGenerous:
+# 	def gabel(self):
+# 		'''duplicates this game, all the tools should be included, but not the cache'''
+# 		raise NotImplementedError
+#
+# 	def gathering(self, gizmo: str = None) -> Iterator[AbstractGadget]:
+# 		'''returns all the gadgets known to this object, generally used to make shallow copies'''
+# 		raise NotImplementedError
 
 
 
 class AbstractConsistentGame(AbstractGame):
 	def is_unchanged(self, gizmo: str):
 		raise NotImplementedError
```

### Comparing `omniply-0.3.1/omniply/core/errors.py` & `omniply-0.3.2/omniply/core/errors.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/gadgets.py` & `omniply-0.3.2/omniply/core/gadgets.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/gaggles.py` & `omniply-0.3.2/omniply/core/gaggles.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,26 +64,14 @@
 
 		Args:
 			gizmo (Optional[str]): The name of the gizmo to check. If not provided, all gadgets are returned.
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the gadgets that can produce the given gizmo.
 		"""
-		yield from self._vendors(gizmo)
-
-	def _vendors(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
-		"""
-		Private method that returns all known subgadgets that can produce the given gizmo.
-
-		Args:
-			gizmo (Optional[str]): The name of the gizmo to check. If not provided, all gadgets are returned.
-
-		Returns:
-			Iterator[AbstractGadget]: An iterator over the gadgets that can produce the given gizmo.
-		"""
 		if gizmo is None:
 			yield from reversed(self._gadgets_list)
 		else:
 			if gizmo not in self._gadgets_table:
 				raise self._MissingGadgetError(gizmo)
 			yield from reversed(self._gadgets_table[gizmo])
 
@@ -94,15 +82,15 @@
 
 		Args:
 			gizmo (Optional[str]): The name of the gizmo to check. If not provided, all gadgets are returned.
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the gadgets that can produce the given gizmo.
 		"""
-		for vendor in self._vendors(gizmo):
+		for vendor in self.vendors(gizmo):
 			if isinstance(vendor, AbstractGaggle):
 				yield from vendor.gadgets(gizmo)
 			else:
 				yield vendor
 
 
 	_AssemblyFailedError = AssemblyError
@@ -132,18 +120,24 @@
 				raise
 		if failures:
 			raise self._AssemblyFailedError(failures)
 		raise self._MissingGadgetError(gizmo)
 
 
 
+# class GenerousGaggle(GaggleBase, AbstractGenerous):
+# 	def gathering(self, gizmo: str = None) -> Iterator[AbstractGadget]:
+# 		yield from self._vendors(gizmo)
+
+
+
 class MultiGadgetBase(AbstractGaggle):
 	"""
-	MultiGadgetBase is a special kind of gaggle that hides all sub-gadgets from being accessed through `gadgets()`
-	and `vendors()`. Instead, it presents itself as a gadget that can produce all the products of the sub-gadgets.
+	MultiGadgetBase is a special kind of gaggle that hides all sub-gadgets from being accessed through `gadgets()`.
+	Instead, it presents itself as a gadget that can produce all the products of the sub-gadgets.
 
 	Generally, if you know before runtime what gizmos a gadget can produce, then it should just be a gadget, however,
 	if you want to be able to dynamically add sub-gadgets, while still preventing delegation, then you can use this.
 
 	"""
 	def gadgets(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
 		"""
@@ -156,28 +150,28 @@
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the known gadgets in this multi-gadget that can produce the
 			specified gizmo. Since this is a multi-gadget, it yields only itself.
 		"""
 		yield self
 
-	def vendors(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
-		"""
-		Lists all known sub-gadgets and sub-gaggles in this multi-gadget that can produce the given gizmo.
-		Since this is a multi-gadget, it doesn't delegate to sub-gadgets, and instead yields itself.
-
-		Args:
-			gizmo (Optional[str]): If specified, yields only the gadgets that can produce this gizmo. In this case, it
-			checks if this multi-gadget can produce the gizmo.
-
-		Returns:
-			Iterator[AbstractGadget]: An iterator over the known gadgets that can directly produce the given gizmo. Since
-			this is a multi-gadget, it yields itself.
-		"""
-		yield self
+	# def vendors(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
+	# 	"""
+	# 	Lists all known sub-gadgets and sub-gaggles in this multi-gadget that can produce the given gizmo.
+	# 	Since this is a multi-gadget, it doesn't delegate to sub-gadgets, and instead yields itself.
+	#
+	# 	Args:
+	# 		gizmo (Optional[str]): If specified, yields only the gadgets that can produce this gizmo. In this case, it
+	# 		checks if this multi-gadget can produce the gizmo.
+	#
+	# 	Returns:
+	# 		Iterator[AbstractGadget]: An iterator over the known gadgets that can directly produce the given gizmo. Since
+	# 		this is a multi-gadget, it yields itself.
+	# 	"""
+	# 	yield self
 
 
 
 class LoopyGaggle(GaggleBase):
 	"""
 	The LoopyGaggle class is mix-in for custom gaggles that allows multiple gadgets that produce the same gizmos to
 	recursively call each other. Specifically, if a subgadget requires the same gizmo as input as it produces, then the
```

### Comparing `omniply-0.3.1/omniply/core/games.py` & `omniply-0.3.2/omniply/core/games.py`

 * *Files 4% similar despite different names*

```diff
@@ -392,12 +392,7 @@
 
 	def check_gadget_cache(self, gadget: AbstractGadget) -> dict[str, Any]:
 		return self._gadget_precomputes.get(gadget, {})
 
 
 
 
-
-
-
-
-
```

### Comparing `omniply-0.3.1/omniply/core/gates.py` & `omniply-0.3.2/omniply/core/gates.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/genetics.py` & `omniply-0.3.2/omniply/core/genetics.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/gizmos.py` & `omniply-0.3.2/omniply/core/gizmos.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/op.py` & `omniply-0.3.2/omniply/core/op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Iterable, Callable
-from .abstract import AbstractGadget, AbstractGaggle, AbstractGame, AbstractGate, AbstractGenerous
+from .abstract import AbstractGadget, AbstractGaggle, AbstractGame, AbstractGate
 from .errors import GadgetFailure, MissingGadget
 from .tools import ToolCraftBase, AutoToolCraft, MIMOToolDecorator, AutoToolDecorator
 from .gizmos import DashGizmo
 from .gaggles import MutableGaggle, LoopyGaggle, CraftyGaggle
 from .games import CacheGame, GatedCache, TraceGame, RollingGame, ConsistentGame
 from .gates import GateBase, CachableGate, SelectiveGate
 from .genetics import GeneticGaggle
@@ -59,16 +59,15 @@
 			args: Variable length argument list.
 			kwargs: Arbitrary keyword arguments.
 		"""
 		super().__init__(*args, **kwargs)
 		self._process_crafts()
 
 
-class Context(GatedCache, ConsistentGame, RollingGame, LoopyGaggle, MutableGaggle, GeneticGaggle,
-			  AbstractGenerous, AbstractGame):
+class Context(GatedCache, ConsistentGame, RollingGame, LoopyGaggle, MutableGaggle, GeneticGaggle, AbstractGame):
 	"""
 	The Context class is a subclass of GateCache, LoopyGaggle, MutableGaggle, and AbstractGame. It provides methods to handle
 	gadgets in a context.
 
 	Methods:
 		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Context class.
 		__getitem__(self, item): Returns the grabbed item from the context.
@@ -88,15 +87,15 @@
 		"""
 		super().__init__(**kwargs)
 		self.include(*gadgets)
 
 
 	def gabel(self):
 		'''effectively a shallow copy, excluding the cache'''
-		return self.__class__(*self._vendors())
+		return self.__class__(*self.vendors())
 
 
 	def __getitem__(self, item):
 		"""
 		Returns the grabbed item from the context.
 
 		Args:
```

### Comparing `omniply-0.3.1/omniply/core/tools.py` & `omniply-0.3.2/omniply/core/tools.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply/core/unit_test.py` & `omniply-0.3.2/omniply/core/unit_test.py`

 * *Files identical despite different names*

### Comparing `omniply-0.3.1/omniply.egg-info/PKG-INFO` & `omniply-0.3.2/omniply.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniply
-Version: 0.3.1
+Version: 0.3.2
 Summary: "Omni-ply Versatile Data Management for Rapid AI Prototyping and Research"
 Author: Felix Leeb
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `omniply-0.3.1/omniply.egg-info/SOURCES.txt` & `omniply-0.3.2/omniply.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,25 @@
 omniply.egg-info/requires.txt
 omniply.egg-info/top_level.txt
 omniply/_future/__init__.py
 omniply/_future/common.py
 omniply/_future/specification.py
 omniply/_future/wrappers.py
 omniply/apps/__init__.py
-omniply/apps/decisions.py
 omniply/apps/simple.py
 omniply/apps/staging.py
 omniply/apps/templating.py
-omniply/apps/unit_test.py
+omniply/apps/decisions/__init__.py
+omniply/apps/decisions/abstract.py
+omniply/apps/decisions/chains.py
+omniply/apps/decisions/decisions.py
+omniply/apps/decisions/errors.py
+omniply/apps/decisions/imports.py
+omniply/apps/decisions/op.py
+omniply/apps/decisions/unit_test.py
 omniply/apps/iterative/__init__.py
 omniply/apps/iterative/abstract.py
 omniply/apps/iterative/guru.py
 omniply/apps/iterative/imports.py
 omniply/apps/iterative/innovators.py
 omniply/apps/iterative/moguls.py
 omniply/core/__init__.py
```

