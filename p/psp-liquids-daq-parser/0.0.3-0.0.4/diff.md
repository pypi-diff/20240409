# Comparing `tmp/psp_liquids_daq_parser-0.0.3.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.3.tar", last modified: Tue Apr  9 05:06:54 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.4.tar", last modified: Tue Apr  9 05:44:11 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.3.tar` & `psp_liquids_daq_parser-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 05:06:54.597463 psp_liquids_daq_parser-0.0.3/
--rw-rw-rw-   0        0        0    35821 2024-04-09 04:28:46.000000 psp_liquids_daq_parser-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      885 2024-04-09 05:06:54.595463 psp_liquids_daq_parser-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      144 2024-04-09 04:30:10.000000 psp_liquids_daq_parser-0.0.3/README.md
--rw-rw-rw-   0        0        0      821 2024-04-09 05:06:37.000000 psp_liquids_daq_parser-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 05:06:54.598463 psp_liquids_daq_parser-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 05:06:54.554298 psp_liquids_daq_parser-0.0.3/src/
--rw-rw-rw-   0        0        0        0 2024-04-09 04:26:44.000000 psp_liquids_daq_parser-0.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:06:54.593466 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/
--rw-rw-rw-   0        0        0      885 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10297 2024-04-09 04:26:27.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 05:44:09.000000 psp_liquids_daq_parser-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.py
```

### Comparing `psp_liquids_daq_parser-0.0.3/LICENSE` & `psp_liquids_daq_parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.3/PKG-INFO` & `psp_liquids_daq_parser-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: psp_liquids_daq_parser
-Version: 0.0.3
-Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
-Author-email: Rajan Phadnis <rajansd28@gmail.com>
-Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
-Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0
-Requires-Dist: numpy>=1.26.4
-
-# Purdue Space Program: Liquids DAQ file parser
-
-Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
+Metadata-Version: 2.1
+Name: psp_liquids_daq_parser
+Version: 0.0.4
+Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
+Author-email: Rajan Phadnis <rajansd28@gmail.com>
+Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
+Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0
+Requires-Dist: numpy>=1.26.4
+
+# Purdue Space Program: Liquids DAQ file parser
+
+Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
```

### Comparing `psp_liquids_daq_parser-0.0.3/pyproject.toml` & `psp_liquids_daq_parser-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psp_liquids_daq_parser"
-version = "0.0.3"
+dynamic = ["version"]
 authors = [{ name = "Rajan Phadnis", email = "rajansd28@gmail.com" }]
 description = "Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes."
 readme = "README.md"
 requires-python = ">=3.11.0"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0",
     "numpy>=1.26.4",
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "__init__.__version__"}
+
 [project.urls]
 Homepage = "https://github.com/Purdue-Space-Program/daq_parser"
 Issues = "https://github.com/Purdue-Space-Program/daq_parser/issues"
```

### Comparing `psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/PKG-INFO` & `psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: psp_liquids_daq_parser
-Version: 0.0.3
-Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
-Author-email: Rajan Phadnis <rajansd28@gmail.com>
-Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
-Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0
-Requires-Dist: numpy>=1.26.4
-
-# Purdue Space Program: Liquids DAQ file parser
-
-Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
+Metadata-Version: 2.1
+Name: psp_liquids_daq_parser
+Version: 0.0.4
+Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
+Author-email: Rajan Phadnis <rajansd28@gmail.com>
+Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
+Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0
+Requires-Dist: numpy>=1.26.4
+
+# Purdue Space Program: Liquids DAQ file parser
+
+Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
```

### Comparing `psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.py` & `psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from numpy.typing import NDArray
 import pickle
 import numpy as np
 import tkinter as tk
 from tkinter import filedialog
 import os
 
+# __version__ = "0.0.4"
 
 class DigitalChannelData:
     def __init__(
         self,
         rawData: NDArray[float64],
         properties: OrderedDict,
         name: str,
```

