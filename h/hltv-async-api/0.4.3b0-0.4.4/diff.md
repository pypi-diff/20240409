# Comparing `tmp/hltv_async_api-0.4.3b0.tar.gz` & `tmp/hltv_async_api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.3b0.tar", last modified: Tue Apr  9 10:18:15 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.4.tar", last modified: Tue Apr  9 13:35:02 2024, max compression
```

## Comparing `hltv_async_api-0.4.3b0.tar` & `hltv_async_api-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:18:15.965416 hltv_async_api-0.4.3b0/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.3b0/LICENSE
--rw-rw-rw-   0        0        0     8673 2024-04-09 10:18:15.962417 hltv_async_api-0.4.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     8048 2024-04-08 17:31:52.000000 hltv_async_api-0.4.3b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:18:15.949420 hltv_async_api-0.4.3b0/hltv_async_api/
--rw-rw-rw-   0        0        0      125 2024-04-09 10:18:08.000000 hltv_async_api-0.4.3b0/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    33428 2024-04-09 10:17:15.000000 hltv_async_api-0.4.3b0/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:18:15.960415 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     8673 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-09 10:18:15.000000 hltv_async_api-0.4.3b0/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      538 2024-04-09 10:18:08.000000 hltv_async_api-0.4.3b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 10:18:15.966419 hltv_async_api-0.4.3b0/setup.cfg
--rw-rw-rw-   0        0        0      923 2024-04-09 10:18:08.000000 hltv_async_api-0.4.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:35:02.884751 hltv_async_api-0.4.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0    11823 2024-04-09 13:35:02.882749 hltv_async_api-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11200 2024-04-09 13:03:53.000000 hltv_async_api-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 13:35:02.868281 hltv_async_api-0.4.4/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-09 13:34:59.000000 hltv_async_api-0.4.4/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    33553 2024-04-09 13:34:27.000000 hltv_async_api-0.4.4/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:35:02.881226 hltv_async_api-0.4.4/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0    11823 2024-04-09 13:35:02.000000 hltv_async_api-0.4.4/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-09 13:35:02.000000 hltv_async_api-0.4.4/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 13:35:02.000000 hltv_async_api-0.4.4/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-09 13:35:02.000000 hltv_async_api-0.4.4/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-09 13:34:59.000000 hltv_async_api-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 13:35:02.885747 hltv_async_api-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-09 13:34:59.000000 hltv_async_api-0.4.4/setup.py
```

### Comparing `hltv_async_api-0.4.3b0/LICENSE` & `hltv_async_api-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.3b0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.4/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from functools import partial
 
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientProxyConnectionError, ClientResponseError, ClientOSError, \
     ServerDisconnectedError, ClientHttpProxyError
 import re
 
-
 import logging
 
 
 class Hltv:
     def __init__(self, max_delay: int = 15,
                  timeout: int = 5,
                  use_proxy: bool = False,
@@ -214,64 +213,62 @@
         day = parts[1][:-2]
         return day + '-' + month
 
     async def get(self, type: str, id: int | str | None = None,
                   title: str | None = None,
                   team1: str | None = None,
                   team2: str | None = None):
-        if type == 'event':
+        if type == 'events':
             if id:
                 return await self.get_event_info(id, title)
             else:
                 return await self.get_events()
-        elif type == 'match':
+        elif type == 'matches':
             if id:
                 return await self.get_match_info(str(id), team1, team2, title)
             else:
                 return await self.get_upcoming_matches()
         elif type == 'news':
             return await self.get_last_news()
-        elif type == 'team':
+        elif type == 'teams':
             if id:
                 return await self.get_team_info(id, title)
             else:
                 return await self.get_top_teams()
 
-    async def get_live_matches(self, max_ = 10):
+    async def get_live_matches(self, max_=10):
         """returns a list of all LIVE matches on HLTV along with the maps being played and the star ratings"""
         r = await self._fetch("https://www.hltv.org/matches")
         if not r:
             return
 
         live_matches = r.find("div", {'class', "liveMatchesContainer"})
 
-        #cant find a way, mby use socketio by hltv-score-bot ?? | other url ?
-
+        # cant find a way, mby use socketio by hltv-score-bot ?? | other url ?
 
     async def get_upcoming_matches(self, days: int = 7, min_rating: int = 1):
         """returns a list of all upcoming matches on HLTV"""
         r = await self._fetch("https://www.hltv.org/matches")
-        if not r:return
+        if not r: return
 
         matches = []
         try:
 
-
             for i, date_div in enumerate(r.find_all('div', {'class': 'upcomingMatchesSection'}), start=1):
                 if i > days:
                     break
                 date_ = date_div.find('span', {'class': 'matchDayHeadline'}).text.split()[-1]
-                matches_today = []
 
                 for match in date_div.find_all('div', {'class': 'upcomingMatch'}):
                     time_ = match.find('div', {'class': 'matchTime'}).text
                     rating = int(match['stars'])
                     if rating >= min_rating:
                         match_id_ = match.find('a')['href'].split('/')[2]
-
+                        t1_id = match['team1']
+                        t2_id = match['team2']
                         maps = match.find('div', {'class': 'matchMeta'}).text[-1:]
                         try:
                             teams = match.find_all('div', {'class': 'matchTeamName text-ellipsis'})
 
                             team1 = teams[0].text
                             team2 = teams[1].text
                         except (IndexError, AttributeError):
@@ -283,62 +280,60 @@
                         except AttributeError:
 
                             try:
                                 event = match.find('span', {'class': 'line-clamp-3'}).text
                             except AttributeError:
                                 event = ''
 
-                        matches_today.append({
-                            'match_id': match_id_,
+                        matches.append({
+                            'id': match_id_,
+                            'date': date_,
+                            'time': time_,
                             'team1': team1,
                             'team2': team2,
-                            'time': time_,
+                            't1_id': t1_id,
+                            't2_id': t2_id,
                             'maps': maps,
                             'rating': rating,
                             'event': event
-                    })
+                        })
 
-                matches.append({
-                    'date': date_,
-                    'matches': matches_today
-                })
         except AttributeError:
             return None
         return matches
 
     async def get_match_info(self, match_id: str, team1: str, team2: str, event_title: str, stats: bool = True):
         r = await self._fetch(f"https://www.hltv.org/matches/{match_id}/"
-                             f"{team1.replace(' ', '-')}-vs-"
-                             f"{team2.replace(' ', '-')}-"
-                             f"{event_title.replace(' ', '-')}")
+                              f"{team1.replace(' ', '-')}-vs-"
+                              f"{team2.replace(' ', '-')}-"
+                              f"{event_title.replace(' ', '-')}")
         if not r:
             return
 
         status = r.find('div', {'class': 'countdown'}).text
 
         score1, score2 = 0, 0
 
         if status == 'Match over':
             scores = r.find_all('div', class_='team')
             score1 = scores[0].get_text().replace('\n', '')[-1]
             score2 = scores[1].get_text().replace('\n', '')[-1]
 
-
         maps = []
         for map_div in r.find_all('div', {'class': 'mapholder'}):
 
-                mapname = map_div.find('div', {'class': 'mapname'}).text
-                try:
-                    r_teams = map_div.find_all('div', {'class': 'results-team-score'})
-                    r_team1 = r_teams[0].text
-                    r_team2 = r_teams[1].text
-                except AttributeError:
-                    r_team1 = '0'
-                    r_team2 = '0'
-                maps.append({'mapname': mapname, 'r_team1': r_team1, 'r_team2': r_team2})
+            mapname = map_div.find('div', {'class': 'mapname'}).text
+            try:
+                r_teams = map_div.find_all('div', {'class': 'results-team-score'})
+                r_team1 = r_teams[0].text
+                r_team2 = r_teams[1].text
+            except AttributeError:
+                r_team1 = '0'
+                r_team2 = '0'
+            maps.append({'mapname': mapname, 'r_team1': r_team1, 'r_team2': r_team2})
 
         stats_ = []
         if stats and status == 'Match over':
             for table_div in r.find_all('table', {'class': 'table totalstats'})[:2]:
                 for player in table_div.find_all('tr')[1:]:
                     player_id = player.find('a', class_='flagAlign')['href'].split('/')[2]
                     player_name = player.find('div', class_='statsPlayerName').text.strip()
@@ -369,15 +364,14 @@
                         score2 += 1
                     else:
                         score2 = 13
                         score1 = int(map["r_team1"])
 
         return match_id, score1, score2, status, maps, stats_
 
-
     async def get_big_results(self, offset=0) -> list[dict[str, Any]] | None:
         """returns a list of big event matches results"""
         r = await self._fetch("https://www.hltv.org/results?offset=" + str(offset))
         if not r:
             return
 
         big_results = []
@@ -438,26 +432,26 @@
         r = await self._fetch("https://www.hltv.org/events/" + str(event_id) + "/matches")
         if not r:
             return
 
         live_matches: List | Any
         matches = []
         try:
-            live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div", {'class', 'liveMatch-container'})
+            live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div",
+                                                                                   {'class', 'liveMatch-container'})
         except AttributeError:
             live_matches = []
         for live in live_matches:
             id_ = live.find('a', {'class': 'match a-reset'})['href'].split('/')[2]
             teams = live.find_all("div", class_="matchTeamName text-ellipsis")
             team1 = teams[0].text.strip()
             team2 = teams[1].text.strip()
             t1_id = live['team1']
             t2_id = live['team2']
 
-
             # TODO FIX SCORES
             """try:
                 scores = live.find("td", class_="matchTeamScore").text.strip().split('-')
                 score_team1 = scores[0].strip()
                 score_team2 = scores[1].strip()
             except AttributeError:
                 score_team1 = 0
@@ -487,30 +481,32 @@
                     team2_ = teams_[1].text.strip()
                     t1_id = match['team1']
                     t2_id = match['team2']
                 except IndexError:
                     pass
 
                 matches.append({
-                        'id': id_,
-                        'date': date_,
-                        'time': time_,
-                        'team1': team1_,
-                        'team2': team2_,
-                        't1_id': t1_id,
-                        't2_id': t2_id
-                    })
+                    'id': id_,
+                    'date': date_,
+                    'time': time_,
+                    'team1': team1_,
+                    'team2': team2_,
+                    't1_id': t1_id,
+                    't2_id': t2_id
+                })
 
         return matches
+
     async def get_featured_events(self, max_: int = 1):
         r = await self._fetch('https://www.hltv.org/events')
 
         events = []
         try:
-            for i, event in enumerate(r.find('div', {'class': 'tab-content', 'id': 'FEATURED'}).find_all('a', {'class': 'a-reset ongoing-event'}), start=1):
+            for i, event in enumerate(r.find('div', {'class': 'tab-content', 'id': 'FEATURED'}).find_all('a', {
+                'class': 'a-reset ongoing-event'}), start=1):
                 if i > max_:
                     break
                 event_name = event.find('div', {'class': 'text-ellipsis'}).text.strip()
                 event_start_date = self._normalize_date(
                     event.find('span', {'data-time-format': 'MMM do'}).text.strip().split())
 
                 event_end_date = self._normalize_date(
@@ -523,14 +519,15 @@
                     'start_date': event_start_date,
                     'end_date': event_end_date,
                 })
         except AttributeError:
             pass
 
         return events
+
     async def get_events(self, featured=True, outgoing=True, future=True, max_events=10):
         """Returns events
         :params:
         outgoing - include live tournaments
         future - include future tournamets
         max_events - use only if future=True
         :return:
@@ -541,15 +538,15 @@
         if not r:
             return
 
         events = []
 
         if outgoing:
             for event in r.find('div', {'class': 'tab-content', 'id': 'TODAY'}).find_all('a', {
-                                'class': 'a-reset ongoing-event'}):
+                'class': 'a-reset ongoing-event'}):
                 event_name = event.find('div', {'class': 'text-ellipsis'}).text.strip()
                 event_start_date = self._normalize_date(
                     event.find('span', {'data-time-format': 'MMM do'}).text.strip().split())
 
                 event_end_date = self._normalize_date(
                     event.find_all('span', {'data-time-format': 'MMM do'})[1].text.strip().split())
                 event_id = event['href'].split('/')[-2]
@@ -580,15 +577,15 @@
                         'start_date': event_start_date,
                         'end_date': event_end_date
                     })
 
         return events
 
     async def get_event_info(self, event_id: str | int, event_title: str):
-        #TODO ADD WINNER?
+        # TODO ADD WINNER?
 
         r = await self._fetch(f"https://www.hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
         if not r:
             return
 
         event_date_div = r.find('td', {'class', 'eventdate'}).find_all('span')
 
@@ -782,27 +779,28 @@
 
         news = []
         reg_news_num = 0
         for i, news_date_div in enumerate(r.find_all('div', {'class', 'standard-box standard-list'}), start=1):
             date_ = article_days[i]
             f_news = []
             reg_news = []
-            for featured_news_div in news_date_div.find_all('a', {'class': 'newsline article featured breaking-featured'}):
+            for featured_news_div in news_date_div.find_all('a',
+                                                            {'class': 'newsline article featured breaking-featured'}):
                 featured_id = featured_news_div['href'].split('/')[2]
                 featured_title = featured_news_div.find('div', {'class': 'featured-newstext'}).text
                 featured_description = featured_news_div.find('div', {'class': 'featured-small-newstext'}).text
                 f_news.append({
                     'f_id': featured_id,
                     'f_title': featured_title,
                     'f_desc': featured_description,
                 })
 
             if not only_featured and reg_news_num < max_reg_news:
                 for news_div in news_date_div.find_all('a',
-                                                           {'class': 'newsline article'}):
+                                                       {'class': 'newsline article'}):
                     if reg_news_num > max_reg_news:
                         break
                     if news_div['class'] != 'newsline article featured breaking-featured':
                         news_id = news_div['href'].split('/')[2]
                         news_title = news_div.find('div', {'class': 'newstext'}).text
                         news_posted = news_div.find('div', {'class': 'newsrecent'}).text
 
@@ -833,9 +831,10 @@
     print(await hltv.get_event_results(7437))
     print(await hltv.get_upcoming_matches(1, 3))
     print(await hltv.get_match_info('2370913', 'FURIA', 'MOUZ', 'betboom-dacha-belgrade-2024-europe-closed-qualifier'))
     print(await hltv.get_last_news())
     print(await hltv.get_top_teams())
     print(await hltv.get_best_players())
 
+
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.4.3b0/pyproject.toml` & `hltv_async_api-0.4.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.3b"
+version = "0.4.4"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.4.3b0/setup.py` & `hltv_async_api-0.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.4.3b',
+    version='0.4.4',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

