# Comparing `tmp/NeoNMM-2.4.tar.gz` & `tmp/NeoNMM-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeoNMM-2.4.tar", last modified: Tue Apr  9 14:26:57 2024, max compression
+gzip compressed data, was "NeoNMM-2.5.tar", last modified: Tue Apr  9 14:31:26 2024, max compression
```

## Comparing `NeoNMM-2.4.tar` & `NeoNMM-2.5.tar`

### file list

```diff
@@ -1,20 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:26:57.006855 NeoNMM-2.4/
--rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.4/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-09 14:26:56.961858 NeoNMM-2.4/NeoNMM/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:26:57.000858 NeoNMM-2.4/NeoNMM/PackageSources/
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.4/NeoNMM/PackageSources/__init__.py
--rw-rw-rw-   0        0        0     5686 2024-04-09 14:26:07.000000 NeoNMM-2.4/NeoNMM/Scrypt2.py
--rw-rw-rw-   0        0        0     6192 2024-04-09 14:26:32.000000 NeoNMM-2.4/NeoNMM/Scrypt_3node.py
--rw-rw-rw-   0        0        0     6088 2024-04-09 14:26:32.000000 NeoNMM-2.4/NeoNMM/Scrypt_interictal_to_seizure.py
--rw-rw-rw-   0        0        0     2599 2024-04-09 14:26:32.000000 NeoNMM-2.4/NeoNMM/Scrypt_single_node.py
--rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.4/NeoNMM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:26:57.002857 NeoNMM-2.4/NeoNMM.egg-info/
--rw-rw-rw-   0        0        0    33229 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    33229 2024-04-09 14:26:57.004853 NeoNMM-2.4/PKG-INFO
--rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.4/README.md
--rw-rw-rw-   0        0        0      636 2024-04-09 14:26:46.000000 NeoNMM-2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 14:26:57.006855 NeoNMM-2.4/setup.cfg
--rw-rw-rw-   0        0        0      406 2024-04-09 14:26:46.000000 NeoNMM-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.636973 NeoNMM-2.5/
+-rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.5/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.607462 NeoNMM-2.5/NeoNMM/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.622974 NeoNMM-2.5/NeoNMM/PackageSources/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.626973 NeoNMM-2.5/NeoNMM/PackageSources/Computation/
+-rw-rw-rw-   0        0        0      893 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Classes.py
+-rw-rw-rw-   0        0        0     1217 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Filter.py
+-rw-rw-rw-   0        0        0    10788 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Generate_Signal.py
+-rw-rw-rw-   0        0        0     9397 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Loading.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.629973 NeoNMM-2.5/NeoNMM/PackageSources/Display/
+-rw-rw-rw-   0        0        0     6681 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/EEG_Viewer.py
+-rw-rw-rw-   0        0        0    32826 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/Mesh3DView.py
+-rw-rw-rw-   0        0        0     4894 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/Spectrogram.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.633973 NeoNMM-2.5/NeoNMM/PackageSources/Model/
+-rw-rw-rw-   0        0        0    16099 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/Cortex_Model_NeoNMM.py
+-rw-rw-rw-   0        0        0    30630 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/Model_NeoNMM.py
+-rw-rw-rw-   0        0        0    22000 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/Model_NeoNMM_GUI.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/__init__.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/__init__.py
+-rw-rw-rw-   0        0        0     5686 2024-04-09 14:26:07.000000 NeoNMM-2.5/NeoNMM/Scrypt2.py
+-rw-rw-rw-   0        0        0     6192 2024-04-09 14:26:32.000000 NeoNMM-2.5/NeoNMM/Scrypt_3node.py
+-rw-rw-rw-   0        0        0     6088 2024-04-09 14:26:32.000000 NeoNMM-2.5/NeoNMM/Scrypt_interictal_to_seizure.py
+-rw-rw-rw-   0        0        0     2599 2024-04-09 14:26:32.000000 NeoNMM-2.5/NeoNMM/Scrypt_single_node.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.5/NeoNMM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.634973 NeoNMM-2.5/NeoNMM.egg-info/
+-rw-rw-rw-   0        0        0    33229 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    33229 2024-04-09 14:31:26.635974 NeoNMM-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.5/README.md
+-rw-rw-rw-   0        0        0      636 2024-04-09 14:31:18.000000 NeoNMM-2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:31:26.636973 NeoNMM-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      406 2024-04-09 14:31:18.000000 NeoNMM-2.5/setup.py
```

### Comparing `NeoNMM-2.4/LICENSE` & `NeoNMM-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.4/NeoNMM/Scrypt2.py` & `NeoNMM-2.5/NeoNMM/Scrypt2.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.4/NeoNMM/Scrypt_3node.py` & `NeoNMM-2.5/NeoNMM/Scrypt_3node.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.4/NeoNMM/Scrypt_interictal_to_seizure.py` & `NeoNMM-2.5/NeoNMM/Scrypt_interictal_to_seizure.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.4/NeoNMM/Scrypt_single_node.py` & `NeoNMM-2.5/NeoNMM/Scrypt_single_node.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.4/NeoNMM.egg-info/PKG-INFO` & `NeoNMM-2.5/NeoNMM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.4
+Version: 2.5
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
 Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `NeoNMM-2.4/PKG-INFO` & `NeoNMM-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.4
+Version: 2.5
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
 Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `NeoNMM-2.4/README.md` & `NeoNMM-2.5/README.md`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.4/pyproject.toml` & `NeoNMM-2.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "NeoNMM"
-version = "2.4"
+version = "2.5"
 authors = [
   { name="MAxime Yochum", email="maxime.yochum@univ-rennes.fr" },
 ]
 description = "NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

