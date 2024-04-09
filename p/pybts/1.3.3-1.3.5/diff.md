# Comparing `tmp/pybts-1.3.3.tar.gz` & `tmp/pybts-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.3.3.tar", max compression
+gzip compressed data, was "pybts-1.3.5.tar", max compression
```

## Comparing `pybts-1.3.3.tar` & `pybts-1.3.5.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0   157658 2024-04-08 02:36:46.847127 pybts-1.3.3/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-08 02:36:46.847127 pybts-1.3.3/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-08 02:36:46.851127 pybts-1.3.3/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-08 02:36:46.851127 pybts-1.3.3/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-08 02:36:46.851127 pybts-1.3.3/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5877 2024-04-08 02:36:46.851127 pybts-1.3.3/README.md
--rw-r--r--   0        0        0      393 2024-04-08 02:36:46.851127 pybts-1.3.3/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/board/__init__.py
--rw-r--r--   0        0        0     2257 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/board/board.py
--rw-r--r--   0        0        0     9681 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/board/server.py
--rw-r--r--   0        0        0     4138 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/builder.py
--rw-r--r--   0        0        0      473 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/__init__.py
--rw-r--r--   0        0        0     8760 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/composite.py
--rw-r--r--   0        0        0     2246 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5862 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/parallel.py
--rw-r--r--   0        0        0     2405 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/selector.py
--rw-r--r--   0        0        0     2606 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/sequence.py
--rw-r--r--   0        0        0     3242 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/constants.py
--rw-r--r--   0        0        0      121 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    16991 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1521 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/main.py
--rw-r--r--   0        0        0     5668 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/node.py
--rw-r--r--   0        0        0      115 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/rl/__init__.py
--rw-r--r--   0        0        0      459 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/rl/common.py
--rw-r--r--   0        0        0    13320 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/rl/on_policy.py
--rw-r--r--   0        0        0    16958 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/templates/index.html
--rw-r--r--   0        0        0  1966405 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/templates/static/index-BUWP2os5.js
--rw-r--r--   0        0        0   320362 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/templates/static/index-BXdrQGHp.css
--rw-r--r--   0        0        0      800 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/tree.py
--rw-r--r--   0        0        0     8814 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-08 02:36:46.867127 pybts-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 pybts-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-09 09:22:05.425870 pybts-1.3.5/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-09 09:22:05.425870 pybts-1.3.5/README.md
+-rw-r--r--   0        0        0      393 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2257 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/board/board.py
+-rw-r--r--   0        0        0     9681 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/board/server.py
+-rw-r--r--   0        0        0     4706 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/builder.py
+-rw-r--r--   0        0        0      548 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     8666 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2118 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5661 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      944 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2541 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/sequence.py
+-rw-r--r--   0        0        0      182 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/composites/template.py
+-rw-r--r--   0        0        0     3242 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/constants.py
+-rw-r--r--   0        0        0     2299 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    16200 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1521 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/main.py
+-rw-r--r--   0        0        0     6327 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/node.py
+-rw-r--r--   0        0        0      115 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/rl/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/rl/common.py
+-rw-r--r--   0        0        0    13874 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0    16958 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-09 09:22:05.429870 pybts-1.3.5/pybts/templates/index.html
+-rw-r--r--   0        0        0  1966405 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/templates/static/index-BUWP2os5.js
+-rw-r--r--   0        0        0   320362 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/templates/static/index-BXdrQGHp.css
+-rw-r--r--   0        0        0     1448 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/tree.py
+-rw-r--r--   0        0        0     9006 2024-04-09 09:22:05.441870 pybts-1.3.5/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-09 09:22:05.441870 pybts-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.3.5/PKG-INFO
```

### Comparing `pybts-1.3.3/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.3.5/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/README.assets/image-20240329031220580.png` & `pybts-1.3.5/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/README.assets/image-20240329031233459.png` & `pybts-1.3.5/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/README.assets/image-20240401211552611.png` & `pybts-1.3.5/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/README.assets/image-20240401211609525.png` & `pybts-1.3.5/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/README.md` & `pybts-1.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,28 +54,31 @@
 
 ```python
 from pybts import Tree, board, builder
 from pybts.node import Action
 from py_trees import common
 import time
 
+
 # Define custom behavior node
 class Person(Action):
   def __init__(self, name: str, age: int):
     super().__init__(name=name)
     self.age = age
 
   def update(self) -> common.Status:
     self.age += 1
     return common.Status.SUCCESS
 
 
 # Build the behavior tree
 builder = builder.Builder()
-builder.register('Person', Person.creator)
+builder.register('Person', Person)
+# or
+builder.register_node(Person)  # will register tag 'Person' and 'person'(snake case)
 root = builder.build_from_file('demos/demo_bt.xml')
 tree = Tree(root=root, name='Person')
 
 # Initialize board for tracking
 bt_board = board.Board(tree=tree, log_dir='logs')
 
 bt_board.clear()
```

### Comparing `pybts-1.3.3/pybts/board/board.py` & `pybts-1.3.5/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/board/server.py` & `pybts-1.3.5/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/builder.py` & `pybts-1.3.5/pybts/builder.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,103 +5,124 @@
 import xml.etree.ElementTree as ET
 import copy
 from pybts.constants import *
 from pybts.node import *
 from pybts.composites import *
 from pybts.decorators import *
 import uuid
+from pybts.utility import camel_case_to_snake_case
 
 
 class Builder:
-    def __init__(self):
-        self.repo = { }
+    def __init__(self, **kwargs):
+        self.repo = { }  # 注册节点的仓库
         self.repo_desc = { }  # 仓库的描述
-        self.repo_node = { }  # 注册的bt节点
         self.register_default()
+        self.kwargs = kwargs.copy()  # 全局参数
 
-    def register(self, name: str | list[str], creator: Callable[[dict, [Node]], Node], desc: str = ''):
+    def register(self, name: str | list[str], creator: Callable, desc: str = ''):
         if isinstance(name, str):
             name_list = name.split('|')
             for _name in name_list:
                 self.repo[_name] = creator
                 if desc != '':
                     self.repo_desc[_name] = desc.strip()
         else:
             for _name in name:
                 self.register(_name, creator, desc=desc)
 
-    def register_bt(self, *nodes: Node.__class__):
+    def register_node(self, *nodes: Node.__class__):
+        """
+        注册节点，注意节点的__init__传递的参数全部都是str类型，在内部要自己处理一下
+        """
         for node in nodes:
-            self.repo_node[node.__name__] = node
-            self.register(node.__name__, node.creator, desc=node.__doc__ or node.__name__)
+            self.register(node.__name__, node, desc=node.__doc__ or node.__name__)
+            self.register(camel_case_to_snake_case(node.__name__), node)
             module_name = f'{node.__module__}.{node.__name__}'
-            self.register(module_name, node.creator)
+            self.register(module_name, node)
 
     def build_from_file(self, filepath: str):
-        with open(filepath, 'r') as f:
+        with open(filepath, 'r', encoding='utf-8') as f:
             text = f.read()
         if filepath.endswith('.json'):
             return self.build_from_json(json_data=text, ignore_children=False)
         elif filepath.endswith('.xml'):
             return self.build_from_xml(xml_data=text, ignore_children=False)
         else:
             raise Exception('Unsupported file')
 
     def build_from_xml(self, xml_data: ET.Element | str, ignore_children: bool = False) -> Node:
         if isinstance(xml_data, str):
             xml_data = ET.fromstring(xml_data)
         from pybts.utility import xml_to_json
-        return self.build_from_json(json_data=xml_to_json(xml_node=xml_data, ignore_children=ignore_children),
-                                    ignore_children=ignore_children)
+        return self.build_from_json(
+                json_data=xml_to_json(
+                        xml_node=xml_data, ignore_children=ignore_children),
+                ignore_children=ignore_children)
 
     def build_from_json(self, json_data: dict | str, ignore_children: bool = False) -> Node:
 
         if isinstance(json_data, str):
             json_data = json.loads(json_data, encoding='utf-8')
         tag = json_data['tag']
         assert tag in self.repo, f'Unsupported tag {tag}'
         creator = self.repo[tag]
         children = []
         if not ignore_children:
             children = [self.build_from_json(json_data=child, ignore_children=ignore_children) for child in
                         json_data['children']]
         data = copy.copy(json_data['data'])
-        if 'name' not in data:
-            data['name'] = json_data['tag']
-        node = creator(data, children)
+
+        # if 'name' not in data:
+        #     data['name'] = json_data['tag']
+
+        attrs = {
+            **self.kwargs,
+            **data,
+        }
+        try:
+            node = creator(**attrs, children=children)
+        except Exception as e:
+            print(creator, e)
+            raise e
+        node.attrs = attrs
+
         if BT_PRESET_DATA_KEY.ID in data and data[BT_PRESET_DATA_KEY.ID]:
             node.id = uuid.UUID(data[BT_PRESET_DATA_KEY.ID])
         if BT_PRESET_DATA_KEY.STATUS in data and data[BT_PRESET_DATA_KEY.STATUS]:
             node.status = Status(data[BT_PRESET_DATA_KEY.STATUS])
 
         if isinstance(node, Action) and 'actions' in data and data['actions']:
             for action in data['actions']:
                 node.actions.put_nowait(action)
         return node
 
     def register_default(self):
-        self.register_bt(
+        self.register_node(
                 Sequence,
                 SequenceWithMemory,
                 ReactiveSequence,
                 Parallel,
                 ReactiveSelector,
                 Selector,
                 ReactiveSelector,
                 SelectorWithMemory,
                 ConditionBranch,
+                Template,
+                PreCondition,
+                PostCondition
         )
 
-        self.register_bt(
+        self.register_node(
                 Failure,
                 Success,
-                Running
+                Running,
         )
 
-        self.register_bt(
+        self.register_node(
                 Inverter,
                 RunningUntilCondition,
                 OneShot,
                 Count,
                 RunningIsFailure,
                 RunningIsSuccess,
                 FailureIsSuccess,
```

### Comparing `pybts-1.3.3/pybts/composites/composite.py` & `pybts-1.3.5/pybts/composites/composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,17 @@
     """
 
     def __init__(
             self,
             children: typing.Optional[typing.List[py_trees.behaviour.Behaviour]] = None,
             **kwargs
     ):
-        super().__init__(**kwargs)
-        if children is not None:
-            for child in children:
-                self.add_child(child)
-        else:
-            self.children = []
+        super().__init__(children=children, **kwargs)
         self.current_child: typing.Optional[behaviour.Behaviour] = None
 
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(children=c, **d)
-
     def stop(self, new_status: Status = Status.INVALID) -> None:
         """
         Provide common stop-level functionality for all composites.
 
          * Retain the current child on :data:`~py_trees.common.Status.SUCCESS` or
            :data:`~py_trees.common.Status.FAILURE` (for introspection), lose it on
            :data:`~py_trees.common.Status.INVALID`
@@ -220,51 +211,50 @@
         Returns:
             uuid.UUID: unique id of the child
         """
         self.children.insert(index, child)
         child.parent = self
         return child.id
 
+    def SEQ_SEL_tick(
+            self,
+            tick_again_status: list[Status],
+            continue_status: list[Status],
+            no_child_status: Status,
+            start_index: int = 0
+    ):
+        """Sequence/Selector的tick逻辑"""
+        self.debug_info['tick_count'] += 1
+        self.logger.debug("%s.tick()" % (self.__class__.__name__))
+
+        if self.status in tick_again_status:
+            # 重新执行上次执行的子节点
+            assert self.current_child is not None
+            index = self.children.index(self.current_child)
+        else:
+            self.current_child = None  # 从头执行
+            index = start_index
 
-def SEQ_SEL_tick(
-        self: Composite,
-        tick_again_status: list[Status],
-        continue_status: list[Status],
-        no_child_status: Status,
-        start_index: int = 0
-):
-    """Sequence/Selector的tick逻辑"""
-    self.debug_info['tick_count'] += 1
-    self.logger.debug("%s.tick()" % (self.__class__.__name__))
-
-    if self.status in tick_again_status:
-        # 重新执行上次执行的子节点
-        assert self.current_child is not None
-        index = self.children.index(self.current_child)
-    else:
-        self.current_child = None  # 从头执行
-        index = start_index
-
-    for child in itertools.islice(self.children, index, None):
-        self.current_child = child
-        yield from child.tick()
-        if child.status not in continue_status:
-            break
-
-    if self.current_child is not None:
-        new_status = self.current_child.status
-
-        index = self.children.index(self.current_child)
-
-        # 剩余的子节点全部停止
-        for child in itertools.islice(self.children, index + 1, None):
-            # 清除子节点的状态（停止正在执行的子节点）
-            child.stop(Status.INVALID)
-    else:
-        new_status = no_child_status
+        for child in itertools.islice(self.children, index, None):
+            self.current_child = child
+            yield from child.tick()
+            if child.status not in continue_status:
+                break
 
-    # TODO: 这里要不要加这个是存疑的（组合节点invalid stop会停止所有子节点，所以某个子节点返回invalid是否要将所有的其他节点都停止？）
-    # if new_status != Status.RUNNING:
-    #     self.stop(new_status)
+        if self.current_child is not None:
+            new_status = self.current_child.status
 
-    self.status = new_status
-    yield self
+            index = self.children.index(self.current_child)
+
+            # 剩余的子节点全部停止
+            for child in itertools.islice(self.children, index + 1, None):
+                # 清除子节点的状态（停止正在执行的子节点）
+                child.stop(Status.INVALID)
+        else:
+            new_status = no_child_status
+
+        # TODO: 这里要不要加这个是存疑的（组合节点invalid stop会停止所有子节点，所以某个子节点返回invalid是否要将所有的其他节点都停止？）
+        # if new_status != Status.RUNNING:
+        #     self.stop(new_status)
+
+        self.status = new_status
+        yield self
```

### Comparing `pybts-1.3.3/pybts/composites/condition_branch.py` & `pybts-1.3.5/pybts/composites/condition_branch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-import py_trees
 from py_trees.behaviour import Behaviour
-
-from pybts.node import Node
-from abc import ABC
 import typing
 from py_trees.common import Status
-from py_trees import behaviour
-import itertools
-from pybts.composites.composite import Composite, SEQ_SEL_tick
-
+from pybts.composites.composite import Composite
 
 class ConditionBranch(Composite):
     """
     条件分支节点
     只能有2或3个子节点
 
     也可以起到打断RUNNING节点的效果（由前面的条件节点来判断是否要进行打断）
```

### Comparing `pybts-1.3.3/pybts/composites/parallel.py` & `pybts-1.3.5/pybts/composites/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,15 @@
 
     def __init__(
             self,
             success_threshold: int = 1,
             **kwargs
     ):
         super().__init__(**kwargs)
-        self.success_threshold = success_threshold
-
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(
-                success_threshold=int(d.get('success_threshold', 1)),
-                children=c,
-                **d
-        )
+        self.success_threshold = int(success_threshold)
 
     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
         """
             同时执行所有子节点，并根据成功阈值来决定返回状态
             - 如果有子节点返回 RUNNING 状态，节点本身返回 RUNNING
             - 子节点的执行不依赖于其它子节点的状态；每个子节点独立执行
             - 如果达到或超过指定的成功阈值（success_threshold），则返回 SUCCESS
```

### Comparing `pybts-1.3.3/pybts/composites/selector.py` & `pybts-1.3.5/pybts/composites/selector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import py_trees
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
-from pybts.composites.composite import Composite, SEQ_SEL_tick
+from pybts.composites.composite import Composite
 
 
 class Selector(Composite):
     """
     组合节点：选择节点
     依次顺序执行子节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 SUCCESS，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return SEQ_SEL_tick(
-                self,
+        return self.SEQ_SEL_tick(
                 tick_again_status=[Status.RUNNING],
                 continue_status=[Status.FAILURE, Status.INVALID],
                 no_child_status=Status.FAILURE,
                 start_index=0)
 
 
 class SelectorWithMemory(Selector):
     """
     记忆选择节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
-    - 当前执行节点返回 SUCCESS，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return SEQ_SEL_tick(
-                self,
+        return self.SEQ_SEL_tick(
                 tick_again_status=[Status.SUCCESS, Status.RUNNING],
                 continue_status=[Status.FAILURE, Status.INVALID],
                 no_child_status=Status.FAILURE,
                 start_index=0)
 
 
 class ReactiveSelector(Selector):
@@ -48,13 +45,12 @@
     依次顺序执行子节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return SEQ_SEL_tick(
-                self,
+        return self.SEQ_SEL_tick(
                 tick_again_status=[],
                 continue_status=[Status.FAILURE, Status.INVALID],
                 no_child_status=Status.FAILURE,
                 start_index=0)
```

### Comparing `pybts-1.3.3/pybts/composites/sequence.py` & `pybts-1.3.5/pybts/composites/sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import py_trees
 from pybts.node import Node
 from abc import ABC
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
 import itertools
-from pybts.composites.composite import Composite, SEQ_SEL_tick
+from pybts.composites.composite import Composite
 
 
 class Sequence(Composite):
     """
     组合节点：顺序节点
     依次顺序执行子节点
     - 当前执行节点返回 SUCCESS，继续执行后续节点
     - 当前执行节点返回 RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 FAILURE/INVALID，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return SEQ_SEL_tick(
-                self,
+        return self.SEQ_SEL_tick(
                 tick_again_status=[Status.RUNNING],
                 continue_status=[Status.SUCCESS],
                 no_child_status=Status.SUCCESS,
                 start_index=0)
 
 
 class SequenceWithMemory(Sequence):
@@ -34,16 +33,15 @@
     - 当前执行节点返回 SUCCESS，继续执行后续节点
     - 当前执行节点返回 FAILURE/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 INVALID，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return SEQ_SEL_tick(
-                self,
+        return self.SEQ_SEL_tick(
                 tick_again_status=[Status.RUNNING, Status.FAILURE],
                 continue_status=[Status.SUCCESS],
                 no_child_status=Status.SUCCESS,
                 start_index=0)
 
 
 class ReactiveSequence(Sequence):
@@ -55,13 +53,12 @@
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
 
     可以起到打断后续RUNNING节点的效果
     - 如果前面的节点返回SUCCESS，则后续的RUNNING节点会继续运行，否则就会打断掉
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return SEQ_SEL_tick(
-                self,
+        return self.SEQ_SEL_tick(
                 tick_again_status=[],
                 continue_status=[Status.SUCCESS],
                 no_child_status=Status.SUCCESS,
                 start_index=0)
```

### Comparing `pybts-1.3.3/pybts/constants.py` & `pybts-1.3.5/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/decorators/nodes.py` & `pybts-1.3.5/pybts/decorators/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,20 @@
 
 class Decorator(Node, ABC):
     """
     装饰节点
     只有一个子节点
     """
 
-    def __init__(self, child: py_trees.behaviour.Behaviour, **kwargs):
+    def __init__(self, children: list[py_trees.behaviour.Behaviour], **kwargs):
         # Checks
-        if not isinstance(child, py_trees.behaviour.Behaviour):
-            raise TypeError(
-                    "A decorator's child must be an instance of py_trees.behaviours.Behaviour"
-            )
         # Initialise
-        super().__init__(**kwargs)
-        self.children.append(child)
+        super().__init__(children=children,**kwargs)
         # Give a convenient alias
         self.decorated = self.children[0]
-        self.decorated.parent = self
-
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(child=c[0], **d)
 
     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
         """
         Manage the decorated child through the tick.
 
         Yields:
             a reference to itself or one of its children
@@ -120,35 +110,28 @@
 
     Encapsulates a behaviour and wait for it's status to flip to the
     desired state. This behaviour will tick with
     :data:`~py_trees.Status.RUNNING` while waiting and
     :data:`~py_trees.Status.SUCCESS` when the flip occurs.
     """
 
-    def __init__(self, child: py_trees.behaviour.Behaviour, status: str | Status, **kwargs):
+    def __init__(self, status: str | Status, **kwargs):
         """
         Initialise with child and optional name, status variables.
 
         Args:
             name: the decorator name
             child: the child to be decorated
             status: the desired status to watch for
         """
-        super().__init__(child=child, **kwargs)
+        super().__init__(**kwargs)
         if isinstance(status, str):
             status = Status(status)
         self.succeed_status = status
 
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(
-                child=c[0],
-                **d
-        )
-
     def to_data(self):
         return {
             **super().to_data(),
             'succeed_status': self.succeed_status
         }
 
     def update(self) -> Status:
@@ -188,40 +171,33 @@
     * With policy :data:`~py_trees.common.OneShotPolicy.ON_COMPLETION`, the oneshot will activate when the child
       returns :data:`~py_trees.Status.SUCCESS` || :data:`~py_trees.Status.FAILURE`.
 
     .. seealso:: :meth:`py_trees.idioms.oneshot`
     """
 
     def __init__(
-            self, child: py_trees.behaviour.Behaviour, policy: str | list[Status] = 'SUCCESS', **kwargs
+            self, policy: str | list[Status] = 'SUCCESS', **kwargs
     ):
         """
         Init with the decorated child.
 
         Args:
             child: behaviour to shoot
             name: the decorator name
             policy: policy determining when the oneshot should activate
             - SUCCESS
             - SUCCESS|FAILURE
         """
-        super(OneShot, self).__init__(child=child, **kwargs)
+        super(OneShot, self).__init__(**kwargs)
         self.final_status: typing.Optional[Status] = None
         if isinstance(policy, str):
             self.policy = list(map(lambda x: Status(x), policy.split('|')))
         else:
             self.policy = policy
 
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(
-                child=c[0],
-                **d
-        )
-
     def to_data(self):
         return {
             **super().to_data(),
             'policy'      : self.policy,
             'final_status': self.final_status
         }
 
@@ -290,23 +266,23 @@
         total_tick_count: number of ticks in total
         running_count: number of ticks resulting in this state
         success_count: number of ticks resulting in this state
         failure_count: number of ticks resulting in this state
         interrupt_count: number of times a higher priority has interrupted
     """
 
-    def __init__(self, child: py_trees.behaviour.Behaviour, name: str = '', **kwargs):
+    def __init__(self, **kwargs):
         """
         Init the counter.
 
         Args:
             name: the decorator name
             child: the child behaviour or subtree
         """
-        super(Count, self).__init__(name=name, child=child, **kwargs)
+        super(Count, self).__init__(**kwargs)
         self.total_tick_count = 0
         self.failure_count = 0
         self.success_count = 0
         self.running_count = 0
         self.interrupt_count = 0
 
     def to_data(self):
```

### Comparing `pybts-1.3.3/pybts/main.py` & `pybts-1.3.5/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/node.py` & `pybts-1.3.5/pybts/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,42 +24,49 @@
     - update
 
     如果update之后状态从RUNNING变更为SUCCESS/FAILURE/INVALID
     - stop
 
     下一次tick的时候状态一开始是RUNNING，则直接调用
     update
-
     """
 
-    def __init__(self, name: str = '', **kwargs):
+    def __init__(self, name: str = '', children: typing.List[py_trees.behaviour.Behaviour] = None, **kwargs):
         super().__init__(name=name or self.__class__.__name__)
         self._updater_iter = None
         self.debug_info = {
             'tick_count'      : 0,
             'update_count'    : 0,
             'reset_count'     : 0,
             'terminate_count' : 0,
             'initialise_count': 0
         }
+        self.attrs: typing.Dict[str, typing.AnyStr] = kwargs # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
+        self.context: typing.Optional[dict] = None  # 共享的字典，在tree.setup的时候提供
+        if children is not None:
+            self.children = children
+            for child in children:
+                child.parent = self
 
     def reset(self):
         self.debug_info['reset_count'] += 1
         self._updater_iter = None
         if self.status != Status.INVALID:
             self.stop(Status.INVALID)
 
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(**d)
+    @property
+    def converter(self):
+        from pybts.converter import Converter
+        return Converter(self)
 
     def to_data(self):
         # 在board上查看的信息
         return {
             'debug_info': self.debug_info,
+            'attrs'     : self.attrs
         }
 
     def update(self) -> Status:
         self.logger.debug("%s.update()" % (self.__class__.__name__))
         self.debug_info['update_count'] += 1
         if self._updater_iter is None:
             self._updater_iter = self.updater()
@@ -137,30 +144,36 @@
 
     def initialise(self) -> None:
         super().initialise()
         self.logger.debug("%s.initialise()" % (self.__class__.__name__))
         self.debug_info['initialise_count'] += 1
 
     def __str__(self):
+        attrs = {
+            'id': self.id.hex,
+            **self.attrs,
+        }
+
+        attrs_str = ' '.join([f'{k}="{attrs[k]}"' for k in attrs if isinstance(attrs[k], str) and attrs[k]])
         if len(self.children) == 0:
-            return f'<{self.name} id="{self.id.hex}"/>'
+            return f'<{self.name} {attrs_str}/>'
         else:
-            return f'<{self.name} id="{self.id.hex}"> {len(self.children)} </{self.name}>'
+            return f'<{self.name} {attrs_str}/>({len(self.children)})'
 
     def __repr__(self):
         return self.__str__()
 
 
 class Action(Node, ABC):
     """
     行为节点
     """
 
-    def __init__(self, name: str = '', **kwargs):
-        super().__init__(name=name, **kwargs)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.actions = Queue()
 
     def to_data(self):
         from pybts.utility import read_queue_without_destroying
         actions = read_queue_without_destroying(self.actions)
         return {
             **super().to_data(),
```

### Comparing `pybts-1.3.3/pybts/rl/on_policy.py` & `pybts-1.3.5/pybts/rl/on_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,18 @@
 class RLOnPolicyNode(ABC):
     """强化学习在线策略节点，拿来多继承用"""
 
     def __init__(self):
         self.rl_on_policy_collector = None
         self.rl_accum_reward = 0
         self.rl_info = None
-        self.rl_reward = 0 # 当前奖励
+        self.rl_reward = 0  # 当前奖励
         self.rl_obs = None
         self.rl_iteration = 0
+        self.rl_done = False
         self.rl_action = None
         self.rl_model: typing.Optional[OnPolicyAlgorithm] = None
 
     def reset(self):
         self.rl_accum_reward = 0
 
     def to_data(self):
@@ -228,37 +229,44 @@
     def rl_gen_info(self) -> dict:
         raise NotImplemented
 
     @abstractmethod
     def rl_gen_reward(self) -> float:
         raise NotImplemented
 
+    @abstractmethod
+    def rl_gen_done(self) -> bool:
+        # 返回当前环境是否结束
+        raise NotImplemented
+
+    def rl_device(self) -> str:
+        return 'cpu'
+
     def rl_take_action(self,
                        train: bool,
                        log_interval: int = 1,
                        save_interval: int = 5,
                        save_path: str = ''
                        ):
         assert self.rl_model is not None, 'RL model not initialized'
         model = self.rl_model
         info = self.rl_gen_info()
         reward = self.rl_gen_reward()
         obs = self.rl_gen_obs()
-
+        done = self.rl_gen_done()
         if train:
             try:
                 if self.rl_on_policy_collector is None:
                     self.rl_on_policy_collector = bt_on_policy_collect_rollouts(
                             model,
                             last_obs=obs)
                     action = self.rl_on_policy_collector.send(None)
                 else:
                     info = info
-                    action = self.rl_on_policy_collector.send(
-                            (obs, reward, info['terminated'] or info['truncated'], info))
+                    action = self.rl_on_policy_collector.send((obs, reward, done, info))
             except StopIteration:
                 self.rl_on_policy_collector = None
                 self.rl_iteration += 1
                 # Display training infos
                 bt_on_policy_train(model, iteration=self.rl_iteration, log_interval=log_interval)
                 if self.rl_iteration % save_interval == 0:
                     model.save(save_path)
@@ -272,65 +280,75 @@
             action, state = model.predict(obs)
 
         self.rl_obs = obs
         self.rl_reward = reward
         self.rl_info = info
         self.rl_accum_reward += reward
         self.rl_action = action
+        self.rl_done = done
         return action
 
     def rl_ppo_setup_model(self,
                            train: bool,
                            path: str,
                            policy: str,
                            tensorboard_log: str = '',
                            verbose: int = 1,
-                           n_steps: int = 8,
-                           batch_size: int = 8,
+                           n_steps: int = 2048,
+                           batch_size: int = 64,
                            tb_log_name: str = ''
                            ):
         env = DummyEnv(
                 env=self.rl_env(),
                 action_space=self.rl_action_space(),
                 observation_space=self.rl_observation_space())
         model: typing.Optional[OnPolicyAlgorithm] = None
 
-        if path != '':
-            try:
-                model = PPO.load(
-                        path=path,
-                        env=env,
-                        tensorboard_log=tensorboard_log,
-                        verbose=verbose,
-                        force_reset=False,
-                        n_steps=n_steps,
-                        batch_size=batch_size,
-                )
-            except:
-                pass
-        if model is None:
+        if train:
             model = PPO(
                     policy=policy,
                     env=env,
                     verbose=1,
                     tensorboard_log=tensorboard_log,
-                    n_steps=8,
-                    batch_size=8,
+                    n_steps=n_steps,
+                    batch_size=batch_size,
+                    device=self.rl_device()
+            )
+
+            if path != '':
+                try:
+                    model.set_parameters(
+                            load_path_or_dict=path,
+                            device=self.rl_device()
+                    )
+                except Exception as e:
+                    pass
+        else:
+            assert path != '', f'No model path provided: {path}'
+            model = PPO.load(
+                    path=path,
+                    env=env,
+                    tensorboard_log=tensorboard_log,
+                    verbose=verbose,
+                    force_reset=False,
+                    n_steps=n_steps,
+                    batch_size=batch_size,
+                    device=self.rl_device()
             )
 
         if train:
             bt_on_policy_setup_learn(
                     model,
                     obs=self.rl_gen_obs(),
-                    tb_log_name=tb_log_name
+                    tb_log_name=tb_log_name,
             )
 
         self.rl_model = model
         return model
-
+    
 # def bt_on_policy_predict(model: OnPolicyAlgorithm, last_obs):
 #     model.predict()
 #     # Switch to eval mode (this affects batch norm / dropout)
 #     model._last_obs = last_obs
 #     model.policy.set_training_mode(False)
 #     with th.no_grad():
 #         # Convert to pytorch tensor or to TensorDict
```

### Comparing `pybts-1.3.3/pybts/templates/favicon.ico` & `pybts-1.3.5/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/templates/static/index-BUWP2os5.js` & `pybts-1.3.5/pybts/templates/static/index-BUWP2os5.js`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/templates/static/index-BXdrQGHp.css` & `pybts-1.3.5/pybts/templates/static/index-BXdrQGHp.css`

 * *Files identical despite different names*

### Comparing `pybts-1.3.3/pybts/utility.py` & `pybts-1.3.5/pybts/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,7 +245,18 @@
     history_dir = os.path.join(log_dir, project, 'history')
     if os.path.exists(history_dir):
         delete_folder_contents(history_dir)
 
 
 def jinja2_render(template: str, context: dict) -> str:
     return jinja2.Template(template).render(context)
+
+
+def camel_case_to_snake_case(name):
+    """
+    驼峰转蛇形
+    :param name:
+    :return:
+    """
+    return ''.join(['_' + i.lower() if i.isupper() else i for i in name]).lstrip('_')
+
+
```

### Comparing `pybts-1.3.3/pyproject.toml` & `pybts-1.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.3.3"
+version = "1.3.5"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.3.3/PKG-INFO` & `pybts-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.3.3
+Version: 1.3.5
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -79,28 +79,31 @@
 
 ```python
 from pybts import Tree, board, builder
 from pybts.node import Action
 from py_trees import common
 import time
 
+
 # Define custom behavior node
 class Person(Action):
   def __init__(self, name: str, age: int):
     super().__init__(name=name)
     self.age = age
 
   def update(self) -> common.Status:
     self.age += 1
     return common.Status.SUCCESS
 
 
 # Build the behavior tree
 builder = builder.Builder()
-builder.register('Person', Person.creator)
+builder.register('Person', Person)
+# or
+builder.register_node(Person)  # will register tag 'Person' and 'person'(snake case)
 root = builder.build_from_file('demos/demo_bt.xml')
 tree = Tree(root=root, name='Person')
 
 # Initialize board for tracking
 bt_board = board.Board(tree=tree, log_dir='logs')
 
 bt_board.clear()
```

