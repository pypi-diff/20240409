# Comparing `tmp/hltv_async_api-0.4.2.tar.gz` & `tmp/hltv_async_api-0.4.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.2.tar", last modified: Mon Apr  8 18:01:29 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.3b0.tar", last modified: Tue Apr  9 10:18:15 2024, max compression
```

## Comparing `hltv_async_api-0.4.2.tar` & `hltv_async_api-0.4.3b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:01:29.783122 hltv_async_api-0.4.2/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     8671 2024-04-08 18:01:29.782120 hltv_async_api-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     8048 2024-04-08 17:31:52.000000 hltv_async_api-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 18:01:29.723698 hltv_async_api-0.4.2/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-08 18:01:25.000000 hltv_async_api-0.4.2/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    33610 2024-04-08 17:31:52.000000 hltv_async_api-0.4.2/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:01:29.780125 hltv_async_api-0.4.2/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     8671 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-08 18:01:25.000000 hltv_async_api-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 18:01:29.784122 hltv_async_api-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-08 18:01:25.000000 hltv_async_api-0.4.2/setup.py
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

### Comparing `hltv_async_api-0.4.2/LICENSE` & `hltv_async_api-0.4.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.2/PKG-INFO` & `hltv_async_api-0.4.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.2
+Version: 0.4.3b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.4.2/README.md` & `hltv_async_api-0.4.3b0/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.2/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.3b0/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,14 @@
 
         live_matches: List | Any
         matches = []
         try:
             live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div", {'class', 'liveMatch-container'})
         except AttributeError:
             live_matches = []
-        live_mat = []
         for live in live_matches:
             id_ = live.find('a', {'class': 'match a-reset'})['href'].split('/')[2]
             teams = live.find_all("div", class_="matchTeamName text-ellipsis")
             team1 = teams[0].text.strip()
             team2 = teams[1].text.strip()
             t1_id = live['team1']
             t2_id = live['team2']
@@ -460,28 +459,24 @@
                 scores = live.find("td", class_="matchTeamScore").text.strip().split('-')
                 score_team1 = scores[0].strip()
                 score_team2 = scores[1].strip()
             except AttributeError:
                 score_team1 = 0
                 score_team2 = 0"""
 
-            live_mat.append({
+            matches.append({
                 'id': id_,
+                'date': 'LIVE',
                 'team1': team1,
                 'team2': team2,
                 't1_id': t1_id,
                 't2_id': t2_id
             })
 
-        matches.append({
-            'date': 'LIVE',
-            'matches': live_mat,
-        })
         for date_sect in r.find_all('div', {'class': 'upcomingMatchesSection'}):
-            upc_matches = []
             date_ = date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1]
             for match in date_sect.find_all('div', {'class': 'upcomingMatch'}):
                 teams_ = match.find_all("div", class_="matchTeamName text-ellipsis")
                 id_ = match.find('a')['href'].split('/')[2]
                 t1_id = 0
                 t2_id = 0
                 time_ = match.find('div', {'class', 'matchTime'}).text
@@ -491,25 +486,24 @@
                     team1_ = teams_[0].text.strip()
                     team2_ = teams_[1].text.strip()
                     t1_id = match['team1']
                     t2_id = match['team2']
                 except IndexError:
                     pass
 
-                upc_matches.append({
+                matches.append({
                         'id': id_,
+                        'date': date_,
                         'time': time_,
                         'team1': team1_,
                         'team2': team2_,
                         't1_id': t1_id,
                         't2_id': t2_id
                     })
 
-            matches.append({'date': date_, 'matches': upc_matches})
-
         return matches
     async def get_featured_events(self, max_: int = 1):
         r = await self._fetch('https://www.hltv.org/events')
 
         events = []
         try:
             for i, event in enumerate(r.find('div', {'class': 'tab-content', 'id': 'FEATURED'}).find_all('a', {'class': 'a-reset ongoing-event'}), start=1):
@@ -586,15 +580,15 @@
                         'start_date': event_start_date,
                         'end_date': event_end_date
                     })
 
         return events
 
     async def get_event_info(self, event_id: str | int, event_title: str):
-        #TODO ADD PLACEC FOR PAST EVENTS? OR WINNER?
+        #TODO ADD WINNER?
 
         r = await self._fetch(f"https://www.hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
         if not r:
             return
 
         event_date_div = r.find('td', {'class', 'eventdate'}).find_all('span')
 
@@ -772,14 +766,15 @@
                     break
         except AttributeError:
             raise AttributeError("Top players parsing error, probably page not fully loaded")
 
         return players
 
     async def get_last_news(self, max_reg_news=2, only_today=True, only_featured=False):
+
         r = await self._fetch('https://www.hltv.org/')
 
         today = datetime.now(tz=pytz.timezone('Europe/Copenhagen'))
         article_days = {
             1: today.strftime('%d-%m'),
             2: (today - timedelta(days=1)).strftime('%d-%m'),
             3: 'old'
```

### Comparing `hltv_async_api-0.4.2/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.4.3b0/hltv_async_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.2
+Version: 0.4.3b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.4.2/pyproject.toml` & `hltv_async_api-0.4.3b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.2"
+version = "0.4.3b"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.4.2/setup.py` & `hltv_async_api-0.4.3b0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.4.2',
+    version='0.4.3b',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

