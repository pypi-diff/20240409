# Comparing `tmp/lacss-0.7.6.tar.gz` & `tmp/lacss-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.7.6.tar", max compression
+gzip compressed data, was "lacss-0.8.0.tar", max compression
```

## Comparing `lacss-0.7.6.tar` & `lacss-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,48 @@
--rw-r--r--   0        0        0     1062 2024-03-02 14:23:44.689876 lacss-0.7.6/LICENSE
--rw-r--r--   0        0        0     2539 2024-03-02 14:23:44.689876 lacss-0.7.6/README.md
--rw-r--r--   0        0        0      157 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/__init__.py
--rw-r--r--   0        0        0       48 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/data/__init__.py
--rw-r--r--   0        0        0    14546 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/data/augment.py
--rw-r--r--   0        0        0    13109 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/data/generator.py
--rw-r--r--   0        0        0       43 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/deploy/__init__.py
--rw-r--r--   0        0        0     3151 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/deploy/lacss_pb2.py
--rw-r--r--   0        0        0    21615 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/deploy/predict.py
--rw-r--r--   0        0        0     4125 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/deploy/server.py
--rw-r--r--   0        0        0       74 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/losses/__init__.py
--rw-r--r--   0        0        0     6115 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0      965 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/losses/common.py
--rw-r--r--   0        0        0     1748 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/losses/detection.py
--rw-r--r--   0        0        0     5406 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/losses/instance.py
--rw-r--r--   0        0        0       22 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/metrics/__init__.py
--rw-r--r--   0        0        0     5435 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      371 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/__init__.py
--rw-r--r--   0        0        0     1704 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/auxiliary.py
--rw-r--r--   0        0        0     2355 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/common.py
--rw-r--r--   0        0        0     7968 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/convnext.py
--rw-r--r--   0        0        0     7808 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/detector.py
--rw-r--r--   0        0        0     3899 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/lacss.py
--rw-r--r--   0        0        0     3292 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3830 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/resnet.py
--rw-r--r--   0        0        0     5557 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     2297 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/modules/unet.py
--rw-r--r--   0        0        0      153 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/__init__.py
--rw-r--r--   0        0        0     2474 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/boxes.py
--rw-r--r--   0        0        0     3537 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/image.py
--rw-r--r--   0        0        0     3136 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/locations.py
--rw-r--r--   0        0        0     5961 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/nms.py
--rw-r--r--   0        0        0    11822 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/patches.py
--rw-r--r--   0        0        0      482 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/ops/uda.py
--rw-r--r--   0        0        0       63 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/tracking/__init__.py
--rw-r--r--   0        0        0     3340 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/tracking/predict.py
--rw-r--r--   0        0        0    12670 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/tracking/seqnms.py
--rw-r--r--   0        0        0     6741 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/tracking/utils.py
--rw-r--r--   0        0        0      248 2024-03-02 14:23:44.689876 lacss-0.7.6/lacss/train/__init__.py
--rw-r--r--   0        0        0    13564 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/train/base_trainer.py
--rw-r--r--   0        0        0     3404 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/train/lacss_mt_trainer.py
--rw-r--r--   0        0        0     8639 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/train/lacss_trainer.py
--rw-r--r--   0        0        0      663 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/train/loss.py
--rw-r--r--   0        0        0     4788 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/train/strategy.py
--rw-r--r--   0        0        0     4408 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/train/utils.py
--rw-r--r--   0        0        0      901 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/typing.py
--rw-r--r--   0        0        0     5712 2024-03-02 14:23:44.693877 lacss-0.7.6/lacss/utils.py
--rw-r--r--   0        0        0     1003 2024-03-02 14:24:01.721859 lacss-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 lacss-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-09 16:25:19.232858 lacss-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2539 2024-04-09 16:25:19.232858 lacss-0.8.0/README.md
+-rw-r--r--   0        0        0      157 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/data/__init__.py
+-rw-r--r--   0        0        0    14546 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/data/augment.py
+-rw-r--r--   0        0        0    13109 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/data/generator.py
+-rw-r--r--   0        0        0       43 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/lacss_pb2.py
+-rw-r--r--   0        0        0    21615 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/predict.py
+-rw-r--r--   0        0        0     4125 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/server.py
+-rw-r--r--   0        0        0       74 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/__init__.py
+-rw-r--r--   0        0        0     6115 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0      965 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/common.py
+-rw-r--r--   0        0        0     1748 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/detection.py
+-rw-r--r--   0        0        0     5406 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/instance.py
+-rw-r--r--   0        0        0       22 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0     5559 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      330 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/common.py
+-rw-r--r--   0        0        0     7968 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     7808 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3899 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     3292 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3830 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     5557 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     2297 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/unet.py
+-rw-r--r--   0        0        0      153 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     3551 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/image.py
+-rw-r--r--   0        0        0     3136 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5961 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/nms.py
+-rw-r--r--   0        0        0    11822 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/patches.py
+-rw-r--r--   0        0        0      482 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/uda.py
+-rw-r--r--   0        0        0       63 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/predict.py
+-rw-r--r--   0        0        0    12670 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/seqnms.py
+-rw-r--r--   0        0        0     6741 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/utils.py
+-rw-r--r--   0        0        0      203 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/__init__.py
+-rw-r--r--   0        0        0    10383 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/base_trainer.py
+-rw-r--r--   0        0        0    10541 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/lacss_trainer.py
+-rw-r--r--   0        0        0     1170 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/loss.py
+-rw-r--r--   0        0        0     4564 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/strategy.py
+-rw-r--r--   0        0        0     5541 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/utils.py
+-rw-r--r--   0        0        0      931 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/typing.py
+-rw-r--r--   0        0        0     5151 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/utils.py
+-rw-r--r--   0        0        0      995 2024-04-09 16:25:35.776837 lacss-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 lacss-0.8.0/PKG-INFO
```

### Comparing `lacss-0.7.6/LICENSE` & `lacss-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/README.md` & `lacss-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/data/augment.py` & `lacss-0.8.0/lacss/data/augment.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/data/generator.py` & `lacss-0.8.0/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/deploy/lacss_pb2.py` & `lacss-0.8.0/lacss/deploy/lacss_pb2.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/deploy/predict.py` & `lacss-0.8.0/lacss/deploy/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/deploy/server.py` & `lacss-0.8.0/lacss/deploy/server.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/losses/auxiliary.py` & `lacss-0.8.0/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/losses/common.py` & `lacss-0.8.0/lacss/losses/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/losses/detection.py` & `lacss-0.8.0/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/losses/instance.py` & `lacss-0.8.0/lacss/losses/instance.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/metrics/ranked.py` & `lacss-0.8.0/lacss/metrics/ranked.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
             indicators.append(0)
 
     return np.array(matches, np.int32), np.array(indicators, np.int32)
 
 
 def np_compute_ap(similarity_matrix, thresholds):
     # avoid edge cases
-    _, k = similarity_matrix.shape
-    if k == 0:
+    n, k = similarity_matrix.shape
+    if k == 0 or n == 0:
         return np.zeros([len(thresholds)], np.float32)
 
     apmks = []
     for th in thresholds:
         _, indicators = _unique_location_matching(similarity_matrix, th)
         p_k = np.cumsum(indicators) / (np.arange(len(indicators)) + 1)
         apmks.append(np.sum(p_k * indicators) / k)
@@ -80,15 +80,18 @@
             self.name = name
         self.reset()
 
     def update(self, sm, scores):
         self.cell_counts += sm.shape[1]
         self.scores.append(scores)
         for th, indicators in zip(self.thresholds, self.indicator_list):
-            _, ind = _unique_location_matching(sm, th)
+            if sm.shape[1] > 0:
+                _, ind = _unique_location_matching(sm, th)
+            else:
+                ind = np.zeros(sm.shape[0], dtype=np.int32)
             indicators.append(ind)
 
         self._result = None
 
     def compute(self):
         if self._result is not None:
             return self._result
```

### Comparing `lacss-0.7.6/lacss/modules/common.py` & `lacss-0.8.0/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/convnext.py` & `lacss-0.8.0/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/detector.py` & `lacss-0.8.0/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/lacss.py` & `lacss-0.8.0/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/lpn.py` & `lacss-0.8.0/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/resnet.py` & `lacss-0.8.0/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/segmentor.py` & `lacss-0.8.0/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/modules/unet.py` & `lacss-0.8.0/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/ops/boxes.py` & `lacss-0.8.0/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/ops/image.py` & `lacss-0.8.0/lacss/ops/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 ) -> Array:
     """Retrieve image values as non-integer locations by interpolation
 
     Args:
         img: Array of shape [D1,D2,..,Dk, ...]
         locs: Array of shape [d1,d2,..,dn, k]
         out_of_bound_value: optional float constant, defualt 0.
-        edge_indexing: if True, the index for the first value in img is 0.5, otherwise 0. Default is False
+        edge_indexing: if True, the index for the top/left pixel is 0.5, otherwise 0. Default is False
 
     Returns:
         values: [d1,d2,..,dn, ...], float
     """
 
     loc_shape = locs.shape
     img_shape = img.shape
@@ -103,15 +103,18 @@
 
     values = values.reshape(out_shape)
 
     return values
 
 
 def sub_pixel_crop_and_resize(
-    img: ArrayLike, bbox: ArrayLike, output_shape: Shape, out_of_bound_value: float = 0
+    img: ArrayLike,
+    bbox: ArrayLike,
+    output_shape: tuple[int],
+    out_of_bound_value: float = 0,
 ) -> Array:
     """Retrieve image values of a bbox. Resize output to output_shape. Used for ROI-Align.
 
     Args:
         img: Array of shape [H, W, ...]
         bbox: [y0, x0, y1, x1]
         output_shape: [h, w]
```

### Comparing `lacss-0.7.6/lacss/ops/locations.py` & `lacss-0.8.0/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/ops/nms.py` & `lacss-0.8.0/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/ops/patches.py` & `lacss-0.8.0/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/tracking/predict.py` & `lacss-0.8.0/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/tracking/seqnms.py` & `lacss-0.8.0/lacss/tracking/seqnms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/tracking/smc.py` & `lacss-0.8.0/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/tracking/utils.py` & `lacss-0.8.0/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.7.6/lacss/train/lacss_trainer.py` & `lacss-0.8.0/lacss/train/lacss_trainer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,86 @@
 from __future__ import annotations
 
 from dataclasses import asdict
 from functools import partial
 from pathlib import Path
-from typing import Iterable, Optional, Union
+from typing import Iterable, Optional, Union, Sequence
 
 import flax.linen as nn
+import jax
 import jax.numpy as jnp
 import optax
 import orbax.checkpoint as ocp
 from tqdm import tqdm
 
 import lacss.metrics
-from lacss.losses import (aux_size_loss, collaborator_border_loss,
-                          collaborator_segm_loss, lpn_loss, segmentation_loss)
 
-from ..modules import Lacss, LacssCollaborator
+from lacss.losses import (
+    aux_size_loss,
+    collaborator_border_loss,
+    collaborator_segm_loss,
+    lpn_loss,
+    segmentation_loss,
+)
+
+from ..modules import Lacss, UNet
 from ..typing import Array, Optimizer
 from .base_trainer import Trainer
 from .strategy import JIT
+from ..typing import *
+
+
+class LacssCollaborator(nn.Module):
+    """Collaborator module for semi-supervised Lacss training
 
+    Attributes:
+        conv_spec: conv-net specificaiton for cell border predicition
+        unet_spec: specification for unet, used to predict cell foreground
+        patch_size: patch size for the unet
+        n_cls: number of classes (cell types) of input images
+    """
+
+    conv_spec: Sequence[int] = (32, 32)
+    unet_spec: Sequence[int] = (16, 32, 64)
+    patch_size: int = 1
+    n_cls: int = 1
+
+    @nn.compact
+    def __call__(
+        self, image: ArrayLike, cls_id: Optional[ArrayLike] = None
+    ) -> DataDict:
+        assert cls_id is not None or self.n_cls == 1
+        c = cls_id.astype(int).squeeze() if cls_id is not None else 0
+
+        net = UNet(self.unet_spec, self.patch_size)
+        _, unet_out = net(image)
+
+        y = unet_out[str(net.start_level)]
+
+        fg = nn.Conv(self.n_cls, (3, 3))(y)
+        fg = fg[..., c]
+
+        if fg.shape != image.shape[:-1]:
+            fg = jax.image.resize(fg, image.shape[:-1], "linear")
+
+        y = image
+        for n_features in self.conv_spec:
+            y = nn.Conv(n_features, (3, 3), use_bias=False)(y)
+            y = nn.GroupNorm(num_groups=None, group_size=1, use_scale=False)(
+                y[None, ...]
+            )[0]
+            y = jax.nn.relu(y)
+
+        y = nn.Conv(self.n_cls, (3, 3))(y)
+        cb = y[..., c]
+
+        return dict(
+            fg_pred=fg,
+            edge_pred=cb,
+        )
 
 class _CKSModel(nn.Module):
     principal: Lacss
     collaborator: LacssCollaborator
 
     def __call__(self, image, cls_id=None, gt_locations=None, *, training=False):
         outputs = self.principal(
@@ -33,15 +90,15 @@
         )
 
         if self.collaborator is not None:
             outputs.update(self.collaborator(image=image, cls_id=cls_id))
         return outputs
 
 
-class LacssTrainer(Trainer):
+class LacssTrainer:
     """Main trainer class for Lacss"""
 
     default_lr: float = 0.001
 
     def __init__(
         self,
         config: dict = {},
@@ -67,117 +124,109 @@
         principal = Lacss.from_config(config)
 
         if collaborator_config is None:
             collaborator = None
         else:
             collaborator = LacssCollaborator(**collaborator_config)
 
-        super().__init__(
-            model=_CKSModel(
-                principal=principal,
-                collaborator=collaborator,
-            ),
-            optimizer=optimizer,
-            seed=seed,
-            strategy=strategy,
+        self.model = _CKSModel(
+            principal=principal,
+            collaborator=collaborator,
         )
 
-        if self.optimizer is None:
-            self.optimizer = optax.adamw(LacssTrainer.default_lr)
-
-        # self._cp_step = 0
-
-    def _train_to_next_interval(
-        self, train_iter, checkpoint_interval, checkpoint_dir, val_dataset
-    ):
-        cur_step = self.state.step
-        next_cp_step = (
-            (cur_step + checkpoint_interval)
-            // checkpoint_interval
-            * checkpoint_interval
-        )
-
-        for _ in tqdm(range(cur_step, next_cp_step)):
-            logs = next(train_iter)
-
-        print(", ".join([f"{k}:{v:.4f}" for k, v in logs.items()]))
-
-        if checkpoint_dir is not None:
-            cps = [int(p.name.split("-")[-1]) for p in checkpoint_dir.glob("chkpt-*")]
-            cp_cnt = max(cps) + 1
-            self.checkpoint(checkpoint_dir / f"chkpt-{cp_cnt}")
+        self.optimizer = optimizer or optax.adamw(LacssTrainer.default_lr)
+        self.seed = seed
+        self.strategy = strategy
+
+    def _train_to_next_interval(self, n_steps, trainer, train_iter, cpm, val_dataset):
+        for _ in tqdm(range(n_steps)):
+            next(train_iter)
+
+        print("Losses: " + repr(train_iter.loss_logs))
+
+        if cpm is not None:
+            cpm.save(
+                cpm.latest_step() + 1,
+                args=ocp.args.StandardSave(train_iter),
+            )
 
         if val_dataset is not None:
             val_metrics = [
                 lacss.metrics.LoiAP([5, 2, 1]),
                 lacss.metrics.BoxAP([0.5, 0.75]),
             ]
 
-            var_logs = self.test_and_compute(val_dataset, metrics=val_metrics)
+            var_logs = trainer.compute_metrics(
+                val_dataset,
+                val_metrics,
+                dict(params=train_iter.parameters),
+            )
+
             for k, v in var_logs.items():
                 print(f"{k}: {v}")
 
-    def _validate(self, val_dataset):
-        if val_dataset is not None:
-            val_metrics = [
-                lacss.metrics.LoiAP([5, 2, 1]),
-                lacss.metrics.BoxAP([0.5, 0.75]),
-            ]
+        train_iter.reset_loss_logs()
 
-            var_logs = self.test_and_compute(
-                val_dataset, metrics=val_metrics, strategy=JIT
-            )
-            for k, v in var_logs.items():
-                print(f"{k}: {v}")
+    def _get_warmup_trainer(self, sigma, pi):
+        pre_seg_loss = partial(segmentation_loss, pretraining=True)
+        pre_col_seg_loss = partial(collaborator_segm_loss, sigma=100.0, pi=1.0)
+        losses = [
+            lpn_loss,
+            pre_seg_loss,
+            pre_col_seg_loss,
+            collaborator_border_loss,
+            aux_size_loss,
+        ]
+        return Trainer(
+            model=self.model,
+            losses=losses,
+            optimizer=self.optimizer,
+            seed=self.seed,
+            strategy=self.strategy,
+        )
 
-    def _make_checkpoint(self, train_iter, checkpoint_manager):
-        if checkpoint_manager is not None:
-            print(train_iter.send(("checkpoint", checkpoint_manager)))
+    def _get_trainer(self, sigma, pi):
+        col_seg_loss = partial(collaborator_segm_loss, sigma=sigma, pi=pi)
+        losses = [
+            lpn_loss,
+            segmentation_loss,
+            col_seg_loss,
+            collaborator_border_loss,
+            aux_size_loss,
+        ]
+        return Trainer(
+            model=self.model,
+            losses=losses,
+            optimizer=self.optimizer,
+            seed=self.seed,
+            strategy=self.strategy,
+        )
 
-    def _reset(
-        self,
-        cur_step,
-        warmup_steps: int = 0,
-        sigma: float = 20.0,
-        pi: float = 2.0,
-    ) -> None:
-        if cur_step >= warmup_steps:
-            col_seg_loss = partial(collaborator_segm_loss, sigma=sigma, pi=pi)
-            # col_seg_loss.name = "collaborator_segm_loss"
-            self.losses = [
-                lpn_loss,
-                segmentation_loss,
-                col_seg_loss,
-                collaborator_border_loss,
-                aux_size_loss,
-            ]
-        else:
-            pre_seg_loss = partial(segmentation_loss, pretraining=True)
-            pre_col_seg_loss = partial(collaborator_segm_loss, sigma=100.0, pi=1.0)
-            self.losses = [
-                lpn_loss,
-                pre_seg_loss,
-                pre_col_seg_loss,
-                collaborator_border_loss,
-                aux_size_loss,
-            ]
+    def get_init_params(self, dataset):
+        trainer = self._get_trainer(20.0, 2.0)
+        train_it = trainer.train(
+            dataset, 
+            rng_cols=["droppath"],
+            training=True,
+        )
+        return train_it.parameters
 
-        self.reset()
 
     def do_training(
         self,
         dataset: Iterable,
         val_dataset: Iterable | None = None,
         n_steps: int = 50000,
         validation_interval: int = 5000,
         checkpoint_manager: Optional[ocp.CheckpointManager] = None,
         *,
         warmup_steps: int = 0,
         sigma: float = 20.0,
         pi: float = 2.0,
+        init_vars = None,
     ) -> None:
         """Runing training.
 
         Args:
             dataset: An data iterator feed training data. The data should be in the form of a tuple:
                 (x, y).
                     x is a dictionary with at least two keys:
@@ -206,43 +255,76 @@
 
         keyword Args:
             warmup_steps: Only used for point-supervised training. Pretraining steps, for which a large
                 sigma values is used. This should be multiples of validation_inteval
             sigma: Only for point-supervised training. Expected cell size
             pi: Only for point-supervised training. Amplitude of the prior term.
         """
-        train_iter = self.train(dataset, rng_cols=["droppath"], training=True)
         cur_step = 0
 
+        if cur_step < warmup_steps:
+            trainer = self._get_warmup_trainer(sigma, pi)
+            train_it = trainer.train(
+                dataset, 
+                rng_cols=["droppath"], 
+                init_vars=init_vars,
+                training=True,
+            )
+
+            while cur_step < warmup_steps:
+                next_cp_step = (
+                    (cur_step + validation_interval)
+                    // validation_interval
+                    * validation_interval
+                )
+
+                print(f"Current step {cur_step} going to {next_cp_step}")
+
+                self._train_to_next_interval(
+                    next_cp_step - cur_step,
+                    trainer,
+                    train_it,
+                    checkpoint_manager,
+                    val_dataset,
+                )
+
+                cur_step = next_cp_step
+
+                self.parameters = train_it.parameters
+
+            init_vars = dict(params=train_it.parameters)
+
+        trainer = self._get_trainer(sigma, pi)
+        train_it = trainer.train(
+            dataset,
+            rng_cols=["droppath"],
+            init_vars=init_vars,
+            training=True,
+        )
+
         while cur_step < n_steps:
             next_cp_step = (
                 (cur_step + validation_interval)
                 // validation_interval
                 * validation_interval
             )
 
-            self._reset(
-                cur_step,
-                warmup_steps=warmup_steps,
-                sigma=sigma,
-                pi=pi,
-            )
-
             print(f"Current step {cur_step} going to {next_cp_step}")
-            for _ in tqdm(range(cur_step, next_cp_step)):
-                logs = next(train_iter)
 
-            cur_step = next_cp_step
+            self._train_to_next_interval(
+                next_cp_step - cur_step,
+                trainer,
+                train_it,
+                checkpoint_manager,
+                val_dataset,
+            )
 
-            print(", ".join([f"{k}:{v:.4f}" for k, v in logs.items()]))
-            
-            self._make_checkpoint(train_iter, checkpoint_manager)
-            
-            self._validate(val_dataset)
+            cur_step = next_cp_step
 
+            self.parameters = train_it.parameters
 
     def save(self, save_path) -> None:
         """Save a pickled copy of the Lacss model in the form of (module:Lacss, weights:FrozenDict). Only saves the principal model.
 
         Args:
             save_path: Path to the pkl file
         """
```

### Comparing `lacss-0.7.6/lacss/typing.py` & `lacss-0.8.0/lacss/typing.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 Params = FrozenDict
 
 Optimizer = optax.GradientTransformation
 
 PathLike = Union[str, Path]
 
 
-class LossFunc(Protocol):
+class LossFunc_(Protocol):
     def __call__(self, batch: Any, prediction: Any) -> float:
         ...
 
 
+LossFunc = LossFunc_ | str
+
+
 class Metric(Protocol):
     def update(self, batch: Any, prediction: Any):
         ...
 
     def compute(self, *args, **kwargs) -> dict:
         ...
```

### Comparing `lacss-0.7.6/lacss/utils.py` & `lacss-0.8.0/lacss/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import dataclasses
 
 import jax.numpy as jnp
 import numpy as np
 from flax.core.frozen_dict import freeze, unfreeze
 
+from lacss.train.utils import pack_x_y_sample_weight, unpack_x_y_sample_weight
+
 
 def _to_str(p):
     return "".join(p.astype(int).reshape(-1).astype(str).tolist())
 
 
 def format_predictions(pred, mask=None, encode_patch=True, threshold=0.5):
     """Produce more readable data from model predictions
@@ -147,37 +149,14 @@
 
     if "params" in params and len(params) == 1:
         params = params["params"]
 
     return module, freeze(params)
 
 
-def pack_x_y_sample_weight(x, y=None, sample_weight=None):
-    """Packs user-provided data into a tuple."""
-    if y is None:
-        return (x,)
-    elif sample_weight is None:
-        return (x, y)
-    else:
-        return (x, y, sample_weight)
-
-
-def unpack_x_y_sample_weight(data):
-    """Unpacks user-provided data tuple."""
-    if not isinstance(data, tuple):
-        return (data, None, None)
-    elif len(data) == 1:
-        return (data[0], None, None)
-    elif len(data) == 2:
-        return (data[0], data[1], None)
-    elif len(data) == 3:
-        return (data[0], data[1], data[2])
-
-    raise ValueError("Data not understood.")
-
 def make_label_continuous(label, dtype=None):
     """ Relabel a label image so that the label values are continuous. It is assumed that the
     label starts with 0. If there is negative numbers in the input, they will be replaced by 0.
 
     Args:
         label: input label image
```

### Comparing `lacss-0.7.6/pyproject.toml` & `lacss-0.8.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacss"
-version = "0.7.6"
+version = "0.8.0"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
@@ -31,13 +31,12 @@
 mkdocs-material = "^9.2.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-gen-files = "^0.5.0"
 
 [[tool.poetry.source]]
 name = "jax"
 url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
-default = false
-secondary = false
+priority = "supplemental"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacss-0.7.6/PKG-INFO` & `lacss-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.7.6
+Version: 0.8.0
 Summary: Cell segmentation and tracking
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

