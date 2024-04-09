# Comparing `tmp/fathomnet-1.3.0.tar.gz` & `tmp/fathomnet-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fathomnet-1.3.0.tar", max compression
+gzip compressed data, was "fathomnet-1.4.0.tar", max compression
```

## Comparing `fathomnet-1.3.0.tar` & `fathomnet-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1097 2024-02-29 23:08:27.423454 fathomnet-1.3.0/LICENSE
--rw-r--r--   0        0        0     1855 2024-02-29 23:08:27.423454 fathomnet-1.3.0/README.md
--rw-r--r--   0        0        0       29 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/__init__.py
--rw-r--r--   0        0        0     2426 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/__init__.py
--rw-r--r--   0        0        0     2517 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/activity.py
--rw-r--r--   0        0        0     6570 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/boundingboxes.py
--rw-r--r--   0        0        0     2271 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/comments.py
--rw-r--r--   0        0        0      461 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/darwincore.py
--rw-r--r--   0        0        0      670 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/firebase.py
--rw-r--r--   0        0        0     1691 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/geoimages.py
--rw-r--r--   0        0        0     4740 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/images.py
--rw-r--r--   0        0        0     2172 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/imagesetuploads.py
--rw-r--r--   0        0        0     1287 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/regions.py
--rw-r--r--   0        0        0      309 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/stats.py
--rw-r--r--   0        0        0     1271 2024-02-29 23:08:27.423454 fathomnet-1.3.0/fathomnet/api/tags.py
--rw-r--r--   0        0        0     1367 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/api/taxa.py
--rw-r--r--   0        0        0     1688 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/api/topics.py
--rw-r--r--   0        0        0     5205 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/api/users.py
--rw-r--r--   0        0        0     3141 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/api/worms.py
--rw-r--r--   0        0        0      726 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/api/xapikey.py
--rw-r--r--   0        0        0    17731 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/dto.py
--rw-r--r--   0        0        0      250 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/models/__init__.py
--rw-r--r--   0        0        0      798 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/models/bases.py
--rw-r--r--   0        0        0     1896 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/models/yolov5.py
--rw-r--r--   0        0        0        0 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/scripts/__init__.py
--rw-r--r--   0        0        0    20634 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/scripts/fathomnet_generate.py
--rw-r--r--   0        0        0     1850 2024-02-29 23:08:27.427454 fathomnet-1.3.0/fathomnet/util.py
--rw-r--r--   0        0        0     3252 2024-02-29 23:08:27.427454 fathomnet-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 fathomnet-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-04-09 16:38:23.616005 fathomnet-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1855 2024-04-09 16:38:23.616005 fathomnet-1.4.0/README.md
+-rw-r--r--   0        0        0       29 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/__init__.py
+-rw-r--r--   0        0        0     2426 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/__init__.py
+-rw-r--r--   0        0        0     2517 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/activity.py
+-rw-r--r--   0        0        0     6570 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/boundingboxes.py
+-rw-r--r--   0        0        0     2271 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/comments.py
+-rw-r--r--   0        0        0      461 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/darwincore.py
+-rw-r--r--   0        0        0      670 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/firebase.py
+-rw-r--r--   0        0        0     1691 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/geoimages.py
+-rw-r--r--   0        0        0     4740 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/images.py
+-rw-r--r--   0        0        0     2172 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/imagesetuploads.py
+-rw-r--r--   0        0        0     1287 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/regions.py
+-rw-r--r--   0        0        0      309 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/stats.py
+-rw-r--r--   0        0        0     1271 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/tags.py
+-rw-r--r--   0        0        0     1367 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/taxa.py
+-rw-r--r--   0        0        0     1688 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/topics.py
+-rw-r--r--   0        0        0     5205 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/users.py
+-rw-r--r--   0        0        0     3196 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/worms.py
+-rw-r--r--   0        0        0      726 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/api/xapikey.py
+-rw-r--r--   0        0        0    17731 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/dto.py
+-rw-r--r--   0        0        0      250 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/models/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/models/bases.py
+-rw-r--r--   0        0        0     1896 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/models/yolov5.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:38:23.616005 fathomnet-1.4.0/fathomnet/scripts/__init__.py
+-rw-r--r--   0        0        0    20634 2024-04-09 16:38:23.620005 fathomnet-1.4.0/fathomnet/scripts/fathomnet_generate.py
+-rw-r--r--   0        0        0     1850 2024-04-09 16:38:23.620005 fathomnet-1.4.0/fathomnet/util.py
+-rw-r--r--   0        0        0     3252 2024-04-09 16:38:23.620005 fathomnet-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 fathomnet-1.4.0/PKG-INFO
```

### Comparing `fathomnet-1.3.0/LICENSE` & `fathomnet-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/README.md` & `fathomnet-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/__init__.py` & `fathomnet-1.4.0/fathomnet/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/activity.py` & `fathomnet-1.4.0/fathomnet/api/activity.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/boundingboxes.py` & `fathomnet-1.4.0/fathomnet/api/boundingboxes.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/comments.py` & `fathomnet-1.4.0/fathomnet/api/comments.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/firebase.py` & `fathomnet-1.4.0/fathomnet/api/firebase.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/geoimages.py` & `fathomnet-1.4.0/fathomnet/api/geoimages.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/images.py` & `fathomnet-1.4.0/fathomnet/api/images.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/imagesetuploads.py` & `fathomnet-1.4.0/fathomnet/api/imagesetuploads.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/regions.py` & `fathomnet-1.4.0/fathomnet/api/regions.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/tags.py` & `fathomnet-1.4.0/fathomnet/api/tags.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/taxa.py` & `fathomnet-1.4.0/fathomnet/api/taxa.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/topics.py` & `fathomnet-1.4.0/fathomnet/api/topics.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/users.py` & `fathomnet-1.4.0/fathomnet/api/users.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/api/worms.py` & `fathomnet-1.4.0/fathomnet/api/worms.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
 
 def get_children_names(name: str) -> List[str]:
     """Get all children's names of a given name."""
     return Worms.get(f'children/{name}')
 
 
-def get_descendants_names(name: str) -> List[str]:
+def get_descendants_names(name: str, accepted: bool = False) -> List[str]:
     """Get all descendants' names of a given name."""
-    return Worms.get(f'descendants/{name}')
+    return Worms.get(f'descendants/{name}', params={'accepted': accepted})
 
 
 def get_parent_name(name: str) -> str:
     """Get the parent's name of a given name."""
     return Worms.get(f'parent/{name}')
```

### Comparing `fathomnet-1.3.0/fathomnet/api/xapikey.py` & `fathomnet-1.4.0/fathomnet/api/xapikey.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/dto.py` & `fathomnet-1.4.0/fathomnet/dto.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/models/bases.py` & `fathomnet-1.4.0/fathomnet/models/bases.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/models/yolov5.py` & `fathomnet-1.4.0/fathomnet/models/yolov5.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/scripts/fathomnet_generate.py` & `fathomnet-1.4.0/fathomnet/scripts/fathomnet_generate.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/fathomnet/util.py` & `fathomnet-1.4.0/fathomnet/util.py`

 * *Files identical despite different names*

### Comparing `fathomnet-1.3.0/pyproject.toml` & `fathomnet-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fathomnet"
-version = "1.3.0"
+version = "1.4.0"
 description = "fathomnet-py is a client-side API to help scientists, researchers, and developers interact with FathomNet data."
 license = "MIT"
 authors = ["Kevin Barnard <kbarnard@mbari.org>"]
 maintainers = ["Kevin Barnard <kbarnard@mbari.org>"]
 readme = "README.md"
 homepage = "https://github.com/fathomnet/fathomnet-py"
 repository = "https://github.com/fathomnet/fathomnet-py"
```

### Comparing `fathomnet-1.3.0/PKG-INFO` & `fathomnet-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fathomnet
-Version: 1.3.0
+Version: 1.4.0
 Summary: fathomnet-py is a client-side API to help scientists, researchers, and developers interact with FathomNet data.
 Home-page: https://github.com/fathomnet/fathomnet-py
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Maintainer: Kevin Barnard
 Maintainer-email: kbarnard@mbari.org
```

