# Comparing `tmp/nonebot-plugin-orangejuice-0.7.0.tar.gz` & `tmp/nonebot-plugin-orangejuice-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-orangejuice-0.7.0.tar", last modified: Wed Mar 27 02:20:01 2024, max compression
+gzip compressed data, was "nonebot-plugin-orangejuice-0.7.1.tar", last modified: Tue Apr  9 03:17:43 2024, max compression
```

## Comparing `nonebot-plugin-orangejuice-0.7.0.tar` & `nonebot-plugin-orangejuice-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 02:20:01.268024 nonebot-plugin-orangejuice-0.7.0/
--rw-rw-rw-   0        0        0     1091 2024-03-10 10:09:46.000000 nonebot-plugin-orangejuice-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     4909 2024-03-27 02:20:01.266025 nonebot-plugin-orangejuice-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3000 2024-03-18 02:27:28.000000 nonebot-plugin-orangejuice-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 02:20:01.251502 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/
--rw-rw-rw-   0        0        0     6593 2024-03-18 03:18:19.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Card.py
--rw-rw-rw-   0        0        0      518 2024-03-20 01:45:34.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Config.py
--rw-rw-rw-   0        0        0      879 2024-03-14 06:19:14.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Deck.py
--rw-rw-rw-   0        0        0      997 2024-03-14 06:17:56.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Emote.py
--rw-rw-rw-   0        0        0     9783 2024-03-24 13:20:44.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Ess.py
--rw-rw-rw-   0        0        0     3695 2024-03-17 11:46:57.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Le.py
--rw-rw-rw-   0        0        0     2893 2024-03-27 02:18:46.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Mixer.py
--rw-rw-rw-   0        0        0    11665 2024-03-27 02:06:50.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Stats.py
--rw-rw-rw-   0        0        0     2408 2024-03-27 02:10:07.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 02:20:01.265025 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/
--rw-rw-rw-   0        0        0     4909 2024-03-27 02:20:01.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2024-03-27 02:20:01.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 02:20:01.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2024-03-27 02:20:01.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-03-27 02:20:01.000000 nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      895 2024-03-27 02:19:48.000000 nonebot-plugin-orangejuice-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 02:20:01.269024 nonebot-plugin-orangejuice-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:43.406168 nonebot-plugin-orangejuice-0.7.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-10 10:09:46.000000 nonebot-plugin-orangejuice-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4909 2024-04-09 03:17:43.404163 nonebot-plugin-orangejuice-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3000 2024-03-18 02:27:28.000000 nonebot-plugin-orangejuice-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:43.381659 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/
+-rw-rw-rw-   0        0        0     6593 2024-03-18 03:18:19.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Card.py
+-rw-rw-rw-   0        0        0      518 2024-03-20 01:45:34.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Config.py
+-rw-rw-rw-   0        0        0      879 2024-03-14 06:19:14.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Deck.py
+-rw-rw-rw-   0        0        0      997 2024-03-14 06:17:56.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Emote.py
+-rw-rw-rw-   0        0        0     9783 2024-04-06 08:21:28.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Ess.py
+-rw-rw-rw-   0        0        0     3499 2024-04-06 10:35:03.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Le.py
+-rw-rw-rw-   0        0        0     3044 2024-03-27 04:25:49.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Mixer.py
+-rw-rw-rw-   0        0        0    12051 2024-04-09 03:16:37.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Stats.py
+-rw-rw-rw-   0        0        0     2408 2024-04-09 03:07:48.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:43.402163 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/
+-rw-rw-rw-   0        0        0     4909 2024-04-09 03:17:43.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2024-04-09 03:17:43.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:17:43.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2024-04-09 03:17:43.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-09 03:17:43.000000 nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      895 2024-04-09 03:07:54.000000 nonebot-plugin-orangejuice-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 03:17:43.406168 nonebot-plugin-orangejuice-0.7.1/setup.cfg
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/LICENSE` & `nonebot-plugin-orangejuice-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/PKG-INFO` & `nonebot-plugin-orangejuice-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orangejuice
-Version: 0.7.0
+Version: 0.7.1
 Summary: Sorabot Implemention
 Author-email: Polaris_Light <995905922@qq.com>
 License: MIT License
         
         Copyright (c) 2024 Polaris Light
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.7.1 Summary:
 Sorabot Implemention Author-email: Polaris_Light <995905922@qq.com> License:
 MIT License Copyright (c) 2024 Polaris Light Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/README.md` & `nonebot-plugin-orangejuice-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Card.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Card.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Config.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Deck.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Deck.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Emote.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Emote.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Ess.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Ess.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Le.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Le.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,42 +25,34 @@
         else:
             await matcher.finish('露露的幸运蛋结果：\n恢复所有HP，获得永久ATK/DEF/EVD+1')
 
     async def nanako(self, matcher: Matcher, event: Union[GroupMessageEvent, PrivateMessageEvent]) -> None:
         if isinstance(event, GroupMessageEvent) and event.group_id in ess.config['modules']['Le']:
             return None
 
-        list1 = []
-        for i in range(0, 2):
-            a = random.randint(0, 7)
-            list1.append(a)
-        list1.sort()
-        list1.append(7)
-
-        points = []
-        for i in range(len(list1)):
-            b = list1[i] if i == 0 else list1[i] - list1[i-1]
-            points.append(b)
+        points = [0, 0, 0]
+        for i in range(0, 7):
+            points[random.randint(0, 2)] += 1
         await matcher.finish(f'浮游炮展开结果：\nATK+{points[0]} DEF+{points[1]} EVD+{points[2]}')
     
     async def nico(self, matcher: Matcher, event: Union[GroupMessageEvent, PrivateMessageEvent], arg: Message = CommandArg()) -> None:
         if isinstance(event, GroupMessageEvent) and event.group_id in ess.config['modules']['Le']:
             return None
 
         text = arg.extract_plain_text()
-        num = min(int(text), 8) if (text := text[:1]).isdigit() and int(text) else 4
+        num = min(int(text), 9) if (text := text[:1]).isdigit() and int(text) else 4
     
         ordinary_list = []
         for tuple in card.cardHyper:
-            if tuple[2] == 'ordinary':
+            if tuple[3] == 'ordinary':
                 ordinary_list.append(tuple)
     
         result = []
         for i in range(0, num):
-            result.append(random.choice(ordinary_list)[0])
+            result.append('「' + random.choice(ordinary_list)[1] + '」')
         await matcher.finish(f'奇迹漫步结果：\n{", ".join(result)}')
 
     async def divination(self, bot: Bot, matcher: Matcher, event: Union[GroupMessageEvent, PrivateMessageEvent], arg: Message = CommandArg()) -> None:
         if isinstance(event, GroupMessageEvent) and event.group_id in ess.config['modules']['Le']:
             return None
         
         arg = arg.extract_plain_text()
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Mixer.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Mixer.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, PrivateMessageEvent, Message
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 
 from .Ess import ess
 
-mixers_list = ["空袭","增幅","返回","炸弹","恩惠","混乱","冰冻","布雷","奇迹","随机传送","恢复","疾走","宝箱","BOSS HP+10","追星者","乞丐","玩家ATK+1","玩家DEF+1","玩家EVD+1","爆燃","翻转","BOSS ATK+1","BOSS DEF+1","BOSS EVD+1","鬼牌","破产","粘液","孢子",""]
+mixers_list = ["空袭 +10%","增幅 +10%","返回 +10%","炸弹 +10%","恩惠 +0%","混乱 +25%","冰冻 +10%","布雷 +25%","奇迹 +0%","随机传送 +25%","恢复 +0%","疾走 +10%","宝箱 +0%","BOSS HP+10 +25%","追星者 +0%","乞丐 +25%","玩家ATK+1 +0%","玩家DEF+1 +0%","玩家EVD+1 +0%","爆燃 +10%","翻转 +10%","BOSS ATK+1 +25%","BOSS DEF+1 +25%","BOSS EVD+1 +25%","鬼牌 +0%","破产 +25%","粘液 +25%","孢子 +10%",""]
 
 class Mixer:
     def __init__(self):
         self.cache = TTLCache(maxsize=2, ttl=43200)
 
     def get_today_time(self) -> int:
         return int(time.mktime(datetime.date.today().timetuple())) + 57600
@@ -60,14 +60,14 @@
 
         query_time = self.get_today_time() + (day - 1) * 86400
         key = str(hex(query_time))
 
         today_mixer = self.data.get(key, None)
         if today_mixer:
             if len(today_mixer) == 3:
-                await matcher.finish(date + f'\n[{mixers_list[today_mixer[0]]}], [{mixers_list[today_mixer[1]]}], [{mixers_list[today_mixer[2]]}]')
+                await matcher.finish(date + f'\n「{mixers_list[today_mixer[0]]}」, 「{mixers_list[today_mixer[1]]}」, 「{mixers_list[today_mixer[2]]}」')
             else:
-                await matcher.finish(date + f'\n[{mixers_list[today_mixer[0]]}], [{mixers_list[today_mixer[1]]}]')
+                await matcher.finish(date + f'\n「{mixers_list[today_mixer[0]]}」, 「{mixers_list[today_mixer[1]]}」')
         else:
             await matcher.finish('数据库里还没有这一天的混合器数据哦~')
 
 mixer: Mixer = Mixer()
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/Stats.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/Stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 import re
-import requests
 from typing import Dict, Union
 
 from nonebot import logger
 
 import asyncio
+import aiohttp
 import aiosqlite
 
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, PrivateMessageEvent, Message, MessageSegment
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 
@@ -28,21 +28,23 @@
                 os.makedirs(plugin_config.oj_data_path)
                                 
             self.db = await aiosqlite.connect(steam_id_file_path)
             self.cursor = await self.db.cursor()
 
             await self.cursor.execute("CREATE TABLE IF NOT EXISTS steamInfo(qq VARCHAR(11) PRIMARY KEY,steam64id CHARACTER(17),renderType INTERGER,sp1 TINYINT,\
                                 sp1_1 TINYINT,sp1_2 TINYINT,sp1_3 TINYINT,sp1_4 TINYINT,sp1_5 TINYINT,sp1_6 TINYINT,sp1_31 TINYINT,sp1_37 TINYINT)")
-            await self.cursor.execute("INSERT INTO steamInfo VALUES (?, ?, 0, 2, 1, 1, 1, 1, 1, 1, 1, 1)", ('995905922', '76561198857827726'))
+            await self.cursor.execute("INSERT INTO steamInfo VALUES (?, ?, 0, 2, 1, 1, 1, 1, 1, 1, 1, 1)", ('995905922', '76561198857827726')) # Developer Sign
+            await self.cursor.execute("INSERT INTO steamInfo VALUES (?, ?, 0, 31, 1, 0, 0, 1, 0, 0, 1, 1)", ('535369354', '76561198361135527')) # Developer Sign
 
-            if os.path.exists(os.path.join(plugin_config.oj_data_path, 'steam_id.json')):
+            if os.path.exists(os.path.join(plugin_config.oj_data_path, 'steam_id.json')): # Change old json into database
                 with open(os.path.join(plugin_config.oj_data_path, 'steam_id.json'), 'r', encoding='utf-8') as f:
                     data: Dict[str, str] = json.load(f)
                     for qq, steam64id in data.items():
                         await self.cursor.execute("INSERT INTO steamInfo VALUES (?, ?, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0)", (qq, steam64id))
+
             await self.db.commit()
             await self.db.close()
 
         self.db = await aiosqlite.connect(steam_id_file_path)
         self.cursor = await self.db.cursor()
 
         return self
@@ -151,18 +153,24 @@
                 data = await self.cursor.fetchall()
                 if data == [] or data is None:
                     await matcher.send('Ta还没有绑定过steam哦~')
                     return None
 
             
             img = f'https://interface.100oj.com/stat/render.php?steamid={data[0][0]}&render={data[0][1]}&sp1={data[0][2]}&limit={limit}'
-            if requests.get(img).content == b'': # Why aiohttp slower?
+            
+            async with aiohttp.ClientSession() as session:
+                req = await session.get(img)
+                data = await req.read()
+            
+            if data == b'':
                 await matcher.send(reply)
             else:
                 await matcher.send(MessageSegment.image(img))
+                
         except Exception as e:
             await matcher.send('诶鸭出错啦~')
             raise e
 
 
 
     async def stats(self, matcher: Matcher, event: Union[GroupMessageEvent, PrivateMessageEvent], arg: Message = CommandArg()) -> None:
@@ -235,14 +243,14 @@
                     case _:
                         await self.send_stats(matcher, at=at)
             case steam64id if steam64id.isdigit() and steam64id.startswith('7656') and len(steam64id) == 17:
                 steam64id = args[0]
                 match args[1]:
                     case limit if limit.isdigit():
                         limit: str = str(min(int(args[1]), 10))
-                        await self.send_stats(matcher, uid=uid, limit=limit)
+                        await self.send_stats(matcher, steam64id=steam64id, limit=limit)
                     case _:
-                        await self.send_stats(matcher, uid=uid)
+                        await self.send_stats(matcher, steam64id=steam64id)
             case _:
                 await self.help(matcher)
 
 stats: Stats = asyncio.run(Stats().init_database())
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice/__init__.py` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     usage= r'See Sorabot Docs.',
     type="application",
     supported_adapters={"~onebot.v11"},
     homepage="https://github.com/FDCraft/nonebot-plugin-orangejuice",
     config=Config,
     extra={
         'author': 'Polaris_Light',
-        'version': '0.7.0',
+        'version': '0.7.1',
         'priority': 10
     }
 )
 
 import re
 
 from nonebot import on_command, on_regex
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/PKG-INFO` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orangejuice
-Version: 0.7.0
+Version: 0.7.1
 Summary: Sorabot Implemention
 Author-email: Polaris_Light <995905922@qq.com>
 License: MIT License
         
         Copyright (c) 2024 Polaris Light
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-orangejuice Version: 0.7.1 Summary:
 Sorabot Implemention Author-email: Polaris_Light <995905922@qq.com> License:
 MIT License Copyright (c) 2024 Polaris Light Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `nonebot-plugin-orangejuice-0.7.0/nonebot_plugin_orangejuice.egg-info/SOURCES.txt` & `nonebot-plugin-orangejuice-0.7.1/nonebot_plugin_orangejuice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-orangejuice-0.7.0/pyproject.toml` & `nonebot-plugin-orangejuice-0.7.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-orangejuice"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.0.0-beta.1",
     "cachetools>=5.0.0",
     "aiohttp>=3.8.0",
     "aiosqlite>=0.20.0",
     "aiomysql>=0.2.0",
```

