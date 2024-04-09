# Comparing `tmp/provisio-0.1.6.tar.gz` & `tmp/provisio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provisio-0.1.6.tar", max compression
+gzip compressed data, was "provisio-0.1.7.tar", max compression
```

## Comparing `provisio-0.1.6.tar` & `provisio-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1259 2024-03-22 10:03:32.843143 provisio-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      919 2024-03-04 16:43:17.892173 provisio-0.1.6/README.md
--rw-r--r--   0        0        0      132 2024-03-22 10:03:32.847143 provisio-0.1.6/src/provisio/__init__.py
--rw-r--r--   0        0        0     2074 2024-03-04 16:26:50.464413 provisio-0.1.6/src/provisio/provisio.py
--rw-r--r--   0        0        0     1723 2024-03-06 11:54:31.106268 provisio-0.1.6/src/provisio/provisio_exceptions.py
--rw-r--r--   0        0        0    12174 2024-03-06 11:52:38.485183 provisio-0.1.6/src/provisio/provision_logic.py
--rw-r--r--   0        0        0     4037 2024-03-23 12:33:50.151255 provisio-0.1.6/src/provisio/utils.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 provisio-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1258 2024-04-09 10:29:28.557794 provisio-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      919 2024-03-04 16:43:17.892173 provisio-0.1.7/README.md
+-rw-r--r--   0        0        0      132 2024-04-09 10:29:28.555808 provisio-0.1.7/src/provisio/__init__.py
+-rw-r--r--   0        0        0     2074 2024-04-09 09:39:54.525765 provisio-0.1.7/src/provisio/provisio.py
+-rw-r--r--   0        0        0     1723 2024-04-09 10:15:59.581532 provisio-0.1.7/src/provisio/provisio_exceptions.py
+-rw-r--r--   0        0        0    12576 2024-04-09 10:26:52.594654 provisio-0.1.7/src/provisio/provision_logic.py
+-rw-r--r--   0        0        0     4037 2024-03-23 12:33:50.151255 provisio-0.1.7/src/provisio/utils.py
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 provisio-0.1.7/PKG-INFO
```

### Comparing `provisio-0.1.6/pyproject.toml` & `provisio-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "provisio"
-version = "0.1.6"
+version = "0.1.7"
 description = "Small utility library containing city provision metric used in other projects"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "provisio", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 geopandas = "^0.14.3"
-osmnx = "^1.9.1"
+osmnx = "^1.9.2"
 tqdm = "^4.66.2"
-osm2geojson = "^0.2.4"
+osm2geojson = "^0.2.5"
 pydantic = "^2.6.1"
-momepy = "^0.7.0"
+momepy = "^0.6.0"
 networkit = "^11.0"
 numpy = "^1.23.5"
 pandas = "^2.2.0"
 networkx = "^3.2.1"
 pulp = "^2.8.0"
 loguru = "^0.7.2"
```

### Comparing `provisio-0.1.6/README.md` & `provisio-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `provisio-0.1.6/src/provisio/provisio.py` & `provisio-0.1.7/src/provisio/provisio.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     """
     demanded = buildings_with_people.copy()
     demanded["demand"] = demanded["population"] * normative
     return demanded
 
 
 def get_service_provision(
-    services: gpd.GeoDataFrame,
-    adjacency_matrix: pd.DataFrame,
     demanded_buildings: gpd.GeoDataFrame,
+    adjacency_matrix: pd.DataFrame,
+    services: gpd.GeoDataFrame,
     threshold: int,
     calculation_type: str = "gravity",
 ) -> Tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
     """Calculate load from buildings with demands on the given services using the distances matrix between them.
 
     Args:
         services (gpd.GeoDataFrame): GeoDataFrame of services
```

### Comparing `provisio-0.1.6/src/provisio/provisio_exceptions.py` & `provisio-0.1.7/src/provisio/provisio_exceptions.py`

 * *Files identical despite different names*

### Comparing `provisio-0.1.6/src/provisio/provision_logic.py` & `provisio-0.1.7/src/provisio/provision_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=singleton-comparison
 from typing import Literal, Tuple
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pulp
+import pydantic
 from loguru import logger
 from pydantic import BaseModel, InstanceOf, field_validator, model_validator
 
 from .provisio_exceptions import *
 from .utils import (
     additional_options,
     provision_matrix_transform,
@@ -80,20 +81,27 @@
                 "{} rows were deleted from the 'services' GeoDataFrame due to null values in the 'capacity' column",
                 dif_rows_count,
             )
         v["capacity_left"] = v["capacity"]
         return v
 
     @model_validator(mode="after")
-    def delete_useless_matrix_columns(self) -> "CityProvision":
-        self.adjacency_matrix.columns = self.adjacency_matrix.columns.astype(int)
+    def delete_useless_matrix_rows(self) -> "CityProvision":
+        self.adjacency_matrix.index = self.adjacency_matrix.index.astype(int)
         indexes = set(self.demanded_buildings.index.astype(int).tolist())
-        columns = set(self.adjacency_matrix.columns.astype(int).tolist())
-        dif = columns ^ indexes
-        self.adjacency_matrix.drop(columns=(list(dif)), inplace=True)
+        rows = set(self.adjacency_matrix.index.astype(int).tolist())
+        dif = rows ^ indexes
+        self.adjacency_matrix.drop(index=(list(dif)), axis=0, inplace=True)
+        return self
+
+    @model_validator(mode="after")
+    def check_crs(self) -> "CityProvision":
+        assert (
+            self.demanded_buildings.crs == self.services.crs
+        ), f"\nThe CRS in the provided geodataframes are different.\nBuildings CRS:{self.demanded_buildings.crs}\nServices CRS:{self.services.crs} \n"
         return self
 
     def get_provisions(self) -> Tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
         self._calculate_provisions()
         additional_options(
             self.demanded_buildings,
             self.services,
@@ -114,17 +122,18 @@
                 self.adjacency_matrix,
             ),
         )
 
     def _calculate_provisions(self):
         self._destination_matrix = pd.DataFrame(
             0,
-            index=self.adjacency_matrix.index,
-            columns=self.adjacency_matrix.columns,
+            index=self.adjacency_matrix.columns,
+            columns=self.adjacency_matrix.index,
         )
+        self.adjacency_matrix = self.adjacency_matrix.transpose()
         logger.debug(
             "Calculating provision from {} services to {} buildings with {} method, it may take a while ...",
             len(self.services),
             len(self.demanded_buildings),
             self.calculation_type,
         )
         if self.calculation_type == "gravity":
```

### Comparing `provisio-0.1.6/src/provisio/utils.py` & `provisio-0.1.7/src/provisio/utils.py`

 * *Files identical despite different names*

### Comparing `provisio-0.1.6/PKG-INFO` & `provisio-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: provisio
-Version: 0.1.6
+Version: 0.1.7
 Summary: Small utility library containing city provision metric used in other projects
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: geopandas (>=0.14.3,<0.15.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: momepy (>=0.7.0,<0.8.0)
+Requires-Dist: momepy (>=0.6.0,<0.7.0)
 Requires-Dist: networkit (>=11.0,<12.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: osm2geojson (>=0.2.4,<0.3.0)
-Requires-Dist: osmnx (>=1.9.1,<2.0.0)
+Requires-Dist: osm2geojson (>=0.2.5,<0.3.0)
+Requires-Dist: osmnx (>=1.9.2,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pulp (>=2.8.0,<3.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

