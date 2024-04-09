# Comparing `tmp/SMmultiio-1.1.1.tar.gz` & `tmp/SMmultiio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMmultiio-1.1.1.tar", last modified: Tue Apr  9 19:21:13 2024, max compression
+gzip compressed data, was "SMmultiio-1.2.0.tar", last modified: Tue Apr  9 19:25:00 2024, max compression
```

## Comparing `SMmultiio-1.1.1.tar` & `SMmultiio-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:21:13.141499 SMmultiio-1.1.1/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 19:21:13.141499 SMmultiio-1.1.1/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8321 2024-04-09 19:21:12.000000 SMmultiio-1.1.1/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:21:13.141499 SMmultiio-1.1.1/SMmultiio.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 19:21:13.000000 SMmultiio-1.1.1/SMmultiio.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      236 2024-04-09 19:21:13.000000 SMmultiio-1.1.1/SMmultiio.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-09 19:21:13.000000 SMmultiio-1.1.1/SMmultiio.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-09 19:21:13.000000 SMmultiio-1.1.1/SMmultiio.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        8 2024-04-09 19:21:13.000000 SMmultiio-1.1.1/SMmultiio.egg-info/top_level.txt
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:21:13.141499 SMmultiio-1.1.1/multiio/
--rwxr-xr-x   0 vlad      (1000) vlad      (1000)    20354 2024-04-09 19:20:00.000000 SMmultiio-1.1.1/multiio/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2124 2024-04-09 19:20:00.000000 SMmultiio-1.1.1/multiio/multiio_data.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-09 19:21:13.141499 SMmultiio-1.1.1/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1477 2024-04-09 19:21:00.000000 SMmultiio-1.1.1/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8351 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/SMmultiio.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      236 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        8 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/multiio/
+-rwxr-xr-x   0 vlad      (1000) vlad      (1000)    20354 2024-04-09 19:22:31.000000 SMmultiio-1.2.0/multiio/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2124 2024-04-09 19:20:00.000000 SMmultiio-1.2.0/multiio/multiio_data.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1477 2024-04-09 19:23:01.000000 SMmultiio-1.2.0/setup.py
```

### Comparing `SMmultiio-1.1.1/PKG-INFO` & `SMmultiio-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMmultiio
-Version: 1.1.1
+Version: 1.2.0
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMmultiio-1.1.1/README.md` & `SMmultiio-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # Initiate class
 
 ```console
 $ python
 Python 3.11.8 (main, Feb 12 2024, 14:50:05) [GCC 13.2.1 20230801] on linux
 Type "help", "copyright", "credits" or "license" for more information.
->>>
+>>> import multiio.SMmultiio as m
 >>> multiio = m()
 >>>
 ```
 
 # Documentation
 
 <a id="module-multiio"></a>
```

### Comparing `SMmultiio-1.1.1/SMmultiio.egg-info/PKG-INFO` & `SMmultiio-1.2.0/SMmultiio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMmultiio
-Version: 1.1.1
+Version: 1.2.0
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMmultiio-1.1.1/multiio/__init__.py` & `SMmultiio-1.2.0/multiio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
 
     def get_motor(self):
         """Get motor speed value in %.
 
         Returns:
             (float) Motor speed value in %
         """
-        return self._get_word(I2C_MEM.MOT_VAL / 10)
+        return self._get_word(I2C_MEM.MOT_VAL) / 10
     def set_motor(self, value):
         """Set motor speed value in %.
 
         Args:
             value (float): Speed value in %
         """
         if(not(-100 <= value and value <= 100)):
```

### Comparing `SMmultiio-1.1.1/multiio/multiio_data.py` & `SMmultiio-1.2.0/multiio/multiio_data.py`

 * *Files identical despite different names*

### Comparing `SMmultiio-1.1.1/setup.py` & `SMmultiio-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #with open("README.md", 'r') as f:
 #    long_description = f.read()
 
 from setuptools import setup, find_packages
 setup(
     name='SMmultiio',
     packages=find_packages(),
-    version='1.1.1',
+    version='1.2.0',
     license='MIT',
     description='Library to control Multi-IO Automation Card',
     #long_description=long_description,
     #long_description_content_type="text/markdown",
     author='Sequent Microsystems',
     author_email='olcitu@gmail.com',
     url='https://sequentmicrosystems.com',
```

