# Comparing `tmp/etl_pipes-0.7.0.tar.gz` & `tmp/etl_pipes-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_pipes-0.7.0.tar", max compression
+gzip compressed data, was "etl_pipes-0.8.0.tar", max compression
```

## Comparing `etl_pipes-0.7.0.tar` & `etl_pipes-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.7.0/etl_pipes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.7.0/etl_pipes/actors/__init__.py
--rw-r--r--   0        0        0     2217 2024-04-09 11:57:50.370449 etl_pipes-0.7.0/etl_pipes/actors/actor.py
--rw-r--r--   0        0        0     8176 2024-04-09 12:09:55.472411 etl_pipes-0.7.0/etl_pipes/actors/actor_system.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.7.0/etl_pipes/actors/common/__init__.py
--rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.7.0/etl_pipes/actors/common/logging.py
--rw-r--r--   0        0        0     1635 2024-04-09 12:09:55.441120 etl_pipes-0.7.0/etl_pipes/actors/common/types.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.7.0/etl_pipes/common/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.7.0/etl_pipes/common/utils/__init__.py
--rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.7.0/etl_pipes/common/utils/type_hints.py
--rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.7.0/etl_pipes/context.py
--rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.7.0/etl_pipes/domain/__init__.py
--rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.7.0/etl_pipes/domain/types.py
--rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.7.0/etl_pipes/pipes/__init__.py
--rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.7.0/etl_pipes/pipes/base_pipe.py
--rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.7.0/etl_pipes/pipes/broadcast_parallel.py
--rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.7.0/etl_pipes/pipes/map_reduce.py
--rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.7.0/etl_pipes/pipes/maybe.py
--rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.7.0/etl_pipes/pipes/parallel.py
--rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.7.0/etl_pipes/pipes/pipeline/__init__.py
--rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.7.0/etl_pipes/pipes/pipeline/exceptions.py
--rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.7.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
--rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.7.0/etl_pipes/pipes/pipeline/pipeline.py
--rw-r--r--   0        0        0     1133 2024-04-09 12:11:31.504815 etl_pipes-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.8.0/etl_pipes/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.8.0/etl_pipes/actors/__init__.py
+-rw-r--r--   0        0        0     2217 2024-04-09 11:57:50.370449 etl_pipes-0.8.0/etl_pipes/actors/actor.py
+-rw-r--r--   0        0        0     8848 2024-04-09 12:24:01.857814 etl_pipes-0.8.0/etl_pipes/actors/actor_system.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.8.0/etl_pipes/actors/common/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.8.0/etl_pipes/actors/common/logging.py
+-rw-r--r--   0        0        0     1635 2024-04-09 12:09:55.441120 etl_pipes-0.8.0/etl_pipes/actors/common/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.8.0/etl_pipes/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.8.0/etl_pipes/common/utils/__init__.py
+-rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.8.0/etl_pipes/common/utils/type_hints.py
+-rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.8.0/etl_pipes/context.py
+-rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.8.0/etl_pipes/domain/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.8.0/etl_pipes/domain/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.8.0/etl_pipes/pipes/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.8.0/etl_pipes/pipes/base_pipe.py
+-rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.8.0/etl_pipes/pipes/broadcast_parallel.py
+-rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.8.0/etl_pipes/pipes/map_reduce.py
+-rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.8.0/etl_pipes/pipes/maybe.py
+-rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.8.0/etl_pipes/pipes/parallel.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.8.0/etl_pipes/pipes/pipeline/__init__.py
+-rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.8.0/etl_pipes/pipes/pipeline/exceptions.py
+-rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.8.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
+-rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.8.0/etl_pipes/pipes/pipeline/pipeline.py
+-rw-r--r--   0        0        0     1133 2024-04-09 12:25:18.705231 etl_pipes-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.8.0/PKG-INFO
```

### Comparing `etl_pipes-0.7.0/README.md` & `etl_pipes-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/actors/actor.py` & `etl_pipes-0.8.0/etl_pipes/actors/actor.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/actors/actor_system.py` & `etl_pipes-0.8.0/etl_pipes/actors/actor_system.py`

 * *Files 11% similar despite different names*

```diff
@@ -194,16 +194,39 @@
         for actor_id, collected_results in self.collected_results.items():
             outputs[actor_id] = (collected_results, asyncio.Queue())
         for actor_id, collected_exceptions in self.collected_exceptions.items():
             collected_results, _ = outputs[actor_id]
             outputs[actor_id] = (collected_results, collected_exceptions)
         return outputs
 
-    async def insert_result_message(self, data: Any, actor_id: ActorId) -> None:
-        message = Message(data=data, receiver_id=actor_id)
-        await self.results_to_send.put(message)
+    async def insert_result_message(
+        self,
+        data: Any,
+        from_actor: ActorId | None = None,
+        to_actor: ActorId | None = None,
+    ) -> None:
+        await self.insert_message(self.results_to_send, data, from_actor, to_actor)
 
     async def insert_exception_message(
-        self, data: Exception, actor_id: ActorId
+        self,
+        data: Exception,
+        from_actor: ActorId | None = None,
+        to_actor: ActorId | None = None,
+    ) -> None:
+        await self.insert_message(self.exceptions_to_send, data, from_actor, to_actor)
+
+    async def insert_message(
+        self,
+        queue: asyncio.Queue[Message],
+        data: Any,
+        from_actor: ActorId | None,
+        to_actor: ActorId | None,
     ) -> None:
-        message = Message(data=data, receiver_id=actor_id)
-        await self.exceptions_to_send.put(message)
+        if to_actor:
+            message = Message(data=data, receiver_id=to_actor)
+            await queue.put(message)
+
+        if from_actor:
+            receivers = self.actors_dict[from_actor].receiving_actors
+            for receiver_id in receivers:
+                message = Message(data=data, receiver_id=receiver_id)
+                await queue.put(message)
```

### Comparing `etl_pipes-0.7.0/etl_pipes/actors/common/logging.py` & `etl_pipes-0.8.0/etl_pipes/actors/common/logging.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/actors/common/types.py` & `etl_pipes-0.8.0/etl_pipes/actors/common/types.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/context.py` & `etl_pipes-0.8.0/etl_pipes/context.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/base_pipe.py` & `etl_pipes-0.8.0/etl_pipes/pipes/base_pipe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/map_reduce.py` & `etl_pipes-0.8.0/etl_pipes/pipes/map_reduce.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/maybe.py` & `etl_pipes-0.8.0/etl_pipes/pipes/maybe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/parallel.py` & `etl_pipes-0.8.0/etl_pipes/pipes/parallel.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/pipeline/exceptions.py` & `etl_pipes-0.8.0/etl_pipes/pipes/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py` & `etl_pipes-0.8.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/etl_pipes/pipes/pipeline/pipeline.py` & `etl_pipes-0.8.0/etl_pipes/pipes/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.7.0/pyproject.toml` & `etl_pipes-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "etl-pipes"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = [ "Tikhon Zaikin <th@thevhs.club>",]
 readme = "README.md"
 
 [tool.ruff]
 select = [ "E", "F", "UP", "W", "I", "N", "PL", "RUF", "PTH",]
```

### Comparing `etl_pipes-0.7.0/PKG-INFO` & `etl_pipes-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-pipes
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: Tikhon Zaikin
 Author-email: th@thevhs.club
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pip (>=23.2,<24.0)
```

