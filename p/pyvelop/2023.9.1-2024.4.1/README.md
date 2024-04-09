# Comparing `tmp/pyvelop-2023.9.1.tar.gz` & `tmp/pyvelop-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvelop-2023.9.1.tar", last modified: Fri Sep 15 20:17:00 2023, max compression
+gzip compressed data, was "pyvelop-2024.4.1.tar", last modified: Tue Apr  9 19:47:53 2024, max compression
```

## Comparing `pyvelop-2023.9.1.tar` & `pyvelop-2024.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-09-15 20:17:00.842848 pyvelop-2023.9.1/
--rw-rw-rw-   0        0        0     1696 2023-09-15 20:17:00.842848 pyvelop-2023.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-09-15 20:17:00.797899 pyvelop-2023.9.1/pyvelop/
--rw-rw-rw-   0        0        0      716 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/__init__.py
--rw-rw-rw-   0        0        0    37288 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/__main__.py
--rw-rw-rw-   0        0        0     7194 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/base.py
--rw-rw-rw-   0        0        0      226 2023-09-15 20:13:14.000000 pyvelop-2023.9.1/pyvelop/const.py
--rw-rw-rw-   0        0        0      598 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/decorators.py
--rw-rw-rw-   0        0        0    12640 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/device.py
--rw-rw-rw-   0        0        0     3139 2023-09-15 15:41:47.000000 pyvelop-2023.9.1/pyvelop/exceptions.py
--rw-rw-rw-   0        0        0    12421 2023-09-15 15:41:47.000000 pyvelop-2023.9.1/pyvelop/jnap.py
--rw-rw-rw-   0        0        0      788 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/logger.py
--rw-rw-rw-   0        0        0    63307 2023-09-15 15:41:47.000000 pyvelop-2023.9.1/pyvelop/mesh.py
--rw-rw-rw-   0        0        0     5403 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/pyvelop/node.py
-drwxrwxrwx   0        0        0        0 2023-09-15 20:17:00.842848 pyvelop-2023.9.1/pyvelop.egg-info/
--rw-rw-rw-   0        0        0     1696 2023-09-15 20:17:00.000000 pyvelop-2023.9.1/pyvelop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-09-15 20:17:00.000000 pyvelop-2023.9.1/pyvelop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-15 20:17:00.000000 pyvelop-2023.9.1/pyvelop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-09-15 20:17:00.000000 pyvelop-2023.9.1/pyvelop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-09-15 20:17:00.000000 pyvelop-2023.9.1/pyvelop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-15 20:17:00.842848 pyvelop-2023.9.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-09-15 10:51:10.000000 pyvelop-2023.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:47:53.328832 pyvelop-2024.4.1/
+-rw-rw-rw-   0        0        0     1696 2024-04-09 19:47:53.327847 pyvelop-2024.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2024-04-09 19:21:23.000000 pyvelop-2024.4.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-09 19:47:53.316844 pyvelop-2024.4.1/pyvelop/
+-rw-rw-rw-   0        0        0      716 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/__init__.py
+-rw-rw-rw-   0        0        0    37881 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/__main__.py
+-rw-rw-rw-   0        0        0     7204 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/base.py
+-rw-rw-rw-   0        0        0      226 2024-04-09 19:41:32.000000 pyvelop-2024.4.1/pyvelop/const.py
+-rw-rw-rw-   0        0        0      598 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/decorators.py
+-rw-rw-rw-   0        0        0    12640 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/device.py
+-rw-rw-rw-   0        0        0     3139 2023-09-15 15:41:47.000000 pyvelop-2024.4.1/pyvelop/exceptions.py
+-rw-rw-rw-   0        0        0    12421 2023-09-15 15:41:47.000000 pyvelop-2024.4.1/pyvelop/jnap.py
+-rw-rw-rw-   0        0        0      788 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/pyvelop/logger.py
+-rw-rw-rw-   0        0        0    63755 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/mesh.py
+-rw-rw-rw-   0        0        0     6059 2024-04-09 19:23:12.000000 pyvelop-2024.4.1/pyvelop/node.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:47:53.325832 pyvelop-2024.4.1/pyvelop.egg-info/
+-rw-rw-rw-   0        0        0     1696 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 19:47:53.000000 pyvelop-2024.4.1/pyvelop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 19:47:53.328832 pyvelop-2024.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-09-15 10:51:10.000000 pyvelop-2024.4.1/setup.py
```

### Comparing `pyvelop-2023.9.1/PKG-INFO` & `pyvelop-2024.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2023.9.1
+Version: 2024.4.1
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 pyvelop
```

### Comparing `pyvelop-2023.9.1/README.rst` & `pyvelop-2024.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/__init__.py` & `pyvelop-2024.4.1/pyvelop/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/__main__.py` & `pyvelop-2024.4.1/pyvelop/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,25 +354,27 @@
                                 speedtest_results=mesh_obj.latest_speedtest_result
                             ),
                         ),
                         ("dhcp_enabled", "DHCP Enabled"),
                         (
                             "dhcp_reservations",
                             "DHCP Reservations",
-                            prefix
-                            + prefix.join(
-                                [
-                                    f"{reservation.get('description')},"
-                                    f"{reservation.get('mac_address')},"
-                                    f"{reservation.get('ip_address')}"
-                                    for reservation in mesh_obj.dhcp_reservations
-                                ]
-                            )
-                            if len(mesh_obj.dhcp_reservations)
-                            else "None",
+                            (
+                                prefix
+                                + prefix.join(
+                                    [
+                                        f"{reservation.get('description')},"
+                                        f"{reservation.get('mac_address')},"
+                                        f"{reservation.get('ip_address')}"
+                                        for reservation in mesh_obj.dhcp_reservations
+                                    ]
+                                )
+                                if len(mesh_obj.dhcp_reservations)
+                                else "None"
+                            ),
                         ),
                         ("parental_control_enabled", "Parental Control Enabled"),
                         ("wps_state", "WPS Enabled"),
                         ("is_channel_scan_running", "Channel Scan Running"),
                         ("homekit_enabled", "HomeKit Integration Enabled"),
                         ("homekit_paired", "HomeKit Integration Paired"),
                         ("client_steering_enabled", "Client Steering Enabled"),
@@ -551,29 +553,33 @@
                                             indent=indent,
                                             mappings=[
                                                 ("parent_name", "Parent"),
                                                 ("connection", "Connection type"),
                                                 (
                                                     "speed_mbps",
                                                     "Speed",
-                                                    f"{found_node.backhaul.get('speed_mbps')}mbps"
-                                                    if found_node.backhaul.get(
-                                                        "speed_mbps"
-                                                    )
-                                                    else None,
+                                                    (
+                                                        f"{found_node.backhaul.get('speed_mbps')}mbps"
+                                                        if found_node.backhaul.get(
+                                                            "speed_mbps"
+                                                        )
+                                                        else None
+                                                    ),
                                                 ),
                                                 ("signal_strength", "Signal strength"),
                                                 (
                                                     "rssi_dbm",
                                                     "RSSI",
-                                                    f"{found_node.backhaul.get('rssi_dbm')}dBm"
-                                                    if found_node.backhaul.get(
-                                                        "rssi_dbm"
-                                                    )
-                                                    else None,
+                                                    (
+                                                        f"{found_node.backhaul.get('rssi_dbm')}dBm"
+                                                        if found_node.backhaul.get(
+                                                            "rssi_dbm"
+                                                        )
+                                                        else None
+                                                    ),
                                                 ),
                                                 ("last_checked", "Last checked"),
                                             ],
                                             obj=dict(
                                                 **found_node.backhaul,
                                                 parent_name=found_node.parent_name,
                                             ),
@@ -782,23 +788,26 @@
 
     ret = _build_display_data(
         indent=indent,
         mappings=[
             ("mac", "MAC"),
             ("ip", "IPv4"),
             ("ipv6", "IPv6"),
+            ("primary", "Primary Adapter"),
             ("reservation", "Reservation"),
             ("reservation_description", "Reserved Name"),
             ("guest_network", "Guest"),
             (
                 "signal_strength",
                 "Signal Strength",
-                f"{adapter.get('signal_strength', None)} ({adapter.get('rssi', None)}dBm)"
-                if adapter.get("signal_strength", None)
-                else "N/A",
+                (
+                    f"{adapter.get('signal_strength', None)} ({adapter.get('rssi', None)}dBm)"
+                    if adapter.get("signal_strength", None)
+                    else "N/A"
+                ),
             ),
         ],
         obj=adapter,
     )
 
     return "\n" + ret.rstrip()
 
@@ -874,32 +883,36 @@
     prefix: str = f"\n{indent * 2 * ' '}"
     ret: str = _build_display_data(
         indent=indent,
         mappings=[
             (
                 "blocked_internet_access",
                 "Blocked Access",
-                prefix
-                + prefix.join(
-                    [
-                        f"{day.title()}: {', '.join(times) if times else 'N/A'}"
-                        for day, times in schedule.get(
-                            "blocked_internet_access", {}
-                        ).items()
-                    ]
-                )
-                if schedule.get("blocked_internet_access", {})
-                else "N/A",
+                (
+                    prefix
+                    + prefix.join(
+                        [
+                            f"{day.title()}: {', '.join(times) if times else 'N/A'}"
+                            for day, times in schedule.get(
+                                "blocked_internet_access", {}
+                            ).items()
+                        ]
+                    )
+                    if schedule.get("blocked_internet_access", {})
+                    else "N/A"
+                ),
             ),
             (
                 "blocked_sites",
                 "Prohibited Sites",
-                prefix + prefix.join(schedule.get("blocked_sites", []))
-                if schedule.get("blocked_sites", [])
-                else "N/A",
+                (
+                    prefix + prefix.join(schedule.get("blocked_sites", []))
+                    if schedule.get("blocked_sites", [])
+                    else "N/A"
+                ),
             ),
         ],
         obj=schedule,
     )
 
     return "\n" + ret.rstrip()
```

### Comparing `pyvelop-2023.9.1/pyvelop/base.py` & `pyvelop-2024.4.1/pyvelop/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             if conn_details.get("macAddress", "").lower() == mac.lower():
                 ret["rssi"] = conn_details.get("wireless", {}).get("signalDecibels")
                 ret["signal_strength"] = signal_strength_to_text(ret["rssi"])
 
         return ret
 
     @property
-    def connected_adapters(self) -> List[dict]:
+    def connected_adapters(self) -> List[dict[str, Any]]:
         """Get the network adapters that are connected to the mesh.
 
         :return: a list of dictionaries that contain the MAC, IP and Guest Network status of the adapter
         """
         ret: List[Dict[str, Any]] = []
 
         for adapter in self._attribs.get("connections", []):
```

### Comparing `pyvelop-2023.9.1/pyvelop/decorators.py` & `pyvelop-2024.4.1/pyvelop/decorators.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/device.py` & `pyvelop-2024.4.1/pyvelop/device.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/exceptions.py` & `pyvelop-2024.4.1/pyvelop/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/jnap.py` & `pyvelop-2024.4.1/pyvelop/jnap.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/logger.py` & `pyvelop-2024.4.1/pyvelop/logger.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.9.1/pyvelop/mesh.py` & `pyvelop-2024.4.1/pyvelop/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,16 +218,16 @@
 
         self._node: str = node
         self._mesh_attributes: Dict = {}
         self._session: aiohttp.ClientSession = session
         self._timeout: int = request_timeout or 10
 
         # flag used to denote that a full gather has been executed
-        self.__gather_details_executed: bool = (  # pylint: disable=unused-private-member
-            False
+        self.__gather_details_executed: bool = (
+            False  # pylint: disable=unused-private-member
         )
 
         self.__username: str = username
         self.__password: str = password
         self.__passed_session: bool = False
 
         _LOGGER.debug(
@@ -265,15 +265,15 @@
     # region #-- private methods --#
     async def _async_make_request(
         self,
         action: str,
         node_address: str | None = None,
         payload: List[Dict] | Dict | None = None,
         raise_on_error: bool = True,
-    ) -> Tuple(api.Request, api.Response):
+    ) -> Tuple[api.Request, api.Response]:
         """Execute the API request against the connected node.
 
         :param action: The JNAP action to execute
         :param node_address: The node to send the request to (only valid for a subset of actions)
         :param payload: The relevant payload for the action
         :param raise_on_error: Raise an error if one is found
         :return: tuple containing the request and response objects or raises an error if need be
@@ -386,15 +386,15 @@
 
         # region #-- handle devices --#
         devices: List[Device | Node] = []
         # region #-- build the properties for the device types --#
         for device in ret.get(JNAPActionMappings.GET_DEVICES.value, {}).get(
             "devices", []
         ):
-            device["results_time"]: int = int(time.time())
+            device["results_time"] = int(time.time())
             if "nodeType" not in device:
                 devices.append(Device(**device))
             else:
                 # region #-- determine the backhaul information --#
                 device_backhaul = [
                     bi
                     for bi in ret.get(JNAPActionMappings.GET_BACKHAUL.value, {}).get(
@@ -603,17 +603,17 @@
 
         Sets the instance variables as necessary.
 
         :return: None
         """
         _LOGGER.debug(self._log_formatter.format("entered"))
 
-        self._mesh_attributes: Dict[
-            int | str, List[Device | Node] | Dict[str, Any]
-        ] = await self._async_gather_details(props=JNAPActionMappings.CMP_MESH_DETAILS)
+        self._mesh_attributes: Dict[int | str, List[Device | Node] | Dict[str, Any]] = (
+            await self._async_gather_details(props=JNAPActionMappings.CMP_MESH_DETAILS)
+        )
 
         self.__gather_details_executed = True  # pylint: disable=unused-private-member
         _LOGGER.debug(self._log_formatter.format("exited"))
 
     async def async_get_channel_scan_info(self) -> Dict[str, Any]:
         """Get the current state of the channel scan."""
         resp = await self._async_gather_details(
@@ -830,19 +830,25 @@
         ]
         if not node_details:
             raise MeshDeviceNotFoundResponse
 
         if node_details[0].type == NodeType.PRIMARY and not force:
             raise MeshInvalidInput(f"{node_name} is a primary node. Use the force.")
 
-        node_ip = [
+        # node_ip = [
+        #     adapter.get("ip")
+        #     for adapter in node_details[0].network
+        #     if adapter.get("ip")
+        # ]
+        node_ip: List[str] | None = [
             adapter.get("ip")
-            for adapter in node_details[0].network
-            if adapter.get("ip")
+            for adapter in node_details[0].connected_adapters
+            if adapter.get("ip") and adapter.get("primary")
         ]
+
         if not node_ip:
             raise MeshInvalidInput(f"{node_name}: no valid address found")
 
         await self._async_make_request(
             action=api.Actions.REBOOT, node_address=node_ip[0]
         )
 
@@ -931,18 +937,18 @@
         )
         device_mac: str = device[0].network[0].get("mac", None)
         if device_mac is None:
             raise MeshException("No MAC available")
         # endregion
 
         # -- get the current rules as they may have changed --#
-        current_parental_control_info: Dict[
-            int | str, Any
-        ] = await self._async_gather_details(
-            props=JNAPActionMappings.GET_PARENTAL_CONTROL_INFO
+        current_parental_control_info: Dict[int | str, Any] = (
+            await self._async_gather_details(
+                props=JNAPActionMappings.GET_PARENTAL_CONTROL_INFO
+            )
         )
         current_parental_control_info = current_parental_control_info.get(
             JNAPActionMappings.GET_PARENTAL_CONTROL_INFO.value, {}
         )
 
         # region #-- determine the rules --#
         keep_rules: List[Dict[str, Any]] = [
@@ -997,32 +1003,36 @@
                     this_device_rules = []
         # endregion
 
         requests: List = [  # build a list of requests to send
             self._async_make_request(
                 action=api.Actions.SET_PARENTAL_CONTROL_INFO,
                 payload={
-                    "isParentalControlEnabled": True
-                    if force_enable
-                    else current_parental_control_info.get(
-                        "isParentalControlEnabled", True
+                    "isParentalControlEnabled": (
+                        True
+                        if force_enable
+                        else current_parental_control_info.get(
+                            "isParentalControlEnabled", True
+                        )
                     ),
                     "rules": keep_rules + this_device_rules,
                 },
             )
         ]
 
         # region #-- calculate the device properties to update --#
-        device_properties: Dict[
-            str, List[str, Dict[str, str]]
-        ] = _get_parental_control_device_attributes(
-            schedule=new_rule,
-            urls=this_device_rules[0].get("blockedURLs", [])
-            if this_device_rules
-            else [],
+        device_properties: Dict[str, List[str, Dict[str, str]]] = (
+            _get_parental_control_device_attributes(
+                schedule=new_rule,
+                urls=(
+                    this_device_rules[0].get("blockedURLs", [])
+                    if this_device_rules
+                    else []
+                ),
+            )
         )
         if new_rule == ParentalControl.ALL_PAUSED_SCHEDULE():
             if current_schedule:
                 device_properties["modify"].append(
                     {
                         "name": "actualWanSchedule",
                         "value": ParentalControl.encode_for_backup(
@@ -1092,18 +1102,18 @@
         )
         device_mac: str = device[0].network[0].get("mac", None)
         if device_mac is None:
             raise MeshException("No MAC available")
         # endregion
 
         # -- get the current rules as they may have changed --#
-        current_parental_control_info: Dict[
-            int | str, Any
-        ] = await self._async_gather_details(
-            props=JNAPActionMappings.GET_PARENTAL_CONTROL_INFO
+        current_parental_control_info: Dict[int | str, Any] = (
+            await self._async_gather_details(
+                props=JNAPActionMappings.GET_PARENTAL_CONTROL_INFO
+            )
         )
         current_parental_control_info = current_parental_control_info.get(
             JNAPActionMappings.GET_PARENTAL_CONTROL_INFO.value, {}
         )
 
         # region #-- determine the rules --#
         keep_rules: List[Dict[str, Any]] = [
@@ -1132,28 +1142,30 @@
                 this_device_rules[0]["blockedURLs"] = urls
             this_device_rules[0]["blockedURLs"] = list(
                 set(this_device_rules[0]["blockedURLs"])
             )
         # endregion
 
         # region #-- build a list of requests to send --#
-        device_properties: Dict[
-            str, List[str | Dict[str, str]]
-        ] = _get_parental_control_device_attributes(
-            schedule=this_device_rules[0].get("wanSchedule", {}), urls=urls
+        device_properties: Dict[str, List[str | Dict[str, str]]] = (
+            _get_parental_control_device_attributes(
+                schedule=this_device_rules[0].get("wanSchedule", {}), urls=urls
+            )
         )
 
         requests: List = [
             self._async_make_request(
                 action=api.Actions.SET_PARENTAL_CONTROL_INFO,
                 payload={
-                    "isParentalControlEnabled": True
-                    if force_enable
-                    else current_parental_control_info.get(
-                        "isParentalControlEnabled", True
+                    "isParentalControlEnabled": (
+                        True
+                        if force_enable
+                        else current_parental_control_info.get(
+                            "isParentalControlEnabled", True
+                        )
                     ),
                     "rules": keep_rules
                     + (
                         this_device_rules
                         if "showInPCList" not in device_properties["remove"]
                         else []
                     ),
```

### Comparing `pyvelop-2023.9.1/pyvelop/node.py` & `pyvelop-2024.4.1/pyvelop/node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Represents a node in the mesh."""
 
 # region #-- imports --#
 from __future__ import annotations
 
 from enum import Enum
-from typing import List
+from typing import Any, List
 
 from . import signal_strength_to_text
 from .base import MeshDevice
 
 # endregion
 
 
@@ -54,14 +54,31 @@
                 "rssi_dbm": signal_strength_raw,
                 "signal_strength": signal_strength_to_text(rssi=signal_strength_raw),
             }
 
         return ret
 
     @property
+    def connected_adapters(self) -> List[dict[str, Any]]:
+        """Get the network adapters that are connected to the mesh.
+
+        :return: a list of dictionaries that contain the MAC, IP and Guest Network status of the adapter
+        """
+
+        ret: List[dict[str, Any]] = []
+        super_adapters: List[dict] = super().connected_adapters
+        backhaul = self._attribs.get("backhaul", {})
+        for adapter in super_adapters:
+            adapter["primary"] = (
+                True if adapter.get("ip") == backhaul.get("ipAddress") else False
+            )
+            ret += [adapter]
+        return ret
+
+    @property
     def connected_devices(self) -> List:
         """List of the devices that are connected to the node.
 
         :return: List of connected devices in alphabetical order sorted by device name
         """
         connected_devices = self.__connected_devices
         return sorted(connected_devices, key=lambda device: device.get("name"))
```

### Comparing `pyvelop-2023.9.1/pyvelop.egg-info/PKG-INFO` & `pyvelop-2024.4.1/pyvelop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2023.9.1
+Version: 2024.4.1
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 pyvelop
```

### Comparing `pyvelop-2023.9.1/setup.py` & `pyvelop-2024.4.1/setup.py`

 * *Files identical despite different names*

