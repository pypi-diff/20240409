# Comparing `tmp/icon_uxarray-0.1.4.tar.gz` & `tmp/icon_uxarray-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icon_uxarray-0.1.4.tar", last modified: Tue Apr  9 13:17:56 2024, max compression
+gzip compressed data, was "icon_uxarray-0.1.5.tar", last modified: Tue Apr  9 13:45:27 2024, max compression
```

## Comparing `icon_uxarray-0.1.4.tar` & `icon_uxarray-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.822269 icon_uxarray-0.1.4/icon_uxarray/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/icon_uxarray/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/icon_uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:17:56.000000 icon_uxarray-0.1.4/icon_uxarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:56.826269 icon_uxarray-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/Torus_Triangles_100m_x_100m_res5m.nc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-09 13:17:48.000000 icon_uxarray-0.1.4/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.683740 icon_uxarray-0.1.5/icon_uxarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/icon_uxarray/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/icon_uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:45:27.000000 icon_uxarray-0.1.5/icon_uxarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:27.687740 icon_uxarray-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/Torus_Triangles_100m_x_100m_res5m.nc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 13:45:15.000000 icon_uxarray-0.1.5/tests/test_base.py
```

### Comparing `icon_uxarray-0.1.4/HISTORY.md` & `icon_uxarray-0.1.5/HISTORY.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 Changelog
 =========
 
 
+(unreleased)
+------------
+- Refactor remove_torus_boundaries function to handle invalid input
+  gracefully. [Jacopo]
+- Actually get make release to work properly with tags. [Jacopo]
+
+
+0.1.4 (2024-04-09)
+------------------
+- Release: version 0.1.4 🚀 [Jacopo]
+
+
 0.1.3 (2024-04-09)
 ------------------
 - Release: version 0.1.3 🚀 [Jacopo]
 - Release: version  🚀 [Jacopo]
 - Release: version  🚀 [Jacopo]
 - Cleanup. [Jacopo]
 - Bump version number for pypi. [Jacopo]
```

### Comparing `icon_uxarray-0.1.4/LICENSE` & `icon_uxarray-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.4/PKG-INFO` & `icon_uxarray-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.4
+Version: 0.1.5
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `icon_uxarray-0.1.4/README.md` & `icon_uxarray-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.4/icon_uxarray/base.py` & `icon_uxarray-0.1.5/icon_uxarray/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,16 +156,18 @@
     Returns:
         ux.Grid | ux.UxDataset: The modified UX grid or dataset with torus
         boundary triangles removed.
     """
 
     if isinstance(ux_grid_or_ds, ux.UxDataset):
         grid = ux_grid_or_ds.uxgrid
-    else:
+    elif isinstance(ux_grid_or_ds, ux.Grid):
         grid = ux_grid_or_ds
+    else:
+        raise TypeError("Invalid input provided.")
 
     if grid is not None:
         lims = [
             float(grid.node_lon.min()),
             float(grid.node_lon.max()),
             float(grid.node_lat.min()),
             float(grid.node_lat.max()),
@@ -181,9 +183,10 @@
             ux_grid_or_ds2 = ux_grid_or_ds.isel(n_face=face_ids)
             ux_grid_or_ds2.uxgrid = grid2
             return ux_grid_or_ds2
         else:
             return grid2
 
     else:
-        print("ERROR: Invalid grid provided.")
+        # we're never supposed to get here, this line is just to please the
+        # linters that otherwise complain about missing return statements
         return ux_grid_or_ds
```

### Comparing `icon_uxarray-0.1.4/icon_uxarray/cli.py` & `icon_uxarray-0.1.5/icon_uxarray/cli.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.4/icon_uxarray.egg-info/PKG-INFO` & `icon_uxarray-0.1.5/icon_uxarray.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.4
+Version: 0.1.5
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `icon_uxarray-0.1.4/setup.py` & `icon_uxarray-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.4/tests/Torus_Triangles_100m_x_100m_res5m.nc` & `icon_uxarray-0.1.5/tests/Torus_Triangles_100m_x_100m_res5m.nc`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.4/tests/conftest.py` & `icon_uxarray-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.4/tests/test_base.py` & `icon_uxarray-0.1.5/tests/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Test module.
 """
 
+import pytest
 import os
 import xarray as xr
 import uxarray as ux
 from icon_uxarray.base import (
     icon_grid_2_ugrid,
     is_boundary_triangle,
     remove_torus_boundaries,
@@ -135,9 +136,9 @@
     assert result.uxgrid.node_lon.values.shape == (208,)
     assert result.uxgrid.face_node_connectivity.shape == (360, 3)
     assert float(result.temperature.min()) == 0.0
     assert float(result.temperature.max()) == 413
 
     # Test with invalid grid
     invalid_grid = None
-    result = remove_torus_boundaries(invalid_grid)
-    assert result is invalid_grid
+    with pytest.raises(Exception) as e_info:
+        remove_torus_boundaries(invalid_grid)
```

