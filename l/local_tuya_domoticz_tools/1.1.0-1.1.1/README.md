# Comparing `tmp/local_tuya_domoticz_tools-1.1.0.tar.gz` & `tmp/local_tuya_domoticz_tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya_domoticz_tools-1.1.0.tar", max compression
+gzip compressed data, was "local_tuya_domoticz_tools-1.1.1.tar", max compression
```

## Comparing `local_tuya_domoticz_tools-1.1.0.tar` & `local_tuya_domoticz_tools-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/LICENSE
--rw-r--r--   0        0        0     2597 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/README.md
--rw-r--r--   0        0        0      360 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/__init__.py
--rw-r--r--   0        0        0      753 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/logger.py
--rw-r--r--   0        0        0      156 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/__init__.py
--rw-r--r--   0        0        0     1309 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/install.py
--rw-r--r--   0        0        0     5798 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/metadata.py
--rw-r--r--   0        0        0     4512 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/plugin.py
--rw-r--r--   0        0        0      843 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/template.txt
--rw-r--r--   0        0        0     1239 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/types.py
--rw-r--r--   0        0        0      621 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/__init__.py
--rw-r--r--   0        0        0     4070 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/base.py
--rw-r--r--   0        0        0      420 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/ids.py
--rw-r--r--   0        0        0     1865 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/manager.py
--rw-r--r--   0        0        0     1790 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/selector_switch.py
--rw-r--r--   0        0        0      687 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/set_point.py
--rw-r--r--   0        0        0      753 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/switch.py
--rw-r--r--   0        0        0      680 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/temperature.py
--rw-r--r--   0        0        0     1354 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/value_preprocessors.py
--rw-r--r--   0        0        0     1031 2023-03-09 17:05:07.663528 local_tuya_domoticz_tools-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 local_tuya_domoticz_tools-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3103 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/README.md
+-rw-r--r--   0        0        0      360 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/__init__.py
+-rw-r--r--   0        0        0      753 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/logger.py
+-rw-r--r--   0        0        0      156 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/__init__.py
+-rw-r--r--   0        0        0     1309 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/install.py
+-rw-r--r--   0        0        0     5798 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/metadata.py
+-rw-r--r--   0        0        0     4773 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/plugin.py
+-rw-r--r--   0        0        0      843 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/template.txt
+-rw-r--r--   0        0        0     1168 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/types.py
+-rw-r--r--   0        0        0      621 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/__init__.py
+-rw-r--r--   0        0        0     3982 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/base.py
+-rw-r--r--   0        0        0      420 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/ids.py
+-rw-r--r--   0        0        0     1865 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/manager.py
+-rw-r--r--   0        0        0     1790 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/selector_switch.py
+-rw-r--r--   0        0        0      687 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/set_point.py
+-rw-r--r--   0        0        0      753 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/switch.py
+-rw-r--r--   0        0        0      680 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/temperature.py
+-rw-r--r--   0        0        0     1354 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/value_preprocessors.py
+-rw-r--r--   0        0        0     1023 2024-04-09 18:11:25.669045 local_tuya_domoticz_tools-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 local_tuya_domoticz_tools-1.1.1/PKG-INFO
```

### Comparing `local_tuya_domoticz_tools-1.1.0/LICENSE` & `local_tuya_domoticz_tools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/README.md` & `local_tuya_domoticz_tools-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # local-tuya-domoticz-tools
+
+[![tests](https://github.com/gpajot/local-tuya-domoticz-tools/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-domoticz-tools/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/local_tuya_domoticz_tools?label=stable)](https://pypi.org/project/local_tuya_domoticz_tools/)
+[![python](https://img.shields.io/pypi/pyversions/local_tuya_domoticz_tools)](https://pypi.org/project/local_tuya_domoticz_tools/)
+
 Tools to create a Domoticz plugin for local-tuya devices.
 > 💡 The Domoticz version should be `2022.1` or higher.
 
 ## Creating the plugin
 To create a plugin, you will need to create 2 things.
 
 ### Plugin metadata
```

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/logger.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/logger.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/install.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/install.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/metadata.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/metadata.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/plugin.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from functools import partial
 from typing import Callable, Dict, Generic, Optional, Type, TypeVar
 
 from concurrent_tasks import BlockingThreadedTaskPool, ThreadedPoolContextManagerWrapper
 from local_tuya import Device, ProtocolConfig, State, Version
 
 from local_tuya_domoticz_tools.logger import DomoticzHandler
 from local_tuya_domoticz_tools.types import DomoticzDevice
@@ -68,25 +69,31 @@
         self._setup_logging(parameters.get("Mode6", "") == "1")
         DomoticzEx.Heartbeat(15)
         name = parameters["Name"]
         included_units = parameters.get("Mode5", "")
         manager: UnitManager[T] = UnitManager(
             name=name,
             units=devices[name].Units if name in devices else {},
-            included_units=self._unit_ids.included(included_units)
-            if self._unit_ids and included_units
-            else None,
+            included_units=(
+                self._unit_ids.included(included_units)
+                if self._unit_ids and included_units
+                else None
+            ),
         )
         self._manager = manager
 
         def _get_device() -> Device[T]:
             device = self._on_start(
                 self._protocol_config(parameters), parameters, manager
             )
             device.set_state_updated_callback(manager.update)
+            # start will stop first, so this will restart everything.
+            device.set_connection_broken_callback(
+                partial(self.start, parameters, devices)
+            )
             return device
 
         self._task_pool = BlockingThreadedTaskPool(
             context_manager=ThreadedPoolContextManagerWrapper(_get_device),
         )
         self._task_pool.start()
 
@@ -96,15 +103,15 @@
             self._task_pool.stop()
             self._task_pool = None
         if self._manager:
             self._manager.cleanup_domoticz_references()
             self._manager = None
 
     def on_command(self, unit_id: int, command: UnitCommand) -> None:
-        """Send an command to the device asynchronously."""
+        """Send a command to the device asynchronously."""
         if self._task_pool and self._manager:
             # Fire and forget.
             self._task_pool.create_task(
                 self._on_command(self._manager, unit_id, command)
             )
         else:
             logger.warning(
@@ -121,12 +128,12 @@
         command: UnitCommand,
     ) -> None:
         """Suppresses and logs exceptions."""
         try:
             await manager.on_command(unit_id, command)
         except Exception:
             logger.exception(
-                "error sending command %s to unit %s of plugin %s",
+                "error sending command %s to unit %d of plugin %s",
                 command,
                 unit_id,
                 self.__class__.__qualname__,
             )
```

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/plugin/template.txt` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/plugin/template.txt`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/types.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Minimal Domoticz types for static typing and mocking in tests.
 """
+
 from typing import Dict, Optional
 
 
 class DomoticzUnit:
     def __init__(
         self,
         Name: str,
@@ -16,48 +17,39 @@
     ):
         self.nValue: int = 0
         self.sValue: str = ""
         self.Color: str = ""
         self.Image: Optional[int] = 0
         self.Options: Optional[Dict[str, str]] = None
 
-    def Create(self) -> None:
-        ...
+    def Create(self) -> None: ...
 
-    def Update(self, Log: bool) -> None:
-        ...
+    def Update(self, Log: bool) -> None: ...
 
-    def Delete(self) -> None:
-        ...
+    def Delete(self) -> None: ...
 
 
 class DomoticzEx:
     @classmethod
-    def Debug(cls, s: str) -> None:
-        ...
+    def Debug(cls, s: str) -> None: ...
 
     @classmethod
-    def Log(cls, s: str) -> None:
-        ...
+    def Log(cls, s: str) -> None: ...
 
     @classmethod
-    def Status(cls, s: str) -> None:
-        ...
+    def Status(cls, s: str) -> None: ...
 
     @classmethod
-    def Error(cls, s: str) -> None:
-        ...
+    def Error(cls, s: str) -> None: ...
 
     @classmethod
-    def Heartbeat(cls, i: int) -> None:
-        ...
+    def Heartbeat(cls, i: int) -> None: ...
 
     @classmethod
-    def Debugging(cls, i: int) -> None:
-        ...
+    def Debugging(cls, i: int) -> None: ...
 
     Unit = DomoticzUnit
 
 
 class DomoticzDevice:
     Units: Dict[int, DomoticzUnit] = {}
```

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/__init__.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/__init__.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/base.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,17 +102,16 @@
                 TypeName=self._type,
                 **({"Options": self._options} if self._options else {}),
             )
             unit.Create()
         else:
             # Update some unit attributes.
             unit.Image = self._image
-            # Should be read/write but raises `AttributeError: readonly attribute`.
-            # if self._options:
-            #     unit.Options = self._options
+            if self._options:
+                unit.Options = self._options
             unit.Update(False)
         self._unit = unit
 
     async def on_command(self, command: UnitCommand) -> None:
         if self._command_to_value and self._command_func:
             value = self._command_to_value(command)
             if value is not None:
```

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/manager.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/manager.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/selector_switch.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/selector_switch.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/set_point.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/set_point.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/switch.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/switch.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/temperature.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/temperature.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/local_tuya_domoticz_tools/units/value_preprocessors.py` & `local_tuya_domoticz_tools-1.1.1/local_tuya_domoticz_tools/units/value_preprocessors.py`

 * *Files identical despite different names*

### Comparing `local_tuya_domoticz_tools-1.1.0/pyproject.toml` & `local_tuya_domoticz_tools-1.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [tool.poetry]
 name = "local_tuya_domoticz_tools"
-version = "1.1.0"
+version = "1.1.1"
 description = "Tools to create a Domoticz plugin for local-tuya devices."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/local-tuya-domoticz-tools"
 include = ["local_tuya_domoticz_tools/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
-local-tuya = ">=2.1,<3"
+local-tuya = ">=2.3.1,<3"
 concurrent-tasks = ">=1.4,<2"
 xmltodict = ">=0.13,<0.14"
 
 [tool.poetry.group.test.dependencies]
-pytest = "==7.2.2"
-pytest-asyncio = "==0.20.3"
-pytest-mock = "==3.10.0"
-ruff = "==0.0.254"
-mypy = "==1.1.1"
-black = "==23.1.0"
-pre-commit = "==3.1.1"
+pytest = "==8.1.1"
+pytest-asyncio = "==0.23.6"
+pytest-mock = "==3.14.0"
+ruff = "==0.3.5"
+mypy = "==1.9.0"
+pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 check_untyped_defs = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["A", "B", "E", "F", "I", "PT"]
 ignore = ["E501"]
-[tool.ruff.per-file-ignores]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `local_tuya_domoticz_tools-1.1.0/PKG-INFO` & `local_tuya_domoticz_tools-1.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
-Name: local-tuya-domoticz-tools
-Version: 1.1.0
+Name: local_tuya_domoticz_tools
+Version: 1.1.1
 Summary: Tools to create a Domoticz plugin for local-tuya devices.
 Home-page: https://github.com/gpajot/local-tuya-domoticz-tools
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: concurrent-tasks (>=1.4,<2)
-Requires-Dist: local-tuya (>=2.1,<3)
+Requires-Dist: local-tuya (>=2.3.1,<3)
 Requires-Dist: xmltodict (>=0.13,<0.14)
 Project-URL: Repository, https://github.com/gpajot/local-tuya-domoticz-tools
 Description-Content-Type: text/markdown
 
 # local-tuya-domoticz-tools
+
+[![tests](https://github.com/gpajot/local-tuya-domoticz-tools/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-domoticz-tools/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/local_tuya_domoticz_tools?label=stable)](https://pypi.org/project/local_tuya_domoticz_tools/)
+[![python](https://img.shields.io/pypi/pyversions/local_tuya_domoticz_tools)](https://pypi.org/project/local_tuya_domoticz_tools/)
+
 Tools to create a Domoticz plugin for local-tuya devices.
 > 💡 The Domoticz version should be `2022.1` or higher.
 
 ## Creating the plugin
 To create a plugin, you will need to create 2 things.
 
 ### Plugin metadata
```

