# Comparing `tmp/aranet4-2.3.1.tar.gz` & `tmp/aranet4-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aranet4-2.3.1.tar", last modified: Mon Apr  8 15:37:34 2024, max compression
+gzip compressed data, was "aranet4-2.3.2.tar", last modified: Mon Apr  8 18:55:30 2024, max compression
```

## Comparing `aranet4-2.3.1.tar` & `aranet4-2.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 15:37:34.665964 aranet4-2.3.1/
--rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.1/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-08 15:37:34.649964 aranet4-2.3.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.3.1/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 15:37:34.633964 aranet4-2.3.1/aranet4/
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-04-08 13:05:57.000000 aranet4-2.3.1/aranet4/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7886 2024-04-08 15:37:07.000000 aranet4-2.3.1/aranet4/aranetctl.py
--rw-r--r--   0 pi        (1000) pi        (1000)    35420 2024-04-08 15:30:15.000000 aranet4-2.3.1/aranet4/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 15:37:34.645964 aranet4-2.3.1/aranet4.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-04-08 15:37:34.000000 aranet4-2.3.1/aranet4.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-08 15:37:33.000000 aranet4-2.3.1/aranet4.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-08 15:37:34.665964 aranet4-2.3.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      746 2024-04-08 13:05:48.000000 aranet4-2.3.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 18:55:30.901981 aranet4-2.3.2/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.2/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-08 18:55:30.885981 aranet4-2.3.2/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.3.2/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 18:55:30.865981 aranet4-2.3.2/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-04-08 18:54:33.000000 aranet4-2.3.2/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7886 2024-04-08 18:51:58.000000 aranet4-2.3.2/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    35204 2024-04-08 18:53:22.000000 aranet4-2.3.2/aranet4/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-08 18:55:30.881981 aranet4-2.3.2/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-08 18:55:30.000000 aranet4-2.3.2/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-04-08 18:55:30.000000 aranet4-2.3.2/aranet4.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-08 18:55:30.000000 aranet4-2.3.2/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-04-08 18:55:30.000000 aranet4-2.3.2/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-04-08 18:55:30.000000 aranet4-2.3.2/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-08 18:55:30.000000 aranet4-2.3.2/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-08 18:55:30.901981 aranet4-2.3.2/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      746 2024-04-08 18:54:40.000000 aranet4-2.3.2/setup.py
```

### Comparing `aranet4-2.3.1/LICENSE` & `aranet4-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.1/PKG-INFO` & `aranet4-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.1
+Version: 2.3.2
 Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.3.1/README.md` & `aranet4-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.1/aranet4/aranetctl.py` & `aranet4-2.3.2/aranet4/aranetctl.py`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.1/aranet4/client.py` & `aranet4-2.3.2/aranet4/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,33 +381,33 @@
                 value_fmt = "<BBBB"
                 value = struct.unpack(value_fmt, raw_bytes[1:5])
                 mf_data.decode(value)
                 self.manufacturer_data = mf_data
 
                 # Extended info / measurements
                 aranetv = raw_bytes[0]
-                if len(raw_bytes) < 9:
-                    mf_data.integrations = False
-                elif aranetv == 0: # Aranet4
-                    value_fmt = "<HHHBBBHH"
-                    value = struct.unpack(value_fmt, raw_bytes[9:22])
-                    self.readings = CurrentReading()
-                    self.readings.decode(value, AranetType.ARANET4)
-                    self.readings.name = device.name
+
+                if aranetv == 0: # Aranet4
+                    value_fmt = "<xxxxxxxxxHHHBBBHH"
+                    aranetv = AranetType.ARANET4
                 elif aranetv == 1: # Aranet2
-                    value_fmt = "<HHHHBBBHHB"
-                    value = struct.unpack(value_fmt, raw_bytes[8:24])
-                    self.readings = CurrentReading()
-                    self.readings.decode(value, AranetType.ARANET2)
-                    self.readings.name = device.name
+                    value_fmt = "<xxxxxxxxHHHHBBBHHB"
+                    aranetv = AranetType.ARANET2
                 elif aranetv == 2: # Aranet Radiation
-                    value_fmt = "<IIHBBBHHB"
-                    value = struct.unpack(value_fmt, raw_bytes[6:24])
+                    value_fmt = "<xxxxxxIIHBBBHHB"
+                    aranetv = AranetType.ARANET_RADIATION
+                else:
+                    value_fmt = ""
+                    aranetv = None
+
+                end = struct.calcsize(value_fmt)
+                if end > 0 and len(raw_bytes[:end]) == end:
+                    value = struct.unpack(value_fmt, raw_bytes[:end])
                     self.readings = CurrentReading()
-                    self.readings.decode(value, AranetType.ARANET_RADIATION)
+                    self.readings.decode(value, aranetv)
                     self.readings.name = device.name
                 else:
                     mf_data.integrations = False
 
 
 @dataclass
 class RecordItem:
```

### Comparing `aranet4-2.3.1/aranet4.egg-info/PKG-INFO` & `aranet4-2.3.2/aranet4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.1
+Version: 2.3.2
 Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.3.1/setup.py` & `aranet4-2.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.3.1",
+    version="2.3.2",
     description="Aranet Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

