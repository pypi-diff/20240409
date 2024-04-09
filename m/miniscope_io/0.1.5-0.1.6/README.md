# Comparing `tmp/miniscope_io-0.1.5.tar.gz` & `tmp/miniscope_io-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniscope_io-0.1.5.tar", max compression
+gzip compressed data, was "miniscope_io-0.1.6.tar", max compression
```

## Comparing `miniscope_io-0.1.5.tar` & `miniscope_io-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,41 @@
--rw-r--r--   0        0        0    34523 2023-06-27 01:14:55.751020 miniscope_io-0.1.5/LICENSE
--rw-r--r--   0        0        0      140 2023-06-27 01:18:46.012470 miniscope_io-0.1.5/README.md
--rw-r--r--   0        0        0       34 2023-09-04 02:37:44.114858 miniscope_io-0.1.5/miniscope_io/__init__.py
--rw-r--r--   0        0        0     2514 2023-09-04 02:44:05.693011 miniscope_io-0.1.5/miniscope_io/data.py
--rw-r--r--   0        0        0      310 2023-09-04 02:37:44.116710 miniscope_io-0.1.5/miniscope_io/exceptions.py
--rw-r--r--   0        0        0     2729 2023-09-04 02:44:05.693276 miniscope_io-0.1.5/miniscope_io/formats.py
--rw-r--r--   0        0        0    17218 2023-09-04 05:17:51.243351 miniscope_io-0.1.5/miniscope_io/io.py
--rw-r--r--   0        0        0        0 2023-09-04 02:44:05.693784 miniscope_io-0.1.5/miniscope_io/plots/__init__.py
--rw-r--r--   0        0        0     2420 2023-09-04 02:44:05.694041 miniscope_io-0.1.5/miniscope_io/plots/headers.py
--rw-r--r--   0        0        0     4302 2023-09-04 02:44:05.694811 miniscope_io-0.1.5/miniscope_io/sdcard.py
--rw-r--r--   0        0        0    16759 2023-09-04 05:17:51.244155 miniscope_io-0.1.5/miniscope_io/uart_daq.py
--rw-r--r--   0        0        0      589 2023-09-04 05:17:51.244413 miniscope_io-0.1.5/miniscope_io/utils.py
--rw-r--r--   0        0        0       52 2023-06-24 01:08:40.857671 miniscope_io-0.1.5/miniscope_io/widgets.py
--rw-r--r--   0        0        0     1121 2023-09-04 05:17:51.247454 miniscope_io-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 miniscope_io-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-27 01:14:55.751020 miniscope_io-0.1.6/LICENSE
+-rw-r--r--   0        0        0      390 2024-04-09 19:35:02.635495 miniscope_io-0.1.6/README.md
+-rw-r--r--   0        0        0       34 2023-10-30 20:07:19.823684 miniscope_io-0.1.6/miniscope_io/__init__.py
+-rw-r--r--   0        0        0     2514 2023-09-04 02:44:05.693011 miniscope_io-0.1.6/miniscope_io/data.py
+-rw-r--r--   0        0        0  1516936 2024-04-09 19:35:02.648205 miniscope_io-0.1.6/miniscope_io/devices/USBInterface-8mhz-3v3-dbg.bit
+-rw-r--r--   0        0        0        0 2024-04-09 19:35:02.648818 miniscope_io-0.1.6/miniscope_io/devices/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-09 19:35:02.649155 miniscope_io-0.1.6/miniscope_io/devices/opalkelly.py
+-rw-r--r--   0        0        0      310 2023-10-23 18:45:53.286043 miniscope_io-0.1.6/miniscope_io/exceptions.py
+-rw-r--r--   0        0        0     2729 2023-09-04 02:44:05.693276 miniscope_io-0.1.6/miniscope_io/formats.py
+-rw-r--r--   0        0        0    17218 2023-10-23 18:45:53.287422 miniscope_io-0.1.6/miniscope_io/io.py
+-rw-r--r--   0        0        0        0 2023-09-04 02:44:05.693784 miniscope_io-0.1.6/miniscope_io/plots/__init__.py
+-rw-r--r--   0        0        0     2420 2023-10-23 18:45:53.288071 miniscope_io-0.1.6/miniscope_io/plots/headers.py
+-rw-r--r--   0        0        0     4302 2023-09-04 02:44:05.694811 miniscope_io-0.1.6/miniscope_io/sdcard.py
+-rw-r--r--   0        0        0    29549 2024-04-09 19:35:02.649644 miniscope_io-0.1.6/miniscope_io/stream_daq.py
+-rw-r--r--   0        0        0      589 2023-09-04 05:17:51.244413 miniscope_io-0.1.6/miniscope_io/utils.py
+-rw-r--r--   0        0        0      541 2024-04-09 19:35:02.649877 miniscope_io-0.1.6/miniscope_io/vendor/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 19:35:02.649945 miniscope_io-0.1.6/miniscope_io/vendor/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-09 19:35:02.650272 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/LICENSE
+-rw-r--r--   0        0        0     1657 2024-04-09 19:35:02.650484 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/README.md
+-rw-r--r--   0        0        0      777 2024-04-09 19:35:02.650689 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:35:02.650872 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/linux/__init__.py
+-rwxr-xr-x   0        0        0  1100816 2024-04-09 19:35:02.659743 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/linux/_ok.so
+-rwxr-xr-x   0        0        0  1951208 2024-04-09 19:35:02.674380 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/linux/libokFrontPanel.so
+-rw-r--r--   0        0        0    71246 2024-04-09 19:35:02.675863 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/linux/ok.py
+-rw-r--r--   0        0        0    82670 2024-04-09 19:35:02.676935 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/linux/okFrontPanel.h
+-rw-r--r--   0        0        0     1355 2024-04-09 19:35:02.677174 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/linux/okFrontPanelDLL.h
+-rw-r--r--   0        0        0        0 2024-04-09 19:35:02.677255 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/mac/__init__.py
+-rwxr-xr-x   0        0        0  1561624 2024-04-09 19:35:02.692734 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/mac/_ok.so
+-rwxr-xr-x   0        0        0  4018904 2024-04-09 19:35:02.717328 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/mac/libokFrontPanel.dylib
+-rw-r--r--   0        0        0    71246 2024-04-09 19:35:02.719476 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/mac/ok.py
+-rw-r--r--   0        0        0    82670 2024-04-09 19:35:02.720150 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/mac/okFrontPanel.h
+-rw-r--r--   0        0        0     1355 2024-04-09 19:35:02.720378 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/mac/okFrontPanelDLL.h
+-rw-r--r--   0        0        0        0 2024-04-09 19:35:02.720458 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/win/__init__.py
+-rw-r--r--   0        0        0    71247 2024-04-09 19:35:02.721062 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/win/ok.py
+-rw-r--r--   0        0        0  1892896 2024-04-09 19:35:02.730819 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/win/okFrontPanel.dll
+-rw-r--r--   0        0        0    82670 2024-04-09 19:35:02.732380 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/win/okFrontPanel.h
+-rw-r--r--   0        0        0    53290 2024-04-09 19:35:02.732982 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/win/okFrontPanel.lib
+-rw-r--r--   0        0        0     1355 2024-04-09 19:35:02.733197 miniscope_io-0.1.6/miniscope_io/vendor/opalkelly/win/okFrontPanelDLL.h
+-rw-r--r--   0        0        0       52 2023-06-24 01:08:40.857671 miniscope_io-0.1.6/miniscope_io/widgets.py
+-rw-r--r--   0        0        0     1148 2024-04-09 19:35:44.715967 miniscope_io-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 miniscope_io-0.1.6/PKG-INFO
```

### Comparing `miniscope_io-0.1.5/LICENSE` & `miniscope_io-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/miniscope_io/data.py` & `miniscope_io-0.1.6/miniscope_io/data.py`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/miniscope_io/formats.py` & `miniscope_io-0.1.6/miniscope_io/formats.py`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/miniscope_io/io.py` & `miniscope_io-0.1.6/miniscope_io/io.py`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/miniscope_io/plots/headers.py` & `miniscope_io-0.1.6/miniscope_io/plots/headers.py`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/miniscope_io/sdcard.py` & `miniscope_io-0.1.6/miniscope_io/sdcard.py`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/miniscope_io/utils.py` & `miniscope_io-0.1.6/miniscope_io/utils.py`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.5/pyproject.toml` & `miniscope_io-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniscope_io"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = [
     "sneakers-the-rat <JLSaunders987@gmail.com>",
     "t-sasatani <sasatani.dev@gmail.com>",
 ]
 readme = "README.md"
 packages = [{include = "miniscope_io"}]
@@ -17,14 +17,15 @@
 jupyter = "^1.0.0"
 matplotlib = "^3.7.1"
 pandas = "^2.1.0"
 pydantic = "^2.3.0"
 coloredlogs = "^15.0.1"
 pyserial = "^3.5"
 tqdm = "^4.66.1"
+bitstring = "^4.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
 [tool.poetry.group.tests]
 optional = true
@@ -46,9 +47,9 @@
 docs = ["sphinx", "furo", "myst-parser"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-uart_image_capture = "miniscope_io.uart_daq:main"
-updateDevice = "miniscope_io.uart_daq:updateDevice"
+stream_image_capture = "miniscope_io.stream_daq:main"
+updateDevice = "miniscope_io.stream_daq:updateDevice"
```

### Comparing `miniscope_io-0.1.5/PKG-INFO` & `miniscope_io-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: miniscope-io
-Version: 0.1.5
+Name: miniscope_io
+Version: 0.1.6
 Summary: 
 Author: sneakers-the-rat
 Author-email: JLSaunders987@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Provides-Extra: tests
+Requires-Dist: bitstring (>=4.1.2,<5.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pandas (>=2.1.0,<3.0.0)
@@ -26,7 +28,16 @@
 # miniscope-io
 
 (Demonstration project for a lab workshop on making modular, testable python code.
 Functionality not guaranteed
 -<3 jonny)
 
 
+
+## Licensing
+
+This package includes software sublicensed from more 
+restrictive licenses. Those licenses can be found
+in the `LICENSE` files in the respective directories 
+containing the unmodified source material
+
+* `miniscope_io/vendor/opalkelly`
```

