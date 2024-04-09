# Comparing `tmp/taskiq_matrix-0.0.9.tar.gz` & `tmp/taskiq_matrix-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_matrix-0.0.9.tar", max compression
+gzip compressed data, was "taskiq_matrix-0.1.0.tar", max compression
```

## Comparing `taskiq_matrix-0.0.9.tar` & `taskiq_matrix-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    34523 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/LICENSE
--rw-r--r--   0        0        0       83 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/README.md
--rw-r--r--   0        0        0      862 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      157 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/__init__.py
--rw-r--r--   0        0        0     2183 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/exceptions.py
--rw-r--r--   0        0        0     6990 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/filters.py
--rw-r--r--   0        0        0      986 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/instance.py
--rw-r--r--   0        0        0     8185 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/lock.py
--rw-r--r--   0        0        0    17948 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/matrix_broker.py
--rw-r--r--   0        0        0    16825 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/matrix_queue.py
--rw-r--r--   0        0        0     6306 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/matrix_result_backend.py
--rw-r--r--   0        0        0     6165 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/schedulesource.py
--rw-r--r--   0        0        0     3425 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/tasks.py
--rw-r--r--   0        0        0     2179 2024-02-05 17:34:07.200129 taskiq_matrix-0.0.9/taskiq_matrix/utils.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 taskiq_matrix-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-12-06 15:52:19.999334 taskiq_matrix-0.1.0/LICENSE
+-rw-r--r--   0        0        0       63 2023-12-06 15:52:19.999334 taskiq_matrix-0.1.0/README.md
+-rw-r--r--   0        0        0      762 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/__init__.py
+-rw-r--r--   0        0        0     2183 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/exceptions.py
+-rw-r--r--   0        0        0     5547 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/filters.py
+-rw-r--r--   0        0        0      508 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/instance.py
+-rw-r--r--   0        0        0     8238 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/lock.py
+-rw-r--r--   0        0        0    16823 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/matrix_broker.py
+-rw-r--r--   0        0        0    15319 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/matrix_queue.py
+-rw-r--r--   0        0        0     6048 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/matrix_result_backend.py
+-rw-r--r--   0        0        0     6165 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/schedulesource.py
+-rw-r--r--   0        0        0     3193 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/tasks.py
+-rw-r--r--   0        0        0     2191 2023-12-06 15:52:20.003334 taskiq_matrix-0.1.0/taskiq_matrix/utils.py
+-rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 taskiq_matrix-0.1.0/PKG-INFO
```

### Comparing `taskiq_matrix-0.0.9/LICENSE` & `taskiq_matrix-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_matrix-0.0.9/pyproject.toml` & `taskiq_matrix-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "taskiq-matrix"
-version = "0.0.9"
+version = "0.1.0"
 description = ""
 authors = ["Mo Balaa <balaa@ether.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 taskiq = "^0.10.4"
 matrix-nio = "^0.22.1"
-fractal-matrix-client = ">=0.0.1"
-async-lru = "^2.0.4"
+fractal-matrix-client = "^0.1.0"
 
 docker = { version = "^6.1.3", optional = true }
 pytest = { version = "^7.4.2", optional = true }
 pytest-asyncio = { version = "^0.21.1", optional = true }
 pytest-cov = { version = "^4.1.0", optional = true }
 pytest-mock = { version = "^3.11.1", optional = true }
 ipython = { version = "^8.17.2", optional = true }
-pytest-benchmark = { version = "^4.0.0", optional = true }
 
 [tool.poetry.extras]
-dev = ["pytest", "pytest-asyncio", "pytest-cov", "pytest-mock", "docker", "ipython", "pytest-benchmark"]
+dev = ["pytest", "pytest-asyncio", "pytest-cov", "pytest-mock", "docker", "ipython"]
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/exceptions.py` & `taskiq_matrix-0.1.0/taskiq_matrix/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/filters.py` & `taskiq_matrix-0.1.0/taskiq_matrix/filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from copy import deepcopy
-from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Union
+from typing import Any, Dict, Optional
 from uuid import uuid4
 
-if TYPE_CHECKING: # pragma: no cover
-    from taskiq_matrix.matrix_queue import TaskTypes
-
 from fractal.matrix.async_client import FractalAsyncClient
-from nio import BadEvent, Event, MessageDirection, RoomMessagesError, SyncError
+from nio import SyncError
 
-EMPTY_FILTER: Dict[str, Union[Dict[str, Any], str]] = {
+EMPTY_FILTER = {
     "presence": {"limit": 0, "types": []},
     "account_data": {"limit": 0, "types": []},
     "room": {
         "rooms": [],
         "state": {"types": [], "limit": 0},
         "timeline": {"types": [], "limit": 0},
         "account_data": {"limit": 0, "types": []},
@@ -41,189 +37,131 @@
 
 def create_filter(
     room_id: str,
     types: list = [],
     not_types: list = [],
     limit: Optional[int] = None,
     not_senders: list = [],
-    room_event_filter: bool = False,
 ) -> Dict[str, Any]:
     """
     Create a filter for a room and/or specific message types.
 
     Returns:
         filter dict
     """
-    message_filter = {
+    if limit is None:
+        return {
+            "presence": {"limit": 0, "types": []},
+            "account_data": {"limit": 0, "types": []},
+            "room": {
+                "rooms": [room_id],
+                "state": {"types": [], "limit": 0},
+                "timeline": {
+                    "types": [*types],
+                    "not_types": [*not_types],
+                    "not_senders": [*not_senders],
+                },
+            },
+            "request_id": str(uuid4()),
+        }
+
+    return {
         "presence": {"limit": 0, "types": []},
         "account_data": {"limit": 0, "types": []},
         "room": {
             "rooms": [room_id],
             "state": {"types": [], "limit": 0},
             "timeline": {
                 "types": [*types],
                 "not_types": [*not_types],
                 "not_senders": [*not_senders],
+                "limit": limit,
             },
         },
         "request_id": str(uuid4()),
     }
-    if limit is not None:
-        message_filter["room"]["timeline"]["limit"] = limit
-
-    if room_event_filter:
-        room_filter = message_filter["room"]["timeline"]
-        room_filter["request_id"] = message_filter["request_id"]
-        return room_filter
-
-    return message_filter
-
-
-def create_sync_filter(
-    room_id: str,
-    types: list = [],
-    not_types: list = [],
-    limit: Optional[int] = None,
-    not_senders: list = [],
-):
-    """
-    Creates a filter that works with the sync endpoint.
-    """
-    return create_filter(
-        room_id, types=types, not_types=not_types, limit=limit, not_senders=not_senders
-    )
 
 
-def create_room_message_filter(
-    room_id: str,
-    types: list = [],
-    not_types: list = [],
-    limit: Optional[int] = None,
-    not_senders: list = [],
-):
+async def get_sync_token(client: FractalAsyncClient) -> str:
     """
-    Creates a filter that works with the room_messages endpoint.
+    Runs an empty sync request and returns the next_batch token.
     """
-    return create_filter(
-        room_id,
-        types=types,
-        not_types=not_types,
-        limit=limit,
-        not_senders=not_senders,
-        room_event_filter=True,
-    )
-
-
-def _get_content_only(event: Union[Event, BadEvent]):
-    content = event.source["content"]
-    content["sender"] = event.sender
-    content["event_id"] = event.event_id
-    return content
+    res = await client.sync(timeout=0, sync_filter=EMPTY_FILTER, since=None)
+    if isinstance(res, SyncError):
+        raise Exception(res.message)
+    return res.next_batch
 
 
 async def run_sync_filter(
     client: FractalAsyncClient,
     filter: dict,
     timeout: int = 30000,
     since: Optional[str] = None,
     content_only: bool = True,
     **kwargs,
 ) -> Dict[str, Any]:
     """
     Execute a filter with the provided client, optionally filter message body by kwargs
     attempts to deserialize json
     """
+
+    def get_content_only(event):
+        content = event.source["content"]
+        content["sender"] = event.sender
+        return content
+
     if since is None:
-        client.next_batch = None  # type:ignore
+        client.next_batch = None
 
     res = await client.sync(timeout=timeout, sync_filter=filter, since=since)
     if isinstance(res, SyncError):
         raise Exception(res.message)
 
     rooms = list(res.rooms.join.keys())
+    filter_keys = kwargs.keys()
     d = {}
     for room in rooms:
         if content_only:
-            d[room] = [_get_content_only(event) for event in res.rooms.join[room].timeline.events]
+            d[room] = [get_content_only(event) for event in res.rooms.join[room].timeline.events]
         else:
             d[room] = [event.source for event in res.rooms.join[room].timeline.events]
 
+    if kwargs:
+        # filter out all keys by value from kwargs
+        for key in filter_keys:
+            d = {k: [i for i in v if i.get(key) == kwargs[key]] for k, v in d.items()}
     return d
 
 
-async def run_room_message_filter(
-    client: FractalAsyncClient,
-    room_id: str,
-    filter: dict,
-    since: Optional[str] = None,
-    content_only: bool = True,
-    direction: MessageDirection = MessageDirection.front,
-    limit: int = 100,
-) -> Tuple[Dict[str, Any], Optional[str]]:
-    """
-    Execute a room message request with the provided client attempts to deserialize json
-    """
-    since = since or ""
-
-    end = None
-
-    if direction == MessageDirection.back:
-        end = ""
-
-    res = await client.room_messages(
-        room_id,
-        start=since,
-        end=end,
-        limit=limit,
-        direction=direction,
-        message_filter=filter,
-    )
-    if isinstance(res, RoomMessagesError):
-        raise Exception(res.message)
-
-    d = {}
-    if res.chunk:
-        if content_only:
-            d[room_id] = [_get_content_only(event) for event in res.chunk]
-        else:
-            d[room_id] = [event.source for event in res.chunk]
-
-    if direction == MessageDirection.back:
-        return d, res.start
-    else:
-        return d, res.end
-
-async def get_first_unacked_task(
-    tasks: list[Dict[str, Any]], task_types: "TaskTypes"
-) -> Dict[str, Any]:
+async def get_first_unacked_task(tasks: list[Dict[str, Any]]) -> Dict[str, Any]:
     """
     Returns the first task object that has not been acknowledged.
     """
     task_dict = {}
     task_order = []
 
     for task in tasks:
         task_body = task["content"]["body"]
         task_id = task_body["task_id"]
 
         # add task id to order list if its not already there
         if task_id not in task_order:
             task_order.append(task_id)
 
-        if task["content"]["msgtype"] == task_types.task:
+        if task["content"]["msgtype"].startswith("taskiq.task"):
             if task_id not in task_dict:
                 # add task to dictionary and initially mark it as unacknowledged
                 task_dict[task_id] = {"task_data": task, "acknowledged": False}
 
             else:
                 # task already exists in dictionary (weve seen an ack for it)
                 # simply update the task's data
                 task_dict[task_id]["task_data"] = task
 
-        elif task["content"]["msgtype"].startswith(task_types.ack):
+        elif task["content"]["msgtype"].startswith("taskiq.ack"):
             if task_id in task_dict:
                 # mark the task as acknowledged if it exists in the task dictionary
                 task_dict[task_id]["ack_data"] = task
                 task_dict[task_id]["acknowledged"] = True
 
             # if the task doesnt exist in the dictionary, add it in as acknowledged
             # this handles the case where the ack is somehow ahead of the task request
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/lock.py` & `taskiq_matrix-0.1.0/taskiq_matrix/lock.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     MessageDirection,
     RoomMessagesError,
     RoomSendResponse,
     SyncError,
 )
 
 from .exceptions import LockAcquireError
-from .filters import create_room_message_filter, run_room_message_filter
+from .filters import create_filter
 from .utils import setup_console_logging
 
 logger = logging.getLogger(__name__)
 
 
 class MatrixLock:
     """
@@ -46,30 +46,33 @@
 
         self.client = FractalAsyncClient(
             homeserver_url=homeserver_url, access_token=access_token, room_id=room_id
         )
         self.client.access_token = access_token
         self.room_id = room_id
         self.lock_id = str(uuid4())
-        self.next_batch = None
+        if MatrixLock.next_batch:
+            self.next_batch = MatrixLock.next_batch
+        else:
+            self.next_batch = None
         setup_console_logging()
 
     def create_filter(
         self, room_id: Optional[str] = None, types: List[str] = [], limit: Union[int, None] = None
     ) -> dict:
         """
         Create a filter for a room and/or specific message types.
 
         Returns:
             filter dict
         """
         if not room_id:
             room_id = self.room_id
 
-        return create_room_message_filter(room_id, types=types, limit=limit)
+        return create_filter(room_id, types=types, limit=limit)
 
     async def send_message(
         self,
         message: Union[bytes, str, Dict[Any, Any]],
         msgtype: str = "m.room.message",
         room: Optional[Union[MatrixRoom, str]] = None,
     ) -> bool:
@@ -151,73 +154,72 @@
         """
         acquire a lock on a specific key
         Args:
             key (str): the key to lock on
             wait (bool): whether to wait for the lock to be available
         """
         lock_types = [f"fn.lock.acquire.{key}", f"fn.lock.release.{key}"]
-        # because we create a new instance of a lock each time, we cache
-        # a next batch that we can use for subsequent invocations of locks.
-        # FIXME: this should be advanced
-        res, next_batch = await self.filter(
-            self.create_filter(types=lock_types), limit=1, message_direction=MessageDirection.back
+        if not self.next_batch:
+            self.next_batch = await self.get_latest_sync_token()
+            MatrixLock.next_batch = self.next_batch
+        res = await self.filter(
+            self.create_filter(types=lock_types), timeout=0, since=self.next_batch
         )
-        self.next_batch = next_batch
+        self.next_batch = self.client.next_batch
 
         # if last event is a lock release or the lock types dont exist in the room,
         # we can acquire the lock
-        if self.room_id not in res or res[self.room_id][0]["type"] == f"fn.lock.release.{key}":
+        if self.room_id not in res or res[self.room_id][-1]["type"] == f"fn.lock.release.{key}":
             await self.send_message(
                 {"type": f"fn.lock.acquire.{key}", "lock_id": self.lock_id},
                 msgtype=f"fn.lock.acquire.{key}",
             )
 
             # filter again to make sure that we got the lock
-            # all mutex tasks from the beginning of room history will be returned, we should
-            # figure out a way to optomize this
-            res, _ = await self.filter(self.create_filter(types=[f"fn.lock.acquire.{key}"]))
+            res = await self.filter(self.create_filter(types=[f"fn.lock.acquire.{key}"]))
             if res[self.room_id] and res[self.room_id][0]["lock_id"] == self.lock_id:
                 return True
             else:
                 logger.info(
                     f'Unable to acquire lock {key}, worker {res[self.room_id][0]["lock_id"]} got it.'
                 )
                 return False
         else:
             return False
 
     async def filter(
-        self,
-        filter: dict,
-        limit: int = 100,
-        message_direction: MessageDirection = MessageDirection.front,
-    ) -> tuple[Dict[str, Any], Optional[str]]:
+        self, filter: dict, timeout: int = 3000, since: Optional[str] = None, **kwargs
+    ) -> Dict[str, Any]:
         """
         execute a filter with the client, optionally filter message body by kwargs
         attempts to deserialize json
         """
         logger.debug("Next batch is %s" % self.next_batch)
-        result, next_batch = await run_room_message_filter(
-            self.client,
-            self.room_id,
-            filter,
-            since=self.next_batch,
-            content_only=True,
-            direction=message_direction,
-        )
-        rooms = list(result.keys())
+        res = await self.client.sync(timeout, sync_filter=filter, since=self.next_batch)
+        if isinstance(res, SyncError):
+            raise Exception(res.message)
+
+        rooms = list(res.rooms.join.keys())
+        filter_keys = kwargs.keys()
         d = {}
         for room in rooms:
             d[room] = list(
                 map(
                     json.loads,
-                    [event["body"] for event in result[room]],
+                    [
+                        event.source["content"]["body"]
+                        for event in res.rooms.join[room].timeline.events
+                    ],
                 )
             )
-        return d, next_batch
+        if kwargs:
+            # filter out all keys by value from kwargs
+            for key in filter_keys:
+                d = {k: [i for i in v if i.get(key) == kwargs[key]] for k, v in d.items()}
+        return d
 
     async def get_latest_sync_token(self) -> str:
         """
         Returns the latest sync token for a room in constant time, using /sync with an empty filter takes longer as the room grows
         """
         res = await self.client.room_messages(
             self.room_id, start="", limit=1, direction=MessageDirection.back
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/matrix_broker.py` & `taskiq_matrix-0.1.0/taskiq_matrix/matrix_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import asyncio
 import itertools
 import json
 import logging
 import os
 import socket
-from typing import Any, AsyncGenerator, List, Optional, Self, TypeVar, Union
+from typing import Any, AsyncGenerator, List, Optional, Self, TypeVar
 from uuid import uuid4
 
 from fractal.matrix.async_client import FractalAsyncClient
 from nio import RoomGetStateEventError, RoomPutStateError
 from taskiq import AckableMessage, AsyncBroker, AsyncResultBackend, BrokerMessage
 
 from .exceptions import (
     DeviceQueueRequiresDeviceLabel,
     LockAcquireError,
     ScheduledTaskRequiresTaskIdLabel,
 )
+from .filters import EMPTY_FILTER, run_sync_filter
 from .lock import MatrixLock
 from .matrix_queue import BroadcastQueue, MatrixQueue, ReplicatedQueue, Task
 from .matrix_result_backend import MatrixResultBackend
 from .schedulesource import SCHEDULE_STATE_TYPE
 from .utils import send_message
 
 logging.getLogger("nio").setLevel(logging.WARNING)
@@ -31,86 +32,59 @@
 
 class MatrixBroker(AsyncBroker):
     device_queue: MatrixQueue
     broadcast_queue: BroadcastQueue
     mutex_queue: MatrixQueue
     replication_queue: ReplicatedQueue
     result_backend: MatrixResultBackend
-    room_id: str
-    homeserver_url: str
-    access_token: str
 
     def __init__(
         self,
         result_backend: Optional[AsyncResultBackend] = None,
         task_id_generator: Any = None,
+        room_id: Optional[str] = None,
     ) -> None:
         """
         A taskiq broker backed by the Matrix protocol.
 
         A MatrixBroker is comprised of four independent task queues:
 
         - device_queue: a device's independent queue of tasks that are
         to be executed by only that device
         - broadcast_queue: a queue of tasks that should be executed
         by all devices in a room (group)
         - mutex_queue: a queue of tasks that should be run by any (only one)
         device in a group
         - replication_queue: a queue of tasks that should be run by each device
+        Requires the following environment variables to be set:
+        - MATRIX_HOMESERVER_URL
+        - MATRIX_ACCESS_TOKEN
+        - MATRIX_ROOM_ID (if room_id not provided as an argument)
 
         NOTE: Rate limiting for the configured user should be disabled:
         `insert into ratelimit_override values ("@mjolnir:my-homeserver.chat", 0, 0);`
         https://github.com/matrix-org/synapse/issues/6286#issuecomment-646944920
 
         TODO: Figure out how to dynamically register queues.
         """
         super().__init__(result_backend=result_backend, task_id_generator=task_id_generator)
+        try:
+            os.environ["MATRIX_HOMESERVER_URL"]
+            os.environ["MATRIX_ACCESS_TOKEN"]
+            self.room_id = room_id or os.environ["MATRIX_ROOM_ID"]
+        except KeyError as e:
+            raise KeyError(f"Missing required environment variable: {e}")
 
         self.device_name = os.environ.get("MATRIX_DEVICE_NAME", socket.gethostname())
+        self.mutex_queue = MatrixQueue("mutex", room_id=self.room_id)
+        self.device_queue = MatrixQueue(f"device.{self.device_name}", room_id=self.room_id)
+        self.broadcast_queue = BroadcastQueue("broadcast", room_id=self.room_id)
+        self.replication_queue = ReplicatedQueue("replication", room_id=self.room_id)
         self.worker_id = uuid4().hex
 
-    def with_matrix_config(self, room_id: str, homeserver_url: str, access_token: str) -> Self:
-        self.room_id = room_id
-        self.homeserver_url = homeserver_url
-        self.access_token = access_token
-        return self
-
-    def _init_queues(self):
-        try:
-            if not all([self.room_id, self.homeserver_url, self.access_token]):
-                raise Exception("Matrix config must be set with with_matrix_config.")
-        except:
-            raise Exception("Matrix config must be set with with_matrix_config.")
-
-        if not hasattr(self, "mutex_queue"):
-            self.mutex_queue = MatrixQueue(
-                "mutex",
-                homeserver_url=self.homeserver_url,
-                access_token=self.access_token,
-                room_id=self.room_id,
-            )
-            self.device_queue = MatrixQueue(
-                f"device.{self.device_name}",
-                homeserver_url=self.homeserver_url,
-                access_token=self.access_token,
-                room_id=self.room_id,
-            )
-            self.broadcast_queue = BroadcastQueue(
-                "broadcast",
-                homeserver_url=self.homeserver_url,
-                access_token=self.access_token,
-                room_id=self.room_id,
-            )
-            self.replication_queue = ReplicatedQueue(
-                "replication",
-                homeserver_url=self.homeserver_url,
-                access_token=self.access_token,
-                room_id=self.room_id,
-            )
-
     def with_result_backend(self, result_backend: AsyncResultBackend[_T]) -> Self:
         if not isinstance(result_backend, MatrixResultBackend):
             raise Exception("result_backend must be an instance of MatrixResultBackend")
 
         return super().with_result_backend(result_backend)
 
     async def add_mutex_checkpoint_task(self) -> bool:
@@ -134,16 +108,16 @@
         )
 
         if isinstance(schedules, RoomGetStateEventError):
             if schedules.status_code != "M_NOT_FOUND":
                 raise Exception(schedules.message)
 
             logger.info(
-                "No schedules found for room %s, will attempt to add checkpoint task",
-                self.mutex_queue.room_id,
+                f"No schedules found for room {self.mutex_queue.room_id}, will attempt to add checkpoint task",
+                "info",
             )
             content = {"tasks": [task]}
 
         # nio for some reason does not return a RoomGetStateEventError when
         # the user is not in the room (M_FORBIDDEN). Instead, the content
         # will be a dict with an "errcode" key.
         elif "errcode" in schedules.content:
@@ -162,15 +136,15 @@
             logger.debug(
                 f"Checkpoint task already exists in {self.mutex_queue.room_id} schedules"
             )
             return True
 
         # update schedule state to include checkpoint task
         try:
-            async with MatrixLock(room_id=self.mutex_queue.room_id).lock(SCHEDULE_STATE_TYPE):
+            async with MatrixLock().lock(SCHEDULE_STATE_TYPE):
                 logger.info(f"Adding checkpoint task to {self.mutex_queue.room_id} schedules")
                 res = await self.mutex_queue.client.room_put_state(
                     self.mutex_queue.room_id,
                     SCHEDULE_STATE_TYPE,
                     content,
                 )
                 if isinstance(res, RoomPutStateError):
@@ -178,79 +152,70 @@
                     return False
                 else:
                     return True
         except LockAcquireError as e:
             logger.error(f"{e}\n\n")
             return False
 
-    async def update_checkpoints(self, interval: int = 60):
+    async def update_device_checkpoints(self, interval: int = 60):
         """
-        Background task that periodically updates the device, broadcast,
-        and replication queue checkpoints.
+        Background task that periodically updates the device and broadcast
+        queue checkpoints.
+
+        Note: Figure out how to test block of code in infinite loop.
+            The infinite loop makes this currently untestable
 
         Args:
             interval (int): The interval in seconds to update the checkpoints.
                             Defaults to 60 seconds.
         """
         from .tasks import update_checkpoint
 
-        try:
-            while True:
-                try:
-                    # run both updates in parallel
-                    await asyncio.gather(
-                        update_checkpoint("device"),
-                        update_checkpoint("broadcast"),
-                        update_checkpoint("replication"),
-                    )
-                except Exception as err:
-                    logger.error("Encountered error in update_device_checkpoint: %s", err)
+        while True:
+            try:
+                # run both updates in parallel
+                await asyncio.gather(
+                    update_checkpoint("device"),
+                    update_checkpoint("broadcast"),
+                    update_checkpoint("replication"),
+                )
+            except Exception as err:
+                logger.warn(f"update_device_checkpoints: {err}")
 
-                await asyncio.sleep(interval)
-        except asyncio.CancelledError:
-            return None
+            await asyncio.sleep(interval)
 
     async def startup(self) -> None:
         """
         Starts up the broker by connecting to the matrix server and
         performing an initial sync.
 
         Will exit if the initial sync fails or the provided room is not found.
         """
         logger.info("Starting Taskiq Matrix Broker")
         await super().startup()
 
-        self._init_queues()
-
         # create and initialize queues
         await self.device_queue.checkpoint.get_or_init_checkpoint()
         await self.broadcast_queue.checkpoint.get_or_init_checkpoint()
         await self.mutex_queue.checkpoint.get_or_init_checkpoint()
-        # full sync is required for replication queue because it needs to
-        # sync any tasks that were sent before the checkpoint was created for
-        # this device
-        await self.replication_queue.checkpoint.get_or_init_checkpoint(full_sync=True)
+        await self.replication_queue.checkpoint.get_or_init_checkpoint()
 
         # ensure that checkpoint schedule task is added to schedules
         await self.add_mutex_checkpoint_task()
 
-        # launch background task that updates device checkpoints
-        self.checkpoint_updater = asyncio.create_task(self.update_checkpoints())
+        # launch brackground task that updates device checkpoints
+        asyncio.create_task(self.update_device_checkpoints())
 
         return None
 
     async def shutdown(self) -> None:
         """
         Shuts down the broker.
         """
         logger.info("Shutting down the broker")
-        if hasattr(self, "checkpoint_updater"):
-            self.checkpoint_updater.cancel()
-            await self.checkpoint_updater
-
         await self.device_queue.shutdown()
         await self.broadcast_queue.shutdown()
         await self.mutex_queue.shutdown()
         await self.replication_queue.shutdown()
         return await super().shutdown()
 
     def _use_task_id(self, task_id: str, message: BrokerMessage) -> BrokerMessage:
@@ -279,43 +244,34 @@
         message.message = message_body
         return message
 
     async def kick(self, message: BrokerMessage) -> None:
         """
         Kicks a task into the broker.
         """
-
-        room_id = message.labels.get("room_id")
-
-        self._init_queues()
-
-        queue_name = message.labels.get("queue", "mutex")
-        device_name = message.labels.get("device")
-        queue: MatrixQueue = (
-            self.device_queue if device_name else getattr(self, f"{queue_name}_queue")
-        )
-        if not room_id:
-            room_id = queue.room_id
-
         # populate next batch on the result backend client to avoid result delay
         if (
             isinstance(self.result_backend, MatrixResultBackend)
             and not self.result_backend.matrix_client.next_batch
         ):
-            since_token = await self.result_backend.matrix_client.get_latest_sync_token(
-                room_id=room_id
-            )
+            since_token = await self.result_backend.matrix_client.get_latest_sync_token()
             self.result_backend.matrix_client.next_batch = since_token
 
+        queue_name = message.labels.get("queue", "mutex")
+        device_name = message.labels.get("device")
+        queue: MatrixQueue = (
+            self.device_queue if device_name else getattr(self, f"{queue_name}_queue")
+        )
         # use a fresh new client here because kicking a task can sometimes be from
         # an ephemeral event loop
         client = FractalAsyncClient(
-            homeserver_url=self.homeserver_url,
-            access_token=self.access_token,
+            homeserver_url=os.environ["MATRIX_HOMESERVER_URL"],
+            access_token=os.environ["MATRIX_ACCESS_TOKEN"],
         )
+        room_id = message.labels.get("room_id", queue.room_id)
 
         if queue == self.device_queue:
             if not device_name:
                 raise DeviceQueueRequiresDeviceLabel(message.task_id)
             msgtype = queue.task_types.device_task(device_name)
             queue_name = "device"
         else:
@@ -327,15 +283,15 @@
             # is provided in the schedule. This ensures that the task
             # is only kicked once.
             task_id = message.labels.get("task_id")
             if not task_id:
                 raise ScheduledTaskRequiresTaskIdLabel(message.task_id)
 
             try:
-                async with MatrixLock(room_id=room_id).lock(f"{queue.task_types.task}.{task_id}"):
+                async with MatrixLock().lock(f"{queue.task_types.task}.{task_id}"):
                     # generate a new unique task id for the message
                     task_id = self.id_generator()
                     message = self._use_task_id(task_id, message)
                     message_body = message.message
                     await send_message(
                         client,
                         room_id,
@@ -361,59 +317,61 @@
             message_body,
             msgtype=msgtype,
             task_id=message.task_id,
             queue=queue_name,
         )
         return await client.close()
 
-    async def get_tasks(self) -> AsyncGenerator[List[Task], Any]:  # pragma: no cover
+    async def get_tasks(self) -> AsyncGenerator[List[Task], Any]:
         while True:
             tasks = {
-                "device_queue": asyncio.create_task(
-                    self.device_queue.get_unacked_tasks(), name="device_queue"
+                self.device_queue.name: asyncio.create_task(
+                    self.device_queue.get_unacked_tasks(), name=self.device_queue.name
                 ),
-                "broadcast_queue": asyncio.create_task(
-                    self.broadcast_queue.get_unacked_tasks(), name="broadcast_queue"
+                self.broadcast_queue.name: asyncio.create_task(
+                    self.broadcast_queue.get_unacked_tasks(), name=self.broadcast_queue.name
                 ),
-                "mutex_queue": asyncio.create_task(
-                    self.mutex_queue.get_unacked_tasks(), name="mutex_queue"
+                self.mutex_queue.name: asyncio.create_task(
+                    self.mutex_queue.get_unacked_tasks(), name=self.mutex_queue.name
                 ),
-                "replication_queue": asyncio.create_task(
+                self.replication_queue.name: asyncio.create_task(
                     self.replication_queue.get_unacked_tasks(exclude_self=True),
-                    name="replication_queue",
+                    name=self.replication_queue.name,
                 ),
             }
-            sync_task_results: List[List[Task]] = []
+            sync_tasks = [
+                tasks[self.device_queue.name],
+                tasks[self.broadcast_queue.name],
+                tasks[self.mutex_queue.name],
+                tasks[self.replication_queue.name],
+            ]
 
-            while tasks:
-                done, _ = await asyncio.wait(tasks.values(), return_when=asyncio.FIRST_COMPLETED)
-
-                for completed_task in done:
-                    queue_name = completed_task.get_name()
-                    try:
-                        queue, pending_tasks = completed_task.result()
-                        if pending_tasks:
-                            sync_task_results.append(pending_tasks)
-                            logger.debug(f"Got {len(pending_tasks)} tasks from {queue}")
-                    except Exception as e:
-                        logger.error(f"Sync failed: {e}")
-
-                    # Reschedule a new task for the completed queue
-                    tasks[queue_name] = asyncio.create_task(
-                        getattr(self, queue_name).get_unacked_tasks(), name=queue_name
-                    )
+            done, pending = await asyncio.wait(sync_tasks, return_when=asyncio.FIRST_COMPLETED)
 
-                if sync_task_results:
-                    yield list(itertools.chain.from_iterable(sync_task_results))
-                    sync_task_results = []  # Reset for the next iteration
-
-                # Optionally, add a short delay before starting the next round
-                await asyncio.sleep(0)
+            sync_task_results: List[List[Task]] = []
+            for completed_task in done:
+                try:
+                    queue, pending_tasks = completed_task.result()
+                    if pending_tasks:
+                        sync_task_results.append(pending_tasks)
+                        logger.debug(f"Got {len(pending_tasks)} tasks from {queue}")
+                except Exception as e:
+                    logger.error(f"Sync failed: {e}")
+                    raise e
+            for pending_task in pending:
+                if pending_task.done():
+                    queue, pending_tasks = pending_task.result()
+                    if pending_tasks:
+                        logger.debug(f"Got {len(pending_tasks)} tasks from {queue}")
+                        sync_task_results.append(pending_tasks)
+                else:
+                    pending_task.cancel()
+            yield list(itertools.chain.from_iterable(sync_task_results))
 
-    async def listen(self) -> AsyncGenerator[Union[AckableMessage, bytes], Any]:
+    async def listen(self) -> AsyncGenerator[AckableMessage, Any]:
         """
         Listen Matrix for new messages.
 
         This function sends sync requests to the Matrix server
         and yields all "taskiq.task" events.
 
         :yields: broker messages.
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/matrix_queue.py` & `taskiq_matrix-0.1.0/taskiq_matrix/matrix_queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import json
 import logging
 import os
 import socket
 from functools import partial
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple
 
 from fractal.matrix.async_client import FractalAsyncClient
 from nio import (
     MessageDirection,
     RoomGetStateEventError,
     RoomMessagesResponse,
     RoomPutStateError,
     WhoamiError,
 )
 from taskiq import AckableMessage
 
 from .exceptions import CheckpointGetOrInitError, LockAcquireError, TaskAlreadyAcked
-from .filters import (
-    create_room_message_filter,
-    create_sync_filter,
-    run_room_message_filter,
-    run_sync_filter,
-)
+from .filters import create_filter, run_sync_filter
 from .lock import MatrixLock
 from .utils import send_message
 
 logger = logging.getLogger(__name__)
 
 
 class TaskTypes:
@@ -35,15 +30,15 @@
 
     def __init__(self, queue_name: str):
         self.task = f"taskiq.{queue_name}.task"
         self.ack = f"{self.task}.ack"
         self.result = "taskiq.result"
         self.lock = f"{self.task}.lock"
 
-    def all(self) -> List[str]: # pragma: no cover
+    def all(self) -> List[str]:
         """
         Returns the task types for the queue.
         """
         return [f"{self.task}", f"{self.ack}", f"{self.result}"]
 
     def device_task(self, device_name: str) -> str:
         """
@@ -97,15 +92,23 @@
         since_token: Optional[str] = None,
     ):
         self.type = type
         self.room_id = room_id
         self.client = client
         self.since_token = since_token
 
-    async def get_or_init_checkpoint(self, full_sync: bool = False) -> Optional[str]:
+        # initialize checkpoint
+        # loop = asyncio.new_event_loop()
+        # https://stackoverflow.com/questions/46827007/runtimeerror-this-event-loop-is-already-running-in-python/56434301#56434301
+        # nest_asyncio.apply()
+        # FIXME: This breaks pytest-asyncio tests (POSSIBLY?)
+        # self.task = loop.create_task(self.get_or_init_checkpoint())
+        # loop.run_until_complete(self.get_or_init_checkpoint())
+
+    async def get_or_init_checkpoint(self) -> Optional[str]:
         """
         Gets the current checkpoint from the Matrix server. If it doesn't exist,
         it will be initialized.
 
         Returns:
             The current checkpoint or None if not found in room state.
         """
@@ -114,21 +117,19 @@
             if resp.status_code != "M_NOT_FOUND":
                 raise Exception(resp.message)
 
             # checkpoint state wasn't found, so initialize it
             logger.debug(f"No checkpoint found for type: {self.type}")
 
             # fetch latest sync token
-            # if full_sync is false, then we fetch the latest sync token
-            # if full_sync is true, then we get a sync token from the beginning of the room's timeline
             res = await self.client.room_messages(
                 self.room_id,
                 start="",
                 limit=1,
-                direction=MessageDirection.back if not full_sync else MessageDirection.front,
+                direction=MessageDirection.back,
             )
             if not isinstance(res, RoomMessagesResponse):
                 raise CheckpointGetOrInitError(self.type)
             # update the checkpoint state in the Matrix room
             await self.put_checkpoint_state(res.start)
 
             self.since_token = res.start
@@ -143,15 +144,15 @@
         Sets the current checkpoint on the Matrix server.
 
         Returns:
             True if the checkpoint was set, else False.
         """
         # acquire lock on checkpoint
         try:
-            async with MatrixLock(room_id=self.room_id).lock(key=self.type):
+            async with MatrixLock().lock(key=self.type):
                 logger.debug(f"Setting checkpoint for type {self.type}")
                 # set checkpoint
                 resp = await self.client.room_put_state(
                     self.room_id,
                     self.type,
                     {"checkpoint": since_token},
                 )
@@ -159,15 +160,15 @@
                     logger.error(f"Failed to set checkpoint for type {self.type}: {resp}")
                     return False
                 else:
                     self.since_token = since_token
                     return True
 
         except LockAcquireError as e:
-            logger.info(f"Failed to set checkpoint: {e}\n")
+            logger.debug(f"Failed to set checkpoint: {e}\n")
             return False
 
     @classmethod
     async def create(cls, type: str, client: FractalAsyncClient, room_id: str) -> "Checkpoint":
         """
         Create a Checkpoint instance for the given type.
         """
@@ -187,98 +188,73 @@
     client: FractalAsyncClient
     checkpoint: Checkpoint
     task_types: TaskTypes
 
     def __init__(
         self,
         name: str,
-        homeserver_url: str,
-        access_token: str,
-        room_id: str,
+        homeserver_url: str = os.environ.get("MATRIX_HOMESERVER_URL", ""),
+        access_token: str = os.environ.get("MATRIX_ACCESS_TOKEN", ""),
+        room_id: str = os.environ.get("MATRIX_ROOM_ID", ""),
         device_name: str = os.environ.get("MATRIX_DEVICE_NAME", socket.gethostname()),
     ):
+        if not homeserver_url:
+            raise Exception(
+                "MatrixQueue requires MATRIX_HOMESERVER_URL environment variable set if not passed explicitly"
+            )
+        if not access_token:
+            raise Exception(
+                "MatrixQueue requires MATRIX_ACCESS_TOKEN environment variable set if not passed explicitly"
+            )
+        if not room_id:
+            raise Exception(
+                "MatrixQueue requires MATRIX_ROOM_ID environment variable set if not passed explicitly"
+            )
+
         self.client = FractalAsyncClient(
             homeserver_url=homeserver_url, access_token=access_token, room_id=room_id
         )
         self.name = name
         self.checkpoint = Checkpoint(type=name, client=self.client, room_id=room_id)
         self.task_types = TaskTypes(name)
         self.device_name = device_name
         self.room_id = room_id
-        # Boolean that determines whether the queue is caught up with the room's timeline
-        # This is used to determine whether to use the room_messages API or the sync API
-        self.caught_up = False
 
     async def verify_room_exists(self) -> None:
         """
         Verifies that the configured room exists
         """
         # verify room exists by fetching a piece of its room state
         res = await self.client.room_get_state_event(self.room_id, "m.room.create")
         if isinstance(res, RoomGetStateEventError):
             raise Exception(f"Matrix room {self.room_id} not found: {res.message}")
 
     async def get_tasks(
-        self,
-        timeout: int = 30000,
-        since_token: Optional[str] = None,
-        task_filter: Optional[Dict[str, Any]] = None,
+        self, timeout: int = 30000, since_token: Optional[str] = None
     ) -> list[Task]:
         """
         Returns a list of tasks and acks.
 
         Args:
             timeout (int): The timeout to use when fetching tasks.
             since_token (str): The next batch token to use when fetching tasks.
                                Defaults to the current checkpoint of the broker.
-            task_fitler (dict): A filter to use when fetching tasks. Defaults to
-                                a filter that fetches all tasks and acks for the
-                                queue.
 
         Returns:
             A list of tasks and acks.
         """
         next_batch = since_token or self.checkpoint.since_token
 
-        if not task_filter:
-            if self.caught_up:
-                task_filter = create_sync_filter(
-                    self.room_id,
-                    types=[self.task_types.task, f"{self.task_types.ack}.*"],
-                )
-            else:
-                task_filter = create_room_message_filter(
-                    self.room_id,
-                    types=[self.task_types.task, f"{self.task_types.ack}.*"],
-                )
-
-        if self.caught_up:
-            task_events = await run_sync_filter(
-                self.client, task_filter, timeout=timeout, since=next_batch
-            )
-        else:
-            task_events, end = await run_room_message_filter(
-                self.client, self.room_id, task_filter, since=next_batch
-            )
-            if not end:
-                self.caught_up = True
-                # finished processing all events in the room, so use the sync API
-                # to get new events from now on
-                self.client.next_batch = await self.client.get_latest_sync_token(self.room_id)
-                logger.info(
-                    f"Caught up - Updating checkpoint in room to: {self.client.next_batch}"
-                )
-                await self.checkpoint.put_checkpoint_state(self.client.next_batch)
-                return await self.get_tasks(timeout=timeout)
-            else:
-                logger.info(f"Still catching up - Updating checkpoint to {end}")
-                self.checkpoint.since_token = end
-
-        # acks should be a separate type
-        # tasks should only be tasks
+        task_filter = create_filter(
+            self.room_id,
+            types=[self.task_types.task, f"{self.task_types.ack}.*"],
+        )
+        task_events = await run_sync_filter(
+            self.client, task_filter, timeout=timeout, since=next_batch
+        )
         tasks = [Task(**task) for task in task_events.get(self.room_id, [])]
         return tasks
 
     def filter_acked_tasks(self, tasks: list["Task"], exclude_self: bool = False) -> list["Task"]:
         """
         Filter out all events that have been acked
 
@@ -306,16 +282,14 @@
                 # if exclude_self is False, then append any unacked task
                 if not exclude_self:
                     unacked.append(task)
                 # if exclude_self is True, then filter out tasks that were sent by us
                 # since we don't want to run tasks that we sent
                 elif task.sender != self.client.user_id:
                     unacked.append(task)
-                else:
-                    logger.warning(f"Filtering out task {task.id} sent by {task.sender}")
 
         logger.debug(f"{self.name} Unacked tasks: {unacked}")
         return unacked
 
     async def get_unacked_tasks(
         self, timeout: int = 30000, exclude_self: bool = False
     ) -> Tuple[str, List[Task]]:
@@ -337,40 +311,36 @@
         if not self.client.user_id:
             whoami = await self.client.whoami()
             if isinstance(whoami, WhoamiError):
                 raise Exception(whoami.message)
 
         tasks = await self.get_tasks(timeout=timeout, since_token=self.checkpoint.since_token)
         unacked = self.filter_acked_tasks(tasks, exclude_self=exclude_self)
-        if not unacked:
-            logger.debug(f"No unacked tasks found for queue: {self.name}")
-
         return self.name, unacked
 
     async def all_tasks_acked(self) -> bool:
         """
         Returns a boolean for all tasks being acked or not.
         """
-        unacked_tasks = await self.get_unacked_tasks(timeout=0)
+        unacked_tasks = await self.get_unacked_tasks()
         return len(unacked_tasks[1]) == 0
 
     async def task_is_acked(self, task_id: str, since: Optional[str] = None) -> bool:
         """
         Returns a boolean for a task being acked or not.
         """
         next_batch = since or self.checkpoint.since_token
 
         # FIXME: Maybe this should be a method on a task type?
         queue_ack_type = self.task_types.ack
         expected_ack = f"{queue_ack_type}.{task_id}"
 
-        task_filter = create_room_message_filter(self.room_id, types=[expected_ack])
-        tasks, _ = await run_room_message_filter(
-            self.client, self.room_id, task_filter, since=next_batch
-        )
+        # attempt to fetch the given task_id's ack from the room
+        task_filter = create_filter(self.room_id, types=[expected_ack])
+        tasks = await run_sync_filter(self.client, task_filter, timeout=0, since=next_batch)
 
         # if anything for the room was returned, then the task was acked
         return tasks.get(self.room_id) is not None
 
     async def ack_msg(self, task_id: str) -> None:
         """
         Acks a given task id.
@@ -389,65 +359,47 @@
             self.room_id,
             message=message,
             msgtype=f"{self.task_types.ack}.{task_id}",
             task_id=task_id,
             queue=self.name,
         )
 
-    async def yield_task(
-        self,
-        task: Task,
-        ignore_acks: bool = False,
-        lock: bool = True,
-    ) -> Union[AckableMessage, bytes]:
+    async def yield_task(self, task: Task) -> AckableMessage:
         """
         Attempts to lock a task and yield it to a worker. If the lock is
         acquired and the task has been acked since the lock was acquired, then
         a TaskAlreadyAcked exception is raised.
 
         Args:
             task (Task): The task to yield.
-            ignore_acks (bool): If true, returns bytes.
-            lock (bool): If true, acquire a lock on the task id.
 
         Returns:
-            An AckableMessage or bytes containing the task data.
+            An AckableMessage containing the task data.
 
         Raises:
             LockAcquireError: If the lock could not be acquired.
             TaskAlreadyAcked: If the task has been acked since the lock was acquired.
         """
-
-        async def _yield_task():
+        async with MatrixLock().lock(f"{self.task_types.lock}.{task.id}"):
             # ensure that task has not been acked since lock was acquired
-            if not ignore_acks:
-                acked = await self.task_is_acked(task.id)
-                if acked:
-                    raise TaskAlreadyAcked(task.id)
+            acked = await self.task_is_acked(task.id)
+            if acked:
+                raise TaskAlreadyAcked(task.id)
 
             # encode task data
             task_data = json.dumps(task.data).encode("utf-8")
 
             logger.info(
                 f"Yielding message {task.data} for task {task.id} to worker {self.device_name}",
             )
-            if ignore_acks:
-                return task_data
-
             return AckableMessage(
                 data=task_data,
                 ack=partial(self.ack_msg, task.id),
             )
 
-        if not lock:
-            return await _yield_task()
-
-        async with MatrixLock(room_id=self.room_id).lock(f"{self.task_types.lock}.{task.id}"):
-            return await _yield_task()
-
     async def shutdown(self) -> None:
         """
         Closes the Queue's Matrix client session.
         """
         await self.client.close()
 
 
@@ -465,15 +417,22 @@
     """
     Replicated queues are broadcast queues whose checkpoints are device specific.
     """
 
     def __init__(
         self,
         name: str,
-        homeserver_url: str,
-        access_token: str,
-        room_id: str,
         *args,
+        homeserver_url: str = os.environ.get("MATRIX_HOMESERVER_URL", ""),
+        access_token: str = os.environ.get("MATRIX_ACCESS_TOKEN", ""),
+        room_id: str = os.environ.get("MATRIX_ROOM_ID", ""),
         **kwargs,
     ):
-        super().__init__(name, homeserver_url, access_token, room_id, *args, **kwargs)
+        super().__init__(
+            name,
+            *args,
+            homeserver_url=homeserver_url,
+            access_token=access_token,
+            room_id=room_id,
+            **kwargs,
+        )
         self.checkpoint.type = f"{self.checkpoint.type}.{self.device_name}"
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/matrix_result_backend.py` & `taskiq_matrix-0.1.0/taskiq_matrix/matrix_result_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 import logging
 import os
 import pickle
 import socket
 from base64 import b64decode, b64encode
-from typing import Any, Dict, Optional, TypeVar, Union
-from uuid import uuid4
+from typing import Dict, Optional, TypeVar, Union
 
-from async_lru import alru_cache
 from fractal.matrix.async_client import FractalAsyncClient
 from nio import MessageDirection, RoomMessagesError
 from taskiq import AsyncResultBackend
 from taskiq.result import TaskiqResult
 
 from .exceptions import (
     DuplicateExpireTimeSelectedError,
     ExpireTimeMustBeMoreThanZeroError,
     ResultDecodeError,
 )
-from .filters import create_room_message_filter, run_room_message_filter
+from .filters import create_filter, run_sync_filter
 from .utils import send_message
 
 _ReturnType = TypeVar("_ReturnType")
 
 
 logger = logging.getLogger(__name__)
 
 
 class MatrixResultBackend(AsyncResultBackend):
     def __init__(
         self,
-        homeserver_url: str,
-        access_token: str,
-        room_id: str,
         result_ex_time: Optional[int] = None,
         result_px_time: Optional[int] = None,
     ):
         """
         Constructs a new Matrix result backend.
 
         :param result_ex_time: expire time in seconds for result.
         :param result_px_time: expire time in milliseconds for result.
         """
-        self.room = room_id
-        self.homeserver_url = homeserver_url
-        self.access_token = access_token
         self.matrix_client = FractalAsyncClient(
-            homeserver_url=homeserver_url,
-            access_token=access_token,
-            room_id=self.room,
+            homeserver_url=os.environ["MATRIX_HOMESERVER_URL"],
+            access_token=os.environ["MATRIX_ACCESS_TOKEN"],
+            room_id=os.environ["MATRIX_ROOM_ID"],
         )
+        self.room = os.environ["MATRIX_ROOM_ID"]
         self.result_ex_time = result_ex_time
         self.result_px_time = result_px_time
         self.device_name = os.environ.get("MATRIX_DEVICE_NAME", socket.gethostname())
         self.next_batch: Optional[str] = None
 
         unavailable_conditions = any(
             (
@@ -105,48 +98,37 @@
         await send_message(
             self.matrix_client,
             self.room,
             message,
             msgtype=f"taskiq.result.{task_id}",
         )
 
-    @alru_cache(maxsize=64, ttl=60)
-    async def _fetch_result_from_matrix(self, task_id: str) -> dict[str, Any]:
-        """
-        Fetches task result from matrix. Caches the result for 60 seconds.
-
-        TODO: Handle waiting for a number of results for a task
-
-        :param task_id: ID of the task.
-        :return: list of task results.
-        """
-        message_filter = create_room_message_filter(self.room, types=[f"taskiq.result.{task_id}"])
-        result, next_batch = await run_room_message_filter(
-            self.matrix_client,
-            self.room,
-            message_filter,
-            since="",  # we can simply search the full room history since we are filtering by a specific type
-            direction=MessageDirection.back,
-        )
-        return result
-
     async def is_result_ready(self, task_id: str) -> bool:
         """
         Returns whether the result is ready.
 
         :param task_id: ID of the task.
 
         :returns: True if the result is ready else False.
         """
-        result = await self._fetch_result_from_matrix(task_id)
-        if not result.get(self.room):
-            # invalidate the cache if the result is not found
-            # we dont want to cache an empty result as it may
-            # be a temporary condition (the result hasn't been pushed yet)
-            self._fetch_result_from_matrix.cache_invalidate(task_id)
+        if not self.next_batch:
+            res = await self.matrix_client.room_messages(
+                self.room, start="", limit=1, direction=MessageDirection.back
+            )
+            if not isinstance(res, RoomMessagesError):
+                self.next_batch = res.start
+                self.matrix_client.next_batch = res.start
+
+        sync_filter = create_filter(self.room, types=[f"taskiq.result.{task_id}"])
+        # cache the next batch token from kick so we can use it later when getting the result
+        # need to do this because when we sync below here, the client's next_batch token will
+        # be updated to the latest sync token, which will be after the result we're looking for
+        result = await run_sync_filter(
+            self.matrix_client, sync_filter, timeout=0, since=self.matrix_client.next_batch
+        )
         return True if result.get(self.room) else False
 
     async def get_result(
         self,
         task_id: str,
         with_logs: bool = False,
     ) -> TaskiqResult[_ReturnType]:
@@ -156,15 +138,20 @@
         :param task_id: task's id.
         :param with_logs: if True it will download task's logs.
         :raises MatrixSyncError: if there is an error syncing with the Matrix server.
         :raises ResultIsMissingError: if there is no result when trying to get it.
         :raises ResultDecodeError: if there is an error decoding the result.
         :return: task's return value.
         """
-        result_object = await self._fetch_result_from_matrix(task_id)
+
+        sync_filter = create_filter(self.room, types=[f"taskiq.result.{task_id}"])
+        result_object = await run_sync_filter(
+            self.matrix_client, sync_filter, timeout=0, since=self.next_batch
+        )
+        # TODO: handle waiting for a number of results for a task
 
         try:
             result = result_object[self.room][0]
         except Exception as e:
             logger.error(f"Error getting task result from Matrix {e}")
             raise ResultDecodeError()
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/schedulesource.py` & `taskiq_matrix-0.1.0/taskiq_matrix/schedulesource.py`

 * *Files identical despite different names*

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/tasks.py` & `taskiq_matrix-0.1.0/taskiq_matrix/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from nio import RoomContextError
 
 from .exceptions import QueueDoesNotExist
 from .filters import create_filter, get_first_unacked_task, run_sync_filter
 from .instance import broker
-from .matrix_queue import MatrixQueue, ReplicatedQueue
+from .matrix_queue import MatrixQueue
 
 logger = logging.getLogger(__name__)
 
 
 @broker.task(task_name="taskiq.update_checkpoint", retry_on_error=True, labels={"queue": "mutex"})
 async def update_checkpoint(queue_name: str) -> bool:
     """
@@ -22,44 +22,40 @@
 
     Args:
         queue: The name of the queue on the broker to update the checkpoint for.
 
     Returns:
         True if checkpoint was successfully updated, False otherwise.
     """
-    broker._init_queues()
     try:
         queue: MatrixQueue = getattr(broker, f"{queue_name}_queue")
     except AttributeError:
         raise QueueDoesNotExist(f"Queue {queue_name} does not exist")
 
-    if isinstance(queue, ReplicatedQueue):
-        current_since_token = await queue.checkpoint.get_or_init_checkpoint(full_sync=True)
-    else:
-        current_since_token = await queue.checkpoint.get_or_init_checkpoint(full_sync=False)
+    current_since_token = await queue.checkpoint.get_or_init_checkpoint()
 
     logger.info(f"Running scheduled task update_checkpoint for queue: {queue.name}")
 
     # gets all tasks and acks since the checkpoint (including their event ids)
     # TODO: handle using results. Once we use them, we can use task_types.all()
     room_filter = create_filter(
-        queue.room_id, types=[queue.task_types.task, f"{queue.task_types.ack}.*"]
+        queue.room_id, types=[queue.task_types.task, queue.task_types.ack]
     )
     tasks = await run_sync_filter(
         queue.client,
         room_filter,
         since=current_since_token,
         content_only=False,
         timeout=0,
     )
 
     # pull tasks for the broker's room
     tasks = tasks.get(queue.room_id)
     if tasks:
-        unacked_task = await get_first_unacked_task(tasks, queue.task_types)
+        unacked_task = await get_first_unacked_task(tasks)
         if unacked_task:
             event_id = unacked_task["event_id"]
 
             # limit on 2 so that the "start" sync token is the event before the first unacked task
             context = await queue.client.room_context(queue.room_id, event_id, limit=2)
             if isinstance(context, RoomContextError):
                 raise Exception("Error fetching context: ", context.message)
```

### Comparing `taskiq_matrix-0.0.9/taskiq_matrix/utils.py` & `taskiq_matrix-0.1.0/taskiq_matrix/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 from typing import Any, Dict, Union
 
 from fractal.matrix.async_client import FractalAsyncClient
 from nio import RoomSendResponse
 
 logging.basicConfig(level=logging.WARNING)
```

### Comparing `taskiq_matrix-0.0.9/PKG-INFO` & `taskiq_matrix-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: taskiq-matrix
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Author: Mo Balaa
 Author-email: balaa@ether.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
-Requires-Dist: async-lru (>=2.0.4,<3.0.0)
 Requires-Dist: docker (>=6.1.3,<7.0.0) ; extra == "dev"
-Requires-Dist: fractal-matrix-client (>=0.0.1)
+Requires-Dist: fractal-matrix-client (>=0.1.0,<0.2.0)
 Requires-Dist: ipython (>=8.17.2,<9.0.0) ; extra == "dev"
 Requires-Dist: matrix-nio (>=0.22.1,<0.23.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0) ; extra == "dev"
 Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra == "dev"
-Requires-Dist: pytest-benchmark (>=4.0.0,<5.0.0) ; extra == "dev"
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "dev"
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0) ; extra == "dev"
 Requires-Dist: taskiq (>=0.10.4,<0.11.0)
 Description-Content-Type: text/markdown
 
-# taskiq-matrix
-
-A taskiq broker implementation powered by the Matrix protocol.
+# Taskiq Matrix
 
+A Matrix [protocol] powered broker for Taskiq.
```

