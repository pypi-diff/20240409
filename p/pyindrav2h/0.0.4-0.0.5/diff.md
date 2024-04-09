# Comparing `tmp/pyindrav2h-0.0.4.tar.gz` & `tmp/pyindrav2h-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyindrav2h-0.0.4.tar", last modified: Sun Apr  7 18:30:35 2024, max compression
+gzip compressed data, was "pyindrav2h-0.0.5.tar", last modified: Mon Apr  8 17:43:19 2024, max compression
```

## Comparing `pyindrav2h-0.0.4.tar` & `pyindrav2h-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.836485 pyindrav2h-0.0.4/
--rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.4/LICENSE
--rw-r--r--   0 paulmorris   (501) staff       (20)     4371 2024-04-07 18:30:35.835671 pyindrav2h-0.0.4/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)     2575 2024-04-07 18:19:36.000000 pyindrav2h-0.0.4/README.md
--rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-07 18:20:14.000000 pyindrav2h-0.0.4/pyproject.toml
--rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-07 18:30:35.836703 pyindrav2h-0.0.4/setup.cfg
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.823136 pyindrav2h-0.0.4/src/
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.828579 pyindrav2h-0.0.4/src/pyindrav2h/
--rw-r--r--   0 paulmorris   (501) staff       (20)      202 2024-04-07 18:20:26.000000 pyindrav2h-0.0.4/src/pyindrav2h/__init__.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     2742 2024-04-07 18:14:52.000000 pyindrav2h-0.0.4/src/pyindrav2h/cli.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     5079 2024-04-07 16:17:53.000000 pyindrav2h-0.0.4/src/pyindrav2h/connection.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      736 2024-04-07 15:13:50.000000 pyindrav2h-0.0.4/src/pyindrav2h/exceptions.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      551 2024-04-04 19:31:06.000000 pyindrav2h-0.0.4/src/pyindrav2h/v2hclient.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     4374 2024-04-07 17:58:54.000000 pyindrav2h-0.0.4/src/pyindrav2h/v2hdevice.py
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.834760 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/
--rw-r--r--   0 paulmorris   (501) staff       (20)     4371 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/SOURCES.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/dependency_links.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/entry_points.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/requires.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/top_level.txt
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-08 17:43:19.420943 pyindrav2h-0.0.5/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.5/LICENSE
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4451 2024-04-08 17:43:19.420103 pyindrav2h-0.0.5/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)     2655 2024-04-08 17:37:43.000000 pyindrav2h-0.0.5/README.md
+-rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-08 17:30:57.000000 pyindrav2h-0.0.5/pyproject.toml
+-rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-08 17:43:19.421123 pyindrav2h-0.0.5/setup.cfg
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-08 17:43:19.401087 pyindrav2h-0.0.5/src/
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-08 17:43:19.409430 pyindrav2h-0.0.5/src/pyindrav2h/
+-rw-r--r--   0 paulmorris   (501) staff       (20)      202 2024-04-08 17:31:08.000000 pyindrav2h-0.0.5/src/pyindrav2h/__init__.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     3024 2024-04-08 17:28:12.000000 pyindrav2h-0.0.5/src/pyindrav2h/cli.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     5079 2024-04-08 17:15:18.000000 pyindrav2h-0.0.5/src/pyindrav2h/connection.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      736 2024-04-07 15:13:50.000000 pyindrav2h-0.0.5/src/pyindrav2h/exceptions.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      899 2024-04-08 17:26:34.000000 pyindrav2h-0.0.5/src/pyindrav2h/v2hclient.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4438 2024-04-08 16:55:40.000000 pyindrav2h-0.0.5/src/pyindrav2h/v2hdevice.py
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-08 17:43:19.419067 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4451 2024-04-08 17:43:19.000000 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-08 17:43:19.000000 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/SOURCES.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-08 17:43:19.000000 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/dependency_links.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-08 17:43:19.000000 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/entry_points.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-08 17:43:19.000000 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/requires.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-08 17:43:19.000000 pyindrav2h-0.0.5/src/pyindrav2h.egg-info/top_level.txt
```

### Comparing `pyindrav2h-0.0.4/LICENSE` & `pyindrav2h-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.4/PKG-INFO` & `pyindrav2h-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.4
+Version: 0.0.5
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,22 +60,23 @@
 ```
 On installation a CLI will become available: ```indracli```
 ## Usage/Examples
 
 ### CLI
 
 ```bash
-usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
+usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,alldevices,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
 
 Indra V2H CLI
 
 positional arguments:
-  {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
+  {statistics,device,alldevices,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
     statistics          show device statistics
     device              show device info
+    alldevices          show data on all available devices
     all                 show all info
     loadmatch           set mode to load matching
     idle                set mode to IDLE
     exportmatch         set mode to export matching
     charge              set mode to CHARGE
     discharge           set mode to discharge
     schedule            return to scheuduled mode
@@ -102,15 +103,15 @@
 Documentation to follow.
 
 ## Support
 
 This is a community project that lacks formal support.
 
 
-For support from the community please join the Indra V2H trial support community: https://indra.v2h.zendesk.com/hc/en-gb/community/topics
+For support from the community please join the Indra V2H trial support community: https://indrav2h.zendesk.com/hc/en-gb/community/topics
 
 
 
 For bugs or feature requests please create a GitHub Issue: https://github.com/creatingwake/pyindrav2h/issues
 
 ---
 #### NOTE: Please do not contact Indra Support.  Indra are unable to assist with unofficial API integrations.
```

### Comparing `pyindrav2h-0.0.4/README.md` & `pyindrav2h-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 ```
 On installation a CLI will become available: ```indracli```
 ## Usage/Examples
 
 ### CLI
 
 ```bash
-usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
+usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,alldevices,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
 
 Indra V2H CLI
 
 positional arguments:
-  {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
+  {statistics,device,alldevices,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
     statistics          show device statistics
     device              show device info
+    alldevices          show data on all available devices
     all                 show all info
     loadmatch           set mode to load matching
     idle                set mode to IDLE
     exportmatch         set mode to export matching
     charge              set mode to CHARGE
     discharge           set mode to discharge
     schedule            return to scheuduled mode
@@ -64,15 +65,15 @@
 Documentation to follow.
 
 ## Support
 
 This is a community project that lacks formal support.
 
 
-For support from the community please join the Indra V2H trial support community: https://indra.v2h.zendesk.com/hc/en-gb/community/topics
+For support from the community please join the Indra V2H trial support community: https://indrav2h.zendesk.com/hc/en-gb/community/topics
 
 
 
 For bugs or feature requests please create a GitHub Issue: https://github.com/creatingwake/pyindrav2h/issues
 
 ---
 #### NOTE: Please do not contact Indra Support.  Indra are unable to assist with unofficial API integrations.
```

### Comparing `pyindrav2h-0.0.4/pyproject.toml` & `pyindrav2h-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyindrav2h"
-version = "0.0.4"
+version = "0.0.5"
 description = "API client and example CLI to interact with Indra V2H Chargers"
 readme = "README.md"
 authors = [{ name = "Paul Morris", email = "paul@creatingwake.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyindrav2h-0.0.4/src/pyindrav2h/cli.py` & `pyindrav2h-0.0.5/src/pyindrav2h/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from getpass import getpass
 import argparse
 import configparser
 import asyncio
 import os
+import json
 from .connection import Connection
 from .v2hclient import v2hClient
 from . import V2H_MODES
 
 logging.basicConfig()
 logging.root.setLevel(logging.WARNING)
 
@@ -20,20 +21,25 @@
     if args.debug:
         logging.root.setLevel(logging.DEBUG)
 
     _LOGGER.debug(f"using {userEmail}, {userPass}")
 
     # create connection
     conn = Connection(userEmail, userPass)
-    await conn.checkAPICreds()
+    # await conn.checkAPICreds()
 
     client = v2hClient(conn)
 
-    # refresh device/stats data
-    await client.refresh()
+    if (args.command == "alldevices"):
+        await client.refresh_device()
+        json_out = json.dumps(client.device.getDevices(), indent=2)
+        print(json_out)
+        exit()
+    
+    await client.refresh() # refresh device/stats data
 
     if args.command == "schedule":
         args.command = "clear" # translate displayed mode commmand to endpoint command
     if (args.command == "device"):
         print(client.device.showDevice())
     elif (args.command == "statistics"):
         print(client.device.showStats())
@@ -61,14 +67,15 @@
         dest="password",
         default=config.get("indra-account", "password")
     )
     parser.add_argument("-d", "--debug", dest="debug", action="store_true")
     subparsers = parser.add_subparsers(dest="command", required=True)
     subparsers.add_parser("statistics", help="show device statistics")
     subparsers.add_parser("device", help="show device info")
+    subparsers.add_parser("alldevices", help="show data on all available devices")
     subparsers.add_parser("all", help="show all info")
     subparsers.add_parser("loadmatch", help="set mode to load matching")
     subparsers.add_parser("idle", help="set mode to IDLE")
     subparsers.add_parser("exportmatch", help="set mode to export matching")
     subparsers.add_parser("charge", help="set mode to CHARGE")
     subparsers.add_parser("discharge", help="set mode to discharge")
     subparsers.add_parser("schedule", help="return to scheuduled mode")
```

### Comparing `pyindrav2h-0.0.4/src/pyindrav2h/connection.py` & `pyindrav2h-0.0.5/src/pyindrav2h/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     async def checkAPICreds(self):
         await self.updateBearerAuth()
         if self._bearerToken is None:
             raise WrongCredentialsException()
     
     async def send(self, method, url, json=None):
         if self._bearerToken is None:
-            _LOGGER.error("Missing BearerToken - calling updateBearerAuth()")
+            _LOGGER.debug("Missing BearerToken - calling updateBearerAuth()")
             await self.updateBearerAuth()
 
         async with httpx.AsyncClient(
             headers=self._headers, timeout=self.timeout
         ) as httpclient:
             for i in range(self._authRetries): # allow retries to obtain a new Bearer Auth token
                 try:
```

### Comparing `pyindrav2h-0.0.4/src/pyindrav2h/exceptions.py` & `pyindrav2h-0.0.5/src/pyindrav2h/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.4/src/pyindrav2h/v2hdevice.py` & `pyindrav2h-0.0.5/src/pyindrav2h/v2hdevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,7 +146,10 @@
         ret = ret + f"Temperature: {self.temperature}\n"
         ret = ret + f"Vehicle SoC: {self.soc}\n"
         ret = ret + f"Schedule active?: {not self.isInterrupted}\n"
         return ret
 
     def showAll(self):
         return self.showDevice() + "\n\n" + self.showStats()
+  
+    def getDevices(self):
+        return self.data["devices"]
```

### Comparing `pyindrav2h-0.0.4/src/pyindrav2h.egg-info/PKG-INFO` & `pyindrav2h-0.0.5/src/pyindrav2h.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.4
+Version: 0.0.5
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,22 +60,23 @@
 ```
 On installation a CLI will become available: ```indracli```
 ## Usage/Examples
 
 ### CLI
 
 ```bash
-usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
+usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,alldevices,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
 
 Indra V2H CLI
 
 positional arguments:
-  {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
+  {statistics,device,alldevices,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
     statistics          show device statistics
     device              show device info
+    alldevices          show data on all available devices
     all                 show all info
     loadmatch           set mode to load matching
     idle                set mode to IDLE
     exportmatch         set mode to export matching
     charge              set mode to CHARGE
     discharge           set mode to discharge
     schedule            return to scheuduled mode
@@ -102,15 +103,15 @@
 Documentation to follow.
 
 ## Support
 
 This is a community project that lacks formal support.
 
 
-For support from the community please join the Indra V2H trial support community: https://indra.v2h.zendesk.com/hc/en-gb/community/topics
+For support from the community please join the Indra V2H trial support community: https://indrav2h.zendesk.com/hc/en-gb/community/topics
 
 
 
 For bugs or feature requests please create a GitHub Issue: https://github.com/creatingwake/pyindrav2h/issues
 
 ---
 #### NOTE: Please do not contact Indra Support.  Indra are unable to assist with unofficial API integrations.
```

