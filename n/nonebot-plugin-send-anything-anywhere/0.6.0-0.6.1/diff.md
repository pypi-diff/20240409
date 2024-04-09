# Comparing `tmp/nonebot_plugin_send_anything_anywhere-0.6.0.tar.gz` & `tmp/nonebot_plugin_send_anything_anywhere-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.6.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.6.1.tar", max compression
```

## Comparing `nonebot_plugin_send_anything_anywhere-0.6.0.tar` & `nonebot_plugin_send_anything_anywhere-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1066 2024-02-23 02:24:51.895458 nonebot_plugin_send_anything_anywhere-0.6.0/LICENSE
--rw-r--r--   0        0        0     6885 2024-02-23 02:24:51.895458 nonebot_plugin_send_anything_anywhere-0.6.0/README.md
--rw-r--r--   0        0        0     2250 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/__init__.py
--rw-r--r--   0        0        0    25514 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/abstract_factories.py
--rw-r--r--   0        0        0      254 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/__init__.py
--rw-r--r--   0        0        0     8877 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/dodo.py
--rw-r--r--   0        0        0     6490 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/feishu.py
--rw-r--r--   0        0        0     6512 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/kaiheila.py
--rw-r--r--   0        0        0     9528 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/onebot_v11.py
--rw-r--r--   0        0        0    13706 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/onebot_v12.py
--rw-r--r--   0        0        0     8102 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/qq.py
--rw-r--r--   0        0        0     7764 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/red.py
--rw-r--r--   0        0        0     7307 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/telegram.py
--rw-r--r--   0        0        0     3789 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/auto_select_bot.py
--rw-r--r--   0        0        0      608 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/config.py
--rw-r--r--   0        0        0     2278 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/__init__.py
--rw-r--r--   0        0        0     1036 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/message_id.py
--rw-r--r--   0        0        0     1794 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/meta.py
--rw-r--r--   0        0        0     9466 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/platform_send_target.py
--rw-r--r--   0        0        0      656 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/receipt.py
--rw-r--r--   0        0        0      259 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/types/__init__.py
--rw-r--r--   0        0        0     3386 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/types/common_message_segment.py
--rw-r--r--   0        0        0     1176 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/types/custom_message_segment.py
--rw-r--r--   0        0        0      498 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/utils/__init__.py
--rw-r--r--   0        0        0      984 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/utils/const.py
--rw-r--r--   0        0        0      492 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/utils/exceptions.py
--rw-r--r--   0        0        0      479 2024-02-23 02:24:51.899458 nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/utils/helpers.py
--rw-r--r--   0        0        0     2135 2024-02-23 02:24:51.903458 nonebot_plugin_send_anything_anywhere-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.6.0/setup.py
--rw-r--r--   0        0        0     8002 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-09 08:51:34.497881 nonebot_plugin_send_anything_anywhere-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6885 2024-04-09 08:51:34.497881 nonebot_plugin_send_anything_anywhere-0.6.1/README.md
+-rw-r--r--   0        0        0     2317 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/__init__.py
+-rw-r--r--   0        0        0    25514 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/abstract_factories.py
+-rw-r--r--   0        0        0      285 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/__init__.py
+-rw-r--r--   0        0        0     8877 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/dodo.py
+-rw-r--r--   0        0        0     6490 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/feishu.py
+-rw-r--r--   0        0        0     6512 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/kaiheila.py
+-rw-r--r--   0        0        0     9528 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/onebot_v11.py
+-rw-r--r--   0        0        0    13706 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     8102 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/qq.py
+-rw-r--r--   0        0        0     7764 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/red.py
+-rw-r--r--   0        0        0    11782 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/satori.py
+-rw-r--r--   0        0        0     7307 2024-04-09 08:51:34.501881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/telegram.py
+-rw-r--r--   0        0        0     3789 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/auto_select_bot.py
+-rw-r--r--   0        0        0      608 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/config.py
+-rw-r--r--   0        0        0     2355 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/__init__.py
+-rw-r--r--   0        0        0     1036 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/message_id.py
+-rw-r--r--   0        0        0     1794 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/meta.py
+-rw-r--r--   0        0        0     9947 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/platform_send_target.py
+-rw-r--r--   0        0        0      656 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/receipt.py
+-rw-r--r--   0        0        0      259 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/types/__init__.py
+-rw-r--r--   0        0        0     3386 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/types/common_message_segment.py
+-rw-r--r--   0        0        0     1176 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/types/custom_message_segment.py
+-rw-r--r--   0        0        0      498 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/utils/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/utils/const.py
+-rw-r--r--   0        0        0      492 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/utils/exceptions.py
+-rw-r--r--   0        0        0      479 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/utils/helpers.py
+-rw-r--r--   0        0        0     2447 2024-04-09 08:51:34.505881 nonebot_plugin_send_anything_anywhere-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7970 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.6.1/setup.py
+-rw-r--r--   0        0        0     8043 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.6.1/PKG-INFO
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/LICENSE` & `nonebot_plugin_send_anything_anywhere-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/README.md` & `nonebot_plugin_send_anything_anywhere-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/__init__.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .registries import TargetDoDoChannel as TargetDoDoChannel
 from .registries import TargetDoDoPrivate as TargetDoDoPrivate
 from .registries import TargetFeishuGroup as TargetFeishuGroup
 from .abstract_factories import MessageFactory as MessageFactory
 from .registries import TargetFeishuPrivate as TargetFeishuPrivate
 from .registries import TargetQQGroupOpenId as TargetQQGroupOpenId
 from .registries import TargetQQGuildDirect as TargetQQGuildDirect
+from .registries import TargetSatoriUnknown as TargetSatoriUnknown
 from .registries import TargetTelegramForum as TargetTelegramForum
 from .registries import TargetQQGuildChannel as TargetQQGuildChannel
 from .registries import TargetTelegramCommon as TargetTelegramCommon
 from .registries import TargetKaiheilaChannel as TargetKaiheilaChannel
 from .registries import TargetKaiheilaPrivate as TargetKaiheilaPrivate
 from .registries import TargetQQPrivateOpenId as TargetQQPrivateOpenId
 from .auto_select_bot import enable_auto_select_bot as enable_auto_select_bot
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/abstract_factories.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/abstract_factories.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/dodo.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/dodo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/feishu.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/kaiheila.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/onebot_v11.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/onebot_v12.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/qq.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/qq.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/red.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/red.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/adapters/telegram.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/auto_select_bot.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/auto_select_bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/config.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/__init__.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .platform_send_target import QQGuildDMSManager as QQGuildDMSManager
 from .platform_send_target import TargetDoDoChannel as TargetDoDoChannel
 from .platform_send_target import TargetDoDoPrivate as TargetDoDoPrivate
 from .platform_send_target import TargetFeishuGroup as TargetFeishuGroup
 from .platform_send_target import TargetFeishuPrivate as TargetFeishuPrivate
 from .platform_send_target import TargetQQGroupOpenId as TargetQQGroupOpenId
 from .platform_send_target import TargetQQGuildDirect as TargetQQGuildDirect
+from .platform_send_target import TargetSatoriUnknown as TargetSatoriUnknown
 from .platform_send_target import TargetTelegramForum as TargetTelegramForum
 from .platform_send_target import TargetQQGuildChannel as TargetQQGuildChannel
 from .platform_send_target import TargetTelegramCommon as TargetTelegramCommon
 from .platform_send_target import register_qqguild_dms as register_qqguild_dms
 from .message_id import register_message_id_getter as register_message_id_getter
 from .platform_send_target import TargetKaiheilaChannel as TargetKaiheilaChannel
 from .platform_send_target import TargetKaiheilaPrivate as TargetKaiheilaPrivate
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/message_id.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/message_id.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/meta.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/meta.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/platform_send_target.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/platform_send_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,33 @@
     detail_type: Literal["private", "group", "channel"]
     user_id: Optional[str] = None
     group_id: Optional[str] = None
     guild_id: Optional[str] = None
     channel_id: Optional[str] = None
 
 
+class TargetSatoriUnknown(PlatformTarget):
+    """暂未识别的 Satori 发送目标
+
+    参数
+        platform: 平台名
+        user_id: 用户 ID
+        guild_id: 群组 ID
+        channel_id: 频道 ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.unknown_satori
+    ] = SupportedPlatform.unknown_satori
+    platform: str
+    user_id: Optional[str] = None
+    guild_id: Optional[str] = None
+    channel_id: Optional[str] = None
+
+
 class TargetKaiheilaChannel(PlatformTarget):
     """开黑啦频道
 
     参数
         channel_id: 频道ID
     """
 
@@ -272,14 +291,15 @@
     TargetKaiheilaPrivate,
     TargetKaiheilaChannel,
     TargetOB12Unknow,
     TargetTelegramCommon,
     TargetTelegramForum,
     TargetFeishuPrivate,
     TargetFeishuGroup,
+    TargetSatoriUnknown,
 ]
 
 
 ConvertToArg = Callable[[PlatformTarget], Dict[str, Any]]
 convert_to_arg_map: Dict[Tuple[SupportedPlatform, SupportedAdapters], ConvertToArg] = {}
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/registries/receipt.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/registries/receipt.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/types/common_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/types/common_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/types/custom_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/types/custom_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/nonebot_plugin_saa/utils/const.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/nonebot_plugin_saa/utils/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,30 @@
     onebot_v12 = "OneBot V12"
     kaiheila = "Kaiheila"
     telegram = "Telegram"
     feishu = "Feishu"
     red = "RedProtocol"
     dodo = "DoDo"
     qq = "QQ"
+    satori = "Satori"
 
     fake = "fake"  # for nonebug
 
 
 class SupportedPlatform(StrEnum):
     qq_group = "QQ Group"
     qq_private = "QQ Private"
     qq_group_openid = "QQ Group OpenID"
     qq_private_openid = "QQ Private OpenID"
     qq_guild_channel = "QQ Guild Channel"
     qq_guild_direct = "QQ Guild Direct"
     kaiheila_channel = "Kaiheila Channel"
     kaiheila_private = "Kaiheila Private"
     unknown_ob12 = "Unknow Onebot 12 Platform"
+    unknown_satori = "Unknown Satori Platform"
     telegram_common = "Telegram Common"
     telegram_forum = "Telegram Forum"
     feishu_private = "Feishu Private"
     feishu_group = "Feishu Group"
     dodo_channel = "DoDo Channel"
     dodo_private = "DoDo Private"
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/pyproject.toml` & `nonebot_plugin_send_anything_anywhere-0.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-send-anything-anywhere"
-version = "0.6.0"
+version = "0.6.1"
 description = "An adaptor for nonebot2 adaptors"
 authors = ["felinae98 <731499577@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_saa" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -20,14 +20,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0"
 strenum = "^0.4.8"
 pydantic = ">=1.10.0,<3.0.0,!=2.5.0,!=2.5.1"
 anyio = ">=3.3.0,<5.0.0"
+filetype = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.2"
 ipdb = "^0.13.9"
 pip = "^23.0"
 pytest-cov = "^4.0.0"
 nonebug = "^0.3.1"
@@ -47,14 +48,15 @@
 nonebot-adapter-onebot = "^2.4.0"
 nonebot-adapter-kaiheila = "^0.3.1"
 nonebot-adapter-telegram = { git = "https://github.com/nonebot/adapter-telegram.git" }
 nonebot-adapter-feishu = "^2.4.0"
 nonebot-adapter-red = "^0.9.0"
 nonebot-adapter-dodo = "^0.2.0"
 nonebot-adapter-qq = "^1.4.1"
+nonebot-adapter-satori = "^0.10.2"
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
@@ -82,7 +84,16 @@
 [tool.coverage.report]
 exclude_also = [
   "raise NotImplementedError",
   "if TYPE_CHECKING:",
   "except ImportError:",
   "except Exception as e:",
 ]
+
+[tool.nonebot]
+adapters = [
+  { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
+  {name = "Satori", module_name = "nonebot.adapters.satori"},
+]
+plugins = ["nonebot_plugin_saa"]
+plugin_dirs = ["extra_plugins"]
+builtin_plugins = ["echo"]
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/setup.py` & `nonebot_plugin_send_anything_anywhere-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,22 @@
  'nonebot_plugin_saa.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['anyio>=3.3.0,<5.0.0',
+ 'filetype>=1.2.0,<2.0.0',
  'nonebot2>=2.0.0,<3.0.0',
  'pydantic>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1',
  'strenum>=0.4.8,<0.5.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-send-anything-anywhere',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'An adaptor for nonebot2 adaptors',
     'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们 | [文档](https://send-anything-anywhere.felinae98.cn/)\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n[![codecov](https://codecov.io/gh/MountainDash/nonebot-plugin-send-anything-anywhere/graph/badge.svg?token=7EV2hcYx8d)](https://codecov.io/gh/MountainDash/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为群号 114514 的群聊\ntarget = TargetQQGroup(group_id=114514)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target, SaaTarget\n\n@matcher.handle()\nasync def handle(event: MessageEvent, bot: Bot):\n    # 只有混入了 Specifier 的 PlatformTarget（例如 OpenID 版 QQ）需要传入 bot\n    target = extract_target(event, bot)\n\n@matcher.handle()\nasync def handle(target: SaaTarget):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | Kaiheila | Telegram | Feishu | Red | DoDo |\n| :--------: | :--------: | :------: | :------: | :----: | :-: | :--: |\n|     ✅     |     ✅     |    ✅    |    ✅    |   ✅   | ✅  |  ✅  |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | 开黑啦 | Telegram | Feishu | Red | DoDo |\n| :--: | :--------: | :--------: | :----: | :------: | :----: | :-: | :--: |\n| 文字 |     ✅     |     ✅     |   ✅   |    ✅    |   ✅   | ✅  |  ✅  |\n| 图片 |     ✅     |     ✅     |   ✅   |    ✅    |   ✅   | ✅  |  ✅  |\n|  at  |     ✅     |     ✅     |   ✅   |    ✅    |   ✅   | ✅  |  ✅  |\n| 回复 |     ✅     |     ✅     |   ✅   |    ✅    |   ✅   | 🚧  |  ✅  |\n\n### 支持的发送目标\n\n|                        | OneBot v11 | OneBot v12 | Kaiheila | Telegram | Feishu | Red | DoDo |\n| :--------------------: | :--------: | :--------: | :------: | :------: | :----: | :-: | :--: |\n|         QQ 群          |     ✅     |     ✅     |          |          |        | ✅  |      |\n|        QQ 私聊         |     ✅     |     ✅     |          |          |        | ✅  |      |\n|   QQ 频道子频道消息    |            |     ✅     |          |          |        |     |      |\n|      QQ 频道私聊       |            |     ✅     |          |          |        |     |      |\n|    开黑啦私聊/频道     |            |            |    ✅    |          |        |     |      |\n| Telegram 普通对话/频道 |            |            |          |    ✅    |        |     |      |\n|     飞书私聊/群聊      |            |            |          |          |   ✅   |     |      |\n|     DoDo 私聊/群聊     |            |            |          |          |        |     |  ✅  |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\n@pic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\n@pic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\n@pic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
     'author': 'felinae98',
     'author_email': '731499577@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.6.0/PKG-INFO` & `nonebot_plugin_send_anything_anywhere-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-send-anything-anywhere
-Version: 0.6.0
+Version: 0.6.1
 Summary: An adaptor for nonebot2 adaptors
 License: MIT
 Author: felinae98
 Author-email: 731499577@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: anyio (>=3.3.0,<5.0.0)
+Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1)
 Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
```

