# Comparing `tmp/inovopy-0.0.2.tar.gz` & `tmp/inovopy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inovopy-0.0.2.tar", last modified: Tue Apr  9 04:26:52 2024, max compression
+gzip compressed data, was "inovopy-0.0.3.tar", last modified: Tue Apr  9 05:25:46 2024, max compression
```

## Comparing `inovopy-0.0.2.tar` & `inovopy-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 04:26:52.081056 inovopy-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.077057 inovopy-0.0.2/inovopy/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/inovopy/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/geometry/jointcoord.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/geometry/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/inovopy/iva/
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/iva/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/inovopy/logger/
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/inovopy/robot/
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/robot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/robridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/inovopy/socket/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/socket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/socket/tcp_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/socket/tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/socket/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 04:26:35.000000 inovopy-0.0.2/inovopy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:26:52.081056 inovopy-0.0.2/inovopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 04:26:52.000000 inovopy-0.0.2/inovopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 04:26:52.000000 inovopy-0.0.2/inovopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:26:52.000000 inovopy-0.0.2/inovopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:26:52.000000 inovopy-0.0.2/inovopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 04:26:52.000000 inovopy-0.0.2/inovopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:26:52.081056 inovopy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 04:26:35.000000 inovopy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 05:25:46.424604 inovopy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 05:25:26.000000 inovopy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/geometry/jointcoord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/geometry/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy/iva/
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/iva/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy/robot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/robot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/robridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy/socket/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/socket/tcp_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/socket/tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/socket/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 05:25:26.000000 inovopy-0.0.3/inovopy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:25:46.424604 inovopy-0.0.3/inovopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 05:25:46.000000 inovopy-0.0.3/inovopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 05:25:46.000000 inovopy-0.0.3/inovopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:25:46.000000 inovopy-0.0.3/inovopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:25:46.000000 inovopy-0.0.3/inovopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 05:25:46.000000 inovopy-0.0.3/inovopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:25:46.424604 inovopy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 05:25:26.000000 inovopy-0.0.3/setup.py
```

### Comparing `inovopy-0.0.2/PKG-INFO` & `inovopy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inovopy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Inovo Robot Arm API
 Author: Alan Chung
 Author-email: deeralan827@gmail.com
 Keywords: python,robotics,inovo robotics,inovo robot arm,motion,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inovopy-0.0.2/inovopy/geometry/__init__.py` & `inovopy-0.0.3/inovopy/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/geometry/jointcoord.py` & `inovopy-0.0.3/inovopy/geometry/jointcoord.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/geometry/transform.py` & `inovopy-0.0.3/inovopy/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/iva/__init__.py` & `inovopy-0.0.3/inovopy/iva/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/logger/__init__.py` & `inovopy-0.0.3/inovopy/logger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,27 +50,26 @@
     NOLOG = 5
 
     def to_str(self) -> str:
         """
         ## Return
         `str`: a string representation of the log level
         """
-        match self:
-            case LogLevel.TRACE:
-                return "TRACE"
-            case LogLevel.DEBUG:
-                return "DEBUG"
-            case LogLevel.INFO:
-                return "INFO"
-            case LogLevel.WARN:
-                return "WARN"
-            case LogLevel.ERROR:
-                return "ERROR"
-            case _:
-                return ""
+        if self == LogLevel.TRACE:
+            return "TRACE"
+        elif self == LogLevel.DEBUG:
+            return "DEBUG"
+        elif self == LogLevel.INFO:
+            return "INFO"
+        elif self == LogLevel.WARN:
+            return "WARN"
+        elif self == LogLevel.ERROR:
+            return "ERROR"
+        else:
+            return ""
 
 class LogTarget(ABC):
     """
     # LogTarget
     This is an interface for logger to log message into
 
     ## Usage
```

### Comparing `inovopy-0.0.2/inovopy/robot/__init__.py` & `inovopy-0.0.3/inovopy/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/robridge.py` & `inovopy-0.0.3/inovopy/robridge.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/socket/__init__.py` & `inovopy-0.0.3/inovopy/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/socket/tcp_listener.py` & `inovopy-0.0.3/inovopy/socket/tcp_listener.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/socket/tcp_stream.py` & `inovopy-0.0.3/inovopy/socket/tcp_stream.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/socket/utils.py` & `inovopy-0.0.3/inovopy/socket/utils.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy/utils.py` & `inovopy-0.0.3/inovopy/utils.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.2/inovopy.egg-info/PKG-INFO` & `inovopy-0.0.3/inovopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inovopy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Inovo Robot Arm API
 Author: Alan Chung
 Author-email: deeralan827@gmail.com
 Keywords: python,robotics,inovo robotics,inovo robot arm,motion,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inovopy-0.0.2/setup.py` & `inovopy-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 setup script for inovopy
 """
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Inovo Robot Arm API'
 LONG_DESCRIPTION = \
 """
 A package that provide a simple python socket based api for controlling inovo robot arms.
 """
 
 # Setting up
```

