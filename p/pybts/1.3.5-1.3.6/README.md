# Comparing `tmp/pybts-1.3.5.tar.gz` & `tmp/pybts-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.3.5.tar", max compression
+gzip compressed data, was "pybts-1.3.6.tar", max compression
```

## Comparing `pybts-1.3.5.tar` & `pybts-1.3.6.tar`

### file list

```diff
@@ -1,36 +1,41 @@
--rw-r--r--   0        0        0   157658 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-09 09:22:05.425870 pybts-1.3.5/README.md
--rw-r--r--   0        0        0      393 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/board/__init__.py
--rw-r--r--   0        0        0     2257 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/board/board.py
--rw-r--r--   0        0        0     9681 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/board/server.py
--rw-r--r--   0        0        0     4706 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/builder.py
--rw-r--r--   0        0        0      548 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/__init__.py
--rw-r--r--   0        0        0     8666 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/composite.py
--rw-r--r--   0        0        0     2118 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5661 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/parallel.py
--rw-r--r--   0        0        0      944 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/selector.py
--rw-r--r--   0        0        0     2541 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/sequence.py
--rw-r--r--   0        0        0      182 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/template.py
--rw-r--r--   0        0        0     3242 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/constants.py
--rw-r--r--   0        0        0     2299 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    16200 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1521 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/main.py
--rw-r--r--   0        0        0     6327 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/node.py
--rw-r--r--   0        0        0      115 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/rl/__init__.py
--rw-r--r--   0        0        0      460 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/rl/common.py
--rw-r--r--   0        0        0    13874 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/rl/on_policy.py
--rw-r--r--   0        0        0    16958 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/templates/index.html
--rw-r--r--   0        0        0  1966405 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/templates/static/index-BUWP2os5.js
--rw-r--r--   0        0        0   320362 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/templates/static/index-BXdrQGHp.css
--rw-r--r--   0        0        0     1448 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/tree.py
--rw-r--r--   0        0        0     9006 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-09 09:22:05.441870 pybts-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-09 16:43:21.380304 pybts-1.3.6/README.md
+-rw-r--r--   0        0        0      423 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/board/board.py
+-rw-r--r--   0        0        0     9589 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/board/server.py
+-rw-r--r--   0        0        0     5897 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/builder.py
+-rw-r--r--   0        0        0      548 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     8666 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2118 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5661 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      944 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2541 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/sequence.py
+-rw-r--r--   0        0        0      182 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/template.py
+-rw-r--r--   0        0        0     3242 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/constants.py
+-rw-r--r--   0        0        0     2482 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    16301 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1073 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/main.py
+-rw-r--r--   0        0        0     6679 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/node.py
+-rw-r--r--   0        0        0     1097 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/ref_file.py
+-rw-r--r--   0        0        0      166 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/rl/__init__.py
+-rw-r--r--   0        0        0      234 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/builder.py
+-rw-r--r--   0        0        0      460 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/common.py
+-rw-r--r--   0        0        0     2689 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/nodes.py
+-rw-r--r--   0        0        0    13874 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0      991 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/templates/index.html
+-rw-r--r--   0        0        0  1966405 2024-04-09 16:43:21.396304 pybts-1.3.6/pybts/templates/static/index-BUWP2os5.js
+-rw-r--r--   0        0        0   320362 2024-04-09 16:43:21.400304 pybts-1.3.6/pybts/templates/static/index-BXdrQGHp.css
+-rw-r--r--   0        0        0     1553 2024-04-09 16:43:21.400304 pybts-1.3.6/pybts/tree.py
+-rw-r--r--   0        0        0     9006 2024-04-09 16:43:21.400304 pybts-1.3.6/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-09 16:43:21.400304 pybts-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.3.6/PKG-INFO
```

### Comparing `pybts-1.3.5/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.3.6/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/README.assets/image-20240329031220580.png` & `pybts-1.3.6/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/README.assets/image-20240329031233459.png` & `pybts-1.3.6/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/README.assets/image-20240401211552611.png` & `pybts-1.3.6/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/README.assets/image-20240401211609525.png` & `pybts-1.3.6/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/README.md` & `pybts-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/board/board.py` & `pybts-1.3.6/pybts/board/board.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,7 +58,8 @@
         if os.path.exists(self.history_dir):
             for filename in os.listdir(self.history_dir):
                 if filename.endswith('.json'):
                     filepath = os.path.join(self.history_dir, filename)
                     with open(filepath, 'r', encoding='utf') as f:
                         json_data = utility.json_loads(f.read())
                         yield json_data
+
```

### Comparing `pybts-1.3.5/pybts/board/server.py` & `pybts-1.3.6/pybts/board/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,14 @@
                 if os.path.exists(os.path.join(TEMPLATES_DIR, target_path)):
                     return send_from_directory(TEMPLATES_DIR, target_path)
         return send_from_directory(TEMPLATES_DIR, 'index.html')
 
     def send_static(self, path):
         return send_from_directory(STATIC_DIR, path)
 
-    def send_template(self, path):
-        return send_from_directory(TEMPLATES_DIR, path)
-
     def get_projects(self):
         # 获取log_dir里面的所有的文件夹
         projects = []
         if not os.path.exists(self.log_dir):
             return []
 
         for dirpath, dirnames, filenames in os.walk(self.log_dir):
```

### Comparing `pybts-1.3.5/pybts/builder.py` & `pybts-1.3.6/pybts/builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from __future__ import annotations
 
 import json
+import os.path
 from typing import Callable
 import xml.etree.ElementTree as ET
 import copy
-from pybts.constants import *
 from pybts.node import *
 from pybts.composites import *
 from pybts.decorators import *
 import uuid
 from pybts.utility import camel_case_to_snake_case
+from pybts.ref_file import RefFile
 
 
 class Builder:
-    def __init__(self, **kwargs):
+    def __init__(self, folders: str | list = '', global_attrs: dict = None):
         self.repo = { }  # 注册节点的仓库
         self.repo_desc = { }  # 仓库的描述
         self.register_default()
-        self.kwargs = kwargs.copy()  # 全局参数
+        self.global_attrs = global_attrs or { }  # 全局参数，会在build时传递给每一个节点
+        if isinstance(folders, str):
+            self.folders = [folders]
+        else:
+            self.folders = folders
 
     def register(self, name: str | list[str], creator: Callable, desc: str = ''):
         if isinstance(name, str):
             name_list = name.split('|')
             for _name in name_list:
                 self.repo[_name] = creator
                 if desc != '':
@@ -36,17 +41,31 @@
         """
         for node in nodes:
             self.register(node.__name__, node, desc=node.__doc__ or node.__name__)
             self.register(camel_case_to_snake_case(node.__name__), node)
             module_name = f'{node.__module__}.{node.__name__}'
             self.register(module_name, node)
 
+    def read_text_from_file(self, filepath: str) -> str:
+        # 从folder中找文件
+        if os.path.exists(filepath) and os.path.isfile(filepath):
+            with open(filepath, 'r', encoding='utf-8') as file:
+                return file.read()
+
+        # 遍历文件夹列表里所有的文件，找到和文件名相同的文件并返回内容
+        for folder in self.folders:
+            folder_filepath = os.path.join(folder, filepath)
+            if os.path.exists(folder_filepath) and os.path.isfile(folder_filepath):
+                with open(folder_filepath, 'r', encoding='utf-8') as file:
+                    return file.read()
+
+        raise Exception(f'Cannot find file: {filepath}')
+
     def build_from_file(self, filepath: str):
-        with open(filepath, 'r', encoding='utf-8') as f:
-            text = f.read()
+        text = self.read_text_from_file(filepath=filepath)
         if filepath.endswith('.json'):
             return self.build_from_json(json_data=text, ignore_children=False)
         elif filepath.endswith('.xml'):
             return self.build_from_xml(xml_data=text, ignore_children=False)
         else:
             raise Exception('Unsupported file')
 
@@ -72,15 +91,15 @@
                         json_data['children']]
         data = copy.copy(json_data['data'])
 
         # if 'name' not in data:
         #     data['name'] = json_data['tag']
 
         attrs = {
-            **self.kwargs,
+            **self.global_attrs,
             **data,
         }
         try:
             node = creator(**attrs, children=children)
         except Exception as e:
             print(creator, e)
             raise e
@@ -127,12 +146,21 @@
                 RunningIsSuccess,
                 FailureIsSuccess,
                 FailureIsRunning,
                 SuccessIsFailure,
                 SuccessIsRunning,
         )
 
+        self.register_node(RefFile)
+
+        # 且或非
+        self.register('And', Sequence)
+        self.register('Or', Selector)
+        self.register('Not', Inverter)
+        self.register('Root', Parallel)  # 可以作为根节点
+        # 强化学习
+
 
 if __name__ == '__main__':
     builder = Builder()
     print(builder.repo_desc)
     # print(Node.__doc__)
```

### Comparing `pybts-1.3.5/pybts/composites/__init__.py` & `pybts-1.3.6/pybts/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/composites/composite.py` & `pybts-1.3.6/pybts/composites/composite.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/composites/condition_branch.py` & `pybts-1.3.6/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/composites/parallel.py` & `pybts-1.3.6/pybts/composites/parallel.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/composites/ppa.py` & `pybts-1.3.6/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/composites/selector.py` & `pybts-1.3.6/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/composites/sequence.py` & `pybts-1.3.6/pybts/composites/sequence.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/constants.py` & `pybts-1.3.6/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/converter.py` & `pybts-1.3.6/pybts/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,42 +6,46 @@
 class Converter:
 
     def __init__(self, node):
         self.node = node
 
     def bool(self, value: typing.Any):
         if isinstance(value, str):
-            return value.lower() == 'true'
+            if value.lower() == 'true':
+                return True
+            elif value.lower() == 'false':
+                return False
+            return bool(eval(self.render(value)))
         return bool(value)
 
     def float(self, value: typing.Any):
         if isinstance(value, str):
-            return float(value)
+            return eval(self.render(value))
         else:
             return float(value)
 
     def int(self, value: typing.Any):
         if isinstance(value, str):
-            return int(value)
+            return int(eval(self.render(value)))
         else:
-            return float(value)
+            return int(value)
 
-    def render(self, value: typing.Any, context: dict = None) -> str:
+    def render(self, value: str, context: dict = None) -> str:
         ctx = { }
         if self.node.context is not None:
             ctx.update(self.node.context)
         if self.node.attrs is not None:
             ctx.update(self.node.attrs)
         if context is not None:
             ctx.update(context)
         return jinja2.Template(value).render(ctx)
 
     def list(self, value: typing.Any) -> typing.List[typing.Any]:
         if isinstance(value, str):
-            return json.loads(value)
+            return eval(self.render(value))
         elif isinstance(value, list):
             return value
         elif isinstance(value, tuple):
             return list(value)
         else:
             try:
                 import numpy
@@ -49,15 +53,15 @@
                     return value.tolist()
             except ImportError:
                 pass
             raise Exception(f'array error {value}')
 
     def dict(self, value: typing.Any) -> typing.Dict[str, typing.Any]:
         if isinstance(value, str):
-            return json.loads(value)
+            return eval(self.render(value))
         elif isinstance(value, dict):
             return value
         else:
             raise Exception(f'dict error {value}')
 
     def json_loads(self, value: typing.Any):
         if isinstance(value, str):
```

### Comparing `pybts-1.3.5/pybts/decorators/nodes.py` & `pybts-1.3.6/pybts/decorators/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     装饰节点
     只有一个子节点
     """
 
     def __init__(self, children: list[py_trees.behaviour.Behaviour], **kwargs):
         # Checks
         # Initialise
-        super().__init__(children=children,**kwargs)
+        super().__init__(children=children, **kwargs)
         # Give a convenient alias
-        self.decorated = self.children[0]
+        if len(self.children) > 0:
+            self.decorated = self.children[0]
+        else:
+            self.decorated: Node | None = None
 
     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
         """
         Manage the decorated child through the tick.
 
         Yields:
             a reference to itself or one of its children
```

### Comparing `pybts-1.3.5/pybts/main.py` & `pybts-1.3.6/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/node.py` & `pybts-1.3.6/pybts/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.debug_info = {
             'tick_count'      : 0,
             'update_count'    : 0,
             'reset_count'     : 0,
             'terminate_count' : 0,
             'initialise_count': 0
         }
-        self.attrs: typing.Dict[str, typing.AnyStr] = kwargs # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
+        self.attrs: typing.Dict[str, typing.AnyStr] = kwargs  # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
         self.context: typing.Optional[dict] = None  # 共享的字典，在tree.setup的时候提供
         if children is not None:
             self.children = children
             for child in children:
                 child.parent = self
 
     def reset(self):
@@ -181,15 +181,25 @@
         }
 
 
 class Condition:
     """
     条件节点，只能多继承使用
     """
-    pass
+
+    def condition_score(self) -> float:
+        """条件达成分数，后面可以作为奖励函数设计使用"""
+        if isinstance(self, Node):
+            if self.status == Status.SUCCESS:
+                return 1
+            elif self.status == Status.RUNNING:
+                return 0.5
+            else:
+                return 0
+        return 0
 
 
 class Success(Node, Condition):
     """
     成功节点
     """
```

### Comparing `pybts-1.3.5/pybts/rl/on_policy.py` & `pybts-1.3.6/pybts/rl/on_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/templates/favicon.ico` & `pybts-1.3.6/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/templates/static/index-BUWP2os5.js` & `pybts-1.3.6/pybts/templates/static/index-BUWP2os5.js`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/templates/static/index-BXdrQGHp.css` & `pybts-1.3.6/pybts/templates/static/index-BXdrQGHp.css`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pybts/tree.py` & `pybts-1.3.6/pybts/tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 
 import py_trees
 from py_trees import common, visitors
 from pybts.node import Node
+from pybts.builder import Builder
 
 
 class Tree(py_trees.trees.BehaviourTree):
     def __init__(self, root: py_trees.behaviour.Behaviour, name: str = '', context: dict = None):
         super().__init__(root=root)
         self.name = name or root.name
         self.reset_handlers: typing.List[
@@ -27,19 +28,20 @@
     def round(self, value):
         self.context['round'] = value
 
     def setup(
             self,
             timeout: typing.Union[float, common.Duration] = common.Duration.INFINITE,
             visitor: typing.Optional[visitors.VisitorBase] = None,
+            builder: typing.Optional[Builder] = None,
             **kwargs: any,
     ) -> None:
         for node in self.root.iterate():
             node.context = self.context
-        super().setup(timeout=timeout, visitor=visitor, **kwargs)
+        super().setup(timeout=timeout, visitor=visitor, builder=builder, **kwargs)
 
     def reset(self):
         self.count = 0
         self.round += 1
         for node in self.root.iterate():
             if isinstance(node, Node):
                 node.reset()
```

### Comparing `pybts-1.3.5/pybts/utility.py` & `pybts-1.3.6/pybts/utility.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.5/pyproject.toml` & `pybts-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.3.5"
+version = "1.3.6"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.3.5/PKG-INFO` & `pybts-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.3.5
+Version: 1.3.6
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

