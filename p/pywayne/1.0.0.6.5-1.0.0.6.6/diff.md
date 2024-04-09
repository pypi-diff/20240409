# Comparing `tmp/pywayne-1.0.0.6.5.tar.gz` & `tmp/pywayne-1.0.0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.6.5.tar", last modified: Tue Apr  9 07:34:23 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.6.6.tar", last modified: Tue Apr  9 07:46:31 2024, max compression
```

## Comparing `pywayne-1.0.0.6.5.tar` & `pywayne-1.0.0.6.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.713084 pywayne-1.0.0.6.5/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-09 07:34:23.712931 pywayne-1.0.0.6.5/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.707154 pywayne-1.0.0.6.5/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.5/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.5/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.709272 pywayne-1.0.0.6.5/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-09 06:21:12.000000 pywayne-1.0.0.6.5/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.710364 pywayne-1.0.0.6.5/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.5/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.5/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.710776 pywayne-1.0.0.6.5/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.711366 pywayne-1.0.0.6.5/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.5/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.5/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.5/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.5/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.5/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    14484 2024-04-09 07:34:04.000000 pywayne-1.0.0.6.5/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.711962 pywayne-1.0.0.6.5/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.5/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.5/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.712519 pywayne-1.0.0.6.5/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.5/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.5/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:34:23.709970 pywayne-1.0.0.6.5/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1023 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      160 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-09 07:34:23.000000 pywayne-1.0.0.6.5/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-09 07:34:23.713220 pywayne-1.0.0.6.5/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.5/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.338756 pywayne-1.0.0.6.6/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1461 2024-04-09 07:46:31.338415 pywayne-1.0.0.6.6/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.332576 pywayne-1.0.0.6.6/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.6/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.6/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.334644 pywayne-1.0.0.6.6/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-09 07:46:25.000000 pywayne-1.0.0.6.6/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.335903 pywayne-1.0.0.6.6/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.6/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.6/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.336301 pywayne-1.0.0.6.6/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.336870 pywayne-1.0.0.6.6/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.6/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.6/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.6/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.6/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.6/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14484 2024-04-09 07:34:04.000000 pywayne-1.0.0.6.6/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.337363 pywayne-1.0.0.6.6/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.6/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.6/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.337831 pywayne-1.0.0.6.6/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.6/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.6/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-09 07:46:31.338134 pywayne-1.0.0.6.6/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1461 2024-04-09 07:46:31.000000 pywayne-1.0.0.6.6/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-09 07:46:31.000000 pywayne-1.0.0.6.6/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-09 07:46:31.000000 pywayne-1.0.0.6.6/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      153 2024-04-09 07:46:31.000000 pywayne-1.0.0.6.6/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-09 07:46:31.000000 pywayne-1.0.0.6.6/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-09 07:46:31.338857 pywayne-1.0.0.6.6/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.6/setup.py
```

### Comparing `pywayne-1.0.0.6.5/LICENSE` & `pywayne-1.0.0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/README.md` & `pywayne-1.0.0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/bin/gettool.py` & `pywayne-1.0.0.6.6/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.6.6/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/ahrs/tools.py` & `pywayne-1.0.0.6.6/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.6.6/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/data_structure.py` & `pywayne-1.0.0.6.6/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/dsp.py` & `pywayne-1.0.0.6.6/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/gui.py` & `pywayne-1.0.0.6.6/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/math.py` & `pywayne-1.0.0.6.6/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/plot.py` & `pywayne-1.0.0.6.6/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/tools.py` & `pywayne-1.0.0.6.6/pywayne/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/vio/tools.py` & `pywayne-1.0.0.6.6/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.6.6/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.6.6/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.5/setup.py` & `pywayne-1.0.0.6.6/setup.py`

 * *Files identical despite different names*

