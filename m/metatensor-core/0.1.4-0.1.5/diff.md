# Comparing `tmp/metatensor-core-0.1.4.tar.gz` & `tmp/metatensor-core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor-core-0.1.4.tar", last modified: Fri Mar  1 16:57:46 2024, max compression
+gzip compressed data, was "metatensor-core-0.1.5.tar", last modified: Tue Apr  9 14:00:51 2024, max compression
```

## Comparing `metatensor-core-0.1.4.tar` & `metatensor-core-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:57:46.694169 metatensor-core-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-01 16:57:46.694169 metatensor-core-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:57:46.690169 metatensor-core-0.1.4/metatensor/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/_c_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/_c_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:57:46.690169 metatensor-core-0.1.4/metatensor/data/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/data/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/data/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    38675 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    27761 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/metatensor/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    84202 2024-03-01 16:57:42.000000 metatensor-core-0.1.4/metatensor-core-cxx-0.1.4.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:57:46.694169 metatensor-core-0.1.4/metatensor_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/metatensor_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/metatensor_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/metatensor_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/metatensor_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/metatensor_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/metatensor_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:57:46.000000 metatensor-core-0.1.4/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:57:46.694169 metatensor-core-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-03-01 16:57:35.000000 metatensor-core-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 14:00:37.000000 metatensor-core-0.1.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-09 14:00:37.000000 metatensor-core-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.740420 metatensor-core-0.1.5/metatensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/_c_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/_c_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.740420 metatensor-core-0.1.5/metatensor/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/data/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/data/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38710 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86573 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor-core-cxx-0.1.5.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/metatensor_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:50.000000 metatensor-core-0.1.5/metatensor_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:50.000000 metatensor-core-0.1.5/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/setup.py
```

### Comparing `metatensor-core-0.1.4/LICENSE` & `metatensor-core-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/PKG-INFO` & `metatensor-core-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/core/CHANGELOG.html
@@ -23,15 +23,15 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: numpy
+Requires-Dist: numpy<2.0
 
 metatensor-core
 ===============
 
 This package contains the Python bindings to the core C API of metatensor. Most
 users will want to use the ``metatensor`` meta package instead, which also
 includes function to operate on the data.
```

### Comparing `metatensor-core-0.1.4/metatensor/__init__.py` & `metatensor-core-0.1.5/metatensor/__init__.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/metatensor/_c_api.py` & `metatensor-core-0.1.5/metatensor/_c_api.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/metatensor/_c_lib.py` & `metatensor-core-0.1.5/metatensor/_c_lib.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/metatensor/block.py` & `metatensor-core-0.1.5/metatensor/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import copy
 import ctypes
 import warnings
-from typing import Generator, List, Optional, Sequence, Tuple
+from typing import Generator, List, Sequence, Tuple
 
 from . import data
 from ._c_api import c_uintptr_t, mts_array_t, mts_block_t, mts_labels_t
 from ._c_lib import _get_library
 from .data import (
     Array,
     ArrayWrapper,
     Device,
     DeviceWarning,
     DType,
     mts_array_to_python_array,
 )
 from .labels import Labels
 from .status import _check_pointer
+from .utils import _to_arguments_parse
 
 
 class TensorBlock:
     """
     Basic building block for a :py:class:`TensorMap`.
 
     A single block contains a n-dimensional :py:class:`metatensor.data.Array`,
@@ -466,32 +467,30 @@
     def device(self) -> Device:
         """
         Get the device of all the values and gradient arrays stored inside this
         :py:class:`TensorBlock`.
         """
         return data.array_device(self.values)
 
-    def to(
-        self,
-        *,
-        dtype: Optional[DType] = None,
-        device: Optional[Device] = None,
-        arrays: Optional[str] = None,
-    ) -> "TensorBlock":
+    def to(self, *args, **kwargs) -> "TensorBlock":
         """
         Move all the arrays in this block (values and gradients) to the given ``dtype``,
         ``device`` and ``arrays`` backend.
 
         :param dtype: new dtype to use for all arrays. The dtype stays the same if this
             is set to ``None``.
         :param device: new device to use for all arrays. The device stays the same if
             this is set to ``None``.
         :param arrays: new backend to use for the arrays. This can be either
-            ``"numpy"``, ``"torch"`` or ``None`` (keeps the existing backend)
+            ``"numpy"``, ``"torch"`` or ``None`` (keeps the existing backend); and must
+            be given as a keyword argument (``arrays="numpy"``).
         """
+        arrays = kwargs.pop("arrays", None)
+        dtype, device = _to_arguments_parse("`TensorBlock.to`", *args, **kwargs)
+
         values = self.values
 
         if arrays is not None:
             values = data.array_change_backend(values, arrays)
 
         if dtype is not None:
             values = data.array_change_dtype(values, dtype)
```

### Comparing `metatensor-core-0.1.4/metatensor/data/array.py` & `metatensor-core-0.1.5/metatensor/data/array.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/metatensor/data/extract.py` & `metatensor-core-0.1.5/metatensor/data/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
         return obj
 
     def __array_finalize__(self, obj):
         # keep the parent around when creating sub-views of this array
         self._parent = getattr(obj, "_parent", None)
 
-    def __array_wrap__(self, new):
+    def __array_wrap__(self, new, context=None, return_scalar=False):
         self_ptr = self.ctypes.data
         self_size = self.nbytes
 
         new_ptr = new.ctypes.data
 
         if self_ptr <= new_ptr <= self_ptr + self_size:
             # if the new array is a view inside memory owned by self, wrap it in
```

### Comparing `metatensor-core-0.1.4/metatensor/io.py` & `metatensor-core-0.1.5/metatensor/io.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/metatensor/labels.py` & `metatensor-core-0.1.5/metatensor/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         return obj
 
     def __array_finalize__(self, obj):
         # keep the parent around when creating sub-views of this array
         self._parent = getattr(obj, "_parent", None)
 
-    def __array_wrap__(self, new):
+    def __array_wrap__(self, new, context=None, return_scalar=False):
         self_ptr = self.ctypes.data
         self_size = self.nbytes
 
         new_ptr = new.ctypes.data
 
         if self_ptr <= new_ptr <= self_ptr + self_size:
             # if the new array is a view inside memory owned by self, wrap it in
```

### Comparing `metatensor-core-0.1.4/metatensor/status.py` & `metatensor-core-0.1.5/metatensor/status.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.4/metatensor/tensor.py` & `metatensor-core-0.1.5/metatensor/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import copy
 import ctypes
 import pathlib
 import warnings
 from pickle import PickleBuffer
-from typing import BinaryIO, Dict, List, Optional, Sequence, Union
+from typing import BinaryIO, Dict, List, Sequence, Union
 
 import numpy as np
 
 from . import data
 from ._c_api import c_uintptr_t, mts_block_t, mts_labels_t
 from ._c_lib import _get_library
 from .block import TensorBlock
 from .data import Device, DeviceWarning, DType
 from .labels import Labels, LabelsEntry
 from .status import _check_pointer
+from .utils import _to_arguments_parse
 
 
 class TensorMap:
     """
     A TensorMap is the main user-facing class of this library, and can store any kind of
     data used in atomistic machine learning similar to a Python :py:class:`dict`.
 
@@ -669,37 +670,37 @@
     def dtype(self) -> DType:
         """get the dtype of all the arrays stored inside this :py:class:`TensorMap`"""
         if len(self.keys) == 0:
             return None
 
         return self.block_by_id(0).dtype
 
-    def to(
-        self,
-        *,
-        dtype: Optional[DType] = None,
-        device: Optional[Device] = None,
-        arrays: Optional[str] = None,
-    ) -> "TensorMap":
+    def to(self, *args, **kwargs) -> "TensorMap":
         """
-        Move all the arrays in this block (values and gradients) to the given ``dtype``,
-        ``device`` and ``arrays`` backend.
+        Move the keys and all the blocks in this :py:class:`TensorMap` to the given
+        ``dtype``, ``device`` and ``arrays`` backend.
+
+        The arguments to this function can be given as positional or keyword arguments.
 
         :param dtype: new dtype to use for all arrays. The dtype stays the same if this
             is set to ``None``.
         :param device: new device to use for all arrays. The device stays the same if
             this is set to ``None``.
         :param arrays: new backend to use for the arrays. This can be either
-            ``"numpy"``, ``"torch"`` or ``None`` (keeps the existing backend)
+            ``"numpy"``, ``"torch"`` or ``None`` (keeps the existing backend); and must
+            be given as a keyword argument (``arrays="numpy"``).
         """
+        arrays = kwargs.pop("arrays", None)
+        dtype, device = _to_arguments_parse("`TensorMap.to`", *args, **kwargs)
+
         blocks = []
 
         with warnings.catch_warnings():
-            # do not warn on device mismatch here, there will be a warning when
-            # constructing the TensorMap
+            # do not warn on device mismatch between values/labels here,
+            # there will be a warning when constructing the TensorMap
             warnings.simplefilter("ignore", DeviceWarning)
 
             for block in self.blocks():
                 blocks.append(block.to(dtype=dtype, device=device, arrays=arrays))
 
         return TensorMap(self.keys, blocks)
 
@@ -728,20 +729,27 @@
     for i, v in enumerate(strings):
         assert isinstance(v, str)
         c_strings[i] = v.encode("utf8")
 
     return c_strings
 
 
+def _can_cast_to_numpy_int(value):
+    return np.can_cast(value, np.int32, casting="same_kind")
+
+
 def _normalize_selection(
     selection: Union[Labels, LabelsEntry, Dict[str, int]]
 ) -> Labels:
     if isinstance(selection, dict):
         for key, value in selection.items():
-            if not np.can_cast(value, np.int32, casting="same_kind"):
+            if isinstance(value, int):
+                # all good
+                pass
+            elif isinstance(value, float) or not _can_cast_to_numpy_int(value):
                 raise TypeError(
                     f"expected integer values in selection, got {key}={value} of "
                     f"type {type(value)}"
                 )
 
         if len(selection) == 0:
             return Labels([], np.empty((0, 0), dtype=np.int32))
```

### Comparing `metatensor-core-0.1.4/metatensor_core.egg-info/PKG-INFO` & `metatensor-core-0.1.5/metatensor_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/core/CHANGELOG.html
@@ -23,15 +23,15 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: numpy
+Requires-Dist: numpy<2.0
 
 metatensor-core
 ===============
 
 This package contains the Python bindings to the core C API of metatensor. Most
 users will want to use the ``metatensor`` meta package instead, which also
 includes function to operate on the data.
```

### Comparing `metatensor-core-0.1.4/metatensor_core.egg-info/SOURCES.txt` & `metatensor-core-0.1.5/metatensor_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
-metatensor-core-cxx-0.1.4.tar.gz
+metatensor-core-cxx-0.1.5.tar.gz
 n_commits_since_last_tag
 pyproject.toml
 setup.py
 metatensor/__init__.py
 metatensor/_c_api.py
 metatensor/_c_lib.py
 metatensor/block.py
```

### Comparing `metatensor-core-0.1.4/pyproject.toml` & `metatensor-core-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = ["version", "authors"]
 requires-python = ">=3.8"
 
 readme = "README.rst"
 license = {text = "BSD-3-Clause"}
 description = "Python bindings for metatensor"
 
-dependencies = ["numpy"]
+dependencies = ["numpy <2.0"]
 
 keywords = ["machine learning", "molecular modeling"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX",
```

### Comparing `metatensor-core-0.1.4/setup.py` & `metatensor-core-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 METATENSOR_CORE = os.path.join(ROOT, "..", "..", "metatensor-core")
 
 
 class universal_wheel(bdist_wheel):
     # When building the wheel, the `wheel` package assumes that if we have a
     # binary extension then we are linking to `libpython.so`; and thus the wheel
     # is only usable with a single python version. This is not the case for
-    # here, and the wheel will be compatible with any Python >=3.7. This is
+    # here, and the wheel will be compatible with any Python >=3. This is
     # tracked in https://github.com/pypa/wheel/issues/185, but until then we
     # manually override the wheel tag.
     def get_tag(self):
         tag = bdist_wheel.get_tag(self)
         # tag[2:] contains the os/arch tags, we want to keep them
         return ("py3", "none") + tag[2:]
 
@@ -98,15 +98,15 @@
 
         subprocess.run(
             ["cmake", source_dir, *cmake_options],
             cwd=build_dir,
             check=True,
         )
         subprocess.run(
-            ["cmake", "--build", build_dir, "--target", "install"],
+            ["cmake", "--build", build_dir, "--parallel", "--target", "install"],
             check=True,
         )
 
 
 class bdist_egg_disabled(bdist_egg):
     """Disabled version of bdist_egg
 
@@ -118,28 +118,65 @@
         sys.exit(
             "Aborting implicit building of eggs.\nUse `pip install .` or "
             "`python -m build --wheel . && pip install "
             "dist/metatensor_core-*.whl` to install from source."
         )
 
 
-class sdist_git_version(sdist):
+class sdist_generate_data(sdist):
     """
-    Create a sdist with an additional generated file containing the extra
-    version from git.
+    Create a sdist with an additional generated files:
+        - `n_commits_since_last_tag`
+        - `metatensor-core-cxx-*.tar.gz`
     """
 
     def run(self):
         with open("n_commits_since_last_tag", "w") as fd:
             fd.write(str(n_commits_since_last_tag()))
 
+        generate_cxx_tar()
+
         # run original sdist
         super().run()
 
         os.unlink("n_commits_since_last_tag")
+        for path in glob.glob("metatensor-core-cxx-*.tar.gz"):
+            os.unlink(path)
+
+
+def generate_cxx_tar():
+    script = os.path.join(ROOT, "..", "..", "scripts", "package-core.sh")
+    assert os.path.exists(script)
+
+    try:
+        output = subprocess.run(
+            ["bash", "--version"],
+            stderr=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            encoding="utf8",
+        )
+    except Exception as e:
+        raise RuntimeError("could not run `bash`, is it installed?") from e
+
+    stderr = ""
+    stdout = ""
+
+    output = subprocess.run(
+        ["bash", script, os.getcwd()],
+        stderr=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        encoding="utf8",
+    )
+    if output.returncode != 0:
+        stderr = output.stderr
+        stdout = output.stdout
+        raise RuntimeError(
+            "failed to collect C++ sources for Python sdist\n"
+            f"stdout:\n {stdout}\n\nstderr:\n {stderr}"
+        )
 
 
 def get_rust_version():
     # read version from Cargo.toml
     with open(os.path.join(METATENSOR_CORE, "Cargo.toml")) as fd:
         for line in fd:
             if line.startswith("version"):
@@ -254,15 +291,15 @@
             # in the build_ext command
             Extension(name="metatensor", sources=[]),
         ],
         cmdclass={
             "build_ext": cmake_ext,
             "bdist_egg": bdist_egg if "bdist_egg" in sys.argv else bdist_egg_disabled,
             "bdist_wheel": universal_wheel,
-            "sdist": sdist_git_version,
+            "sdist": sdist_generate_data,
         },
         package_data={
             "metatensor-core": [
                 "metatensor/core/lib/*",
                 "metatensor/core/include/*",
             ]
         },
```

