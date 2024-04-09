# Comparing `tmp/typed_ffmpeg-2.0.0a1.tar.gz` & `tmp/typed_ffmpeg-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed_ffmpeg-2.0.0a1.tar", max compression
+gzip compressed data, was "typed_ffmpeg-2.0.0a2.tar", max compression
```

## Comparing `typed_ffmpeg-2.0.0a1.tar` & `typed_ffmpeg-2.0.0a2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1066 2024-03-15 03:04:45.036248 typed_ffmpeg-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     5732 2024-03-15 03:04:45.036248 typed_ffmpeg-2.0.0a1/README.md
--rw-r--r--   0        0        0     3235 2024-03-15 03:05:01.900233 typed_ffmpeg-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      596 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/__init__.py
--rw-r--r--   0        0        0     3176 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/base.py
--rw-r--r--   0        0        0        0 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/common/__init__.py
--rw-r--r--   0        0        0     9460 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/common/schema.py
--rw-r--r--   0        0        0     4155 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/common/serialize.py
--rw-r--r--   0        0        0      286 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/__init__.py
--rw-r--r--   0        0        0     1565 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/compile.py
--rw-r--r--   0        0        0     5804 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/context.py
--rw-r--r--   0        0        0     1221 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/factory.py
--rw-r--r--   0        0        0        0 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/global_runnable/__init__.py
--rw-r--r--   0        0        0     7416 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/global_runnable/global_args.py
--rw-r--r--   0        0        0     5289 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/global_runnable/runnable.py
--rw-r--r--   0        0        0        0 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/__init__.py
--rw-r--r--   0        0        0     7020 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/_input.py
--rw-r--r--   0        0        0    12128 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/_output.py
--rw-r--r--   0        0        0    13602 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/output_args.py
--rw-r--r--   0        0        0    14210 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/nodes.py
--rw-r--r--   0        0        0     4956 2024-03-15 03:04:45.044248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/schema.py
--rw-r--r--   0        0        0     1141 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/utils.py
--rw-r--r--   0        0        0     5792 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/validate.py
--rw-r--r--   0        0        0      968 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/exceptions.py
--rw-r--r--   0        0        0   106428 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/filters.py
--rw-r--r--   0        0        0     1408 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/probe.py
--rw-r--r--   0        0        0        0 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/py.typed
--rw-r--r--   0        0        0      534 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/schema.py
--rw-r--r--   0        0        0      141 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/__init__.py
--rw-r--r--   0        0        0   238390 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/audio.py
--rw-r--r--   0        0        0      544 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/av.py
--rw-r--r--   0        0        0      662 2024-03-15 03:04:45.056248 typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/channel_layout.py
--rw-r--r--   0        0        0   421829 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/video.py
--rw-r--r--   0        0        0     3628 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/types.py
--rw-r--r--   0        0        0        0 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/__init__.py
--rw-r--r--   0        0        0     1208 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/escaping.py
--rw-r--r--   0        0        0      619 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/run.py
--rw-r--r--   0        0        0      813 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/snapshot.py
--rw-r--r--   0        0        0      316 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/typing.py
--rw-r--r--   0        0        0     1672 2024-03-15 03:04:45.060248 typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/view.py
--rw-r--r--   0        0        0     7014 1970-01-01 00:00:00.000000 typed_ffmpeg-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-15 04:04:00.773752 typed_ffmpeg-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     5732 2024-03-15 04:04:00.773752 typed_ffmpeg-2.0.0a2/README.md
+-rw-r--r--   0        0        0     3235 2024-03-15 04:04:17.001875 typed_ffmpeg-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      643 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/__init__.py
+-rw-r--r--   0        0        0     3176 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/base.py
+-rw-r--r--   0        0        0        0 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/common/__init__.py
+-rw-r--r--   0        0        0     9460 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/common/schema.py
+-rw-r--r--   0        0        0     4155 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/common/serialize.py
+-rw-r--r--   0        0        0      286 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/__init__.py
+-rw-r--r--   0        0        0     1565 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/compile.py
+-rw-r--r--   0        0        0     5804 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/context.py
+-rw-r--r--   0        0        0     1221 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/factory.py
+-rw-r--r--   0        0        0        0 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/global_runnable/__init__.py
+-rw-r--r--   0        0        0     7416 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/global_runnable/global_args.py
+-rw-r--r--   0        0        0     5289 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/global_runnable/runnable.py
+-rw-r--r--   0        0        0        0 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/__init__.py
+-rw-r--r--   0        0        0     7020 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/_input.py
+-rw-r--r--   0        0        0    12128 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/_output.py
+-rw-r--r--   0        0        0    13602 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/output_args.py
+-rw-r--r--   0        0        0    14210 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/nodes.py
+-rw-r--r--   0        0        0     4956 2024-03-15 04:04:00.781752 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/schema.py
+-rw-r--r--   0        0        0     1141 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/utils.py
+-rw-r--r--   0        0        0     5792 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/validate.py
+-rw-r--r--   0        0        0      968 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/exceptions.py
+-rw-r--r--   0        0        0   106428 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/filters.py
+-rw-r--r--   0        0        0     1408 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/probe.py
+-rw-r--r--   0        0        0        0 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/py.typed
+-rw-r--r--   0        0        0      534 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/schema.py
+-rw-r--r--   0        0        0      141 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/__init__.py
+-rw-r--r--   0        0        0   238390 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/audio.py
+-rw-r--r--   0        0        0      544 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/av.py
+-rw-r--r--   0        0        0      662 2024-03-15 04:04:00.793753 typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/channel_layout.py
+-rw-r--r--   0        0        0   421829 2024-03-15 04:04:00.797752 typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/video.py
+-rw-r--r--   0        0        0     3628 2024-03-15 04:04:00.797752 typed_ffmpeg-2.0.0a2/src/ffmpeg/types.py
+-rw-r--r--   0        0        0        0 2024-03-15 04:04:00.797752 typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/__init__.py
+-rw-r--r--   0        0        0     1208 2024-03-15 04:04:00.801752 typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/escaping.py
+-rw-r--r--   0        0        0      619 2024-03-15 04:04:00.801752 typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/run.py
+-rw-r--r--   0        0        0      813 2024-03-15 04:04:00.801752 typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/snapshot.py
+-rw-r--r--   0        0        0      316 2024-03-15 04:04:00.801752 typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/typing.py
+-rw-r--r--   0        0        0     1672 2024-03-15 04:04:00.801752 typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/view.py
+-rw-r--r--   0        0        0     7014 1970-01-01 00:00:00.000000 typed_ffmpeg-2.0.0a2/PKG-INFO
```

### Comparing `typed_ffmpeg-2.0.0a1/LICENSE` & `typed_ffmpeg-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/README.md` & `typed_ffmpeg-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/pyproject.toml` & `typed_ffmpeg-2.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typed-ffmpeg"
-version = "2.0.0a1"
+version = "2.0.0a2"
 description = "Modern Python FFmpeg wrappers offer comprehensive support for complex filters, complete with detailed typing and documentation."
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "ffmpeg", from = "src" }]
 include = ["ffmpeg/py.typed"]
 exclude = ["**/tests", "**/scripts"]
 license = "MIT"
```

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/__init__.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from . import dag, filters
 from .base import afilter, filter_multi_output, input, merge_outputs, output, vfilter
+from .common import serialize
 from .dag import Stream
 from .exceptions import FFMpegExecuteError, FFMpegTypeError, FFMpegValueError
 from .probe import probe
 from .streams import AudioStream, AVStream, VideoStream
 
 __all__ = [
+    "serialize",
     "filters",
     "input",
     "output",
     "merge_outputs",
     "FFMpegExecuteError",
     "FFMpegTypeError",
     "FFMpegValueError",
```

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/base.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/base.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/common/schema.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/common/schema.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/common/serialize.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/common/serialize.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/compile.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/compile.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/context.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/context.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/factory.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/factory.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/global_runnable/global_args.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/global_runnable/global_args.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/global_runnable/runnable.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/global_runnable/runnable.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/_input.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/_input.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/_output.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/_output.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/io/output_args.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/io/output_args.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/nodes.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/nodes.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/schema.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/schema.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/utils.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/utils.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/dag/validate.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/dag/validate.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/exceptions.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/exceptions.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/filters.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/filters.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/probe.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/probe.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/schema.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/schema.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/audio.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/audio.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/av.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/av.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/channel_layout.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/channel_layout.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/streams/video.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/streams/video.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/types.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/types.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/escaping.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/escaping.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/run.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/run.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/snapshot.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/src/ffmpeg/utils/view.py` & `typed_ffmpeg-2.0.0a2/src/ffmpeg/utils/view.py`

 * *Files identical despite different names*

### Comparing `typed_ffmpeg-2.0.0a1/PKG-INFO` & `typed_ffmpeg-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-ffmpeg
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Modern Python FFmpeg wrappers offer comprehensive support for complex filters, complete with detailed typing and documentation.
 Home-page: https://livingbio.github.io/typed-ffmpeg/
 License: MIT
 Keywords: ffmpeg,video,audio,multimedia,filter
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
```

