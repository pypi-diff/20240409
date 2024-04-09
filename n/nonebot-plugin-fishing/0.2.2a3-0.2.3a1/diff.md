# Comparing `tmp/nonebot-plugin-fishing-0.2.2a3.tar.gz` & `tmp/nonebot-plugin-fishing-0.2.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fishing-0.2.2a3.tar", last modified: Fri Apr  5 11:18:29 2024, max compression
+gzip compressed data, was "nonebot-plugin-fishing-0.2.3a1.tar", last modified: Tue Apr  9 14:32:26 2024, max compression
```

## Comparing `nonebot-plugin-fishing-0.2.2a3.tar` & `nonebot-plugin-fishing-0.2.3a1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/68463f3e5f33_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/da5a91612ef2_init_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/setup.cfg
```

### Comparing `nonebot-plugin-fishing-0.2.2a3/LICENSE` & `nonebot-plugin-fishing-0.2.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.2a3/PKG-INFO` & `nonebot-plugin-fishing-0.2.3a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.2a3
+Version: 0.2.3a1
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
@@ -83,23 +83,26 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 说明 |
 |:-----:|:----:|:----:|
 | fishes | 否 | 配置鱼塘内鱼们的名称、权重、等待时间和价格 |
 | fishing_limit | 否 | 填入每次钓鱼后，限制钓鱼的秒数 |
+| fishing_coin_name | 否 | 填入卖鱼获取的货币名称 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
+| 卖鱼 | 所有 | 卖鱼 |
 
 ## 📝 Todo
 
-- [x] 重写数据库逻辑（改为使用[nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
-- [ ] 增加系统商店，卖出钓到的鱼们
+- [x] 重写数据库逻辑（改为使用 [nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
+- [x] 增加系统商店，卖出钓到的鱼们
+- [ ] 赛博放生 [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4)
 - [ ] 为鱼竿增加耐久度，耐久度为0时需重新购买鱼竿
 - [ ] 为钓鱼背包添加排序
 - [ ] 添加成就系统
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.2a3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a1 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -18,15 +18,17 @@
 install nonebot-plugin-fishing æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_fishing"] æ³¨æï¼å®è£è¿åï¼éå¨æ§å¶å°è¾å¥ `nb
 orm upgrade` æä»¤ä»¥åå§åæ°æ®åºã ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
-fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| |
-éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° |
-| èå | ææ | æ¥çèå | ## ð Todo - [x]
-éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨[nonebot/plugin-orm](https://github.com/
-nonebot/plugin-orm)ï¼ - [ ] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
-ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
+fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
+fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | ## ð ä½¿ç¨
+### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ |
+ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå
+| ææ | æ¥çèå | | åé±¼ | ææ | åé±¼ | ## ð Todo - [x]
+éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/plugin-orm](https://github.com/
+nonebot/plugin-orm)ï¼ - [x] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
+èµåæ¾ç [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4) -
+[ ] ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.2a3/README.md` & `nonebot-plugin-fishing-0.2.3a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,23 +67,26 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 说明 |
 |:-----:|:----:|:----:|
 | fishes | 否 | 配置鱼塘内鱼们的名称、权重、等待时间和价格 |
 | fishing_limit | 否 | 填入每次钓鱼后，限制钓鱼的秒数 |
+| fishing_coin_name | 否 | 填入卖鱼获取的货币名称 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
+| 卖鱼 | 所有 | 卖鱼 |
 
 ## 📝 Todo
 
-- [x] 重写数据库逻辑（改为使用[nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
-- [ ] 增加系统商店，卖出钓到的鱼们
+- [x] 重写数据库逻辑（改为使用 [nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
+- [x] 增加系统商店，卖出钓到的鱼们
+- [ ] 赛博放生 [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4)
 - [ ] 为鱼竿增加耐久度，耐久度为0时需重新购买鱼竿
 - [ ] 为钓鱼背包添加排序
 - [ ] 添加成就系统
```

#### html2text {}

```diff
@@ -11,15 +11,17 @@
 install nonebot-plugin-fishing æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_fishing"] æ³¨æï¼å®è£è¿åï¼éå¨æ§å¶å°è¾å¥ `nb
 orm upgrade` æä»¤ä»¥åå§åæ°æ®åºã ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
-fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| |
-éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° |
-| èå | ææ | æ¥çèå | ## ð Todo - [x]
-éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨[nonebot/plugin-orm](https://github.com/
-nonebot/plugin-orm)ï¼ - [ ] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
-ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
+fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
+fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | ## ð ä½¿ç¨
+### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ |
+ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå
+| ææ | æ¥çèå | | åé±¼ | ææ | åé±¼ | ## ð Todo - [x]
+éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/plugin-orm](https://github.com/
+nonebot/plugin-orm)ï¼ - [x] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
+èµåæ¾ç [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4) -
+[ ] ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/__init__.py` & `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from nonebot import on_command, require
 
 require("nonebot_plugin_orm")  # noqa
 from nonebot.plugin import PluginMetadata
-from nonebot.adapters import Event
+from nonebot.adapters import Event, Message
+from nonebot.params import CommandArg
 
 import asyncio
 
 from .config import Config
 from .data_source import (choice,
                           is_fishing,
                           get_stats,
                           save_fish,
-                          get_backpack)
+                          get_backpack,
+                          sell_fish,
+                          get_balance)
 
 __plugin_meta__ = PluginMetadata(
     name="赛博钓鱼",
     description="你甚至可以电子钓鱼",
     usage="发送“钓鱼”，放下鱼竿。",
     type="application",
     homepage="https://github.com/C14H22O/nonebot-plugin-fishing",
-    config=Config
+    config=Config,
+    supported_adapters=None
 )
 
-fishing = on_command("fishing", aliases={"钓鱼"})
-stats = on_command("stats", aliases={"统计信息"})
-backpack = on_command("backpack", aliases={"背包"})
-sell = on_command("sell", aliases={"卖鱼"})
+fishing = on_command("fishing", aliases={"钓鱼"}, priority=5)
+stats = on_command("stats", aliases={"统计信息"}, priority=5)
+backpack = on_command("backpack", aliases={"背包"}, priority=5)
+sell = on_command("sell", aliases={"卖鱼"}, priority=5)
+balance = on_command("balance", aliases={"余额"}, priority=5)
 
 
 @fishing.handle()
 async def _fishing(event: Event):
     user_id = event.get_user_id()
     if not await is_fishing(user_id):
         await fishing.finish("河累了, 休息一下吧")
@@ -52,9 +57,19 @@
 @backpack.handle()
 async def _backpack(event: Event):
     user_id = event.get_user_id()
     await backpack.finish(await get_backpack(user_id))
 
 
 @sell.handle()
-async def _sell(event: Event):
-    await sell.finish("商店正在施工中…")
+async def _sell(event: Event, arg: Message = CommandArg()):
+    fish_name = arg.extract_plain_text()
+    if fish_name == "":
+        await sell.finish("请输入要卖出的鱼的名字, 如 /卖鱼 小鱼")
+    user_id = event.get_user_id()
+    await sell.finish(await sell_fish(user_id, fish_name))
+
+
+@balance.handle()
+async def _balance(event: Event):
+    user_id = event.get_user_id()
+    await balance.finish(await get_balance(user_id))
```

### Comparing `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/config.py` & `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pydantic import BaseModel
-
 from typing import List, Dict
 from nonebot import get_plugin_config
 
 
 class Config(BaseModel):
 
     fishes: List[Dict] = [
@@ -31,9 +30,11 @@
             "weight": 1,
             "price": 50
         }
     ]
 
     fishing_limit: int = 30
 
+    fishing_coin_name: str = "FC"  # Fishing Coin
+
 
 config = get_plugin_config(Config)
```

### Comparing `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py` & `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/da5a91612ef2_init_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-"""init db
-
-迁移 ID: 7609e6d106dd
-父迁移: 
-创建时间: 2024-04-05 19:08:58.835014
-
-"""
-from __future__ import annotations
-
-from collections.abc import Sequence
-
-from alembic import op
-import sqlalchemy as sa
-
-
-revision: str = '7609e6d106dd'
-down_revision: str | Sequence[str] | None = None
-branch_labels: str | Sequence[str] | None = ('nonebot_plugin_fishing',)
-depends_on: str | Sequence[str] | None = None
-
-
-def upgrade(name: str = "") -> None:
-    if name:
-        return
-    # ### commands auto generated by Alembic - please adjust! ###
-    op.create_table('nonebot_plugin_fishing_fishingrecord',
-    sa.Column('id', sa.Integer(), nullable=False),
-    sa.Column('user_id', sa.String(length=32), nullable=False),
-    sa.Column('time', sa.Integer(), nullable=False),
-    sa.Column('frequency', sa.Integer(), nullable=False),
-    sa.Column('fishes', sa.TEXT(), nullable=False),
-    sa.Column('coin', sa.Integer(), nullable=False),
-    sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_fishing_fishingrecord')),
-    info={'bind_key': 'nonebot_plugin_fishing'}
-    )
-    # ### end Alembic commands ###
-
-
-def downgrade(name: str = "") -> None:
-    if name:
-        return
-    # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_table('nonebot_plugin_fishing_fishingrecord')
-    # ### end Alembic commands ###
+"""init db
+迁移 ID: da5a91612ef2
+父迁移: 
+创建时间: 2024-03-09 15:10:34.633951
+"""
+from __future__ import annotations
+
+from collections.abc import Sequence
+
+from alembic import op
+import sqlalchemy as sa
+
+
+revision: str = 'da5a91612ef2'
+down_revision: str | Sequence[str] | None = None
+branch_labels: str | Sequence[str] | None = ('nonebot_plugin_fishing',)
+depends_on: str | Sequence[str] | None = None
+
+
+def upgrade(name: str = "") -> None:
+    if name:
+        return
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.create_table('nonebot_plugin_fishing_fishingrecord',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.String(), nullable=False),
+    sa.Column('time', sa.Integer(), nullable=False),
+    sa.Column('frequency', sa.Integer(), nullable=False),
+    sa.Column('fishes', sa.String(), nullable=False),
+    sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_fishing_fishingrecord')),
+    info={'bind_key': 'nonebot_plugin_fishing'}
+    )
+    # ### end Alembic commands ###
+
+
+def downgrade(name: str = "") -> None:
+    if name:
+        return
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.drop_table('nonebot_plugin_fishing_fishingrecord')
+    # ### end Alembic commands ###
```

### Comparing `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/PKG-INFO` & `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.2a3
+Version: 0.2.3a1
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
@@ -83,23 +83,26 @@
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 说明 |
 |:-----:|:----:|:----:|
 | fishes | 否 | 配置鱼塘内鱼们的名称、权重、等待时间和价格 |
 | fishing_limit | 否 | 填入每次钓鱼后，限制钓鱼的秒数 |
+| fishing_coin_name | 否 | 填入卖鱼获取的货币名称 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
+| 卖鱼 | 所有 | 卖鱼 |
 
 ## 📝 Todo
 
-- [x] 重写数据库逻辑（改为使用[nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
-- [ ] 增加系统商店，卖出钓到的鱼们
+- [x] 重写数据库逻辑（改为使用 [nonebot/plugin-orm](https://github.com/nonebot/plugin-orm)）
+- [x] 增加系统商店，卖出钓到的鱼们
+- [ ] 赛博放生 [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4)
 - [ ] 为鱼竿增加耐久度，耐久度为0时需重新购买鱼竿
 - [ ] 为钓鱼背包添加排序
 - [ ] 添加成就系统
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.2a3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a1 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -18,15 +18,17 @@
 install nonebot-plugin-fishing æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_fishing"] æ³¨æï¼å®è£è¿åï¼éå¨æ§å¶å°è¾å¥ `nb
 orm upgrade` æä»¤ä»¥åå§åæ°æ®åºã ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
-fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| |
-éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° |
-| èå | ææ | æ¥çèå | ## ð Todo - [x]
-éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨[nonebot/plugin-orm](https://github.com/
-nonebot/plugin-orm)ï¼ - [ ] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
-ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
+fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
+fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | ## ð ä½¿ç¨
+### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ |
+ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå
+| ææ | æ¥çèå | | åé±¼ | ææ | åé±¼ | ## ð Todo - [x]
+éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/plugin-orm](https://github.com/
+nonebot/plugin-orm)ï¼ - [x] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
+èµåæ¾ç [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4) -
+[ ] ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

