# Comparing `tmp/kaspad_client-1.0.3.tar.gz` & `tmp/kaspad_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaspad_client-1.0.3.tar", max compression
+gzip compressed data, was "kaspad_client-1.0.4.tar", max compression
```

## Comparing `kaspad_client-1.0.3.tar` & `kaspad_client-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      993 2024-04-08 23:48:26.224402 kaspad_client-1.0.3/README.md
--rw-r--r--   0        0        0      125 2024-04-08 23:48:26.224402 kaspad_client-1.0.3/kaspad_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 23:48:26.224402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/__init__.py
--rw-r--r--   0        0        0    12456 2024-04-08 23:48:26.224402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/messages_pb2.py
--rw-r--r--   0        0        0     2441 2024-04-08 23:48:26.224402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/messages_pb2_grpc.py
--rw-r--r--   0        0        0     7961 2024-04-08 23:48:26.224402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/protos/messages.proto
--rw-r--r--   0        0        0    22350 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/protos/rpc.proto
--rw-r--r--   0        0        0    37938 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/rpc_pb2.py
--rw-r--r--   0        0        0      148 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/kaspad_client/kaspa_grpc/rpc_pb2_grpc.py
--rw-r--r--   0        0        0    14745 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/kaspad_client/modules/KaspadClient.py
--rw-r--r--   0        0        0     2479 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/kaspad_client/modules/KaspadStream.py
--rw-r--r--   0        0        0        0 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/kaspad_client/modules/__init__.py
--rw-r--r--   0        0        0      728 2024-04-08 23:48:26.228402 kaspad_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 kaspad_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-09 19:51:32.090416 kaspad_client-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1972 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/README.md
+-rw-r--r--   0        0        0      125 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/__init__.py
+-rw-r--r--   0        0        0    12456 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/messages_pb2.py
+-rw-r--r--   0        0        0     2441 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/messages_pb2_grpc.py
+-rw-r--r--   0        0        0     7961 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/protos/messages.proto
+-rw-r--r--   0        0        0    22350 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/protos/rpc.proto
+-rw-r--r--   0        0        0    37938 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/rpc_pb2.py
+-rw-r--r--   0        0        0      148 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/kaspa_grpc/rpc_pb2_grpc.py
+-rw-r--r--   0        0        0    17093 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/modules/KaspadClient.py
+-rw-r--r--   0        0        0     2842 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/modules/KaspadStream.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/kaspad_client/modules/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-09 19:51:32.094416 kaspad_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2692 1970-01-01 00:00:00.000000 kaspad_client-1.0.4/PKG-INFO
```

### Comparing `kaspad_client-1.0.3/kaspad_client/kaspa_grpc/messages_pb2.py` & `kaspad_client-1.0.4/kaspad_client/kaspa_grpc/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.3/kaspad_client/kaspa_grpc/messages_pb2_grpc.py` & `kaspad_client-1.0.4/kaspad_client/kaspa_grpc/messages_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.3/kaspad_client/kaspa_grpc/protos/messages.proto` & `kaspad_client-1.0.4/kaspad_client/kaspa_grpc/protos/messages.proto`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.3/kaspad_client/kaspa_grpc/protos/rpc.proto` & `kaspad_client-1.0.4/kaspad_client/kaspa_grpc/protos/rpc.proto`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.3/kaspad_client/kaspa_grpc/rpc_pb2.py` & `kaspad_client-1.0.4/kaspad_client/kaspa_grpc/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.3/kaspad_client/modules/KaspadClient.py` & `kaspad_client-1.0.4/kaspad_client/modules/KaspadClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # encoding: utf-8
+import asyncio
 
 from kaspad_client.modules.KaspadStream import KaspadStream
 
 
 # pipenv run python -m grpc_tools.protoc -I./protos --python_out=. --grpc_python_out=. ./protos/rpc.proto ./protos/messages.proto ./protos/p2p.proto
 
 class KaspadClient(object):
@@ -344,14 +345,54 @@
         ???
         :param daa_scores:
         :return:
         """
         return await self.request("GetDaaScoreTimestampEstimateRequest",
                                   wait_for_response_key="GetDaaScoreTimestampEstimateResponse")
 
+    def notify_block_added(self, f):
+        asyncio.get_running_loop().create_task(self.kaspa_stream.register_callback("blockAddedNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifyBlockAddedRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
+    def notify_virtual_chain_changed(self, f):
+        asyncio.get_running_loop().create_task(
+            self.kaspa_stream.register_callback("virtualChainChangedNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifyVirtualChainChangedRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
+    def notify_finality_conflict(self, f):
+        asyncio.get_running_loop().create_task(self.kaspa_stream.register_callback("finalityConflictNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifyFinalityConflictRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
+    def notify_sink_blue_score_changed(self, f):
+        asyncio.get_running_loop().create_task(
+            self.kaspa_stream.register_callback("sinkBlueScoreChangedNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifySinkBlueScoreChangedRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
+    def notify_virtual_daa_score_changed(self, f):
+        asyncio.get_running_loop().create_task(
+            self.kaspa_stream.register_callback("virtualDaaScoreChangedNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifyVirtualDaaScoreChangedRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
+    def notify_pruning_point_utxo_set_override(self, f):
+        asyncio.get_running_loop().create_task(
+            self.kaspa_stream.register_callback("pruningPointUtxoSetOverrideNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifyPruningPointUtxoSetOverrideRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
+    def notify_new_block_template(self, f):
+        asyncio.get_running_loop().create_task(
+            self.kaspa_stream.register_callback("newBlockTemplateNotification", f))
+        asyncio.get_running_loop().create_task(self.request("notifyNewBlockTemplateRequest"))
+        return lambda *args, **kwargs: f(*args, **kwargs)
+
     # async def estimate_network_hashes_per_second(self, window_size: int, start_hash: str):
     #     return await self.request("EstimateNetworkHashesPerSecondRequest",
     #                               {
     #                                   "windowSize": window_size,
     #                                   "startHash": start_hash
     #                               },
     #                               wait_for_response_key="EstimateNetworkHashesPerSecondResponse")
```

### Comparing `kaspad_client-1.0.3/kaspad_client/modules/KaspadStream.py` & `kaspad_client-1.0.4/kaspad_client/modules/KaspadStream.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,36 +30,44 @@
                                                        ('kaspa_grpc.max_send_message_length', MAX_MESSAGE_LENGTH),
                                                        ('kaspa_grpc.max_receive_message_length', MAX_MESSAGE_LENGTH),
                                                    ])
 
         self.__stub = messages_pb2_grpc.RPCStub(self.__channel)
         asyncio.get_running_loop().create_task(self.__loop())
 
+        self.__callback_functions = {}
+
     async def read(self, wait_for_response_key=None):
         while True:
             response = await self.__read_queue.get()
             if wait_for_response_key is None or wait_for_response_key in response:
                 return response
 
     async def send(self, command: str, params: dict = None):
         await self.__command_queue.put((command, params))
 
     async def __loop(self):
         async for resp in self.__stub.MessageStream(self.yield_cmd()):
             await self.__read_queue.put(msg := json_format.MessageToDict(resp, including_default_value_fields=True))
-            _logger.info(f"RECV {msg}")
+            _logger.debug(f"recv: {msg}")
+            for callback in self.__callback_functions.get(next(iter(msg)), []):
+                await callback(msg)
 
     async def yield_cmd(self):
         while True:
             (cmd, params) = await self.__command_queue.get()
+            _logger.debug(f"send: {cmd}")
             msg = KaspadRequest()
             msg2 = getattr(msg, cmd)
             payload = params
 
             if payload:
                 if isinstance(payload, dict):
                     json_format.ParseDict(payload, msg2)
                 if isinstance(payload, str):
                     json_format.Parse(payload, msg2)
 
             msg2.SetInParent()
             yield msg
+
+    async def register_callback(self, response, callback):
+        self.__callback_functions[response] = self.__callback_functions.get(response, []) + [callback]
```

