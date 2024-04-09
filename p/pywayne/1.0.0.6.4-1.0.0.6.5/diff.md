# Comparing `tmp/pywayne-1.0.0.6.4.tar.gz` & `tmp/pywayne-1.0.0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.6.4.tar", last modified: Mon Apr  8 10:17:58 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.6.5.tar", last modified: Tue Apr  9 07:34:23 2024, max compression
```

## Comparing `pywayne-1.0.0.6.4.tar` & `pywayne-1.0.0.6.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.264108 pywayne-1.0.0.6.4/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-08 10:17:58.263984 pywayne-1.0.0.6.4/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.258602 pywayne-1.0.0.6.4/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.4/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.4/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.260578 pywayne-1.0.0.6.4/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-08 10:16:51.000000 pywayne-1.0.0.6.4/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.261608 pywayne-1.0.0.6.4/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.4/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.4/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.262125 pywayne-1.0.0.6.4/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.262741 pywayne-1.0.0.6.4/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.4/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.4/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.4/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.4/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.4/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    13551 2024-04-08 10:16:51.000000 pywayne-1.0.0.6.4/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.263229 pywayne-1.0.0.6.4/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.4/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.4/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.263684 pywayne-1.0.0.6.4/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.4/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.4/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-08 10:17:58.261254 pywayne-1.0.0.6.4/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      148 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-08 10:17:58.000000 pywayne-1.0.0.6.4/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-08 10:17:58.264156 pywayne-1.0.0.6.4/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.4/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.713084 pywayne-1.0.0.6.5/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-09 07:34:23.712931 pywayne-1.0.0.6.5/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.707154 pywayne-1.0.0.6.5/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.5/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.5/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.709272 pywayne-1.0.0.6.5/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-09 06:21:12.000000 pywayne-1.0.0.6.5/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.710364 pywayne-1.0.0.6.5/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.5/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.5/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.710776 pywayne-1.0.0.6.5/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.711366 pywayne-1.0.0.6.5/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.5/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.5/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.5/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.5/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14484 2024-04-09 07:34:04.000000 pywayne-1.0.0.6.5/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.711962 pywayne-1.0.0.6.5/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.5/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.5/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.712519 pywayne-1.0.0.6.5/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.5/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.5/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.709970 pywayne-1.0.0.6.5/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      160 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-09 07:34:23.713220 pywayne-1.0.0.6.5/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.5/setup.py
```

### Comparing `pywayne-1.0.0.6.4/LICENSE` & `pywayne-1.0.0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/PKG-INFO` & `pywayne-1.0.0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.6.4
+Version: 1.0.0.6.5
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.6.4/README.md` & `pywayne-1.0.0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/bin/gettool.py` & `pywayne-1.0.0.6.5/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.6.5/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/ahrs/tools.py` & `pywayne-1.0.0.6.5/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.6.5/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/data_structure.py` & `pywayne-1.0.0.6.5/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/dsp.py` & `pywayne-1.0.0.6.5/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/gui.py` & `pywayne-1.0.0.6.5/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/math.py` & `pywayne-1.0.0.6.5/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/plot.py` & `pywayne-1.0.0.6.5/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/tools.py` & `pywayne-1.0.0.6.5/pywayne/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -343,14 +343,39 @@
     batch_file_handler.setLevel(batch_file_level)
     batch_file_handler.setFormatter(formatter)
     logger.addHandler(batch_file_handler)
 
     return logger
 
 
+def wayne_print(text: object, color: str = "default", bold: bool = False):
+    """
+    Function to print text in color and/or bold.
+
+    Parameters:
+    - text: Text to be printed
+    - color: Text color, options include "default", "red", "green", "yellow", "blue", "magenta", "cyan", "white"
+    - bold: Boolean, if True, prints the text in bold
+    """
+    colors = {
+        "default": "\033[0m",  # Default color
+        "red": "\033[31m",  # Red
+        "green": "\033[32m",  # Green
+        "yellow": "\033[33m",  # Yellow
+        "blue": "\033[34m",  # Blue
+        "magenta": "\033[35m",  # Magenta
+        "cyan": "\033[36m",  # Cyan
+        "white": "\033[37m"  # White
+    }
+    bold_code = "\033[1m" if bold else ""
+    color_code = colors.get(color, colors["default"])
+    end_code = colors["default"]  # Reset color and style to avoid affecting subsequent prints
+    print(f"{color_code}{bold_code}{text}{end_code}")
+
+
 def write_yaml_config(config_yaml_file: str, config: dict, update=False):
     """
     Writes the given configuration dictionary to a YAML file.
 
     :param config_yaml_file: The path to the YAML file where the config should be written.
     :param config: A dictionary containing the configuration settings to write.
     :param update: If True, the function will update the existing YAML file with the new config. If False, the function will overwrite the existing YAML file with the new config.
```

### Comparing `pywayne-1.0.0.6.4/pywayne/vio/tools.py` & `pywayne-1.0.0.6.5/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.6.5/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.6.5/pywayne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.6.4
+Version: 1.0.0.6.5
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.6.4/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.6.5/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.4/setup.py` & `pywayne-1.0.0.6.5/setup.py`

 * *Files identical despite different names*

