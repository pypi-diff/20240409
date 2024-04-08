# Comparing `tmp/kaspad_client-1.0.1.tar.gz` & `tmp/kaspad_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaspad_client-1.0.1.tar", max compression
+gzip compressed data, was "kaspad_client-1.0.2.tar", max compression
```

## Comparing `kaspad_client-1.0.1.tar` & `kaspad_client-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      708 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/README.md
--rw-r--r--   0        0        0      125 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/__init__.py
--rw-r--r--   0        0        0    12456 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/messages_pb2.py
--rw-r--r--   0        0        0     2441 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/messages_pb2_grpc.py
--rw-r--r--   0        0        0     7961 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/protos/messages.proto
--rw-r--r--   0        0        0    22350 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/protos/rpc.proto
--rw-r--r--   0        0        0    37938 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/rpc_pb2.py
--rw-r--r--   0        0        0      148 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/kaspa_grpc/rpc_pb2_grpc.py
--rw-r--r--   0        0        0    14745 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/modules/KaspadClient.py
--rw-r--r--   0        0        0     2479 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/modules/KaspadStream.py
--rw-r--r--   0        0        0        0 2024-04-08 23:09:56.750794 kaspad_client-1.0.1/kaspad_client/modules/__init__.py
--rw-r--r--   0        0        0      708 2024-04-08 23:09:56.754794 kaspad_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 kaspad_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      993 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/README.md
+-rw-r--r--   0        0        0      125 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/__init__.py
+-rw-r--r--   0        0        0    12456 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/messages_pb2.py
+-rw-r--r--   0        0        0     2441 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/messages_pb2_grpc.py
+-rw-r--r--   0        0        0     7961 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/protos/messages.proto
+-rw-r--r--   0        0        0    22350 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/protos/rpc.proto
+-rw-r--r--   0        0        0    37938 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/rpc_pb2.py
+-rw-r--r--   0        0        0      148 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/kaspa_grpc/rpc_pb2_grpc.py
+-rw-r--r--   0        0        0    14745 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/modules/KaspadClient.py
+-rw-r--r--   0        0        0     2479 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/modules/KaspadStream.py
+-rw-r--r--   0        0        0        0 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/kaspad_client/modules/__init__.py
+-rw-r--r--   0        0        0      728 2024-04-08 23:32:08.878755 kaspad_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 kaspad_client-1.0.2/PKG-INFO
```

### Comparing `kaspad_client-1.0.1/kaspad_client/kaspa_grpc/messages_pb2.py` & `kaspad_client-1.0.2/kaspad_client/kaspa_grpc/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/kaspad_client/kaspa_grpc/messages_pb2_grpc.py` & `kaspad_client-1.0.2/kaspad_client/kaspa_grpc/messages_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/kaspad_client/kaspa_grpc/protos/messages.proto` & `kaspad_client-1.0.2/kaspad_client/kaspa_grpc/protos/messages.proto`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/kaspad_client/kaspa_grpc/protos/rpc.proto` & `kaspad_client-1.0.2/kaspad_client/kaspa_grpc/protos/rpc.proto`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/kaspad_client/kaspa_grpc/rpc_pb2.py` & `kaspad_client-1.0.2/kaspad_client/kaspa_grpc/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/kaspad_client/modules/KaspadClient.py` & `kaspad_client-1.0.2/kaspad_client/modules/KaspadClient.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/kaspad_client/modules/KaspadStream.py` & `kaspad_client-1.0.2/kaspad_client/modules/KaspadStream.py`

 * *Files identical despite different names*

### Comparing `kaspad_client-1.0.1/pyproject.toml` & `kaspad_client-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "kaspad_client"
-version = "1.0.1"
+version = "1.0.2"
 description = "This is a simple gRPC client for a python application which communiactes with the Kaspa node called KASPAD."
 authors = ["lAmeR1 <lamer1@github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 grpcio = "^1.62.1"
+protobuf = "4.21.6"
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 grpcio-tools = "^1.62.1"
 pytest-asyncio = "^0.23.6"
```

### Comparing `kaspad_client-1.0.1/PKG-INFO` & `kaspad_client-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: kaspad_client
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a simple gRPC client for a python application which communiactes with the Kaspa node called KASPAD.
 Author: lAmeR1
 Author-email: lamer1@github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.62.1,<2.0.0)
+Requires-Dist: protobuf (==4.21.6)
 Description-Content-Type: text/markdown
 
 This is a simple gRPC client for a python application which communiactes with the Kaspa node called KASPAD.
 
 The module is based on asyncio, since the Kaspa BlockDAG is unbelievable fast and also needs the support of notifications.
 
 # Usage
@@ -29,8 +30,13 @@
     asyncio.run(main())
 
 
 returns
 
     {'getInfoResponse': {'p2pId': 'd3d2af24-9ddd-4cf8-86eb-d1acd539857a', 'serverVersion': '0.13.4', 'isUtxoIndexed': True, 'isSynced': True, 'hasNotifyCommand': True, 'hasMessageId': True, 'mempoolSize': '0'}, 'id': '0'}
 
+# Donation
+
+We are doing this in our free time. Please consider a donation if this helps! Thank you!
+
+[kaspa:qrlsm9tvmak6909pr9f35g6scapz5t689nhhls54sfxx5m46sn085ajhn9hn8](https://explorer.kaspa.org/addresses/kaspa:qrlsm9tvmak6909pr9f35g6scapz5t689nhhls54sfxx5m46sn085ajhn9hn8?page=1)
```

