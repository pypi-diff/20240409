# Comparing `tmp/local_tuya-2.2.1.tar.gz` & `tmp/local_tuya-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya-2.2.1.tar", max compression
+gzip compressed data, was "local_tuya-2.3.0.tar", max compression
```

## Comparing `local_tuya-2.2.1.tar` & `local_tuya-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-04-01 15:42:55.128870 local_tuya-2.2.1/LICENSE
--rw-r--r--   0        0        0     2499 2024-04-01 15:42:55.128870 local_tuya-2.2.1/README.md
--rw-r--r--   0        0        0      445 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/__init__.py
--rw-r--r--   0        0        0      939 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/backoff.py
--rw-r--r--   0        0        0     1580 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/README.md
--rw-r--r--   0        0        0      213 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/buffer.py
--rw-r--r--   0        0        0      395 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/config.py
--rw-r--r--   0        0        0     1855 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/constraints.py
--rw-r--r--   0        0        0     2268 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/device.py
--rw-r--r--   0        0        0      786 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/enums.py
--rw-r--r--   0        0        0     1288 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/device/state.py
--rw-r--r--   0        0        0      541 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/errors.py
--rw-r--r--   0        0        0     1149 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/events.py
--rw-r--r--   0        0        0      943 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/README.md
--rw-r--r--   0        0        0      167 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/config.py
--rw-r--r--   0        0        0      616 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/events.py
--rw-r--r--   0        0        0     1051 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/heartbeat.py
--rw-r--r--   0        0        0      321 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/__init__.py
--rw-r--r--   0        0        0      549 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/__init__.py
--rw-r--r--   0        0        0      827 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/crypto.py
--rw-r--r--   0        0        0      759 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/handler.py
--rw-r--r--   0        0        0     6480 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/handlers/v33.py
--rw-r--r--   0        0        0     1562 2024-04-01 15:42:55.128870 local_tuya-2.2.1/local_tuya/protocol/message/messages.py
--rw-r--r--   0        0        0     2632 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/protocol.py
--rw-r--r--   0        0        0     1711 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/receiver.py
--rw-r--r--   0        0        0     3453 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/sender.py
--rw-r--r--   0        0        0     2368 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/state.py
--rw-r--r--   0        0        0     4318 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/protocol/transport.py
--rw-r--r--   0        0        0        0 2024-04-01 15:42:55.132870 local_tuya-2.2.1/local_tuya/py.typed
--rw-r--r--   0        0        0      957 2024-04-01 15:42:55.132870 local_tuya-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 local_tuya-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-09 17:15:36.819489 local_tuya-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2499 2024-04-09 17:15:36.819489 local_tuya-2.3.0/README.md
+-rw-r--r--   0        0        0      445 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/backoff.py
+-rw-r--r--   0        0        0     1580 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/README.md
+-rw-r--r--   0        0        0      213 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/buffer.py
+-rw-r--r--   0        0        0      395 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/config.py
+-rw-r--r--   0        0        0     1855 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/constraints.py
+-rw-r--r--   0        0        0     2268 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/device.py
+-rw-r--r--   0        0        0      786 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/enums.py
+-rw-r--r--   0        0        0     1288 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/device/state.py
+-rw-r--r--   0        0        0      541 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/errors.py
+-rw-r--r--   0        0        0     1149 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/events.py
+-rw-r--r--   0        0        0      943 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/README.md
+-rw-r--r--   0        0        0      167 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/config.py
+-rw-r--r--   0        0        0      653 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/events.py
+-rw-r--r--   0        0        0     1239 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/heartbeat.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/message/__init__.py
+-rw-r--r--   0        0        0      549 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/message/handlers/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/message/handlers/crypto.py
+-rw-r--r--   0        0        0      759 2024-04-09 17:15:36.819489 local_tuya-2.3.0/local_tuya/protocol/message/handlers/handler.py
+-rw-r--r--   0        0        0     6480 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/message/handlers/v33.py
+-rw-r--r--   0        0        0     1562 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/message/messages.py
+-rw-r--r--   0        0        0     3129 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/protocol.py
+-rw-r--r--   0        0        0     1711 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/receiver.py
+-rw-r--r--   0        0        0     3453 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/sender.py
+-rw-r--r--   0        0        0     2368 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/state.py
+-rw-r--r--   0        0        0     4919 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/protocol/transport.py
+-rw-r--r--   0        0        0        0 2024-04-09 17:15:36.823489 local_tuya-2.3.0/local_tuya/py.typed
+-rw-r--r--   0        0        0      957 2024-04-09 17:15:36.823489 local_tuya-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 local_tuya-2.3.0/PKG-INFO
```

### Comparing `local_tuya-2.2.1/LICENSE` & `local_tuya-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/README.md` & `local_tuya-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/backoff.py` & `local_tuya-2.3.0/local_tuya/backoff.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/device/README.md` & `local_tuya-2.3.0/local_tuya/device/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/device/buffer.py` & `local_tuya-2.3.0/local_tuya/device/buffer.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/device/constraints.py` & `local_tuya-2.3.0/local_tuya/device/constraints.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/device/device.py` & `local_tuya-2.3.0/local_tuya/device/device.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/device/enums.py` & `local_tuya-2.3.0/local_tuya/device/enums.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/device/state.py` & `local_tuya-2.3.0/local_tuya/device/state.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/errors.py` & `local_tuya-2.3.0/local_tuya/errors.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/events.py` & `local_tuya-2.3.0/local_tuya/events.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/README.md` & `local_tuya-2.3.0/local_tuya/protocol/README.md`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/config.py` & `local_tuya-2.3.0/local_tuya/protocol/config.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/events.py` & `local_tuya-2.3.0/local_tuya/protocol/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 
 @dataclass
 class ConnectionLost(Event):
     error: Optional[Exception]
 
 
+class ConnectionBroken(Event): ...
+
+
 class DataSent(bytes, Event): ...
 
 
 class DataReceived(bytes, Event): ...
 
 
 @dataclass
```

### Comparing `local_tuya-2.2.1/local_tuya/protocol/heartbeat.py` & `local_tuya-2.3.0/local_tuya/protocol/heartbeat.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from concurrent_tasks import PeriodicTask
 
 from local_tuya.errors import CommandTimeoutError
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
     CommandSent,
+    ConnectionBroken,
     ConnectionEstablished,
     ConnectionLost,
 )
 from local_tuya.protocol.message import HeartbeatCommand
 
 logger = logging.getLogger(__name__)
 
@@ -26,7 +27,10 @@
 
 
 async def _heartbeat(event_notifier: EventNotifier) -> None:
     try:
         await event_notifier.emit(CommandSent(HeartbeatCommand()))
     except CommandTimeoutError:
         logger.warning("timeout waiting for heartbeat response")
+        # This would typically happen when connection succeeded,
+        # but it is impossible to communicate.
+        await event_notifier.emit(ConnectionBroken())
```

### Comparing `local_tuya-2.2.1/local_tuya/protocol/message/handlers/__init__.py` & `local_tuya-2.3.0/local_tuya/protocol/message/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/message/handlers/crypto.py` & `local_tuya-2.3.0/local_tuya/protocol/message/handlers/crypto.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/message/handlers/handler.py` & `local_tuya-2.3.0/local_tuya/protocol/message/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/message/handlers/v33.py` & `local_tuya-2.3.0/local_tuya/protocol/message/handlers/v33.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/message/messages.py` & `local_tuya-2.3.0/local_tuya/protocol/message/messages.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/protocol.py` & `local_tuya-2.3.0/local_tuya/protocol/protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from contextlib import AsyncExitStack
-from typing import Awaitable, Callable, Optional
+from typing import Any, Awaitable, Callable, Optional
 
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.config import ProtocolConfig
-from local_tuya.protocol.events import CommandSent, StateUpdated
+from local_tuya.protocol.events import CommandSent, ConnectionBroken, StateUpdated
 from local_tuya.protocol.heartbeat import Heartbeat
 from local_tuya.protocol.message import (
     MessageHandler,
     UpdateCommand,
     Values,
     get_handler,
 )
@@ -23,28 +23,43 @@
 ) -> Callable[[StateUpdated], Awaitable]:
     async def _wrapper(event: StateUpdated) -> None:
         await func(event.values)
 
     return _wrapper
 
 
+def _connection_broken_callback(
+    func: Callable[[], Any],
+) -> Callable[[ConnectionBroken], Any]:
+    async def _wrapper(_: ConnectionBroken) -> None:
+        await func()
+
+    return _wrapper
+
+
 class Protocol(asyncio.Protocol, AsyncExitStack):
     def __init__(
         self,
         config: ProtocolConfig,
         state_updated_callback: Optional[Callable[[Values], Awaitable]] = None,
+        connection_broken_callback: Optional[Callable[[], Any]] = None,
     ):
         super().__init__()
         self._config = config
         self._event_notifier = EventNotifier()
         if state_updated_callback:
             self._event_notifier.register(
                 StateUpdated,
                 _state_updated_callback(state_updated_callback),
             )
+        if connection_broken_callback:
+            self._event_notifier.register(
+                ConnectionBroken,
+                _connection_broken_callback(connection_broken_callback),
+            )
         message_handler: MessageHandler = get_handler(config)
         self._transport = Transport(
             address=config.address,
             port=config.port,
             backoff=config.connection_backoff,
             event_notifier=self._event_notifier,
         )
```

### Comparing `local_tuya-2.2.1/local_tuya/protocol/receiver.py` & `local_tuya-2.3.0/local_tuya/protocol/receiver.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/sender.py` & `local_tuya-2.3.0/local_tuya/protocol/sender.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/state.py` & `local_tuya-2.3.0/local_tuya/protocol/state.py`

 * *Files identical despite different names*

### Comparing `local_tuya-2.2.1/local_tuya/protocol/transport.py` & `local_tuya-2.3.0/local_tuya/protocol/transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+import re
 from typing import Optional, cast
 
 from concurrent_tasks import BackgroundTask
 
 from local_tuya.backoff import Backoff
 from local_tuya.events import EventNotifier
 from local_tuya.protocol.events import (
@@ -71,15 +72,15 @@
 
     async def _get_transport(self) -> asyncio.transports.WriteTransport:
         with self._backoff as backoff:
             while True:
                 try:
                     transport, _ = await asyncio.get_running_loop().create_connection(
                         lambda: self,
-                        self._address,
+                        await _get_host(self._address),
                         self._port,
                     )
                     return cast(asyncio.transports.WriteTransport, transport)
                 except Exception:
                     logger.warning("could not connect, retrying...", exc_info=True)
                     await backoff()
 
@@ -111,7 +112,22 @@
         if self._closed.is_set():
             raise RuntimeError("transport is closed")
         if self._closing:
             raise RuntimeError("transport is closing")
         await self._connected.wait()
         # Writing is asynchronous, errors will be raised through the `connection_lost` method.
         cast(asyncio.transports.WriteTransport, self._transport).write(data)
+
+
+async def _get_host(address: str) -> str:
+    """Resolve MAC to IP if given."""
+    if re.match(r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$", address):
+        process = await asyncio.create_subprocess_shell(
+            f"arp -n | grep -w -i '{address}' | awk '{{print $1}}'",
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+        )
+        stdout, _ = await process.communicate()
+        if not stdout:
+            raise ValueError(f"no device found for MAC {address}")
+        return stdout.decode().strip()
+    return address
```

### Comparing `local_tuya-2.2.1/pyproject.toml` & `local_tuya-2.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "local_tuya"
-version = "2.2.1"
+version = "2.3.0"
 description = "Interface to Tuya devices over LAN."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/local-tuya"
 include = ["local_tuya/py.typed"]
 
@@ -15,15 +15,15 @@
 concurrent-tasks = ">=1.6,<2"
 typing-extensions = ">=4.10"
 
 [tool.poetry.group.test.dependencies]
 pytest = "==8.1.1"
 pytest-asyncio = "==0.21.1"
 pytest-mock = "==3.14.0"
-ruff = "==0.3.4"
+ruff = "==0.3.5"
 mypy = "==1.9.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `local_tuya-2.2.1/PKG-INFO` & `local_tuya-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_tuya
-Version: 2.2.1
+Version: 2.3.0
 Summary: Interface to Tuya devices over LAN.
 Home-page: https://github.com/gpajot/local-tuya
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

