# Comparing `tmp/devicebay-0.1.2.tar.gz` & `tmp/devicebay-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.2.tar", max compression
+gzip compressed data, was "devicebay-0.1.3.tar", max compression
```

## Comparing `devicebay-0.1.2.tar` & `devicebay-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.2/LICENSE
--rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.2/README.md
--rw-r--r--   0        0        0       73 2024-04-09 02:39:38.879030 devicebay-0.1.2/devicebay/__init__.py
--rw-r--r--   0        0        0     1128 2024-04-09 16:59:04.446395 devicebay-0.1.2/devicebay/base.py
--rw-r--r--   0        0        0      342 2024-04-09 16:59:10.428616 devicebay-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.3/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.3/README.md
+-rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.3/devicebay/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-09 17:22:14.964987 devicebay-0.1.3/devicebay/base.py
+-rw-r--r--   0        0        0      342 2024-04-09 17:22:21.916071 devicebay-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.3/PKG-INFO
```

### Comparing `devicebay-0.1.2/LICENSE` & `devicebay-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.2/devicebay/base.py` & `devicebay-0.1.3/devicebay/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Optional, TypeVar, Type
+from typing import Optional, TypeVar, Type, Generic
 
 from pydantic import BaseModel
 from toolfuse import Tool, action, observation, Action, Observation
 
 D = TypeVar("D", bound="Device")
 C = TypeVar("C", bound="BaseModel")
 
@@ -12,48 +12,48 @@
     """A react component for a device"""
 
     source: str
     server_uri: str
     token: Optional[str] = None
 
 
-class Device(Tool, ABC):
+class Device(Generic[C, D], Tool, ABC):
     """An agent device"""
 
     @classmethod
     @abstractmethod
     def envs(cls) -> dict:
         pass
 
     @abstractmethod
     def to_env(self) -> dict:
         pass
 
     @classmethod
     @abstractmethod
-    def from_env(cls, config: BaseModel) -> D:
+    def from_env(cls, config: C) -> D:
         pass
 
     @classmethod
     @abstractmethod
-    def ensure(cls) -> D:
+    def ensure(cls, config: C) -> D:
         pass
 
     @classmethod
     @abstractmethod
     def react_component(cls) -> ReactComponent:
         pass
 
     @abstractmethod
     def view(self, background: bool = False) -> None:
         pass
 
     @classmethod
     @abstractmethod
-    def config(cls) -> Type[BaseModel]:
+    def config(cls) -> Type[C]:
         pass
 
     @classmethod
     def serve(cls) -> None:
         pass
```

### Comparing `devicebay-0.1.2/PKG-INFO` & `devicebay-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicebay
-Version: 0.1.2
+Version: 0.1.3
 Summary: Devices for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

