# Comparing `tmp/psp_liquids_daq_parser-0.0.1.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.1.tar", last modified: Tue Apr  9 04:44:09 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.2.tar", last modified: Tue Apr  9 04:50:15 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.1.tar` & `psp_liquids_daq_parser-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 04:44:09.854441 psp_liquids_daq_parser-0.0.1/
--rw-rw-rw-   0        0        0    35821 2024-04-09 04:28:46.000000 psp_liquids_daq_parser-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      789 2024-04-09 04:44:09.851283 psp_liquids_daq_parser-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      144 2024-04-09 04:30:10.000000 psp_liquids_daq_parser-0.0.1/README.md
--rw-rw-rw-   0        0        0      788 2024-04-09 04:43:04.000000 psp_liquids_daq_parser-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 04:44:09.855454 psp_liquids_daq_parser-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 04:44:09.819553 psp_liquids_daq_parser-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2024-04-09 04:26:44.000000 psp_liquids_daq_parser-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 04:44:09.849319 psp_liquids_daq_parser-0.0.1/src/psp_liquids_daq_parser.egg-info/
--rw-rw-rw-   0        0        0      789 2024-04-09 04:44:09.000000 psp_liquids_daq_parser-0.0.1/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-09 04:44:09.000000 psp_liquids_daq_parser-0.0.1/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 04:44:09.000000 psp_liquids_daq_parser-0.0.1/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-09 04:44:09.000000 psp_liquids_daq_parser-0.0.1/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10297 2024-04-09 04:26:27.000000 psp_liquids_daq_parser-0.0.1/src/tdms_conversion.py
+drwxrwxrwx   0        0        0        0 2024-04-09 04:50:15.450261 psp_liquids_daq_parser-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 04:28:46.000000 psp_liquids_daq_parser-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      789 2024-04-09 04:50:15.447266 psp_liquids_daq_parser-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2024-04-09 04:30:10.000000 psp_liquids_daq_parser-0.0.2/README.md
+-rw-rw-rw-   0        0        0      788 2024-04-09 04:49:52.000000 psp_liquids_daq_parser-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 04:50:15.450261 psp_liquids_daq_parser-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 04:50:15.417204 psp_liquids_daq_parser-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2024-04-09 04:26:44.000000 psp_liquids_daq_parser-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 04:50:15.446263 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/
+-rw-rw-rw-   0        0        0      789 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-09 04:50:15.000000 psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10297 2024-04-09 04:26:27.000000 psp_liquids_daq_parser-0.0.2/src/tdms_conversion.py
```

### Comparing `psp_liquids_daq_parser-0.0.1/LICENSE` & `psp_liquids_daq_parser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.1/PKG-INFO` & `psp_liquids_daq_parser-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.7
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Purdue Space Program: Liquids DAQ file parser
 
 Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
```

### Comparing `psp_liquids_daq_parser-0.0.1/pyproject.toml` & `psp_liquids_daq_parser-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0", "npTDMS[hdf,pandas,thermocouple_scaling]>=1.9.0", "numpy>=1.26.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psp_liquids_daq_parser"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Rajan Phadnis", email="rajansd28@gmail.com" },
 ]
 description = "Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes."
 readme = "README.md"
-requires-python = ">=3.11.7"
+requires-python = ">=3.11.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `psp_liquids_daq_parser-0.0.1/src/psp_liquids_daq_parser.egg-info/PKG-INFO` & `psp_liquids_daq_parser-0.0.2/src/psp_liquids_daq_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.7
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Purdue Space Program: Liquids DAQ file parser
 
 Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
```

### Comparing `psp_liquids_daq_parser-0.0.1/src/tdms_conversion.py` & `psp_liquids_daq_parser-0.0.2/src/tdms_conversion.py`

 * *Files identical despite different names*

