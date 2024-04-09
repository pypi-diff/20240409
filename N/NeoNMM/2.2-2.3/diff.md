# Comparing `tmp/NeoNMM-2.2.tar.gz` & `tmp/NeoNMM-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeoNMM-2.2.tar", last modified: Tue Apr  9 13:58:19 2024, max compression
+gzip compressed data, was "NeoNMM-2.3.tar", last modified: Tue Apr  9 14:21:24 2024, max compression
```

## Comparing `NeoNMM-2.2.tar` & `NeoNMM-2.3.tar`

### file list

```diff
@@ -1,32 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.839585 NeoNMM-2.2/
--rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.2/LICENSE
--rw-rw-rw-   0        0        0    33206 2024-04-09 13:58:19.838579 NeoNMM-2.2/PKG-INFO
--rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.2/README.md
--rw-rw-rw-   0        0        0      636 2024-04-09 13:58:10.000000 NeoNMM-2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 13:58:19.840586 NeoNMM-2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.800585 NeoNMM-2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.837579 NeoNMM-2.2/src/NeoNMM.egg-info/
--rw-rw-rw-   0        0        0    33206 2024-04-09 13:58:19.000000 NeoNMM-2.2/src/NeoNMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2024-04-09 13:58:19.000000 NeoNMM-2.2/src/NeoNMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:58:19.000000 NeoNMM-2.2/src/NeoNMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-09 13:58:19.000000 NeoNMM-2.2/src/NeoNMM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.825580 NeoNMM-2.2/src/PackageSources/
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.828578 NeoNMM-2.2/src/PackageSources/Computation/
--rw-rw-rw-   0        0        0      893 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Computation/Classes.py
--rw-rw-rw-   0        0        0     1217 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Computation/Filter.py
--rw-rw-rw-   0        0        0    10788 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Computation/Generate_Signal.py
--rw-rw-rw-   0        0        0     9397 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Computation/Loading.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.833579 NeoNMM-2.2/src/PackageSources/Display/
--rw-rw-rw-   0        0        0     6681 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Display/EEG_Viewer.py
--rw-rw-rw-   0        0        0    32826 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Display/Mesh3DView.py
--rw-rw-rw-   0        0        0     4894 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Display/Spectrogram.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:58:19.836579 NeoNMM-2.2/src/PackageSources/Model/
--rw-rw-rw-   0        0        0    16099 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Model/Cortex_Model_NeoNMM.py
--rw-rw-rw-   0        0        0    30630 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Model/Model_NeoNMM.py
--rw-rw-rw-   0        0        0    22000 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/Model/Model_NeoNMM_GUI.py
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/PackageSources/__init__.py
--rw-rw-rw-   0        0        0     5630 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/Scrypt2.py
--rw-rw-rw-   0        0        0     6143 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/Scrypt_3node.py
--rw-rw-rw-   0        0        0     6032 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/Scrypt_interictal_to_seizure.py
--rw-rw-rw-   0        0        0     2550 2024-04-09 12:18:37.000000 NeoNMM-2.2/src/Scrypt_single_node.py
--rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.091246 NeoNMM-2.3/
+-rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.088247 NeoNMM-2.3/NeoNMM.egg-info/
+-rw-rw-rw-   0        0        0    33229 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    33229 2024-04-09 14:21:24.090247 NeoNMM-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.3/README.md
+-rw-rw-rw-   0        0        0      636 2024-04-09 14:18:09.000000 NeoNMM-2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:21:24.091246 NeoNMM-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      406 2024-04-09 14:20:52.000000 NeoNMM-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.087247 NeoNMM-2.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.087247 NeoNMM-2.3/src/PackageSources/
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/PackageSources/__init__.py
+-rw-rw-rw-   0        0        0     5630 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt2.py
+-rw-rw-rw-   0        0        0     6143 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt_3node.py
+-rw-rw-rw-   0        0        0     6032 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt_interictal_to_seizure.py
+-rw-rw-rw-   0        0        0     2550 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt_single_node.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.3/src/__init__.py
```

### Comparing `NeoNMM-2.2/LICENSE` & `NeoNMM-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.2/PKG-INFO` & `NeoNMM-2.3/NeoNMM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.2
+Version: 2.3
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
+Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `NeoNMM-2.2/README.md` & `NeoNMM-2.3/README.md`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.2/pyproject.toml` & `NeoNMM-2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "NeoNMM"
-version = "2.2"
+version = "2.3"
 authors = [
   { name="MAxime Yochum", email="maxime.yochum@univ-rennes.fr" },
 ]
 description = "NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `NeoNMM-2.2/src/NeoNMM.egg-info/PKG-INFO` & `NeoNMM-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.2
+Version: 2.3
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
+Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `NeoNMM-2.2/src/Scrypt2.py` & `NeoNMM-2.3/src/Scrypt2.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.2/src/Scrypt_3node.py` & `NeoNMM-2.3/src/Scrypt_3node.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.2/src/Scrypt_interictal_to_seizure.py` & `NeoNMM-2.3/src/Scrypt_interictal_to_seizure.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.2/src/Scrypt_single_node.py` & `NeoNMM-2.3/src/Scrypt_single_node.py`

 * *Files identical despite different names*

