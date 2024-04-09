# Comparing `tmp/wechat_pyrobot-1.2.6.tar.gz` & `tmp/wechat_pyrobot-1.3.0.tar.gz`

## Comparing `wechat_pyrobot-1.2.6.tar` & `wechat_pyrobot-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/__init__.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/anti_revoke32.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/anti_revoke64.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/ctypes_json.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/hooklog32.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/hooklog64.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/hookmsg32.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/hookmsg64.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/offset.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/plugin_class.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/sendmsg32.py
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/sendmsg64.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/msg_plugins/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/msg_plugins/download_emotion.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/msg_plugins/monitor_biz.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/msg_plugins/print_msg.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/other_plugins/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/src/wechat_pyrobot/other_plugins/http_api.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/tests/case.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/tests/case1.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/LICENSE
--rw-r--r--   0        0        0     6116 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 wechat_pyrobot-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/__init__.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/anti_revoke32.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/anti_revoke64.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/ctypes_json.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/get_contact_list.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/hooklog32.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/hooklog64.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/hookmsg32.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/hookmsg64.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/offset.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/plugin_class.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/sendmsg32.py
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/sendmsg64.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/msg_plugins/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/msg_plugins/download_emotion.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/msg_plugins/monitor_biz.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/msg_plugins/print_msg.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/other_plugins/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/src/wechat_pyrobot/other_plugins/http_api.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/tests/case.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/tests/case1.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 wechat_pyrobot-1.3.0/PKG-INFO
```

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/__init__.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 
 
 if "64" in platform.architecture()[0]:
     from .sendmsg64 import SendMsg
     from .hooklog64 import HookLog
     from .anti_revoke64 import AntiRevoke
     from .hookmsg64 import HookMsg
+    from .get_contact_list import GetContacts
 else:
     from .sendmsg32 import SendMsg
     from .hooklog32 import HookLog
     from .anti_revoke32 import AntiRevoke
     from .hookmsg32 import HookMsg
 
 
-__version__ = "1.2.6"
+__version__ = "1.3.0"
 
 __all__ = [
     "SendMsg",
     "HookLog",
     "HookMsg",
     "AntiRevoke",
+    "GetContacts",
     "get_on_startup"
 ]
 
 
 def get_on_startup(msg_plugins=[], other_plugins=[]):
     '''注入后立即执行的函数'''
     msg_queue = queue.Queue()
```

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/anti_revoke32.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/anti_revoke32.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/anti_revoke64.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/anti_revoke64.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/ctypes_json.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/ctypes_json.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/hooklog32.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/hooklog32.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/hooklog64.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/hooklog64.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/hookmsg32.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/hookmsg32.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/hookmsg64.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/hookmsg64.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/plugin_class.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/plugin_class.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/sendmsg32.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/sendmsg32.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/sendmsg64.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/sendmsg64.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/msg_plugins/download_emotion.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/msg_plugins/download_emotion.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/msg_plugins/monitor_biz.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/msg_plugins/monitor_biz.py`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/src/wechat_pyrobot/other_plugins/http_api.py` & `wechat_pyrobot-1.3.0/src/wechat_pyrobot/other_plugins/http_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 给发送消息提供http接口服务
 '''
 from threading import Thread
-from .. import SendMsg
+from .. import SendMsg, GetContacts
 from typing import List
 import uvicorn
 from fastapi import FastAPI
 from pydantic import BaseModel
 
 app = FastAPI()
 
@@ -23,15 +23,15 @@
     msg: str 
     atwxid: List[str]
 
 class HttpApi(Thread):
     def __init__(self) -> None:
         super().__init__()
         sg = SendMsg()
-
+        
         @app.post("/post_sendmsg")
         def post_sendmsg(item:MsgItem):
             touser = item.touser
             msg = item.msg
             r = sg.send_text(touser, msg)
             return {"result": r}
 
@@ -62,14 +62,18 @@
             r = sg.send_at_text(touser, msg, [atwxid])
             return {"result": r}
         
         @app.get("/sendimage")
         def sendimage(touser: str, path: str):
             r = sg.send_image(touser, path)
             return {"result": r}
+        
+        @app.get("/contacts")
+        def getcontacts():
+            return GetContacts().value
     
     def run(self):
         uvicorn.run(app="wechat_pyrobot.other_plugins.http_api:app", host="127.0.0.1", port=26666, reload=False)
 
 
 if __name__ == "__main__":
     HttpApi().start()
```

### Comparing `wechat_pyrobot-1.2.6/LICENSE` & `wechat_pyrobot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wechat_pyrobot-1.2.6/README.md` & `wechat_pyrobot-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,35 +21,38 @@
 64位:
 - `3.9.8.15`
 
 等这个系列教程结束再更新新版本，hook库和主动调用都已经说完了，也可以等群友提pr来更新。
 
 #### 群二维码
 
-![](http://cdn.ikanade.cn/Python_room_qrcode_20240229.jpg)
+![](http://cdn.ikanade.cn/Python_room_qrcode_20240407.jpg)
 
-如果二维码失效了，可以加我好友`kanadeblisst`，备注`进群`
+如果二维码失效了，可以加我好友`kanadeblisst`，备注`机器人群`
 
 ## 使用教程
 
 #### 当前支持功能
 
 - 发送文本消息
 - 发送AT消息
 - 发送图片消息
 - hook微信日志输出
 - hook接收消息
 - 消息防撤回
 - 下载聊天表情包
+- 获取好友列表
+- 获取群列表
+- 获取公众号列表
 
 #### 准备环境
 
 1. 安装支持的版本(`3.9.8.15`)微信
-2. 安装Python，版本大于等于3.8
-3. `pip install wechat_pyrobot==1.2.2`
+2. 安装Python，版本大于等于3.8 (最好就用3.8)，测试3.10+容易出bug
+3. `pip install wechat_pyrobot==1.3.0`
 
 如果国内源还没有同步最新版本，可以指定`-i https://pypi.org/simple/` 选项使用pip官方库
 
 #### 使用
 
 首先创建一个目录，例如`robot_code`，再创建一个`main.py`(名称随意)写入以下代码:
 ```python
@@ -137,18 +140,28 @@
 data = {
     "touser": "filehelper",
     "msg": "测试消息2"
 }
 
 requests.post(url, json=data)
 ```
+#### 联系人列表
+
+目前没有区分公众号、群和好友，有需求的可以自己加判断区分
+
+```python
+import requests
+
+url = "http://127.0.0.1:26666/contacts"
+print(requests.get(url).json())
+```
 
 #### 接收消息
 
-接收消息现在由插件控制，你可以编写自己的插件然后在`get_on_startup`的参数msg_plugins添加它
+接收消息现在由插件控制，你可以编写自己的插件然后在`get_on_startup`的参数msg_plugins添加它。插件执行目前是同步单线程，如果需要多线程的话，可以自己根据需要修改get_on_startup里的msg_thread_func函数。
 
 例如我想写一个将消息保存到文件的插件, `robot_code`下新建一个目录my_msg_plugin，下面新建一个文件`save_to_file.py`：
 
 ```python
 import os
 import json
 from wechat_pyrobot.plugin_class import MsgPluginTemplate
@@ -173,14 +186,15 @@
 ```python
 from py_process_hooker import inject_python_and_monitor_dir
 from wechat_pyrobot import get_on_startup
 from wechat_pyrobot.msg_plugins import PrintMsg, DownLoadEmotion
 from wechat_pyrobot.other_plugins import HttpApi
 from my_msg_plugin.save_to_file import SaveToFile
 
+
 if __name__ == "__main__":
     process_name = "WeChat.exe"
     open_console = True
     on_startup = get_on_startup(msg_plugins=[PrintMsg, DownLoadEmotion, SaveToFile], other_plugins=[HttpApi])
     
     inject_python_and_monitor_dir(process_name, __file__, open_console=open_console, on_startup=on_startup)
 ```
```

### Comparing `wechat_pyrobot-1.2.6/pyproject.toml` & `wechat_pyrobot-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wechat_pyrobot"
-version = "1.2.6"
+version = "1.3.0"
 authors = [
   { name="kanadeblisst", email="kanade@blisst.cn" },
 ]
 description = "注入Python到微信，并实现Python发送消息和接收消息"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "keystone-engine",
     "pywin32",
-    "py_process_hooker>=0.2.1",
+    "py_process_hooker>=0.3.0",
     "requests",
     "uvicorn",
     "fastapi"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/kanadeblisst00/WeChat-PyRobot"
```

### Comparing `wechat_pyrobot-1.2.6/PKG-INFO` & `wechat_pyrobot-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wechat_pyrobot
-Version: 1.2.6
+Version: 1.3.0
 Summary: 注入Python到微信，并实现Python发送消息和接收消息
 Project-URL: Homepage, https://github.com/kanadeblisst00/WeChat-PyRobot
 Project-URL: Bug Tracker, https://github.com/kanadeblisst00/WeChat-PyRobot/issues
 Author-email: kanadeblisst <kanade@blisst.cn>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: fastapi
 Requires-Dist: keystone-engine
-Requires-Dist: py-process-hooker>=0.2.1
+Requires-Dist: py-process-hooker>=0.3.0
 Requires-Dist: pywin32
 Requires-Dist: requests
 Requires-Dist: uvicorn
 Description-Content-Type: text/markdown
 
 #### 教程目录
 
@@ -59,35 +59,38 @@
 64位:
 - `3.9.8.15`
 
 等这个系列教程结束再更新新版本，hook库和主动调用都已经说完了，也可以等群友提pr来更新。
 
 #### 群二维码
 
-![](http://cdn.ikanade.cn/Python_room_qrcode_20240229.jpg)
+![](http://cdn.ikanade.cn/Python_room_qrcode_20240407.jpg)
 
-如果二维码失效了，可以加我好友`kanadeblisst`，备注`进群`
+如果二维码失效了，可以加我好友`kanadeblisst`，备注`机器人群`
 
 ## 使用教程
 
 #### 当前支持功能
 
 - 发送文本消息
 - 发送AT消息
 - 发送图片消息
 - hook微信日志输出
 - hook接收消息
 - 消息防撤回
 - 下载聊天表情包
+- 获取好友列表
+- 获取群列表
+- 获取公众号列表
 
 #### 准备环境
 
 1. 安装支持的版本(`3.9.8.15`)微信
-2. 安装Python，版本大于等于3.8
-3. `pip install wechat_pyrobot==1.2.2`
+2. 安装Python，版本大于等于3.8 (最好就用3.8)，测试3.10+容易出bug
+3. `pip install wechat_pyrobot==1.3.0`
 
 如果国内源还没有同步最新版本，可以指定`-i https://pypi.org/simple/` 选项使用pip官方库
 
 #### 使用
 
 首先创建一个目录，例如`robot_code`，再创建一个`main.py`(名称随意)写入以下代码:
 ```python
@@ -175,18 +178,28 @@
 data = {
     "touser": "filehelper",
     "msg": "测试消息2"
 }
 
 requests.post(url, json=data)
 ```
+#### 联系人列表
+
+目前没有区分公众号、群和好友，有需求的可以自己加判断区分
+
+```python
+import requests
+
+url = "http://127.0.0.1:26666/contacts"
+print(requests.get(url).json())
+```
 
 #### 接收消息
 
-接收消息现在由插件控制，你可以编写自己的插件然后在`get_on_startup`的参数msg_plugins添加它
+接收消息现在由插件控制，你可以编写自己的插件然后在`get_on_startup`的参数msg_plugins添加它。插件执行目前是同步单线程，如果需要多线程的话，可以自己根据需要修改get_on_startup里的msg_thread_func函数。
 
 例如我想写一个将消息保存到文件的插件, `robot_code`下新建一个目录my_msg_plugin，下面新建一个文件`save_to_file.py`：
 
 ```python
 import os
 import json
 from wechat_pyrobot.plugin_class import MsgPluginTemplate
@@ -211,14 +224,15 @@
 ```python
 from py_process_hooker import inject_python_and_monitor_dir
 from wechat_pyrobot import get_on_startup
 from wechat_pyrobot.msg_plugins import PrintMsg, DownLoadEmotion
 from wechat_pyrobot.other_plugins import HttpApi
 from my_msg_plugin.save_to_file import SaveToFile
 
+
 if __name__ == "__main__":
     process_name = "WeChat.exe"
     open_console = True
     on_startup = get_on_startup(msg_plugins=[PrintMsg, DownLoadEmotion, SaveToFile], other_plugins=[HttpApi])
     
     inject_python_and_monitor_dir(process_name, __file__, open_console=open_console, on_startup=on_startup)
 ```
```

