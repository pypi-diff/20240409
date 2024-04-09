# Comparing `tmp/datatransformationsbertas-0.6.0.tar.gz` & `tmp/datatransformationsbertas-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransformationsbertas-0.6.0.tar", max compression
+gzip compressed data, was "datatransformationsbertas-0.7.0.tar", max compression
```

## Comparing `datatransformationsbertas-0.6.0.tar` & `datatransformationsbertas-0.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.6.0/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.6.0/README.md
--rw-r--r--   0        0        0      341 2024-04-09 09:00:24.974204 datatransformationsbertas-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2502 2024-04-09 08:59:14.980726 datatransformationsbertas-0.6.0/src/datatransformationsbertas/__init__.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.7.0/README.md
+-rw-r--r--   0        0        0      341 2024-04-09 09:01:48.082165 datatransformationsbertas-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2524 2024-04-09 09:01:40.362905 datatransformationsbertas-0.7.0/src/datatransformationsbertas/__init__.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.7.0/PKG-INFO
```

### Comparing `datatransformationsbertas-0.6.0/LICENSE` & `datatransformationsbertas-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.6.0/README.md` & `datatransformationsbertas-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.6.0/src/datatransformationsbertas/__init__.py` & `datatransformationsbertas-0.7.0/src/datatransformationsbertas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 
     Args:
         input_matrix (list[list[float]]): Matrix as list
 
     Returns:
         list: Switched matrix
     """
-    if not input_matrix:
+    if not input_matrix or not input_matrix[0]:
         return []
 
     cols = len(input_matrix[0])
     return [[input_matrix[i][j] for i in range(len(input_matrix))] for j in range(cols)]
 
 
-
 def window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]:
     """Extracts sliding windows from a 1D array of real numbers,
       such as a time series data.
 
     Args:
         input_array (list | np.ndarray):
         A list or 1D NumPy array of real numbers representing the time series data.
```

### Comparing `datatransformationsbertas-0.6.0/PKG-INFO` & `datatransformationsbertas-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataTransformationsBertas
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tool to automate data scientist daily work
 License: MIT
 Author: Bertoldas
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

