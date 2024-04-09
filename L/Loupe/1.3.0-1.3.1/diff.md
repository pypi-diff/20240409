# Comparing `tmp/Loupe-1.3.0.tar.gz` & `tmp/Loupe-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Loupe-1.3.0.tar", last modified: Sat Feb 10 03:35:45 2024, max compression
+gzip compressed data, was "Loupe-1.3.1.tar", last modified: Tue Apr  9 14:18:41 2024, max compression
```

## Comparing `Loupe-1.3.0.tar` & `Loupe-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:35:45.835848 Loupe-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-10 03:35:30.000000 Loupe-1.3.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:35:45.835848 Loupe-1.3.0/Loupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-10 03:35:45.000000 Loupe-1.3.0/Loupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-10 03:35:45.000000 Loupe-1.3.0/Loupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 03:35:45.000000 Loupe-1.3.0/Loupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-10 03:35:45.000000 Loupe-1.3.0/Loupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-10 03:35:45.000000 Loupe-1.3.0/Loupe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-02-10 03:35:30.000000 Loupe-1.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-10 03:35:45.835848 Loupe-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-10 03:35:30.000000 Loupe-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:35:45.835848 Loupe-1.3.0/loupe/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/einsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10826 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/special.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/tensordot.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-02-10 03:35:30.000000 Loupe-1.3.0/loupe/zernike.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-10 03:35:45.835848 Loupe-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-10 03:35:30.000000 Loupe-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:35:45.835848 Loupe-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_einsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_special.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_tensordot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-10 03:35:30.000000 Loupe-1.3.0/tests/test_zernike.py
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:18:41.778767 Loupe-1.3.1/
+-rw-r--r--   0 akee       (501) staff       (20)     1516 2023-06-13 01:13:06.000000 Loupe-1.3.1/LICENSE
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:18:41.775365 Loupe-1.3.1/Loupe.egg-info/
+-rw-r--r--   0 akee       (501) staff       (20)     2179 2024-04-09 14:18:41.000000 Loupe-1.3.1/Loupe.egg-info/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)      384 2024-04-09 14:18:41.000000 Loupe-1.3.1/Loupe.egg-info/SOURCES.txt
+-rw-r--r--   0 akee       (501) staff       (20)        1 2024-04-09 14:18:41.000000 Loupe-1.3.1/Loupe.egg-info/dependency_links.txt
+-rw-r--r--   0 akee       (501) staff       (20)       12 2024-04-09 14:18:41.000000 Loupe-1.3.1/Loupe.egg-info/requires.txt
+-rw-r--r--   0 akee       (501) staff       (20)        6 2024-04-09 14:18:41.000000 Loupe-1.3.1/Loupe.egg-info/top_level.txt
+-rw-r--r--   0 akee       (501) staff       (20)     3137 2023-06-13 01:13:06.000000 Loupe-1.3.1/NOTICE
+-rw-r--r--   0 akee       (501) staff       (20)     2179 2024-04-09 14:18:41.778830 Loupe-1.3.1/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)     1248 2023-06-13 01:13:06.000000 Loupe-1.3.1/README.rst
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:18:41.778400 Loupe-1.3.1/loupe/
+-rw-r--r--   0 akee       (501) staff       (20)      782 2024-04-09 14:18:27.000000 Loupe-1.3.1/loupe/__init__.py
+-rw-r--r--   0 akee       (501) staff       (20)     8909 2023-12-13 04:22:46.000000 Loupe-1.3.1/loupe/core.py
+-rw-r--r--   0 akee       (501) staff       (20)     6896 2024-02-10 03:26:56.000000 Loupe-1.3.1/loupe/cost.py
+-rw-r--r--   0 akee       (501) staff       (20)     3432 2023-06-13 01:13:06.000000 Loupe-1.3.1/loupe/einsum.py
+-rw-r--r--   0 akee       (501) staff       (20)     7712 2024-04-09 14:18:27.000000 Loupe-1.3.1/loupe/fourier.py
+-rw-r--r--   0 akee       (501) staff       (20)    10826 2023-12-10 05:46:27.000000 Loupe-1.3.1/loupe/numeric.py
+-rw-r--r--   0 akee       (501) staff       (20)     6302 2023-12-05 14:20:23.000000 Loupe-1.3.1/loupe/optimize.py
+-rw-r--r--   0 akee       (501) staff       (20)     2735 2023-06-13 01:13:06.000000 Loupe-1.3.1/loupe/shape.py
+-rw-r--r--   0 akee       (501) staff       (20)     3318 2024-02-10 02:00:46.000000 Loupe-1.3.1/loupe/special.py
+-rw-r--r--   0 akee       (501) staff       (20)     4738 2023-06-13 01:13:06.000000 Loupe-1.3.1/loupe/tensordot.py
+-rw-r--r--   0 akee       (501) staff       (20)    10159 2023-06-13 01:13:06.000000 Loupe-1.3.1/loupe/util.py
+-rw-r--r--   0 akee       (501) staff       (20)    11966 2023-06-13 01:13:06.000000 Loupe-1.3.1/loupe/zernike.py
+-rw-r--r--   0 akee       (501) staff       (20)      955 2024-04-09 14:18:41.779078 Loupe-1.3.1/setup.cfg
+-rw-r--r--   0 akee       (501) staff       (20)      256 2023-06-13 01:13:06.000000 Loupe-1.3.1/setup.py
```

### Comparing `Loupe-1.3.0/LICENSE` & `Loupe-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/Loupe.egg-info/PKG-INFO` & `Loupe-1.3.1/Loupe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loupe
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python library for solving parametric optimization problems with built-in autograd.
 Home-page: https://loupe.readthedocs.io
 Author: Andy Kee
 License: BSD-3-Clause
 Project-URL: Documentation, https://loupe.readthedocs.io
 Project-URL: Code, https://github.com/andykee/loupe
 Project-URL: Issue tracker, https://github.com/andykee/loupe/issues
@@ -16,16 +16,14 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
-Requires-Dist: numpy
-Requires-Dist: scipy
 
 Loupe
 =====
 |build status| |coverage| |docs status| |pypi version|
 
 Loupe is a Python library for solving parametric optimization problems. Loupe makes 
 it easy to build and manipulate numerical models and efficiently solve optimization
```

### Comparing `Loupe-1.3.0/NOTICE` & `Loupe-1.3.1/NOTICE`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/PKG-INFO` & `Loupe-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Loupe
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python library for solving parametric optimization problems with built-in autograd.
 Home-page: https://loupe.readthedocs.io
 Author: Andy Kee
 License: BSD-3-Clause
 Project-URL: Documentation, https://loupe.readthedocs.io
 Project-URL: Code, https://github.com/andykee/loupe
 Project-URL: Issue tracker, https://github.com/andykee/loupe/issues
@@ -16,16 +16,14 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
-Requires-Dist: numpy
-Requires-Dist: scipy
 
 Loupe
 =====
 |build status| |coverage| |docs status| |pypi version|
 
 Loupe is a Python library for solving parametric optimization problems. Loupe makes 
 it easy to build and manipulate numerical models and efficiently solve optimization
```

### Comparing `Loupe-1.3.0/README.rst` & `Loupe-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/__init__.py` & `Loupe-1.3.1/loupe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 from loupe.core import array
 
 from loupe.cost import sserror
 
 from loupe.einsum import einsum
```

### Comparing `Loupe-1.3.0/loupe/core.py` & `Loupe-1.3.1/loupe/core.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/cost.py` & `Loupe-1.3.1/loupe/cost.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/einsum.py` & `Loupe-1.3.1/loupe/einsum.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/fourier.py` & `Loupe-1.3.1/loupe/fourier.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,22 +204,20 @@
     mask = np.ones(3, dtype=bool)
     mask[axes] = False
     return np.squeeze(np.arange(3)[mask])
 
 
 def _dft2_matrices(m, n, M, N, alphar, alphac, shiftr, shiftc, offsetr, offsetc):
     R, S, U, V = _dft2_coords(m, n, M, N)
-    E1 = np.exp(-2.0 * 1j * np.pi * alphar * np.outer(R-shiftr+offsetr, U-shiftr)).T
-    E2 = np.exp(-2.0 * 1j * np.pi * alphac * np.outer(S-shiftc+offsetc, V-shiftc))
+    E1 = np.exp(-2.0 * 1j * np.pi * alphar * np.outer(R+offsetr, U-shiftr)).T
+    E2 = np.exp(-2.0 * 1j * np.pi * alphac * np.outer(S+offsetc, V-shiftc))
     return E1, E2
 
 @functools.lru_cache(maxsize=32)
 def _dft2_coords(m, n, M, N):
     # R and S are (r,c) coordinates in the (m x n) input plane f
-    # V and U are (r,c) coordinates in the (M x N) output plane F
-
+    # U and V are (r,c) coordinates in the (M x N) output plane F
     R = np.arange(m) - np.floor(m/2.0)
     S = np.arange(n) - np.floor(n/2.0)
     U = np.arange(M) - np.floor(M/2.0)
     V = np.arange(N) - np.floor(N/2.0)
-
     return R, S, U, V
```

### Comparing `Loupe-1.3.0/loupe/numeric.py` & `Loupe-1.3.1/loupe/numeric.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/optimize.py` & `Loupe-1.3.1/loupe/optimize.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/shape.py` & `Loupe-1.3.1/loupe/shape.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/special.py` & `Loupe-1.3.1/loupe/special.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/tensordot.py` & `Loupe-1.3.1/loupe/tensordot.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/util.py` & `Loupe-1.3.1/loupe/util.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/loupe/zernike.py` & `Loupe-1.3.1/loupe/zernike.py`

 * *Files identical despite different names*

### Comparing `Loupe-1.3.0/setup.cfg` & `Loupe-1.3.1/setup.cfg`

 * *Files identical despite different names*

