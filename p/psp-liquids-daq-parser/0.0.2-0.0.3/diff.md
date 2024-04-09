# Comparing `tmp/psp_liquids_daq_parser-0.0.2.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.2.tar", last modified: Tue Apr  9 04:50:15 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.3.tar", last modified: Tue Apr  9 05:06:54 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.2.tar` & `psp_liquids_daq_parser-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 04:50:15.450261 psp_liquids_daq_parser-0.0.2/
--rw-rw-rw-   0        0        0    35821 2024-04-09 04:28:46.000000 psp_liquids_daq_parser-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      789 2024-04-09 04:50:15.447266 psp_liquids_daq_parser-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      144 2024-04-09 04:30:10.000000 psp_liquids_daq_parser-0.0.2/README.md
--rw-rw-rw-   0        0        0      788 2024-04-09 04:49:52.000000 psp_liquids_daq_parser-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 04:50:15.450261 psp_liquids_daq_parser-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 04:50:15.417204 psp_liquids_daq_parser-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2024-04-09 04:26:44.000000 psp_liquids_daq_parser-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 04:50:15.446263 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/
--rw-rw-rw-   0        0        0      789 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10297 2024-04-09 04:26:27.000000 psp_liquids_daq_parser-0.0.2/src/tdms_conversion.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:06:54.597463 psp_liquids_daq_parser-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 04:28:46.000000 psp_liquids_daq_parser-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      885 2024-04-09 05:06:54.595463 psp_liquids_daq_parser-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2024-04-09 04:30:10.000000 psp_liquids_daq_parser-0.0.3/README.md
+-rw-rw-rw-   0        0        0      821 2024-04-09 05:06:37.000000 psp_liquids_daq_parser-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:06:54.598463 psp_liquids_daq_parser-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 05:06:54.554298 psp_liquids_daq_parser-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2024-04-09 04:26:44.000000 psp_liquids_daq_parser-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:06:54.593466 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/
+-rw-rw-rw-   0        0        0      885 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2024-04-09 05:06:54.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10297 2024-04-09 04:26:27.000000 psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.py
```

### Comparing `psp_liquids_daq_parser-0.0.2/LICENSE` & `psp_liquids_daq_parser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.2/PKG-INFO` & `psp_liquids_daq_parser-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0
+Requires-Dist: numpy>=1.26.4
 
 # Purdue Space Program: Liquids DAQ file parser
 
 Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
```

### Comparing `psp_liquids_daq_parser-0.0.2/pyproject.toml` & `psp_liquids_daq_parser-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
-requires = ["setuptools>=61.0", "npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0", "numpy>=1.26.4"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psp_liquids_daq_parser"
-version = "0.0.2"
-authors = [
-  { name="Rajan Phadnis", email="rajansd28@gmail.com" },
-]
+version = "0.0.3"
+authors = [{ name = "Rajan Phadnis", email = "rajansd28@gmail.com" }]
 description = "Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes."
 readme = "README.md"
 requires-python = ">=3.11.0"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0",
+    "numpy>=1.26.4",
+]
 
 [project.urls]
 Homepage = "https://github.com/Purdue-Space-Program/daq_parser"
-Issues = "https://github.com/Purdue-Space-Program/daq_parser/issues"
+Issues = "https://github.com/Purdue-Space-Program/daq_parser/issues"
```

### Comparing `psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/PKG-INFO` & `psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0
+Requires-Dist: numpy>=1.26.4
 
 # Purdue Space Program: Liquids DAQ file parser
 
 Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
```

### Comparing `psp_liquids_daq_parser-0.0.2/src/tdms_conversion.py` & `psp_liquids_daq_parser-0.0.3/src/psp_liquids_daq_parser.py`

 * *Files identical despite different names*

