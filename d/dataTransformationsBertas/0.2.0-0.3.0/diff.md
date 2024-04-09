# Comparing `tmp/datatransformationsbertas-0.2.0.tar.gz` & `tmp/datatransformationsbertas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransformationsbertas-0.2.0.tar", max compression
+gzip compressed data, was "datatransformationsbertas-0.3.0.tar", max compression
```

## Comparing `datatransformationsbertas-0.2.0.tar` & `datatransformationsbertas-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.2.0/LICENSE
--rw-r--r--   0        0        0     1214 2024-04-08 09:49:58.895011 datatransformationsbertas-0.2.0/README.md
--rw-r--r--   0        0        0      341 2024-04-08 10:55:02.311093 datatransformationsbertas-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2697 2024-04-08 10:03:34.134898 datatransformationsbertas-0.2.0/src/datatransformationsbertas/__init__.py
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 datatransformationsbertas-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.3.0/README.md
+-rw-r--r--   0        0        0      341 2024-04-08 11:26:05.706849 datatransformationsbertas-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2697 2024-04-08 10:03:34.134898 datatransformationsbertas-0.3.0/src/datatransformationsbertas/__init__.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.3.0/PKG-INFO
```

### Comparing `datatransformationsbertas-0.2.0/LICENSE` & `datatransformationsbertas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.2.0/README.md` & `datatransformationsbertas-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # Data Tranformation package
+https://pypi.org/project/dataTransformationsBertas/
 
 ## This is a data transformation package to automate daily data scientist tasks.
 #### The package contains: Transpose, Time Series Windowing and Cross-Correlation funcitons. 
 
 # To use them download the package
-`pip install your-package-name`
+`pip install dataTransformationsBertas`
 
 ## And then use it in your python.py file:
-`from dataTransformationBertas import *` - to import all functions. 
+`from datatransformationsbertas import *` - to import all functions. 
 ## If you need them seperately: 
-`from dataTransformationBertas import transpose2d`
-`from dataTransformationBertas import window1d`
-`from dataTransformationBertas import convolution2d`
+`from datatransformationsbertas import transpose2d`
+`from datatransformationsbertas import window1d`
+`from datatransformationsbertas import convolution2d`
 
 ## Example 
 
 ```python 
-from datatransformations import transpose2d
+from datatransformationsbertas import transpose2d
 
 test = transpose2d ([
     [1, 2, 3],
     [4, 5, 6],
     [7, 8, 9]
 ])
 print (test)
 ```
 ```python 
-from datatransformations import window1d
+from datatransformationsbertas import window1d
 input_array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 size = 3
 shift = 2
 stride = 1
 print(window1d(input_array, size, shift, stride))
 ```
 ```python 
-from datatransformations import convolution2d
+from datatransformationsbertas import convolution2d
+import numpy as np
 input_matrix = np.array([[1, 2, 3],
                          [4, 5, 6],
                          [7, 8, 9]])
 
 kernel = np.array([[1, 0, 1],
                    [0, 1, 0],
                    [1, 0, 1]])
```

### Comparing `datatransformationsbertas-0.2.0/src/datatransformationsbertas/__init__.py` & `datatransformationsbertas-0.3.0/src/datatransformationsbertas/__init__.py`

 * *Files identical despite different names*

