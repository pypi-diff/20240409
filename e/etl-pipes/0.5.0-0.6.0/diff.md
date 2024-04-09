# Comparing `tmp/etl_pipes-0.5.0.tar.gz` & `tmp/etl_pipes-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_pipes-0.5.0.tar", max compression
+gzip compressed data, was "etl_pipes-0.6.0.tar", max compression
```

## Comparing `etl_pipes-0.5.0.tar` & `etl_pipes-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.5.0/etl_pipes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.5.0/etl_pipes/actors/__init__.py
--rw-r--r--   0        0        0     2049 2024-03-31 18:15:41.761652 etl_pipes-0.5.0/etl_pipes/actors/actor.py
--rw-r--r--   0        0        0     8182 2024-03-31 18:15:41.762013 etl_pipes-0.5.0/etl_pipes/actors/actor_system.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.5.0/etl_pipes/actors/common/__init__.py
--rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.5.0/etl_pipes/actors/common/logging.py
--rw-r--r--   0        0        0     1434 2024-03-31 18:15:41.762619 etl_pipes-0.5.0/etl_pipes/actors/common/types.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.5.0/etl_pipes/common/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.5.0/etl_pipes/common/utils/__init__.py
--rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.5.0/etl_pipes/common/utils/type_hints.py
--rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.5.0/etl_pipes/context.py
--rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.5.0/etl_pipes/domain/__init__.py
--rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.5.0/etl_pipes/domain/types.py
--rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.5.0/etl_pipes/pipes/__init__.py
--rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.5.0/etl_pipes/pipes/base_pipe.py
--rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.5.0/etl_pipes/pipes/broadcast_parallel.py
--rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.5.0/etl_pipes/pipes/map_reduce.py
--rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.5.0/etl_pipes/pipes/maybe.py
--rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.5.0/etl_pipes/pipes/parallel.py
--rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/__init__.py
--rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/exceptions.py
--rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
--rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipeline.py
--rw-r--r--   0        0        0     1133 2024-04-08 19:43:30.227481 etl_pipes-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.6.0/etl_pipes/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.6.0/etl_pipes/actors/__init__.py
+-rw-r--r--   0        0        0     2102 2024-04-09 11:42:12.618153 etl_pipes-0.6.0/etl_pipes/actors/actor.py
+-rw-r--r--   0        0        0     8014 2024-04-09 11:42:12.618243 etl_pipes-0.6.0/etl_pipes/actors/actor_system.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.6.0/etl_pipes/actors/common/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.6.0/etl_pipes/actors/common/logging.py
+-rw-r--r--   0        0        0     1591 2024-04-09 11:42:12.618309 etl_pipes-0.6.0/etl_pipes/actors/common/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.6.0/etl_pipes/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.6.0/etl_pipes/common/utils/__init__.py
+-rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.6.0/etl_pipes/common/utils/type_hints.py
+-rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.6.0/etl_pipes/context.py
+-rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.6.0/etl_pipes/domain/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.6.0/etl_pipes/domain/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.6.0/etl_pipes/pipes/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.6.0/etl_pipes/pipes/base_pipe.py
+-rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.6.0/etl_pipes/pipes/broadcast_parallel.py
+-rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.6.0/etl_pipes/pipes/map_reduce.py
+-rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.6.0/etl_pipes/pipes/maybe.py
+-rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.6.0/etl_pipes/pipes/parallel.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.6.0/etl_pipes/pipes/pipeline/__init__.py
+-rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.6.0/etl_pipes/pipes/pipeline/exceptions.py
+-rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.6.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
+-rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.6.0/etl_pipes/pipes/pipeline/pipeline.py
+-rw-r--r--   0        0        0     1133 2024-04-09 11:45:07.819671 etl_pipes-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.6.0/PKG-INFO
```

### Comparing `etl_pipes-0.5.0/README.md` & `etl_pipes-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/actors/actor.py` & `etl_pipes-0.6.0/etl_pipes/actors/actor.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 import asyncio
 import uuid
 from collections.abc import AsyncGenerator
 from dataclasses import dataclass, field
 from typing import Any
 
-from etl_pipes.actors.common.types import ActorId, Output
+from etl_pipes.actors.common.types import ActorId, IActorSystem, Output
 
 
 @dataclass
 class Actor:
     name: str
     id: ActorId = field(default_factory=lambda: ActorId(str(uuid.uuid4())))
 
     results_buffer: asyncio.Queue[Any] = field(default_factory=asyncio.Queue)
     exceptions_buffer: asyncio.Queue[Exception] = field(default_factory=asyncio.Queue)
 
     receiving_actors: dict[ActorId, Actor] = field(default_factory=dict)
     sending_actors: dict[ActorId, Actor] = field(default_factory=dict)
+    system: IActorSystem | None = None
 
     async def process_result(self, result: Any) -> Output | None:
         raise NotImplementedError("Actor must implement process_message method")
 
     async def process_exception(self, exception: Exception) -> Output | None:
         return Output().save_exception(exception)
```

### Comparing `etl_pipes-0.5.0/etl_pipes/actors/actor_system.py` & `etl_pipes-0.6.0/etl_pipes/actors/actor_system.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 )
 
 
 @dataclass
 class ActorSystem:
     actors: list[Actor]
     connections: list[tuple[Actor, Actor]] = field(default_factory=list)
-    initial_result_messages: list[Message] = field(default_factory=list)
-    initial_exception_messages: list[Message] = field(default_factory=list)
 
     no_outcome_timeout: timedelta = field(default_factory=lambda: timedelta(seconds=10))
     should_be_killed_event: asyncio.Event = field(default_factory=asyncio.Event)
 
     results_to_send: asyncio.Queue[Message] = field(default_factory=asyncio.Queue)
     exceptions_to_send: asyncio.Queue[Message] = field(default_factory=asyncio.Queue)
 
@@ -45,18 +43,19 @@
     starting_actor_ids: set[ActorId] = field(default_factory=set)
 
     process_tasks: dict[MessageId, asyncio.Task[None]] = field(default_factory=dict)
 
     def __post_init__(self) -> None:
         self.actors_dict = {actor.id: actor for actor in self.actors}
         self.actor_ids = {actor.id for actor in self.actors}
+        for actor in self.actors:
+            actor.system = self
 
     async def run(self) -> None:
         self.generate_pairs()
-        await self.distribute_initial_messages()
 
         async def process_message(
             message: Message,
             process_func: Callable[[Actor, Any], Coroutine[None, None, Output | None]],
             collected: dict[ActorId, asyncio.Queue[Message]],
         ) -> None:
             if message.receiver_id is None:
@@ -114,20 +113,14 @@
             for receiver_actor_id in sender_actor.receiving_actors:
                 pairs.add((sender_actor_id, receiver_actor_id))
         self.connections = [
             (self.actors_dict[sender_actor_id], self.actors_dict[receiver_actor_id])
             for (sender_actor_id, receiver_actor_id) in pairs
         ]
 
-    async def distribute_initial_messages(self) -> None:
-        for message in self.initial_result_messages:
-            await self.results_to_send.put(message)
-        for exception in self.initial_exception_messages:
-            await self.exceptions_to_send.put(exception)
-
     async def distribute_output(
         self, trace_id: MessageTraceId, output: Output, sender: Actor
     ) -> None:
         async def queue_messages(
             data_items: list[Any], queue: asyncio.Queue[Any]
         ) -> None:
             receiver_ids = sender.receiving_actors or [
@@ -200,7 +193,13 @@
         ] = {}
         for actor_id, collected_results in self.collected_results.items():
             outputs[actor_id] = (collected_results, asyncio.Queue())
         for actor_id, collected_exceptions in self.collected_exceptions.items():
             collected_results, _ = outputs[actor_id]
             outputs[actor_id] = (collected_results, collected_exceptions)
         return outputs
+
+    async def insert_result_message(self, message: Message) -> None:
+        await self.results_to_send.put(message)
+
+    async def insert_exception_message(self, message: Message) -> None:
+        await self.exceptions_to_send.put(message)
```

### Comparing `etl_pipes-0.5.0/etl_pipes/actors/common/logging.py` & `etl_pipes-0.6.0/etl_pipes/actors/common/logging.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/actors/common/types.py` & `etl_pipes-0.6.0/etl_pipes/actors/common/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,8 +49,12 @@
 
     def save_exception(self, exception: Exception) -> Output:
         self.exceptions.append(exception)
         return self
 
 
 class IActorSystem(Protocol):
-    pass
+    async def insert_result_message(self, message: Message) -> None:
+        ...
+
+    async def insert_exception_message(self, message: Message) -> None:
+        ...
```

### Comparing `etl_pipes-0.5.0/etl_pipes/context.py` & `etl_pipes-0.6.0/etl_pipes/context.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/base_pipe.py` & `etl_pipes-0.6.0/etl_pipes/pipes/base_pipe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/map_reduce.py` & `etl_pipes-0.6.0/etl_pipes/pipes/map_reduce.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/maybe.py` & `etl_pipes-0.6.0/etl_pipes/pipes/maybe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/parallel.py` & `etl_pipes-0.6.0/etl_pipes/pipes/parallel.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/pipeline/exceptions.py` & `etl_pipes-0.6.0/etl_pipes/pipes/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py` & `etl_pipes-0.6.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipeline.py` & `etl_pipes-0.6.0/etl_pipes/pipes/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.5.0/pyproject.toml` & `etl_pipes-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "etl-pipes"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = [ "Tikhon Zaikin <th@thevhs.club>",]
 readme = "README.md"
 
 [tool.ruff]
 select = [ "E", "F", "UP", "W", "I", "N", "PL", "RUF", "PTH",]
```

### Comparing `etl_pipes-0.5.0/PKG-INFO` & `etl_pipes-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-pipes
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Tikhon Zaikin
 Author-email: th@thevhs.club
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pip (>=23.2,<24.0)
```

