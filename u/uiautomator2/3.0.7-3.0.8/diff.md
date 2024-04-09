# Comparing `tmp/uiautomator2-3.0.7.tar.gz` & `tmp/uiautomator2-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautomator2-3.0.7.tar", max compression
+gzip compressed data, was "uiautomator2-3.0.8.tar", max compression
```

## Comparing `uiautomator2-3.0.7.tar` & `uiautomator2-3.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1064 2024-04-08 04:35:03.442009 uiautomator2-3.0.7/LICENSE
--rw-r--r--   0        0        0    53306 2024-04-08 04:35:03.442009 uiautomator2-3.0.7/README.md
--rw-r--r--   0        0        0     1036 2024-04-08 04:35:19.758088 uiautomator2-3.0.7/pyproject.toml
--rw-r--r--   0        0        0    68753 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/__init__.py
--rw-r--r--   0        0        0     8063 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/__main__.py
--rw-r--r--   0        0        0      289 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/_proto.py
--rw-r--r--   0        0        0    21287 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/_selector.py
--rw-r--r--   0        0        0      647 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/abcd.py
--rw-r--r--   0        0        0       27 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/assets/.gitignore
--rw-r--r--   0        0        0  1061950 2024-04-08 04:35:18.818083 uiautomator2-3.0.7/uiautomator2/assets/app-uiautomator-test.apk
--rw-r--r--   0        0        0  2191186 2024-04-08 04:35:18.546082 uiautomator2-3.0.7/uiautomator2/assets/app-uiautomator.apk
--rwxr-xr-x   0        0        0 10092696 2024-04-07 08:30:35.000000 uiautomator2-3.0.7/uiautomator2/assets/atx-agent
--rwxr-xr-x   0        0        0      886 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/assets/sync.sh
--rw-r--r--   0        0        0       80 2024-04-08 04:35:18.842084 uiautomator2-3.0.7/uiautomator2/assets/version.txt
--rw-r--r--   0        0        0     2602 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/__init__.py
--rw-r--r--   0        0        0      405 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/htmlreport/README.md
--rw-r--r--   0        0        0     5574 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/htmlreport/__init__.py
--rw-r--r--   0        0        0     4802 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/index.html
--rw-r--r--   0        0        0    61137 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/pig.jpg
--rw-r--r--   0        0        0     1100 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
--rw-r--r--   0        0        0       29 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/start.bat
--rw-r--r--   0        0        0     2645 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/info/__init__.py
--rw-r--r--   0        0        0    28515 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/info/conf.py
--rw-r--r--   0        0        0     2852 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/perf/README.md
--rw-r--r--   0        0        0    12384 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/perf/__init__.py
--rw-r--r--   0        0        0    41467 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext/perf/net.png
--rw-r--r--   0        0        0    26928 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/ext/perf/summary.png
--rw-r--r--   0        0        0     4180 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext-archived/aircv/README.md
--rw-r--r--   0        0        0    18456 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext-archived/aircv/__init__.py
--rw-r--r--   0        0        0      947 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext-archived/ocr/README.md
--rw-r--r--   0        0        0     2495 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext-archived/ocr/__init__.py
--rw-r--r--   0        0        0     3308 2024-04-08 04:35:03.446009 uiautomator2-3.0.7/uiautomator2/ext-archived/ocr/baiduOCR.py
--rw-r--r--   0        0        0    10476 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/image.py
--rw-r--r--   0        0        0    15094 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/init.py
--rw-r--r--   0        0        0     1801 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/messagebox.py
--rw-r--r--   0        0        0     3776 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/screenrecord.py
--rw-r--r--   0        0        0     3342 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/settings.py
--rw-r--r--   0        0        0     1762 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/swipe.py
--rw-r--r--   0        0        0     5856 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/utils.py
--rw-r--r--   0        0        0     4908 2024-04-08 04:35:19.758088 uiautomator2-3.0.7/uiautomator2/version.py
--rw-r--r--   0        0        0     9456 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/watcher.py
--rw-r--r--   0        0        0     6710 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/webview.py
--rw-r--r--   0        0        0    14389 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/widget.py
--rw-r--r--   0        0        0    23845 2024-04-08 04:35:03.450009 uiautomator2-3.0.7/uiautomator2/xpath.py
--rw-r--r--   0        0        0    54216 1970-01-01 00:00:00.000000 uiautomator2-3.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-09 14:35:00.879628 uiautomator2-3.0.8/LICENSE
+-rw-r--r--   0        0        0    53306 2024-04-09 14:35:00.883628 uiautomator2-3.0.8/README.md
+-rw-r--r--   0        0        0     1036 2024-04-09 14:35:16.503848 uiautomator2-3.0.8/pyproject.toml
+-rw-r--r--   0        0        0    68753 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/__init__.py
+-rw-r--r--   0        0        0     8063 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/__main__.py
+-rw-r--r--   0        0        0      289 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/_proto.py
+-rw-r--r--   0        0        0    21287 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/_selector.py
+-rw-r--r--   0        0        0      646 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/abcd.py
+-rw-r--r--   0        0        0       27 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/assets/.gitignore
+-rw-r--r--   0        0        0  1061950 2024-04-09 14:35:15.599835 uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator-test.apk
+-rw-r--r--   0        0        0  2191186 2024-04-09 14:35:14.835825 uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator.apk
+-rwxr-xr-x   0        0        0 10092696 2024-04-07 08:30:35.000000 uiautomator2-3.0.8/uiautomator2/assets/atx-agent
+-rwxr-xr-x   0        0        0      886 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/assets/sync.sh
+-rw-r--r--   0        0        0       80 2024-04-09 14:35:15.623836 uiautomator2-3.0.8/uiautomator2/assets/version.txt
+-rw-r--r--   0        0        0     2602 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/README.md
+-rw-r--r--   0        0        0     5574 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/__init__.py
+-rw-r--r--   0        0        0     4802 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/index.html
+-rw-r--r--   0        0        0    61137 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/pig.jpg
+-rw-r--r--   0        0        0     1100 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
+-rw-r--r--   0        0        0       29 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/start.bat
+-rw-r--r--   0        0        0     2645 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/info/__init__.py
+-rw-r--r--   0        0        0    28515 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/info/conf.py
+-rw-r--r--   0        0        0     2852 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/README.md
+-rw-r--r--   0        0        0    12384 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/__init__.py
+-rw-r--r--   0        0        0    41467 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/net.png
+-rw-r--r--   0        0        0    26928 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/ext/perf/summary.png
+-rw-r--r--   0        0        0     4180 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/README.md
+-rw-r--r--   0        0        0    18456 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/README.md
+-rw-r--r--   0        0        0     2495 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/__init__.py
+-rw-r--r--   0        0        0     3308 2024-04-09 14:35:00.887628 uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/baiduOCR.py
+-rw-r--r--   0        0        0    10476 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/image.py
+-rw-r--r--   0        0        0    15094 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/init.py
+-rw-r--r--   0        0        0     1801 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/messagebox.py
+-rw-r--r--   0        0        0     3776 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/screenrecord.py
+-rw-r--r--   0        0        0     3342 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/settings.py
+-rw-r--r--   0        0        0     1762 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/swipe.py
+-rw-r--r--   0        0        0     5856 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/utils.py
+-rw-r--r--   0        0        0     4908 2024-04-09 14:35:16.503848 uiautomator2-3.0.8/uiautomator2/version.py
+-rw-r--r--   0        0        0     9456 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/watcher.py
+-rw-r--r--   0        0        0     6710 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/webview.py
+-rw-r--r--   0        0        0    14389 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/widget.py
+-rw-r--r--   0        0        0    24156 2024-04-09 14:35:00.891628 uiautomator2-3.0.8/uiautomator2/xpath.py
+-rw-r--r--   0        0        0    54216 1970-01-01 00:00:00.000000 uiautomator2-3.0.8/PKG-INFO
```

### Comparing `uiautomator2-3.0.7/LICENSE` & `uiautomator2-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/README.md` & `uiautomator2-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/pyproject.toml` & `uiautomator2-3.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uiautomator2"
-version = "3.0.7"
+version = "3.0.8"
 description = "automator for anroid device"
 homepage = "https://github.com/openatx/uiautomator2"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["*/assets/*"]
```

### Comparing `uiautomator2-3.0.7/uiautomator2/__init__.py` & `uiautomator2-3.0.8/uiautomator2/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/__main__.py` & `uiautomator2-3.0.8/uiautomator2/__main__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/_selector.py` & `uiautomator2-3.0.8/uiautomator2/_selector.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/abcd.py` & `uiautomator2-3.0.8/uiautomator2/abcd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # abcd: Abstract Class about Device
 #
 
 import abc
 
 
-class DeviceInterface(metaclass=abc.ABCMeta):
+class AbstractDevice(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def click(self, x: int, y: int):
         pass
     
     @abc.abstractmethod
     def swipe(self, fx: int, fy: int, tx: int, ty: int, duration: float):
         """ duration is float type, indicate seconds """
```

### Comparing `uiautomator2-3.0.7/uiautomator2/assets/app-uiautomator-test.apk` & `uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator-test.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/assets/app-uiautomator.apk` & `uiautomator2-3.0.8/uiautomator2/assets/app-uiautomator.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/assets/atx-agent` & `uiautomator2-3.0.8/uiautomator2/assets/atx-agent`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/assets/sync.sh` & `uiautomator2-3.0.8/uiautomator2/assets/sync.sh`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/exceptions.py` & `uiautomator2-3.0.8/uiautomator2/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/htmlreport/__init__.py` & `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/index.html` & `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/index.html`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/pig.jpg` & `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/pig.jpg`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/htmlreport/assets/simplehttpserver.py` & `uiautomator2-3.0.8/uiautomator2/ext/htmlreport/assets/simplehttpserver.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/info/__init__.py` & `uiautomator2-3.0.8/uiautomator2/ext/info/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/info/conf.py` & `uiautomator2-3.0.8/uiautomator2/ext/info/conf.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/perf/README.md` & `uiautomator2-3.0.8/uiautomator2/ext/perf/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/perf/__init__.py` & `uiautomator2-3.0.8/uiautomator2/ext/perf/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/perf/net.png` & `uiautomator2-3.0.8/uiautomator2/ext/perf/net.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext/perf/summary.png` & `uiautomator2-3.0.8/uiautomator2/ext/perf/summary.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext-archived/aircv/README.md` & `uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext-archived/aircv/__init__.py` & `uiautomator2-3.0.8/uiautomator2/ext-archived/aircv/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext-archived/ocr/README.md` & `uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext-archived/ocr/__init__.py` & `uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/ext-archived/ocr/baiduOCR.py` & `uiautomator2-3.0.8/uiautomator2/ext-archived/ocr/baiduOCR.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/image.py` & `uiautomator2-3.0.8/uiautomator2/image.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/init.py` & `uiautomator2-3.0.8/uiautomator2/init.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/messagebox.py` & `uiautomator2-3.0.8/uiautomator2/messagebox.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/screenrecord.py` & `uiautomator2-3.0.8/uiautomator2/screenrecord.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/settings.py` & `uiautomator2-3.0.8/uiautomator2/settings.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/swipe.py` & `uiautomator2-3.0.8/uiautomator2/swipe.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/utils.py` & `uiautomator2-3.0.8/uiautomator2/utils.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/version.py` & `uiautomator2-3.0.8/uiautomator2/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 #
 
 # version managed by poetry
-__version__ = "3.0.7"
+__version__ = "3.0.8"
 
 # See ChangeLog for details
 
 __apk_version__ = '2.3.3'
 # 2.3.3 make float windows smaller
 # 2.3.2 merge pull requests # require atx-agent>=0.10.0
 # 2.3.1 support minicapagent, rotationagent, minitouchagent
```

### Comparing `uiautomator2-3.0.7/uiautomator2/watcher.py` & `uiautomator2-3.0.8/uiautomator2/watcher.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/webview.py` & `uiautomator2-3.0.8/uiautomator2/webview.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/widget.py` & `uiautomator2-3.0.8/uiautomator2/widget.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.7/uiautomator2/xpath.py` & `uiautomator2-3.0.8/uiautomator2/xpath.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from deprecated import deprecated
 from PIL import Image
 from lxml import etree
 
 from uiautomator2._proto import Direction
-from uiautomator2.abcd import DeviceInterface
+from uiautomator2.abcd import AbstractDevice
 from uiautomator2.exceptions import XPathElementNotFoundError
 from uiautomator2.utils import inject_call, swipe_in_bounds
 
 
 logger = logging.getLogger(__name__)
 
-def safe_xmlstr(s):
+def safe_xmlstr(s: str) -> str:
     return s.replace("$", "-")
 
 
-def string_quote(s):
+def string_quote(s: str) -> str:
     """quick way to quote string"""
     return "{!r}".format(s)
 
 
 def str2bytes(v: Union[str, bytes]) -> bytes:
     if isinstance(v, bytes):
         return v
@@ -42,19 +42,32 @@
     try:
         etree.XPath(xpath_expression)
         return True  # No error means the XPath syntax is likely okay
     except etree.XPathSyntaxError:
         return False  # Indicates a syntax error in the XPath expression
 
 
+def convert_to_camel_case(s: str) -> str:
+    """
+    Convert a string from kebab-case to camelCase.
+
+    :param s: A string in kebab-case format.
+    :return: A string converted to camelCase format.
+    """
+    parts = s.split('-')
+    # Convert the first letter of each part to uppercase, except for the first part
+    camel_case_str = parts[0] + ''.join(part.capitalize() for part in parts[1:])
+    return camel_case_str
+
+
 def strict_xpath(xpath: str) -> str:
     """make xpath to be computer recognized xpath"""
     orig_xpath = xpath
 
-    if xpath.startswith("/"):
+    if xpath.startswith("/") or xpath.startswith("(/"):
         pass
     elif xpath.startswith("@"):
         xpath = "//*[@resource-id={!r}]".format(xpath[1:])
     elif xpath.startswith("^"):
         xpath = "//*[re:match(@text, {0}) or re:match(@content-desc, {0}) or re:match(@resource-id, {0})]".format(
             string_quote(xpath)
         )
@@ -92,15 +105,15 @@
     pass
 
 
 class XPathError(Exception):
     """basic error for xpath plugin"""
 
 class XPath(object):
-    def __init__(self, d: DeviceInterface):
+    def __init__(self, d: AbstractDevice):
         """
         Args:
             d (uiautomator2 instance)
         """
         self._d = d
         assert hasattr(d, "wait_timeout")
         # TODO: remove wait_timeout
@@ -271,15 +284,15 @@
         """
         if direction == Direction.FORWARD:
             direction = Direction.UP
         elif direction == Direction.BACKWARD:
             direction = Direction.DOWN
         elif direction == Direction.HORIZ_FORWARD:  # Horizontal
             direction = Direction.LEFT
-        elif direction == Direction.HBACKWORD:
+        elif direction == Direction.HORIZ_BACKWARD:
             direction = Direction.RIGHT
 
         # FIXME(ssx): 还差一个检测是否到底的功能
         assert max_swipes > 0
         target = self(xpath)
         for i in range(max_swipes):
             if target.exists:
@@ -753,29 +766,22 @@
     @property
     def attrib(self):
         return self.elem.attrib
 
     @property
     def info(self) -> Dict[str, Any]:
         ret = {}
-        for key in (
-            "text",
-            "focusable",
-            "enabled",
-            "focused",
-            "scrollable",
-            "selected",
-            "clickable",
-        ):
-            ret[key] = self.attrib.get(key)
+        for k, v in dict(self.attrib).items():
+            if k in ("bounds", "class", "package", "content-desc"):
+                continue
+            ret[convert_to_camel_case(k)] = v
+
+        ret["childCount"] = len(self.elem.getchildren())
         ret["className"] = self.elem.tag
         lx, ly, rx, ry = self.bounds
         ret["bounds"] = {"left": lx, "top": ly, "right": rx, "bottom": ry}
-        ret["contentDescription"] = self.attrib.get("content-desc")
-        ret["longClickable"] = self.attrib.get("long-clickable")
+
+        # 名字命名的有点奇怪，为了兼容性暂时保留
         ret["packageName"] = self.attrib.get("package")
+        ret["contentDescription"] = self.attrib.get("content-desc")
         ret["resourceName"] = self.attrib.get("resource-id")
-        ret["resourceId"] = self.attrib.get(
-            "resource-id"
-        )  # this is better than resourceName
-        ret["childCount"] = len(self.elem.getchildren())
         return ret
```

### Comparing `uiautomator2-3.0.7/PKG-INFO` & `uiautomator2-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiautomator2
-Version: 3.0.7
+Version: 3.0.8
 Summary: automator for anroid device
 Home-page: https://github.com/openatx/uiautomator2
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

