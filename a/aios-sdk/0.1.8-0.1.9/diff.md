# Comparing `tmp/aios_sdk-0.1.8.tar.gz` & `tmp/aios_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aios_sdk-0.1.8.tar", max compression
+gzip compressed data, was "aios_sdk-0.1.9.tar", max compression
```

## Comparing `aios_sdk-0.1.8.tar` & `aios_sdk-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1575 2024-04-08 17:35:05.050215 aios_sdk-0.1.8/README.md
--rw-r--r--   0        0        0     1389 2024-04-08 17:16:11.666395 aios_sdk-0.1.8/aios_sdk/__init__.py
--rw-r--r--   0        0        0       39 2024-04-08 16:54:15.111610 aios_sdk-0.1.8/aios_sdk/cli.py
--rw-r--r--   0        0        0      490 2024-04-08 16:54:15.149136 aios_sdk-0.1.8/aios_sdk/inference.py
--rw-r--r--   0        0        0      399 2024-04-08 17:09:25.255495 aios_sdk-0.1.8/aios_sdk/models.py
--rw-r--r--   0        0        0     2945 2024-04-08 16:54:15.111805 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.py
--rw-r--r--   0        0        0     4770 2024-04-08 16:54:15.112012 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.pyi
--rw-r--r--   0        0        0     5673 2024-04-08 16:54:15.112215 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.py
--rw-r--r--   0        0        0     2457 2024-04-08 16:54:15.112300 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2024-04-08 16:54:15.112379 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.py
--rw-r--r--   0        0        0     1034 2024-04-08 16:54:15.112462 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.pyi
--rw-r--r--   0        0        0     2405 2024-04-08 16:54:15.112553 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.py
--rw-r--r--   0        0        0     1238 2024-04-08 16:54:15.112659 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.pyi
--rw-r--r--   0        0        0     2902 2024-04-08 16:54:15.112754 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.py
--rw-r--r--   0        0        0     4952 2024-04-08 16:54:15.112973 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.pyi
--rw-r--r--   0        0        0     4020 2024-04-08 16:54:15.113073 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.py
--rw-r--r--   0        0        0     1842 2024-04-08 16:54:15.113168 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.pyi
--rw-r--r--   0        0        0     1298 2024-04-08 16:54:15.113273 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.py
--rw-r--r--   0        0        0      632 2024-04-08 16:54:15.113361 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.pyi
--rw-r--r--   0        0        0     2331 2024-04-08 16:54:15.113436 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.py
--rw-r--r--   0        0        0     1178 2024-04-08 16:54:15.113517 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.pyi
--rw-r--r--   0        0        0     3604 2024-04-08 16:54:15.113607 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.py
--rw-r--r--   0        0        0     6093 2024-04-08 16:54:15.113815 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.pyi
--rw-r--r--   0        0        0     8333 2024-04-08 16:54:15.113915 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.py
--rw-r--r--   0        0        0     3179 2024-04-08 16:54:15.114003 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.pyi
--rw-r--r--   0        0        0     1833 2024-04-08 16:54:15.114081 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.py
--rw-r--r--   0        0        0     2498 2024-04-08 16:54:15.114172 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.pyi
--rw-r--r--   0        0        0     2525 2024-04-08 16:54:15.114265 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.py
--rw-r--r--   0        0        0     1340 2024-04-08 16:54:15.114356 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.pyi
--rw-r--r--   0        0        0     3459 2024-04-08 16:54:15.114449 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.py
--rw-r--r--   0        0        0     5489 2024-04-08 16:54:15.114650 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.pyi
--rw-r--r--   0        0        0     5581 2024-04-08 16:54:15.114842 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.py
--rw-r--r--   0        0        0     2369 2024-04-08 16:54:15.114917 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.pyi
--rw-r--r--   0        0        0      533 2024-04-08 17:22:50.520354 aios_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 aios_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1575 2024-04-08 17:35:05.050215 aios_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0     1389 2024-04-08 17:16:11.666395 aios_sdk-0.1.9/aios_sdk/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-08 18:09:32.004809 aios_sdk-0.1.9/aios_sdk/cli.py
+-rw-r--r--   0        0        0      490 2024-04-08 16:54:15.149136 aios_sdk-0.1.9/aios_sdk/inference.py
+-rw-r--r--   0        0        0      399 2024-04-08 17:09:25.255495 aios_sdk-0.1.9/aios_sdk/models.py
+-rw-r--r--   0        0        0     2945 2024-04-08 16:54:15.111805 aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2.py
+-rw-r--r--   0        0        0     4770 2024-04-08 16:54:15.112012 aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2.pyi
+-rw-r--r--   0        0        0     5673 2024-04-08 16:54:15.112215 aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2_grpc.py
+-rw-r--r--   0        0        0     2457 2024-04-08 16:54:15.112300 aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2024-04-08 16:54:15.112379 aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2.py
+-rw-r--r--   0        0        0     1034 2024-04-08 16:54:15.112462 aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2.pyi
+-rw-r--r--   0        0        0     2405 2024-04-08 16:54:15.112553 aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2_grpc.py
+-rw-r--r--   0        0        0     1238 2024-04-08 16:54:15.112659 aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2902 2024-04-08 16:54:15.112754 aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2.py
+-rw-r--r--   0        0        0     4952 2024-04-08 18:09:29.812395 aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2.pyi
+-rw-r--r--   0        0        0     4020 2024-04-08 16:54:15.113073 aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2_grpc.py
+-rw-r--r--   0        0        0     1842 2024-04-08 16:54:15.113168 aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1298 2024-04-08 16:54:15.113273 aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2.py
+-rw-r--r--   0        0        0      632 2024-04-08 16:54:15.113361 aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2.pyi
+-rw-r--r--   0        0        0     2331 2024-04-08 16:54:15.113436 aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2_grpc.py
+-rw-r--r--   0        0        0     1178 2024-04-08 16:54:15.113517 aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3604 2024-04-08 16:54:15.113607 aios_sdk-0.1.9/aios_sdk/rpc/models_pb2.py
+-rw-r--r--   0        0        0     6093 2024-04-08 16:54:15.113815 aios_sdk-0.1.9/aios_sdk/rpc/models_pb2.pyi
+-rw-r--r--   0        0        0     8333 2024-04-08 16:54:15.113915 aios_sdk-0.1.9/aios_sdk/rpc/models_pb2_grpc.py
+-rw-r--r--   0        0        0     3179 2024-04-08 16:54:15.114003 aios_sdk-0.1.9/aios_sdk/rpc/models_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1833 2024-04-08 16:54:15.114081 aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2.py
+-rw-r--r--   0        0        0     2498 2024-04-08 16:54:15.114172 aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2.pyi
+-rw-r--r--   0        0        0     2525 2024-04-08 16:54:15.114265 aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2_grpc.py
+-rw-r--r--   0        0        0     1340 2024-04-08 16:54:15.114356 aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3459 2024-04-08 16:54:15.114449 aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2.py
+-rw-r--r--   0        0        0     5489 2024-04-08 16:54:15.114650 aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2.pyi
+-rw-r--r--   0        0        0     5581 2024-04-08 16:54:15.114842 aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2_grpc.py
+-rw-r--r--   0        0        0     2369 2024-04-08 16:54:15.114917 aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2_grpc.pyi
+-rw-r--r--   0        0        0      546 2024-04-09 16:44:11.977929 aios_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1978 1970-01-01 00:00:00.000000 aios_sdk-0.1.9/PKG-INFO
```

### Comparing `aios_sdk-0.1.8/README.md` & `aios_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/__init__.py` & `aios_sdk-0.1.9/aios_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/app_state_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/helloworld_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/inference_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/kill_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/models_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/models_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/system_info_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.py` & `aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.py` & `aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.pyi` & `aios_sdk-0.1.9/aios_sdk/rpc/websocket_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.8/pyproject.toml` & `aios_sdk-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "aios-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ginkoe <ginkoe@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 grpcio = "^1.62.1"
+torch = "^2.2.2"
+protobuf = "^5.26.1"
 
 [tool.poetry.group.dev.dependencies]
-grpcio-tools = "^1.62.1"
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aios_sdk-0.1.8/PKG-INFO` & `aios_sdk-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: aios-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Ginkoe
 Author-email: ginkoe@protonmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.62.1,<2.0.0)
+Requires-Dist: protobuf (>=5.26.1,<6.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://i.imgur.com/dvk7vte.png" width="100%" alt="project-logo">
 </p>
 <p align="center">
     <h1 align="center">aiOS</h1>
```

