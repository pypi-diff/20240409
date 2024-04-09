# Comparing `tmp/devicebay-0.1.3.tar.gz` & `tmp/devicebay-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.3.tar", max compression
+gzip compressed data, was "devicebay-0.1.4.tar", max compression
```

## Comparing `devicebay-0.1.3.tar` & `devicebay-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.3/LICENSE
--rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.3/README.md
--rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.3/devicebay/__init__.py
--rw-r--r--   0        0        0     1147 2024-04-09 17:22:14.964987 devicebay-0.1.3/devicebay/base.py
--rw-r--r--   0        0        0      342 2024-04-09 17:22:21.916071 devicebay-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.4/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.4/README.md
+-rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.4/devicebay/__init__.py
+-rw-r--r--   0        0        0     1290 2024-04-09 17:36:09.977768 devicebay-0.1.4/devicebay/base.py
+-rw-r--r--   0        0        0      342 2024-04-09 17:36:33.922115 devicebay-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.4/PKG-INFO
```

### Comparing `devicebay-0.1.3/LICENSE` & `devicebay-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.3/devicebay/base.py` & `devicebay-0.1.4/devicebay/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from typing import Optional, TypeVar, Type, Generic
 
 from pydantic import BaseModel
 from toolfuse import Tool, action, observation, Action, Observation
 
 D = TypeVar("D", bound="Device")
 C = TypeVar("C", bound="BaseModel")
+P = TypeVar("P", bound="BaseModel")
 
 
 class ReactComponent:
     """A react component for a device"""
 
     source: str
     server_uri: str
     token: Optional[str] = None
 
 
-class Device(Generic[C, D], Tool, ABC):
+class Device(Generic[C, D, P], Tool, ABC):
     """An agent device"""
 
     @classmethod
     @abstractmethod
     def envs(cls) -> dict:
         pass
 
@@ -31,15 +32,15 @@
     @classmethod
     @abstractmethod
     def from_env(cls, config: C) -> D:
         pass
 
     @classmethod
     @abstractmethod
-    def ensure(cls, config: C) -> D:
+    def ensure(cls, name: str, config: P) -> D:
         pass
 
     @classmethod
     @abstractmethod
     def react_component(cls) -> ReactComponent:
         pass
 
@@ -49,13 +50,18 @@
 
     @classmethod
     @abstractmethod
     def config(cls) -> Type[C]:
         pass
 
     @classmethod
+    @abstractmethod
+    def provision_config(cls) -> Type[P]:
+        pass
+
+    @classmethod
     def serve(cls) -> None:
         pass
 
 
 class MultiDevice(Device):
     pass
```

### Comparing `devicebay-0.1.3/PKG-INFO` & `devicebay-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicebay
-Version: 0.1.3
+Version: 0.1.4
 Summary: Devices for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

