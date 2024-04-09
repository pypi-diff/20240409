# Comparing `tmp/trinnov-altitude-0.1.0.tar.gz` & `tmp/trinnov-altitude-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.0.tar", last modified: Tue Apr  9 01:46:56 2024, max compression
+gzip compressed data, was "trinnov-altitude-0.1.1.tar", last modified: Tue Apr  9 16:52:34 2024, max compression
```

## Comparing `trinnov-altitude-0.1.0.tar` & `trinnov-altitude-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:46:56.202651 trinnov-altitude-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-09 01:46:56.202651 trinnov-altitude-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:46:56.202651 trinnov-altitude-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:46:56.202651 trinnov-altitude-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/tests/mock_trinnov_altitude_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:46:56.202651 trinnov-altitude-0.1.0/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-09 01:46:44.000000 trinnov-altitude-0.1.0/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:46:56.202651 trinnov-altitude-0.1.0/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-09 01:46:56.000000 trinnov-altitude-0.1.0/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 01:46:56.000000 trinnov-altitude-0.1.0/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:46:56.000000 trinnov-altitude-0.1.0/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 01:46:56.000000 trinnov-altitude-0.1.0/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.755650 trinnov-altitude-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.755650 trinnov-altitude-0.1.1/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-09 16:52:30.000000 trinnov-altitude-0.1.1/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:52:34.759650 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:52:34.000000 trinnov-altitude-0.1.1/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.0/LICENSE` & `trinnov-altitude-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.0/PKG-INFO` & `trinnov-altitude-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: trinnov-altitude
-Version: 0.1.0
-Summary: Python client for interfacing with the Trinnov Altitude processor
-Home-page: https://github.com/binarylogic/py-trinnov-altitude
-Author: Ben Johnson
-Author-email: ben@binarylogic.com
-License: Apache 2.0
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Home Automation
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Trinnov Altitude Python Library
 
 A Python library for interacting with the [Trinnov Altitude processor](https://www.trinnov.com/en/products/altitude32/) via the TCP/IP
 automation protocol provided by the Trinnov Altitude.
 
 ## Overview
```

### Comparing `trinnov-altitude-0.1.0/tests/mock_trinnov_altitude_server.py` & `trinnov-altitude-0.1.1/trinnov_altitude/mocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 """
-Creates a mock Trinnov Altitude server for use in tests
+Utilities for mocking a Trinnov Altitude
 """
 
 import asyncio
 import logging
 import re
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
 
 class MockTrinnovAltitudeServer:
+    """
+    Mocks a real Trinnov Altitude
+
+    This class starts a TCP server on the proviced `host` (default `localhost`)
+    and mimics a real Trinnov Altitude server. This is useful for integration
+    testing a Trinnov Altitude integration.
+    """
+
+    DEFAULT_HOST = "localhost"
+    ENCODING = "ascii"
+
     INITIAL_MESSAGES = [
         "OK",
         "SOURCES_CHANGED",
         "OPTSOURCE 0 Source 1",
         "OK",
         "SOURCE 0",
         "CURRENT_SOURCE_FORMAT_NAME Atmos narrow",
@@ -87,46 +98,80 @@
         "OK",
         "SRATE 48000",
         "AUDIOSYNC_STATUS 0",
         "DECODER NONAUDIO 1 PLAYABLE 0 DECODER none UPMIXER none",
         "AUDIOSYNC Slave",
     ]
 
-    ENCODING = "ascii"
-
-    def __init__(self, host="localhost", port=TrinnovAltitude.DEFAULT_PORT):
+    def __init__(self, host=DEFAULT_HOST, port=TrinnovAltitude.DEFAULT_PORT):
         # Configuration
         self.host = host
         self.port = port
         self.server = None
         self.logger = logging.getLogger(__name__)
 
         # State
         self.active_handlers = set()
         self.volume = -40
 
+    async def start_server(self):
+        self.logger.info(
+            "Starting mock Trinnov Altitude server on %s:%d", self.host, self.port
+        )
+        self.server = await asyncio.start_server(
+            self.handle_client, self.host, self.port
+        )
+        self.logger.info("Mock Trinnov Altitude server started")
+        await self.server.start_serving()
+
+    async def stop_server(self):
+        self.logger.info("Stopping mock Trinnov Altitude server")
+
+        if not self.server:
+            return
+
+        # Stop accepting new connections immediately
+        self.server.close()
+
+        # Cancel active handlers
+        for task in self.active_handlers:
+            task.cancel()
+
+        # Wait for all active client handlers to acknowledge cancellation and cleanup
+        await asyncio.gather(*self.active_handlers, return_exceptions=True)
+
+        # Wait for the server to close
+        await self.server.wait_closed()
+
+        self.logger.info("Mock server stopped")
+
     async def handle_client(self, reader, writer):
         self.logger.debug("Client connected")
 
         task = asyncio.current_task()
         self.active_handlers.add(task)
 
         try:
+            # When you connect to an Altitude it will send a welcome message with
+            # the firmware vesion and ID of the unit.
             writer.write(
                 b"Welcome on Trinnov Optimizer (Version 4.3.2rc1, ID 10485761)\n"
             )
             await writer.drain()
 
-            # An actual Altitude will wait to send the initial state messages, so we account for that here
+            # An actual Altitude will wait to send the initial state messages
             await asyncio.sleep(0.1)
 
+            # Upon connecting the Altitude will send a variety of messages reflecting
+            # current state.
             for message in self.INITIAL_MESSAGES:
                 writer.write(f"{message}\n".encode(self.ENCODING))
                 await writer.drain()
 
+            # Listen for messages
             while True:
                 message_bytes = await reader.readline()
                 if not message_bytes:
                     break
 
                 message = message_bytes.decode(self.ENCODING).strip()
                 responses = self._handle_message(message)
@@ -143,54 +188,21 @@
             try:
                 await writer.wait_closed()
             except ConnectionResetError:
                 pass
 
         self.logger.info("Client disconnected")
 
-    def _send_initial_state(self, writer):
-        for message in self.INITIAL_MESSAGES:
-            writer.write(message.encode(self.ENCODING))
-
     def _handle_message(self, message):
         self.logger.debug("Received message from client: %s", message)
 
         if match := re.match(r"^dvolume\s(-?\d+(\.\d+)?)", message):
             delta = float(match.group(1))
             self.volume += delta
             return ["OK", f"VOLUME {self.volume}"]
         if match := re.match(r"^id (.*)", message):
             return ["OK"]
         elif match := re.match(r"^volume\s(-?\d+(\.\d+)?)", message):
             self.volume = float(match.group(1))
             return ["OK", f"VOLUME {self.volume}"]
         else:
             return [f"ERROR: invalid command: {message}"]
-
-    async def start_server(self):
-        self.logger.info("Starting mock server on %s:%d", self.host, self.port)
-        self.server = await asyncio.start_server(
-            self.handle_client, self.host, self.port
-        )
-        self.logger.info("Mock server started")
-        await self.server.start_serving()
-
-    async def stop_server(self):
-        self.logger.info("Stopping mock server")
-
-        if not self.server:
-            return
-
-        # Stop accepting new connections immediately
-        self.server.close()
-
-        # Cancel active handlers
-        for task in self.active_handlers:
-            task.cancel()
-
-        # Wait for all active client handlers to acknowledge cancellation and cleanup
-        await asyncio.gather(*self.active_handlers, return_exceptions=True)
-
-        # Wait for the server to close
-        await self.server.wait_closed()
-
-        self.logger.info("Mock server stopped")
```

### Comparing `trinnov-altitude-0.1.0/tests/test_trinnov_altitude.py` & `trinnov-altitude-0.1.1/tests/test_trinnov_altitude.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import pytest
 import pytest_asyncio
 
 from trinnov_altitude.exceptions import ConnectionFailedError, ConnectionTimeoutError
+from trinnov_altitude.mocks import MockTrinnovAltitudeServer
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
-from .mock_trinnov_altitude_server import MockTrinnovAltitudeServer
 
 
 @pytest_asyncio.fixture
 async def mock_server():
     server = MockTrinnovAltitudeServer()
     await server.start_server()
     yield server
```

### Comparing `trinnov-altitude-0.1.0/trinnov_altitude/exceptions.py` & `trinnov-altitude-0.1.1/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.0/trinnov_altitude/trinnov_altitude.py` & `trinnov-altitude-0.1.1/trinnov_altitude/trinnov_altitude.py`

 * *Files identical despite different names*

