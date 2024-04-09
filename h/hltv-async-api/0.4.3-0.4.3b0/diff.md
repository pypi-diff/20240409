# Comparing `tmp/hltv_async_api-0.4.3.tar.gz` & `tmp/hltv_async_api-0.4.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.3.tar", last modified: Tue Apr  9 13:04:12 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.3b0.tar", last modified: Tue Apr  9 10:18:15 2024, max compression
```

## Comparing `hltv_async_api-0.4.3.tar` & `hltv_async_api-0.4.3b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:04:12.974704 hltv_async_api-0.4.3/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.3/LICENSE
--rw-rw-rw-   0        0        0    11823 2024-04-09 13:04:12.973702 hltv_async_api-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    11200 2024-04-09 13:03:53.000000 hltv_async_api-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 13:04:12.963667 hltv_async_api-0.4.3/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-09 12:49:36.000000 hltv_async_api-0.4.3/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    33432 2024-04-09 12:49:11.000000 hltv_async_api-0.4.3/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:04:12.972704 hltv_async_api-0.4.3/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0    11823 2024-04-09 13:04:12.000000 hltv_async_api-0.4.3/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-09 13:04:12.000000 hltv_async_api-0.4.3/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:04:12.000000 hltv_async_api-0.4.3/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-09 13:04:12.000000 hltv_async_api-0.4.3/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-09 13:04:11.000000 hltv_async_api-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 13:04:12.974704 hltv_async_api-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-09 12:49:36.000000 hltv_async_api-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:18:15.965416 hltv_async_api-0.4.3b0/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.3b0/LICENSE
+-rw-rw-rw-   0        0        0     8673 2024-04-09 10:18:15.962417 hltv_async_api-0.4.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     8048 2024-04-08 17:31:52.000000 hltv_async_api-0.4.3b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 10:18:15.949420 hltv_async_api-0.4.3b0/hltv_async_api/
+-rw-rw-rw-   0        0        0      125 2024-04-09 10:18:08.000000 hltv_async_api-0.4.3b0/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    33428 2024-04-09 10:17:15.000000 hltv_async_api-0.4.3b0/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:18:15.960415 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     8673 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      538 2024-04-09 10:18:08.000000 hltv_async_api-0.4.3b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:18:15.966419 hltv_async_api-0.4.3b0/setup.cfg
+-rw-rw-rw-   0        0        0      923 2024-04-09 10:18:08.000000 hltv_async_api-0.4.3b0/setup.py
```

### Comparing `hltv_async_api-0.4.3/LICENSE` & `hltv_async_api-0.4.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.3/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.3b0/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,27 +214,27 @@
         day = parts[1][:-2]
         return day + '-' + month
 
     async def get(self, type: str, id: int | str | None = None,
                   title: str | None = None,
                   team1: str | None = None,
                   team2: str | None = None):
-        if type == 'events':
+        if type == 'event':
             if id:
                 return await self.get_event_info(id, title)
             else:
                 return await self.get_events()
-        elif type == 'matches':
+        elif type == 'match':
             if id:
                 return await self.get_match_info(str(id), team1, team2, title)
             else:
                 return await self.get_upcoming_matches()
         elif type == 'news':
             return await self.get_last_news()
-        elif type == 'teams':
+        elif type == 'team':
             if id:
                 return await self.get_team_info(id, title)
             else:
                 return await self.get_top_teams()
 
     async def get_live_matches(self, max_ = 10):
         """returns a list of all LIVE matches on HLTV along with the maps being played and the star ratings"""
```

### Comparing `hltv_async_api-0.4.3/pyproject.toml` & `hltv_async_api-0.4.3b0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.3"
+version = "0.4.3b"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

