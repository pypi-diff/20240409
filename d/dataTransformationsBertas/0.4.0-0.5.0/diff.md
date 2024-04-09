# Comparing `tmp/datatransformationsbertas-0.4.0.tar.gz` & `tmp/datatransformationsbertas-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransformationsbertas-0.4.0.tar", max compression
+gzip compressed data, was "datatransformationsbertas-0.5.0.tar", max compression
```

## Comparing `datatransformationsbertas-0.4.0.tar` & `datatransformationsbertas-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.4.0/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.4.0/README.md
--rw-r--r--   0        0        0      341 2024-04-09 08:42:59.846382 datatransformationsbertas-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2461 2024-04-09 08:42:37.849387 datatransformationsbertas-0.4.0/src/datatransformationsbertas/__init__.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.5.0/README.md
+-rw-r--r--   0        0        0      341 2024-04-09 08:52:35.710181 datatransformationsbertas-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2628 2024-04-09 08:52:04.995885 datatransformationsbertas-0.5.0/src/datatransformationsbertas/__init__.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.5.0/PKG-INFO
```

### Comparing `datatransformationsbertas-0.4.0/LICENSE` & `datatransformationsbertas-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.4.0/README.md` & `datatransformationsbertas-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.4.0/src/datatransformationsbertas/__init__.py` & `datatransformationsbertas-0.5.0/src/datatransformationsbertas/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import numpy as np
 
 def transpose2d(input_matrix: list[list[float]]) -> list:
     """Transpose function that switches the axes of a tensor
 
     Args:
         input_matrix (list[list[float]]): Matrix as list
+
     Returns:
         list: Switched matrix
     """
-    return [
-        [input_matrix[i][j] for i in range(len(input_matrix))]
-        for j in range(len(input_matrix[0]))
-    ]
+    if not input_matrix:  # Check if input_matrix is empty
+        return []
+
+    rows = len(input_matrix)
+    cols = len(input_matrix[0]) if input_matrix else 0  # Get the number of columns, handle empty matrix case
+    return [[input_matrix[i][j] for i in range(rows)] for j in range(cols)]
 
 
 
 def window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]:
     """Extracts sliding windows from a 1D array of real numbers,
       such as a time series data.
```

### Comparing `datatransformationsbertas-0.4.0/PKG-INFO` & `datatransformationsbertas-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataTransformationsBertas
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tool to automate data scientist daily work
 License: MIT
 Author: Bertoldas
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

