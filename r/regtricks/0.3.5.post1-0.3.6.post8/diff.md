# Comparing `tmp/regtricks-0.3.5.post1.tar.gz` & `tmp/regtricks-0.3.6.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regtricks-0.3.5.post1.tar", last modified: Thu Jul 20 21:23:44 2023, max compression
+gzip compressed data, was "regtricks-0.3.6.post8.tar", last modified: Tue Apr  9 14:21:35 2024, max compression
```

## Comparing `regtricks-0.3.5.post1.tar` & `regtricks-0.3.6.post8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.879392 regtricks-0.3.5.post1/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/LICENSE
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/MANIFEST.in
--rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-07-20 21:23:44.879155 regtricks-0.3.5.post1/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/README.md
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.877230 regtricks-0.3.5.post1/regtricks/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/__init__.py
--rw-r--r--   0 thomaskirk   (501) staff       (20)       77 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks/_version.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7424 2023-07-10 10:27:24.000000 regtricks-0.3.5.post1/regtricks/application_helpers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15302 2023-07-09 12:24:53.000000 regtricks-0.3.5.post1/regtricks/fnirt_coefficients.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11883 2023-07-10 10:23:15.000000 regtricks-0.3.5.post1/regtricks/image_space.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/multiplication.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.878972 regtricks-0.3.5.post1/regtricks/transforms/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/transforms/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11570 2023-07-09 13:14:48.000000 regtricks-0.3.5.post1/regtricks/transforms/linear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14424 2023-07-10 10:04:05.000000 regtricks-0.3.5.post1/regtricks/transforms/nonlinear.py
--rwxr-xr-x   0 thomaskirk   (501) staff       (20)     9434 2023-07-20 21:23:08.000000 regtricks-0.3.5.post1/regtricks/transforms/transform.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3238 2023-07-09 13:15:39.000000 regtricks-0.3.5.post1/regtricks/wrappers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/regtricks/x5_interface.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-20 21:23:44.878108 regtricks-0.3.5.post1/regtricks.egg-info/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/SOURCES.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/dependency_links.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/requires.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-07-20 21:23:44.000000 regtricks-0.3.5.post1/regtricks.egg-info/top_level.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.5.post1/requirements.txt
--rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-07-20 21:23:44.879438 regtricks-0.3.5.post1/setup.cfg
--rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.5.post1/setup.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2024-04-09 14:21:35.013124 regtricks-0.3.6.post8/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/LICENSE
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/MANIFEST.in
+-rw-r--r--   0 thomaskirk   (501) staff       (20)     1100 2024-04-09 14:21:35.012982 regtricks-0.3.6.post8/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/README.md
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2024-04-09 14:21:35.011062 regtricks-0.3.6.post8/regtricks/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/regtricks/__init__.py
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       77 2024-04-09 14:21:34.000000 regtricks-0.3.6.post8/regtricks/_version.py
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     7279 2024-01-06 17:47:05.000000 regtricks-0.3.6.post8/regtricks/application_helpers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15423 2024-01-24 21:03:24.000000 regtricks-0.3.6.post8/regtricks/fnirt_coefficients.py
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)    11994 2024-01-04 16:23:56.000000 regtricks-0.3.6.post8/regtricks/image_space.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/regtricks/multiplication.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2024-04-09 14:21:35.012632 regtricks-0.3.6.post8/regtricks/transforms/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/regtricks/transforms/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11570 2023-07-09 13:14:48.000000 regtricks-0.3.6.post8/regtricks/transforms/linear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14398 2024-01-06 18:11:28.000000 regtricks-0.3.6.post8/regtricks/transforms/nonlinear.py
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)    10369 2024-02-23 16:50:13.000000 regtricks-0.3.6.post8/regtricks/transforms/transform.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3238 2023-07-09 13:15:39.000000 regtricks-0.3.6.post8/regtricks/wrappers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/regtricks/x5_interface.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2024-04-09 14:21:35.011811 regtricks-0.3.6.post8/regtricks.egg-info/
+-rw-r--r--   0 thomaskirk   (501) staff       (20)     1100 2024-04-09 14:21:34.000000 regtricks-0.3.6.post8/regtricks.egg-info/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2024-04-09 14:21:35.000000 regtricks-0.3.6.post8/regtricks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2024-04-09 14:21:34.000000 regtricks-0.3.6.post8/regtricks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2024-04-09 14:21:34.000000 regtricks-0.3.6.post8/regtricks.egg-info/requires.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2024-04-09 14:21:34.000000 regtricks-0.3.6.post8/regtricks.egg-info/top_level.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.6.post8/requirements.txt
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2024-04-09 14:21:35.013176 regtricks-0.3.6.post8/setup.cfg
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3588 2024-01-04 16:23:56.000000 regtricks-0.3.6.post8/setup.py
```

### Comparing `regtricks-0.3.5.post1/LICENSE` & `regtricks-0.3.6.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/PKG-INFO` & `regtricks-0.3.6.post8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.5.post1
+Version: 0.3.6.post8
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
-Author-email: thomas.kirk@eng.ox.ac.uk
+Author-email: tomfrankkirk@gmail.com
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Regtricks
 Tools for manipulating, combining and applying image transformations.
```

### Comparing `regtricks-0.3.5.post1/README.md` & `regtricks-0.3.6.post8/README.md`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/application_helpers.py` & `regtricks-0.3.6.post8/regtricks/application_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,213 +1,224 @@
 import functools
-import multiprocessing as mp 
-from pathlib import Path 
+import multiprocessing as mp
+from pathlib import Path
 
 import nibabel
-from nibabel import Nifti1Image, MGHImage
+import numpy as np
 from fsl.data.image import Image as FSLImage
-import numpy as np 
+from nibabel import MGHImage, Nifti1Image
 from scipy.ndimage import map_coordinates
 
 
 def src_load_helper(src):
     if isinstance(src, (str, Path)):
         src = nibabel.load(src)
         data = src.get_fdata()
     elif isinstance(src, (Nifti1Image, MGHImage)):
         data = src.get_fdata()
     elif isinstance(src, FSLImage):
         data = src.data
-    else: 
-        raise RuntimeError("src must be a nibabel Nifti/MGH, FSL Image," 
-                           " or path to image")
+    else:
+        raise RuntimeError(
+            "src must be a nibabel Nifti/MGH, FSL Image," " or path to image"
+        )
 
     return data, type(src)
 
 
 def _make_iterable(data, series_length):
     """
     Ensure array is 4D, with the fourth dimension at the front (ie, T, XYZ).
     3D volumes will be expanded with a singleton dimension: 1, XYZ
-    Used for iterating over the volumes of a series. 
+    Used for iterating over the volumes of a series.
     """
-    if len(data.shape) == 4: 
+    if len(data.shape) == 4:
         return np.moveaxis(data, 3, 0)
-    elif series_length == 1: 
+    elif series_length == 1:
         return data.reshape(1, *data.shape)
-    else: 
-        assert data.ndim == 3, 'series expansion should be with 3D volume'
-        return [ data ] * series_length
+    else:
+        assert data.ndim == 3, "series expansion should be with 3D volume"
+        return [data] * series_length
 
 
-def interpolate_and_scale(idx, data, transform, src_spc, ref_spc, **kwargs):
+def interpolate_and_scale(
+    idx, data, transform, src_spc, ref_spc, superfactor, **kwargs
+):
     """
     Used for partial function application to share interpolation jobs
     amongst workers of a mp.Pool(). Interpolate data onto the coordinates
     given in the tuple coords_scale, and multiply the output by the other
-    value in coords_scale. Reshape the output to size out_size. 
+    value in coords_scale. Reshape the output to size out_size.
 
-    Args: 
-        data (np.ndarray): 3D, image data 
+    Args:
+        data (np.ndarray): 3D, image data
         coords_scale (np.ndarray, np.ndarray): (N,3) coordinates to interpolate
             onto (indices into data array), value by which to scale output
             (int or another np.ndarray for intensity correction)
         out_size (np.ndarray): 3-vector, shape of output
         **kwargs: passed onto scipy map_coordinates
 
-    Returns: 
-       (np.ndarray), sized as out_size, interpolated output 
+    Returns:
+       (np.ndarray), sized as out_size, interpolated output
     """
 
-    # We transform a bool mask along with the input data to guard
-    # against spline interpolation artefacts in the transformed data 
-    superfactor = kwargs.pop('superfactor')
     ijk, scale = transform.resolve(src_spc, ref_spc, idx)
-    interp = map_coordinates(data, ijk, mode='constant', 
-                             prefilter=True, **kwargs)
+    interp = map_coordinates(data, ijk, mode="constant", prefilter=True, **kwargs)
 
     # If the fill value has been specified, set the min/max
-    # range for clipping in light of this 
-    if 'cval' in kwargs:
-        cval = kwargs['cval']
+    # range for clipping in light of this
+    if "cval" in kwargs:
+        cval = kwargs["cval"]
         cmin = data.min() if cval > data.min() else cval
-        cmax = data.max() if cval < data.max() else cval 
-    else: 
-        cmin = data.min() 
+        cmax = data.max() if cval < data.max() else cval
+    else:
+        cmin = data.min()
         cmax = data.max()
 
     # Clip output values to the required min max
     interp = np.clip(interp, cmin, cmax)
-    interp = interp.reshape(ref_spc.size) * scale 
+    interp = interp.reshape(ref_spc.size) * scale
 
-    # If supersampling used, sum array blocks back down to target 
+    # If supersampling used, sum array blocks back down to target
     if (superfactor > 1).any():
         interp = sum_array_blocks(interp, superfactor)
         interp = interp / np.prod(superfactor)
-    
+
     return interp
 
 
 def despatch(data, transform, src_spc, ref_spc, cores, **kwargs):
     """
-    Apply a transform to an array of data, mapping from source space 
-    to reference. Essentially this is an extended wrapper for Scipy 
-    map_coordinates. 
+    Apply a transform to an array of data, mapping from source space
+    to reference. Essentially this is an extended wrapper for Scipy
+    map_coordinates.
 
-    Args: 
+    Args:
         data (array): np.array of data (3D or 4D)
-        transform (Transformation): between source and reference space 
+        transform (Transformation): between source and reference space
         src_spc (ImageSpace): in which data currently lies
         ref_spc (ImageSpace): towards which data will be transformed
         cores (int): number of cores to use (for 4D data)
         **kwargs: passed onto scipy.ndimage.interpolate.map_coordinates
 
-    Returns: 
-        (np.array) transformed data 
+    Returns:
+        (np.array) transformed data
     """
 
-    if data.ndim not in (3,4): 
+    if data.ndim not in (3, 4):
         raise RuntimeError("Can only handle 3D/4D data")
-            
-    if ((data.ndim == 4) and (len(transform) > 1) and 
-        (len(transform)) != data.shape[3]):
-        raise RuntimeError("Number of volumes in 4D series does not match "
-                "length of transformation series")
 
-    if len(transform) == 1: 
+    if (data.ndim == 4) and (len(transform) > 1) and (len(transform)) != data.shape[3]:
+        raise RuntimeError(
+            "Number of volumes in 4D series does not match "
+            "length of transformation series"
+        )
+
+    if len(transform) == 1:
         series_length = 1 if data.ndim == 3 else data.shape[3]
-    else: 
+    else:
         series_length = len(transform)
 
-    # Make the data 4D so that the workers of the pool can iterate over it 
+    # Make the data 4D so that the workers of the pool can iterate over it
     # Each worker recieves a tuple of (vol, idx), one frame of the series and
     # its corresponding index number (which is used to get the correct bit
-    # of the transform). Pre-calculate and cache any information that can be 
-    # shared amongst the workers 
+    # of the transform). Pre-calculate and cache any information that can be
+    # shared amongst the workers
     data = _make_iterable(data, series_length)
     transform.prepare_cache(ref_spc)
     worker_args = zip(range(series_length), data)
-    worker = functools.partial(interpolate_and_scale, 
-        transform=transform, ref_spc=ref_spc, src_spc=src_spc, **kwargs)
-
-    # Distribute amongst workers 
-    if cores == 1:  
-        resamp = [ worker(*vc) for vc in worker_args ] 
-    else: 
-        with mp.Pool(cores) as p: 
+    worker = functools.partial(
+        interpolate_and_scale,
+        transform=transform,
+        ref_spc=ref_spc,
+        src_spc=src_spc,
+        **kwargs
+    )
+
+    # Distribute amongst workers
+    if cores == 1:
+        resamp = [worker(*vc) for vc in worker_args]
+    else:
+        with mp.Pool(cores) as p:
             resamp = p.starmap(worker, worker_args)
 
-    # Stack all the individual volumes back up in time dimension 
-    # Clip the array to the original min/max values 
-    # Reset the cache on the transform to be safe. 
+    # Stack all the individual volumes back up in time dimension
+    # Clip the array to the original min/max values
+    # Reset the cache on the transform to be safe.
     transform.reset_cache()
     resamp = np.stack(resamp, axis=3)
-    if resamp.shape[3] == 1: 
-        resamp = np.squeeze(resamp, axis=3) 
+    if resamp.shape[3] == 1:
+        resamp = np.squeeze(resamp, axis=3)
     return resamp
 
 
-def aff_trans(matrix, points): 
+def aff_trans(matrix, points):
     """Affine transform a 3D set of points"""
 
-    if not matrix.shape == (4,4): 
+    if not matrix.shape == (4, 4):
         raise ValueError("Matrix needs to be a 4x4 array")
 
-    if points.shape[1] == 3: 
-        transpose = True 
-        points = points.T 
-    else: 
-        transpose = False 
+    if points.shape[1] == 3:
+        transpose = True
+        points = points.T
+    else:
+        transpose = False
 
     p = np.ones((4, points.shape[1]))
-    p[:3,:] = points 
-    t = matrix @ p 
+    p[:3, :] = points
+    t = matrix @ p
+
+    if transpose:
+        return t[:3, :].T
+    else:
+        return t[:3, :]
 
-    if transpose: 
-        return t[:3,:].T
-    else: 
-        return t[:3,:]
 
 def sum_array_blocks(array, factor):
-    """Sum sub-arrays of a larger array, each of which is sized according to factor. 
-    The array is split into smaller subarrays of size given by factor, each of which 
-    is summed, and the results returned in a new array, shrunk accordingly. 
+    """Sum sub-arrays of a larger array, each of which is sized according to factor.
+    The array is split into smaller subarrays of size given by factor, each of which
+    is summed, and the results returned in a new array, shrunk accordingly.
 
     Args:
         array: n-dimensional array of data to sum
         factor: n-length tuple, size of sub-arrays to sum over
 
     Returns:
-        array of size array.shape/factor, each element containing the sum of the 
+        array of size array.shape/factor, each element containing the sum of the
             corresponding subarray in the input
     """
 
     if len(factor) != len(array.shape):
         raise RuntimeError("factor must be of same length as number of dimensions")
 
     if np.any(np.mod(factor, np.ones_like(factor))):
         raise RuntimeError("factor must be of integer values only")
 
     factor = np.array(factor, dtype=int)
-    if (np.mod(array.shape, factor) > 0).any(): 
-        raise RuntimeError(("Factor {} must be a perfect divisor of array shape {}".
-            format(factor, array.shape)))
+    if (np.mod(array.shape, factor) > 0).any():
+        raise RuntimeError(
+            (
+                "Factor {} must be a perfect divisor of array shape {}".format(
+                    factor, array.shape
+                )
+            )
+        )
 
-    outshape = [ int(s/f) for (s,f) in zip(array.shape, factor) ]
+    outshape = [int(s / f) for (s, f) in zip(array.shape, factor)]
     out = np.copy(array)
 
     for dim in range(3):
         newshape = [0] * 4
 
         for d in range(3):
-            if d < dim: 
+            if d < dim:
                 newshape[d] = outshape[d]
-            elif d == dim: 
-                newshape[d+1] = factor[d]
+            elif d == dim:
+                newshape[d + 1] = factor[d]
                 newshape[d] = outshape[d]
-            else: 
-                newshape[d+1] = array.shape[d]
+            else:
+                newshape[d + 1] = array.shape[d]
 
         newshape = newshape + list(array.shape[3:])
-        out = np.sum(out.reshape(newshape), axis=dim+1)
+        out = np.sum(out.reshape(newshape), axis=dim + 1)
 
-    return out 
+    return out
```

### Comparing `regtricks-0.3.5.post1/regtricks/fnirt_coefficients.py` & `regtricks-0.3.6.post8/regtricks/fnirt_coefficients.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,395 +1,420 @@
-import tempfile 
+import tempfile
 import subprocess
-import os.path as op 
-import warnings 
+import os.path as op
+import shutil
+import warnings
 from pathlib import Path
 
-import nibabel 
-import numpy as np 
+import nibabel
+import numpy as np
 
 from regtricks.image_space import ImageSpace
 from regtricks.application_helpers import aff_trans
 
+
 class FNIRTCoefficients(object):
     """
-    Private encapsulation of FNIRT warp field. Only to be used 
+    Private encapsulation of FNIRT warp field. Only to be used
     from within a NonLinearTransformation
 
-    Args: 
+    Args:
         coeffs; nibabel object or path to coefficients file
         src: Pathlike or ImageSpace, path to original source for transform
         ref: Pathlike or ImageSpace, path to original reference for transform
         constrain_jac (bool/tuple): constrain the Jacobian of the transform
-            (default False). If True, default limits of (0.01, 100) are used, 
-            otherwise the limits (min,max) can be passed directly. 
+            (default False). If True, default limits of (0.01, 100) are used,
+            otherwise the limits (min,max) can be passed directly.
     """
 
     def __init__(self, coeffs, src, ref, constrain_jac=False):
         if isinstance(coeffs, (str, Path)):
             coeffs = nibabel.load(coeffs)
-        else: 
+        else:
             assert isinstance(coeffs, nibabel.Nifti1Image)
 
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
-        self.ref_spc = ref 
+        self.ref_spc = ref
 
         if not isinstance(src, ImageSpace):
             src = ImageSpace(src)
-        self.src_spc = src 
+        self.src_spc = src
 
-        if constrain_jac == True: 
+        if constrain_jac == True:
             self.constrain_jac = (0.01, 100)
-        elif constrain_jac == False: 
+        elif constrain_jac == False:
             self.constrain_jac = (None, None)
-        else: 
-            if not all([ isinstance(j, (int, float)) for j in constrain_jac]):
+        else:
+            if not all([isinstance(j, (int, float)) for j in constrain_jac]):
                 raise ValueError("Constrain_jac should be 2 numeric values")
             self.constrain_jac = constrain_jac
 
-        self.is_field = False 
-        if 'spline coef' not in coeffs.header.get_intent()[0]: 
-
-            if (coeffs.shape[:3] != ref.size).any(): 
-                raise RuntimeError("Input file seems to be a displacement field", 
-                    " but size does not match reference image")
+        self.is_field = False
+        if "spline coef" not in coeffs.header.get_intent()[0]:
+            if (coeffs.shape[:3] != ref.size).any():
+                raise RuntimeError(
+                    "Input file seems to be a displacement field",
+                    " but size does not match reference image",
+                )
 
-            warp0 = coeffs.dataobj[0,0,0,:]
-            warpN = coeffs.dataobj[-1,-1,-1,:]
+            warp0 = coeffs.dataobj[0, 0, 0, :]
+            warpN = coeffs.dataobj[-1, -1, -1, :]
 
             # If the distance between the first and last displacement vector
-            # is covers a significant portion of the FoV, we probably have an 
+            # is covers a significant portion of the FoV, we probably have an
             # absolute displacement field
-            if (np.abs(warp0 - warpN) > 0.5 * ref.fov_size).all(): 
-                warnings.warn("NonLinearRegistration.from_fnirt(): absolute "
-                    + "displacement field detected, making relative.")
-                
-                ijk = ref.ijk_grid().reshape(-1,3)
+            if (np.abs(warp0 - warpN) > 0.5 * ref.fov_size).all():
+                warnings.warn(
+                    "NonLinearRegistration.from_fnirt(): absolute "
+                    + "displacement field detected, making relative."
+                )
+
+                ijk = ref.ijk_grid().reshape(-1, 3)
                 ijk = aff_trans(ref.vox2FSL, ijk)
-                ijk = coeffs.get_fdata().reshape(-1,3) - ijk
-                coeffs = nibabel.Nifti1Image(ijk.reshape(*ref.size, 3), 
-                         coeffs.affine, coeffs.header)
+                ijk = coeffs.get_fdata().reshape(-1, 3) - ijk
+                coeffs = nibabel.Nifti1Image(
+                    ijk.reshape(*ref.size, 3), coeffs.affine, coeffs.header
+                )
 
-        # We now have either an absolute field, or coefficients volume 
-        self.coefficients = coeffs 
+        # We now have either an absolute field, or coefficients volume
+        self.coefficients = coeffs
 
     @property
     def jmin(self):
         return self.constrain_jac[0]
 
     @property
     def jmax(self):
         return self.constrain_jac[1]
 
     def get_cache_value(self, ref, postmat):
         """
-        Return cacheable values, if possible, else return None. 
+        Return cacheable values, if possible, else return None.
 
-        When can we cache? If there are only one midmat/postmat, or all of the 
-        midmats and postmats are actually the same (due to series expansion 
-        required to match the size of the premats), then we can compute and  
-        cache displacement field as it will be the same for all workers. 
-        If not, then we cannot cache and all workes must compute a new 
-        displacement field for each mid/post pair 
+        When can we cache? If there are only one midmat/postmat, or all of the
+        midmats and postmats are actually the same (due to series expansion
+        required to match the size of the premats), then we can compute and
+        cache displacement field as it will be the same for all workers.
+        If not, then we cannot cache and all workes must compute a new
+        displacement field for each mid/post pair
         """
 
         # If we have series of postmats, check if they are all identitical
-        if len(postmat) > 1: 
-            same1 = all([ np.allclose(postmat.src2ref[0], m) 
-                          for m in postmat.src2ref ])
-            if same1: 
+        if len(postmat) > 1:
+            same1 = all([np.allclose(postmat.src2ref[0], m) for m in postmat.src2ref])
+            if same1:
                 pmat = postmat[0].to_fsl(self.ref_spc, ref)
-        else: 
-            same1 = True 
+        else:
+            same1 = True
             pmat = postmat.to_fsl(self.ref_spc, ref)
 
-        if same1: 
-            return get_field(self.coefficients, ref, post=pmat, 
-                             jmin=self.jmin, jmax=self.jmax)
-        else: 
-            return None 
+        if same1:
+            return get_field(
+                self.coefficients, ref, post=pmat, jmin=self.jmin, jmax=self.jmax
+            )
+        else:
+            return None
 
-    def get_displacements(self, ref, postmat, at_idx=None): 
+    def get_displacements(self, ref, postmat, at_idx=None):
         """
         Resolve displacements of transform within reference space with postmat.
 
-        Args: 
+        Args:
             ref (ImageSpace): space within which to resolve displacements
             postmat (Registration/MotionCorrection): post-warp transform
             at_idx (int): index number within postmat to use (for MC). Default
-                None, which corresponds to Registration postmats (not MC). 
+                None, which corresponds to Registration postmats (not MC).
 
-        Returns: 
-            (array): Nx3 array of absolute positions of reference voxels in the 
+        Returns:
+            (array): Nx3 array of absolute positions of reference voxels in the
                 grid of the warp's source space, in FSL coordinates
         """
 
-        if at_idx is None: 
+        if at_idx is None:
             assert len(postmat) == 1
-            p = postmat 
-        else: 
+            p = postmat
+        else:
             p = postmat[at_idx]
         post = p.to_fsl(self.ref_spc, ref)
-        return get_field(self.coefficients, ref, post=post, jmin=self.jmin, 
-                         jmax=self.jmax)
+        return get_field(
+            self.coefficients, ref, post=post, jmin=self.jmin, jmax=self.jmax
+        )
 
 
 class NonLinearProduct(object):
     """
     Lazy evaluation of the combination of two non-linear warps. The two warps
     are stored separately as FNIRTCoefficients objects, and combined into a
-    single field via convertwarp when resolve() is called. 
+    single field via convertwarp when resolve() is called.
 
-    Args: 
-        first (FNIRTCoefficients): first warp 
+    Args:
+        first (FNIRTCoefficients): first warp
         first_post (Registration/MotionCorrection): after first warp transform
         second_pre (Registration/MotionCorrection): before second warp transform
-        second (FNIRTCoefficients): second warp 
+        second (FNIRTCoefficients): second warp
     """
 
     def __init__(self, first, first_post, second_pre, second):
-        
-        if ((type(first) is NonLinearProduct) 
-            or (type(second) is NonLinearProduct)): 
-            raise NotImplementedError("Cannot chain more than two non-linear transforms")
+        if (type(first) is NonLinearProduct) or (type(second) is NonLinearProduct):
+            raise NotImplementedError(
+                "Cannot chain more than two non-linear transforms"
+            )
 
         self.warp1 = first
         self.warp2 = second
-        self.src_spc = first.src_spc 
-        self.ref_spc = second.ref_spc 
+        self.src_spc = first.src_spc
+        self.ref_spc = second.ref_spc
         self.midmat = second_pre @ first_post
 
         jmin = None
-        jmax = None 
-        if first.jmin is not None: 
+        jmax = None
+        if first.jmin is not None:
             jmin = first.jmin
-        if ((second.jmin is not None) 
-             and (jmin is None)):
+        if (second.jmin is not None) and (jmin is None):
             jmin = second.jmin
-        if ((second.jmin is not None) 
-             and (jmin is not None)
-             and (second.jmin > jmin)):
+        if (second.jmin is not None) and (jmin is not None) and (second.jmin > jmin):
             jmin = second.jmin
 
-        if first.jmax is not None: 
+        if first.jmax is not None:
             jmax = first.jmax
-        if ((second.jmax is not None) 
-             and (jmax is None)):
+        if (second.jmax is not None) and (jmax is None):
             jmax = second.jmax
-        if ((second.jmax is not None) 
-             and (jmax is not None)
-             and (second.jmax < jmax)):
+        if (second.jmax is not None) and (jmax is not None) and (second.jmax < jmax):
             jmax = second.jmax
 
-        assert (((jmin is None) and (jmax is None)) 
-                or all([ isinstance(j, (int, float)) for j in [jmin,jmax] ]))
+        assert ((jmin is None) and (jmax is None)) or all(
+            [isinstance(j, (int, float)) for j in [jmin, jmax]]
+        )
         self.constrain_jac = (jmin, jmax)
 
     @property
     def jmin(self):
         return self.constrain_jac[0]
 
     @property
     def jmax(self):
         return self.constrain_jac[1]
 
     def get_cache_value(self, ref, postmat):
         """
-        Return cacheable values, if possible, else return None. 
+        Return cacheable values, if possible, else return None.
 
-        When can we cache? If there are only one midmat/postmat, or all of the 
-        midmats and postmats are actually the same (due to series expansion 
-        required to match the size of the premats), then we can compute and  
-        cache displacement field as it will be the same for all workers. 
-        If not, then we cannot cache and all workes must compute a new 
-        displacement field for each mid/post pair 
+        When can we cache? If there are only one midmat/postmat, or all of the
+        midmats and postmats are actually the same (due to series expansion
+        required to match the size of the premats), then we can compute and
+        cache displacement field as it will be the same for all workers.
+        If not, then we cannot cache and all workes must compute a new
+        displacement field for each mid/post pair
         """
 
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
 
         # If we have series of mid and postmats, check if they are all identitical
-        if len(postmat) > 1: 
-            same1 = all([ np.allclose(postmat.src2ref[0], m) 
-                          for m in postmat.src2ref ])
-            if same1: 
+        if len(postmat) > 1:
+            same1 = all([np.allclose(postmat.src2ref[0], m) for m in postmat.src2ref])
+            if same1:
                 pmat = postmat[0].to_fsl(self.warp2.ref_spc, ref)
-        else: 
-            same1 = True 
+        else:
+            same1 = True
             pmat = postmat.to_fsl(self.warp2.ref_spc, ref)
 
-        if len(self.midmat) > 1: 
-            same2 = all([ np.allclose(self.midmat.src2ref[0], m) 
-                          for m in self.midmat.src2ref ])
-            if same2: 
+        if len(self.midmat) > 1:
+            same2 = all(
+                [np.allclose(self.midmat.src2ref[0], m) for m in self.midmat.src2ref]
+            )
+            if same2:
                 mmat = self.midmat[0].to_fsl(self.warp1.ref_spc, self.warp2.src_spc)
 
-        else: 
-            same2 = True 
+        else:
+            same2 = True
             mmat = self.midmat.to_fsl(self.warp1.ref_spc, self.warp2.src_spc)
 
-        same = (same1 & same2)
+        same = same1 & same2
 
-        if same: 
-            return get_field(self.warp1.coefficients, ref, 
-                             coeff2=self.warp2.coefficients, mid=mmat, 
-                             post=pmat, jmin=self.constrain_jac[0], 
-                             jmax=self.constrain_jac[1])
-        else: 
-            return None 
+        if same:
+            return get_field(
+                self.warp1.coefficients,
+                ref,
+                coeff2=self.warp2.coefficients,
+                mid=mmat,
+                post=pmat,
+                jmin=self.constrain_jac[0],
+                jmax=self.constrain_jac[1],
+            )
+        else:
+            return None
 
     def get_displacements(self, ref, postmat, at_idx=None):
         """
         Resolve displacements of transform within reference space with postmat.
 
-        Args: 
+        Args:
             ref (ImageSpace): space within which to resolve displacements
             postmat (Registration/MotionCorrection): post-warp transform
-            at_idx (int): index number within mid/postmat to use (for MC). 
-                Default is None, which corresponds to Registration mid/postmats. 
+            at_idx (int): index number within mid/postmat to use (for MC).
+                Default is None, which corresponds to Registration mid/postmats.
 
-        Returns: 
-            (array): Nx3 array of absolute positions of reference voxels in the 
+        Returns:
+            (array): Nx3 array of absolute positions of reference voxels in the
                 grid of the warp's source space, in FSL coordinates
         """
 
-        if at_idx is None: 
+        if at_idx is None:
             assert (len(postmat) == 1) and (len(self.midmat) == 1)
-            p = postmat 
+            p = postmat
             m = self.midmat
-        else: 
+        else:
             p = postmat[at_idx]
             m = self.midmat[at_idx]
-       
+
         mid = m.to_fsl(self.warp1.ref_spc, self.warp2.src_spc)
         post = p.to_fsl(self.warp2.ref_spc, ref)
-        return get_field(self.warp1.coefficients, ref, 
-                            coeff2=self.warp2.coefficients, mid=mid, post=post,
-                            jmin=self.jmin, jmax=self.jmax)
+        return get_field(
+            self.warp1.coefficients,
+            ref,
+            coeff2=self.warp2.coefficients,
+            mid=mid,
+            post=post,
+            jmin=self.jmin,
+            jmax=self.jmax,
+        )
 
 
 def get_field(coeff1, ref, coeff2=None, mid=None, post=None, jmin=None, jmax=None):
     """
-    Resolve coefficients into displacement field via convertwarp. 
+    Resolve coefficients into displacement field via convertwarp.
 
-    Args: 
-        coeff1 (FNIRTCoefficients): first warp 
-        ref (ImageSpace): reference grid for output 
-        coeff2 (FNIRTCoefficients): optional, second warp 
-        mid (np.ndarray): optional, between-warp affine matrix 
-        post (np.ndarray): optional, after-warp affine matrix 
-
-    Returns: 
-        np.ndarray, shape Nx3, arranged by voxel index down the rows and 
-            XYZ in columns. Row M in the array gives the position of the 
+    Args:
+        coeff1 (FNIRTCoefficients): first warp
+        ref (ImageSpace): reference grid for output
+        coeff2 (FNIRTCoefficients): optional, second warp
+        mid (np.ndarray): optional, between-warp affine matrix
+        post (np.ndarray): optional, after-warp affine matrix
+
+    Returns:
+        np.ndarray, shape Nx3, arranged by voxel index down the rows and
+            XYZ in columns. Row M in the array gives the position of the
             reference voxel with linear index M in the *source* voxel grid
-            of warp1, *in FSL coordinates*. 
+            of warp1, *in FSL coordinates*.
     """
 
     for m in [mid, post]:
-        if not isinstance(m, (np.ndarray, type(None))): 
-            raise ValueError('mid/post should be np.array in FSL convention')
+        if not isinstance(m, (np.ndarray, type(None))):
+            raise ValueError("mid/post should be np.array in FSL convention")
+
+    if not shutil.which("convertwarp"):
+        raise RuntimeError(
+            "'convertwarp' not found. Please ensure FSL is installed and "
+            + "available on the system path"
+        )
 
-    with tempfile.TemporaryDirectory() as d: 
-        w1 = op.join(d, 'w1.nii.gz')
+    with tempfile.TemporaryDirectory() as d:
+        w1 = op.join(d, "w1.nii.gz")
         nibabel.save(coeff1, w1)
-        refvol = op.join(d, 'ref.nii.gz')
+        refvol = op.join(d, "ref.nii.gz")
         ref.touch(refvol)
-        cmd = f'convertwarp --warp1={w1} --ref={refvol}'
+        cmd = f"convertwarp --warp1={w1} --ref={refvol}"
 
-        if coeff2 is not None: 
-            w2 = op.join(d, 'w2.nii.gz')
+        if coeff2 is not None:
+            w2 = op.join(d, "w2.nii.gz")
             nibabel.save(coeff2, w2)
-            cmd += f' --warp2={w2}'        
+            cmd += f" --warp2={w2}"
 
-        if mid is not None: 
-            m = op.join(d, 'mid.mat')
+        if mid is not None:
+            m = op.join(d, "mid.mat")
             np.savetxt(m, mid)
-            cmd += f' --midmat={m}'
+            cmd += f" --midmat={m}"
 
-        if post is not None: 
-            p = op.join(d, 'post.mat')
+        if post is not None:
+            p = op.join(d, "post.mat")
             np.savetxt(p, post)
-            cmd += f' --postmat={p}'
+            cmd += f" --postmat={p}"
 
         if (jmin is not None) and (jmax is not None):
-            assert all([ isinstance(j, (int, float)) for j in [jmin,jmax] ])
-            cmd += f' --constrainj --jmin={jmin} --jmax={jmax}' 
+            assert all([isinstance(j, (int, float)) for j in [jmin, jmax]])
+            cmd += f" --constrainj --jmin={jmin} --jmax={jmax}"
 
-        field = op.join(d, 'field.nii.gz')
-        cmd += f' --out={field} --absout'
+        field = op.join(d, "field.nii.gz")
+        cmd += f" --out={field} --absout"
 
-        subprocess.run(cmd, shell=True)  
-        field = nibabel.load(field).get_fdata().reshape(-1,3)
-    return field 
+        subprocess.run(cmd, shell=True)
+        field = nibabel.load(field).get_fdata().reshape(-1, 3)
+    return field
 
 
 def det_jacobian(vec_field, vox_size):
     """
     Calculate determinant of Jacobian for vector field, with homogenous
-    spacing along each axis. Second order central differences are used 
-    to estimate partial derivatives. 
+    spacing along each axis. Second order central differences are used
+    to estimate partial derivatives.
 
-    Args: 
-        vec_field (np.ndarray): sized XYZ3, where the last dimension 
+    Args:
+        vec_field (np.ndarray): sized XYZ3, where the last dimension
             corresponds to displacements along the x,y,z axis respectively
         vox_size (np.ndarray): array sized 3, step size along each spatial axis
 
-    Returns: 
+    Returns:
         (np.ndarray), sized XYZ, values of the determinant of the Jacobian
-            matrix evaluated at each point within the array 
+            matrix evaluated at each point within the array
 
     """
 
     if not ((len(vec_field.shape) == 4) and (vec_field.shape[3] == 3)):
-        raise ValueError("vec_field should be a 4D array with size 3 in "
-            "the last dimension")
+        raise ValueError(
+            "vec_field should be a 4D array with size 3 in " "the last dimension"
+        )
 
-    if not len(vox_size) == 3: 
-        raise ValueError("vox_size should be a 3-vector of dimensions") 
+    if not len(vox_size) == 3:
+        raise ValueError("vox_size should be a 3-vector of dimensions")
 
     # One of the sneakiest bugs I have ever had the misfortune of dealing
     # with.... If any of the coordinate axes have been flipped (due to FSL
-    # conventions, for example), then the absolute displacement vectors 
-    # will be strictly decreasing in that dimension (ie X, X-1, X-2 etc). 
-    # This means all partial derivatives in that dimension will also be 
+    # conventions, for example), then the absolute displacement vectors
+    # will be strictly decreasing in that dimension (ie X, X-1, X-2 etc).
+    # This means all partial derivatives in that dimension will also be
     # negative, which means a negative Jacobian determinant. So, check each
-    # dimension to see if it is ascending / descending, and flip the 
-    # corresponding voxel dimension to compensate if so. 
-    if (np.diff(vec_field[:,0,0,0]) < 0).all(): 
-        vox_size[0] *= -1 
+    # dimension to see if it is ascending / descending, and flip the
+    # corresponding voxel dimension to compensate if so.
+    if (np.diff(vec_field[:, 0, 0, 0]) < 0).all():
+        vox_size[0] *= -1
 
-    if (np.diff(vec_field[0,:,0,1]) < 0).all(): 
+    if (np.diff(vec_field[0, :, 0, 1]) < 0).all():
         vox_size[1] *= -1
 
-    if (np.diff(vec_field[0,0,:,2]) < 0).all(): 
-        vox_size[2] *= -1 
+    if (np.diff(vec_field[0, 0, :, 2]) < 0).all():
+        vox_size[2] *= -1
 
     # Calculate partial derivatives in each direction. Note that each of these
     # returns an array of size (X,Y,Z,3), arranged d/dx, d/dy, d/dz in the last
     # dimension. So dfx is a stack of arrays df(i)/dx, df(i)/dy, df(i)/dz. We
     # need to calculate the derivative with respect to each direction because
     # f is a vector field, ie, it contains i,j,k components, each of which are
     # independent functions of x,y,z
     dfi = np.gradient(vec_field, vox_size[0], axis=0)
     dfj = np.gradient(vec_field, vox_size[1], axis=1)
     dfk = np.gradient(vec_field, vox_size[2], axis=2)
 
-    # Construct an array of Jacobian matrices, sized (3,3,X,Y,Z) (ie, each 
+    # Construct an array of Jacobian matrices, sized (3,3,X,Y,Z) (ie, each
     # point in space get its own 3x3 Jacobian matrix). The elements need
-    # to be arranged df(i)/dx --- df(i)/dz 
+    # to be arranged df(i)/dx --- df(i)/dz
     #                   |      |     |
     #                df(k)/dx --- df(k)/dz
-    jacobian = np.array([[dfi[...,0], dfi[...,1], dfi[...,2]],
-                         [dfj[...,0], dfj[...,1], dfj[...,2]],
-                         [dfk[...,0], dfk[...,1], dfk[...,2]]
-                        ])
+    jacobian = np.array(
+        [
+            [dfi[..., 0], dfi[..., 1], dfi[..., 2]],
+            [dfj[..., 0], dfj[..., 1], dfj[..., 2]],
+            [dfk[..., 0], dfk[..., 1], dfk[..., 2]],
+        ]
+    )
 
     # Reshape into a single stack of (N,3,3) arrays and calculate the det
-    # Return an array of scalars sized (XYZ) again 
-    jacobian = np.moveaxis(jacobian.reshape(3,3,-1), 2, 0)
+    # Return an array of scalars sized (XYZ) again
+    jacobian = np.moveaxis(jacobian.reshape(3, 3, -1), 2, 0)
     jdet = np.linalg.det(jacobian).reshape(vec_field.shape[:3])
-    if ((jdet < 0).sum() / jdet.size) > 0.1: 
-        warnings.warn('regtricks: numerous negative values returned for Jacobian determinant')
+    if ((jdet < 0).sum() / jdet.size) > 0.1:
+        warnings.warn(
+            "regtricks: numerous negative values returned for Jacobian determinant"
+        )
 
     return jdet
```

### Comparing `regtricks-0.3.5.post1/regtricks/image_space.py` & `regtricks-0.3.6.post8/regtricks/image_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 ImageSpace: image matrix, inc dimensions, voxel size, vox2world matrix and
 inverse, of an image. Used for resampling operations between different 
 spaces and also for saving images into said space (eg, save PV estimates 
 into the space of an image)
 """
 
-import copy 
-from textwrap import dedent
+import copy
 from pathlib import Path
+from textwrap import dedent
 
 import nibabel
-import numpy as np 
-from nibabel import Nifti1Image, MGHImage
+import numpy as np
 from fsl.data.image import Image as FSLImage
+from nibabel import MGHImage, Nifti1Image
 
 
 class ImageSpace(object):
     """
     Voxel grid of an image, ignoring actual image data. 
 
     Args: 
@@ -217,14 +217,17 @@
             rounder = np.ceil 
       
         factor = np.array(factor)
         if factor.size == 1:
             factor = factor * np.ones(3)
 
         new_size = rounder(self.size / factor).astype(int)
+        if (new_size == 0).any(): 
+            raise RuntimeError("ImageSpace with resized voxels has no size")
+
         new_vox2world = copy.deepcopy(self.vox2world)
         new_vox2world[:3,:3] *= factor[None,:]
         bbox_shift = (new_vox2world[:3,:3] @ [0.5, 0.5, 0.5])
         new_vox2world[:3,3] = self.bbox_origin + bbox_shift
         return ImageSpace.manual(new_vox2world, new_size)
```

### Comparing `regtricks-0.3.5.post1/regtricks/multiplication.py` & `regtricks-0.3.6.post8/regtricks/multiplication.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/transforms/linear.py` & `regtricks-0.3.6.post8/regtricks/transforms/linear.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/transforms/nonlinear.py` & `regtricks-0.3.6.post8/regtricks/transforms/nonlinear.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,266 +1,278 @@
-import os.path as op 
-import tempfile 
+import os.path as op
 import subprocess
+import tempfile
 from textwrap import dedent
 
 import nibabel
-import numpy as np 
+import numpy as np
 
-from regtricks.transforms.transform import Transform
-from regtricks.transforms.linear import Registration, MotionCorrection
-from regtricks.image_space import ImageSpace
 from regtricks import application_helpers as apply
 from regtricks import multiplication as multiply
-from regtricks.fnirt_coefficients import (FNIRTCoefficients, NonLinearProduct, 
-                                          det_jacobian)
+from regtricks.fnirt_coefficients import (
+    FNIRTCoefficients,
+    NonLinearProduct,
+    det_jacobian,
+)
+from regtricks.image_space import ImageSpace
+from regtricks.transforms.linear import MotionCorrection, Registration
+from regtricks.transforms.transform import Transform
+
 
 class NonLinearRegistration(Transform):
     """
     Non linear registration transformation. Currently only FSL FNIRT warps
     are supported. Note that the --premat and --postmat used by FSL command
-    line tools should not be supplied here. Instead, defined them as 
-    Registration objects and use chain() to concatenate them with NLRs. 
+    line tools should not be supplied here. Instead, defined them as
+    Registration objects and use chain() to concatenate them with NLRs.
     """
 
     def __init__():
-
-        raise NotImplementedError("Currently only FNIRT supported, use "
-                                "NonLinearRegistration.from_fnirt() instead")
+        raise NotImplementedError(
+            "Currently only FNIRT supported, use "
+            "NonLinearRegistration.from_fnirt() instead"
+        )
 
         # Transform.__init__(self)
         # self.warp = FNIRTCoefficients(warp, src, ref)
         # self._intensity_correct = int(intensity_correct)
 
     @classmethod
-    def from_fnirt(cls, coefficients, src, ref, intensity_correct=False, 
-                   constrain_jac=False):
+    def from_fnirt(
+        cls, coefficients, src, ref, intensity_correct=False, constrain_jac=False
+    ):
         """
         FNIRT non-linear registration from a coefficients file. If a pre-warp
-        and post-warp transformation need to be applied, create these as 
-        separate Registration objects and combine them via chain, ie, 
+        and post-warp transformation need to be applied, create these as
+        separate Registration objects and combine them via chain, ie,
         combined = chain(pre, non-linear, post)
 
-        Args: 
-            coefficients (Pathlike): FNIRT coefficient field 
+        Args:
+            coefficients (Pathlike): FNIRT coefficient field
             src (Pathlike, ImageSpace): source image used for generating FNIRT coefficients
-            ref (Pathlike, ImageSpace): reference image used for generating FNIRT coefficients 
+            ref (Pathlike, ImageSpace): reference image used for generating FNIRT coefficients
             intensity_correct: intensity correct output via the Jacobian determinant
                 of this warp (when self.apply_to*() is called)
             constrain_jac (bool/array-like): constrain Jacobian for intensity
-                correction (default False). If True, limits of (0.01, 100) will 
+                correction (default False). If True, limits of (0.01, 100) will
                 be used, or explicit limits can be given as (min, max)
-                
-        Returns: 
-            NonLinearRegistration object 
+
+        Returns:
+            NonLinearRegistration object
         """
 
         warp = FNIRTCoefficients(coefficients, src, ref, constrain_jac)
-        return NonLinearRegistration._manual_construct(warp, 
-            np.eye(4), np.eye(4), intensity_correct)
+        return NonLinearRegistration._manual_construct(
+            warp, np.eye(4), np.eye(4), intensity_correct
+        )
 
     @property
     def intensity_correct(self):
         return bool(self._intensity_correct)
 
     @intensity_correct.setter
     def intensity_correct(self, flag):
         self._intensity_correct = int(flag)
 
     def __len__(self):
         return 1
 
     @classmethod
-    def _manual_construct(cls, warp, premat, postmat, 
-                          intensity_correct):
+    def _manual_construct(cls, warp, premat, postmat, intensity_correct):
         """Manual constructor, do not use from outside regtricks"""
 
         # # We store intensity correction as an integer private variable,
         # # as it can take the values 0,1,2,3 (this includes NonLinearMC subclass)
         # # 0: no intensity correction
         # # 1: intensity correction, or if the warp is a NonLinearProduct, then
-        # #       intensity correct the FIRST warp 
-        # # 2: intensity correct the second warp of a NLP 
-        # # 3: intensity correct both warps of a NLP  
-        
+        # #       intensity correct the FIRST warp
+        # # 2: intensity correct the second warp of a NLP
+        # # 3: intensity correct both warps of a NLP
+
         x = cls.__new__(cls)
         Transform.__init__(x)
         assert isinstance(warp, (FNIRTCoefficients, NonLinearProduct))
         x.warp = warp
         x.premat = multiply.cast_potential_array(premat)
-        x.postmat = multiply.cast_potential_array(postmat) 
+        x.postmat = multiply.cast_potential_array(postmat)
         x.intensity_correct = int(intensity_correct)
 
-        return x 
+        return x
 
     def inverse(self):
         """Iverse warpfield, via FSL invwarp"""
 
-        # TODO: lazy evaluation of this? And move into FNIRT coeffs somehow 
+        # TODO: lazy evaluation of this? And move into FNIRT coeffs somehow
         with tempfile.TemporaryDirectory() as d:
-            oldcoeffs = op.join(d, 'oldcoeffs.nii.gz')
-            newcoeffs = op.join(d, 'newcoeffs.nii.gz')
-            old_src = op.join(d, 'src.nii.gz')
-            old_ref = op.join(d, 'ref.nii.gz')
+            oldcoeffs = op.join(d, "oldcoeffs.nii.gz")
+            newcoeffs = op.join(d, "newcoeffs.nii.gz")
+            old_src = op.join(d, "src.nii.gz")
+            old_ref = op.join(d, "ref.nii.gz")
             self.warp.src_spc.touch(old_src)
             self.warp.ref_spc.touch(old_ref)
             nibabel.save(self.warp.coefficients, oldcoeffs)
-            cmd = 'invwarp -w {} -o {} -r {}'.format(oldcoeffs, 
-                                                     newcoeffs, old_src)
+            cmd = "invwarp -w {} -o {} -r {}".format(oldcoeffs, newcoeffs, old_src)
             subprocess.run(cmd, shell=True)
             newcoeffs = nibabel.load(newcoeffs)
             newcoeffs.get_fdata()
             inv = NonLinearRegistration.from_fnirt(newcoeffs, old_ref, old_src)
-        return inv 
+        return inv
 
-    def premat_to_fsl(self, src, ref): 
-        """Return list of premats in FSL convention""" 
+    def premat_to_fsl(self, src, ref):
+        """Return list of premats in FSL convention"""
 
-        if type(self.premat) is Registration: 
+        if type(self.premat) is Registration:
             return self.premat.to_fsl(src, ref)
-        else: 
+        else:
             assert type(self.premat) is list
-            return [ t.to_fsl(src, ref) for t in self.premat ]
+            return [t.to_fsl(src, ref) for t in self.premat]
 
-    def postmat_to_fsl(self, src, ref): 
-        """Return list of postmats in FSL convention""" 
+    def postmat_to_fsl(self, src, ref):
+        """Return list of postmats in FSL convention"""
 
-        if type(self.postmat) is Registration: 
+        if type(self.postmat) is Registration:
             return self.postmat.to_fsl(src, ref)
-        else: 
+        else:
             assert type(self.postmat) is list
-            return [ t.to_fsl(src, ref) for t in self.postmat ]
+            return [t.to_fsl(src, ref) for t in self.postmat]
 
     def __repr__(self):
-        text = (f"""\
+        text = f"""\
         NonLinearRegistration with properties:
-        """)
+        """
         return dedent(text)
 
     def prepare_cache(self, ref):
         """
-        Pre-compute and store the displacement field, including any postmats. 
-        This is because premats can be applied after calculating the field, 
+        Pre-compute and store the displacement field, including any postmats.
+        This is because premats can be applied after calculating the field,
         but postmats must be included as part of that calculation. Note that
-        get_cache_value() return None, signifying that the field could not 
+        get_cache_value() return None, signifying that the field could not
         be cached (which implies a NLMC)
 
-        Args: 
+        Args:
             ref (ImageSapce): the space in towards which the transform will
-                be applied 
+                be applied
         """
         self.cache = self.warp.get_cache_value(ref, self.postmat)
-        if self.cache is None: 
+        if self.cache is None:
             assert type(self) is NonLinearMotionCorrection
 
     def resolve(self, src, ref, *unused):
         """
         Return a coordinate array and scale factor that maps reference voxels
         into source voxels, including the transform. Uses cached values, if
         available.  A scale factor of 1 will be returned if no intensity
-        correction was requested. 
+        correction was requested.
 
-        Args: 
+        Args:
             src (ImageSpace): in which data currently exists and interpolation
                 will be performed
             ref (ImageSpace): in which data needs to be expressed
 
-        Returns: 
-            (np.ndarray, np.ndarray/int) coordinates on which to interpolate, 
-                scaling factor to apply after interpolation 
+        Returns:
+            (np.ndarray, np.ndarray/int) coordinates on which to interpolate,
+                scaling factor to apply after interpolation
         """
 
-        ref2src_vox = (src.world2vox 
-                       @ self.premat.ref2src 
-                       @ self.warp.src_spc.FSL2world)
+        ref2src_vox = src.world2vox @ self.premat.ref2src @ self.warp.src_spc.FSL2world
 
-        if self.cache is not None: 
+        if self.cache is not None:
             ijk = apply.aff_trans(ref2src_vox, self.cache).T
-        else: 
+        else:
             raise RuntimeError("Should always be able to cache a NLR")
 
-        if not self.intensity_correct: 
+        if not self.intensity_correct:
             scale = 1
-        else: 
-
-            # Either a single warp, or intensity correction from both warps. 
+        else:
+            # Either a single warp, or intensity correction from both warps.
             # Either way, calculate detJ on the overall final displacement field, which is
             # given by dfield (including any reqd postmats)
-            if (type(self.warp) is not NonLinearProduct) or (self._intensity_correct == 3): 
+            if (type(self.warp) is not NonLinearProduct) or (
+                self._intensity_correct == 3
+            ):
                 scale = det_jacobian(self.cache.reshape(*ref.size, 3), ref.vox_size)
 
             # Intensity correct on second warp. Just calculate the displacement field
-            # for the second warp and the corresponding postmat. 
-            elif self._intensity_correct == 2: 
+            # for the second warp and the corresponding postmat.
+            elif self._intensity_correct == 2:
                 dfield2 = self.warp.warp2.get_displacements(ref, self.postmat)
                 scale = det_jacobian(dfield2.reshape(*ref.size, 3), ref.vox_size)
 
-            # Intensity correct on first warp. Calculate the displacement field on 
-            # the first warp. Then calculate the successor transform: the midmat, 
-            # the second warp, and the final postmat; and run the detJ through the 
-            # successor transform 
-            else: 
-                assert self._intensity_correct == 1 
-                dfield1 = self.warp.warp1.get_displacements(ref, Registration.identity())
+            # Intensity correct on first warp. Calculate the displacement field on
+            # the first warp. Then calculate the successor transform: the midmat,
+            # the second warp, and the final postmat; and run the detJ through the
+            # successor transform
+            else:
+                assert self._intensity_correct == 1
+                dfield1 = self.warp.warp1.get_displacements(
+                    ref, Registration.identity()
+                )
                 dj = det_jacobian(dfield1.reshape(*ref.size, 3), ref.vox_size)
-                successor = NonLinearRegistration._manual_construct(self.warp.warp2, premat=self.warp.midmat, 
-                    postmat=self.postmat, intensity_correct=False)
+                successor = NonLinearRegistration._manual_construct(
+                    self.warp.warp2,
+                    premat=self.warp.midmat,
+                    postmat=self.postmat,
+                    intensity_correct=False,
+                )
                 scale = successor.apply_to_array(dj, ref, ref, cores=1, superfactor=1)
 
         return (ijk, scale)
 
+
 class NonLinearMotionCorrection(NonLinearRegistration):
     """
     Only to be created by multiplication of other classes. Don't go here!
 
-    Args: 
-        warp: FNIRTCoefficients object or NonLinearProduct 
+    Args:
+        warp: FNIRTCoefficients object or NonLinearProduct
         src: src of transform
         ref: ref of transform
         premat: list of Registration objects
         postmat: list of Registration objects
         intensity_correct: int (0/1/2/3), whether to apply intensity
             correction, and at what stage in the case of NLPs
         constrain_jac (bool/array-like): constrain Jacobian for intensity
-            correction (default False). If True, limits of (0.01, 100) will 
+            correction (default False). If True, limits of (0.01, 100) will
             be used, or explicit limits can be given as (min, max)
     """
 
-    def __init__(self, warp, premat, postmat, intensity_correct=0, 
-                 constrain_jac=False):
-        
+    def __init__(self, warp, premat, postmat, intensity_correct=0, constrain_jac=False):
         self.warp = warp
 
-        assert (isinstance(premat, (Registration, np.ndarray)) 
-                or isinstance(postmat, (Registration, np.ndarray)))
+        assert isinstance(premat, (Registration, np.ndarray)) or isinstance(
+            postmat, (Registration, np.ndarray)
+        )
 
-        # Expand the pre/postmats to be MotionCorrections of equal length, 
-        # if they are not already 
+        # Expand the pre/postmats to be MotionCorrections of equal length,
+        # if they are not already
         if len(premat) > len(postmat):
-            assert len(postmat) == 1, 'Different length pre/postmats given'
+            assert len(postmat) == 1, "Different length pre/postmats given"
             postmat = MotionCorrection.from_registration(postmat, len(premat))
-        
-        elif len(postmat) > len(premat): 
-            assert len(premat) == 1, 'Different length pre/postmats given'
+
+        elif len(postmat) > len(premat):
+            assert len(premat) == 1, "Different length pre/postmats given"
             premat = MotionCorrection.from_registration(premat, len(postmat))
 
         else:
-            if not len(premat) == len(postmat): 
-                raise ValueError('Different length pre/postmats')
+            if not len(premat) == len(postmat):
+                raise ValueError("Different length pre/postmats")
 
-        # Likewise expand the midmat if we have a NLP as the warp 
+        # Likewise expand the midmat if we have a NLP as the warp
         if (type(warp) is NonLinearProduct) and (len(warp.midmat) != len(premat)):
-            if len(warp.midmat) == 1: 
-                self.warp.midmat = MotionCorrection.from_registration(warp.midmat, len(premat))
-            else: 
+            if len(warp.midmat) == 1:
+                self.warp.midmat = MotionCorrection.from_registration(
+                    warp.midmat, len(premat)
+                )
+            else:
                 raise ValueError("Different length pre/midmats")
 
         self.premat = multiply.cast_potential_array(premat)
-        self.postmat = multiply.cast_potential_array(postmat) 
-        if intensity_correct > 1 and (type(warp) is not NonLinearProduct): 
+        self.postmat = multiply.cast_potential_array(postmat)
+        if intensity_correct > 1 and (type(warp) is not NonLinearProduct):
             raise ValueError("Intensity correction value implies NonLinearProduct")
         self._intensity_correct = intensity_correct
 
     def __len__(self):
         return len(self.premat)
 
     def __repr__(self):
@@ -271,64 +283,69 @@
         return dedent(text)
 
     def resolve(self, src, ref, at_idx):
         """
         Return a coordinate array and scale factor that maps reference voxels
         into source voxels, including the transform. Uses cached values, if
         available. A scale factor of 1 will be returned if no intensity
-        correction was requested. 
+        correction was requested.
 
-        Args: 
+        Args:
             src (ImageSpace): in which data currently exists and interpolation
                 will be performed
             ref (ImageSpace): in which data needs to be expressed
             at_idx (int): index number within MC series of transforms to apply
 
-        Returns: 
-            (np.ndarray, np.ndarray/int) coordinates on which to interpolate, 
-                scaling factor to apply after interpolation 
+        Returns:
+            (np.ndarray, np.ndarray/int) coordinates on which to interpolate,
+                scaling factor to apply after interpolation
         """
 
-        if self.cache is not None: 
+        if self.cache is not None:
             dfield = self.cache
-        else: 
+        else:
             dfield = self.warp.get_displacements(ref, self.postmat, at_idx)
 
         # Prepare the single overall transformation of premat and
-        #  world/voxel matrices that is required for interpolation 
-        ref2src_vox = (src.world2vox 
-                        @ self.premat.ref2src[at_idx] 
-                        @ self.warp.src_spc.FSL2world)
+        #  world/voxel matrices that is required for interpolation
+        ref2src_vox = (
+            src.world2vox @ self.premat.ref2src[at_idx] @ self.warp.src_spc.FSL2world
+        )
         ijk = apply.aff_trans(ref2src_vox, dfield).T
 
-        if not self.intensity_correct: 
+        if not self.intensity_correct:
             scale = 1
 
-        else: 
-
+        else:
             # TODO: cache the intensity correction?
-            # Either a single warp, or intensity correction from both warps. 
+            # Either a single warp, or intensity correction from both warps.
             # Either way, calculate detJ on the overall final displacement field, which is
             # given by dfield (including any reqd postmats)
-            if (type(self.warp) is not NonLinearProduct) or (self._intensity_correct == 3): 
+            if (type(self.warp) is not NonLinearProduct) or (
+                self._intensity_correct == 3
+            ):
                 scale = det_jacobian(dfield.reshape(*ref.size, 3), ref.vox_size)
 
             # Intensity correct on second warp. Just calculate the displacement field
-            # for the second warp and the corresponding postmat. 
-            elif self._intensity_correct == 2: 
+            # for the second warp and the corresponding postmat.
+            elif self._intensity_correct == 2:
                 df = self.warp.warp2.get_displacements(ref, self.postmat, at_idx)
                 scale = det_jacobian(df.reshape(*ref.size, 3), ref.vox_size)
 
-            # Intensity correct on first warp. Calculate the displacement field on 
-            # the first warp. Then calculate the successor transform: the midmat, 
-            # the second warp, and the final postmat; and run the detJ through the 
-            # successor transform 
-            else: 
-                assert self._intensity_correct == 1 
+            # Intensity correct on first warp. Calculate the displacement field on
+            # the first warp. Then calculate the successor transform: the midmat,
+            # the second warp, and the final postmat; and run the detJ through the
+            # successor transform
+            else:
+                assert self._intensity_correct == 1
                 df = self.warp.warp1.get_displacements(ref, Registration.identity())
                 dj = det_jacobian(df.reshape(*ref.size, 3), ref.vox_size)
-                successor = NonLinearRegistration._manual_construct(self.warp.warp2, self.warp.warp2.src_spc, 
-                    self.warp.warp2.ref_spc, premat=self.warp.midmat[at_idx], postmat=self.postmat[at_idx])
+                successor = NonLinearRegistration._manual_construct(
+                    self.warp.warp2,
+                    self.warp.warp2.src_spc,
+                    self.warp.warp2.ref_spc,
+                    premat=self.warp.midmat[at_idx],
+                    postmat=self.postmat[at_idx],
+                )
                 scale = successor.apply_to_array(dj, ref, ref, cores=1, superfactor=1)
 
         return (ijk, scale)
-
```

### Comparing `regtricks-0.3.5.post1/regtricks/transforms/transform.py` & `regtricks-0.3.6.post8/regtricks/transforms/transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,240 +1,297 @@
-import os.path as op 
-from textwrap import dedent
-from multiprocessing import cpu_count
-
-from nibabel import Nifti1Image, MGHImage
-import numpy as np 
+import numpy as np
 from fsl.data.image import Image as FSLImage
+from nibabel import MGHImage, Nifti1Image
 from scipy.ndimage import binary_fill_holes
 
-from regtricks.image_space import ImageSpace
-from regtricks import x5_interface as x5 
 from regtricks import application_helpers as apply
 from regtricks import multiplication as multiply
+from regtricks import x5_interface as x5
+from regtricks.image_space import ImageSpace
 
 # cache for intensity correction?
-# cast_space method 
+# cast_space method
+
 
 class Transform(object):
     """
-    Base object for all transformations. This should never actually be 
-    instantiated but is instead used to provide common functions. 
-    
-    Attributes: 
+    Base object for all transformations. This should never actually be
+    instantiated but is instead used to provide common functions.
+
+    Attributes:
         _cache: use for storing resolved displacement fields and sharing
-            amongst workers in multiprocessing pool 
+            amongst workers in multiprocessing pool
         islinear: Registrations or MotionCorrections
-        isnonlinear: NonLinearRegistrations or NLMCs 
+        isnonlinear: NonLinearRegistrations or NLMCs
 
     """
-    
+
     def __init__(self):
-        self._cache = None 
+        self._cache = None
 
     @property
     def is_linear(self):
-        from regtricks.transforms.linear import Registration, MotionCorrection
-        return (type(self) in [Registration, MotionCorrection])
+        from regtricks.transforms.linear import MotionCorrection, Registration
+
+        return type(self) in [Registration, MotionCorrection]
 
-    @property 
+    @property
     def is_nonlinear(self):
         return not self.is_linear
 
     def save(self, path):
         """Save transformation at path in X5 format (experimental)"""
 
         x5.save_manager(self, path)
 
     def __repr__(self):
         raise NotImplementedError()
 
     def reset_cache(self):
-        self.cache = None 
+        self.cache = None
 
     @property
     def cache(self):
         return self._cache
 
     @cache.setter
     def cache(self, new):
         if not ((new is None) or isinstance(new, np.ndarray)):
             raise ValueError("Cache can only be None or np.ndarray")
-        self._cache = new 
+        self._cache = new
 
     # We need to explicitly not implement np.array_ufunc to allow overriding
     # of __matmul__, see: https://github.com/numpy/numpy/issues/9028
-    __array_ufunc__ = None 
+    __array_ufunc__ = None
 
     def __matmul__(self, other):
-
-        from regtricks.transforms.linear import Registration, MotionCorrection
-        from regtricks.transforms.nonlinear import NonLinearMotionCorrection, NonLinearRegistration
+        from regtricks.transforms.linear import MotionCorrection, Registration
+        from regtricks.transforms.nonlinear import (
+            NonLinearMotionCorrection,
+            NonLinearRegistration,
+        )
 
         other = multiply.cast_potential_array(other)
         high_type = multiply.get_highest_type(self, other)
 
-        if high_type is Registration: 
+        if high_type is Registration:
             return multiply.registration(self, other)
-        elif high_type is MotionCorrection: 
+        elif high_type is MotionCorrection:
             return multiply.moco(self, other)
-        elif high_type is NonLinearRegistration: 
+        elif high_type is NonLinearRegistration:
             return multiply.nonlinearreg(self, other)
         elif high_type is NonLinearMotionCorrection:
             return multiply.nonlinearmoco(self, other)
-        else: 
+        else:
             raise NotImplementedError("Not Transformation objects")
 
     def __rmatmul__(self, other):
-
-        from regtricks.transforms.linear import Registration, MotionCorrection
-        from regtricks.transforms.nonlinear import NonLinearMotionCorrection, NonLinearRegistration
+        from regtricks.transforms.linear import MotionCorrection, Registration
+        from regtricks.transforms.nonlinear import (
+            NonLinearMotionCorrection,
+            NonLinearRegistration,
+        )
 
         other = multiply.cast_potential_array(other)
         high_type = multiply.get_highest_type(self, other)
 
-        if high_type is Registration: 
+        if high_type is Registration:
             return multiply.registration(other, self)
-        elif high_type is MotionCorrection: 
+        elif high_type is MotionCorrection:
             return multiply.moco(other, self)
-        elif high_type is NonLinearRegistration: 
+        elif high_type is NonLinearRegistration:
             return multiply.nonlinearreg(other, self)
         elif high_type is NonLinearMotionCorrection:
             return multiply.nonlinearmoco(other, self)
-        else: 
+        else:
             raise NotImplementedError("Not Transformation objects")
 
-    def apply_to_image(self, src, ref, order=3, superfactor=True, 
-                        mask=True, cval=0.0, cores=cpu_count(), **kwargs):
+    def apply_to_image(
+        self,
+        src,
+        ref,
+        order=3,
+        superfactor=True,
+        mask=True,
+        cval=0.0,
+        cores=1,
+        **kwargs,
+    ):
         """
-        Applies transformation to data array. If a registration is applied 
-        to 4D data, the same transformation will be applied to all volumes 
-        in the series. 
-
-        Args:   
-            src (Pathlike/NII/MGZ/FSLImage): image to transform 
-            ref (Pathlike/NII/MGZ/FSLImage/ImageSpace): target space for data 
-            order (int): 0 for NN, 1 for linear, 2-5 for splines. 
+        Applies transformation to data array. If a registration is applied
+        to 4D data, the same transformation will be applied to all volumes
+        in the series.
+
+        Args:
+            src (Pathlike/NII/MGZ/FSLImage): image to transform
+            ref (Pathlike/NII/MGZ/FSLImage/ImageSpace): target space for data
+            order (int): 0 for NN, 1 for linear, 2-5 for splines.
             superfactor (bool/int/iterable): default True for any order > 0,
                 (chosen automatically); intermediate super-sampling (replicates
-                applywarp -super), enabled by default when resampling from 
-                high to low resolution. Set as False to disable, or set an 
-                int/iterable to manually specify level for each image dimension. 
-            mask (bool): for order > 1, mask output to remove negligible 
-                values due to spline artefact 
+                applywarp -super), enabled by default when resampling from
+                high to low resolution. Set as False to disable, or set an
+                int/iterable to manually specify level for each image dimension.
+            mask (bool): for order > 1, mask output to remove negligible
+                values due to spline artefact
             cval (float): fill value for background, used for correcting
                 spline artefact
             cores (int): CPU cores to use for 4D data
             **kwargs: passed on to scipy.ndimage.map_coordinates
 
-        Returns: 
+        Returns:
             (np.array) transformed image data in ref voxel grid.
         """
 
         data, creator = apply.src_load_helper(src)
-        resamp = self.apply_to_array(data, src=src, ref=ref, order=order, 
-                                     superfactor=superfactor, mask=mask, 
-                                     cores=cores, cval=cval, **kwargs)
+        resamp = self.apply_to_array(
+            data,
+            src=src,
+            ref=ref,
+            order=order,
+            superfactor=superfactor,
+            mask=mask,
+            cores=cores,
+            cval=cval,
+            **kwargs,
+        )
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
-        
+
         if creator is MGHImage:
             ret = MGHImage(resamp, ref.vox2world, ref.header)
-            return ret 
-        else: 
+            return ret
+        else:
             ret = Nifti1Image(resamp, ref.vox2world, ref.header)
             if creator is FSLImage:
                 return FSLImage(ret)
-            else: 
-                return ret 
+            else:
+                return ret
 
-    def apply_to_array(self, data, src, ref, order=3, superfactor=True,
-                        mask=True, cval=0.0, cores=cpu_count(), **kwargs):
+    def apply_to_array(
+        self,
+        data,
+        src,
+        ref,
+        order=3,
+        superfactor=True,
+        mask=True,
+        cval=0.0,
+        cores=1,
+        **kwargs,
+    ):
         """
-        Applies transformation to data array. If a registration is applied 
-        to 4D data, the same transformation will be applied to all volumes 
-        in the series. 
-
-        Args:   
-            data (array): 3D or 4D array. 
-            src (Pathlike/NII/MGZ/FSLImage/ImageSpace): current space of data 
-            ref (Pathlike/NII/MGZ/FSLImage/ImageSpace): target space for data 
-            order (int): 0 for NN, 1 for linear, 2-5 for splines. 
+        Applies transformation to data array. If a registration is applied
+        to 4D data, the same transformation will be applied to all volumes
+        in the series.
+
+        Args:
+            data (array): 3D or 4D array.
+            src (Pathlike/NII/MGZ/FSLImage/ImageSpace): current space of data
+            ref (Pathlike/NII/MGZ/FSLImage/ImageSpace): target space for data
+            order (int): 0 for NN, 1 for linear, 2-5 for splines.
             superfactor (bool/int/iterable): default True for any order > 0,
                 (chosen automatically); intermediate super-sampling (replicates
-                applywarp -super), enabled by default when resampling from 
-                high to low resolution. Set as False to disable, or set an 
-                int/iterable to manually specify level for each image dimension. 
-            mask (bool): for order > 1, mask output to remove negligible 
-                values due to spline artefact 
+                applywarp -super), enabled by default when resampling from
+                high to low resolution. Set as False to disable, or set an
+                int/iterable to manually specify level for each image dimension.
+            mask (bool): for order > 1, mask output to remove negligible
+                values due to spline artefact
             cval (float): fill value for background, used for correcting
                 spline artefact
             cores (int): CPU cores to use for 4D data
             **kwargs: passed on to scipy.ndimage.map_coordinates
 
-        Returns: 
+        Returns:
             (np.array) transformed image data in ref voxel grid.
         """
 
+        from regtricks.transforms import (
+            NonLinearMotionCorrection,
+            NonLinearRegistration,
+        )
+
         if not isinstance(src, ImageSpace):
             src = ImageSpace(src)
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
 
         # Create super-resolution reference grid if necessary
         # Automatic is to use the ratio of input / output voxel size,
         # but for NN we leave it at 1 unless the user has expressly
-        # set a factor. 
-        if superfactor is not (False): 
-            if superfactor is True: 
-                if (src.vox_size < ref.vox_size).any() and (order != 0): 
-                    superfactor = np.floor(ref.vox_size / src.vox_size)
-                else: 
-                    superfactor = 1 
-
-            # Manually specified 
-            # Force superfactor into an integer array of length 3
-            superfactor = np.array(superfactor).round() * np.ones(3)
-        else: 
-            superfactor = np.ones(3)
-        superfactor = superfactor.astype(int)
+        # set a factor.
+        sfactor = np.ones(3)
+        if superfactor is not False:
+            if (superfactor is True) and (order > 0):
+                superfactor = np.floor(ref.vox_size / src.vox_size)
+                sfactor *= np.maximum(superfactor, 1)
+            else:
+                try:
+                    superfactor = np.asanyarray(superfactor)
+                    sfactor *= superfactor
+                except:
+                    raise ValueError(
+                        f"Unrecognised value for superfactor: {superfactor}"
+                    )
+
+        sfactor = sfactor.astype(int)
 
-        if (superfactor < 1).any(): 
+        if (sfactor < 1).any():
             raise ValueError("Superfactor must be integer > 0")
 
-        if (superfactor != 1).any(): 
-            super_ref = ref.resize_voxels(1 / superfactor, 'ceil')
-        else: 
-            super_ref = ref 
-
-        if not ((data.ndim in (3,4)) and (np.array_equal(src.size, data.shape[:3]))): 
-            raise ValueError("Data shape {} does not match source space {}"
-                                .format(data.shape, src.size))
-
-        # Force to float data 
-        data = data.astype(float32)
-
-        # Only use multiprocessing on 4D data 
-        if data.ndim == 3: 
-            cores = 1 
-        else: 
+        if (sfactor > 1).any():
+            super_ref = ref.resize_voxels(1 / sfactor, "ceil")
+        else:
+            super_ref = ref
+
+        if not ((data.ndim in (3, 4)) and (np.array_equal(src.size, data.shape[:3]))):
+            raise ValueError(
+                "Data shape {} does not match source space {}".format(
+                    data.shape, src.size
+                )
+            )
+
+        # Force to float data
+        data = data.astype(np.float32)
+
+        # Only use multiprocessing on 4D data
+        if data.ndim == 3:
+            cores = 1
+        else:
             cores = min([cores, data.shape[-1]])
 
-        kwargs.update({
-            'cval': cval,
-            'superfactor': superfactor,
-            'order': order
-            })
+        kwargs.update({"cval": cval, "superfactor": sfactor, "order": order})
         resamp = apply.despatch(data, self, src, super_ref, cores, **kwargs)
 
-        if mask and (order > 1): 
-            mvol = (data != cval) 
-            while mvol.ndim < 4: 
-                mvol = mvol[...,None]
-            mvol = np.stack([ binary_fill_holes(mvol[...,idx]) for idx in range(mvol.shape[3]) ], axis=-1) 
-            if mvol.ndim > data.ndim: 
+        if mask and (order > 1):
+            mvol = data != cval
+            while mvol.ndim < 4:
+                mvol = mvol[..., None]
+            mvol = np.stack(
+                [binary_fill_holes(mvol[..., idx]) for idx in range(mvol.shape[3])],
+                axis=-1,
+            )
+            if mvol.ndim > data.ndim:
                 mvol = np.squeeze(mvol)
-            mres = self.apply_to_array(mvol, src, ref, order=1, mask=False)
-            mres = (np.squeeze(mres) > 0.5)
-            resamp[~mres] = cval 
 
-        return resamp      
+            if isinstance(self, NonLinearMotionCorrection):
+                t = NonLinearMotionCorrection(
+                    self.warp, self.premat, self.postmat, intensity_correct=0
+                )
+            elif isinstance(self, NonLinearRegistration):
+                t = NonLinearRegistration._manual_construct(
+                    self.warp, self.premat, self.postmat, intensity_correct=0
+                )
+            else:
+                t = self
+
+            mres = t.apply_to_array(mvol, src, ref, order=1, mask=False, cores=cores)
+            mres = mres.astype(bool)
+            while mres.ndim < 4:
+                mres = mres[..., None]
+            mres = np.stack(
+                [binary_fill_holes(mres[..., idx]) for idx in range(mres.shape[3])],
+                axis=-1,
+            )
+            mres = np.squeeze(mres)
+            resamp[~mres] = cval
+
+        return resamp
```

### Comparing `regtricks-0.3.5.post1/regtricks/wrappers.py` & `regtricks-0.3.6.post8/regtricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks/x5_interface.py` & `regtricks-0.3.6.post8/regtricks/x5_interface.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/regtricks.egg-info/PKG-INFO` & `regtricks-0.3.6.post8/regtricks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.5.post1
+Version: 0.3.6.post8
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
-Author-email: thomas.kirk@eng.ox.ac.uk
+Author-email: tomfrankkirk@gmail.com
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Regtricks
 Tools for manipulating, combining and applying image transformations.
```

### Comparing `regtricks-0.3.5.post1/regtricks.egg-info/SOURCES.txt` & `regtricks-0.3.6.post8/regtricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.5.post1/setup.py` & `regtricks-0.3.6.post8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,12 @@
     
     setup(name=PACKAGE_NAME,
         version=get_version(),
         description="Tools for manipulating and applying registrations",
         long_description=get_filetext('README.md'),
         long_description_content_type='text/markdown',
         author='Tom Kirk',
-        author_email='thomas.kirk@eng.ox.ac.uk',
+        author_email='tomfrankkirk@gmail.com',
         license='BSD-3-clause', 
         url='https://github.com/tomfrankkirk/regtricks',
         install_requires=get_requirements(),
         packages=find_packages())
```

