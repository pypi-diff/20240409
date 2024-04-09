# Comparing `tmp/robotframework-xlibrary-1.0.0.tar.gz` & `tmp/robotframework-xlibrary-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-1.0.0.tar", last modified: Mon Mar 18 09:36:36 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-1.0.1.tar", last modified: Tue Apr  9 08:47:22 2024, max compression
```

## Comparing `robotframework-xlibrary-1.0.0.tar` & `robotframework-xlibrary-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2024-03-18 09:26:17.000000 robotframework-xlibrary-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-03-18 09:28:41.000000 robotframework-xlibrary-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/XLibrary/
--rw-rw-rw-   0        0        0     1790 2024-03-18 09:34:23.000000 robotframework-xlibrary-1.0.0/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-1.0.0/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     1440 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.0/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 09:36:36.000000 robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1584 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-09 08:42:21.000000 robotframework-xlibrary-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/XLibrary/
+-rw-rw-rw-   0        0        0     1790 2024-03-18 09:34:23.000000 robotframework-xlibrary-1.0.1/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-1.0.1/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     1833 2024-04-09 08:45:47.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0      155 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0      312 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-1.0.1/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     1584 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 08:47:22.000000 robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-1.0.0/PKG-INFO` & `robotframework-xlibrary-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 1.0.0
+Version: 1.0.1
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,8 +21,8 @@
 XLibrary เสนอชุดของคำสั่งที่ทำให้การเขียนทดสอบสำหรับแอปพลิเคชัน Flutter โดยใช้ Robot Framework สามารถทำได้ง่ายขึ้น ไลบรารีนี้เชื่อมโยงระหว่างการทดสอบแอปพลิเคชันบนมือถือที่ถูกพัฒนาด้วย Flutter กับความสามารถทดสอบอันทรงพลังของ Robot Framework.
 
 ## การติดตั้ง
 
 เพื่อติดตั้ง XLibrary, เพียงแค่รันคำสั่งต่อไปนี้:
 
 ```bash
-pip install XLibrary
+pip install robotframework-xlibrary
```

### Comparing `robotframework-xlibrary-1.0.0/README.md` & `robotframework-xlibrary-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 XLibrary เสนอชุดของคำสั่งที่ทำให้การเขียนทดสอบสำหรับแอปพลิเคชัน Flutter โดยใช้ Robot Framework สามารถทำได้ง่ายขึ้น ไลบรารีนี้เชื่อมโยงระหว่างการทดสอบแอปพลิเคชันบนมือถือที่ถูกพัฒนาด้วย Flutter กับความสามารถทดสอบอันทรงพลังของ Robot Framework.
 
 ## การติดตั้ง
 
 เพื่อติดตั้ง XLibrary, เพียงแค่รันคำสั่งต่อไปนี้:
 
 ```bash
-pip install XLibrary
+pip install robotframework-xlibrary
```

### Comparing `robotframework-xlibrary-1.0.0/setup.py` & `robotframework-xlibrary-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="1.0.0",
+    version="1.0.1",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Test Library for robotframework-xlibrary",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-1.0.0/src/XLibrary/__init__.py` & `robotframework-xlibrary-1.0.1/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-1.0.0/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-1.0.1/src/XLibrary/submodule1/module1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #submodule1/module1.py
 # -*- coding: utf-8 -*-
 from robot.api.deco import keyword
 from .module2 import XDrint
 from robot.libraries.BuiltIn import BuiltIn
+#
+from AppiumFlutterFinder import FlutterFinder
+from AppiumFlutterLibrary import AppiumFlutterLibrary
 
 class XPrint:
 
     def __init__(self):
         self._ne=XDrint()
         self._bi = BuiltIn()
 
@@ -35,8 +38,15 @@
 
         if mode == 'FLUTTER':
             driver.switch_to.context('FLUTTER')
 
 
     def _current_application(self):
         """คืนค่าอินสแตนซ์ของแอปพลิเคชันปัจจุบัน"""
-        return self._bi.get_library_instance('AppiumFlutterLibrary')._current_application()
+        return self._bi.get_library_instance('AppiumFlutterLibrary')._current_application()
+    
+    def Chack_Button_Active(self, key):
+        """เช็คว่า Button Active หรือไม่"""
+        finder = FlutterFinder()
+        button = finder.by_value_key(key)
+        element = self.driver.find_element(button)
+        return element.is_enabled()
```

### Comparing `robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 1.0.0
+Version: 1.0.1
 Summary: Test Library for robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,8 +21,8 @@
 XLibrary เสนอชุดของคำสั่งที่ทำให้การเขียนทดสอบสำหรับแอปพลิเคชัน Flutter โดยใช้ Robot Framework สามารถทำได้ง่ายขึ้น ไลบรารีนี้เชื่อมโยงระหว่างการทดสอบแอปพลิเคชันบนมือถือที่ถูกพัฒนาด้วย Flutter กับความสามารถทดสอบอันทรงพลังของ Robot Framework.
 
 ## การติดตั้ง
 
 เพื่อติดตั้ง XLibrary, เพียงแค่รันคำสั่งต่อไปนี้:
 
 ```bash
-pip install XLibrary
+pip install robotframework-xlibrary
```

### Comparing `robotframework-xlibrary-1.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-1.0.1/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

