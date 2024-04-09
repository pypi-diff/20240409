# Comparing `tmp/pyetp-0.0.3.tar.gz` & `tmp/pyetp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetp-0.0.3.tar", max compression
+gzip compressed data, was "pyetp-0.0.4.tar", max compression
```

## Comparing `pyetp-0.0.3.tar` & `pyetp-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2024-03-26 13:05:23.003556 pyetp-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1224 2024-03-26 13:05:23.003556 pyetp-0.0.3/README.md
--rw-r--r--   0        0        0      123 2024-03-26 13:05:23.771560 pyetp-0.0.3/pyetp/__init__.py
--rw-r--r--   0        0        0    32280 2024-03-26 13:05:23.771560 pyetp-0.0.3/pyetp/client.py
--rw-r--r--   0        0        0      879 2024-03-26 13:05:23.771560 pyetp-0.0.3/pyetp/config.py
--rw-r--r--   0        0        0    50492 2024-03-26 13:05:23.771560 pyetp-0.0.3/pyetp/resqml_objects/__init__.py
--rw-r--r--   0        0        0   783914 2024-03-26 13:05:23.775560 pyetp-0.0.3/pyetp/resqml_objects/generated.py
--rw-r--r--   0        0        0     2487 2024-03-26 13:05:23.775560 pyetp-0.0.3/pyetp/types.py
--rw-r--r--   0        0        0     2675 2024-03-26 13:05:23.775560 pyetp-0.0.3/pyetp/uri.py
--rw-r--r--   0        0        0     2248 2024-03-26 13:05:23.775560 pyetp-0.0.3/pyetp/utils_arrays.py
--rw-r--r--   0        0        0    18443 2024-03-26 13:05:23.775560 pyetp-0.0.3/pyetp/utils_xml.py
--rw-r--r--   0        0        0      768 2024-03-26 13:05:51.575701 pyetp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 pyetp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-09 12:18:29.210834 pyetp-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1224 2024-04-09 12:18:29.210834 pyetp-0.0.4/README.md
+-rw-r--r--   0        0        0      123 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/__init__.py
+-rw-r--r--   0        0        0    32411 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/client.py
+-rw-r--r--   0        0        0      879 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/config.py
+-rw-r--r--   0        0        0    50492 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/resqml_objects/__init__.py
+-rw-r--r--   0        0        0   783914 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/resqml_objects/generated.py
+-rw-r--r--   0        0        0     2487 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/types.py
+-rw-r--r--   0        0        0     2675 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/uri.py
+-rw-r--r--   0        0        0     2248 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/utils_arrays.py
+-rw-r--r--   0        0        0    18443 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/utils_xml.py
+-rw-r--r--   0        0        0      877 2024-04-09 12:19:03.038812 pyetp-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pyetp-0.0.4/PKG-INFO
```

### Comparing `pyetp-0.0.3/LICENSE.md` & `pyetp-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/README.md` & `pyetp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/client.py` & `pyetp-0.0.4/pyetp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import sys
 import datetime
 import logging
 import typing as T
 import uuid
 from collections import defaultdict
 from types import TracebackType
 from async_timeout import timeout
@@ -361,23 +362,24 @@
     # xtgeo
     #
 
     async def get_xtgeo_surface(self, epc_uri: T.Union[DataObjectURI , str] ,gri_uri: T.Union[DataObjectURI , str]):
         gri, = await self.get_resqml_objects(gri_uri)
 
         # some checks
+        
         assert isinstance(gri, ro.Grid2dRepresentation), "obj must be Grid2dRepresentation"
-        assert isinstance(gri.grid2d_patch.geometry.points, ro.Point3dZValueArray), "Points must be Point3dZValueArray"
-        assert isinstance(gri.grid2d_patch.geometry.points.zvalues, ro.DoubleHdf5Array), "Values must be DoubleHdf5Array"
-        assert isinstance(gri.grid2d_patch.geometry.points.zvalues.values, ro.Hdf5Dataset), "Values must be Hdf5Dataset"
-        assert isinstance(gri.grid2d_patch.geometry.points.supporting_geometry, ro.Point3dLatticeArray), "Points support_geo must be Point3dLatticeArray"
-
         sgeo = gri.grid2d_patch.geometry.points.supporting_geometry  # type: ignore
-        assert isinstance(sgeo, ro.Point3dLatticeArray), "supporting_geometry must be Point3dLatticeArray"
-
+        if sys.version_info[1] != 10:
+            assert isinstance(gri.grid2d_patch.geometry.points, ro.Point3dZValueArray), "Points must be Point3dZValueArray"
+            assert isinstance(gri.grid2d_patch.geometry.points.zvalues, ro.DoubleHdf5Array), "Values must be DoubleHdf5Array"
+            assert isinstance(gri.grid2d_patch.geometry.points.supporting_geometry, ro.Point3dLatticeArray), "Points support_geo must be Point3dLatticeArray"
+            assert isinstance(sgeo, ro.Point3dLatticeArray), "supporting_geometry must be Point3dLatticeArray"
+        assert isinstance(gri.grid2d_patch.geometry.points.zvalues.values, ro.Hdf5Dataset), "Values must be Hdf5Dataset"
+        
         # get array
         array = await self.get_array(
             DataArrayIdentifier(
                 uri=str(epc_uri), pathInResource=gri.grid2d_patch.geometry.points.zvalues.values.path_in_hdf_file
             )
         )
 
@@ -412,18 +414,19 @@
 
     async def get_epc_mesh(self, epc_uri: T.Union[DataObjectURI , str], uns_uri: T.Union[DataObjectURI , str]):
         uns, = await self.get_resqml_objects(uns_uri)
 
         # some checks
         assert isinstance(uns, ro.UnstructuredGridRepresentation), "obj must be Grid2dRepresentation"
         assert isinstance(uns.geometry, ro.UnstructuredGridGeometry), "geometry must be UnstructuredGridGeometry"
-        assert isinstance(uns.geometry.points, ro.Point3dHdf5Array), "points must be Point3dHdf5Array"
+        if sys.version_info[1] != 10:
+            assert isinstance(uns.geometry.points, ro.Point3dHdf5Array), "points must be Point3dHdf5Array"
+            assert isinstance(uns.geometry.faces_per_cell.elements, ro.IntegerHdf5Array), "faces_per_cell must be IntegerHdf5Array"
+            assert isinstance(uns.geometry.faces_per_cell.cumulative_length, ro.IntegerHdf5Array), "faces_per_cell cl must be IntegerHdf5Array"
         assert isinstance(uns.geometry.points.coordinates, ro.Hdf5Dataset), "coordinates must be Hdf5Dataset"
-        assert isinstance(uns.geometry.faces_per_cell.elements, ro.IntegerHdf5Array), "faces_per_cell must be IntegerHdf5Array"
-        assert isinstance(uns.geometry.faces_per_cell.cumulative_length, ro.IntegerHdf5Array), "faces_per_cell cl must be IntegerHdf5Array"
 
         # # get array
         points = await self.get_array(
             DataArrayIdentifier(
                 uri=str(epc_uri), pathInResource=uns.geometry.points.coordinates.path_in_hdf_file
             )
         )
```

### Comparing `pyetp-0.0.3/pyetp/config.py` & `pyetp-0.0.4/pyetp/config.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/resqml_objects/__init__.py` & `pyetp-0.0.4/pyetp/resqml_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/resqml_objects/generated.py` & `pyetp-0.0.4/pyetp/resqml_objects/generated.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/types.py` & `pyetp-0.0.4/pyetp/types.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/uri.py` & `pyetp-0.0.4/pyetp/uri.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/utils_arrays.py` & `pyetp-0.0.4/pyetp/utils_arrays.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyetp/utils_xml.py` & `pyetp-0.0.4/pyetp/utils_xml.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.3/pyproject.toml` & `pyetp-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "pyetp"
-version = "0.0.3"
-description = ""
+version = "0.0.4"
+description = "Interface with OSDU RDDMS using ETP protocol"
 authors = ["Adam Cheng <52572642+adamchengtkc@users.noreply.github.com>"]
 readme = "README.md"
 license = "LGPL-3.0-only"
+homepage = "https://github.com/equinor/pyetp"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = "^1.26.3"
 websockets = "^12.0"
 lxml = "^4.9.4"
 pydantic = "^1.10"
@@ -17,14 +18,15 @@
 pyarrow = "^15.0.0"  # added to fix pandas deprecated warning in xtgeo
 etpproto = "^1.0.5"
 httpx = "^0.26.0"
 xtgeo = "^3.8.0"
 xsdata = "^24.3.1"
 resqpy = "^4.14.3"
 async-timeout = "^4.0.3"
+pillow = "^10.3.0"
 
 [tool.poetry.group.dev.dependencies]
 notebook = "^7.0.7"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.4"
 fakeredis = "^2.21.0"
 pytest-cov = "^4.1.0"
```

### Comparing `pyetp-0.0.3/PKG-INFO` & `pyetp-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pyetp
-Version: 0.0.3
-Summary: 
+Version: 0.0.4
+Summary: Interface with OSDU RDDMS using ETP protocol
+Home-page: https://github.com/equinor/pyetp
 License: LGPL-3.0-only
 Author: Adam Cheng
 Author-email: 52572642+adamchengtkc@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: async-lru (>=2.0.4,<3.0.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: etpproto (>=1.0.5,<2.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: lxml (>=4.9.4,<5.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: redis (>=5.0.1,<6.0.0)
 Requires-Dist: resqpy (>=4.14.3,<5.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Requires-Dist: xsdata (>=24.3.1,<25.0.0)
 Requires-Dist: xtgeo (>=3.8.0,<4.0.0)
```

