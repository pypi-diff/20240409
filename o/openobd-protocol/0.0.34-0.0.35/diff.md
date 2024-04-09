# Comparing `tmp/openobd-protocol-0.0.34.tar.gz` & `tmp/openobd-protocol-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd-protocol-0.0.34.tar", last modified: Fri Apr  5 08:02:14 2024, max compression
+gzip compressed data, was "openobd-protocol-0.0.35.tar", last modified: Tue Apr  9 11:44:29 2024, max compression
```

## Comparing `openobd-protocol-0.0.34.tar` & `openobd-protocol-0.0.35.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.393140 openobd-protocol-0.0.34/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-05 08:02:14.392140 openobd-protocol-0.0.34/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 08:02:14.393140 openobd-protocol-0.0.34/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.376139 openobd-protocol-0.0.34/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.385140 openobd-protocol-0.0.34/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.388140 openobd-protocol-0.0.34/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     2376 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4415 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2636 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2994 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3706 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3032 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    14057 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.391140 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     2008 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6578 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-05 08:02:09.000000 openobd-protocol-0.0.34/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 08:02:14.392140 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1485 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-05 08:02:14.000000 openobd-protocol-0.0.34/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.963477 openobd-protocol-0.0.35/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-09 11:44:29.963477 openobd-protocol-0.0.35/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 11:44:29.963477 openobd-protocol-0.0.35/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.943476 openobd-protocol-0.0.35/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.953476 openobd-protocol-0.0.35/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.957476 openobd-protocol-0.0.35/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2994 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ModuleConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ModuleConfiguration_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ObdMessage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ObdMessage_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      549 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    14057 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.959476 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     9440 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.961476 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6578 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.962477 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd-protocol-0.0.34/LICENSE` & `openobd-protocol-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/PKG-INFO` & `openobd-protocol-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.34
+Version: 0.0.35
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.34/pyproject.toml` & `openobd-protocol-0.0.35/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/Authentication_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/BasicResponse_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/ModuleConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/ModuleConfiguration_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/ModuleConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/ObdMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/ObdMessage_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/ObdMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/Status_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol.egg-info/PKG-INFO` & `openobd-protocol-0.0.35/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.34
+Version: 0.0.35
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.34/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd-protocol-0.0.35/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,12 +23,15 @@
 src/openobd_protocol.egg-info/requires.txt
 src/openobd_protocol.egg-info/top_level.txt
 src/openobd_protocol/CAN/CanServices_pb2.py
 src/openobd_protocol/CAN/CanServices_pb2.pyi
 src/openobd_protocol/CAN/CanServices_pb2_grpc.py
 src/openobd_protocol/CAN/Isotp_pb2.py
 src/openobd_protocol/CAN/Isotp_pb2.pyi
+src/openobd_protocol/SessionController/AuthenticationServices_pb2.py
+src/openobd_protocol/SessionController/AuthenticationServices_pb2.pyi
+src/openobd_protocol/SessionController/AuthenticationServices_pb2_grpc.py
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
 src/openobd_protocol/UserInterface/UserInterface_pb2.py
 src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
```

