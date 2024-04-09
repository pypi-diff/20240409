# Comparing `tmp/datatransformationsbertas-0.3.0.tar.gz` & `tmp/datatransformationsbertas-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransformationsbertas-0.3.0.tar", max compression
+gzip compressed data, was "datatransformationsbertas-0.4.0.tar", max compression
```

## Comparing `datatransformationsbertas-0.3.0.tar` & `datatransformationsbertas-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.3.0/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.3.0/README.md
--rw-r--r--   0        0        0      341 2024-04-08 11:26:05.706849 datatransformationsbertas-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2697 2024-04-08 10:03:34.134898 datatransformationsbertas-0.3.0/src/datatransformationsbertas/__init__.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.4.0/README.md
+-rw-r--r--   0        0        0      341 2024-04-09 08:42:59.846382 datatransformationsbertas-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2461 2024-04-09 08:42:37.849387 datatransformationsbertas-0.4.0/src/datatransformationsbertas/__init__.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.4.0/PKG-INFO
```

### Comparing `datatransformationsbertas-0.3.0/LICENSE` & `datatransformationsbertas-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.3.0/README.md` & `datatransformationsbertas-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.3.0/src/datatransformationsbertas/__init__.py` & `datatransformationsbertas-0.4.0/src/datatransformationsbertas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,63 @@
-import numpy as np 
+import numpy as np
 
 def transpose2d(input_matrix: list[list[float]]) -> list:
     """Transpose function that switches the axes of a tensor
 
     Args:
-        input_matrix (list[list[float]]): Matrix as list 
-
+        input_matrix (list[list[float]]): Matrix as list
     Returns:
-        list: Switched matrix 
+        list: Switched matrix
     """
-    
-    rows = len(input_matrix)
-    cols = len(input_matrix[0])
+    return [
+        [input_matrix[i][j] for i in range(len(input_matrix))]
+        for j in range(len(input_matrix[0]))
+    ]
 
-    transposed_matrix = [[0] * rows for _ in range(cols)]
 
-    for i in range(rows):
-        for j in range(cols):
-            transposed_matrix[j][i] = input_matrix[i][j]
-
-    return transposed_matrix
 
 def window1d(input_array: list | np.ndarray, size: int, shift: int = 1, stride: int = 1) -> list[list | np.ndarray]:
     """Extracts sliding windows from a 1D array of real numbers,
       such as a time series data.
 
     Args:
-        input_array (list | np.ndarray): A list or 1D NumPy array of real numbers representing the time series data.
+        input_array (list | np.ndarray):
+        A list or 1D NumPy array of real numbers representing the time series data.
         size (int): An integer specifying the size of the window.
         shift (int, optional): Step size between different windows. Defaults to 1.
         stride (int, optional): Step size between each windows. Defaults to 1.
 
     Returns:
         list[list | np.ndarray]: Returns a list of lists or 1D NumPy arrays,
         containing the windows extracted from the input array.
-
-
     """
     if isinstance(input_array, list):
-        input_array = np.array(input_array) 
+        input_array = np.array(input_array)
 
-    windows = []
-    for i in range(0, len(input_array) - size + 1, shift):
-        window = input_array[i:i+size:stride]
-        windows.append(window)
+    return [input_array[i:i+size:stride] for i in range(0, len(input_array) - size + 1, shift)]
 
-    return windows
 
-def convolution2d(input_matrix: np.ndarray, kernel: np.ndarray, stride : int = 1) -> np.ndarray:
+def convolution2d(
+    input_matrix: np.ndarray, kernel: np.ndarray, stride: int = 1
+) -> np.ndarray:
     """Performs a 2D convolution operation between an input matrix and a kernel matrix.
 
     Args:
-        input_matrix (np.ndarray): A 2D NumPy array of real numbers representing the input image or feature map.
-        kernel (np.ndarray): A 2D NumPy array of real numbers representing the convolution kernel or filter.
+        input_matrix (np.ndarray):
+          A 2D NumPy array of real numbers representing the input image or feature map.
+        kernel (np.ndarray):
+          A 2D NumPy array of real numbers representing the convolution kernel or filter.
         stride (int, optional): Step size for the convolution operation. Defaults to 1.
 
     Returns:
         np.ndarray: Returns a 2D Numpy array of real numbers
     """
 
     input_height, input_width = input_matrix.shape
     kernel_height, kernel_width = kernel.shape
     output_height = (input_height - kernel_height) // stride + 1
     output_width = (input_width - kernel_width) // stride + 1
-    output_matrix = np.zeros((output_height, output_width))
-
-    for i in range(0, input_height - kernel_height + 1, stride):
-        for j in range(0, input_width - kernel_width + 1, stride):
-            roi = input_matrix[i:i+kernel_height, j:j+kernel_width]
-            output_matrix[i//stride, j//stride] = np.sum(roi * kernel)
-    return output_matrix
+    output_matrix = np.array([[np.sum(input_matrix[i:i+kernel_height, j:j+kernel_width] * kernel)
+                               for j in range(0, input_width - kernel_width + 1, stride)]
+                              for i in range(0, input_height - kernel_height + 1, stride)])
+    
+    return output_matrix
```

### Comparing `datatransformationsbertas-0.3.0/PKG-INFO` & `datatransformationsbertas-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataTransformationsBertas
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tool to automate data scientist daily work
 License: MIT
 Author: Bertoldas
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

