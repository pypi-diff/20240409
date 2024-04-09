# Comparing `tmp/p4adev_tools-0.0.1.tar.gz` & `tmp/p4adev_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4adev_tools-0.0.1.tar", max compression
+gzip compressed data, was "p4adev_tools-0.0.2.tar", max compression
```

## Comparing `p4adev_tools-0.0.1.tar` & `p4adev_tools-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11324 2024-04-09 03:49:43.737319 p4adev_tools-0.0.1/LICENSE
--rw-r--r--   0        0        0     2552 2024-04-09 03:49:28.538320 p4adev_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-09 03:09:16.596456 p4adev_tools-0.0.1/src/p4adev_tools/__init__.py
--rw-r--r--   0        0        0     1554 2024-04-09 03:04:39.094471 p4adev_tools-0.0.1/src/p4adev_tools/ftp_server.py
--rw-r--r--   0        0        0     6720 2024-04-09 03:14:10.625439 p4adev_tools-0.0.1/src/p4adev_tools/ipykernel_threaded.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 p4adev_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-09 03:49:43.737319 p4adev_tools-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2552 2024-04-09 03:55:23.282300 p4adev_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-09 03:09:16.596456 p4adev_tools-0.0.2/src/p4adev_tools/__init__.py
+-rw-r--r--   0        0        0     1522 2024-04-09 03:55:19.269300 p4adev_tools-0.0.2/src/p4adev_tools/ftp_server.py
+-rw-r--r--   0        0        0     6720 2024-04-09 03:14:10.625439 p4adev_tools-0.0.2/src/p4adev_tools/ipykernel_threaded.py
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 p4adev_tools-0.0.2/PKG-INFO
```

### Comparing `p4adev_tools-0.0.1/LICENSE` & `p4adev_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `p4adev_tools-0.0.1/pyproject.toml` & `p4adev_tools-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "p4adev_tools"
-version = "0.0.1"
+version = "0.0.2"
 description = "Collection of widgets for the older kivymd 1.1.1 lib (material design 2)."
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 packages = [
     { include = "p4adev_tools", from = "src" },
 ]
```

### Comparing `p4adev_tools-0.0.1/src/p4adev_tools/ftp_server.py` & `p4adev_tools-0.0.2/src/p4adev_tools/ftp_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# TODO: Publish tools to PyPi..
 from __future__ import annotations
 
 from multiprocessing import Process
 from socket import AF_INET, SOCK_DGRAM, socket
 
 from pyftpdlib.authorizers import DummyAuthorizer
 from pyftpdlib.handlers import FTPHandler
```

### Comparing `p4adev_tools-0.0.1/src/p4adev_tools/ipykernel_threaded.py` & `p4adev_tools-0.0.2/src/p4adev_tools/ipykernel_threaded.py`

 * *Files identical despite different names*

### Comparing `p4adev_tools-0.0.1/PKG-INFO` & `p4adev_tools-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4adev_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collection of widgets for the older kivymd 1.1.1 lib (material design 2).
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

