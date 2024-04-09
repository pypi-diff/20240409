# Comparing `tmp/moobius-1.1.6.tar.gz` & `tmp/moobius-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.1.6.tar", last modified: Wed Apr  3 05:37:41 2024, max compression
+gzip compressed data, was "moobius-1.1.7.tar", last modified: Tue Apr  9 05:35:07 2024, max compression
```

## Comparing `moobius-1.1.6.tar` & `moobius-1.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.324196 moobius-1.1.6/
--rw-rw-rw-   0        0        0     8910 2024-04-03 05:37:41.323200 moobius-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.6/license.md
--rw-rw-rw-   0        0        0      647 2024-04-03 04:47:09.000000 moobius-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.6/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-03 05:37:41.324196 moobius-1.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.303965 moobius-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.307116 moobius-1.1.6/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.6/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.314667 moobius-1.1.6/src/moobius/core/
--rw-rw-rw-   0        0        0    56123 2024-04-02 21:26:58.000000 moobius-1.1.6/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.6/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.317651 moobius-1.1.6/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.6/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4062 2024-03-25 06:01:03.000000 moobius-1.1.6/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.6/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.6/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.6/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.321207 moobius-1.1.6/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.6/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    43927 2024-04-02 20:28:42.000000 moobius-1.1.6/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25652 2024-04-02 21:30:49.000000 moobius-1.1.6/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-04-01 23:40:33.000000 moobius-1.1.6/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.6/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.322208 moobius-1.1.6/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8910 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-03-26 23:06:54.000000 moobius-1.1.6/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.293119 moobius-1.1.7/
+-rw-rw-rw-   0        0        0     8910 2024-04-09 05:35:07.292117 moobius-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.7/license.md
+-rw-rw-rw-   0        0        0      647 2024-04-09 04:35:53.000000 moobius-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.7/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:35:07.293119 moobius-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.275178 moobius-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.277172 moobius-1.1.7/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.7/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.283149 moobius-1.1.7/src/moobius/core/
+-rw-rw-rw-   0        0        0    57346 2024-04-09 05:09:27.000000 moobius-1.1.7/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.7/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.288132 moobius-1.1.7/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.7/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4062 2024-03-25 06:01:03.000000 moobius-1.1.7/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.7/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.7/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.7/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.291121 moobius-1.1.7/src/moobius/network/
+-rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.7/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    43927 2024-04-02 20:28:42.000000 moobius-1.1.7/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25652 2024-04-03 05:51:15.000000 moobius-1.1.7/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.1.7/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.7/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:35:07.292117 moobius-1.1.7/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8910 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 05:35:07.000000 moobius-1.1.7/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.1.7/src/setup.py
```

### Comparing `moobius-1.1.6/PKG-INFO` & `moobius-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.6
+Version: 1.1.7
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.6/license.md` & `moobius-1.1.7/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/pyproject.toml` & `moobius-1.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moobius"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Kevin Kostlan", email="sdk@moobius.app"},
 ]
 description = "Moobius Platform SDK"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moobius-1.1.6/readme.md` & `moobius-1.1.7/readme.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/core/sdk.py` & `moobius-1.1.7/src/moobius/core/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,22 @@
 
         self.queue = aioprocessing.AioQueue()
 
         self.refresh_interval = 6 * 60 * 60             # 24h expire, 6h refresh
         self.authenticate_interval = 7 * 24 * 60 * 60   # 30d expire, 7d refresh
         self.heartbeat_interval = 30                    # 30s heartbeat
         self.checkin_interval = 90
+        self.log_retention = kwargs.get('log_retention', {'rotation':"1 day", 'retention':"7 days"})
 
         self.scheduler = None
 
+        self.log_file = kwargs.get('log_file')
+        self.error_log_file = kwargs.get('error_log_file')
+        self.init_all_channels = kwargs.get('initialize_all_bound_channels')
+
     async def start(self):
         """
         Start the Service/Agent. start() fns are called with wand.run. There are 6 steps:
           1. Authenticate.
           2. Connect to the websocket server.
           3. (if a Service) Bind the Service to the channels. If there is no service_id in the config file, create a new service and update the config file.
           4. Start the scheduler, run refresh(), authenticate(), send_heartbeat() periodically.
@@ -240,17 +245,32 @@
         self.scheduler = AsyncIOScheduler()
 
         # The details of access_token and refresh_token are managed by self.http_api
         self.scheduler.add_job(self.refresh, 'interval', seconds=self.refresh_interval)
         self.scheduler.add_job(self.authenticate, 'interval', seconds=self.authenticate_interval)
         self.scheduler.add_job(self.send_heartbeat, 'interval', seconds=self.heartbeat_interval)
 
+        if self.log_file:
+            logger.add(self.log_file, level="DEBUG", **self.log_retention)
+        if self.error_log_file:
+            logger.add(self.error_log_file, level="ERROR", **self.log_retention)
+
         self.scheduler.start()
         logger.debug("Scheduler started.")
 
+        if not self.is_agent:
+            channel_ids = await self.fetch_bound_channels()
+            for c_id in channel_ids:
+                if c_id not in self.channels:
+                    if self.init_all_channels:
+                        logger.info(f'Extra channel bound to this service on startup will be initialized  (self.init_all_channels is True): {c_id}')
+                        await self.initialize_channel(c_id) # This channel was not initialized in the main "initialize channels" for loop because it is not in self.channels.
+                    else:
+                        logger.info(f'Extra channel bound to this service on startup will NOT be initialized (self.init_all_channels is False): {c_id}')
+
         await self.on_start()
         logger.debug("on_start() finished.")
 
         self.scheduler.add_job(self.checkin, 'interval', seconds=self.checkin_interval) # This check-in must be after on_start()
 
         await asyncio.gather(self.ws_client.receive(), self.listen_loop())
```

### Comparing `moobius-1.1.6/src/moobius/core/wand.py` & `moobius-1.1.7/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/database/database_interface.py` & `moobius-1.1.7/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/database/json_database.py` & `moobius-1.1.7/src/moobius/database/json_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/database/null_database.py` & `moobius-1.1.7/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/database/redis_database.py` & `moobius-1.1.7/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/database/storage.py` & `moobius-1.1.7/src/moobius/database/storage.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/network/asserts.py` & `moobius-1.1.7/src/moobius/network/asserts.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/network/http_api_wrapper.py` & `moobius-1.1.7/src/moobius/network/http_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/network/ws_client.py` & `moobius-1.1.7/src/moobius/network/ws_client.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/types.py` & `moobius-1.1.7/src/moobius/types.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius/utils.py` & `moobius-1.1.7/src/moobius/utils.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.6/src/moobius.egg-info/PKG-INFO` & `moobius-1.1.7/src/moobius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.6
+Version: 1.1.7
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.6/src/moobius.egg-info/SOURCES.txt` & `moobius-1.1.7/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

