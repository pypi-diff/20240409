# Comparing `tmp/yolink-api-0.4.2.tar.gz` & `tmp/yolink-api-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolink-api-0.4.2.tar", last modified: Sat Apr  6 13:22:21 2024, max compression
+gzip compressed data, was "yolink-api-0.4.3.tar", last modified: Tue Apr  9 03:45:27 2024, max compression
```

## Comparing `yolink-api-0.4.2.tar` & `yolink-api-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:21.328843 yolink-api-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-06 13:22:18.000000 yolink-api-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-06 13:22:21.328843 yolink-api-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-06 13:22:18.000000 yolink-api-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 13:22:18.000000 yolink-api-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:22:21.328843 yolink-api-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-06 13:22:18.000000 yolink-api-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:21.328843 yolink-api-0.4.2/yolink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/auth_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/home_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/message_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/message_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/outlet_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/thermostat_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/unit_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:21.328843 yolink-api-0.4.2/yolink_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:27.437464 yolink-api-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 03:45:22.000000 yolink-api-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-09 03:45:27.437464 yolink-api-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 03:45:22.000000 yolink-api-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 03:45:22.000000 yolink-api-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 03:45:27.437464 yolink-api-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 03:45:22.000000 yolink-api-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:27.437464 yolink-api-0.4.3/yolink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/auth_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/home_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/message_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/outlet_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/thermostat_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-09 03:45:22.000000 yolink-api-0.4.3/yolink/unit_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:45:27.437464 yolink-api-0.4.3/yolink_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 03:45:27.000000 yolink-api-0.4.3/yolink_api.egg-info/top_level.txt
```

### Comparing `yolink-api-0.4.2/LICENSE` & `yolink-api-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/PKG-INFO` & `yolink-api-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolink-api
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library to authenticate with yolink device
 Home-page: https://github.com/YoSmart-Inc/yolink-api
 Author: YoSmart
 License: MIT
 Project-URL: Bug Tracker, https://github.com/YoSmart-Inc/yolink-api/issues
 Keywords: yolink api
 Platform: UNKNOWN
```

### Comparing `yolink-api-0.4.2/README.md` & `yolink-api-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/setup.py` & `yolink-api-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="yolink-api",
-    version="0.4.2",
+    version="0.4.3",
     author="YoSmart",
     description="A library to authenticate with yolink device",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YoSmart-Inc/yolink-api",
     project_urls={
         "Bug Tracker": "https://github.com/YoSmart-Inc/yolink-api/issues",
```

### Comparing `yolink-api-0.4.2/yolink/auth_mgr.py` & `yolink-api-0.4.3/yolink/auth_mgr.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/client.py` & `yolink-api-0.4.3/yolink/client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/const.py` & `yolink-api-0.4.3/yolink/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 ATTR_DEVICE_ID = "deviceId"
 ATTR_DEVICE_NAME = "name"
 ATTR_DEVICE_TYPE = "type"
 ATTR_DEVICE_TOKEN = "token"
 ATTR_DEVICE_MODEL_NAME = "modelName"
 ATTR_DEVICE_PARENT_ID = "parentDeviceId"
+ATTR_DEVICE_SERVICE_ZONE = "serviceZone"
 
 ATTR_DEVICE_DOOR_SENSOR = "DoorSensor"
 ATTR_DEVICE_TH_SENSOR = "THSensor"
 ATTR_DEVICE_MOTION_SENSOR = "MotionSensor"
 ATTR_DEVICE_MULTI_OUTLET = "MultiOutlet"
 ATTR_DEVICE_LEAK_SENSOR = "LeakSensor"
 ATTR_DEVICE_VIBRATION_SENSOR = "VibrationSensor"
```

### Comparing `yolink-api-0.4.2/yolink/device.py` & `yolink-api-0.4.3/yolink/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .const import (
     ATTR_DEVICE_ID,
     ATTR_DEVICE_NAME,
     ATTR_DEVICE_TOKEN,
     ATTR_DEVICE_TYPE,
     ATTR_DEVICE_MODEL_NAME,
     ATTR_DEVICE_PARENT_ID,
+    ATTR_DEVICE_SERVICE_ZONE,
     ATTR_DEVICE_WATER_DEPTH_SENSOR,
     ATTR_DEVICE_WATER_METER_CONTROLLER,
 )
 from .client_request import ClientRequest
 from .message_resolver import (
     water_depth_sensor_message_resolve,
     water_meter_sensor_message_resolver,
@@ -37,14 +38,15 @@
 
     device_id: str = Field(alias=ATTR_DEVICE_ID)
     device_name: str = Field(alias=ATTR_DEVICE_NAME)
     device_token: str = Field(alias=ATTR_DEVICE_TOKEN)
     device_type: str = Field(alias=ATTR_DEVICE_TYPE)
     device_model_name: str = Field(alias=ATTR_DEVICE_MODEL_NAME)
     device_parent_id: Optional[str] = Field(alias=ATTR_DEVICE_PARENT_ID)
+    device_service_zone: Optional[str] = Field(alias=ATTR_DEVICE_SERVICE_ZONE)
 
     @validator("device_parent_id")
     def check_parent_id(cls, val):
         """Checking and replace parent id."""
         if val == "null":
             val = None
         return val
@@ -56,21 +58,28 @@
     def __init__(self, device: YoLinkDeviceMode, client: YoLinkClient) -> None:
         self.device_id: str = device.device_id
         self.device_name: str = device.device_name
         self.device_token: str = device.device_token
         self.device_type: str = device.device_type
         self.device_model_name: str = device.device_model_name
         self.device_attrs: dict | None = None
-        self.device_endpoint: Endpoint = (
-            Endpoints.EU.value
-            if device.device_model_name.endswith("-EC")
-            else Endpoints.US.value
-        )
         self.parent_id: str = device.device_parent_id
         self._client: YoLinkClient = client
+        if device.device_service_zone is not None:
+            self.device_endpoint: Endpoint = (
+                Endpoints.EU.value
+                if device.device_service_zone.startswith("eu_")
+                else Endpoints.US.value
+            )
+        else:
+            self.device_endpoint: Endpoint = (
+                Endpoints.EU.value
+                if device.device_model_name.endswith("-EC")
+                else Endpoints.US.value
+            )
 
     async def __invoke(self, method: str, params: dict | None) -> BRDP:
         """Invoke device."""
         try:
             bsdp_helper = BSDPHelper(
                 self.device_id,
                 self.device_token,
```

### Comparing `yolink-api-0.4.2/yolink/endpoint.py` & `yolink-api-0.4.3/yolink/endpoint.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/exception.py` & `yolink-api-0.4.3/yolink/exception.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/home_manager.py` & `yolink-api-0.4.3/yolink/home_manager.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/message_resolver.py` & `yolink-api-0.4.3/yolink/message_resolver.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/model.py` & `yolink-api-0.4.3/yolink/model.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/mqtt_client.py` & `yolink-api-0.4.3/yolink/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/outlet_request_builder.py` & `yolink-api-0.4.3/yolink/outlet_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/thermostat_request_builder.py` & `yolink-api-0.4.3/yolink/thermostat_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink/unit_helper.py` & `yolink-api-0.4.3/yolink/unit_helper.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.2/yolink_api.egg-info/PKG-INFO` & `yolink-api-0.4.3/yolink_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolink-api
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library to authenticate with yolink device
 Home-page: https://github.com/YoSmart-Inc/yolink-api
 Author: YoSmart
 License: MIT
 Project-URL: Bug Tracker, https://github.com/YoSmart-Inc/yolink-api/issues
 Keywords: yolink api
 Platform: UNKNOWN
```

### Comparing `yolink-api-0.4.2/yolink_api.egg-info/SOURCES.txt` & `yolink-api-0.4.3/yolink_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

