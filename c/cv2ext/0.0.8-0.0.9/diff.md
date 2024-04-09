# Comparing `tmp/cv2ext-0.0.8.tar.gz` & `tmp/cv2ext-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv2ext-0.0.8.tar", last modified: Wed Mar 13 19:54:32 2024, max compression
+gzip compressed data, was "cv2ext-0.0.9.tar", last modified: Sat Mar 30 23:44:56 2024, max compression
```

## Comparing `cv2ext-0.0.8.tar` & `cv2ext-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.127900 cv2ext-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 19:54:24.000000 cv2ext-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-13 19:54:24.000000 cv2ext-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-13 19:54:32.127900 cv2ext-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-13 19:54:24.000000 cv2ext-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-03-13 19:54:24.000000 cv2ext-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 19:54:32.127900 cv2ext-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.115900 cv2ext-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.119900 cv2ext-0.0.8/src/cv2ext/
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/_iterablevideo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.119900 cv2ext-0.0.8/src/cv2ext/bboxes/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/bboxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/bboxes/_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/bboxes/_mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/bboxes/_nms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.119900 cv2ext-0.0.8/src/cv2ext/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.119900 cv2ext-0.0.8/src/cv2ext/cli/annotate/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/annotate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/annotate/_annotate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.123900 cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.123900 cv2ext-0.0.8/src/cv2ext/cli/resize_video/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/resize_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/resize_video/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/cli/resize_video/_resize_video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.123900 cv2ext-0.0.8/src/cv2ext/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/metrics/_ncc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.123900 cv2ext-0.0.8/src/cv2ext/template/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-13 19:54:24.000000 cv2ext-0.0.8/src/cv2ext/template/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:54:32.123900 cv2ext-0.0.8/src/cv2ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-13 19:54:32.000000 cv2ext-0.0.8/src/cv2ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-13 19:54:32.000000 cv2ext-0.0.8/src/cv2ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:54:32.000000 cv2ext-0.0.8/src/cv2ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-13 19:54:32.000000 cv2ext-0.0.8/src/cv2ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 19:54:32.000000 cv2ext-0.0.8/src/cv2ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.972254 cv2ext-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-30 23:44:50.000000 cv2ext-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-30 23:44:50.000000 cv2ext-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-30 23:44:56.972254 cv2ext-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-30 23:44:50.000000 cv2ext-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-03-30 23:44:50.000000 cv2ext-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 23:44:56.972254 cv2ext-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.964254 cv2ext-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.964254 cv2ext-0.0.9/src/cv2ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/_iterablevideo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.964254 cv2ext-0.0.9/src/cv2ext/bboxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/bboxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/bboxes/_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/bboxes/_mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/bboxes/_nms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/cli/annotate/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/annotate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/annotate/_annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/cli/resize_video/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/resize_video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/resize_video/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/resize_video/_resize_video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/cli/timeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/timeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/timeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/cli/timeline/_timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/metrics/_ncc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-30 23:44:50.000000 cv2ext-0.0.9/src/cv2ext/template/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:44:56.968254 cv2ext-0.0.9/src/cv2ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-30 23:44:56.000000 cv2ext-0.0.9/src/cv2ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-30 23:44:56.000000 cv2ext-0.0.9/src/cv2ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 23:44:56.000000 cv2ext-0.0.9/src/cv2ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-30 23:44:56.000000 cv2ext-0.0.9/src/cv2ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-30 23:44:56.000000 cv2ext-0.0.9/src/cv2ext.egg-info/top_level.txt
```

### Comparing `cv2ext-0.0.8/LICENSE` & `cv2ext-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/PKG-INFO` & `cv2ext-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2ext
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Justin Davis <davisjustin302@gmail.com>
 Maintainer-email: Justin Davis <davisjustin302@gmail.com>
 Project-URL: Homepage, https://github.com/justincdavis/cv2ext
 Project-URL: Bug Tracker, https://github.com/justincdavis/cv2ext/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cv2ext-0.0.8/README.md` & `cv2ext-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/pyproject.toml` & `cv2ext-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cv2ext"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   {name="Justin Davis", email="davisjustin302@gmail.com"},
 ]
 maintainers = [
   {name="Justin Davis", email="davisjustin302@gmail.com"},
 ]
 readme = "README.md"
@@ -79,15 +79,15 @@
     "bumpver>=2023.1126",
     "pyclean>=2.7.0",
     "pyright>=1.1.348",
     "seaborn>=0.13.0",
 ]
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `cv2ext-0.0.8/src/cv2ext/__init__.py` & `cv2ext-0.0.9/src/cv2ext/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,36 @@
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 # ruff: noqa: E402, I001
 """
 Package containing helpful tools for working with opencv.
 
 Submodules
 ----------
+bboxes
+    Submodule containing tools for working with bounding boxes in images.
 cli
     Submodule containing command line interface tools.
 template
     Submodule containing tools for working with templates in images.
 metrics
     Submodule containing tools for working with image metrics.
 
 Classes
 -------
 Display
     A class for displaying images using a separate thread.
 IterableVideo
     A class for iterating over frames in a video, optionally with threading.
+
+Functions
+---------
+set_log_level
+    Set the log level for the cv2ext package.
+enable_jit
+    Enable just-in-time compilation using Numba for some functions.
 """
 from __future__ import annotations
 
 # setup the logger before importing anything else
 import logging
 import os
 import sys
@@ -66,15 +75,15 @@
     stdout_handler.setLevel(log_level)
     stdout_handler.setFormatter(formatter)
     logger.addHandler(stdout_handler)
 
 
 def set_log_level(level: str) -> None:
     """
-    Set the log level for the oakutils package.
+    Set the log level for the cv2ext package.
 
     Parameters
     ----------
     level : str
         The log level to set. One of "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL".
 
     Raises
@@ -85,15 +94,15 @@
     """
     if level.upper() not in ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]:
         err_msg = f"Invalid log level: {level}"
         raise ValueError(err_msg)
     _setup_logger(level)
 
 
-level = os.getenv("OAKUTILS_LOG_LEVEL")
+level = os.getenv("CV2EXT_LOG_LEVEL")
 _setup_logger(level)
 _log = logging.getLogger(__name__)
 if level is not None and level.upper() not in [
     "DEBUG",
     "INFO",
     "WARNING",
     "ERROR",
@@ -182,15 +191,15 @@
     ----------
     on : bool | None
         If True, enable jit. If False, disable jit. If None, enable jit.
 
     """
     if on is None:
         on = True
-    _FLAGS.USEJIT = on
+    _FLAGSOBJ.USEJIT = on
     _log.info(f"JIT is {'enabled' if on else 'disabled'}.")
 
 
 from . import bboxes, metrics, template
 from ._display import Display
 from ._iterablevideo import IterableVideo
 
@@ -202,15 +211,15 @@
     "bboxes",
     "cli",
     "enable_jit",
     "metrics",
     "set_log_level",
     "template",
 ]
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 _log.info(f"Initialized cv2ext with version {__version__}")
 
 from . import cli
 
 _log.info("cv2ext.cli initialized.")
```

### Comparing `cv2ext-0.0.8/src/cv2ext/_display.py` & `cv2ext-0.0.9/src/cv2ext/_display.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,30 +80,62 @@
         # thread allocation
         _DELOBJ.logwindow(self._windowname)
         self._thread = Thread(target=self._display, daemon=True)
         self._thread.start()
 
     @property
     def frame(self: Self) -> np.ndarray:
-        """The most recent frame."""
+        """
+        The most recent frame.
+
+        Returns
+        -------
+        np.ndarray
+            The most recent frame.
+
+        """
         return self._image
 
     @property
     def frameid(self: Self) -> int:
-        """The current frame id."""
+        """
+        The current frame id.
+
+        Returns
+        -------
+        int
+            The current frame id.
+
+        """
         return self._frameid
 
     @property
     def stopped(self: Self) -> bool:
-        """Whether the display is stopped."""
+        """
+        Whether the display is stopped.
+
+        Returns
+        -------
+        bool
+            Whether the display is stopped.
+
+        """
         return not self._running
 
     @property
     def is_alive(self: Self) -> bool:
-        """Whether the display is running."""
+        """
+        Whether the display is running.
+
+        Returns
+        -------
+        bool
+            Whether the display is running.
+
+        """
         return self._thread.is_alive()
 
     def __call__(self: Self, frame: np.ndarray) -> None:
         """
         Update the frame being displayed.
 
         Parameters
@@ -157,17 +189,12 @@
         Update the frame being displayed.
 
         Parameters
         ----------
         frame : np.ndarray
             The frame to display.
 
-        Raises
-        ------
-        queue.Full
-            If timeout is provided, and the queue if full at the end of timeout.
-
         """
         self._image = frame
         self._frameid += 1
         with contextlib.suppress(Full):
             self._queue.put_nowait(frame)
```

### Comparing `cv2ext-0.0.8/src/cv2ext/_iterablevideo.py` & `cv2ext-0.0.9/src/cv2ext/_iterablevideo.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/bboxes/__init__.py` & `cv2ext-0.0.9/src/cv2ext/bboxes/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/bboxes/_iou.py` & `cv2ext-0.0.9/src/cv2ext/bboxes/_iou.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/bboxes/_mean_ap.py` & `cv2ext-0.0.9/src/cv2ext/bboxes/_mean_ap.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/bboxes/_nms.py` & `cv2ext-0.0.9/src/cv2ext/bboxes/_nms.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/__init__.py` & `cv2ext-0.0.9/src/cv2ext/cli/resize_video/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 """
-Command line interface for cv2ext.
+Resize videos using opencv.
 
-Submodules
-----------
-annotate
-    Annotate videos with bounding boxes.
+Functions
+---------
 resize_video
-    Resize videos using opencv.
+    Resize a video file.
 """
 from __future__ import annotations
 
-from . import annotate, resize_video
+from ._resize_video import resize_video
 
-__all__ = ["annotate", "resize_video"]
+__all__ = ["resize_video"]
```

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/annotate/__init__.py` & `cv2ext-0.0.9/src/cv2ext/cli/annotate/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/annotate/__main__.py` & `cv2ext-0.0.9/src/cv2ext/cli/annotate/__main__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/annotate/_annotate.py` & `cv2ext-0.0.9/src/cv2ext/cli/annotate/_annotate.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/__init__.py` & `cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/__main__.py` & `cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/__main__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/convert_annotations/_convert.py` & `cv2ext-0.0.9/src/cv2ext/cli/convert_annotations/_convert.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/resize_video/__init__.py` & `cv2ext-0.0.9/src/cv2ext/cli/resize_video/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-Resize videos using opencv.
-
-Functions
----------
-resize_video
-    Resize a video file.
-"""
+"""Resize videos using opencv."""
 from __future__ import annotations
 
 from ._resize_video import resize_video
 
-__all__ = ["resize_video"]
+if __name__ == "__main__":
+    resize_video()
```

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/resize_video/__main__.py` & `cv2ext-0.0.9/src/cv2ext/cli/timeline/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""Resize videos using opencv."""
+"""Create a timeline of a video."""
 from __future__ import annotations
 
-from ._resize_video import resize_video
+from ._timeline import timeline_cli
 
 if __name__ == "__main__":
-    resize_video()
+    timeline_cli()
```

### Comparing `cv2ext-0.0.8/src/cv2ext/cli/resize_video/_resize_video.py` & `cv2ext-0.0.9/src/cv2ext/cli/resize_video/_resize_video.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/metrics/__init__.py` & `cv2ext-0.0.9/src/cv2ext/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/metrics/_ncc.py` & `cv2ext-0.0.9/src/cv2ext/metrics/_ncc.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/template/__init__.py` & `cv2ext-0.0.9/src/cv2ext/template/__init__.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext/template/_core.py` & `cv2ext-0.0.9/src/cv2ext/template/_core.py`

 * *Files identical despite different names*

### Comparing `cv2ext-0.0.8/src/cv2ext.egg-info/PKG-INFO` & `cv2ext-0.0.9/src/cv2ext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv2ext
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Justin Davis <davisjustin302@gmail.com>
 Maintainer-email: Justin Davis <davisjustin302@gmail.com>
 Project-URL: Homepage, https://github.com/justincdavis/cv2ext
 Project-URL: Bug Tracker, https://github.com/justincdavis/cv2ext/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cv2ext-0.0.8/src/cv2ext.egg-info/SOURCES.txt` & `cv2ext-0.0.9/src/cv2ext.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,14 @@
 src/cv2ext/cli/annotate/_annotate.py
 src/cv2ext/cli/convert_annotations/__init__.py
 src/cv2ext/cli/convert_annotations/__main__.py
 src/cv2ext/cli/convert_annotations/_convert.py
 src/cv2ext/cli/resize_video/__init__.py
 src/cv2ext/cli/resize_video/__main__.py
 src/cv2ext/cli/resize_video/_resize_video.py
+src/cv2ext/cli/timeline/__init__.py
+src/cv2ext/cli/timeline/__main__.py
+src/cv2ext/cli/timeline/_timeline.py
 src/cv2ext/metrics/__init__.py
 src/cv2ext/metrics/_ncc.py
 src/cv2ext/template/__init__.py
 src/cv2ext/template/_core.py
```

### Comparing `cv2ext-0.0.8/src/cv2ext.egg-info/requires.txt` & `cv2ext-0.0.9/src/cv2ext.egg-info/requires.txt`

 * *Files identical despite different names*

