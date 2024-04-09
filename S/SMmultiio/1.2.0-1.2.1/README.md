# Comparing `tmp/SMmultiio-1.2.0.tar.gz` & `tmp/SMmultiio-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMmultiio-1.2.0.tar", last modified: Tue Apr  9 19:25:00 2024, max compression
+gzip compressed data, was "SMmultiio-1.2.1.tar", last modified: Tue Apr  9 20:03:35 2024, max compression
```

## Comparing `SMmultiio-1.2.0.tar` & `SMmultiio-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8351 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/SMmultiio.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      236 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        8 2024-04-09 19:25:00.000000 SMmultiio-1.2.0/SMmultiio.egg-info/top_level.txt
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/multiio/
--rwxr-xr-x   0 vlad      (1000) vlad      (1000)    20354 2024-04-09 19:22:31.000000 SMmultiio-1.2.0/multiio/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2124 2024-04-09 19:20:00.000000 SMmultiio-1.2.0/multiio/multiio_data.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-09 19:25:00.567599 SMmultiio-1.2.0/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1477 2024-04-09 19:23:01.000000 SMmultiio-1.2.0/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:03:35.640742 SMmultiio-1.2.1/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 20:03:35.640742 SMmultiio-1.2.1/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8351 2024-04-09 20:03:35.000000 SMmultiio-1.2.1/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:03:35.640742 SMmultiio-1.2.1/SMmultiio.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 20:03:35.000000 SMmultiio-1.2.1/SMmultiio.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      236 2024-04-09 20:03:35.000000 SMmultiio-1.2.1/SMmultiio.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-09 20:03:35.000000 SMmultiio-1.2.1/SMmultiio.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-09 20:03:35.000000 SMmultiio-1.2.1/SMmultiio.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        8 2024-04-09 20:03:35.000000 SMmultiio-1.2.1/SMmultiio.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:03:35.640742 SMmultiio-1.2.1/multiio/
+-rwxr-xr-x   0 vlad      (1000) vlad      (1000)    20506 2024-04-09 20:02:06.000000 SMmultiio-1.2.1/multiio/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2124 2024-04-09 19:20:00.000000 SMmultiio-1.2.1/multiio/multiio_data.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-09 20:03:35.640742 SMmultiio-1.2.1/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1477 2024-04-09 20:03:28.000000 SMmultiio-1.2.1/setup.py
```

### Comparing `SMmultiio-1.2.0/PKG-INFO` & `SMmultiio-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMmultiio
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMmultiio-1.2.0/README.md` & `SMmultiio-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SMmultiio-1.2.0/SMmultiio.egg-info/PKG-INFO` & `SMmultiio-1.2.1/SMmultiio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMmultiio
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMmultiio-1.2.0/multiio/__init__.py` & `SMmultiio-1.2.1/multiio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     def _set_byte(self, address, value):
         self.bus.write_byte_data(self._hw_address_, address, int(value))
     def _set_word(self, address, value):
         self.bus.write_word_data(self._hw_address_, address, int(value))
     def _set_float(self, address, value):
         ba = bytearray(struct.pack("f", value))
         self.bus.write_block_data(self._hw_address_, address, ba)
+    def _set_i16(self, address, value):
+        ba = bytearray(struct.pack("h", value))
+        self.bus.write_block_data(self._hw_address_, address, ba)
     def _set_i32(self, address, value):
         ba = bytearray(struct.pack("i", value))
         self.bus.write_block_data(self._hw_address_, address, ba)
     def _set_block(self, address, ba):
         self.bus.write_i2c_block_data(self._hw_address_, address, ba)
 
     @staticmethod
@@ -569,15 +572,15 @@
         Args:
             channel (int): Channel number
             value (float): Servo position value in %
         """
         self._check_channel("servo", channel)
         if(not(-140 <= value and value <= 140)):
             raise ValueError("Servo value out of range! Must be [-140..140]")
-        self._set_word(I2C_MEM.SERVO_VAL1 + (channel - 1) * 2, value * 10)
+        self._set_i16(I2C_MEM.SERVO_VAL1 + (channel - 1) * 2, value * 10)
 
     def get_motor(self):
         """Get motor speed value in %.
 
         Returns:
             (float) Motor speed value in %
         """
@@ -586,15 +589,15 @@
         """Set motor speed value in %.
 
         Args:
             value (float): Speed value in %
         """
         if(not(-100 <= value and value <= 100)):
             raise ValueError("Motor value out of range! Must be [-100..100]")
-        self._set_word(I2C_MEM.MOT_VAL, value * 10)
+        self._set_i16(I2C_MEM.MOT_VAL, value * 10)
 
     def get_button(self):
         """Get button status.
 
         Returns:
             (bool) status
                 True(ON)/False(OFF)
```

### Comparing `SMmultiio-1.2.0/multiio/multiio_data.py` & `SMmultiio-1.2.1/multiio/multiio_data.py`

 * *Files identical despite different names*

### Comparing `SMmultiio-1.2.0/setup.py` & `SMmultiio-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #with open("README.md", 'r') as f:
 #    long_description = f.read()
 
 from setuptools import setup, find_packages
 setup(
     name='SMmultiio',
     packages=find_packages(),
-    version='1.2.0',
+    version='1.2.1',
     license='MIT',
     description='Library to control Multi-IO Automation Card',
     #long_description=long_description,
     #long_description_content_type="text/markdown",
     author='Sequent Microsystems',
     author_email='olcitu@gmail.com',
     url='https://sequentmicrosystems.com',
```

