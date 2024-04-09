# Comparing `tmp/line-web-0.0.5.tar.gz` & `tmp/line-web-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-web-0.0.5.tar", last modified: Tue Apr  9 07:12:01 2024, max compression
+gzip compressed data, was "line-web-0.0.6.tar", last modified: Tue Apr  9 07:30:14 2024, max compression
```

## Comparing `line-web-0.0.5.tar` & `line-web-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:12:01.343369 line-web-0.0.5/
--rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 line-web-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 line-web-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1661 2024-04-09 07:12:01.343369 line-web-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      960 2024-04-03 10:07:33.000000 line-web-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 07:12:01.327640 line-web-0.0.5/line/
--rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 line-web-0.0.5/line/__init__.py
--rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 line-web-0.0.5/line/authentications.py
--rw-rw-rw-   0        0        0    33342 2024-04-09 07:11:42.000000 line-web-0.0.5/line/core.py
--rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 line-web-0.0.5/line/exceptions.py
--rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 line-web-0.0.5/line/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:12:01.327640 line-web-0.0.5/line_web.egg-info/
--rw-rw-rw-   0        0        0     1661 2024-04-09 07:12:01.000000 line-web-0.0.5/line_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-09 07:12:01.000000 line-web-0.0.5/line_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:12:01.000000 line-web-0.0.5/line_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-09 07:12:01.000000 line-web-0.0.5/line_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-09 07:12:01.000000 line-web-0.0.5/line_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 07:12:01.343369 line-web-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3899 2024-04-09 07:11:42.000000 line-web-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:30:14.727615 line-web-0.0.6/
+-rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 line-web-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 line-web-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1661 2024-04-09 07:30:14.723609 line-web-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2024-04-03 10:07:33.000000 line-web-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:30:14.719605 line-web-0.0.6/line/
+-rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 line-web-0.0.6/line/__init__.py
+-rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 line-web-0.0.6/line/authentications.py
+-rw-rw-rw-   0        0        0    33219 2024-04-09 07:24:35.000000 line-web-0.0.6/line/core.py
+-rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 line-web-0.0.6/line/exceptions.py
+-rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 line-web-0.0.6/line/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:30:14.723609 line-web-0.0.6/line_web.egg-info/
+-rw-rw-rw-   0        0        0     1661 2024-04-09 07:30:14.000000 line-web-0.0.6/line_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-09 07:30:14.000000 line-web-0.0.6/line_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:30:14.000000 line-web-0.0.6/line_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-09 07:30:14.000000 line-web-0.0.6/line_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-09 07:30:14.000000 line-web-0.0.6/line_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 07:30:14.727615 line-web-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3899 2024-04-09 07:25:15.000000 line-web-0.0.6/setup.py
```

### Comparing `line-web-0.0.5/LICENSE` & `line-web-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `line-web-0.0.5/PKG-INFO` & `line-web-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-web
-Version: 0.0.5
+Version: 0.0.6
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-web
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `line-web-0.0.5/README.md` & `line-web-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `line-web-0.0.5/line/authentications.py` & `line-web-0.0.6/line/authentications.py`

 * *Files identical despite different names*

### Comparing `line-web-0.0.5/line/core.py` & `line-web-0.0.6/line/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,30 +49,30 @@
         self.bot_id = self.bot["botId"]
         self.basic_search_id = self.bot["basicSearchId"]
         self.enable_chat()
 
         self.event_funcs = {"event": []}
         self.event_emitter = pyee.executor.ExecutorEventEmitter()
 
-    def select_bot(self, name: str) -> dict | typing.NoReturn:
+    def select_bot(self, name: str) -> dict:
         bots = self.bots()
         try:
             if not bots["list"]:
                 raise BotNotExistsException(bots["list"])
 
             for bot in bots["list"]:
                 if bot["name"] == name:
                     return bot
         except KeyError:
             pass
 
         raise BotNotFoundException(bots)
 
     @classmethod
-    def extract_emojis(cls, raw_text: str) -> list | None:
+    def extract_emojis(cls, raw_text: str) -> typing.Union[list, None]:
         pattern = "\[EM:([\w\d]+),id=([\w\d]+)\]"
         emojis = []
         gap = 0
         for match in re.finditer(pattern, raw_text):
             product_id = match.group(1)
             emoji_id = match.group(2)
             start = match.start()
@@ -630,30 +630,30 @@
         response = self.session.put(url)
         return response.json()
 
     @classmethod
     def make_send_id(cls, contact_id: str) -> str:
         return "_".join([contact_id, str(int(time.time() * 1000)), str(int(random.random() * 1e8))])
 
-    def upload_file(self, contact_id: str, file: bytes | typing.IO) -> dict:
+    def upload_file(self, contact_id: str, file: typing.Union[bytes, typing.IO]) -> dict:
         """上传待发送文件"""
         url = self.CHAT_HOST + f"/api/v1/bots/{self.bot_id}/messages/{contact_id}/uploadFile"
         files = {
             "file": file
         }
         response = self.session.post(url, files=files)
         return response.json()
 
     def bulk_send_files(self, contact_id: str, data: dict) -> dict:
         """批量发送文件"""
         url = self.CHAT_HOST + f"/api/v1/bots/{self.bot_id}/messages/{contact_id}/bulkSendFiles"
         response = self.session.post(url, json=data)
         return response.json()
 
-    def send(self, **kwargs: typing.Any) -> dict | typing.NoReturn:
+    def send(self, **kwargs: typing.Any) -> dict:
         """发送消息"""
         if "emojis" in kwargs:
             emojis = kwargs.get("emojis")
             if emojis is not None:
                 if not isinstance(emojis, list):
                     raise TypeError("emojis must be a list.")
 
@@ -682,28 +682,28 @@
         response = self.session.post(url, json=data)
         return {
             "send_id": send_id,
             **response.json(),
         }
 
     @staticmethod
-    def manual_chat_mode(f: typing.Callable) -> typing.Callable[["Line", typing.Any], dict | typing.NoReturn]:
-        def wrapper(self: "Line", *args: typing.Any, **kwargs: typing.Any) -> dict | typing.NoReturn:
+    def manual_chat_mode(f: typing.Callable) -> typing.Callable[["Line", typing.Any], dict]:
+        def wrapper(self: "Line", *args: typing.Any, **kwargs: typing.Any) -> dict:
             if "contact_id" not in kwargs:
                 raise ValueError("Missing required argument: contact_id")
 
             self.set_use_manual_chat(kwargs["contact_id"])
             data = f(self, *args, **kwargs)
             self.delete_use_manual_chat(kwargs["contact_id"])
             return data
 
         return wrapper
 
     @manual_chat_mode
-    def send_file_msg(self, contact_id: str, file: bytes | typing.IO) -> dict:
+    def send_file_msg(self, contact_id: str, file: typing.Union[bytes, typing.IO]) -> dict:
         """发送文件"""
         send_id = self.make_send_id(contact_id)
         content_message_token = self.upload_file(contact_id, file)["contentMessageToken"]
         data = {"items": [{"contentMessageToken": content_message_token, "sendId": send_id}]}
         return {
             "send_id": send_id,
             **self.bulk_send_files(
@@ -715,15 +715,15 @@
     @manual_chat_mode
     def send_text_msg(
         self,
         contact_id: str,
         text: str,
         escape: typing.Optional[bool] = False,
         quote_token: typing.Optional[bool] = None
-    ) -> dict | typing.NoReturn:
+    ) -> dict:
         """发送文本消息"""
         return self.send(**{
             "type": "text",
             "contact_id": contact_id,
             "text": text,
             "emojis": self.extract_emojis(text) if not escape else None,
             "quoteToken": quote_token
@@ -732,35 +732,35 @@
     @manual_chat_mode
     def send_sticker_msg(
         self,
         contact_id: str,
         package_id: int,
         sticker_id: int,
         quote_token: typing.Optional[str] = None
-    ) -> dict | typing.NoReturn:
+    ) -> dict:
         """发送表情包消息"""
         return self.send(**{
             "type": "sticker",
             "contact_id": contact_id,
             "stickerId": sticker_id,
             "packageId": package_id,
             "quoteToken": quote_token
         })
 
     @manual_chat_mode
-    def send_card_msg(self, contact_id: str, card_type_message_id: str) -> dict | typing.NoReturn:
+    def send_card_msg(self, contact_id: str, card_type_message_id: str) -> dict:
         """发送卡片消息"""
         return self.send(**{
             "type": "cardType",
             "contact_id": contact_id,
             "cardTypeMessageId": card_type_message_id
         })
 
     @manual_chat_mode
-    def send_call_msg(self, contact_id: str) -> dict | typing.NoReturn:
+    def send_call_msg(self, contact_id: str) -> dict:
         """发送语音聊天邀请"""
         return self.send(**{
             "type": "callGuide",
             "contact_id": contact_id,
         })
 
     def sse(
@@ -782,15 +782,15 @@
         }
         response = self.session.get(url, params=params, stream=True)
         for event_data in response.iter_lines(delimiter=b"\n\n"):
             if event_data != b"":
                 yield event_data
 
     def handle(self, event: typing.Optional[str] = None, sub_event: typing.Optional[str] = None) -> typing.Callable:
-        def wrapper(f: typing.Callable) -> None | typing.NoReturn:
+        def wrapper(f: typing.Callable) -> None:
             if event is not None:
                 if not isinstance(event, str):
                     raise TypeError("event must be a str.")
 
             if sub_event is not None:
                 if not isinstance(sub_event, str):
                     raise TypeError("sub_event must be a str.")
```

### Comparing `line-web-0.0.5/line_web.egg-info/PKG-INFO` & `line-web-0.0.6/line_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-web
-Version: 0.0.5
+Version: 0.0.6
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-web
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `line-web-0.0.5/setup.py` & `line-web-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'line-web'
 DESCRIPTION = 'Line chatbot framework.'
 URL = 'https://github.com/miloira/line-web'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'loguru',
     'pyee'
 ]
```

