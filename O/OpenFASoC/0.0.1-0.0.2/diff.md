# Comparing `tmp/OpenFASoC-0.0.1.tar.gz` & `tmp/OpenFASoC-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFASoC-0.0.1.tar", last modified: Sat Apr  6 16:15:15 2024, max compression
+gzip compressed data, was "OpenFASoC-0.0.2.tar", last modified: Tue Apr  9 01:48:29 2024, max compression
```

## Comparing `OpenFASoC-0.0.1.tar` & `OpenFASoC-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,28 @@
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:15:15.673965 OpenFASoC-0.0.1/
--rw-r--r--   0 labtob    (1000) labtob    (1000)    11357 2024-04-06 16:10:50.000000 OpenFASoC-0.0.1/LICENSE
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:15:15.673965 OpenFASoC-0.0.1/OpenFASoC.egg-info/
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-06 16:15:15.000000 OpenFASoC-0.0.1/OpenFASoC.egg-info/PKG-INFO
--rw-r--r--   0 labtob    (1000) labtob    (1000)      201 2024-04-06 16:15:15.000000 OpenFASoC-0.0.1/OpenFASoC.egg-info/SOURCES.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-06 16:15:15.000000 OpenFASoC-0.0.1/OpenFASoC.egg-info/dependency_links.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)      130 2024-04-06 16:15:15.000000 OpenFASoC-0.0.1/OpenFASoC.egg-info/requires.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-06 16:15:15.000000 OpenFASoC-0.0.1/OpenFASoC.egg-info/top_level.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-06 16:15:15.673965 OpenFASoC-0.0.1/PKG-INFO
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8013 2024-04-06 16:10:50.000000 OpenFASoC-0.0.1/README.rst
--rw-r--r--   0 labtob    (1000) labtob    (1000)      399 2024-04-06 16:15:15.673965 OpenFASoC-0.0.1/setup.cfg
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1023 2024-04-06 16:10:51.000000 OpenFASoC-0.0.1/setup.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    11357 2024-04-06 16:10:50.000000 OpenFASoC-0.0.2/LICENSE
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.425215 OpenFASoC-0.0.2/OpenFASoC.egg-info/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      741 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/SOURCES.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/dependency_links.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      130 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/requires.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       10 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/top_level.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8013 2024-04-06 16:10:50.000000 OpenFASoC-0.0.2/README.rst
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.425215 OpenFASoC-0.0.2/openfasoc/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:39:12.000000 OpenFASoC-0.0.2/openfasoc/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      467 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/config.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.425215 OpenFASoC-0.0.2/openfasoc/generators/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      202 2024-04-09 01:47:29.000000 OpenFASoC-0.0.2/openfasoc/generators/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/openfasoc/generators/common/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1323 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3369 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/check_gen_files.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      583 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/get_ngspice_version.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4203 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1809 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/classify_sim_error.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     6779 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/simulation_config.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4289 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/simulation_run.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1316 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4298 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/verilog_generation.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      399 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/setup.cfg
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1023 2024-04-09 01:45:32.000000 OpenFASoC-0.0.2/setup.py
```

### Comparing `OpenFASoC-0.0.1/LICENSE` & `OpenFASoC-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.1/OpenFASoC.egg-info/PKG-INFO` & `OpenFASoC-0.0.2/OpenFASoC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFASoC
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
 Home-page: https://github.com/idea-fasoc/OpenFASOC
 Author:  msaligane
 Author-email: mehdi@umich.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenFASoC-0.0.1/PKG-INFO` & `OpenFASoC-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFASoC
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
 Home-page: https://github.com/idea-fasoc/OpenFASOC
 Author:  msaligane
 Author-email: mehdi@umich.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenFASoC-0.0.1/README.rst` & `OpenFASoC-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.1/setup.py` & `OpenFASoC-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def get_install_requires():
     with open("requirements.txt", "r") as f:
         return [line.strip() for line in f.readlines() if not line.startswith("-")]
 
 
 setup(
     name="OpenFASoC",
-    version="0.0.1",
+    version="0.0.2",
     url="https://github.com/idea-fasoc/OpenFASOC",
     license="MIT",
     author=" msaligane",
     author_email="mehdi@umich.edu",
     description="Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
```

