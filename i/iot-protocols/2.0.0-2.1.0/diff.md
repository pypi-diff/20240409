# Comparing `tmp/iot-protocols-2.0.0.tar.gz` & `tmp/iot-protocols-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iot-protocols-2.0.0.tar", last modified: Fri Mar 22 09:30:29 2024, max compression
+gzip compressed data, was "iot-protocols-2.1.0.tar", last modified: Tue Apr  9 12:48:49 2024, max compression
```

## Comparing `iot-protocols-2.0.0.tar` & `iot-protocols-2.1.0.tar`

### file list

```diff
@@ -1,39 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.204943 iot-protocols-2.0.0/
--rw-rw-rw-   0        0        0     1093 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     3884 2024-03-22 09:30:29.200821 iot-protocols-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3149 2024-03-22 09:30:11.000000 iot-protocols-2.0.0/README.md
--rw-rw-rw-   0        0        0      920 2024-03-22 09:14:09.000000 iot-protocols-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 09:30:29.205491 iot-protocols-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:28.967012 iot-protocols-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.051039 iot-protocols-2.0.0/src/iot_protocols/
--rw-rw-rw-   0        0        0        0 2024-03-22 08:47:02.000000 iot-protocols-2.0.0/src/iot_protocols/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.108133 iot-protocols-2.0.0/src/iot_protocols/iec62056/
--rw-rw-rw-   0        0        0       39 2024-03-22 09:20:22.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/__init__.py
--rw-rw-rw-   0        0        0    10563 2024-03-22 09:17:29.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/client.py
--rw-rw-rw-   0        0        0      315 2024-03-21 20:38:45.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.147421 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/
--rw-rw-rw-   0        0        0       65 2024-03-22 09:20:09.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/__init__.py
--rw-rw-rw-   0        0        0    12431 2024-03-22 09:18:29.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/client.py
--rw-rw-rw-   0        0        0      318 2024-03-21 13:41:07.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/constants.py
--rw-rw-rw-   0        0        0     1387 2024-03-21 13:41:07.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/exceptions.py
--rw-rw-rw-   0        0        0    11468 2024-03-22 09:18:57.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/messages.py
--rw-rw-rw-   0        0        0    12603 2024-03-22 09:19:16.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/transports.py
--rw-rw-rw-   0        0        0     1872 2024-03-22 09:19:08.000000 iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.169937 iot-protocols-2.0.0/src/iot_protocols/modbus/
--rw-rw-rw-   0        0        0      541 2024-03-22 09:21:25.000000 iot-protocols-2.0.0/src/iot_protocols/modbus/__init__.py
--rw-rw-rw-   0        0        0     8839 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/modbus/client.py
--rw-rw-rw-   0        0        0     1905 2024-03-22 09:21:35.000000 iot-protocols-2.0.0/src/iot_protocols/modbus/decoder.py
--rw-rw-rw-   0        0        0      331 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/modbus/exceptions.py
--rw-rw-rw-   0        0        0      981 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/modbus/requests.py
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.189761 iot-protocols-2.0.0/src/iot_protocols/snap7/
--rw-rw-rw-   0        0        0        0 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/snap7/__init__.py
--rw-rw-rw-   0        0        0     2738 2024-03-22 09:27:18.000000 iot-protocols-2.0.0/src/iot_protocols/snap7/client.py
--rw-rw-rw-   0        0        0      198 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/snap7/exceptions.py
--rw-rw-rw-   0        0        0      232 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/snap7/requests.py
--rw-rw-rw-   0        0        0        0 2024-03-21 09:14:47.000000 iot-protocols-2.0.0/src/iot_protocols/snap7/responses.py
-drwxrwxrwx   0        0        0        0 2024-03-22 09:30:29.195377 iot-protocols-2.0.0/src/iot_protocols.egg-info/
--rw-rw-rw-   0        0        0     3884 2024-03-22 09:30:28.000000 iot-protocols-2.0.0/src/iot_protocols.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2024-03-22 09:30:28.000000 iot-protocols-2.0.0/src/iot_protocols.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 09:30:28.000000 iot-protocols-2.0.0/src/iot_protocols.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-22 09:30:28.000000 iot-protocols-2.0.0/src/iot_protocols.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-22 09:30:28.000000 iot-protocols-2.0.0/src/iot_protocols.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.301625 iot-protocols-2.1.0/
+-rw-rw-rw-   0        0        0     1093 2024-03-21 09:14:47.000000 iot-protocols-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3885 2024-04-09 12:48:49.295632 iot-protocols-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3150 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.136628 iot-protocols-2.1.0/iot_protocols/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/data.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.185628 iot-protocols-2.1.0/iot_protocols/devices/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/__init__.py
+-rw-rw-rw-   0        0        0     2402 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/basics.py
+-rw-rw-rw-   0        0        0     5054 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/iec62056_meter.py
+-rw-rw-rw-   0        0        0     5755 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/interfaces.py
+-rw-rw-rw-   0        0        0     1135 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/models.py
+-rw-rw-rw-   0        0        0     5891 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/devices/moxa_iologik_r1214.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.188625 iot-protocols-2.1.0/iot_protocols/protocols/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.202624 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/
+-rw-rw-rw-   0        0        0       39 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/__init__.py
+-rw-rw-rw-   0        0        0    10568 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/client.py
+-rw-rw-rw-   0        0        0      315 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.232627 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/
+-rw-rw-rw-   0        0        0       65 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/__init__.py
+-rw-rw-rw-   0        0        0    12431 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/client.py
+-rw-rw-rw-   0        0        0      318 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/constants.py
+-rw-rw-rw-   0        0        0     1387 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/exceptions.py
+-rw-rw-rw-   0        0        0    11468 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/messages.py
+-rw-rw-rw-   0        0        0    12642 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/transports.py
+-rw-rw-rw-   0        0        0     1872 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.254634 iot-protocols-2.1.0/iot_protocols/protocols/modbus/
+-rw-rw-rw-   0        0        0      541 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/__init__.py
+-rw-rw-rw-   0        0        0     8706 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/client.py
+-rw-rw-rw-   0        0        0     1905 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/decoder.py
+-rw-rw-rw-   0        0        0      331 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/exceptions.py
+-rw-rw-rw-   0        0        0      981 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/modbus/requests.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.277633 iot-protocols-2.1.0/iot_protocols/protocols/snap7/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/__init__.py
+-rw-rw-rw-   0        0        0     2738 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/client.py
+-rw-rw-rw-   0        0        0      198 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/exceptions.py
+-rw-rw-rw-   0        0        0      232 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/requests.py
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/iot_protocols/protocols/snap7/responses.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.290629 iot-protocols-2.1.0/iot_protocols.egg-info/
+-rw-rw-rw-   0        0        0     3885 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 12:48:49.000000 iot-protocols-2.1.0/iot_protocols.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      888 2024-04-09 12:44:59.000000 iot-protocols-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 12:48:49.302629 iot-protocols-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 12:48:49.286627 iot-protocols-2.1.0/test/
+-rw-rw-rw-   0        0        0     2058 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/test/test_iologik_r1214.py
+-rw-rw-rw-   0        0        0     1238 2024-04-09 12:44:32.000000 iot-protocols-2.1.0/test/tests_iec62056.py
```

### Comparing `iot-protocols-2.0.0/LICENSE` & `iot-protocols-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/PKG-INFO` & `iot-protocols-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-protocols
-Version: 2.0.0
+Version: 2.1.0
 Summary: Generic IIoT protocols package
 Author-email: Adrien Delhaye <adrien.delhaye@memoco.eu>
 Project-URL: Homepage, https://pypi.org/manage/project/iot-protocols
 Keywords: python,iiot,protocols
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
@@ -102,15 +102,15 @@
 ```
 
 ## How to use
 
 ### Installation
 
 ```shell
-pip install iot-protools
+pip install iot-protocols
 ```
 
 ### Modbus Client
 
 ```python
 from iot_protocols.modbus import ModbusClient
 from iot_protocols.modbus import requests
```

### Comparing `iot-protocols-2.0.0/README.md` & `iot-protocols-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 ```
 
 ## How to use
 
 ### Installation
 
 ```shell
-pip install iot-protools
+pip install iot-protocols
 ```
 
 ### Modbus Client
 
 ```python
 from iot_protocols.modbus import ModbusClient
 from iot_protocols.modbus import requests
```

### Comparing `iot-protocols-2.0.0/pyproject.toml` & `iot-protocols-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iot-protocols"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Adrien Delhaye", email="adrien.delhaye@memoco.eu" },
 ]
 description = "Generic IIoT protocols package"
 readme = "README.md"
 requires-python = ">=3.7"
 
@@ -23,12 +23,11 @@
 dependencies = [ # Optional
   "pyserial>=3.5",
   "pymodbus==2.5.3",
   "python-snap7==1.3",
   "multipledispatch==1.0.0"
 ]
 [tool.setuptools.packages.find]
-where = ["src"]
 include = ["iot_protocols*"]
-exclude = ["iot_protocols.tests"]
+exclude = ["test"]
 [project.urls]
 Homepage = "https://pypi.org/manage/project/iot-protocols"
```

### Comparing `iot-protocols-2.0.0/src/iot_protocols/iec62056/client.py` & `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 import logging
 import time
 import serial
 from serial.serialutil import SerialException
 
 from typing import List
 
-from iot_protocols.iec62056.tools import client, messages, constants, exceptions
+from iot_protocols.protocols.iec62056.tools import client, messages, constants, exceptions
 
-from iot_protocols.iec62056.exceptions import *
+from iot_protocols.protocols.iec62056.exceptions import *
+from iot_protocols.protocols.iec62056.exceptions import IEC62056RequestException, MeterIdentificationFailed, SerialPortBusyException
 
 
 IEC62056_REACTION_TIME = 1.5 # Maximum reaction time for IEC62056
 
 
 @dataclass
 class TariffResponse:
@@ -75,15 +76,14 @@
     def __init__(
             self,
             baudrate: int,
             port: str,
             parity: str,
             bytesize: int,
             stopbits: int,
-            transport: str="serial",
             **kwargs):
         
         self._baudrate = baudrate
         self._port = port
         self._parity = parity
         self._bytesize = bytesize
         self._stopbits = stopbits
@@ -91,14 +91,21 @@
         self._client: client.Iec6205621Client = client.Iec6205621Client.with_serial_transport(
             port=self._port,
             device_address=""
         )
 
         self._client.transport.TRANSPORT_REQUIRES_ADDRESS = True
 
+    def __enter__(self) -> SerialClient:
+        self.connect()
+        return self
+    
+    def __exit__(self, *args) -> None:
+        self.disconnect()
+    
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(baudrate : {self._baudrate} | port: {self._port} | {self._parity} | {self._bytesize} | {self._stopbits})"
     
     @property
     def baudrate(self) -> int:
         try:
             return self._client.transport.port.baudrate
@@ -130,93 +137,82 @@
             registers (list, optional): list of registers obis code to read. Defaults to [].
             table (str, optional): table to be read. Defaults to 0 which is equivalent to a standart readout.
 
         Returns:
             List[messages.DataSet]: A list of Dataset element that contains the requested registers if found.
         """
         try:
-            self.connect()
-        except SerialPortBusyException as err:
-            raise err
-
-        try:
             logging.debug(f"[Meter.Identification] Start Identification Message.")
             identification = self.read_tariff_identification(device_address=meter_address)
             logging.debug(f"[Meter.Identification] Meter Identification has been read : {identification}")
             
-            self.send_ack_message(table=table)
+            self._send_ack_message(table=table)
 
             logging.debug(f"[Meter.ACK.Sent] ACK message.")
             response: TariffResponse = self.read_tariff_response(timeout=timeout)
             logging.debug(f"[Meter.Data.Received] Response from tariff device : {response!r}")
 
-            self.disconnect()
-
             return response
 
         except Exception as err:
-            self.disconnect()
             if type(err) == SerialException:
                 raise IEC62056RequestException(f"The communication port has failed : {err}")
             else:
                 logging.error(f"Error during the request : {err}")
 
     def read_tariff_identification(self, device_address: str="", ack_stop: bool=False):
         try:
             request = messages.RequestMessage(device_address=device_address)
             logging.debug(f"[Identification.Request] Sending identification request: {request}.")
-            self.connect()
             self._client.transport.send(request.to_bytes())
         except TimeoutError as err:
             raise TimeoutError(f"Reading meter's identification timeouted : {err}")
         
         # Wait to ensure the tariff device has time to responds.
         self._client.rest(IEC62056_REACTION_TIME)
 
         response = self._client.read_identification()
         if isinstance(response, messages.IdentificationMessage):
             logging.debug(f"[Identification.Response] Received : {response}")
             if ack_stop:
                 logging.debug(f"Sending ACK stop to end tariff exchange...")
-                self.send_ack_stop()
-                stop_ack_response = self.read_ack_stop_response()
+                self._send_ack_stop()
+                stop_ack_response = self._read_ack_stop_response()
                 logging.debug(f"ACK Response from tariff device : {stop_ack_response}")
                 if isinstance(stop_ack_response, AckStopResponse):
-                    self.disconnect()
                     return response
                 else:
-                    self.disconnect()
                     logging.warning("Tariff device did not return ACK STOP message back !")
 
             return response
         else:
-            self.send_ack_stop()
+            self._send_ack_stop()
             raise MeterIdentificationFailed(f"Invalid message identification. (COM set with : {self.baudrate} | {self._parity} | {self._bytesize} | {self._stopbits})")
         
     def _get_ack_message(self, table: int=0) -> messages.AckOptionSelectMessage:
         message = messages.AckOptionSelectMessage(
             baud_char=self.BAUDRATE_CHAR[self._baudrate],
             mode_char=table
         )
 
         return message
 
-    def send_ack_message(self, table: int=0) -> None:
+    def _send_ack_message(self, table: int=0) -> None:
         message = self._get_ack_message(table)
         data = message.to_bytes()
         self._client.transport.send(data)
         self._client.rest(IEC62056_REACTION_TIME)
 
-    def send_ack_stop(self) -> None:
+    def _send_ack_stop(self) -> None:
         message = messages.AckOptionSelectMessage("", "")
         data = message.to_bytes()
         self._client.transport.send(data)
         self._client.rest(IEC62056_REACTION_TIME)
 
-    def read_ack_stop_response(self) -> AckStopResponse:
+    def _read_ack_stop_response(self) -> AckStopResponse:
         serial_client : serial.Serial = self._client.transport.port
         serial_client.timeout = 2.2
         data = serial_client.read_until(constants.ETX.encode())
         data += serial_client.read()
         return AckStopResponse.from_bytes(data)
     
     @staticmethod
@@ -242,15 +238,15 @@
         """
         result = []
         port: serial.Serial = self._client.transport.port
         port.timeout = timeout
         start = time.perf_counter()
         encoded = port.read_until(constants.ETX.encode())
         if (time.perf_counter() - start) > timeout:
-            self.send_ack_stop()
+            self._send_ack_stop()
             raise TimeoutError(f"Timeout exceed for this request ! ")
 
         bcc = port.read(1)
         bcc_checked = self.check_bcc(encoded, bcc)
 
         logging.debug(f"[Meter.ReadTariffResponse.Received] Received {len(encoded)} bytes (bcc: {bcc}).")
```

### Comparing `iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/client.py` & `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/client.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/exceptions.py` & `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/messages.py` & `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/messages.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/transports.py` & `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/transports.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
     def send(self, data: bytes):
         """
         Will send data over the transport
 
         :param data:
         """
-        print(f"SENDING: --> {data}")
+        logging.debug(f"Sending bytes through serial transport: --> {data}")
         as_hex = data.hex()
         message = " ".join(as_hex[i:i+2] for i in range(0, len(as_hex), 2))
         logging.debug(f"{message}")
         self._send(data)
         logger.debug(f"Sent {data!r} over transport: {self.__class__.__name__}")
 
     def _send(self, data: bytes):
```

### Comparing `iot-protocols-2.0.0/src/iot_protocols/iec62056/tools/utils.py` & `iot-protocols-2.1.0/iot_protocols/protocols/iec62056/tools/utils.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/modbus/__init__.py` & `iot-protocols-2.1.0/iot_protocols/protocols/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/modbus/client.py` & `iot-protocols-2.1.0/iot_protocols/protocols/modbus/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Any, List
 
 from pymodbus.client.sync import ModbusTcpClient, ModbusSerialClient
 from pymodbus.framer import socket_framer, rtu_framer, tls_framer, ModbusFramer
 from pymodbus.exceptions import ConnectionException
 from multipledispatch import dispatch
 
-from exceptions import *
-from modbus import requests
-from decoder import ModbusPayloadDecoder
+from .exceptions import *
+from . import requests
+from .decoder import ModbusPayloadDecoder
 
 
 MODBUS_FUNCTION_TO_CODE={
     0x01: "ReadCoils",
     0x02: "ReadDiscreteInput",
     0x03: "ReadHoldingRegister",
     0x04: "ReadInputRegister",
@@ -24,14 +24,21 @@
 
 
 class ModbusClient:
 
     def __init__(self, client):
         self._client: ModbusSerialClient | ModbusTcpClient = client
 
+    def __enter__(self):
+        self.connect()
+        return self
+    
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.disconnect()
+    
     def connect(self) -> bool:
         return self._client.connect()
     
     def disconnect(self) -> None:
         self._client.close()
     
     @dispatch(dict)
@@ -43,36 +50,33 @@
         
         except (KeyError, AttributeError) as err:
             raise ModbusRequestException(f"Wrong request configuration: {err}.")
     
     @dispatch(requests.ReadCoils)
     def request(self, request: requests.ReadCoils) -> List[bool]:
         try:
-            self.connect()
             _response = self._client.read_coils(**request.__dict__)
             if _response.isError():
                 raise ModbusRequestException(self._get_error_message(_response, request))
             
             result =  _response.bits[:request.count]
             if request.count==1:
                 return result[0]
-            self.disconnect()
             return result
         
         except ConnectionException as err:
             raise ModbusClientException(f"Could not connect to modbus client : {err}")
         except TimeoutError as err:
             raise ModbusRequestException(f"Request to the modbus device timeout : {err}")
         except Exception as err:
             raise ModbusRequestException(f"Request to the modbus device failed: {err}")
     
     @dispatch(requests.WriteCoils)
     def request(self, request: requests.WriteCoils) -> List[bool]:
         try:
-            self.connect()
             _request = self._client.write_coils(**request.__dict__)
             print(f"MODBUS RESPONSE ---> {_request}")
             if _request.isError():
                 raise ModbusRequestException(self._get_error_message(_request, request))
             
             return self.request(requests.ReadCoils(address=request.address, count=len(request.values), unit=request.unit))
         except ConnectionException as err:
@@ -81,74 +85,67 @@
             raise ModbusRequestException(f"Request to the modbus device timeout : {err}")
         except Exception as err:
             raise ModbusRequestException(f"Request to the modbus device failed: {err}")
         
     @dispatch(requests.ReadDiscreteInput)
     def request(self, request: requests.ReadDiscreteInput) -> List[bool]:
         try:
-            self.connect()
             _response = self._client.read_discrete_inputs(**request.__dict__)
             if _response.isError():
                 return ModbusRequestException(self._get_error_message(_response, request))
 
             result =  _response.bits[:request.count]
             if request.count==1:
                 return result[0]
-            self.disconnect()
             return result
         except ConnectionException as err:
             raise ModbusClientException(f"Could not connect to modbus client : {err}")
         except TimeoutError as err:
             raise ModbusRequestException(f"Request to the modbus device timeout : {err}")
         except Exception as err:
             raise ModbusRequestException(f"Request to the modbus device failed: {err}")
         
     @dispatch(requests.ReadInputRegister)
     def request(self, request: requests.ReadInputRegister) -> List[float | int | str] | float | int | str:
         try:
-            self.connect()
             _response = self._client.read_input_registers(**request.__dict__)
             if _response.isError():
                 return ModbusRequestException(self._get_error_message(_response, request))
             
             decoded = ModbusPayloadDecoder.decode(_response.registers, request.encoding)
-            self.disconnect()
             return decoded
         
         except ConnectionException as err:
             raise ModbusClientException(f"Could not connect to modbus client : {err}")
         except TimeoutError as err:
             raise ModbusRequestException(f"Request to the modbus device timeout : {err}")
         except Exception as err:
             raise ModbusRequestException(f"Request to the modbus device failed: {err}")
         
     @dispatch(requests.ReadHoldingRegister)
     def request(self, request: requests.ReadHoldingRegister) -> List[float | int | str] | float | int | str:
         try:
-            self.connect()
             _response = self._client.read_holding_registers(**request.__dict__)
             if _response.isError():
                 return ModbusRequestException(self._get_error_message(_response, request))
         
             decoded = ModbusPayloadDecoder.decode(_response.registers, request.encoding)
-            self.disconnect()
 
             return decoded
     
         except ConnectionException as err:
             raise ModbusClientException(f"Could not connect to modbus client : {err}")
         except TimeoutError as err:
             raise ModbusRequestException(f"Request to the modbus device timeout : {err}")
         except Exception as err:
             raise ModbusRequestException(f"Request to the modbus device failed: {err}")
         
     @dispatch(requests.WriteRegister)
     def request(self, request: requests.WriteRegister) -> List[float | int | str] | float | int | str:
         try:
-            self.connect()
             _response = self._client.write_registers(**request.__dict__)
             if _response.isError():
                 raise ModbusRequestException(self._get_error_message(_response, request))
             
             return self.request(requests.ReadHoldingRegister(address=request.address, count=len(request.values), unit=request.unit, encoding=str(type(request.values))))
         
         except ConnectionException as err:
```

### Comparing `iot-protocols-2.0.0/src/iot_protocols/modbus/decoder.py` & `iot-protocols-2.1.0/iot_protocols/protocols/modbus/decoder.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/modbus/requests.py` & `iot-protocols-2.1.0/iot_protocols/protocols/modbus/requests.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols/snap7/client.py` & `iot-protocols-2.1.0/iot_protocols/protocols/snap7/client.py`

 * *Files identical despite different names*

### Comparing `iot-protocols-2.0.0/src/iot_protocols.egg-info/PKG-INFO` & `iot-protocols-2.1.0/iot_protocols.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-protocols
-Version: 2.0.0
+Version: 2.1.0
 Summary: Generic IIoT protocols package
 Author-email: Adrien Delhaye <adrien.delhaye@memoco.eu>
 Project-URL: Homepage, https://pypi.org/manage/project/iot-protocols
 Keywords: python,iiot,protocols
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: MacOS :: MacOS X
@@ -102,15 +102,15 @@
 ```
 
 ## How to use
 
 ### Installation
 
 ```shell
-pip install iot-protools
+pip install iot-protocols
 ```
 
 ### Modbus Client
 
 ```python
 from iot_protocols.modbus import ModbusClient
 from iot_protocols.modbus import requests
```

