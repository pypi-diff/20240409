# Comparing `tmp/datatransformationsbertas-0.7.0.tar.gz` & `tmp/datatransformationsbertas-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransformationsbertas-0.7.0.tar", max compression
+gzip compressed data, was "datatransformationsbertas-0.7.1.tar", max compression
```

## Comparing `datatransformationsbertas-0.7.0.tar` & `datatransformationsbertas-0.7.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.7.0/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.7.0/README.md
--rw-r--r--   0        0        0      341 2024-04-09 09:01:48.082165 datatransformationsbertas-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2524 2024-04-09 09:01:40.362905 datatransformationsbertas-0.7.0/src/datatransformationsbertas/__init__.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.7.1/README.md
+-rw-r--r--   0        0        0      341 2024-04-09 09:11:34.732699 datatransformationsbertas-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2606 2024-04-09 09:11:28.923958 datatransformationsbertas-0.7.1/src/datatransformationsbertas/__init__.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.7.1/PKG-INFO
```

### Comparing `datatransformationsbertas-0.7.0/LICENSE` & `datatransformationsbertas-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.7.0/README.md` & `datatransformationsbertas-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.7.0/src/datatransformationsbertas/__init__.py` & `datatransformationsbertas-0.7.1/src/datatransformationsbertas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,20 @@
     Returns:
         list[list | np.ndarray]: Returns a list of lists or 1D NumPy arrays,
         containing the windows extracted from the input array.
     """
     if isinstance(input_array, list):
         input_array = np.array(input_array)
 
-    return [input_array[i:i+size:stride] for i in range(0, len(input_array) - size + 1, shift)]
+    if len(input_array) == 0:
+        return []
 
+    windows = [input_array[i:i + size:stride].tolist() for i in range(0, len(input_array) - size + 1, shift)]
+
+    return windows
 
 def convolution2d(
     input_matrix: np.ndarray, kernel: np.ndarray, stride: int = 1
 ) -> np.ndarray:
     """Performs a 2D convolution operation between an input matrix and a kernel matrix.
 
     Args:
```

### Comparing `datatransformationsbertas-0.7.0/PKG-INFO` & `datatransformationsbertas-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataTransformationsBertas
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tool to automate data scientist daily work
 License: MIT
 Author: Bertoldas
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

