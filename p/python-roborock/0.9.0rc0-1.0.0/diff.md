# Comparing `tmp/python_roborock-0.9.0rc0.tar.gz` & `tmp/python_roborock-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.9.0rc0.tar", max compression
+gzip compressed data, was "python_roborock-1.0.0.tar", max compression
```

## Comparing `python_roborock-0.9.0rc0.tar` & `python_roborock-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-02-15 23:23:41.026106 python_roborock-0.9.0rc0/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-17 23:50:22.944797 python_roborock-0.9.0rc0/README.md
--rw-r--r--   0        0        0     1373 2023-04-29 00:38:52.377261 python_roborock-0.9.0rc0/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-17 23:50:22.945724 python_roborock-0.9.0rc0/roborock/__init__.py
--rw-r--r--   0        0        0    20953 2023-04-29 00:19:12.443894 python_roborock-0.9.0rc0/roborock/api.py
--rw-r--r--   0        0        0     4102 2023-04-29 00:14:20.401256 python_roborock-0.9.0rc0/roborock/cli.py
--rw-r--r--   0        0        0     7261 2023-04-29 00:18:57.528713 python_roborock-0.9.0rc0/roborock/cloud_api.py
--rw-r--r--   0        0        0     4620 2023-04-29 00:15:07.502108 python_roborock-0.9.0rc0/roborock/code_mappings.py
--rw-r--r--   0        0        0      209 2023-04-27 14:49:49.843263 python_roborock-0.9.0rc0/roborock/const.py
--rw-r--r--   0        0        0    10730 2023-04-27 14:49:49.843775 python_roborock-0.9.0rc0/roborock/containers.py
--rw-r--r--   0        0        0     1483 2023-04-27 14:49:49.930465 python_roborock-0.9.0rc0/roborock/exceptions.py
--rw-r--r--   0        0        0     5635 2023-04-29 00:24:11.618489 python_roborock-0.9.0rc0/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-22 02:10:16.435351 python_roborock-0.9.0rc0/roborock/roborock_future.py
--rw-r--r--   0        0        0     6358 2023-04-29 00:14:58.499142 python_roborock-0.9.0rc0/roborock/roborock_message.py
--rw-r--r--   0        0        0     4626 2023-04-29 00:06:49.142059 python_roborock-0.9.0rc0/roborock/test.py
--rw-r--r--   0        0        0    18391 2023-04-29 00:18:15.411897 python_roborock-0.9.0rc0/roborock/typing.py
--rw-r--r--   0        0        0      783 2023-04-25 18:03:12.110531 python_roborock-0.9.0rc0/roborock/util.py
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 python_roborock-0.9.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 15:49:07.233429 python_roborock-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1220 2024-04-09 15:49:07.233429 python_roborock-1.0.0/README.md
+-rw-r--r--   0        0        0     1677 2024-04-09 15:49:08.057433 python_roborock-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/__init__.py
+-rw-r--r--   0        0        0     4392 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/api.py
+-rw-r--r--   0        0        0     6826 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/cli.py
+-rw-r--r--   0        0        0     7144 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/cloud_api.py
+-rw-r--r--   0        0        0    11343 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/code_mappings.py
+-rw-r--r--   0        0        0     7912 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/command_cache.py
+-rw-r--r--   0        0        0     2339 2024-04-09 15:49:07.233429 python_roborock-1.0.0/roborock/const.py
+-rw-r--r--   0        0        0    27590 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/containers.py
+-rw-r--r--   0        0        0     1962 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/exceptions.py
+-rw-r--r--   0        0        0     4367 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/local_api.py
+-rw-r--r--   0        0        0    12331 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/protocol.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/py.typed
+-rw-r--r--   0        0        0      834 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     4381 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/roborock_message.py
+-rw-r--r--   0        0        0    21816 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/roborock_typing.py
+-rw-r--r--   0        0        0     3465 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/util.py
+-rw-r--r--   0        0        0      183 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/__init__.py
+-rw-r--r--   0        0        0    19949 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/roborock_client_v1.py
+-rw-r--r--   0        0        0     3477 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/roborock_local_client_v1.py
+-rw-r--r--   0        0        0     3342 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
+-rw-r--r--   0        0        0      111 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_a01_apis/__init__.py
+-rw-r--r--   0        0        0     5046 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_a01_apis/roborock_client_a01.py
+-rw-r--r--   0        0        0     2482 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
+-rw-r--r--   0        0        0    13040 2024-04-09 15:49:07.237429 python_roborock-1.0.0/roborock/web_api.py
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-1.0.0/PKG-INFO
```

### Comparing `python_roborock-0.9.0rc0/LICENSE` & `python_roborock-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0rc0/pyproject.toml` & `python_roborock-1.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.9.0-rc"
+version = "1.0.0"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
+documentation = "https://python-roborock.readthedocs.io/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{include = "roborock"}]
+keywords = ["roborock", "vacuum", "homeassistant"]
 
 [tool.poetry.scripts]
 roborock = "roborock.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 click = ">=8"
-aiohttp = "*"
+aiohttp = "^3.8.2"
 async-timeout = "*"
-pycryptodome = "~3.17.0"
-pycryptodomex = {version = "~3.17.0", markers = "sys_platform == 'darwin'"}
-paho-mqtt = "~1.6.1"
-dacite = "~1.8.0"
+pycryptodome = "^3.18"
+pycryptodomex = {version = "^3.18", markers = "sys_platform == 'darwin'"}
+paho-mqtt = "^1.6.1"
+dacite = "^1.8.0"
+construct = "^2.10.57"
 
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core==1.8.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest-asyncio = "*"
 pytest = "*"
-pre-commit = "*"
+pre-commit = "^3.5.0"
 mypy = "*"
 ruff = "*"
-isort = "*"
-black = "*"
 codespell = "*"
+pyshark = "^0.6"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 build_command = "pip install poetry && poetry build"
+[tool.semantic_release.commit_parser_options]
+allowed_tags = [
+    "chore",
+    "docs",
+    "feat",
+    "fix",
+    "refactor"
+]
+major_tags= ["refactor"]
 
 [tool.ruff]
 ignore = ["F403", "E741"]
 line-length = 120
+select=["E", "F", "UP", "I"]
 
-[tool.black]
-line-length = 120
-
-[tool.isort]
-profile = "black"
-line_length = 120
+[tool.ruff.lint.per-file-ignores]
+"*/__init__.py" = ["F401"]
```

### Comparing `python_roborock-0.9.0rc0/roborock/api.py` & `python_roborock-1.0.0/roborock/version_1_apis/roborock_client_v1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,531 +1,469 @@
-"""The Roborock api."""
-
-from __future__ import annotations
-
 import asyncio
-import base64
-import gzip
-import hashlib
-import hmac
+import dataclasses
 import json
-import logging
 import math
-import secrets
 import struct
 import time
+from collections.abc import Callable, Coroutine
 from random import randint
-from typing import Any, Callable, Coroutine, Optional
-
-import aiohttp
-from Crypto.Cipher import AES
-from Crypto.Util.Padding import unpad
+from typing import Any, TypeVar, final
 
-from .code_mappings import RoborockDockTypeCode, RoborockEnum
-from .containers import (
+from roborock import (
+    DeviceProp,
+    DockSummary,
+    RoborockCommand,
+    RoborockDockTypeCode,
+    RoborockException,
+    UnknownMethodError,
+    VacuumError,
+)
+from roborock.api import RoborockClient
+from roborock.command_cache import (
+    CacheableAttribute,
+    CommandType,
+    RoborockAttribute,
+    find_cacheable_attribute,
+    get_cache_map,
+)
+from roborock.containers import (
+    ChildLockStatus,
     CleanRecord,
     CleanSummary,
     Consumable,
-    DNDTimer,
+    DeviceData,
+    DnDTimer,
     DustCollectionMode,
-    HomeData,
+    FlowLedStatus,
+    ModelStatus,
     MultiMapsList,
     NetworkInfo,
-    RoborockDeviceInfo,
+    RoborockBase,
     RoomMapping,
+    S7MaxVStatus,
+    ServerTimer,
     SmartWashParams,
     Status,
-    UserData,
+    ValleyElectricityTimer,
     WashTowelMode,
 )
-from .exceptions import (
-    RoborockAccountDoesNotExist,
-    RoborockException,
-    RoborockInvalidCode,
-    RoborockInvalidEmail,
-    RoborockTimeout,
-    RoborockUrlException,
-    VacuumError,
+from roborock.protocol import Utils
+from roborock.roborock_message import (
+    ROBOROCK_DATA_CONSUMABLE_PROTOCOL,
+    ROBOROCK_DATA_STATUS_PROTOCOL,
+    RoborockDataProtocol,
+    RoborockMessage,
+    RoborockMessageProtocol,
 )
-from .roborock_future import RoborockFuture
-from .roborock_message import RoborockMessage
-from .typing import DeviceProp, DockSummary, RoborockCommand
-from .util import unpack_list
-
-_LOGGER = logging.getLogger(__name__)
-KEEPALIVE = 60
-QUEUE_TIMEOUT = 4
-SPECIAL_COMMANDS = [
+from roborock.util import RepeatableTask, unpack_list
+
+COMMANDS_SECURED = [
     RoborockCommand.GET_MAP_V1,
+    RoborockCommand.GET_MULTI_MAP,
 ]
 
+WASH_N_FILL_DOCK = [
+    RoborockDockTypeCode.empty_wash_fill_dock,
+    RoborockDockTypeCode.s8_dock,
+    RoborockDockTypeCode.p10_dock,
+]
+RT = TypeVar("RT", bound=RoborockBase)
+EVICT_TIME = 60
 
-def md5hex(message: str) -> str:
-    md5 = hashlib.md5()
-    md5.update(message.encode())
-    return md5.hexdigest()
-
-
-class PreparedRequest:
-    def __init__(self, base_url: str, base_headers: Optional[dict] = None) -> None:
-        self.base_url = base_url
-        self.base_headers = base_headers or {}
-
-    async def request(self, method: str, url: str, params=None, data=None, headers=None) -> dict:
-        _url = "/".join(s.strip("/") for s in [self.base_url, url])
-        _headers = {**self.base_headers, **(headers or {})}
-        async with aiohttp.ClientSession() as session:
-            async with session.request(
-                method,
-                _url,
-                params=params,
-                data=data,
-                headers=_headers,
-            ) as resp:
-                return await resp.json()
-
-
-class RoborockClient:
-    def __init__(self, endpoint: str, device_info: RoborockDeviceInfo) -> None:
-        self.device_info = device_info
-        self._endpoint = endpoint
-        self._nonce = secrets.token_bytes(16)
-        self._waiting_queue: dict[int, RoborockFuture] = {}
-        self._last_device_msg_in = self.time_func()
-        self._last_disconnection = self.time_func()
-        self.keep_alive = KEEPALIVE
 
-    def __del__(self) -> None:
-        self.sync_disconnect()
+class AttributeCache:
+    def __init__(self, attribute: RoborockAttribute, api: RoborockClient):
+        self.attribute = attribute
+        self.api = api
+        self.attribute = attribute
+        self.task = RepeatableTask(self.api.event_loop, self._async_value, EVICT_TIME)
+        self._value: Any = None
+        self._mutex = asyncio.Lock()
+        self.unsupported: bool = False
 
     @property
-    def time_func(self) -> Callable[[], float]:
-        try:
-            # Use monotonic clock if available
-            time_func = time.monotonic
-        except AttributeError:
-            time_func = time.time
-        return time_func
+    def value(self):
+        return self._value
 
-    async def async_connect(self):
-        raise NotImplementedError
-
-    def sync_disconnect(self) -> Any:
-        raise NotImplementedError
-
-    async def async_disconnect(self) -> Any:
-        raise NotImplementedError
-
-    def on_message_received(self, messages: list[RoborockMessage]) -> None:
-        try:
-            self._last_device_msg_in = self.time_func()
-            for data in messages:
-                protocol = data.protocol
-                if protocol == 102 or protocol == 4:
-                    payload = json.loads(data.payload.decode())
-                    for data_point_number, data_point in payload.get("dps").items():
-                        if data_point_number == "102":
-                            data_point_response = json.loads(data_point)
-                            request_id = data_point_response.get("id")
-                            queue = self._waiting_queue.get(request_id)
-                            if queue and queue.protocol == protocol:
-                                error = data_point_response.get("error")
-                                if error:
-                                    queue.resolve(
-                                        (
-                                            None,
-                                            VacuumError(
-                                                error.get("code"),
-                                                error.get("message"),
-                                            ),
-                                        )
-                                    )
-                                else:
-                                    result = data_point_response.get("result")
-                                    if isinstance(result, list) and len(result) == 1:
-                                        result = result[0]
-                                    queue.resolve((result, None))
-                elif protocol == 301:
-                    payload = data.payload[0:24]
-                    [endpoint, _, request_id, _] = struct.unpack("<15sBH6s", payload)
-                    if endpoint.decode().startswith(self._endpoint):
-                        iv = bytes(AES.block_size)
-                        decipher = AES.new(self._nonce, AES.MODE_CBC, iv)
-                        decrypted = unpad(decipher.decrypt(data.payload[24:]), AES.block_size)
-                        decrypted = gzip.decompress(decrypted)
-                        queue = self._waiting_queue.get(request_id)
-                        if queue:
-                            if isinstance(decrypted, list):
-                                decrypted = decrypted[0]
-                            queue.resolve((decrypted, None))
-                else:
-                    queue = self._waiting_queue.get(data.seq)
-                    if queue:
-                        queue.resolve((data.payload, None))
-        except Exception as ex:
-            _LOGGER.exception(ex)
-
-    def on_connection_lost(self, exc: Optional[Exception]) -> None:
-        self._last_disconnection = self.time_func()
-        _LOGGER.warning("Roborock client disconnected")
-        if exc is not None:
-            _LOGGER.warning(exc)
-
-    def should_keepalive(self) -> bool:
-        now = self.time_func()
-        # noinspection PyUnresolvedReferences
-        if now - self._last_disconnection > self.keep_alive**2 and now - self._last_device_msg_in > self.keep_alive:
-            return False
-        return True
-
-    async def validate_connection(self) -> None:
-        if not self.should_keepalive():
-            await self.async_disconnect()
-        await self.async_connect()
-
-    async def _async_response(self, request_id: int, protocol_id: int = 0) -> tuple[Any, VacuumError | None]:
-        try:
-            queue = RoborockFuture(protocol_id)
-            self._waiting_queue[request_id] = queue
-            (response, err) = await queue.async_get(QUEUE_TIMEOUT)
-            return response, err
-        except (asyncio.TimeoutError, asyncio.CancelledError):
-            raise RoborockTimeout(f"Timeout after {QUEUE_TIMEOUT} seconds waiting for response") from None
-        finally:
-            del self._waiting_queue[request_id]
-
-    def _get_payload(self, method: RoborockCommand, params: Optional[list | dict] = None, secured=False):
-        timestamp = math.floor(time.time())
-        request_id = randint(10000, 99999)
-        inner = {
-            "id": request_id,
-            "method": method,
-            "params": params or [],
+    async def _async_value(self):
+        if self.unsupported:
+            return None
+        try:
+            self._value = await self.api._send_command(self.attribute.get_command)
+        except UnknownMethodError as err:
+            # Limit the amount of times we call unsupported methods
+            self.unsupported = True
+            raise err
+        return self._value
+
+    async def async_value(self):
+        async with self._mutex:
+            if self._value is None:
+                return await self.task.reset()
+            return self._value
+
+    def stop(self):
+        self.task.cancel()
+
+    async def update_value(self, params):
+        if self.attribute.set_command is None:
+            raise RoborockException(f"{self.attribute.attribute} have no set command")
+        response = await self.api._send_command(self.attribute.set_command, params)
+        await self._async_value()
+        return response
+
+    async def add_value(self, params):
+        if self.attribute.add_command is None:
+            raise RoborockException(f"{self.attribute.attribute} have no add command")
+        response = await self.api._send_command(self.attribute.add_command, params)
+        await self._async_value()
+        return response
+
+    async def close_value(self, params=None):
+        if self.attribute.close_command is None:
+            raise RoborockException(f"{self.attribute.attribute} have no close command")
+        response = await self.api._send_command(self.attribute.close_command, params)
+        await self._async_value()
+        return response
+
+    async def refresh_value(self):
+        await self._async_value()
+
+
+@dataclasses.dataclass
+class ListenerModel:
+    protocol_handlers: dict[RoborockDataProtocol, list[Callable[[Status | Consumable], None]]]
+    cache: dict[CacheableAttribute, AttributeCache]
+
+
+class RoborockClientV1(RoborockClient):
+    _listeners: dict[str, ListenerModel] = {}
+
+    def __init__(self, device_info: DeviceData, logger, endpoint: str):
+        super().__init__(endpoint, device_info)
+        self._status_type: type[Status] = ModelStatus.get(device_info.model, S7MaxVStatus)
+        self._logger = logger
+        self.cache: dict[CacheableAttribute, AttributeCache] = {
+            cacheable_attribute: AttributeCache(attr, self) for cacheable_attribute, attr in get_cache_map().items()
         }
-        if secured:
-            inner["security"] = {
-                "endpoint": self._endpoint,
-                "nonce": self._nonce.hex().lower(),
-            }
-        payload = bytes(
-            json.dumps(
-                {
-                    "dps": {"101": json.dumps(inner, separators=(",", ":"))},
-                    "t": timestamp,
-                },
-                separators=(",", ":"),
-            ).encode()
-        )
-        return request_id, timestamp, payload
-
-    async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
-        raise NotImplementedError
-
-    async def get_status(self) -> Status | None:
-        status = await self.send_command(RoborockCommand.GET_STATUS)
-        if isinstance(status, dict):
-            return Status.from_dict(status)
-        return None
+        if device_info.device.duid not in self._listeners:
+            self._listeners[device_info.device.duid] = ListenerModel({}, self.cache)
+        self.listener_model = self._listeners[device_info.device.duid]
+
+    def release(self):
+        super().release()
+        [item.stop() for item in self.cache.values()]
+
+    async def async_release(self):
+        await super().async_release()
+        [item.stop() for item in self.cache.values()]
 
-    async def get_dnd_timer(self) -> DNDTimer | None:
-        try:
-            dnd_timer = await self.send_command(RoborockCommand.GET_DND_TIMER)
-            if isinstance(dnd_timer, dict):
-                return DNDTimer.from_dict(dnd_timer)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+    @property
+    def status_type(self) -> type[Status]:
+        """Gets the status type for this device"""
+        return self._status_type
+
+    async def get_status(self) -> Status:
+        data = self._status_type.from_dict(await self.cache[CacheableAttribute.status].async_value())
+        if data is None:
+            return self._status_type()
+        return data
+
+    async def get_dnd_timer(self) -> DnDTimer | None:
+        return DnDTimer.from_dict(await self.cache[CacheableAttribute.dnd_timer].async_value())
+
+    async def get_valley_electricity_timer(self) -> ValleyElectricityTimer | None:
+        return ValleyElectricityTimer.from_dict(
+            await self.cache[CacheableAttribute.valley_electricity_timer].async_value()
+        )
 
     async def get_clean_summary(self) -> CleanSummary | None:
-        try:
-            clean_summary = await self.send_command(RoborockCommand.GET_CLEAN_SUMMARY)
-            if isinstance(clean_summary, dict):
-                return CleanSummary.from_dict(clean_summary)
-            elif isinstance(clean_summary, list):
-                clean_time, clean_area, clean_count, records = unpack_list(clean_summary, 4)
-                return CleanSummary(
-                    clean_time=clean_time, clean_area=clean_area, clean_count=clean_count, records=records
-                )
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
+        clean_summary: dict | list | int = await self.send_command(RoborockCommand.GET_CLEAN_SUMMARY)
+        if isinstance(clean_summary, dict):
+            return CleanSummary.from_dict(clean_summary)
+        elif isinstance(clean_summary, list):
+            clean_time, clean_area, clean_count, records = unpack_list(clean_summary, 4)
+            return CleanSummary(
+                clean_time=clean_time,
+                clean_area=clean_area,
+                clean_count=clean_count,
+                records=records,
+            )
+        elif isinstance(clean_summary, int):
+            return CleanSummary(clean_time=clean_summary)
         return None
 
     async def get_clean_record(self, record_id: int) -> CleanRecord | None:
-        try:
-            clean_record = await self.send_command(RoborockCommand.GET_CLEAN_RECORD, [record_id])
-            if isinstance(clean_record, dict):
-                return CleanRecord.from_dict(clean_record)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        record: dict | list = await self.send_command(RoborockCommand.GET_CLEAN_RECORD, [record_id])
+        if isinstance(record, dict):
+            return CleanRecord.from_dict(record)
+        elif isinstance(record, list):
+            # There are still a few unknown variables in this.
+            begin, end, duration, area = unpack_list(record, 4)
+            return CleanRecord(begin=begin, end=end, duration=duration, area=area)
+        else:
+            self._logger.warning("Clean record was of a new type, please submit an issue request: %s", record)
+            return None
 
-    async def get_consumable(self) -> Consumable | None:
-        try:
-            consumable = await self.send_command(RoborockCommand.GET_CONSUMABLE)
-            if isinstance(consumable, dict):
-                return Consumable.from_dict(consumable)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+    async def get_consumable(self) -> Consumable:
+        data = Consumable.from_dict(await self.cache[CacheableAttribute.consumable].async_value())
+        if data is None:
+            return Consumable()
+        return data
 
     async def get_wash_towel_mode(self) -> WashTowelMode | None:
-        try:
-            washing_mode = await self.send_command(RoborockCommand.GET_WASH_TOWEL_MODE)
-            if isinstance(washing_mode, dict):
-                return WashTowelMode.from_dict(washing_mode)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        return WashTowelMode.from_dict(await self.cache[CacheableAttribute.wash_towel_mode].async_value())
 
     async def get_dust_collection_mode(self) -> DustCollectionMode | None:
-        try:
-            dust_collection = await self.send_command(RoborockCommand.GET_DUST_COLLECTION_MODE)
-            if isinstance(dust_collection, dict):
-                return DustCollectionMode.from_dict(dust_collection)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        return DustCollectionMode.from_dict(await self.cache[CacheableAttribute.dust_collection_mode].async_value())
 
     async def get_smart_wash_params(self) -> SmartWashParams | None:
-        try:
-            mop_wash_mode = await self.send_command(RoborockCommand.GET_SMART_WASH_PARAMS)
-            if isinstance(mop_wash_mode, dict):
-                return SmartWashParams.from_dict(mop_wash_mode)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        return SmartWashParams.from_dict(await self.cache[CacheableAttribute.smart_wash_params].async_value())
 
-    async def get_dock_summary(self, dock_type: RoborockEnum) -> DockSummary | None:
+    async def get_dock_summary(self, dock_type: RoborockDockTypeCode) -> DockSummary:
         """Gets the status summary from the dock with the methods available for a given dock.
 
         :param dock_type: RoborockDockTypeCode"""
-        try:
-            commands: list[
-                Coroutine[
-                    Any,
-                    Any,
-                    DustCollectionMode | WashTowelMode | SmartWashParams | None,
-                ]
-            ] = [self.get_dust_collection_mode()]
-            if dock_type == RoborockDockTypeCode["3"]:
-                commands += [
-                    self.get_wash_towel_mode(),
-                    self.get_smart_wash_params(),
-                ]
-            [dust_collection_mode, wash_towel_mode, smart_wash_params] = unpack_list(
-                list(await asyncio.gather(*commands)), 3
-            )
+        commands: list[
+            Coroutine[
+                Any,
+                Any,
+                DustCollectionMode | WashTowelMode | SmartWashParams | None,
+            ]
+        ] = [self.get_dust_collection_mode()]
+        if dock_type in WASH_N_FILL_DOCK:
+            commands += [
+                self.get_wash_towel_mode(),
+                self.get_smart_wash_params(),
+            ]
+        [dust_collection_mode, wash_towel_mode, smart_wash_params] = unpack_list(
+            list(await asyncio.gather(*commands)), 3
+        )  # type: DustCollectionMode, WashTowelMode | None, SmartWashParams | None # type: ignore
 
-            return DockSummary(dust_collection_mode, wash_towel_mode, smart_wash_params)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        return DockSummary(dust_collection_mode, wash_towel_mode, smart_wash_params)
 
     async def get_prop(self) -> DeviceProp | None:
-        [status, dnd_timer, clean_summary, consumable] = await asyncio.gather(
+        """Gets device general properties."""
+        # Mypy thinks that each one of these is typed as a union of all the others. so we do type ignore.
+        status, clean_summary, consumable = await asyncio.gather(
             *[
                 self.get_status(),
-                self.get_dnd_timer(),
                 self.get_clean_summary(),
                 self.get_consumable(),
             ]
-        )
+        )  # type: Status, CleanSummary, Consumable # type: ignore
         last_clean_record = None
         if clean_summary and clean_summary.records and len(clean_summary.records) > 0:
             last_clean_record = await self.get_clean_record(clean_summary.records[0])
         dock_summary = None
-        if status and status.dock_type is not None and status.dock_type != RoborockDockTypeCode["0"]:
+        if status and status.dock_type is not None and status.dock_type != RoborockDockTypeCode.no_dock:
             dock_summary = await self.get_dock_summary(status.dock_type)
-        if any([status, dnd_timer, clean_summary, consumable]):
+        if any([status, clean_summary, consumable]):
             return DeviceProp(
                 status,
-                dnd_timer,
                 clean_summary,
                 consumable,
                 last_clean_record,
                 dock_summary,
             )
         return None
 
     async def get_multi_maps_list(self) -> MultiMapsList | None:
-        try:
-            multi_maps_list = await self.send_command(RoborockCommand.GET_MULTI_MAPS_LIST)
-            if isinstance(multi_maps_list, dict):
-                return MultiMapsList.from_dict(multi_maps_list)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        return await self.send_command(RoborockCommand.GET_MULTI_MAPS_LIST, return_type=MultiMapsList)
 
     async def get_networking(self) -> NetworkInfo | None:
-        try:
-            networking_info = await self.send_command(RoborockCommand.GET_NETWORK_INFO)
-            if isinstance(networking_info, dict):
-                return NetworkInfo.from_dict(networking_info)
-        except RoborockTimeout as e:
-            _LOGGER.error(e)
-        return None
+        return await self.send_command(RoborockCommand.GET_NETWORK_INFO, return_type=NetworkInfo)
 
-    async def get_room_mapping(self) -> list[RoomMapping]:
+    async def get_room_mapping(self) -> list[RoomMapping] | None:
         """Gets the mapping from segment id -> iot id. Only works on local api."""
-        mapping = await self.send_command(RoborockCommand.GET_ROOM_MAPPING)
+        mapping: list = await self.send_command(RoborockCommand.GET_ROOM_MAPPING)
         if isinstance(mapping, list):
             return [
                 RoomMapping(segment_id=segment_id, iot_id=iot_id)  # type: ignore
-                for segment_id, iot_id in [unpack_list(room, 2) for room in mapping]
+                for segment_id, iot_id in [unpack_list(room, 2) for room in mapping if isinstance(room, list)]
             ]
-        return []
-
+        return None
 
-class RoborockApiClient:
-    def __init__(self, username: str, base_url=None) -> None:
-        """Sample API Client."""
-        self._username = username
-        self._default_url = "https://euiot.roborock.com"
-        self.base_url = base_url
-        self._device_identifier = secrets.token_urlsafe(16)
-
-    async def _get_base_url(self) -> str:
-        if not self.base_url:
-            url_request = PreparedRequest(self._default_url)
-            response = await url_request.request(
-                "post",
-                "/api/v1/getUrlByEmail",
-                params={"email": self._username, "needtwostepauth": "false"},
-            )
-            if response is None:
-                raise RoborockUrlException("get url by email returned None")
-            response_code = response.get("code")
-            if response_code != 200:
-                if response_code == 2003:
-                    raise RoborockInvalidEmail("Your email was incorrectly formatted.")
-                raise RoborockUrlException(response.get("error"))
-            response_data = response.get("data")
-            if response_data is None:
-                raise RoborockUrlException("response does not have 'data'")
-            self.base_url = response_data.get("url")
-        return self.base_url
-
-    def _get_header_client_id(self):
-        md5 = hashlib.md5()
-        md5.update(self._username.encode())
-        md5.update(self._device_identifier.encode())
-        return base64.b64encode(md5.digest()).decode()
-
-    async def request_code(self) -> None:
-        base_url = await self._get_base_url()
-        header_clientid = self._get_header_client_id()
-        code_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
-
-        code_response = await code_request.request(
-            "post",
-            "/api/v1/sendEmailCode",
-            params={
-                "username": self._username,
-                "type": "auth",
-            },
-        )
-        if code_response is None:
-            raise RoborockException("Failed to get a response from send email code")
-        response_code = code_response.get("code")
-        if response_code != 200:
-            if response_code == 2008:
-                raise RoborockAccountDoesNotExist("Account does not exist - check your login and try again.")
-            else:
-                raise RoborockException(f"{code_response.get('msg')} - response code: {code_response.get('code')}")
-
-    async def pass_login(self, password: str) -> UserData:
-        base_url = await self._get_base_url()
-        header_clientid = self._get_header_client_id()
-
-        login_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
-        login_response = await login_request.request(
-            "post",
-            "/api/v1/login",
-            params={
-                "username": self._username,
-                "password": password,
-                "needtwostepauth": "false",
-            },
-        )
-        if login_response is None:
-            raise RoborockException("Login response is none")
-        if login_response.get("code") != 200:
-            raise RoborockException(f"{login_response.get('msg')} - response code: {login_response.get('code')}")
-        user_data = login_response.get("data")
-        if not isinstance(user_data, dict):
-            raise RoborockException("Got unexpected data type for user_data")
-        return UserData.from_dict(user_data)
-
-    async def code_login(self, code) -> UserData:
-        base_url = await self._get_base_url()
-        header_clientid = self._get_header_client_id()
-
-        login_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
-        login_response = await login_request.request(
-            "post",
-            "/api/v1/loginWithCode",
-            params={
-                "username": self._username,
-                "verifycode": code,
-                "verifycodetype": "AUTH_EMAIL_CODE",
-            },
-        )
-        if login_response is None:
-            raise RoborockException("Login request response is None")
-        response_code = login_response.get("code")
-        if response_code != 200:
-            if response_code == 2018:
-                raise RoborockInvalidCode("Invalid code - check your code and try again.")
-            raise RoborockException(f"{login_response.get('msg')} - response code: {response_code}")
-        user_data = login_response.get("data")
-        if not isinstance(user_data, dict):
-            raise RoborockException("Got unexpected data type for user_data")
-        return UserData.from_dict(user_data)
-
-    async def get_home_data(self, user_data: UserData) -> HomeData:
-        base_url = await self._get_base_url()
-        header_clientid = self._get_header_client_id()
-        rriot = user_data.rriot
-        if rriot is None:
-            raise RoborockException("rriot is none")
-        home_id_request = PreparedRequest(base_url, {"header_clientid": header_clientid})
-        home_id_response = await home_id_request.request(
-            "get",
-            "/api/v1/getHomeDetail",
-            headers={"Authorization": user_data.token},
-        )
-        if home_id_response is None:
-            raise RoborockException("home_id_response is None")
-        if home_id_response.get("code") != 200:
-            raise RoborockException(f"{home_id_response.get('msg')} - response code: {home_id_response.get('code')}")
+    async def get_child_lock_status(self) -> ChildLockStatus:
+        """Gets current child lock status."""
+        return ChildLockStatus.from_dict(await self.cache[CacheableAttribute.child_lock_status].async_value())
+
+    async def get_flow_led_status(self) -> FlowLedStatus:
+        """Gets current flow led status."""
+        return FlowLedStatus.from_dict(await self.cache[CacheableAttribute.flow_led_status].async_value())
+
+    async def get_sound_volume(self) -> int | None:
+        """Gets current volume level."""
+        return await self.cache[CacheableAttribute.sound_volume].async_value()
+
+    async def get_server_timer(self) -> list[ServerTimer]:
+        """Gets current server timer."""
+        server_timers = await self.cache[CacheableAttribute.server_timer].async_value()
+        if server_timers:
+            if isinstance(server_timers[0], list):
+                return [ServerTimer(*server_timer) for server_timer in server_timers]
+            return [ServerTimer(*server_timers)]
+        return []
 
-        home_id = home_id_response["data"].get("rrHomeId")
+    def _get_payload(
+        self,
+        method: RoborockCommand | str,
+        params: list | dict | int | None = None,
+        secured=False,
+    ):
         timestamp = math.floor(time.time())
-        nonce = secrets.token_urlsafe(6)
-        prestr = ":".join(
-            [
-                rriot.u,
-                rriot.s,
-                nonce,
-                str(timestamp),
-                hashlib.md5(("/user/homes/" + str(home_id)).encode()).hexdigest(),
-                "",
-                "",
-            ]
-        )
-        mac = base64.b64encode(hmac.new(rriot.h.encode(), prestr.encode(), hashlib.sha256).digest()).decode()
-        if rriot.r.a is None:
-            raise RoborockException("Missing field 'a' in rriot reference")
-        home_request = PreparedRequest(
-            rriot.r.a,
-            {
-                "Authorization": f'Hawk id="{rriot.u}", s="{rriot.s}", ts="{timestamp}", nonce="{nonce}", mac="{mac}"',
-            },
+        request_id = randint(10000, 32767)
+        inner = {
+            "id": request_id,
+            "method": method,
+            "params": params or [],
+        }
+        if secured:
+            inner["security"] = {
+                "endpoint": self._endpoint,
+                "nonce": self._nonce.hex().lower(),
+            }
+        payload = bytes(
+            json.dumps(
+                {
+                    "dps": {"101": json.dumps(inner, separators=(",", ":"))},
+                    "t": timestamp,
+                },
+                separators=(",", ":"),
+            ).encode()
         )
-        home_response = await home_request.request("get", "/user/homes/" + str(home_id))
-        if not home_response.get("success"):
-            raise RoborockException(home_response)
-        home_data = home_response.get("result")
-        if isinstance(home_data, dict):
-            return HomeData.from_dict(home_data)
+        return request_id, timestamp, payload
+
+    def on_message_received(self, messages: list[RoborockMessage]) -> None:
+        try:
+            self._last_device_msg_in = self.time_func()
+            for data in messages:
+                protocol = data.protocol
+                if data.payload and protocol in [
+                    RoborockMessageProtocol.RPC_RESPONSE,
+                    RoborockMessageProtocol.GENERAL_REQUEST,
+                ]:
+                    payload = json.loads(data.payload.decode())
+                    for data_point_number, data_point in payload.get("dps").items():
+                        if data_point_number == "102":
+                            data_point_response = json.loads(data_point)
+                            request_id = data_point_response.get("id")
+                            queue = self._waiting_queue.get(request_id)
+                            if queue and queue.protocol == protocol:
+                                error = data_point_response.get("error")
+                                if error:
+                                    queue.resolve(
+                                        (
+                                            None,
+                                            VacuumError(
+                                                error.get("code"),
+                                                error.get("message"),
+                                            ),
+                                        )
+                                    )
+                                else:
+                                    result = data_point_response.get("result")
+                                    if isinstance(result, list) and len(result) == 1:
+                                        result = result[0]
+                                    queue.resolve((result, None))
+                        else:
+                            try:
+                                data_protocol = RoborockDataProtocol(int(data_point_number))
+                                self._logger.debug(f"Got device update for {data_protocol.name}: {data_point}")
+                                if data_protocol in ROBOROCK_DATA_STATUS_PROTOCOL:
+                                    if data_protocol not in self.listener_model.protocol_handlers:
+                                        self._logger.debug(
+                                            f"Got status update({data_protocol.name}) before get_status was called."
+                                        )
+                                        return
+                                    value = self.listener_model.cache[CacheableAttribute.status].value
+                                    value[data_protocol.name] = data_point
+                                    status = self._status_type.from_dict(value)
+                                    for listener in self.listener_model.protocol_handlers.get(data_protocol, []):
+                                        listener(status)
+                                elif data_protocol in ROBOROCK_DATA_CONSUMABLE_PROTOCOL:
+                                    if data_protocol not in self.listener_model.protocol_handlers:
+                                        self._logger.debug(
+                                            f"Got consumable update({data_protocol.name})"
+                                            + "before get_consumable was called."
+                                        )
+                                        return
+                                    value = self.listener_model.cache[CacheableAttribute.consumable].value
+                                    value[data_protocol.name] = data_point
+                                    consumable = Consumable.from_dict(value)
+                                    for listener in self.listener_model.protocol_handlers.get(data_protocol, []):
+                                        listener(consumable)
+                                return
+                            except ValueError:
+                                self._logger.warning(
+                                    f"Got listener data for {data_point_number}, data: {data_point}. "
+                                    f"This lets us update data quicker, please open an issue "
+                                    f"at https://github.com/humbertogontijo/python-roborock/issues"
+                                )
+
+                                pass
+                            dps = {data_point_number: data_point}
+                            self._logger.debug(f"Got unknown data point {dps}")
+                elif data.payload and protocol == RoborockMessageProtocol.MAP_RESPONSE:
+                    payload = data.payload[0:24]
+                    [endpoint, _, request_id, _] = struct.unpack("<8s8sH6s", payload)
+                    if endpoint.decode().startswith(self._endpoint):
+                        try:
+                            decrypted = Utils.decrypt_cbc(data.payload[24:], self._nonce)
+                        except ValueError as err:
+                            raise RoborockException(f"Failed to decode {data.payload!r} for {data.protocol}") from err
+                        decompressed = Utils.decompress(decrypted)
+                        queue = self._waiting_queue.get(request_id)
+                        if queue:
+                            if isinstance(decompressed, list):
+                                decompressed = decompressed[0]
+                            queue.resolve((decompressed, None))
+                else:
+                    queue = self._waiting_queue.get(data.seq)
+                    if queue:
+                        queue.resolve((data.payload, None))
+        except Exception as ex:
+            self._logger.exception(ex)
+
+    async def get_from_cache(self, key: CacheableAttribute) -> AttributeCache | None:
+        val = self.cache.get(key)
+        if val is not None:
+            return await val.async_value()
+        return None
+
+    def add_listener(
+        self, protocol: RoborockDataProtocol, listener: Callable, cache: dict[CacheableAttribute, AttributeCache]
+    ) -> None:
+        self.listener_model.cache = cache
+        if protocol not in self.listener_model.protocol_handlers:
+            self.listener_model.protocol_handlers[protocol] = []
+        self.listener_model.protocol_handlers[protocol].append(listener)
+
+    def remove_listener(self, protocol: RoborockDataProtocol, listener: Callable) -> None:
+        self.listener_model.protocol_handlers[protocol].remove(listener)
+
+    @final
+    async def send_command(
+        self,
+        method: RoborockCommand | str,
+        params: list | dict | int | None = None,
+        return_type: type[RT] | None = None,
+    ) -> RT:
+        cacheable_attribute_result = find_cacheable_attribute(method)
+
+        cache = None
+        command_type = None
+        if cacheable_attribute_result is not None:
+            cache = self.cache[cacheable_attribute_result.attribute]
+            command_type = cacheable_attribute_result.type
+
+        response: Any = None
+        if cache is not None and command_type == CommandType.GET:
+            response = await cache.async_value()
         else:
-            raise RoborockException("home_response result was an unexpected type")
+            response = await self._send_command(method, params)
+            if cache is not None and command_type == CommandType.CHANGE:
+                await cache.refresh_value()
+
+        if return_type:
+            return return_type.from_dict(response)
+        return response
```

### Comparing `python_roborock-0.9.0rc0/roborock/cloud_api.py` & `python_roborock-1.0.0/roborock/cloud_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,174 +1,180 @@
 from __future__ import annotations
 
+import asyncio
 import base64
 import logging
 import threading
+import typing
 import uuid
-from asyncio import Lock
-from typing import Optional
+from asyncio import Lock, Task
+from typing import Any
 from urllib.parse import urlparse
 
 import paho.mqtt.client as mqtt
 
-from .api import KEEPALIVE, SPECIAL_COMMANDS, RoborockClient, md5hex
-from .containers import RoborockDeviceInfo, UserData
-from .exceptions import CommandVacuumError, RoborockException, VacuumError
+from .api import KEEPALIVE, RoborockClient
+from .containers import DeviceData, UserData
+from .exceptions import RoborockException, VacuumError
+from .protocol import MessageParser, Utils, md5hex
 from .roborock_future import RoborockFuture
-from .roborock_message import RoborockMessage, RoborockParser, md5bin
-from .typing import RoborockCommand
+from .roborock_message import RoborockMessage
+from .roborock_typing import RoborockCommand
+from .util import RoborockLoggerAdapter
 
+if typing.TYPE_CHECKING:
+    pass
 _LOGGER = logging.getLogger(__name__)
 CONNECT_REQUEST_ID = 0
 DISCONNECT_REQUEST_ID = 1
 
 
 class RoborockMqttClient(RoborockClient, mqtt.Client):
     _thread: threading.Thread
     _client_id: str
 
-    def __init__(self, user_data: UserData, device_info: RoborockDeviceInfo) -> None:
+    def __init__(self, user_data: UserData, device_info: DeviceData, queue_timeout: int = 10) -> None:
         rriot = user_data.rriot
         if rriot is None:
             raise RoborockException("Got no rriot data from user_data")
-        endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
-        RoborockClient.__init__(self, endpoint, device_info)
+        endpoint = base64.b64encode(Utils.md5(rriot.k.encode())[8:14]).decode()
+        RoborockClient.__init__(self, endpoint, device_info, queue_timeout)
         mqtt.Client.__init__(self, protocol=mqtt.MQTTv5)
+        self._logger = RoborockLoggerAdapter(device_info.device.name, _LOGGER)
         self._mqtt_user = rriot.u
         self._hashed_user = md5hex(self._mqtt_user + ":" + rriot.k)[2:10]
         url = urlparse(rriot.r.m)
         if not isinstance(url.hostname, str):
             raise RoborockException("Url parsing returned an invalid hostname")
         self._mqtt_host = str(url.hostname)
         self._mqtt_port = url.port
         self._mqtt_ssl = url.scheme == "ssl"
         if self._mqtt_ssl:
             super().tls_set()
         self._mqtt_password = rriot.s
         self._hashed_password = md5hex(self._mqtt_password + ":" + rriot.k)[16:]
         super().username_pw_set(self._hashed_user, self._hashed_password)
-        self._endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
+        self._endpoint = base64.b64encode(Utils.md5(rriot.k.encode())[8:14]).decode()
         self._waiting_queue: dict[int, RoborockFuture] = {}
         self._mutex = Lock()
         self.update_client_id()
 
     def on_connect(self, *args, **kwargs):
         _, __, ___, rc, ____ = args
         connection_queue = self._waiting_queue.get(CONNECT_REQUEST_ID)
         if rc != mqtt.MQTT_ERR_SUCCESS:
-            message = f"Failed to connect (rc: {rc})"
-            _LOGGER.error(message)
+            message = f"Failed to connect ({mqtt.error_string(rc)})"
+            self._logger.error(message)
             if connection_queue:
-                connection_queue.resolve((None, VacuumError(rc, message)))
+                connection_queue.resolve((None, VacuumError(message)))
             return
-        _LOGGER.info(f"Connected to mqtt {self._mqtt_host}:{self._mqtt_port}")
+        self._logger.info(f"Connected to mqtt {self._mqtt_host}:{self._mqtt_port}")
         topic = f"rr/m/o/{self._mqtt_user}/{self._hashed_user}/{self.device_info.device.duid}"
         (result, mid) = self.subscribe(topic)
         if result != 0:
-            message = f"Failed to subscribe (rc: {result})"
-            _LOGGER.error(message)
+            message = f"Failed to subscribe ({mqtt.error_string(rc)})"
+            self._logger.error(message)
             if connection_queue:
-                connection_queue.resolve((None, VacuumError(rc, message)))
+                connection_queue.resolve((None, VacuumError(message)))
             return
-        _LOGGER.info(f"Subscribed to topic {topic}")
+        self._logger.info(f"Subscribed to topic {topic}")
         if connection_queue:
             connection_queue.resolve((True, None))
 
     def on_message(self, *args, **kwargs):
-        _, __, msg = args
+        client, __, msg = args
         try:
-            messages, _ = RoborockParser.decode(msg.payload, self.device_info.device.local_key)
+            messages, _ = MessageParser.parse(msg.payload, local_key=self.device_info.device.local_key)
             super().on_message_received(messages)
         except Exception as ex:
-            _LOGGER.exception(ex)
+            self._logger.exception(ex)
 
     def on_disconnect(self, *args, **kwargs):
         _, __, rc, ___ = args
         try:
-            super().on_connection_lost(RoborockException(f"(rc: {rc})"))
+            exc = RoborockException(mqtt.error_string(rc)) if rc != mqtt.MQTT_ERR_SUCCESS else None
+            super().on_connection_lost(exc)
             if rc == mqtt.MQTT_ERR_PROTOCOL:
                 self.update_client_id()
             connection_queue = self._waiting_queue.get(DISCONNECT_REQUEST_ID)
             if connection_queue:
                 connection_queue.resolve((True, None))
         except Exception as ex:
-            _LOGGER.exception(ex)
+            self._logger.exception(ex)
 
     def update_client_id(self):
         self._client_id = mqtt.base62(uuid.uuid4().int, padding=22)
 
     def sync_stop_loop(self) -> None:
         if self._thread:
-            _LOGGER.info("Stopping mqtt loop")
+            self._logger.info("Stopping mqtt loop")
             super().loop_stop()
 
     def sync_start_loop(self) -> None:
         if not self._thread or not self._thread.is_alive():
             self.sync_stop_loop()
-            _LOGGER.info("Starting mqtt loop")
+            self._logger.info("Starting mqtt loop")
             super().loop_start()
 
-    def sync_disconnect(self) -> bool:
-        rc = mqtt.MQTT_ERR_AGAIN
+    def sync_disconnect(self) -> tuple[bool, Task[tuple[Any, VacuumError | None]] | None]:
+        if not self.is_connected():
+            return False, None
+
+        self._logger.info("Disconnecting from mqtt")
+        disconnected_future = asyncio.ensure_future(self._async_response(DISCONNECT_REQUEST_ID))
+        rc = super().disconnect()
+
+        if rc == mqtt.MQTT_ERR_NO_CONN:
+            disconnected_future.cancel()
+            return False, None
+
+        if rc != mqtt.MQTT_ERR_SUCCESS:
+            disconnected_future.cancel()
+            raise RoborockException(f"Failed to disconnect ({mqtt.error_string(rc)})")
+
+        return True, disconnected_future
+
+    def sync_connect(self) -> tuple[bool, Task[tuple[Any, VacuumError | None]] | None]:
         if self.is_connected():
-            _LOGGER.info("Disconnecting from mqtt")
-            rc = super().disconnect()
-            if rc not in [mqtt.MQTT_ERR_SUCCESS, mqtt.MQTT_ERR_NO_CONN]:
-                raise RoborockException(f"Failed to disconnect (rc:{rc})")
-        return rc == mqtt.MQTT_ERR_SUCCESS
+            self.sync_start_loop()
+            return False, None
+
+        if self._mqtt_port is None or self._mqtt_host is None:
+            raise RoborockException("Mqtt information was not entered. Cannot connect.")
+
+        self._logger.debug("Connecting to mqtt")
+        connected_future = asyncio.ensure_future(self._async_response(CONNECT_REQUEST_ID))
+        super().connect(host=self._mqtt_host, port=self._mqtt_port, keepalive=KEEPALIVE)
 
-    def sync_connect(self) -> bool:
         self.sync_start_loop()
-        if not self.is_connected():
-            if self._mqtt_port is None or self._mqtt_host is None:
-                raise RoborockException("Mqtt information was not entered. Cannot connect.")
-            _LOGGER.info("Connecting to mqtt")
-            super().connect_async(host=self._mqtt_host, port=self._mqtt_port, keepalive=KEEPALIVE)
-            return True
-        return False
+        return True, connected_future
 
     async def async_disconnect(self) -> None:
         async with self._mutex:
-            disconnecting = self.sync_disconnect()
-            if disconnecting:
-                (_, err) = await self._async_response(DISCONNECT_REQUEST_ID)
+            (disconnecting, disconnected_future) = self.sync_disconnect()
+            if disconnecting and disconnected_future:
+                (_, err) = await disconnected_future
                 if err:
                     raise RoborockException(err) from err
 
     async def async_connect(self) -> None:
         async with self._mutex:
-            connecting = self.sync_connect()
-            if connecting:
-                (_, err) = await self._async_response(CONNECT_REQUEST_ID)
+            (connecting, connected_future) = self.sync_connect()
+            if connecting and connected_future:
+                (_, err) = await connected_future
                 if err:
                     raise RoborockException(err) from err
 
     def _send_msg_raw(self, msg: bytes) -> None:
         info = self.publish(f"rr/m/i/{self._mqtt_user}/{self._hashed_user}/{self.device_info.device.duid}", msg)
         if info.rc != mqtt.MQTT_ERR_SUCCESS:
-            raise RoborockException(f"Failed to publish (rc: {info.rc})")
+            raise RoborockException(f"Failed to publish ({mqtt.error_string(info.rc)})")
 
-    async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
-        await self.validate_connection()
-        request_id, timestamp, payload = super()._get_payload(method, params, True)
-        _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
-        request_protocol = 101
-        response_protocol = 301 if method in SPECIAL_COMMANDS else 102
-        roborock_message = RoborockMessage(timestamp=timestamp, protocol=request_protocol, payload=payload)
-        local_key = self.device_info.device.local_key
-        msg = RoborockParser.encode(roborock_message, local_key)
-        self._send_msg_raw(msg)
-        (response, err) = await self._async_response(request_id, response_protocol)
-        if err:
-            raise CommandVacuumError(method, err) from err
-        if response_protocol == 301:
-            _LOGGER.debug(f"id={request_id} Response from {method}: {len(response)} bytes")
-        else:
-            _LOGGER.debug(f"id={request_id} Response from {method}: {response}")
-        return response
+    async def send_message(self, roborock_message: RoborockMessage):
+        raise NotImplementedError
 
-    async def get_map_v1(self):
-        try:
-            return await self.send_command(RoborockCommand.GET_MAP_V1)
-        except RoborockException as e:
-            _LOGGER.error(e)
-        return None
+    async def _send_command(
+        self,
+        method: RoborockCommand | str,
+        params: list | dict | int | None = None,
+    ):
+        raise NotImplementedError
```

### Comparing `python_roborock-0.9.0rc0/roborock/exceptions.py` & `python_roborock-1.0.0/roborock/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Roborock exceptions."""
+from __future__ import annotations
 
 
 class RoborockException(Exception):
     """Class for Roborock exceptions."""
 
 
 class RoborockTimeout(RoborockException):
@@ -16,39 +17,54 @@
 class RoborockBackoffException(RoborockException):
     """Class for Roborock exceptions when many retries were made."""
 
 
 class VacuumError(RoborockException):
     """Class for vacuum errors."""
 
-    def __init__(self, code, message):
-        self.code = code
-        self.message = message
-        super().__init__()
-
-    def __str__(self, *args, **kwargs):  # real signature unknown
-        """Return str(self)."""
-        return f"{self.code}: {self.message}"
-
 
 class CommandVacuumError(RoborockException):
     """Class for command vacuum errors."""
 
-    def __init__(self, command: str, vacuum_error: VacuumError):
-        self.message = f"{command}: {str(vacuum_error)}"
+    def __init__(self, command: str | None, vacuum_error: VacuumError):
+        self.message = f"{command or 'unknown'}: {str(vacuum_error)}"
         super().__init__(self.message)
 
 
+class UnknownMethodError(RoborockException):
+    """Class for an invalid method being sent."""
+
+
 class RoborockAccountDoesNotExist(RoborockException):
     """Class for Roborock account does not exist exceptions."""
 
 
 class RoborockUrlException(RoborockException):
     """Class for being unable to get the URL for the Roborock account."""
 
 
 class RoborockInvalidCode(RoborockException):
     """Class for Roborock invalid code exceptions."""
 
 
 class RoborockInvalidEmail(RoborockException):
     """Class for Roborock invalid formatted email exceptions."""
+
+
+class RoborockInvalidUserAgreement(RoborockException):
+    """Class for Roborock invalid user agreement exceptions."""
+
+
+class RoborockNoUserAgreement(RoborockException):
+    """Class for Roborock no user agreement exceptions."""
+
+
+class RoborockInvalidCredentials(RoborockException):
+    """Class for Roborock credentials have expired or changed."""
+
+
+class RoborockTooFrequentCodeRequests(RoborockException):
+    """Class for Roborock too frequent code requests exceptions."""
+
+
+class RoborockMissingParameters(RoborockException):
+    """Class for Roborock missing parameters exceptions."""
```

### Comparing `python_roborock-0.9.0rc0/roborock/roborock_future.py` & `python_roborock-1.0.0/roborock/roborock_future.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 
 class RoborockFuture:
     def __init__(self, protocol: int):
         self.protocol = protocol
         self.fut: Future = Future()
         self.loop = self.fut.get_loop()
 
+    def _resolve(self, item: tuple[Any, VacuumError | None]) -> None:
+        if not self.fut.cancelled():
+            self.fut.set_result(item)
+
     def resolve(self, item: tuple[Any, VacuumError | None]) -> None:
-        self.loop.call_soon_threadsafe(self.fut.set_result, item)
+        self.loop.call_soon_threadsafe(self._resolve, item)
 
     async def async_get(self, timeout: float | int) -> tuple[Any, VacuumError | None]:
         try:
             async with async_timeout.timeout(timeout):
                 return await self.fut
         finally:
             self.fut.cancel()
```

