# Comparing `tmp/SMmultiio-1.2.2.tar.gz` & `tmp/SMmultiio-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMmultiio-1.2.2.tar", last modified: Tue Apr  9 20:14:33 2024, max compression
+gzip compressed data, was "SMmultiio-1.2.3.tar", last modified: Tue Apr  9 20:31:25 2024, max compression
```

## Comparing `SMmultiio-1.2.2.tar` & `SMmultiio-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:14:33.958853 SMmultiio-1.2.2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 20:14:33.958853 SMmultiio-1.2.2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8351 2024-04-09 20:14:33.000000 SMmultiio-1.2.2/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:14:33.958853 SMmultiio-1.2.2/SMmultiio.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 20:14:33.000000 SMmultiio-1.2.2/SMmultiio.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      236 2024-04-09 20:14:33.000000 SMmultiio-1.2.2/SMmultiio.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-09 20:14:33.000000 SMmultiio-1.2.2/SMmultiio.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-09 20:14:33.000000 SMmultiio-1.2.2/SMmultiio.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        8 2024-04-09 20:14:33.000000 SMmultiio-1.2.2/SMmultiio.egg-info/top_level.txt
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:14:33.958853 SMmultiio-1.2.2/multiio/
--rwxr-xr-x   0 vlad      (1000) vlad      (1000)    20523 2024-04-09 20:13:56.000000 SMmultiio-1.2.2/multiio/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2124 2024-04-09 19:20:00.000000 SMmultiio-1.2.2/multiio/multiio_data.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-09 20:14:33.958853 SMmultiio-1.2.2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1477 2024-04-09 20:14:12.000000 SMmultiio-1.2.2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:31:25.436271 SMmultiio-1.2.3/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 20:31:25.436271 SMmultiio-1.2.3/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8351 2024-04-09 20:31:25.000000 SMmultiio-1.2.3/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:31:25.436271 SMmultiio-1.2.3/SMmultiio.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      801 2024-04-09 20:31:25.000000 SMmultiio-1.2.3/SMmultiio.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      236 2024-04-09 20:31:25.000000 SMmultiio-1.2.3/SMmultiio.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-09 20:31:25.000000 SMmultiio-1.2.3/SMmultiio.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-09 20:31:25.000000 SMmultiio-1.2.3/SMmultiio.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        8 2024-04-09 20:31:25.000000 SMmultiio-1.2.3/SMmultiio.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-09 20:31:25.436271 SMmultiio-1.2.3/multiio/
+-rwxr-xr-x   0 vlad      (1000) vlad      (1000)    20354 2024-04-09 20:30:38.000000 SMmultiio-1.2.3/multiio/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2124 2024-04-09 19:20:00.000000 SMmultiio-1.2.3/multiio/multiio_data.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-09 20:31:25.436271 SMmultiio-1.2.3/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1477 2024-04-09 20:30:54.000000 SMmultiio-1.2.3/setup.py
```

### Comparing `SMmultiio-1.2.2/PKG-INFO` & `SMmultiio-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMmultiio
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMmultiio-1.2.2/README.md` & `SMmultiio-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `SMmultiio-1.2.2/SMmultiio.egg-info/PKG-INFO` & `SMmultiio-1.2.3/SMmultiio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMmultiio
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMmultiio-1.2.2/multiio/__init__.py` & `SMmultiio-1.2.3/multiio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,21 +52,18 @@
     def _get_block_data(self, address, byteno=4):
         return self.bus.read_i2c_block_data(self._hw_address_, address, byteno)
     def _set_byte(self, address, value):
         self.bus.write_byte_data(self._hw_address_, address, int(value))
     def _set_word(self, address, value):
         self.bus.write_word_data(self._hw_address_, address, int(value))
     def _set_float(self, address, value):
-        ba = bytearray(struct.pack("f", float(value)))
-        self.bus.write_block_data(self._hw_address_, address, ba)
-    def _set_i16(self, address, value):
-        ba = bytearray(struct.pack("h", int(value)))
+        ba = bytearray(struct.pack("f", value))
         self.bus.write_block_data(self._hw_address_, address, ba)
     def _set_i32(self, address, value):
-        ba = bytearray(struct.pack("i", int(value)))
+        ba = bytearray(struct.pack("i", value))
         self.bus.write_block_data(self._hw_address_, address, ba)
     def _set_block(self, address, ba):
         self.bus.write_i2c_block_data(self._hw_address_, address, ba)
 
     @staticmethod
     def _check_channel(channel_type, channel):
         if not (0 <= channel and channel <= CHANNEL_NO[channel_type]):
@@ -572,15 +569,15 @@
         Args:
             channel (int): Channel number
             value (float): Servo position value in %
         """
         self._check_channel("servo", channel)
         if(not(-140 <= value and value <= 140)):
             raise ValueError("Servo value out of range! Must be [-140..140]")
-        self._set_i16(I2C_MEM.SERVO_VAL1 + (channel - 1) * 2, value * 10)
+        self._set_word(I2C_MEM.SERVO_VAL1 + (channel - 1) * 2, value * 10)
 
     def get_motor(self):
         """Get motor speed value in %.
 
         Returns:
             (float) Motor speed value in %
         """
@@ -589,15 +586,15 @@
         """Set motor speed value in %.
 
         Args:
             value (float): Speed value in %
         """
         if(not(-100 <= value and value <= 100)):
             raise ValueError("Motor value out of range! Must be [-100..100]")
-        self._set_i16(I2C_MEM.MOT_VAL, value * 10)
+        self._set_word(I2C_MEM.MOT_VAL, value * 10)
 
     def get_button(self):
         """Get button status.
 
         Returns:
             (bool) status
                 True(ON)/False(OFF)
```

### Comparing `SMmultiio-1.2.2/multiio/multiio_data.py` & `SMmultiio-1.2.3/multiio/multiio_data.py`

 * *Files identical despite different names*

### Comparing `SMmultiio-1.2.2/setup.py` & `SMmultiio-1.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #with open("README.md", 'r') as f:
 #    long_description = f.read()
 
 from setuptools import setup, find_packages
 setup(
     name='SMmultiio',
     packages=find_packages(),
-    version='1.2.2',
+    version='1.2.3',
     license='MIT',
     description='Library to control Multi-IO Automation Card',
     #long_description=long_description,
     #long_description_content_type="text/markdown",
     author='Sequent Microsystems',
     author_email='olcitu@gmail.com',
     url='https://sequentmicrosystems.com',
```

