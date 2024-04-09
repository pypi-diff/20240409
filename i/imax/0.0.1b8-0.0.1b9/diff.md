# Comparing `tmp/imax-0.0.1b8.tar.gz` & `tmp/imax-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imax-0.0.1b8.tar", last modified: Mon Apr  8 10:29:31 2024, max compression
+gzip compressed data, was "imax-0.0.1b9.tar", last modified: Mon Apr  8 13:05:44 2024, max compression
```

## Comparing `imax-0.0.1b8.tar` & `imax-0.0.1b9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 10:29:27.000000 imax-0.0.1b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-08 10:29:31.893623 imax-0.0.1b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 10:29:27.000000 imax-0.0.1b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/imax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/color_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/randaugment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/imax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:29:31.893623 imax-0.0.1b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-08 10:29:27.000000 imax-0.0.1b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-08 10:29:27.000000 imax-0.0.1b8/tests/test_color_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-08 10:29:27.000000 imax-0.0.1b8/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:05:44.251318 imax-0.0.1b9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 13:05:40.000000 imax-0.0.1b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-08 13:05:44.251318 imax-0.0.1b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 13:05:40.000000 imax-0.0.1b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:05:44.251318 imax-0.0.1b9/imax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:05:40.000000 imax-0.0.1b9/imax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-04-08 13:05:40.000000 imax-0.0.1b9/imax/color_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-04-08 13:05:40.000000 imax-0.0.1b9/imax/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-08 13:05:40.000000 imax-0.0.1b9/imax/randaugment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-08 13:05:40.000000 imax-0.0.1b9/imax/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:05:44.251318 imax-0.0.1b9/imax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-08 13:05:44.000000 imax-0.0.1b9/imax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 13:05:44.000000 imax-0.0.1b9/imax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:05:44.000000 imax-0.0.1b9/imax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 13:05:44.000000 imax-0.0.1b9/imax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 13:05:44.000000 imax-0.0.1b9/imax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:05:44.251318 imax-0.0.1b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-08 13:05:40.000000 imax-0.0.1b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:05:44.251318 imax-0.0.1b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-08 13:05:40.000000 imax-0.0.1b9/tests/test_color_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-08 13:05:40.000000 imax-0.0.1b9/tests/test_transforms.py
```

### Comparing `imax-0.0.1b8/LICENSE` & `imax-0.0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b8/PKG-INFO` & `imax-0.0.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imax
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Image augmentation library for Jax
 Home-page: https://github.com/4rtemi5/imax
 Author: Raphael Pisoni
 Author-email: raphael.pisoni@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `imax-0.0.1b8/README.md` & `imax-0.0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b8/imax/color_transforms.py` & `imax-0.0.1b9/imax/color_transforms.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b8/imax/project.py` & `imax-0.0.1b9/imax/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,43 +101,43 @@
         coords = jnp.stack([x_t, y_t, ones], axis=0)
     else:
         coords = jnp.stack([x_t, y_t], axis=0)
     # coords = jnp.tile(jnp.expand_dims(coords, 0), [batch, 1, 1, 1])
     return coords
 
 
-def bilinear_project(points_yx, depth, values, height, width, mask_value=0):
+def bilinear_project(points, depth, values, height, width, mask_value=0):
     # Create empty matrices, starting from 0 to p.max
     channels = values.shape[-1] + 1
     w = jnp.zeros((height, width))
     i = jnp.zeros((height, width, channels))
 
     valid_mask = (
         jnp.isfinite(depth) 
         # & jnp.greater_equal(depth, 0)
-        & jnp.isfinite(points_yx).all(axis=1)
+        & jnp.isfinite(points).all(axis=0)
         # & ~compute_occlusions(points_yx, depth)
-        & jnp.greater_equal(points_yx, 0.).all(axis=1)
-        & (points_yx[:, 0] < (height))
-        & (points_yx[:, 1] < (width))
+        & jnp.greater_equal(points, 0.).all(axis=0)
+        & (points[0] < (height))
+        & (points[1] < (width))
     )
     
     # Calc weights
-    floor = jnp.floor(points_yx)
+    floor = jnp.floor(points)
     ceil = floor + 1
-    upper_diff = ceil - points_yx
-    lower_diff = points_yx - floor
-    w1 = upper_diff[:, 0] * upper_diff[:, 1] * valid_mask
-    w2 = upper_diff[:, 0] * lower_diff[:, 1] * valid_mask
-    w3 = lower_diff[:, 0] * upper_diff[:, 1] * valid_mask
-    w4 = lower_diff[:, 0] * lower_diff[:, 1] * valid_mask
+    upper_diff = ceil - points
+    lower_diff = points - floor
+    w1 = upper_diff[0] * upper_diff[1] * valid_mask
+    w2 = upper_diff[0] * lower_diff[1] * valid_mask
+    w3 = lower_diff[0] * upper_diff[1] * valid_mask
+    w4 = lower_diff[0] * lower_diff[1] * valid_mask
     
     # Get indices
-    ix = floor[:, 0].astype("uint32")
-    iy = floor[:, 1].astype("uint32")
+    ix = floor[0].astype("uint32")
+    iy = floor[1].astype("uint32")
 
     w = w.at[ix, iy].add(w1, mode="drop")
     w = w.at[ix, iy + 1].add(w2, mode="drop")
     w = w.at[ix + 1, iy].add(w3, mode="drop")
     w = w.at[ix + 1, iy + 1].add(w4, mode="drop")
     #w += 1e-6
 
@@ -197,18 +197,18 @@
     target_pixel_coords = jnp.concatenate(
         [target_pixel_coords[:2] * depth, depth, ones], axis=0
     )
 
     target_pixel_coords = transform @ target_pixel_coords
     
     x, y, z, _ = jnp.split(target_pixel_coords, 4, axis=0)
-    target_pixel_coords = jnp.concatenate([target_pixel_coords[:2] / jnp.clip(depth, 1.0, jnp.inf), ones], axis=0)
+    target_pixel_coords = jnp.concatenate([target_pixel_coords[:2] / jnp.clip(depth, 1e-10, jnp.inf), ones], axis=0)
     target_pixel_coords = intrinsics @ target_pixel_coords
 
-    coords = jnp.concatenate([target_pixel_coords[0:1], target_pixel_coords[1:2]], axis=0).T  # new y, x coordinates
+    coords = jnp.concatenate([target_pixel_coords[0:1], target_pixel_coords[1:2]], axis=0)  # new y, x coordinates
 
     values = jnp.concatenate([
         input_image.reshape((-1, input_image.shape[-1])),  # original image values (eg. rgb)
     ], axis=1)
     
     new_depth = z.reshape((-1,))  # new z-coordinates
```

### Comparing `imax-0.0.1b8/imax/randaugment.py` & `imax-0.0.1b9/imax/randaugment.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b8/imax/transforms.py` & `imax-0.0.1b9/imax/transforms.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b8/imax.egg-info/PKG-INFO` & `imax-0.0.1b9/imax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imax
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Image augmentation library for Jax
 Home-page: https://github.com/4rtemi5/imax
 Author: Raphael Pisoni
 Author-email: raphael.pisoni@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `imax-0.0.1b8/setup.py` & `imax-0.0.1b9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imax",
-    version="0.0.1-beta8",
+    version="0.0.1-beta9",
     author="Raphael Pisoni",
     author_email="raphael.pisoni@gmail.com",
     description="Image augmentation library for Jax",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/4rtemi5/imax",
     classifiers=[
```

### Comparing `imax-0.0.1b8/tests/test_color_transforms.py` & `imax-0.0.1b9/tests/test_color_transforms.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b8/tests/test_transforms.py` & `imax-0.0.1b9/tests/test_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 def test_scale():
     factor = 3
     inputs = jnp.pad(
         jnp.ones((1, 1, 4), dtype="uint8") * 255,
         ((1, 1), (1, 1), (0, 0)),
         constant_values=0,
     )
-    targets = inputs  # jnp.ones_like(rgba_img) * 255
+    targets = inputs
     outputs = transforms.apply_transform(
         jnp.pad(
             jnp.ones((1, 1, 4), dtype="uint8"),
             ((1, 1), (1, 1), (0, 0)),
             constant_values=0,
         )
         * 255,
```

