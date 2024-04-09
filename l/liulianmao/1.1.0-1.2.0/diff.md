# Comparing `tmp/liulianmao-1.1.0.tar.gz` & `tmp/liulianmao-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liulianmao-1.1.0.tar", max compression
+gzip compressed data, was "liulianmao-1.2.0.tar", max compression
```

## Comparing `liulianmao-1.1.0.tar` & `liulianmao-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.1.0/LICENSE
--rw-r--r--   0        0        0      781 2024-04-05 06:13:28.357557 liulianmao-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3346 2024-04-04 10:15:27.974883 liulianmao-1.1.0/README.md
--rw-r--r--   0        0        0       84 2024-04-03 13:08:57.859474 liulianmao-1.1.0/src/liulianmao/__init__.py
--rw-r--r--   0        0        0     3606 2024-04-05 06:11:53.754203 liulianmao-1.1.0/src/liulianmao/__main__.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:28.446436 liulianmao-1.1.0/src/liulianmao/client/__init__.py
--rw-r--r--   0        0        0     5032 2024-04-03 13:07:44.762569 liulianmao-1.1.0/src/liulianmao/client/core.py
--rw-r--r--   0        0        0      583 2024-04-03 13:08:46.866069 liulianmao-1.1.0/src/liulianmao/client/langchain.py
--rw-r--r--   0        0        0      117 2024-04-01 16:47:06.824622 liulianmao-1.1.0/src/liulianmao/module/__init__.py
--rw-r--r--   0        0        0     1751 2024-04-02 06:21:17.164107 liulianmao-1.1.0/src/liulianmao/module/authentication.py
--rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.1.0/src/liulianmao/module/const.py
--rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.1.0/src/liulianmao/module/log.py
--rw-r--r--   0        0        0      542 2024-03-20 13:24:32.988008 liulianmao-1.1.0/src/liulianmao/module/model.py
--rw-r--r--   0        0        0     1359 2024-04-01 11:46:03.350081 liulianmao-1.1.0/src/liulianmao/module/storage.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.1.0/src/liulianmao/tool/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.1.0/src/liulianmao/tool/ls.py
--rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 liulianmao-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.2.0/LICENSE
+-rw-r--r--   0        0        0      781 2024-04-09 02:24:00.217950 liulianmao-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3830 2024-04-05 10:51:08.732993 liulianmao-1.2.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-03 13:08:57.859474 liulianmao-1.2.0/src/liulianmao/__init__.py
+-rw-r--r--   0        0        0     4200 2024-04-09 02:48:15.775349 liulianmao-1.2.0/src/liulianmao/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:28.446436 liulianmao-1.2.0/src/liulianmao/client/__init__.py
+-rw-r--r--   0        0        0     6925 2024-04-06 12:29:52.522613 liulianmao-1.2.0/src/liulianmao/client/core.py
+-rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.2.0/src/liulianmao/client/langchain.py
+-rw-r--r--   0        0        0      117 2024-04-01 16:47:06.824622 liulianmao-1.2.0/src/liulianmao/module/__init__.py
+-rw-r--r--   0        0        0     2803 2024-04-08 07:16:31.906417 liulianmao-1.2.0/src/liulianmao/module/authentication.py
+-rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.2.0/src/liulianmao/module/const.py
+-rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.2.0/src/liulianmao/module/log.py
+-rw-r--r--   0        0        0     2120 2024-04-07 04:12:04.940254 liulianmao-1.2.0/src/liulianmao/module/model.py
+-rw-r--r--   0        0        0     1409 2024-04-05 08:42:44.890771 liulianmao-1.2.0/src/liulianmao/module/storage.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.2.0/src/liulianmao/tool/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.2.0/src/liulianmao/tool/ls.py
+-rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 liulianmao-1.2.0/PKG-INFO
```

### Comparing `liulianmao-1.1.0/LICENSE` & `liulianmao-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liulianmao-1.1.0/pyproject.toml` & `liulianmao-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liulianmao"
-version = "1.1.0"
+version = "1.2.0"
 description = "A LLM client for use from the command line or IDE."
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 repository = "https://github.com/LaoshuBaby/liulianmao"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `liulianmao-1.1.0/README.md` & `liulianmao-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 pip install langchain langchain_openai
 ```
 
 在系统环境变量中配置`OPENAI_API_KEY`的值为你所使用的API，`OPENAI_BASE_URL`的值为你使用的服务商的endpoint。 （如果您配置过langchain，那就不需要再次配置了！）
 
 如果您不懂什么是环境变量，也可以在同目录下放置同名文件，亦可在代码中硬编码，但鼠宝宝不推荐这么做。
 
+## 示例
+
+- `python your_script.py` 将使用默认的recipe（即["init", "chat"]）。
+- `python your_script.py --recipe init other_operation` 将使用自定义的recipe（即["init", "other_operation"]）。
+- `python your_script.py --question` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
+- `python your_script.py --question --recipe init other_operation` 将打开并打印`question.txt`文件的内容，并使用自定义的recipe。
+
 ## 参考文档
 
 虽然我觉得正常用户用不到这东西，给自己看方便debug的
 
 * https://platform.openai.com/docs/api-reference/audio/createSpeech
 * https://platform.openai.com/docs/guides/text-to-speech
```

### Comparing `liulianmao-1.1.0/src/liulianmao/__main__.py` & `liulianmao-1.2.0/src/liulianmao/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,51 +19,67 @@
     else:
         # Running in a normal Python environment
         current_dir = os.path.dirname(os.path.abspath(__file__))
         bundled_dir = current_dir
 
     parent_dir = os.path.dirname(bundled_dir)
 
-    # print(__file__)
-    # print(bundled_dir)
-    # print(parent_dir)
-    # print(os.getcwd())
-    # print(os.listdir(bundled_dir))
+    try:
+        from module.log import logger
+
+        logger.debug(f'[ENV] "__file__" = {__file__}')
+        logger.debug(f'[ENV] "bundled_dir" = {bundled_dir}')
+        logger.debug(f'[ENV] "parent_dir" = {parent_dir}')
+        logger.debug(f'[ENV] "os.getcwd()" = {os.getcwd()}')
+        logger.debug(
+            f'[ENV] "os.listdir(bundled_dir)" = {os.listdir(bundled_dir)}'
+        )
+    except Exception as e:
+        print(
+            __file__,
+            "\n",
+            bundled_dir,
+            "\n",
+            parent_dir,
+            "\n",
+            os.getcwd(),
+            "\n",
+            os.listdir(bundled_dir),
+        )
 
     if parent_dir not in sys.path:
         sys.path.append(parent_dir)
 
 
-def main(recipe: List[str], question: bool):
+def main(recipe: List[str], actions: List[str]):
     """Execute the operations specified in the recipe list.
 
-    如果question为真，则打开并打印'question.txt'文件的内容。
-    根据提供的recipe列表执行一系列操作。
+    根据提供的recipe列表和actions列表执行一系列操作。
 
     Args:
-        recipe: A list of strings representing the operations to be processed.
-            默认为["init", "chat"]。
-        question: A boolean flag that, when True, triggers the reading and printing
-            of the 'question.txt' file's content.
-
-    示例：
-    - `python your_script.py` 将使用默认的recipe（即["init", "chat"]）。
-    - `python your_script.py --recipe init other_operation` 将使用自定义的recipe（即["init", "other_operation"]）。
-    - `python your_script.py --question` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
-    - `python your_script.py --question --recipe init other_operation` 将打开并打印`question.txt`文件的内容，并使用自定义的recipe。
+        recipe: A list of strings representing the operations to be processed.默认为["init", "chat"]。
+        actions: A list of strings representing additional actions to be taken.
     """
-
-    if question:
+    if "question" in actions:
         from module.const import PROJECT_FOLDER, get_user_folder
 
         question_file_path = os.path.join(
             str(get_user_folder()), PROJECT_FOLDER, "terminal", "question.txt"
         )
         os.startfile(question_file_path)
-        exit(0)
+        sys.exit(0)
+
+    if "config" in actions:
+        from module.const import PROJECT_FOLDER, get_user_folder
+
+        config_file_path = os.path.join(
+            str(get_user_folder()), PROJECT_FOLDER, "assets", "config.json"
+        )
+        os.startfile(config_file_path)
+        sys.exit(0)
 
     import importlib.util
 
     FEATURE = {"core": True, "langchain": False}
 
     spec = importlib.util.find_spec(".core", package="client")
     core = importlib.util.module_from_spec(spec)
@@ -72,35 +88,55 @@
     if FEATURE["langchain"]:
         # spec = importlib.util.find_spec('.langchain', package='client')
         # langchain = importlib.util.module_from_spec(spec)
         # spec.loader.exec_module(langchain)
         from client.langchain import main as langchain
 
     operations = {
-        "init": core.init,
         "chat": core.chat,
+        "talk": core.talk,
+        "models": core.models,
     }
 
     for operation_name in recipe:
         operation = operations.get(operation_name)
         if operation:
             operation()
         else:
             print(f"Operation {operation_name} is not defined.")
 
 
 if __name__ == "__main__":
     init_env()
-    default_recipe = ["init", "chat"]
+    default_recipe = ["chat"]
     parser = argparse.ArgumentParser(description="Process some operations.")
     parser.add_argument(
-        "--question", action="store_true", help="Read the question.txt file"
+        "-q",
+        "-question",
+        "--question",
+        action="store_true",
+        help="Read the question.txt file",
+    )
+    parser.add_argument(
+        "-c",
+        "-config",
+        "--config",
+        action="store_true",
+        help="Read the config.txt file",
     )
     parser.add_argument(
+        "-r",
+        "-recipe",
         "--recipe",
         nargs="*",
         default=default_recipe,
         help="List of operations to process",
     )
     args = parser.parse_args()
-    print("AAA")
-    main(recipe=args.recipe, question=args.question)
+
+    actions = []
+    if args.question:
+        actions.append("question")
+    if args.config:
+        actions.append("config")
+
+    main(recipe=args.recipe, actions=actions)
```

### Comparing `liulianmao-1.1.0/src/liulianmao/client/core.py` & `liulianmao-1.2.0/src/liulianmao/client/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,77 @@
 import json
 import os
 import sys
+from typing import List
 
 import requests
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(current_dir, ".."))
 
 from module.authentication import API_KEY, API_URL
 from module.log import logger
 from module.model import select_model
 from module.storage import PROJECT_FOLDER, get_user_folder, init
 
+conversation = []
 
 def load_conf():
     config_file_path = os.path.join(
         get_user_folder(), PROJECT_FOLDER, "assets", "config.json"
     )
     with open(config_file_path, "r") as file:
         config = json.load(file)
 
-    system_role = config["system_message"]["content"]
-    temperature = float(config["settings"]["temperature"])
-    return system_role, temperature
+    logger.trace("[Config]\n" + f"{config}")
+    return config
 
 
-conversation = []
+def models():
+    headers = {
+        "Authorization": f"Bearer {API_KEY}",
+        "Content-Type": "application/json",
+    }
+    logger.trace("[Headers]\n" + f"{headers}")
+
+    response = requests.get(
+        API_URL + "/v1/models", headers=headers
+    )
+
+    def extract_ids(data):
+        collected_ids = []
+
+        for item in data:
+            for key, value in item.items():
+                if key == 'id':
+                    if value[0:3].lower() == "gpt":
+                        collected_ids.append(value)
 
+        return collected_ids
 
-def tts(msg):
+    if response.status_code == 200:
+        logger.trace("[Debug] response.status_code == 200")
+        # judge mime
+        try:
+            logger.trace("[Response]\n" + str(response.json()))
+        except Exception as e:
+            logger.trace(e)
+            logger.critical("RESPONSE NOT JSON")
+        extracted_ids=extract_ids(response.json()["data"])
+        logger.debug(extracted_ids)
+        return extracted_ids
+    else:
+        logger.trace("[Debug] response.status_code != 200")
+        logger.error(
+            f"Error: {response.status_code} {response.content.decode('utf-8')}"
+        )
+        return {}
+
+
+def speech(msg):
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
     data = {"model": "tts-1", "input": msg, "voice": "alloy"}
     response = requests.post(
@@ -50,25 +89,28 @@
         logger.error(
             "生成语音失败。状态码：",
             response.status_code,
             "\n",
             response.content.decode("utf-8"),
         )
 
+def completion(question,available_models:List[str]=[]):
+    config = load_conf()
+    model_type = config["model_type"]
+    system_content = config["system_message"]["content"]
+    temperature = float(config["settings"]["temperature"])
 
-def requester(question, model_type="gpt-4-turbo-preview"):
-    system_content, temperature = load_conf()
 
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
     payload = {
-        "model": select_model(model_type),
+        "model": select_model(model_type,available_models,direct_debug=True),
         "messages": (
             [{"role": "system", "content": system_content}]
             + conversation
             + [{"role": "user", "content": question}]
         ),
         "temperature": temperature,
         "max_tokens": 2048,
@@ -94,50 +136,64 @@
         logger.trace("[Question]\n" + f"{question}")
 
     response = requests.post(
         API_URL + "/v1/chat/completions", headers=headers, json=payload
     )
 
     if response.status_code == 200:
-        conversation.append({"role": "user", "content": question})
-        conversation.append(
-            {
-                "role": "system",
-                "content": response.json()["choices"][0]["message"]["content"],
-            }
-        )
+        logger.trace("[Debug] response.status_code == 200")
+        # judge mime
+        try:
+            logger.trace("[Response]\n" + str(response.json()))
+        except Exception as e:
+            logger.trace(e)
+            logger.critical("RESPONSE NOT JSON")
+        # judge schema
+        try:
+            conversation.append({"role": "user", "content": question})
+            conversation.append(
+                {
+                    "role": "system",
+                    "content": response.json()["choices"][0]["message"]["content"],
+                }
+            )
+        except Exception as e:
+            logger.trace(e)
+            logger.critical("WRONG RESPONSE SCHEMA")
         logger.trace("[History]\n" + str(conversation))
-        logger.trace("[Response]\n" + str(response.json()))
         return response.json()
     else:
+        logger.trace("[Debug] response.status_code != 200")
         logger.error(
             f"Error: {response.status_code} {response.content.decode('utf-8')}"
         )
         return {}
 
 
-def ask(msg: str):
-    response = requester(msg)
+def ask(msg: str,available_models:List[str]):
+    response = completion(msg,available_models)
     content = response["choices"][0]["message"]["content"]
     logger.success("[Answer]\n" + content)
     return content
 
 
 def chat():
+    available_models=models()
+
     with open(
         os.path.join(
             get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
         ),
         "r",
         encoding="utf-8",
     ) as file:
         msg = file.read()
 
     flag_continue = True
-    response = ask(msg)
+    response = ask(msg,available_models)
 
     if not flag_continue:
         with open(
             os.path.join(
                 get_user_folder(), PROJECT_FOLDER, "terminal", "answer.txt"
             ),
             "w",
@@ -153,24 +209,24 @@
             time.sleep(0.05)
             logger.info("[Interaction] 请输入追问")
             append_question = input()
             append_question_judge = append_question.replace("\n", "").replace(
                 " ", ""
             )
             if append_question_judge != "END" and append_question_judge != "":
-                response = ask(append_question)
+                response = ask(append_question,available_models)
             else:
                 flag_end = True
                 break
 
 
 def talk():
     with open("terminal/question.txt", "r", encoding="utf-8") as file:
         msg = file.read()
-    tts(msg)
+    speech(msg)
 
 
 def main():
     logger.critical("THIS PROGRAM NOT INTENT TO RUN SUBMODULE".upper())
     exit(0)
```

### Comparing `liulianmao-1.1.0/src/liulianmao/client/langchain.py` & `liulianmao-1.2.0/src/liulianmao/client/langchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import sys
+
 from langchain_openai import ChatOpenAI
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(current_dir, ".."))
 
 from module.authentication import API_KEY, API_URL
 from module.log import logger
```

### Comparing `liulianmao-1.1.0/src/liulianmao/module/log.py` & `liulianmao-1.2.0/src/liulianmao/module/log.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.1.0/src/liulianmao/module/storage.py` & `liulianmao-1.2.0/src/liulianmao/module/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def init():
     # 假设file_list中的JSON字符串需要格式化
     file_list = [
         (["terminal", "question.txt"], "Hello World!"),
         (["terminal", "answer.txt"], "Hello! How can I assist you today?"),
         # 使用json.dumps()格式化JSON字符串，并指定缩进为4个空格
         (["assets", "config.json"], json.dumps({
+            "model_type": "gpt-4-turbo-preview",
             "system_message": {"content": "You are a helpful assistant."},
             "settings": {"temperature": 0.5}
         }, indent=4))
     ]
     folder_list = ["logs", "audios", "terminal", "assets"]
 
     for folder in folder_list:
```

### Comparing `liulianmao-1.1.0/src/liulianmao/tool/ls.py` & `liulianmao-1.2.0/src/liulianmao/tool/ls.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.1.0/PKG-INFO` & `liulianmao-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liulianmao
-Version: 1.1.0
+Version: 1.2.0
 Summary: A LLM client for use from the command line or IDE.
 Home-page: https://github.com/LaoshuBaby/liulianmao
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -56,14 +56,21 @@
 pip install langchain langchain_openai
 ```
 
 在系统环境变量中配置`OPENAI_API_KEY`的值为你所使用的API，`OPENAI_BASE_URL`的值为你使用的服务商的endpoint。 （如果您配置过langchain，那就不需要再次配置了！）
 
 如果您不懂什么是环境变量，也可以在同目录下放置同名文件，亦可在代码中硬编码，但鼠宝宝不推荐这么做。
 
+## 示例
+
+- `python your_script.py` 将使用默认的recipe（即["init", "chat"]）。
+- `python your_script.py --recipe init other_operation` 将使用自定义的recipe（即["init", "other_operation"]）。
+- `python your_script.py --question` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
+- `python your_script.py --question --recipe init other_operation` 将打开并打印`question.txt`文件的内容，并使用自定义的recipe。
+
 ## 参考文档
 
 虽然我觉得正常用户用不到这东西，给自己看方便debug的
 
 * https://platform.openai.com/docs/api-reference/audio/createSpeech
 * https://platform.openai.com/docs/guides/text-to-speech
```

