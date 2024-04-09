# Comparing `tmp/rtisdev-2.12.3.tar.gz` & `tmp/rtisdev-2.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\woute\Projects\rtisdev\dist\.tmp-oy2ti1gx\rtisdev-2.12.3.tar", last modified: Fri Apr  5 08:51:35 2024, max compression
+gzip compressed data, was "C:\Users\woute\Projects\rtisdev\dist\.tmp-y9knme4e\rtisdev-2.13.0.tar", last modified: Tue Apr  9 07:01:55 2024, max compression
```

## Comparing `rtisdev-2.12.3.tar` & `rtisdev-2.13.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/
--rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdev-2.12.3/LICENSE
--rw-rw-rw-   0        0        0       52 2024-04-05 08:40:05.000000 rtisdev-2.12.3/MANIFEST.in
--rw-rw-rw-   0        0        0    34213 2024-04-05 08:51:35.000000 rtisdev-2.12.3/PKG-INFO
--rw-rw-rw-   0        0        0     8123 2024-04-05 08:00:27.000000 rtisdev-2.12.3/README.md
--rw-rw-rw-   0        0        0     1832 2024-04-05 08:51:25.000000 rtisdev-2.12.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/
--rw-rw-rw-   0        0        0   223482 2024-04-05 08:18:48.000000 rtisdev-2.12.3/rtisdev/RTISDev.py
--rw-rw-rw-   0        0        0    11893 2024-04-05 08:18:48.000000 rtisdev-2.12.3/rtisdev/RTISGenerateSettings.py
--rw-rw-rw-   0        0        0     4457 2024-03-28 14:10:26.000000 rtisdev-2.12.3/rtisdev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v2/
--rw-rw-rw-   0        0        0      700 2023-03-24 10:15:41.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v2REC/
--rw-rw-rw-   0        0        0      281 2023-04-27 11:51:07.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v3D1/
--rw-rw-rw-   0        0        0      699 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/
--rw-rw-rw-   0        0        0      266 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/uRTIS_v1/
--rw-rw-rw-   0        0        0      259 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/uRTIS_v1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/xRTIS_v1/
--rw-rw-rw-   0        0        0      318 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/microphoneLayouts/xRTIS_v1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/
--rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/2D_5m_181.json
--rw-rw-rw-   0        0        0      114 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/2D_5m_91.json
--rw-rw-rw-   0        0        0      117 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/3D_10m_3000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/3D_5m_1000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/3D_5m_3000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/3D_5m_4000.json
--rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/3D_5m_500.json
--rw-rw-rw-   0        0        0      182 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/custom_example_2D_5m_91.json
--rw-rw-rw-   0        0        0     8056 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/delaymatrix.csv
--rw-rw-rw-   0        0        0     1992 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/directions.csv
--rw-rw-rw-   0        0        0     8277 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/ranges.csv
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/default_20_80.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/default_25_50.json
--rw-rw-rw-   0        0        0    29236 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/flutter.csv
--rw-rw-rw-   0        0        0      180 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/flutter.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/long_20_80.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/long_25_50.json
--rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/short_20_80.json
--rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/short_25_50.json
--rw-rw-rw-   0        0        0   655360 2023-03-22 13:54:21.000000 rtisdev-2.12.3/rtisdev/simulate.bin
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev.egg-info/
--rw-rw-rw-   0        0        0    34213 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3486 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-05 08:51:35.000000 rtisdev-2.12.3/rtisdev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 08:51:35.000000 rtisdev-2.12.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 08:51:35.000000 rtisdev-2.12.3/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:54:21.000000 rtisdev-2.12.3/tests/__init__.py
--rw-rw-rw-   0        0        0    22523 2024-04-05 08:26:25.000000 rtisdev-2.12.3/tests/test_rtisdev.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/
+-rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdev-2.13.0/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-04-05 08:40:05.000000 rtisdev-2.13.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    34213 2024-04-09 07:01:55.000000 rtisdev-2.13.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8123 2024-04-05 08:00:27.000000 rtisdev-2.13.0/README.md
+-rw-rw-rw-   0        0        0     1832 2024-04-09 07:00:17.000000 rtisdev-2.13.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/
+-rw-rw-rw-   0        0        0     7881 2024-04-05 08:47:07.000000 rtisdev-2.13.0/rtisdev/GenerateWiki.py
+-rw-rw-rw-   0        0        0   223482 2024-04-09 07:00:17.000000 rtisdev-2.13.0/rtisdev/RTISDev.py
+-rw-rw-rw-   0        0        0    11893 2024-04-05 08:18:48.000000 rtisdev-2.13.0/rtisdev/RTISGenerateSettings.py
+-rw-rw-rw-   0        0        0     4457 2024-04-09 07:00:17.000000 rtisdev-2.13.0/rtisdev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2/
+-rw-rw-rw-   0        0        0      700 2023-03-24 10:15:41.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/
+-rw-rw-rw-   0        0        0      281 2023-04-27 11:51:07.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/
+-rw-rw-rw-   0        0        0      699 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/
+-rw-rw-rw-   0        0        0      266 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/uRTIS_v1/
+-rw-rw-rw-   0        0        0      259 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/uRTIS_v1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/xRTIS_v1/
+-rw-rw-rw-   0        0        0      318 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/xRTIS_v1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/
+-rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/2D_5m_181.json
+-rw-rw-rw-   0        0        0      114 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/2D_5m_91.json
+-rw-rw-rw-   0        0        0      117 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_10m_3000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_1000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_3000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_4000.json
+-rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_500.json
+-rw-rw-rw-   0        0        0      182 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/custom_example_2D_5m_91.json
+-rw-rw-rw-   0        0        0     8056 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv
+-rw-rw-rw-   0        0        0     1992 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/directions.csv
+-rw-rw-rw-   0        0        0     8277 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/ranges.csv
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/default_20_80.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/default_25_50.json
+-rw-rw-rw-   0        0        0    29236 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/flutter.csv
+-rw-rw-rw-   0        0        0      180 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/flutter.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/long_20_80.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/long_25_50.json
+-rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/short_20_80.json
+-rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/short_25_50.json
+-rw-rw-rw-   0        0        0   655360 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/simulate.bin
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev.egg-info/
+-rw-rw-rw-   0        0        0    34213 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3536 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 07:01:55.000000 rtisdev-2.13.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:54:21.000000 rtisdev-2.13.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    22523 2024-04-05 08:26:25.000000 rtisdev-2.13.0/tests/test_rtisdev.py
```

### Comparing `rtisdev-2.12.3/LICENSE` & `rtisdev-2.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/PKG-INFO` & `rtisdev-2.13.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdev
-Version: 2.12.3
+Version: 2.13.0
 Summary: Python module to make it easy to code with RTIS devices
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>, Arne Aerts <arne.aerts@uantwerpen.be>, Dennis Laurijssen <dennis.laurijssen@uantwerpen.be>, Jan Steckel <jan.steckel@uantwerpen.be>
 Maintainer-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `rtisdev-2.12.3/README.md` & `rtisdev-2.13.0/README.md`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/pyproject.toml` & `rtisdev-2.13.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rtisdev"
-version = "2.12.3"
+version = "2.13.0"
 description = "Python module to make it easy to code with RTIS devices"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be" },
            { name = "Arne Aerts", email = "arne.aerts@uantwerpen.be"},
            { name = "Dennis Laurijssen", email = "dennis.laurijssen@uantwerpen.be"},
            { name = "Jan Steckel", email = "jan.steckel@uantwerpen.be"}]
 maintainers = [{name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be"}]
```

### Comparing `rtisdev-2.12.3/rtisdev/RTISDev.py` & `rtisdev-2.13.0/rtisdev/RTISDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 SETTINGS = {}
 WORKERS = []
 CUDA_USED = False
 PACKAGE_DIRECTORY = os.path.dirname(os.path.abspath(__file__))
 BEHAVIOUR = False
 AMPLIFIER_ACTIVE = False
 DEBUG_COUNTER = 0
-VERSION = "v2.11.0"
+VERSION = "v2.13.0"
 CURRENT_RECORDING_CONFIG = ""
 
 
 class CustomFormatter(logging.Formatter):
     grey = "\x1b[38m"
     green = "\x1b[32m"
     yellow = "\x1b[33m"
```

### Comparing `rtisdev-2.12.3/rtisdev/RTISGenerateSettings.py` & `rtisdev-2.13.0/rtisdev/RTISGenerateSettings.py`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/__init__.py` & `rtisdev-2.13.0/rtisdev/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,8 @@
     ...             axs[microphone_index_i, microphone_index_j].set_xlabel("Time (Samples)")
     ...         if microphone_index_j == 0:
     ...             axs[microphone_index_i, microphone_index_j].set_ylabel("Amplitude")
     >>> plt.show()
     >>> fig.suptitle("RTIS Dev - Microphone Signals")
 """
 from .RTISDev import *
-__version__ = "2.11.0"
+__version__ = "2.13.0"
```

### Comparing `rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat` & `rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat` & `rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/delaymatrix.csv` & `rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/directions.csv` & `rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/directions.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/config/premadeSettings/processing/ranges.csv` & `rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/ranges.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/config/premadeSettings/recording/flutter.csv` & `rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/flutter.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev/simulate.bin` & `rtisdev-2.13.0/rtisdev/simulate.bin`

 * *Files identical despite different names*

### Comparing `rtisdev-2.12.3/rtisdev.egg-info/PKG-INFO` & `rtisdev-2.13.0/rtisdev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdev
-Version: 2.12.3
+Version: 2.13.0
 Summary: Python module to make it easy to code with RTIS devices
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>, Arne Aerts <arne.aerts@uantwerpen.be>, Dennis Laurijssen <dennis.laurijssen@uantwerpen.be>, Jan Steckel <jan.steckel@uantwerpen.be>
 Maintainer-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `rtisdev-2.12.3/rtisdev.egg-info/SOURCES.txt` & `rtisdev-2.13.0/rtisdev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+./rtisdev/GenerateWiki.py
 ./rtisdev/RTISDev.py
 ./rtisdev/RTISGenerateSettings.py
 ./rtisdev/__init__.py
 ./rtisdev/simulate.bin
 ./rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
 ./rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
 ./rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
@@ -29,14 +30,15 @@
 ./rtisdev/config/premadeSettings/recording/flutter.json
 ./rtisdev/config/premadeSettings/recording/long_20_80.json
 ./rtisdev/config/premadeSettings/recording/long_25_50.json
 ./rtisdev/config/premadeSettings/recording/short_20_80.json
 ./rtisdev/config/premadeSettings/recording/short_25_50.json
 ./tests/__init__.py
 ./tests/test_rtisdev.py
+rtisdev/GenerateWiki.py
 rtisdev/RTISDev.py
 rtisdev/RTISGenerateSettings.py
 rtisdev/__init__.py
 rtisdev/simulate.bin
 rtisdev.egg-info/PKG-INFO
 rtisdev.egg-info/SOURCES.txt
 rtisdev.egg-info/dependency_links.txt
```

### Comparing `rtisdev-2.12.3/tests/test_rtisdev.py` & `rtisdev-2.13.0/tests/test_rtisdev.py`

 * *Files identical despite different names*

