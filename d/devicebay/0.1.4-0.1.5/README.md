# Comparing `tmp/devicebay-0.1.4.tar.gz` & `tmp/devicebay-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.4.tar", max compression
+gzip compressed data, was "devicebay-0.1.5.tar", max compression
```

## Comparing `devicebay-0.1.4.tar` & `devicebay-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.4/LICENSE
--rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.4/README.md
--rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.4/devicebay/__init__.py
--rw-r--r--   0        0        0     1290 2024-04-09 17:36:09.977768 devicebay-0.1.4/devicebay/base.py
--rw-r--r--   0        0        0      342 2024-04-09 17:36:33.922115 devicebay-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.5/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.5/README.md
+-rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.5/devicebay/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-09 21:33:50.707870 devicebay-0.1.5/devicebay/base.py
+-rw-r--r--   0        0        0      342 2024-04-09 21:33:55.210237 devicebay-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.5/PKG-INFO
```

### Comparing `devicebay-0.1.4/LICENSE` & `devicebay-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.4/devicebay/base.py` & `devicebay-0.1.5/devicebay/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,29 +18,25 @@
 
 
 class Device(Generic[C, D, P], Tool, ABC):
     """An agent device"""
 
     @classmethod
     @abstractmethod
-    def envs(cls) -> dict:
-        pass
-
-    @abstractmethod
-    def to_env(self) -> dict:
+    def from_config(cls, config: C) -> D:
         pass
 
     @classmethod
     @abstractmethod
-    def from_env(cls, config: C) -> D:
+    def ensure(cls, name: str, config: P) -> D:
         pass
 
     @classmethod
     @abstractmethod
-    def ensure(cls, name: str, config: P) -> D:
+    def create(cls, name: str, config: P) -> D:
         pass
 
     @classmethod
     @abstractmethod
     def react_component(cls) -> ReactComponent:
         pass
```

### Comparing `devicebay-0.1.4/PKG-INFO` & `devicebay-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicebay
-Version: 0.1.4
+Version: 0.1.5
 Summary: Devices for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

