# Comparing `tmp/icon_uxarray-0.1.3.tar.gz` & `tmp/icon_uxarray-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icon_uxarray-0.1.3.tar", last modified: Tue Apr  9 13:17:59 2024, max compression
+gzip compressed data, was "icon_uxarray-0.1.4.tar", last modified: Tue Apr  9 13:17:56 2024, max compression
```

## Comparing `icon_uxarray-0.1.3.tar` & `icon_uxarray-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:59.054655 icon_uxarray-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:17:59.054655 icon_uxarray-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:59.050655 icon_uxarray-0.1.3/icon_uxarray/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/icon_uxarray/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/icon_uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/icon_uxarray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/icon_uxarray/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/icon_uxarray/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:59.050655 icon_uxarray-0.1.3/icon_uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:17:59.000000 icon_uxarray-0.1.3/icon_uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 13:17:59.000000 icon_uxarray-0.1.3/icon_uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:17:59.000000 icon_uxarray-0.1.3/icon_uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 13:17:59.000000 icon_uxarray-0.1.3/icon_uxarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 13:17:59.000000 icon_uxarray-0.1.3/icon_uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:17:59.000000 icon_uxarray-0.1.3/icon_uxarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:17:59.054655 icon_uxarray-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:59.050655 icon_uxarray-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/tests/Torus_Triangles_100m_x_100m_res5m.nc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-09 13:17:50.000000 icon_uxarray-0.1.3/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.822269 icon_uxarray-0.1.4/icon_uxarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/icon_uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/Torus_Triangles_100m_x_100m_res5m.nc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/test_base.py
```

### Comparing `icon_uxarray-0.1.3/HISTORY.md` & `icon_uxarray-0.1.4/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Changelog
 =========
 
 
-(unreleased)
-------------
+0.1.3 (2024-04-09)
+------------------
+- Release: version 0.1.3 🚀 [Jacopo]
 - Release: version  🚀 [Jacopo]
 - Release: version  🚀 [Jacopo]
 - Cleanup. [Jacopo]
 - Bump version number for pypi. [Jacopo]
 
 
 0.1.2 (2024-04-09)
```

### Comparing `icon_uxarray-0.1.3/LICENSE` & `icon_uxarray-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/PKG-INFO` & `icon_uxarray-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.3
+Version: 0.1.4
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `icon_uxarray-0.1.3/README.md` & `icon_uxarray-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/icon_uxarray/base.py` & `icon_uxarray-0.1.4/icon_uxarray/base.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/icon_uxarray/cli.py` & `icon_uxarray-0.1.4/icon_uxarray/cli.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/icon_uxarray.egg-info/PKG-INFO` & `icon_uxarray-0.1.4/icon_uxarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.3
+Version: 0.1.4
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `icon_uxarray-0.1.3/setup.py` & `icon_uxarray-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/tests/Torus_Triangles_100m_x_100m_res5m.nc` & `icon_uxarray-0.1.4/tests/Torus_Triangles_100m_x_100m_res5m.nc`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/tests/conftest.py` & `icon_uxarray-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.3/tests/test_base.py` & `icon_uxarray-0.1.4/tests/test_base.py`

 * *Files identical despite different names*

