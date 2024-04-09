# Comparing `tmp/devicebay-0.1.0.tar.gz` & `tmp/devicebay-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.0.tar", max compression
+gzip compressed data, was "devicebay-0.1.1.tar", max compression
```

## Comparing `devicebay-0.1.0.tar` & `devicebay-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-08 22:07:37.745806 devicebay-0.1.0/LICENSE
--rw-r--r--   0        0        0       35 2024-04-08 22:10:58.296205 devicebay-0.1.0/README.md
--rw-r--r--   0        0        0      633 2024-04-08 22:12:17.535998 devicebay-0.1.0/devicebay/base.py
--rw-r--r--   0        0        0      342 2024-04-08 22:10:41.081948 devicebay-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 22:07:37.745806 devicebay-0.1.1/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-08 22:10:58.296205 devicebay-0.1.1/README.md
+-rw-r--r--   0        0        0       73 2024-04-08 22:14:30.536573 devicebay-0.1.1/devicebay/__init__.py
+-rw-r--r--   0        0        0      675 2024-04-08 22:14:06.274128 devicebay-0.1.1/devicebay/base.py
+-rw-r--r--   0        0        0      342 2024-04-08 22:14:40.826073 devicebay-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.1/PKG-INFO
```

### Comparing `devicebay-0.1.0/LICENSE` & `devicebay-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.0/devicebay/base.py` & `devicebay-0.1.1/devicebay/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import TypeVar
 
-from toolfuse import Tool
+from toolfuse import Tool, action, observation, Action, Observation
 
 D = TypeVar("D", bound="Device")
 
 
 class Device(Tool, ABC):
     """An agent device"""
```

### Comparing `devicebay-0.1.0/PKG-INFO` & `devicebay-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicebay
-Version: 0.1.0
+Version: 0.1.1
 Summary: Devices for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

