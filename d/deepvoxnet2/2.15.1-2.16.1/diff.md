# Comparing `tmp/deepvoxnet2-2.15.1.tar.gz` & `tmp/deepvoxnet2-2.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepvoxnet2-2.15.1.tar", last modified: Fri Mar 29 09:52:48 2024, max compression
+gzip compressed data, was "deepvoxnet2-2.16.1.tar", last modified: Tue Apr  9 15:11:11 2024, max compression
```

## Comparing `deepvoxnet2-2.15.1.tar` & `deepvoxnet2-2.16.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.049584 deepvoxnet2-2.15.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.041583 deepvoxnet2-2.15.1/deepvoxnet2/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.041583 deepvoxnet2-2.15.1/deepvoxnet2/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/analysis/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    98819 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/analysis/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.041583 deepvoxnet2-2.15.1/deepvoxnet2/backwards_compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/backwards_compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/backwards_compatibility/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/backwards_compatibility/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/deepvoxnet2/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    37805 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/mirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    30936 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    94486 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/components/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/deepvoxnet2/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/factories/directory_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/deepvoxnet2/keras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    24514 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/deepvoxnet2/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19339 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/models/deepmedic_generalized.py
--rw-r--r--   0 runner    (1001) docker     (127)    25068 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/models/deepmedic_generalized_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20596 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/models/unet_generalized.py
--rw-r--r--   0 runner    (1001) docker     (127)    28988 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/models/unet_generalized_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/keras/optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/deepvoxnet2/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/utilities/calculate_gpu_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18585 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/utilities/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/utilities/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-03-29 09:52:35.000000 deepvoxnet2-2.15.1/deepvoxnet2/utilities/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:52:48.045584 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-03-29 09:52:48.000000 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-29 09:52:48.000000 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:52:48.000000 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:52:48.000000 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-29 09:52:48.000000 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 09:52:48.000000 deepvoxnet2-2.15.1/deepvoxnet2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 09:52:48.049584 deepvoxnet2-2.15.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-29 09:52:36.000000 deepvoxnet2-2.15.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.247194 deepvoxnet2-2.16.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-09 15:11:11.247194 deepvoxnet2-2.16.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.239194 deepvoxnet2-2.16.1/deepvoxnet2/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.239194 deepvoxnet2-2.16.1/deepvoxnet2/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/analysis/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98819 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/analysis/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.239194 deepvoxnet2-2.16.1/deepvoxnet2/backwards_compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/backwards_compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/backwards_compatibility/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/backwards_compatibility/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.243194 deepvoxnet2-2.16.1/deepvoxnet2/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37805 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/mirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30936 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96039 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/components/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.243194 deepvoxnet2-2.16.1/deepvoxnet2/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/factories/directory_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.243194 deepvoxnet2-2.16.1/deepvoxnet2/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24514 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.243194 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19339 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/deepmedic_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25068 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/deepmedic_generalized_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20596 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/unet_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28988 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/unet_generalized_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35729 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/models/unet_generalized_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/keras/optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.247194 deepvoxnet2-2.16.1/deepvoxnet2/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/utilities/calculate_gpu_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18585 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/utilities/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/utilities/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/deepvoxnet2/utilities/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:11.247194 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-09 15:11:11.000000 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 15:11:11.000000 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:11:11.000000 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:11:11.000000 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-09 15:11:11.000000 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 15:11:11.000000 deepvoxnet2-2.16.1/deepvoxnet2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:11:11.247194 deepvoxnet2-2.16.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 15:11:03.000000 deepvoxnet2-2.16.1/setup.py
```

### Comparing `deepvoxnet2-2.15.1/LICENSE` & `deepvoxnet2-2.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/PKG-INFO` & `deepvoxnet2-2.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepvoxnet2
-Version: 2.15.1
+Version: 2.16.1
 Summary: Yet another CNN framework: From pre- to postprocessing and keeping track of the spatial origin of the data.
 Home-page: https://github.com/JeroenBertels/deepvoxnet2
 Author: Jeroen Bertels
 Author-email: jeroen.bertels@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Requires-Dist: scikit-learn
 Requires-Dist: xlrd>=2.0
 Requires-Dist: openpyxl>=3.0
 Requires-Dist: opencv-python>=4.5
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: comet-ml>=3.31.17
 Requires-Dist: twine>=4.0.1
+Requires-Dist: pydot>=2.0.0
 Requires-Dist: pymirc
 Provides-Extra: sitk
 Requires-Dist: simpleitk-simpleelastix; extra == "sitk"
 
 # DeepVoxNet2
 DeepVoxNet2 (DVN2) is a Python library to make it easier to implement deep learning pipelines for medical applications using convolutional neural networks (CNNs).
 It is lightly based on the private [DeepVoxNet](https://github.com/JeroenBertels/deepvoxnet) library.
```

### Comparing `deepvoxnet2-2.15.1/README.md` & `deepvoxnet2-2.16.1/README.md`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/analysis/analysis.py` & `deepvoxnet2-2.16.1/deepvoxnet2/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/analysis/data.py` & `deepvoxnet2-2.16.1/deepvoxnet2/analysis/data.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/analysis/plotting.py` & `deepvoxnet2-2.16.1/deepvoxnet2/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/backwards_compatibility/losses.py` & `deepvoxnet2-2.16.1/deepvoxnet2/backwards_compatibility/losses.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/backwards_compatibility/metrics.py` & `deepvoxnet2-2.16.1/deepvoxnet2/backwards_compatibility/metrics.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/components/creator.py` & `deepvoxnet2-2.16.1/deepvoxnet2/components/creator.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/components/mirc.py` & `deepvoxnet2-2.16.1/deepvoxnet2/components/mirc.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/components/model.py` & `deepvoxnet2-2.16.1/deepvoxnet2/components/model.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/components/sample.py` & `deepvoxnet2-2.16.1/deepvoxnet2/components/sample.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/components/sampler.py` & `deepvoxnet2-2.16.1/deepvoxnet2/components/sampler.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/components/transformers.py` & `deepvoxnet2-2.16.1/deepvoxnet2/components/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,31 +792,32 @@
         If buffer_size is not None, it continues filling the buffer until it reaches that size.
 
         Raises
         ------
         StopIteration
             If `drop_remainder` is True and there are not enough samples to fill the buffer completely.
         """
-
+        initial_sample_ids = [transformer.sample_id for transformer in Connection.trace([connection for idx in self.active_indices for connection in self.connections[idx]], only_active=True)[0]]
         self.buffered_outputs = [[[sample for sample in self.connections[idx][0]]] if idx in self.active_indices else None for idx in range(len(self.outputs))]
         while self.buffer_size is None or len(self.buffered_outputs[0]) < self.buffer_size:
             try:
                 sample_id = uuid.uuid4()
                 for idx in self.active_indices:
                     self.buffered_outputs[idx].append([sample for sample in self.connections[idx][0].eval(sample_id)])
 
             except (StopIteration, RuntimeError):
                 break
 
         if self.buffer_size is not None and self.drop_remainder and len(self.buffered_outputs[0]) < self.buffer_size:
             raise StopIteration
 
         else:
-            for transformer in Connection.trace([connection for connections in self.connections for connection in connections], only_active=True)[0]:
-                transformer.sample_id = self.sample_id
+            for i, transformer in enumerate(Connection.trace([connection for idx in self.active_indices for connection in self.connections[idx]], only_active=True)[0]):
+                if initial_sample_ids[i] != transformer.sample_id:
+                    transformer.sample_id = self.sample_id
 
 
 class Group(Transformer):
     """The `Group` transformer groups together all samples in all input connections at each index into one output connection at that index.
     """
 
     def __init__(self, **kwargs):
@@ -977,20 +978,20 @@
         axis : int, optional
             The axis along which to compute the mean. Default is -1.
         **kwargs
             Additional arguments passed to the parent class constructor.
         """
 
         super(Mean, self).__init__(**kwargs)
-        assert axis in [4, -1]
+        # assert axis in [4, -1]
         self.axis = axis if axis != -1 else 4
 
     def _update_idx(self, idx):
         for idx_, sample in enumerate(self.connections[idx][0]):
-            self.outputs[idx][idx_] = sample.mean(axis=self.axis, keepdims=True)
+            self.outputs[idx][idx_] = sample.mean(axis=self.axis, keepdims=True) if self.axis != 0 else Sample(np.mean(sample, axis=0, keepdims=True), affine=sample.affine[0])
 
     def _calculate_output_shape_at_idx(self, idx):
         assert len(self.connections[idx]) == 1, "This transformer accepts only a single connection at every idx."
         return [tuple([output_shape_ if axis_i != self.axis else 1 for axis_i, output_shape_ in enumerate(output_shape)]) for output_shape in self.connections[idx][0].shapes]
 
     def _randomize(self):
         pass
@@ -1567,14 +1568,17 @@
     def _randomize(self):
         pass
 
 
 class Flip(Transformer):
     def __init__(self, flip_probabilities=(0.5, 0.5, 0.5), **kwargs):
         super(Flip, self).__init__(**kwargs)
+        if isinstance(flip_probabilities, str):
+            assert flip_probabilities == "all" and self.n == 8
+
         self.flip_probabilities = flip_probabilities
         self.flip_state = None
 
     def _update_idx(self, idx):
         for idx_, sample in enumerate(self.connections[idx][0]):
             flipped_array = sample[:, ::self.flip_state[0], ::self.flip_state[1], ::self.flip_state[2], :]
             backward_affine = Sample.update_affine(reflection=self.flip_state) @ Sample.update_affine(translation=[1 - shape if state == -1 else 0 for state, shape in zip(self.flip_state, sample.shape[1:4])])
@@ -1582,15 +1586,44 @@
             self.outputs[idx][idx_] = Sample(flipped_array, flipped_affine)
 
     def _calculate_output_shape_at_idx(self, idx):
         assert len(self.connections[idx]) == 1, "This transformer accepts only a single connection at every idx."
         return self.connections[idx][0].shapes
 
     def _randomize(self):
-        self.flip_state = [-1 if random.random() < flip_probability else 1 for flip_probability in self.flip_probabilities]
+        if isinstance(self.flip_probabilities, str):
+            if self.n_ == 0:
+                self.flip_state = [1, 1, 1]
+            
+            elif self.n_ == 1:
+                self.flip_state = [-1, 1, 1]
+            
+            elif self.n_ == 2:
+                self.flip_state = [1, -1, 1]
+            
+            elif self.n_ == 3:
+                self.flip_state = [-1, -1, 1]
+            
+            elif self.n_ == 4:
+                self.flip_state = [1, 1, -1]
+            
+            elif self.n_ == 5:
+                self.flip_state = [-1, 1, -1]
+            
+            elif self.n_ == 6:
+                self.flip_state = [1, -1, -1]
+            
+            elif self.n_ == 7:
+                self.flip_state = [-1, -1, -1]
+
+            else:
+                raise ValueError
+                        
+        else:
+            self.flip_state = [-1 if random.random() < flip_probability else 1 for flip_probability in self.flip_probabilities]
 
 
 class GaussianNoise(Transformer):
     def __init__(self, mean=0, std=1, **kwargs):
         super(GaussianNoise, self).__init__(**kwargs)
         mean, std = np.array(mean), np.array(std)
         assert mean.ndim <= 5 and std.ndim <= 5, "mean and std must be broadcastable with the shape of the samples that pass through and may have a maximum of 5 dimensions."
@@ -1718,18 +1751,18 @@
 
     def _randomize(self):
         assert all([np.array_equal(self.reference_connection[0].shape[1:4], sample.shape[1:4]) for connection in self.connections for sample in connection[0] if sample is not None])
         if random.random() < self.transform_probability:
             self.backward_affine = transformations.get_affine_matrix(
                 I_shape=self.reference_connection[0].shape[1:4],
                 voxel_size=self.voxel_size,
-                shear=[np.random.normal(0, w) if self.width_as_std[0] else random.uniform(-w, w) for w in self.shear_window_width],
-                rotation=[np.random.normal(0, w) if self.width_as_std[1] else random.uniform(-w, w) for w in self.rotation_window_width],
-                translation=[np.random.normal(0, w) if self.width_as_std[2] else random.uniform(-w, w) for w in self.translation_window_width],
-                scaling=[1 + (np.random.normal(0, w) if self.width_as_std[3] else random.uniform(-w, w)) for w in self.scaling_window_width],
+                shear=[np.random.normal(0, w) if self.width_as_std[0] else random.uniform(-w, w) for w in self.shear_window_width] * (3 if len(self.shear_window_width) == 1 else 1),
+                rotation=[np.random.normal(0, w) if self.width_as_std[1] else random.uniform(-w, w) for w in self.rotation_window_width] * (3 if len(self.rotation_window_width) == 1 else 1),
+                translation=[np.random.normal(0, w) if self.width_as_std[2] else random.uniform(-w, w) for w in self.translation_window_width] * (3 if len(self.translation_window_width) == 1 else 1),
+                scaling=[1 + (np.random.normal(0, w) if self.width_as_std[3] else random.uniform(-w, w)) for w in self.scaling_window_width] * (3 if len(self.scaling_window_width) == 1 else 1),
             )
 
         else:
             self.backward_affine = None
 
 
 class ElasticDeformation(Transformer):
```

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/factories/directory_structure.py` & `deepvoxnet2-2.16.1/deepvoxnet2/factories/directory_structure.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/callbacks.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/losses.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/losses.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/metrics.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/metrics.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/models/deepmedic_generalized.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/models/deepmedic_generalized.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/models/deepmedic_generalized_v2.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/models/deepmedic_generalized_v2.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/models/unet_generalized.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/models/unet_generalized.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/keras/models/unet_generalized_v2.py` & `deepvoxnet2-2.16.1/deepvoxnet2/keras/models/unet_generalized_v2.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/utilities/calculate_gpu_memory.py` & `deepvoxnet2-2.16.1/deepvoxnet2/utilities/calculate_gpu_memory.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/utilities/conversions.py` & `deepvoxnet2-2.16.1/deepvoxnet2/utilities/conversions.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/utilities/drawing.py` & `deepvoxnet2-2.16.1/deepvoxnet2/utilities/drawing.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2/utilities/transformations.py` & `deepvoxnet2-2.16.1/deepvoxnet2/utilities/transformations.py`

 * *Files identical despite different names*

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2.egg-info/PKG-INFO` & `deepvoxnet2-2.16.1/deepvoxnet2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepvoxnet2
-Version: 2.15.1
+Version: 2.16.1
 Summary: Yet another CNN framework: From pre- to postprocessing and keeping track of the spatial origin of the data.
 Home-page: https://github.com/JeroenBertels/deepvoxnet2
 Author: Jeroen Bertels
 Author-email: jeroen.bertels@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Requires-Dist: scikit-learn
 Requires-Dist: xlrd>=2.0
 Requires-Dist: openpyxl>=3.0
 Requires-Dist: opencv-python>=4.5
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: comet-ml>=3.31.17
 Requires-Dist: twine>=4.0.1
+Requires-Dist: pydot>=2.0.0
 Requires-Dist: pymirc
 Provides-Extra: sitk
 Requires-Dist: simpleitk-simpleelastix; extra == "sitk"
 
 # DeepVoxNet2
 DeepVoxNet2 (DVN2) is a Python library to make it easier to implement deep learning pipelines for medical applications using convolutional neural networks (CNNs).
 It is lightly based on the private [DeepVoxNet](https://github.com/JeroenBertels/deepvoxnet) library.
```

### Comparing `deepvoxnet2-2.15.1/deepvoxnet2.egg-info/SOURCES.txt` & `deepvoxnet2-2.16.1/deepvoxnet2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 deepvoxnet2/keras/metrics.py
 deepvoxnet2/keras/optimizers.py
 deepvoxnet2/keras/models/__init__.py
 deepvoxnet2/keras/models/deepmedic_generalized.py
 deepvoxnet2/keras/models/deepmedic_generalized_v2.py
 deepvoxnet2/keras/models/unet_generalized.py
 deepvoxnet2/keras/models/unet_generalized_v2.py
+deepvoxnet2/keras/models/unet_generalized_v3.py
 deepvoxnet2/utilities/__init__.py
 deepvoxnet2/utilities/calculate_gpu_memory.py
 deepvoxnet2/utilities/conversions.py
 deepvoxnet2/utilities/drawing.py
 deepvoxnet2/utilities/transformations.py
```

### Comparing `deepvoxnet2-2.15.1/setup.py` & `deepvoxnet2-2.16.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='deepvoxnet2',
-    version='2.15.1',
+    version='2.16.1',
     description='Yet another CNN framework: From pre- to postprocessing and keeping track of the spatial origin of the data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/JeroenBertels/deepvoxnet2',
     author='Jeroen Bertels',
     author_email='jeroen.bertels@gmail.com',
     license_files=('LICENSE',),
@@ -38,14 +38,15 @@
         'scikit-learn',
         'xlrd>=2.0',
         'openpyxl>=3.0',
         'opencv-python>=4.5',
         'seaborn>=0.11.2',
         'comet-ml>=3.31.17',
         'twine>=4.0.1',
+        'pydot>=2.0.0',
         'pymirc'
     ],
     extras_require={
         "sitk": [
             'simpleitk-simpleelastix',
         ]
     }
```

