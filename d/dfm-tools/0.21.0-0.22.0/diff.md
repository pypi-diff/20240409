# Comparing `tmp/dfm_tools-0.21.0.tar.gz` & `tmp/dfm_tools-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfm_tools-0.21.0.tar", last modified: Thu Mar 14 14:17:46 2024, max compression
+gzip compressed data, was "dfm_tools-0.22.0.tar", last modified: Tue Apr  9 17:27:47 2024, max compression
```

## Comparing `dfm_tools-0.21.0.tar` & `dfm_tools-0.22.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:17:46.536221 dfm_tools-0.21.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-14 14:17:46.536221 dfm_tools-0.21.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:17:46.532221 dfm_tools-0.21.0/dfm_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/coastlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/energy_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    27388 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/get_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/get_nc_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30674 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/hydrolib_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    35052 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/interpolate_grid2bnd.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/linebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/modelbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    23869 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/modplot.py
--rw-r--r--   0 runner    (1001) docker     (127)    41056 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/xarray_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28439 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/dfm_tools/xugrid_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:17:46.536221 dfm_tools-0.21.0/dfm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-14 14:17:46.000000 dfm_tools-0.21.0/dfm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-14 14:17:46.000000 dfm_tools-0.21.0/dfm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:17:46.000000 dfm_tools-0.21.0/dfm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-14 14:17:46.000000 dfm_tools-0.21.0/dfm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-14 14:17:46.000000 dfm_tools-0.21.0/dfm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 14:17:46.536221 dfm_tools-0.21.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:17:46.536221 dfm_tools-0.21.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_coastlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21328 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_dfm_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_external_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_get_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_hydrolib_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22937 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_interpolate_grid2bnd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_modelbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_xarray_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-03-14 14:16:50.000000 dfm_tools-0.21.0/tests/test_xugrid_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.313413 dfm_tools-0.22.0/dfm_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/energy_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27388 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/get_nc_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30674 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35052 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/linebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23869 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/modplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47235 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/xarray_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28439 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/dfm_tools/xugrid_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/dfm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 17:27:47.000000 dfm_tools-0.22.0/dfm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:47.317414 dfm_tools-0.22.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21328 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_dfm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_external_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22937 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_xarray_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-09 17:26:54.000000 dfm_tools-0.22.0/tests/test_xugrid_helpers.py
```

### Comparing `dfm_tools-0.21.0/LICENSE` & `dfm_tools-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/PKG-INFO` & `dfm_tools-0.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfm_tools
-Version: 0.21.0
+Version: 0.22.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Maintainer-email: Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: LGPLv3
 Project-URL: Home, https://github.com/deltares/dfm_tools
 Project-URL: Code, https://github.com/deltares/dfm_tools
 Project-URL: Issues, https://github.com/deltares/dfm_tools/issues
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles,modelbuilder
@@ -34,16 +34,16 @@
 Requires-Dist: dask>=2023.9.0
 Requires-Dist: netcdf4>=1.5.4
 Requires-Dist: bottleneck>=1.3.3
 Requires-Dist: xugrid>=0.9.0
 Requires-Dist: cdsapi>=0.6.1
 Requires-Dist: pydap>=3.4.0
 Requires-Dist: erddapy>=2.0.0
-Requires-Dist: copernicusmarine>=1.0.2
-Requires-Dist: rws-ddlpy>=0.3.0
+Requires-Dist: copernicusmarine>=1.1.0
+Requires-Dist: rws-ddlpy>=0.4.0
 Requires-Dist: pooch>=1.1.0
 Requires-Dist: hydrolib-core>=0.7.0
 Requires-Dist: meshkernel>=4.1.0
 Provides-Extra: dev
 Requires-Dist: bump2version>=0.5.11; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `dfm_tools-0.21.0/README.md` & `dfm_tools-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/__init__.py` & `dfm_tools-0.22.0/dfm_tools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 .. include:: ../README.md
 """
 
 __author__ = """Jelmer Veenstra"""
 __email__ = "jelmer.veenstra@deltares.nl"
-__version__ = "0.21.0"
+__version__ = "0.22.0"
 
 from dfm_tools.deprecated import *
 from dfm_tools.download import *
 from dfm_tools.get_nc import *
 from dfm_tools.get_nc_helpers import *
 from dfm_tools.hydrolib_helpers import *
 from dfm_tools.meshkernel_helpers import *
```

### Comparing `dfm_tools-0.21.0/dfm_tools/bathymetry.py` & `dfm_tools-0.22.0/dfm_tools/bathymetry.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/coastlines.py` & `dfm_tools-0.22.0/dfm_tools/coastlines.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/data.py` & `dfm_tools-0.22.0/dfm_tools/data.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/deprecated.py` & `dfm_tools-0.22.0/dfm_tools/deprecated.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/download.py` & `dfm_tools-0.22.0/dfm_tools/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pandas as pd
 from pathlib import Path
 import xarray as xr
 from dfm_tools.errors import OutOfRangeError
 import cdsapi
 import copernicusmarine
+from copernicusmarine.core_functions.credentials_utils import InvalidUsernameOrPassword
 import cftime
 import getpass
 import shutil
 import subprocess
 import sys
 
 __all__ = [
@@ -273,19 +274,31 @@
                 dataset_id = 'cmems_mod_glo_phy-so_anfc_0.083deg_P1D-m'
             elif varkey in ['thetao']:
                 dataset_id = 'cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m'
             else:
                 dataset_id = 'cmems_mod_glo_phy_anfc_0.083deg_P1D-m'
         else: #reanalysis: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/description
             dataset_id = 'cmems_mod_glo_phy_my_0.083deg_P1D-m'
-    else: #for bio (resolution is 1/4 degrees)
+    elif varkey in ['nppv','o2','talk','dissic','ph','spco2','no3','po4','si','fe','chl','phyc']: # for bio
+        # resolution is 1/4 degrees
         if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_BGC_001_028/description
-            dataset_id = 'global-analysis-forecast-bio-001-028-daily'
+            if varkey in ['nppv','o2']:
+                dataset_id = 'cmems_mod_glo_bgc-bio_anfc_0.25deg_P1D-m'
+            elif varkey in ['talk','dissic','ph']:
+                dataset_id = 'cmems_mod_glo_bgc-car_anfc_0.25deg_P1D-m'
+            elif varkey in ['spco2']:
+                dataset_id = 'cmems_mod_glo_bgc-co2_anfc_0.25deg_P1D-m'
+            elif varkey in ['no3','po4','si','fe']:
+                dataset_id = 'cmems_mod_glo_bgc-nut_anfc_0.25deg_P1D-m'
+            elif varkey in ['chl','phyc']:
+                dataset_id = 'cmems_mod_glo_bgc-pft_anfc_0.25deg_P1D-m'
         else: #https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/description
             dataset_id = 'cmems_mod_glo_bgc_my_0.25_P1D-m'
+    else:
+        raise KeyError(f"unknown varkey for cmems: {varkey}")
     return dataset_id
 
 
 def copernicusmarine_get_buffer(dataset_id):
     ds = copernicusmarine.open_dataset(dataset_id=dataset_id)
     try:
         resolution = ds.latitude.attrs["step"]
@@ -300,37 +313,22 @@
     cmems_file_old = os.path.expanduser("~/CMEMS_credentials.txt")
     if os.path.isfile(cmems_file_old):
         os.remove(cmems_file_old)
 
 
 def copernicusmarine_credentials():
     """
-    To login at copernicusmarine if this was not the case yet.
-    If the credentials file is present, the function returns None.
-    If the credentials file is not present, get_and_check_username_password first
-    checks env vars and if not present it prompts the user for credentials.
-    Feeding the returned credentials to copernicusmarine.login() generates the credentials file.
-    If the file is available, it gets the credentials from the file.
-    Either way, the credentials are returned for use in e.g. ftp login
-    """
-    from copernicusmarine.core_functions.credentials_utils import (
-        DEFAULT_CLIENT_CREDENTIALS_FILEPATH,
-        InvalidUsernameOrPassword,
-        get_and_check_username_password,
-    )
-    login_kwargs = dict(username=None, password=None, credentials_file=DEFAULT_CLIENT_CREDENTIALS_FILEPATH, no_metadata_cache=False)
-    if not DEFAULT_CLIENT_CREDENTIALS_FILEPATH.is_file():
-        print("Downloading CMEMS data requires a Copernicus Marine username and password, sign up for free at: https://data.marine.copernicus.eu/register.")
-        username, password = get_and_check_username_password(**login_kwargs)
-        success = copernicusmarine.login(username, password)
-        if not success:
-            raise InvalidUsernameOrPassword("invalid credentials")
-    else:
-        username, password = get_and_check_username_password(**login_kwargs)
-    return username, password
+    Login at copernicusmarine if user not logged in yet.
+    Works via prompt, environment variables or credentials file.
+    """
+    print("Downloading CMEMS data requires a Copernicus Marine username and password, "
+          "sign up for free at: https://data.marine.copernicus.eu/register.")
+    success = copernicusmarine.login(skip_if_user_logged_in=True)
+    if not success:
+        raise InvalidUsernameOrPassword("Invalid credentials, please try again")
 
 
 def copernicusmarine_reset(remove_folder=False, overwrite_cache=True, update_package=False):
     if remove_folder:
         dir_copernicusmarine = os.path.expanduser("~/.copernicusmarine")
         print(f"reset copernicusmarine: removing {dir_copernicusmarine}, you will have to login again.")
         shutil.rmtree(dir_copernicusmarine, ignore_errors=True)
```

### Comparing `dfm_tools-0.21.0/dfm_tools/energy_dissipation.py` & `dfm_tools-0.22.0/dfm_tools/energy_dissipation.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/get_nc.py` & `dfm_tools-0.22.0/dfm_tools/get_nc.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/get_nc_helpers.py` & `dfm_tools-0.22.0/dfm_tools/get_nc_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/hydrolib_helpers.py` & `dfm_tools-0.22.0/dfm_tools/hydrolib_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/interpolate_grid2bnd.py` & `dfm_tools-0.22.0/dfm_tools/interpolate_grid2bnd.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/linebuilder.py` & `dfm_tools-0.22.0/dfm_tools/linebuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/meshkernel_helpers.py` & `dfm_tools-0.22.0/dfm_tools/meshkernel_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/modelbuilder.py` & `dfm_tools-0.22.0/dfm_tools/modelbuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/modplot.py` & `dfm_tools-0.22.0/dfm_tools/modplot.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/observations.py` & `dfm_tools-0.22.0/dfm_tools/observations.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,35 @@
 import numpy as np
 from urllib.request import urlopen
 import unicodedata
 import geopandas as gpd
 from shapely import Point
 import os
 import xarray as xr
-from ftplib import FTP
 from dfm_tools.download import copernicusmarine_credentials
+from dfm_tools.data import get_dir_testdata
 from erddapy import ERDDAP
 import requests
 from zipfile import ZipFile
 from io import BytesIO
 import functools
 import tempfile
 import ddlpy
+import glob
+import matplotlib.pyplot as plt
+import matplotlib.dates as md
+import shutil
+import fiona
+import copernicusmarine
 
 __all__ = ["ssh_catalog_subset",
            "ssh_catalog_toxynfile",
+           "ssh_catalog_tokmlfile",
            "ssh_retrieve_data",
+           "ssh_netcdf_overview",
            ]
 
 
 def _make_hydrotools_consistent(ds):
     """
     to make resulting netcdf file consistent with hydro_tools matlab post-processing
     """
@@ -187,57 +195,63 @@
             ssc_catalog_gpd.loc[station_ssc_id,'dist_dict'] = [station_check_dict]
             ssc_catalog_gpd.loc[station_ssc_id,'dist_min'] = np.min(station_check_dist_all)
             ssc_catalog_gpd.loc[station_ssc_id,'dist_max'] = np.max(station_check_dist_all)
 
     return ssc_catalog_gpd
 
 
-def get_cmems_params(source):
-    params_cmems_my = {"host": "my.cmems-du.eu",
-                       "cwd": "Core/INSITU_GLO_PHY_SSH_DISCRETE_MY_013_053/cmems_obs-ins_glo_phy-ssh_my_na_PT1H"}
-    params_cmems_nrt = {"host": "nrt.cmems-du.eu",
-                        "cwd": "Core/INSITU_GLO_PHYBGCWAV_DISCRETE_MYNRT_013_030/cmems_obs-ins_glo_phybgcwav_mynrt_na_irr"}
-    params_dict = {"cmems": params_cmems_my,
-                   "cmems-nrt": params_cmems_nrt}
-    params = params_dict[source]
-    return params
+def get_cmems_dataset_id(source):
+    dataset_id_dict = {"cmems": "cmems_obs-ins_glo_phy-ssh_my_na_PT1H",
+                       "cmems-nrt": "cmems_obs-ins_glo_phybgcwav_mynrt_na_irr"}
+    dataset_id = dataset_id_dict[source]
+    return dataset_id
 
 
-def cmems_my_ssh_read_catalog():
-    cmems_catalog_gpd = cmems_ssh_read_catalog(source="cmems")
+def cmems_my_ssh_read_catalog(overwrite=True):
+    cmems_catalog_gpd = cmems_ssh_read_catalog(source="cmems", overwrite=overwrite)
     return cmems_catalog_gpd
     
 
-def cmems_nrt_ssh_read_catalog():
-    cmems_catalog_gpd = cmems_ssh_read_catalog(source="cmems-nrt")
+def cmems_nrt_ssh_read_catalog(overwrite=True):
+    cmems_catalog_gpd = cmems_ssh_read_catalog(source="cmems-nrt", overwrite=overwrite)
     return cmems_catalog_gpd
 
 
-def cmems_ssh_read_catalog(source):
-    cmems_params = get_cmems_params(source)
+def cmems_ssh_read_catalog(source, overwrite=True):
+    dataset_id = get_cmems_dataset_id(source)
+    
+    dir_cache = get_dir_testdata()
+    dir_index = os.path.join(dir_cache, dataset_id)
+    os.makedirs(dir_index, exist_ok=True)
+    file_index = os.path.join(dir_index, 'index_history.txt')
+    
+    if not os.path.exists(file_index) or overwrite:
+        #TODO: downloading all index files since filter does not work, can be avoided?
+        copernicusmarine_credentials()
+        copernicusmarine.get(
+            dataset_id=dataset_id,
+            service="files",
+            index_parts=True,
+            filter="*index_history.txt",
+            output_directory=dir_index,
+            overwrite_output_data=True,
+            force_download=True,
+            no_directories=True,
+            )
+    else:
+        print(f"CMEMS insitu catalog for dataset_id='{dataset_id}' is already present and overwrite=False")
     
-    # setup ftp connection
-    ftp = FTP(host=cmems_params["host"])
-    username, password = copernicusmarine_credentials()
-    ftp.login(user=username, passwd=password)
-    ftp.cwd(cmems_params["cwd"])
-    
-    # read index
-    fname = 'index_history.txt'
-    with open(fname, 'wb') as fp:
-        ftp.retrbinary(f'RETR {fname}', fp.write)
-    with open(fname, 'r') as f:
+    with open(file_index, 'r') as f:
         for line in f:
             if line.startswith('#'):
                 header = line
             else:
                 break #stop when there are no more #
     colnames = header.strip('#').strip().split(',')
-    index_history_pd = pd.read_csv(fname,comment='#',names=colnames)
-    os.remove(fname) # remove the local file again
+    index_history_pd = pd.read_csv(file_index,comment='#',names=colnames)
     
     # filter only history tidegauges (TG) containing SLEV variable, relevant for nrt dataset
     # TODO: why are there non-SLEV files in TG folder? Cleanup possible?
     bool_tidegauge = index_history_pd["file_name"].str.contains("/history/TG/")
     bool_slev = index_history_pd["parameters"].str.contains("SLEV")
     index_history_pd = index_history_pd.loc[bool_tidegauge & bool_slev]
     
@@ -527,51 +541,55 @@
     ddl_slev_gdf["station_name_unique"] = ddl_slev_gdf["Code"]
     ddl_slev_gdf["station_id"] = ddl_slev_gdf["Code"]
     ddl_slev_gdf["country"] = "NLD"
     
     return ddl_slev_gdf
 
 
-@functools.lru_cache
-def cmems_ftp_login(host, dir_data):
-    """
-    cache ftp connection so it does not matter that we call it for each station
-    """
-    # setup ftp connection
-    ftp = FTP(host=host)
-    username, password = copernicusmarine_credentials()
-    ftp.login(user=username, passwd=password)
-    ftp.cwd(dir_data)
-    return ftp
-
-
-def cmems_ssh_retrieve_data(row, dir_output, time_min=None, time_max=None):
+def cmems_ssh_retrieve_data(row, dir_output, time_min=None, time_max=None, 
+                            level="WARNING", disable_progress_bar=True):
     """
-    Retrieve data from FTP
+    Retrieve data from copernicusmarine files service
     Can only retrieve entire files, subsetting is done during reconstruction
     
+    Sometimes the process hangs when using disable_progress_bar=True
     """
     
-    # get source from gdf, uniqueness is checked in ssh_retrieve_data
+    # get source from gdf
     source = row['source']
-    cmems_params = get_cmems_params(source)
+    dataset_id = get_cmems_dataset_id(source)
 
-    # get cached ftp connection
-    host = cmems_params["host"]
-    dir_data = os.path.dirname(row["file_name"]).split(host)[1]
-    ftp = cmems_ftp_login(host, dir_data)
-    
-    fname = os.path.basename(row["file_name"])
     tempdir = tempfile.gettempdir()
-    fname_out_raw = os.path.join(tempdir, "dfmtools_cmems_ssh_retrieve_data_temporary_file.nc")
-    with open(fname_out_raw, 'wb') as fp:
-        ftp.retrbinary(f'RETR {fname}', fp.write)
+    url_file = row["file_name"]
+    
+    copernicusmarine_credentials()
+    
+    import logging
+    logging.getLogger("copernicus_marine_root_logger").setLevel(level)
+    copernicusmarine.get(
+        dataset_id=dataset_id,
+        dataset_part="history",
+        service="files",
+        filter=url_file,
+        output_directory=tempdir,
+        overwrite_output_data=True,
+        force_download=True,
+        no_directories=True,
+        disable_progress_bar=disable_progress_bar,
+        )
+    
+    file_data_org = os.path.join(tempdir, os.path.basename(url_file))
+    random_suffix = str(pd.Timestamp.now().microsecond)[0]
+    file_data_raw = os.path.join(tempdir, f"dfmtools_cmems_ssh_retrieve_data_temporary_file_{random_suffix}.nc")
+    if os.path.exists(file_data_raw):
+        os.remove(file_data_raw)
+    os.rename(file_data_org, file_data_raw)
     
     # reconstruct this dataset (including time subsetting) and write again
-    ds = xr.open_dataset(fname_out_raw)
+    ds = xr.open_dataset(file_data_raw)
     
     # reduce DEPTH dimension if present (nrt dataset)
     if "DEPTH" in ds.dims:
         ds = ds.max(dim="DEPTH", keep_attrs=True)
 
     ds = ds.rename(TIME="time")
     
@@ -585,24 +603,24 @@
     # check order of time variable
     if not ds.time.to_pandas().index.is_monotonic_increasing:
         # TODO: happens in some MO_TS_TG_RMN-* stations in NRT dataset, asked to fix
         # Genova, Imperia, LaSpezia, Livorno, Ravenna, Venice
         stat_name = row.loc["station_name_unique"]
         print(f"[{stat_name} NOT MONOTONIC] ", end="")
         del ds
-        os.remove(fname_out_raw)
+        os.remove(file_data_raw)
         return
         # ds = ds.sortby("time")
     
     # slice on time extent
     ds = ds.sel(time=slice(time_min, time_max))
     if len(ds.time) == 0:
         print("[NODATA] ", end="")
         del ds
-        os.remove(fname_out_raw)
+        os.remove(file_data_raw)
         return
     
     return ds
 
 
 def uhslc_ssh_retrieve_data(row, dir_output, time_min=None, time_max=None):
     
@@ -788,58 +806,59 @@
 
     ds = ds.sel(time=slice(time_min, time_max))
     if len(ds.time) == 0:
         return
     return ds
 
 
-def rwsddl_ssh_retrieve_data(row, dir_output, time_min, time_max, meta_dict=None):
+def rwsddl_ssh_retrieve_data(row, dir_output, time_min, time_max):
     
     if time_min is None or time_max is None:
         raise ValueError("cannot supply None for 'time_min' or 'time_max' to 'rwsddl_ssh_retrieve_data()'")
-
-    if meta_dict is None:
-        meta_dict = rwsddl_ssh_meta_dict()
     
     # if we pass one row to the measurements function you can get all the measurements
     measurements = ddlpy.measurements(row, time_min, time_max)
     
     if measurements.empty:
         # no output so this station is skipped
         return
     
-    # drop alfanumeriek if duplicate of numeriek
-    if "Meetwaarde.Waarde_Alfanumeriek" in measurements.columns and 'Meetwaarde.Waarde_Numeriek' in measurements.columns:
-        measurements = measurements.drop("Meetwaarde.Waarde_Alfanumeriek", axis=1)
+    # minimize disk usage of StatuswaardeLijst by converting to U1
+    varn_status = "WaarnemingMetadata.StatuswaardeLijst"
+    status_dict = {"O":"Ongecontroleerd",
+                   "G":"Gecontroleerd",
+                   "D":"Definitief"}
+    for k,v in status_dict.items():
+        measurements[varn_status] = measurements[varn_status].str.replace(v, k)
+    
+    # convert to xarray (dropping some constant columns)
+    drop_if_constant = ["WaarnemingMetadata.OpdrachtgevendeInstantieLijst",
+                        "WaarnemingMetadata.BemonsteringshoogteLijst",
+                        "WaarnemingMetadata.ReferentievlakLijst",
+                        "AquoMetadata_MessageID", 
+                        "BioTaxonType", 
+                        "BemonsteringsSoort.Code", 
+                        "Compartiment.Code", "Eenheid.Code", "Grootheid.Code", "Hoedanigheid.Code",
+                        "WaardeBepalingsmethode.Code", "MeetApparaat.Code",
+                        ]
+    ds = ddlpy.dataframe_to_xarray(measurements, drop_if_constant)
+    
+    ds[varn_status] = ds[varn_status].assign_attrs(status_dict)
     
     rename_dict = {'Meetwaarde.Waarde_Numeriek':'waterlevel',
-                   'WaarnemingMetadata.KwaliteitswaardecodeLijst':'QC',
-                   'WaarnemingMetadata.StatuswaardeLijst':'Status'}
-    measurements = measurements.rename(columns=rename_dict)
-    
-    # simplify dataframe
-    simplified = ddlpy.simplify_dataframe(measurements)
-    
-    # get dataframe attrs
-    ds_attrs = simplified.attrs
-    # drop irrelevant attrs
-    ds_attrs = {k:v for k,v in ds_attrs.items() if not k.startswith("Bemonstering") and not k.startswith("BioTaxon")}
-    
-    # dropping timezone is required to get proper encoding in time variable (in netcdf file)
-    simplified.index = simplified.index.tz_convert(None)
-    ds = simplified.to_xarray()
-    ds = ds.assign_attrs(ds_attrs)
+                   'WaarnemingMetadata.KwaliteitswaardecodeLijst':'qc',
+                   'WaarnemingMetadata.StatuswaardeLijst':'status'}
+    ds = ds.rename_vars(rename_dict)
     
     # convert meters to cm
-    if ds_attrs['Eenheid.Code'] != 'cm':
+    eenheid = ds.attrs.pop('Eenheid.Code')
+    if eenheid != 'cm':
         raise Exception("unexpected unit")
     ds['waterlevel'] = ds['waterlevel'].assign_attrs(units="m")
     ds['waterlevel'] /= 100 #convert from cm to m
-    ds.attrs.pop('Eenheid.Code')
-    ds.attrs.pop('Eenheid.Omschrijving')
     return ds
 
 
 def ssh_catalog_subset(source=None,
                        lon_min=-180, lon_max=180, 
                        lat_min=-90, lat_max=90, 
                        time_min=None, time_max=None,
@@ -879,22 +898,14 @@
         intime_bool = ((ssh_catalog_gpd['time_min']<time_max) &
                        (ssh_catalog_gpd['time_max']>time_min)
                        )
         ssh_catalog_gpd = ssh_catalog_gpd.loc[intime_bool].copy()
     return ssh_catalog_gpd
 
 
-def ssh_catalog_toxynfile(ssc_catalog_gpd, file_xyn):
-    lon = ssc_catalog_gpd.geometry.x
-    lat = ssc_catalog_gpd.geometry.y
-    name = ssc_catalog_gpd['station_name_unique']
-    data = np.c_[lon, lat, name]
-    np.savetxt(file_xyn, data, fmt='%11.6f %11.6f %-s')
-
-
 def ssh_retrieve_data(ssh_catalog_gpd, dir_output, time_min=None, time_max=None,
                       **kwargs):
     
     if ssh_catalog_gpd.empty:
         raise ValueError("empty ssh_catalog_gpd provided to ssh_retrieve_data")
     
     source_list = ssh_catalog_gpd["source"].unique()
@@ -912,14 +923,15 @@
                    "rwsddl": rwsddl_ssh_retrieve_data,
                    }
     
     if source not in ssh_sources.keys():
         raise ValueError(f"source for ssh_retrieve_data should be one of {list(ssh_sources.keys())}, recieved '{source}'")
     
     retrieve_data_func = ssh_sources[source]
+    os.makedirs(dir_output, exist_ok=True)
     
     # retrieve
     print(f"retrieving data for {len(ssh_catalog_gpd)} {source} stations:", end=" ")
     for idx_arbitrary, row in ssh_catalog_gpd.iterrows():
         irow = ssh_catalog_gpd.index.tolist().index(idx_arbitrary)
         print(irow+1, end=" ")
         ds = retrieve_data_func(row, dir_output, time_min=time_min, time_max=time_max, **kwargs)
@@ -928,19 +940,150 @@
             continue
         
         # assign attrs from station catalog row
         ds = ds.assign_attrs(station_name=row["station_name"],
                              station_id=row["station_id"],
                              station_name_unique=row["station_name_unique"],
                              longitude=row.geometry.x,
-                             latitude=row.geometry.x,
+                             latitude=row.geometry.y,
                              country=row["country"])
         
         ds["waterlevel"] = ds["waterlevel"].astype("float32")
         _make_hydrotools_consistent(ds)
         
         stat_name = ds.attrs["station_name_unique"]
         file_out = os.path.join(dir_output, f"{stat_name}.nc")
         ds.to_netcdf(file_out)
         del ds
     print()
 
+
+def ssh_catalog_toxynfile(ssc_catalog_gpd, file_xyn):
+    """
+    converts a ssh_catalog to a _obs.xyn file for easy visualisation in FM GUI and interacter
+    """
+    lon = ssc_catalog_gpd.geometry.x
+    lat = ssc_catalog_gpd.geometry.y
+    name = ssc_catalog_gpd['station_name_unique']
+    data = np.c_[lon, lat, name]
+    np.savetxt(file_xyn, data, fmt='%13.8f %13.8f %-s')
+
+
+def ssh_catalog_tokmlfile(ssc_catalog_gpd, file_kml):
+    """
+    converts a ssh_catalog to a kml file for easy visualisation in google earth
+    """
+    # Enable fiona driver
+    # TODO: gpd sometimes fails with "AttributeError: 'NoneType' object has no attribute 'drvsupport'" 
+    # gpd.io.file.fiona.drvsupport.supported_drivers['KML'] = 'rw' # 
+    # gpd.io.file.fiona.drvsupport.supported_drivers['LIBKML'] = 'rw'
+    fiona.supported_drivers['KML'] = 'rw'
+    fiona.supported_drivers['LIBKML'] = 'rw'
+    
+    #select only names and geometry column to reduce file size
+    ssc_catalog_gpd_minimal = ssc_catalog_gpd[["station_name_unique","geometry"]]
+    # rename to "name" results in a label in Google Earth
+    ssc_catalog_gpd_minimal = ssc_catalog_gpd_minimal.rename({"station_name_unique":"name"},axis=1)
+    
+    # Write file
+    ssc_catalog_gpd_minimal.to_file(file_kml, driver='KML')
+
+
+def ssh_netcdf_overview(dir_netcdf, perplot=30, time_min=None, time_max=None, yearstep=None):
+    """
+    reads all netcdf files in a directory and makes figures of the non-nan waterlevel time availability
+    it also writes a csv file with statistics
+    """
+    dir_output = os.path.join(dir_netcdf, "overview")
+    if os.path.isdir(dir_output):
+        shutil.rmtree(dir_output)
+    os.makedirs(dir_output, exist_ok=False)
+    
+    file_list = glob.glob(os.path.join(dir_netcdf, "*.nc"))
+    file_list = sorted(file_list, key=str.casefold)
+    
+    print(f"creating overview for {len(file_list)} files: ", end="")
+    fig, ax = plt.subplots(figsize=(15,8))
+    stats_list = []
+    fig_file_list = []
+    for ifile, file_nc in enumerate(file_list):
+        
+        fname = os.path.basename(file_nc)
+        print(f"{ifile+1} ", end="")
+        
+        ds = xr.open_dataset(file_nc)
+        ds = ds.sortby("time") # necessary for BODC data
+        
+        fname_clean = fname.replace(".nc","")
+        longitude = float(ds.station_x_coordinate)
+        latitude = float(ds.station_y_coordinate)
+        
+        fig_file_list.append(fname_clean)
+        
+        # stats
+        ds_ndays = round(int(ds.time.max() - ds.time.min())/1e9/3600/24, 2)
+        nvalues = len(ds.waterlevel)
+        nnan = int(ds.waterlevel.isnull().sum())
+        time_diff_min = ds.time.to_pandas().diff().dt.total_seconds()/60
+        
+        stats_one = {"fname_clean":fname_clean,
+                     "longitude":longitude,
+                     "latitude":latitude,
+                     "tstart":str(ds.time[0].dt.strftime("%Y-%m-%d").values),
+                     "tstop":str(ds.time[-1].dt.strftime("%Y-%m-%d").values),
+                     "ndays": ds_ndays,
+                     "#values": nvalues,
+                     "#nan": nnan,
+                     "%nan": (nnan/nvalues)*100,
+                     "dt min [min]":int(time_diff_min.min()),
+                     "dt max [min]":int(time_diff_min.max()),
+                     "dt mean [min]":time_diff_min.mean(),
+                     "dt mode [min]":time_diff_min.mode().iloc[0],
+                     "ndupl": ds.time.to_pandas().duplicated().sum(),
+                     "min": float(ds.waterlevel.min()),
+                     "max": float(ds.waterlevel.max()),
+                     }
+        stats_one_pd = pd.DataFrame(stats_one, index=[fname])
+        stats_list.append(stats_one_pd)
+        
+        # derive unique hourly times with non-nan values
+        bool_nan = ds.waterlevel.isnull()
+        ds_nonan = ds.sel(time=~bool_nan)
+        ds_slice = ds_nonan.sel(time=slice(time_min, time_max))
+        # take unique timestamps after rounding to hours, this is faster and consumes less memory
+        time_hr_uniq = ds_slice.time.to_pandas().index.round("H").drop_duplicates()
+        time_yaxis_value = pd.Series(index=time_hr_uniq)
+        time_yaxis_value[:] = -(ifile%perplot)
+        time_yaxis_value.plot(ax=ax, marker='s', linestyle='none', markersize=1, color="r")
+        
+        # clear file links
+        del ds
+        
+        bool_lastinrange = (ifile%perplot) == (perplot-1)
+        bool_lastfile = ifile == (len(file_list)-1)
+        if bool_lastinrange | bool_lastfile:
+            # finish and save figure
+            nlines = len(fig_file_list)
+            ax.set_yticks(range(0,-nlines,-1), fig_file_list)
+            figname = f"overview_availability_{ifile-nlines+2:03d}_{ifile+1:03d}"
+            ax.set_xlim(time_min, time_max)
+            if yearstep is not None:
+                # set xtick steps
+                ax.xaxis.set_major_locator(md.YearLocator(base=yearstep))
+                ax.xaxis.set_major_formatter(md.DateFormatter('%Y'))
+            ax.grid()
+            ax.set_xlabel(None)
+            fig.tight_layout()
+            fig.savefig(os.path.join(dir_output, figname), dpi=200)
+        
+        if bool_lastinrange:
+            # reset figure
+            ax.cla()
+            fig_file_list = []
+    print()
+    
+    # write statistics csv
+    stats = pd.concat(stats_list)
+    stats.index.name = "file_name"
+    file_csv = os.path.join(dir_output, "waterlevel_data_netcdf_overview.csv")
+    stats.to_csv(file_csv, float_format="%.2f")
+
```

### Comparing `dfm_tools-0.21.0/dfm_tools/xarray_helpers.py` & `dfm_tools-0.22.0/dfm_tools/xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools/xugrid_helpers.py` & `dfm_tools-0.22.0/dfm_tools/xugrid_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/dfm_tools.egg-info/PKG-INFO` & `dfm_tools-0.22.0/dfm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfm_tools
-Version: 0.21.0
+Version: 0.22.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Maintainer-email: Jelmer Veenstra <jelmer.veenstra@deltares.nl>
 License: LGPLv3
 Project-URL: Home, https://github.com/deltares/dfm_tools
 Project-URL: Code, https://github.com/deltares/dfm_tools
 Project-URL: Issues, https://github.com/deltares/dfm_tools/issues
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles,modelbuilder
@@ -34,16 +34,16 @@
 Requires-Dist: dask>=2023.9.0
 Requires-Dist: netcdf4>=1.5.4
 Requires-Dist: bottleneck>=1.3.3
 Requires-Dist: xugrid>=0.9.0
 Requires-Dist: cdsapi>=0.6.1
 Requires-Dist: pydap>=3.4.0
 Requires-Dist: erddapy>=2.0.0
-Requires-Dist: copernicusmarine>=1.0.2
-Requires-Dist: rws-ddlpy>=0.3.0
+Requires-Dist: copernicusmarine>=1.1.0
+Requires-Dist: rws-ddlpy>=0.4.0
 Requires-Dist: pooch>=1.1.0
 Requires-Dist: hydrolib-core>=0.7.0
 Requires-Dist: meshkernel>=4.1.0
 Provides-Extra: dev
 Requires-Dist: bump2version>=0.5.11; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `dfm_tools-0.21.0/dfm_tools.egg-info/SOURCES.txt` & `dfm_tools-0.22.0/dfm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/pyproject.toml` & `dfm_tools-0.22.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfm_tools"
-version = "0.21.0"
+version = "0.22.0"
 maintainers = [{ name = "Jelmer Veenstra", email = "jelmer.veenstra@deltares.nl" }]
 description = "dfm_tools are pre- and post-processing tools for Delft3D FM"
 readme = "README.md"
 keywords = ["dfm_tools", "D-FlowFM", "D-HYDRO", "post-processing", "pre-processing", "mapfiles", "hisfiles", "modelbuilder"]
 license = { text = "LGPLv3" }
 requires-python = ">=3.9"
 dependencies = [
@@ -40,18 +40,18 @@
 	"xugrid>=0.9.0",
 	#cdsapi<0.6.1 is from Feb 2021 and does not support newer python versions
 	"cdsapi>=0.6.1",
 	#pydap<3.4.0 is from May 2017 and does not support newer python versions
 	"pydap>=3.4.0",
 	#erddapy<2.0.0 does not support pandas>=2.0.0
 	"erddapy>=2.0.0",
-	#copernicusmarine<1.0.2 does not support no_metadata_cache in get_and_check_username_password function
-	"copernicusmarine>=1.0.2",
-	#rws-ddlpy<0.3.0 is very old and does not support newer pandas versions
-	"rws-ddlpy>=0.3.0",
+	#copernicusmarine<1.1.0 does not support insitu data via files service and does not check credentials upon login
+	"copernicusmarine>=1.1.0",
+	#rws-ddlpy<0.4.0 does not yet have `ddlpy.dataframe_to_xarray()`
+	"rws-ddlpy>=0.4.0",
 	#pooch<1.1.0 do not have attribute retrieve
 	"pooch>=1.1.0",
 	#hydrolib-core 0.7.0 supports meshkernel>=4.1.0
 	"hydrolib-core>=0.7.0",
 	#meshkernel<4.1.0 does not support contacts_get, no macos support, etc
 	"meshkernel>=4.1.0",
 ]
```

### Comparing `dfm_tools-0.21.0/tests/test_bathymetry.py` & `dfm_tools-0.22.0/tests/test_bathymetry.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_coastlines.py` & `dfm_tools-0.22.0/tests/test_coastlines.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_data.py` & `dfm_tools-0.22.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_dfm_tools.py` & `dfm_tools-0.22.0/tests/test_dfm_tools.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_download.py` & `dfm_tools-0.22.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_examples.py` & `dfm_tools-0.22.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_external_packages.py` & `dfm_tools-0.22.0/tests/test_external_packages.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_get_nc.py` & `dfm_tools-0.22.0/tests/test_get_nc.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_hydrolib_helpers.py` & `dfm_tools-0.22.0/tests/test_hydrolib_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_interpolate_grid2bnd.py` & `dfm_tools-0.22.0/tests/test_interpolate_grid2bnd.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_meshkernel_helpers.py` & `dfm_tools-0.22.0/tests/test_meshkernel_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_modelbuilder.py` & `dfm_tools-0.22.0/tests/test_modelbuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_observations.py` & `dfm_tools-0.22.0/tests/test_observations.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,17 +67,14 @@
     # ssc does not contain data, only station locations, so early return
     if source=="ssc":
         return
     
     if source=="uhslc-rqds":
         # 2020 not available in uhslc-rqds yet
         time_min, time_max = '2018-01-01','2018-02-01'
-    elif source=="rwsddl":
-        #TODO: temporarily more recent period since ddl data is being replaced
-        time_min, time_max = '2023-01-01','2023-02-01'
     else:
         time_min, time_max = '2020-01-01','2020-02-01'
     
     ssc_catalog_gpd = dfmt.ssh_catalog_subset(source=source)
     if source=="rwsddl":
         # order of rows in rwsddl locations dataframe is python-version-dependent
         # make sure we always test on the same hist station (no realtime data)
@@ -94,14 +91,35 @@
     dfmt.ssh_retrieve_data(ssc_catalog_gpd_sel, dir_output=tmp_path, 
                            time_min=time_min, time_max=time_max)
     nc_list = glob.glob(os.path.join(tmp_path, "*.nc"))
     assert len(nc_list)==1
 
 
 @pytest.mark.unittest
+def test_ssh_netcdf_overview(tmp_path):
+    source = "rwsddl"
+    time_min, time_max = '2020-01-01','2020-01-05'
+    
+    ssc_catalog_gpd = dfmt.ssh_catalog_subset(source=source)
+    
+    # order of rows in rwsddl locations dataframe is python-version-dependent
+    # make sure we always test on the same hist station (no realtime data)
+    bool_hoekvhld = ssc_catalog_gpd["Code"].isin(["HOEKVHLD"])
+    ssc_catalog_gpd_sel = ssc_catalog_gpd.loc[bool_hoekvhld]
+    
+    dfmt.ssh_retrieve_data(ssc_catalog_gpd_sel, dir_output=tmp_path, 
+                           time_min=time_min, time_max=time_max)
+    
+    dfmt.ssh_netcdf_overview(tmp_path)
+    assert os.path.isdir(os.path.join(tmp_path, "overview"))
+    assert os.path.isfile(os.path.join(tmp_path, "overview", "overview_availability_001_001.png"))
+    assert os.path.isfile(os.path.join(tmp_path, "overview", "waterlevel_data_netcdf_overview.csv"))
+
+
+@pytest.mark.unittest
 def test_rwsddl_ssh_get_time_max():
     locations = ddlpy.locations()
     bool_hoedanigheid = locations['Hoedanigheid.Code'].isin(['NAP'])
     bool_stations = locations.index.isin(['HOEKVHLD', 'IJMDBTHVN','SCHEVNGN'])
     bool_grootheid = locations['Grootheid.Code'].isin(['WATHTE'])
     bool_groepering = locations['Groepering.Code'].isin(['NVT'])
     selected = locations.loc[bool_grootheid & bool_hoedanigheid & bool_groepering & bool_stations]
@@ -129,7 +147,15 @@
 @pytest.mark.unittest
 def test_ssh_catalog_toxynfile(tmp_path):
     ssc_catalog_gpd = dfmt.ssh_catalog_subset(source="ssc")
     file_xyn = tmp_path / 'test_ssc_obs.xyn'
     dfmt.ssh_catalog_toxynfile(ssc_catalog_gpd, file_xyn)
     assert os.path.isfile(file_xyn)
 
+
+@pytest.mark.unittest
+def test_ssh_catalog_tokmlfile(tmp_path):
+    ssc_catalog_gpd = dfmt.ssh_catalog_subset(source="ssc")
+    file_xyn = tmp_path / 'test_ssc.kml'
+    dfmt.ssh_catalog_tokmlfile(ssc_catalog_gpd, file_xyn)
+    assert os.path.isfile(file_xyn)
+
```

### Comparing `dfm_tools-0.21.0/tests/test_xarray_helpers.py` & `dfm_tools-0.22.0/tests/test_xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.21.0/tests/test_xugrid_helpers.py` & `dfm_tools-0.22.0/tests/test_xugrid_helpers.py`

 * *Files identical despite different names*

