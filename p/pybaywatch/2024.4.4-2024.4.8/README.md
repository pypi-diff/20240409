# Comparing `tmp/pybaywatch-2024.4.4.tar.gz` & `tmp/pybaywatch-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaywatch-2024.4.4.tar", last modified: Fri Apr  5 00:41:37 2024, max compression
+gzip compressed data, was "pybaywatch-2024.4.8.tar", last modified: Tue Apr  9 19:08:44 2024, max compression
```

## Comparing `pybaywatch-2024.4.4.tar` & `pybaywatch-2024.4.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:41:37.238664 pybaywatch-2024.4.4/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2024-03-17 02:29:06.000000 pybaywatch-2024.4.4/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       33 2024-03-17 18:02:15.000000 pybaywatch-2024.4.4/MANIFEST.in
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      481 2024-04-05 00:41:37.236826 pybaywatch-2024.4.4/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       32 2024-03-17 02:29:06.000000 pybaywatch-2024.4.4/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:41:37.228649 pybaywatch-2024.4.4/pybaywatch/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3119 2024-03-27 06:04:37.000000 pybaywatch-2024.4.4/pybaywatch/TEX_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1717 2024-03-28 04:18:11.000000 pybaywatch-2024.4.4/pybaywatch/UK_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      276 2024-03-28 04:36:12.000000 pybaywatch-2024.4.4/pybaywatch/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2131 2024-03-28 04:25:40.000000 pybaywatch-2024.4.4/pybaywatch/bayfox_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7017 2024-03-29 01:14:10.000000 pybaywatch-2024.4.4/pybaywatch/baymag_forward_ln.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2824 2024-03-28 03:57:42.000000 pybaywatch-2024.4.4/pybaywatch/baymbt_forward.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12833 2024-04-04 23:45:06.000000 pybaywatch-2024.4.4/pybaywatch/core.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      461 2024-03-24 20:42:45.000000 pybaywatch-2024.4.4/pybaywatch/fnval.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1256 2024-03-17 16:27:16.000000 pybaywatch-2024.4.4/pybaywatch/normrnd.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     4622 2024-03-24 20:43:51.000000 pybaywatch-2024.4.4/pybaywatch/randsample.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7777 2024-03-17 16:38:54.000000 pybaywatch-2024.4.4/pybaywatch/rndcheck.m
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2960 2024-03-24 20:59:29.000000 pybaywatch-2024.4.4/pybaywatch/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3900 2024-03-29 01:12:36.000000 pybaywatch-2024.4.4/pybaywatch/wrapper.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:41:37.235517 pybaywatch-2024.4.4/pybaywatch.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      481 2024-04-05 00:41:37.229673 pybaywatch-2024.4.4/pybaywatch.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      546 2024-04-05 00:41:37.230452 pybaywatch-2024.4.4/pybaywatch.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-05 00:41:37.232131 pybaywatch-2024.4.4/pybaywatch.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-03-17 02:47:06.000000 pybaywatch-2024.4.4/pybaywatch.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       16 2024-04-05 00:41:37.234371 pybaywatch-2024.4.4/pybaywatch.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       11 2024-04-05 00:41:37.235621 pybaywatch-2024.4.4/pybaywatch.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-05 00:41:37.238788 pybaywatch-2024.4.4/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      762 2024-04-05 00:41:15.000000 pybaywatch-2024.4.4/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-09 19:08:44.815387 pybaywatch-2024.4.8/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2024-03-17 02:29:06.000000 pybaywatch-2024.4.8/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       33 2024-03-17 18:02:15.000000 pybaywatch-2024.4.8/MANIFEST.in
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3187 2024-04-09 19:08:44.814400 pybaywatch-2024.4.8/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2719 2024-04-09 19:06:14.000000 pybaywatch-2024.4.8/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-09 19:08:44.809687 pybaywatch-2024.4.8/pybaywatch/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3119 2024-03-27 06:04:37.000000 pybaywatch-2024.4.8/pybaywatch/TEX_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1717 2024-03-28 04:18:11.000000 pybaywatch-2024.4.8/pybaywatch/UK_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      276 2024-03-28 04:36:12.000000 pybaywatch-2024.4.8/pybaywatch/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2131 2024-03-28 04:25:40.000000 pybaywatch-2024.4.8/pybaywatch/bayfox_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7017 2024-03-29 01:14:10.000000 pybaywatch-2024.4.8/pybaywatch/baymag_forward_ln.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2824 2024-03-28 03:57:42.000000 pybaywatch-2024.4.8/pybaywatch/baymbt_forward.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12763 2024-04-09 18:58:59.000000 pybaywatch-2024.4.8/pybaywatch/core.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      461 2024-03-24 20:42:45.000000 pybaywatch-2024.4.8/pybaywatch/fnval.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1256 2024-03-17 16:27:16.000000 pybaywatch-2024.4.8/pybaywatch/normrnd.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     4622 2024-03-24 20:43:51.000000 pybaywatch-2024.4.8/pybaywatch/randsample.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7777 2024-03-17 16:38:54.000000 pybaywatch-2024.4.8/pybaywatch/rndcheck.m
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2960 2024-03-24 20:59:29.000000 pybaywatch-2024.4.8/pybaywatch/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3822 2024-04-09 18:58:59.000000 pybaywatch-2024.4.8/pybaywatch/wrapper.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-09 19:08:44.813619 pybaywatch-2024.4.8/pybaywatch.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3187 2024-04-09 19:08:44.810350 pybaywatch-2024.4.8/pybaywatch.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      546 2024-04-09 19:08:44.811058 pybaywatch-2024.4.8/pybaywatch.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-09 19:08:44.811767 pybaywatch-2024.4.8/pybaywatch.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-03-17 02:47:06.000000 pybaywatch-2024.4.8/pybaywatch.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       16 2024-04-09 19:08:44.813030 pybaywatch-2024.4.8/pybaywatch.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       11 2024-04-09 19:08:44.813699 pybaywatch-2024.4.8/pybaywatch.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-09 19:08:44.815479 pybaywatch-2024.4.8/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      781 2024-04-09 19:08:33.000000 pybaywatch-2024.4.8/setup.py
```

### Comparing `pybaywatch-2024.4.4/LICENSE` & `pybaywatch-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/TEX_forward.m` & `pybaywatch-2024.4.8/pybaywatch/TEX_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/UK_forward.m` & `pybaywatch-2024.4.8/pybaywatch/UK_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/bayfox_forward.m` & `pybaywatch-2024.4.8/pybaywatch/bayfox_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/baymag_forward_ln.m` & `pybaywatch-2024.4.8/pybaywatch/baymag_forward_ln.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/baymbt_forward.m` & `pybaywatch-2024.4.8/pybaywatch/baymbt_forward.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/core.py` & `pybaywatch-2024.4.8/pybaywatch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-'''
-BAYWATCH in pure Python
-@author: Feng Zhu (fengzhu@ucar.edu)
-'''
-
 import os
 import numpy as np
 import pandas as pd
 import xarray as xr
 from scipy.interpolate import BSpline, interp1d
 from scipy.io import loadmat
 from . import utils
```

### Comparing `pybaywatch-2024.4.4/pybaywatch/normrnd.m` & `pybaywatch-2024.4.8/pybaywatch/normrnd.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/randsample.m` & `pybaywatch-2024.4.8/pybaywatch/randsample.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/rndcheck.m` & `pybaywatch-2024.4.8/pybaywatch/rndcheck.m`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/utils.py` & `pybaywatch-2024.4.8/pybaywatch/utils.py`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/pybaywatch/wrapper.py` & `pybaywatch-2024.4.8/pybaywatch/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-'''
-Wrappers for BAYWATCH in Matlab
-@author: Feng Zhu (fengzhu@ucar.edu)
-'''
-
 import os
 import numpy as np
 import oct2py
 from . import utils
 dirpath = os.path.dirname(__file__)
 
 def TEX_forward_M(lat, lon, temp, seed=2333, type='SST', mode='standard', tolerance=None):
```

### Comparing `pybaywatch-2024.4.4/pybaywatch.egg-info/SOURCES.txt` & `pybaywatch-2024.4.8/pybaywatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybaywatch-2024.4.4/setup.py` & `pybaywatch-2024.4.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='pybaywatch',  # required
-    version='2024.4.4',
+    version='2024.4.8',
     description='PyBAYWATCH: BAYWATCH in Python',
     long_description=long_description,
-    long_description_content_type='text/x-rst',
+    long_description_content_type='text/markdown',
     author='Feng Zhu, Jessica Tierney',
     author_email='fengzhu@ucar.edu, jesst@arizona.edu',
     url='https://github.com/fzhu2e/pybaywatch',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
-    keywords='Proxy System Models for Ocean Sediments',
+    keywords='Bayeisan Hierarchical Proxy System Models for Sediments',
     classifiers=[
         'Programming Language :: Python :: 3.11',
     ],
     include_package_data=True,
     install_requires=[
         'colorama',
         'oct2py',
```

