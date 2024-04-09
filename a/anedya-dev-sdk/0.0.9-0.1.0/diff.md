# Comparing `tmp/anedya-dev-sdk-0.0.9.tar.gz` & `tmp/anedya-dev-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anedya-dev-sdk-0.0.9.tar", last modified: Sat Feb  3 06:49:32 2024, max compression
+gzip compressed data, was "anedya-dev-sdk-0.1.0.tar", last modified: Tue Apr  9 10:31:46 2024, max compression
```

## Comparing `anedya-dev-sdk-0.0.9.tar` & `anedya-dev-sdk-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-02-03 06:49:32.466612 anedya-dev-sdk-0.0.9/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya-dev-sdk-0.0.9/LICENSE
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya-dev-sdk-0.0.9/MANIFEST.in
--rw-r--r--   0 invesun   (1000) invesun   (1000)     1802 2024-02-03 06:49:32.466612 anedya-dev-sdk-0.0.9/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      699 2024-01-04 06:10:43.000000 anedya-dev-sdk-0.0.9/README.md
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1035 2024-02-03 06:49:32.466612 anedya-dev-sdk-0.0.9/setup.cfg
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      469 2024-02-03 06:47:20.000000 anedya-dev-sdk-0.0.9/setup.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-02-03 06:49:32.462612 anedya-dev-sdk-0.0.9/src/
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-02-03 06:49:32.466612 anedya-dev-sdk-0.0.9/src/anedya/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      162 2023-11-29 10:23:23.000000 anedya-dev-sdk-0.0.9/src/anedya/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4174 2024-01-09 10:27:14.000000 anedya-dev-sdk-0.0.9/src/anedya/anedya.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1748 2024-01-09 10:26:58.000000 anedya-dev-sdk-0.0.9/src/anedya/config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      214 2024-01-09 10:26:50.000000 anedya-dev-sdk-0.0.9/src/anedya/encoder.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      373 2024-01-09 10:27:10.000000 anedya-dev-sdk-0.0.9/src/anedya/float.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      427 2023-11-28 12:05:34.000000 anedya-dev-sdk-0.0.9/src/anedya/store.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-02-03 06:49:32.466612 anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/
--rw-r--r--   0 invesun   (1000) invesun   (1000)     1802 2024-02-03 06:49:32.000000 anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      424 2024-02-03 06:49:32.000000 anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-02-03 06:49:32.000000 anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        9 2024-02-03 06:49:32.000000 anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/requires.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-02-03 06:49:32.000000 anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-02-03 06:49:32.466612 anedya-dev-sdk-0.0.9/tests/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.0.9/tests/test_config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.0.9/tests/test_core.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya-dev-sdk-0.1.0/LICENSE
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya-dev-sdk-0.1.0/MANIFEST.in
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2015 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      898 2024-04-09 07:19:02.000000 anedya-dev-sdk-0.1.0/README.md
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1169 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/setup.cfg
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya-dev-sdk-0.1.0/setup.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.680589 anedya-dev-sdk-0.1.0/src/
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.680589 anedya-dev-sdk-0.1.0/src/anedya/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.0/src/anedya/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4167 2024-04-09 10:16:37.000000 anedya-dev-sdk-0.1.0/src/anedya/anedya.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2578 2024-04-09 07:29:26.000000 anedya-dev-sdk-0.1.0/src/anedya/config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya-dev-sdk-0.1.0/src/anedya/errors.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1354 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.0/src/anedya/models.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya-dev-sdk-0.1.0/src/anedya/transaction.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2015 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      389 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/tests/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.0/tests/test_config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.0/tests/test_core.py
```

### Comparing `anedya-dev-sdk-0.0.9/LICENSE` & `anedya-dev-sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.0.9/PKG-INFO` & `anedya-dev-sdk-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.0.9
-Summary: Anedya python based SDK for IoT devices. This SDK is currently under development. Future versions may include breaking changes.
+Version: 0.1.0
+Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Project-URL: Source, https://github.com/anedyaio/anedya-dev-sdk-pyhton
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
+
+<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">
+<img src="https://cdn.anedya.io/android-chrome-512x512.png" style="width:50%; margin:0 auto;">
+</div>
 
 # Anedya SDK
 
 <p>
     <a href="https://pypi.org/project/anedya-dev-sdk/">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk?style=for-the-badge">
     </a>
 </p>
 
 
 The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
 
 This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io)
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.0.9 Summary: Anedya
-python based SDK for IoT devices. This SDK is currently under development.
-Future versions may include breaking changes. Home-page: https://github.com/
-anedyaio/anedya-dev-sdk-pyhton Author: Anedya Systems Author-email:
-support@anedya.io License: Apache License 2.0 Project-URL: Documentation,
-https://docs.anedya.io Project-URL: Release notes, https://github.com/anedyaio/
-anedya-dev-sdk-pyhton Project-URL: Source, https://github.com/anedyaio/anedya-
-dev-sdk-pyhton Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: requests # Anedya SDK
+Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.1.0 Summary: Anedya
+python based SDK for IoT devices. This SDK streamlines connectivity with Anedya
+platform. As this SDK is in Beta release, future versions may have breaking
+changes. Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton Author:
+Anedya Systems Author-email: support@anedya.io License: Apache License 2.0
+Project-URL: Documentation, https://docs.anedya.io Project-URL: Release notes,
+https://github.com/anedyaio/anedya-dev-sdk-pyhton Project-URL: Source, https://
+github.com/anedyaio/anedya-dev-sdk-pyhton Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Description-
+Content-Type: text/markdown License-File: LICENSE
+[https://cdn.anedya.io/android-chrome-512x512.png]
+# Anedya SDK
 _[_P_y_P_I_]
 The **Anedya SDK** is a Python package designed to provide an easy-to-use
 interface for [Anedya](https://anedya.io) cloud services, which enables
 seamless connectivity and data retrieval from IoT devices. This SDK supports
 both MQTT and HTTP communication methods. This SDK wraps the Device APIs
 available in the [Anedya Documentation](https://docs.anedya.io) This is a
 Device SDK, i.e. it is meant to be used by an IoT device. ## Installation To
```

### Comparing `anedya-dev-sdk-0.0.9/README.md` & `anedya-dev-sdk-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">
+<img src="https://cdn.anedya.io/android-chrome-512x512.png" style="width:50%; margin:0 auto;">
+</div>
+
 # Anedya SDK
 
 <p>
     <a href="https://pypi.org/project/anedya-dev-sdk/">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk?style=for-the-badge">
     </a>
 </p>
 
 
 The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
 
 This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io)
@@ -15,8 +19,8 @@
 
 ## Installation
 
 To install the Anedya SDK, you can use `pip`:
 
 ```bash
 pip install anedya-dev-sdk
-```
+```
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+[https://cdn.anedya.io/android-chrome-512x512.png]
 # Anedya SDK
 _[_P_y_P_I_]
 The **Anedya SDK** is a Python package designed to provide an easy-to-use
 interface for [Anedya](https://anedya.io) cloud services, which enables
 seamless connectivity and data retrieval from IoT devices. This SDK supports
 both MQTT and HTTP communication methods. This SDK wraps the Device APIs
 available in the [Anedya Documentation](https://docs.anedya.io) This is a
```

### Comparing `anedya-dev-sdk-0.0.9/setup.cfg` & `anedya-dev-sdk-0.1.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [metadata]
 name = anedya-dev-sdk
-version = 0.0.9
+version = 0.1.0
 url = https://github.com/anedyaio/anedya-dev-sdk-pyhton
 author = Anedya Systems
 author_email = support@anedya.io
-description = Anedya python based SDK for IoT devices. This SDK is currently under development. Future versions may include breaking changes.
+description = Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 long_description = file: README.md
+requires-python = ">=3.7"
+dependencies = ["requests","paho-mqtt>=2.0.0"]
 license = Apache License 2.0
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -22,13 +24,14 @@
 	Release notes = https://github.com/anedyaio/anedya-dev-sdk-pyhton
 	Source = https://github.com/anedyaio/anedya-dev-sdk-pyhton
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
+max-line-length = 120
 ignore = E501
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `anedya-dev-sdk-0.0.9/src/anedya/anedya.py` & `anedya-dev-sdk-0.1.0/src/anedya/anedya.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,95 +10,99 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
+from .config import AnedyaConfig
+from .errors import AnedyaInvalidConfig
+from .config import ConnectionMode
+from .config import MQTTMode
+from .transaction import Transactions
+from .client.certs import ANEDYA_CA_CERTS
+from ssl import SSLContext
 import requests
-import time
-import json
-from .config import *
-from .store import *
+from paho.mqtt import client as mqtt
+from paho.mqtt.client import MQTTv5
+import ssl
+
 
 class AnedyaClient:
 
     def __init__(self, config: AnedyaConfig):
         self.set_config(config)
+
+        # Internal Parameters
+        if config.connection_mode == ConnectionMode.MQTT:
+            # MQTT Related setup
+            self._mqttclient = mqtt.Client(
+                callback_api_version=mqtt.CallbackAPIVersion.VERSION2,
+                client_id=str(self._config._deviceID),
+                transport='websockets',
+                protocol=MQTTv5)
+            self._mqttclient.username_pw_set(
+                username=str(self._config._deviceID),
+                password=self._config.connection_key)
+            self.on_connect = config.on_connect
+            self.on_disconnect = config.on_disconnect
+            self.on_message = config.on_message
+            self._mqttclient.on_connect = self.onconnect_handler
+            self._mqttclient.on_disconnect = self.ondisconnect_handler
+            # self._mqttclient.on_message = self.onmessage_handler
+            self._mqttclient._connect_timeout = 1.0
+            self._transactions = Transactions()
+            # Set TLS Context
+            context = SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+            context.load_verify_locations(cadata=ANEDYA_CA_CERTS)
+            # self._mqttclient.tls_set()
+            self._mqttclient.tls_set_context(context)
+        else:
+            self._mqttclient = None
+        self._httpsession = requests.Session()
+        # Base URL setup
+        self._baseurl = "device." + self._config.region + ".anedya.io"
+        headers = {'Content-type': 'application/json',
+                   'Auth-mode': self._config.authmode,
+                   'Authorization': self._config.connection_key}
+        self._httpsession.headers.update(headers)
         return
 
     def set_config(self, config: AnedyaConfig):
         """
         Initialize the Anedya SDK.
 
         Args:
             config (AnedyaConfig): Anedya SDK configuration.
         """
         if config.connection_key == "":
-            raise ValueError('Configuration: connection key can not be empty!')
-        if config._deviceid_set == False:
-            raise ValueError('Configuration: need to set a valid Device ID')
+            raise AnedyaInvalidConfig(
+                'Configuration: connection key can not be empty!')
+        if config._deviceid_set is False:
+            raise AnedyaInvalidConfig(
+                'Configuration: need to set a valid Device ID')
         self._config = config
-        # Create 
-        
-    def bind_device(self, binding_secret: str):
-        """
-        Bind device to Anedya Cloud
-        """
-        headers = {'Content-type': 'application/json', 'Auth-mode': self._config.authmode, 'Authorization' : self._config.connection_key}
-        if self._config._testmode :
-            url = "https://device.stageapi.anedya.io/v1/submitData"
-        else:
-            url = "https://device." + self._config.region + ".anedya.io/v1/bindDevice/json"
-        requestPayload = {"bindingsecret" : binding_secret, "deviceid" : str(self._config._deviceID)}
-        r = requests.post(url, data=json.dumps(requestPayload), headers=headers)
-        jsonResponse = r.json()
-        if r.status_code != 200:
-            raise Exception(jsonResponse)
-        # Check whether the call was successful or not
-        if jsonResponse["success"] != True:
-            raise Exception(jsonResponse)
-        return True
-    
-    def submit_data(self, d: batch):
-        """
-        Send data to Anedya Cloud
-        """
-        headers = {'Content-type': 'application/json', 'Auth-mode': self._config.authmode, 'Authorization' : self._config.connection_key}
-        if self._config._testmode :
-            url = "https://device.stageapi.anedya.io/v1/submitData"
-        else:
-            url = "https://device." + self._config.region + ".anedya.io/v1/submitData"
-        r = requests.post(url, data=d.encodeJSON(), headers=headers)
-        #print(r.json())
-        if r.status_code != 200:
-            jsonResponse = r.json()
-            print(jsonResponse)
-            return False
-        return True
-    
-    def get_time_http(self):
-        """
-        Get current time from Anedya Time Service using HTTP request - Gets current time using HTTP requests.
-        Accuracy is generally within few tens of millisecond. For greater accuracy consider using NTP time service from Anedya
-        """
-        #print("called time API")
-        if self._config._testmode :
-            url = "https://device.stageapi.anedya.io/v1/time"
-        else:
-            url = "https://device." + self._config.region + ".anedya.io/v1/time"
-        deviceSendTime = int(time.time_ns()/1000000)
-        requestPayload = {"deviceSendTime" : deviceSendTime}
-        #print(json.dumps(requestPayload))
-        headers = {'Content-type': 'application/json'}
-        r = requests.post(url, data=json.dumps(requestPayload), headers=headers)
-        deviceRecTime = int(time.time_ns()/1000000)
-        jsonResponse = r.json()
-        #print(jsonResponse)
-        if r.status_code != 200:
-            raise Exception(jsonResponse)
-        # Now compute the time from response
-        ServerReceiveTime = jsonResponse["serverReceiveTime"]
-        ServerSendTime = jsonResponse["serverSendTime"]
-        currentTime = (ServerReceiveTime + ServerSendTime + deviceRecTime - deviceSendTime)/2
-        return currentTime
-        
+        return
+
+    def connect(self):
+        if self._config.connection_mode == ConnectionMode.HTTP:
+            raise AnedyaInvalidConfig(
+                'Connection mode is HTTP, connect is not supported')
+        if self._config.mqtt_mode == MQTTMode.TCP:
+            print(self._mqttclient)
+            self._mqttclient.loop_start()
+            print("device." + self._config.region + ".anedya.io")
+            err = self._mqttclient.connect(
+                host="device.ap-in-1.anedya.io", port=8804,
+                keepalive=60)
+            print(err)
+        # Start the loop
+
+    def disconnect(self):
+        self._mqttclient.disconnect()
+        return
+
+    from .client.bindDevice import bind_device
+    from .client.submitData import submit_data
+    from .client.timeSync import get_time
+    from .client.mqttHandlers import onconnect_handler, ondisconnect_handler
+    from .client.callbacks import _error_callback, _response_callback
```

### Comparing `anedya-dev-sdk-0.0.9/src/anedya_dev_sdk.egg-info/PKG-INFO` & `anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.0.9
-Summary: Anedya python based SDK for IoT devices. This SDK is currently under development. Future versions may include breaking changes.
+Version: 0.1.0
+Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Project-URL: Source, https://github.com/anedyaio/anedya-dev-sdk-pyhton
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
+
+<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">
+<img src="https://cdn.anedya.io/android-chrome-512x512.png" style="width:50%; margin:0 auto;">
+</div>
 
 # Anedya SDK
 
 <p>
     <a href="https://pypi.org/project/anedya-dev-sdk/">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk?style=for-the-badge">
     </a>
 </p>
 
 
 The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
 
 This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io)
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.0.9 Summary: Anedya
-python based SDK for IoT devices. This SDK is currently under development.
-Future versions may include breaking changes. Home-page: https://github.com/
-anedyaio/anedya-dev-sdk-pyhton Author: Anedya Systems Author-email:
-support@anedya.io License: Apache License 2.0 Project-URL: Documentation,
-https://docs.anedya.io Project-URL: Release notes, https://github.com/anedyaio/
-anedya-dev-sdk-pyhton Project-URL: Source, https://github.com/anedyaio/anedya-
-dev-sdk-pyhton Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: requests # Anedya SDK
+Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.1.0 Summary: Anedya
+python based SDK for IoT devices. This SDK streamlines connectivity with Anedya
+platform. As this SDK is in Beta release, future versions may have breaking
+changes. Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton Author:
+Anedya Systems Author-email: support@anedya.io License: Apache License 2.0
+Project-URL: Documentation, https://docs.anedya.io Project-URL: Release notes,
+https://github.com/anedyaio/anedya-dev-sdk-pyhton Project-URL: Source, https://
+github.com/anedyaio/anedya-dev-sdk-pyhton Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Description-
+Content-Type: text/markdown License-File: LICENSE
+[https://cdn.anedya.io/android-chrome-512x512.png]
+# Anedya SDK
 _[_P_y_P_I_]
 The **Anedya SDK** is a Python package designed to provide an easy-to-use
 interface for [Anedya](https://anedya.io) cloud services, which enables
 seamless connectivity and data retrieval from IoT devices. This SDK supports
 both MQTT and HTTP communication methods. This SDK wraps the Device APIs
 available in the [Anedya Documentation](https://docs.anedya.io) This is a
 Device SDK, i.e. it is meant to be used by an IoT device. ## Installation To
```

### Comparing `anedya-dev-sdk-0.0.9/tests/test_config.py` & `anedya-dev-sdk-0.1.0/tests/test_config.py`

 * *Files identical despite different names*

