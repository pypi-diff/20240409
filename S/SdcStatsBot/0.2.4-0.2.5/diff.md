# Comparing `tmp/SdcStatsBot-0.2.4.tar.gz` & `tmp/SdcStatsBot-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SdcStatsBot-0.2.4.tar", last modified: Tue Apr  9 10:44:21 2024, max compression
+gzip compressed data, was "SdcStatsBot-0.2.5.tar", last modified: Tue Apr  9 10:49:40 2024, max compression
```

## Comparing `SdcStatsBot-0.2.4.tar` & `SdcStatsBot-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:44:21.830501 SdcStatsBot-0.2.4/
--rw-rw-rw-   0        0        0      344 2024-04-09 10:44:21.831506 SdcStatsBot-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 10:44:21.821576 SdcStatsBot-0.2.4/SDcStatsBot/
--rw-rw-rw-   0        0        0       26 2024-04-09 09:32:35.000000 SdcStatsBot-0.2.4/SDcStatsBot/__init__.py
--rw-rw-rw-   0        0        0     2072 2024-04-09 10:39:02.000000 SdcStatsBot-0.2.4/SDcStatsBot/client.py
--rw-rw-rw-   0        0        0       32 2024-04-09 10:30:59.000000 SdcStatsBot-0.2.4/SDcStatsBot/interval.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:44:21.829079 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 10:44:21.000000 SdcStatsBot-0.2.4/SdcStatsBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:44:21.832505 SdcStatsBot-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-04-09 10:44:05.000000 SdcStatsBot-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:49:40.858356 SdcStatsBot-0.2.5/
+-rw-rw-rw-   0        0        0      344 2024-04-09 10:49:40.858356 SdcStatsBot-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 10:49:40.848710 SdcStatsBot-0.2.5/SDcStatsBot/
+-rw-rw-rw-   0        0        0       26 2024-04-09 09:32:35.000000 SdcStatsBot-0.2.5/SDcStatsBot/__init__.py
+-rw-rw-rw-   0        0        0     2065 2024-04-09 10:49:11.000000 SdcStatsBot-0.2.5/SDcStatsBot/client.py
+-rw-rw-rw-   0        0        0       32 2024-04-09 10:30:59.000000 SdcStatsBot-0.2.5/SDcStatsBot/interval.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:49:40.856350 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 10:49:40.000000 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-09 10:49:40.000000 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:49:40.000000 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 10:49:40.000000 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2024-04-09 10:49:40.000000 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 10:49:40.000000 SdcStatsBot-0.2.5/SdcStatsBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:49:40.859353 SdcStatsBot-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-04-09 10:49:25.000000 SdcStatsBot-0.2.5/setup.py
```

### Comparing `SdcStatsBot-0.2.4/SDcStatsBot/client.py` & `SdcStatsBot-0.2.5/SDcStatsBot/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,13 +30,13 @@
             headers = {"Authorization": f"SDC {sdc_token}"}
             url = f"{self.web_url}/bots/{bot_id}/stats"
             payload = {"shards": shard_count, "servers": servers_count}
             async with self.session.post(url, headers=headers, json=payload) as response:
                 if response.status != 200:
                     self.logger.error("Failed to send statistics to SDC API: %s", await response.text())
                 else:
-                    self.logger.success("Statistics successfully sent to SDC API. Next update in %s minutes", self.interval)
+                    self.logger.info("Statistics successfully sent to SDC API. Next update in %s minutes", self.interval)
         except aiohttp.ClientError as e:
-            self.logger.exception("Error while sending statistics to SDC API")
+            self.logger.error("Error while sending statistics to SDC API")
 
     async def start_posting_stats(self, bot_id, sdc_token, servers_count, shard_count=1):
         asyncio.create_task(self.post_stats_loop(bot_id, sdc_token, servers_count, shard_count))
```

### Comparing `SdcStatsBot-0.2.4/setup.py` & `SdcStatsBot-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(name='SdcStatsBot',
       author="Masezev",
       url="https://github.com/masezev/SdcStatsBot",
       project_urls={
           'Поддержка': 'https://discord.gg/H7FQFGEPz5',
       },
       repository='https://github.com/masezev/SdcStatsBot',
-      version='0.2.4',
+      version='0.2.5',
       description='A Python wrapper for the SDC API',
       python_requires='>=3.8.0',
       keywords='A Python wrapper for the SDC API',
       install_requires=[
             'aiohttp',
             'loguru',
             'logging',
```

