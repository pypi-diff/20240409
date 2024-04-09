# Comparing `tmp/prtools-1.1.0.tar.gz` & `tmp/prtools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prtools-1.1.0.tar", last modified: Tue Feb 13 05:30:14 2024, max compression
+gzip compressed data, was "prtools-1.1.1.tar", last modified: Tue Apr  9 14:16:55 2024, max compression
```

## Comparing `prtools-1.1.0.tar` & `prtools-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-02-13 05:30:14.573705 prtools-1.1.0/
--rw-r--r--   0 akee       (501) staff       (20)     1064 2023-06-13 01:13:17.000000 prtools-1.1.0/LICENSE
--rw-r--r--   0 akee       (501) staff       (20)     2076 2023-11-29 06:11:20.000000 prtools-1.1.0/NOTICE
--rw-r--r--   0 akee       (501) staff       (20)      824 2024-02-13 05:30:14.573770 prtools-1.1.0/PKG-INFO
--rw-r--r--   0 akee       (501) staff       (20)      858 2023-06-13 01:13:17.000000 prtools-1.1.0/README.rst
-drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-02-13 05:30:14.572912 prtools-1.1.0/prtools/
--rw-r--r--   0 akee       (501) staff       (20)      683 2024-02-13 05:07:47.000000 prtools-1.1.0/prtools/__init__.py
--rw-r--r--   0 akee       (501) staff       (20)    17482 2024-02-12 15:45:08.000000 prtools-1.1.0/prtools/array.py
--rw-r--r--   0 akee       (501) staff       (20)     8454 2024-01-21 18:10:10.000000 prtools-1.1.0/prtools/fourier.py
--rw-r--r--   0 akee       (501) staff       (20)     6855 2024-02-12 15:45:08.000000 prtools-1.1.0/prtools/misc.py
--rw-r--r--   0 akee       (501) staff       (20)     3792 2024-02-12 15:45:08.000000 prtools-1.1.0/prtools/segmented.py
--rw-r--r--   0 akee       (501) staff       (20)    10801 2024-02-12 15:45:08.000000 prtools-1.1.0/prtools/shape.py
--rw-r--r--   0 akee       (501) staff       (20)     2360 2024-01-21 17:24:22.000000 prtools-1.1.0/prtools/sparse.py
--rw-r--r--   0 akee       (501) staff       (20)     4109 2024-02-12 15:45:08.000000 prtools-1.1.0/prtools/stats.py
--rw-r--r--   0 akee       (501) staff       (20)    11497 2024-02-12 15:45:08.000000 prtools-1.1.0/prtools/zernike.py
-drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-02-13 05:30:14.573599 prtools-1.1.0/prtools.egg-info/
--rw-r--r--   0 akee       (501) staff       (20)      824 2024-02-13 05:30:14.000000 prtools-1.1.0/prtools.egg-info/PKG-INFO
--rw-r--r--   0 akee       (501) staff       (20)      362 2024-02-13 05:30:14.000000 prtools-1.1.0/prtools.egg-info/SOURCES.txt
--rw-r--r--   0 akee       (501) staff       (20)        1 2024-02-13 05:30:14.000000 prtools-1.1.0/prtools.egg-info/dependency_links.txt
--rw-r--r--   0 akee       (501) staff       (20)       12 2024-02-13 05:30:14.000000 prtools-1.1.0/prtools.egg-info/requires.txt
--rw-r--r--   0 akee       (501) staff       (20)        8 2024-02-13 05:30:14.000000 prtools-1.1.0/prtools.egg-info/top_level.txt
--rw-r--r--   0 akee       (501) staff       (20)      720 2024-02-13 05:30:14.573989 prtools-1.1.0/setup.cfg
--rw-r--r--   0 akee       (501) staff       (20)      122 2023-06-13 01:13:17.000000 prtools-1.1.0/setup.py
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:16:55.277984 prtools-1.1.1/
+-rw-r--r--   0 akee       (501) staff       (20)     1064 2023-06-13 01:13:17.000000 prtools-1.1.1/LICENSE
+-rw-r--r--   0 akee       (501) staff       (20)     2076 2023-11-29 06:11:20.000000 prtools-1.1.1/NOTICE
+-rw-r--r--   0 akee       (501) staff       (20)      824 2024-04-09 14:16:55.278040 prtools-1.1.1/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)      858 2023-06-13 01:13:17.000000 prtools-1.1.1/README.rst
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:16:55.277186 prtools-1.1.1/prtools/
+-rw-r--r--   0 akee       (501) staff       (20)      704 2024-04-09 14:16:25.000000 prtools-1.1.1/prtools/__init__.py
+-rw-r--r--   0 akee       (501) staff       (20)    17482 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/array.py
+-rw-r--r--   0 akee       (501) staff       (20)     8426 2024-04-09 14:16:25.000000 prtools-1.1.1/prtools/fourier.py
+-rw-r--r--   0 akee       (501) staff       (20)     6855 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/misc.py
+-rw-r--r--   0 akee       (501) staff       (20)     3792 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/segmented.py
+-rw-r--r--   0 akee       (501) staff       (20)    10771 2024-04-02 03:32:15.000000 prtools-1.1.1/prtools/shape.py
+-rw-r--r--   0 akee       (501) staff       (20)     2360 2024-01-21 17:24:22.000000 prtools-1.1.1/prtools/sparse.py
+-rw-r--r--   0 akee       (501) staff       (20)     4109 2024-02-12 15:45:08.000000 prtools-1.1.1/prtools/stats.py
+-rw-r--r--   0 akee       (501) staff       (20)    11335 2024-04-03 00:16:47.000000 prtools-1.1.1/prtools/zernike.py
+drwxr-xr-x   0 akee       (501) staff       (20)        0 2024-04-09 14:16:55.277891 prtools-1.1.1/prtools.egg-info/
+-rw-r--r--   0 akee       (501) staff       (20)      824 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/PKG-INFO
+-rw-r--r--   0 akee       (501) staff       (20)      362 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/SOURCES.txt
+-rw-r--r--   0 akee       (501) staff       (20)        1 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/dependency_links.txt
+-rw-r--r--   0 akee       (501) staff       (20)       12 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/requires.txt
+-rw-r--r--   0 akee       (501) staff       (20)        8 2024-04-09 14:16:55.000000 prtools-1.1.1/prtools.egg-info/top_level.txt
+-rw-r--r--   0 akee       (501) staff       (20)      720 2024-04-09 14:16:55.278460 prtools-1.1.1/setup.cfg
+-rw-r--r--   0 akee       (501) staff       (20)      122 2023-06-13 01:13:17.000000 prtools-1.1.1/setup.py
```

### Comparing `prtools-1.1.0/LICENSE` & `prtools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/NOTICE` & `prtools-1.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/PKG-INFO` & `prtools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prtools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility functions for image-based phase retrieval
 Author: Andy Kee
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prtools-1.1.0/README.rst` & `prtools-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/prtools/__init__.py` & `prtools-1.1.1/prtools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 from prtools.array import (
     centroid, pad, boundary, rebin, rescale, normpow,
     shift, register, medfix
     )
 
 from prtools.fourier import dft2, idft2
@@ -23,9 +23,9 @@
     spindex, sparray, spmatrix, spmask
     )
 
 from prtools.stats import ee, rms, pv
 
 from prtools.zernike import (
     zernike, zernike_compose, zernike_basis, zernike_fit, 
-    zernike_remove
+    zernike_remove, zernike_coordinates
     )
```

### Comparing `prtools-1.1.0/prtools/array.py` & `prtools-1.1.1/prtools/array.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/prtools/fourier.py` & `prtools-1.1.1/prtools/fourier.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,23 +115,23 @@
 
 def _dft2_matrices(m, n, M, N, alphar, alphac, shiftr, shiftc, offsetr, offsetc, forward):
     if forward:
         sign = -1
     else:
         sign = 1
     R, S, U, V = _dft2_coords(m, n, M, N)
-    E1 = np.exp(sign*2.0 * 1j * np.pi * alphar * np.outer(R-shiftr+offsetr, U-shiftr)).T
-    E2 = np.exp(sign*2.0 * 1j * np.pi * alphac * np.outer(S-shiftc+offsetc, V-shiftc))
+    E1 = np.exp(sign*2.0 * 1j * np.pi * alphar * np.outer(R+offsetr, U-shiftr)).T
+    E2 = np.exp(sign*2.0 * 1j * np.pi * alphac * np.outer(S+offsetc, V-shiftc))
     return E1, E2
 
 
 def _idft2_matrices(m, n, M, N, alphar, alphac, shiftr, shiftc, offsetr, offsetc):
     R, S, U, V = _dft2_coords(m, n, M, N)
-    E1 = np.exp(2.0 * 1j * np.pi * alphar * np.outer(R-shiftr+offsetr, U-shiftr)).T
-    E2 = np.exp(2.0 * 1j * np.pi * alphac * np.outer(S-shiftc+offsetc, V-shiftc))
+    E1 = np.exp(2.0 * 1j * np.pi * alphar * np.outer(R+offsetr, U-shiftr)).T
+    E2 = np.exp(2.0 * 1j * np.pi * alphac * np.outer(S+offsetc, V-shiftc))
     return E1, E2
 
 
 @functools.lru_cache(maxsize=32)
 def _dft2_coords(m, n, M, N):
     # R and S are (r,c) coordinates in the (m x n) input plane f
     # V and U are (r,c) coordinates in the (M x N) output plane F
```

### Comparing `prtools-1.1.0/prtools/misc.py` & `prtools-1.1.1/prtools/misc.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/prtools/segmented.py` & `prtools-1.1.1/prtools/segmented.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/prtools/shape.py` & `prtools-1.1.1/prtools/shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 def _meshij(shape, shift, angle):
     nr = shape[0]
     nc = shape[1]
     rr, cc = np.meshgrid(np.arange(nr) - np.floor(nr/2.0) - shift[0],
                          np.arange(nc) - np.floor(nc/2.0) - shift[1], 
                          indexing='ij')
-    angle = np.deg2rad(angle)
     r = rr * np.cos(angle) + cc * np.sin(angle)
     c = rr * -np.sin(angle) + cc * np.cos(angle)
     return r, c
 
 
 def circle(shape, radius, shift=(0, 0), antialias=True, indexing='ij'):
     """Draw a circle
```

### Comparing `prtools-1.1.0/prtools/sparse.py` & `prtools-1.1.1/prtools/sparse.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/prtools/stats.py` & `prtools-1.1.1/prtools/stats.py`

 * *Files identical despite different names*

### Comparing `prtools-1.1.0/prtools/zernike.py` & `prtools-1.1.1/prtools/zernike.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,42 +354,40 @@
             row_m.append(row_m[-1])
 
         m = row_m[r] * sign
 
     return m, n
 
 
-def zernike_coordinates(mask, shift=None, angle=0, indexing='ij'):
+def zernike_coordinates(mask, shift=(0,0), angle=0, indexing='ij'):
     """Compute the Zernike coordinate system for a given mask.
     
     Parameters
     ----------
     mask : array_like
         Binary mask defining the extent to compute the Zernike polynomial 
         over.
-    shift : (2,) array_like or None, optional
-        x, y shift of the coordinate system origin in pixels. If None 
-        (default), shift is computed automatically to locate the origin at the
-        mask centroid.
+    shift : (2,) array_like, optional
+        How far to shift center in float (rows, cols). Default is (0, 0).
     angle: float, optional
         Angle to rotate coordinate system by in degrees. rotate is specified 
         relative to the x-axis. Default is 0.
-
+    indexing : {'ij', 'xy'}, optional
+        Matrix ('ij', default) or cartesian ('xy') indexing of output.
+    
+    Returns
+    -------
+    rho, theta : ndarrays
+    
     """
     mask = np.asarray(mask)
 
-    if shift is None:
-        center = np.asarray(mask.shape)/2
-        centroid = prtools.centroid(mask)
-        shift = (centroid[1]-center[1], centroid[0]-center[0])
-
-
-    yy, xx = prtools.mesh(shape=mask.shape, shift=shift, indexing=indexing)
+    yy, xx = prtools.mesh(shape=mask.shape, shift=shift, angle=angle, indexing=indexing)
 
     r = np.abs(xx+1j*yy)
     rho = r/np.max(r*mask)  # rho is defined to be 1 on the edge of the aperture
+    rho[np.where(rho==0)] = 1e-99
 
-    # there is a 90 degree offset since np.angle places 0 degrees up
-    angle = (90-angle) * np.pi/180
-    theta = np.angle(xx*np.exp(1j*angle) + 1j*yy*np.exp(1j*angle))
+    theta = np.angle(xx + 1j*yy)
+    theta[np.where(theta==0)] = 1e-99
 
     return rho, theta
```

### Comparing `prtools-1.1.0/prtools.egg-info/PKG-INFO` & `prtools-1.1.1/prtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prtools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility functions for image-based phase retrieval
 Author: Andy Kee
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prtools-1.1.0/setup.cfg` & `prtools-1.1.1/setup.cfg`

 * *Files identical despite different names*

