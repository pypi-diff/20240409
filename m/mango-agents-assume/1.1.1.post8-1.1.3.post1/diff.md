# Comparing `tmp/mango_agents_assume-1.1.1.post8.tar.gz` & `tmp/mango_agents_assume-1.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_agents_assume-1.1.1.post8.tar", max compression
+gzip compressed data, was "mango_agents_assume-1.1.3.post1.tar", max compression
```

## Comparing `mango_agents_assume-1.1.1.post8.tar` & `mango_agents_assume-1.1.3.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1067 2022-11-03 13:22:16.556574 mango_agents_assume-1.1.1.post8/LICENSE
--rw-r--r--   0        0        0      141 2023-04-06 22:19:54.843999 mango_agents_assume-1.1.1.post8/mango/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 13:56:18.197719 mango_agents_assume-1.1.1.post8/mango/agent/__init__.py
--rw-r--r--   0        0        0    17440 2024-01-21 23:08:01.951540 mango_agents_assume-1.1.1.post8/mango/agent/core.py
--rw-r--r--   0        0        0    15746 2024-01-22 12:20:43.697234 mango_agents_assume-1.1.1.post8/mango/agent/role.py
--rw-r--r--   0        0        0        0 2023-01-10 13:56:18.197719 mango_agents_assume-1.1.1.post8/mango/container/__init__.py
--rw-r--r--   0        0        0    32371 2024-01-21 22:58:44.373765 mango_agents_assume-1.1.1.post8/mango/container/core.py
--rw-r--r--   0        0        0     6037 2024-01-22 12:20:43.529233 mango_agents_assume-1.1.1.post8/mango/container/external_coupling.py
--rw-r--r--   0        0        0     8927 2023-11-08 08:40:32.898862 mango_agents_assume-1.1.1.post8/mango/container/factory.py
--rw-r--r--   0        0        0    10859 2023-11-08 08:40:32.898862 mango_agents_assume-1.1.1.post8/mango/container/mqtt.py
--rw-r--r--   0        0        0     3946 2023-09-11 10:52:50.668639 mango_agents_assume-1.1.1.post8/mango/container/protocol.py
--rw-r--r--   0        0        0     9980 2023-09-11 10:52:50.668639 mango_agents_assume-1.1.1.post8/mango/container/tcp.py
--rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.1.post8/mango/messages/__init__.py
--rw-r--r--   0        0        0      992 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.1.post8/mango/messages/acl_message.proto
--rw-r--r--   0        0        0     2416 2024-01-22 12:24:19.685957 mango_agents_assume-1.1.1.post8/mango/messages/acl_message_pb2.py
--rw-r--r--   0        0        0    11319 2023-11-06 23:31:59.293673 mango_agents_assume-1.1.1.post8/mango/messages/codecs.py
--rw-r--r--   0        0        0     6006 2023-11-07 11:08:26.783856 mango_agents_assume-1.1.1.post8/mango/messages/message.py
--rw-r--r--   0        0        0       88 2023-01-07 21:29:58.312170 mango_agents_assume-1.1.1.post8/mango/messages/other_proto_msgs.proto
--rw-r--r--   0        0        0     1051 2024-01-22 12:24:19.685957 mango_agents_assume-1.1.1.post8/mango/messages/other_proto_msgs_pb2.py
--rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.1.post8/mango/modules/__init__.py
--rw-r--r--   0        0        0     2591 2023-09-11 10:52:43.728609 mango_agents_assume-1.1.1.post8/mango/modules/base_module.py
--rw-r--r--   0        0        0     4167 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.1.post8/mango/modules/mqtt_module.py
--rw-r--r--   0        0        0     4179 2024-01-22 12:20:43.589233 mango_agents_assume-1.1.1.post8/mango/modules/rabbit_module.py
--rw-r--r--   0        0        0     2827 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.1.post8/mango/modules/zero_module.py
--rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.1.post8/mango/util/__init__.py
--rw-r--r--   0        0        0     2670 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.1.post8/mango/util/clock.py
--rw-r--r--   0        0        0     4705 2024-01-22 12:20:43.637233 mango_agents_assume-1.1.1.post8/mango/util/distributed_clock.py
--rw-r--r--   0        0        0     9512 2024-01-22 12:20:43.689234 mango_agents_assume-1.1.1.post8/mango/util/distributed_termination.py
--rw-r--r--   0        0        0     9179 2023-09-11 10:52:50.672639 mango_agents_assume-1.1.1.post8/mango/util/multiprocessing.py
--rw-r--r--   0        0        0    28606 2024-01-21 23:07:00.611333 mango_agents_assume-1.1.1.post8/mango/util/scheduling.py
--rw-r--r--   0        0        0     1999 2023-10-20 14:46:08.168707 mango_agents_assume-1.1.1.post8/mango/util/termination_detection.py
--rw-r--r--   0        0        0     1325 2024-01-22 12:23:07.501715 mango_agents_assume-1.1.1.post8/pyproject.toml
--rw-r--r--   0        0        0     7488 2023-11-08 08:44:41.520711 mango_agents_assume-1.1.1.post8/readme.md
--rw-r--r--   0        0        0     8819 1970-01-01 00:00:00.000000 mango_agents_assume-1.1.1.post8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-11-03 13:22:16.556574 mango_agents_assume-1.1.3.post1/LICENSE
+-rw-r--r--   0        0        0      141 2023-04-06 22:19:54.843999 mango_agents_assume-1.1.3.post1/mango/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 13:56:18.197719 mango_agents_assume-1.1.3.post1/mango/agent/__init__.py
+-rw-r--r--   0        0        0    17623 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post1/mango/agent/core.py
+-rw-r--r--   0        0        0    17574 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post1/mango/agent/role.py
+-rw-r--r--   0        0        0        0 2023-01-10 13:56:18.197719 mango_agents_assume-1.1.3.post1/mango/container/__init__.py
+-rw-r--r--   0        0        0    32729 2024-04-09 10:17:04.387085 mango_agents_assume-1.1.3.post1/mango/container/core.py
+-rw-r--r--   0        0        0     6037 2024-04-09 08:54:16.173551 mango_agents_assume-1.1.3.post1/mango/container/external_coupling.py
+-rw-r--r--   0        0        0     8927 2024-03-18 17:17:20.173174 mango_agents_assume-1.1.3.post1/mango/container/factory.py
+-rw-r--r--   0        0        0    10859 2024-03-18 17:17:20.177174 mango_agents_assume-1.1.3.post1/mango/container/mqtt.py
+-rw-r--r--   0        0        0     3946 2023-09-11 10:52:50.668639 mango_agents_assume-1.1.3.post1/mango/container/protocol.py
+-rw-r--r--   0        0        0     9981 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post1/mango/container/tcp.py
+-rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post1/mango/messages/__init__.py
+-rw-r--r--   0        0        0      992 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post1/mango/messages/acl_message.proto
+-rw-r--r--   0        0        0     2416 2024-01-22 12:24:19.685957 mango_agents_assume-1.1.3.post1/mango/messages/acl_message_pb2.py
+-rw-r--r--   0        0        0    11319 2023-11-06 23:31:59.293673 mango_agents_assume-1.1.3.post1/mango/messages/codecs.py
+-rw-r--r--   0        0        0     6006 2023-11-07 11:08:26.783856 mango_agents_assume-1.1.3.post1/mango/messages/message.py
+-rw-r--r--   0        0        0       88 2023-01-07 21:29:58.312170 mango_agents_assume-1.1.3.post1/mango/messages/other_proto_msgs.proto
+-rw-r--r--   0        0        0     1051 2024-01-22 12:24:19.685957 mango_agents_assume-1.1.3.post1/mango/messages/other_proto_msgs_pb2.py
+-rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post1/mango/modules/__init__.py
+-rw-r--r--   0        0        0     2591 2023-09-11 10:52:43.728609 mango_agents_assume-1.1.3.post1/mango/modules/base_module.py
+-rw-r--r--   0        0        0     4167 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.3.post1/mango/modules/mqtt_module.py
+-rw-r--r--   0        0        0     4179 2024-03-18 17:17:20.177174 mango_agents_assume-1.1.3.post1/mango/modules/rabbit_module.py
+-rw-r--r--   0        0        0     2827 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.3.post1/mango/modules/zero_module.py
+-rw-r--r--   0        0        0        0 2022-11-03 13:22:16.560574 mango_agents_assume-1.1.3.post1/mango/util/__init__.py
+-rw-r--r--   0        0        0     2670 2023-04-06 22:19:54.847998 mango_agents_assume-1.1.3.post1/mango/util/clock.py
+-rw-r--r--   0        0        0     4705 2024-04-09 08:56:29.145255 mango_agents_assume-1.1.3.post1/mango/util/distributed_clock.py
+-rw-r--r--   0        0        0     9512 2024-03-18 17:17:20.181174 mango_agents_assume-1.1.3.post1/mango/util/distributed_termination.py
+-rw-r--r--   0        0        0     9179 2023-09-11 10:52:50.672639 mango_agents_assume-1.1.3.post1/mango/util/multiprocessing.py
+-rw-r--r--   0        0        0    30940 2024-03-18 17:18:29.556656 mango_agents_assume-1.1.3.post1/mango/util/scheduling.py
+-rw-r--r--   0        0        0     2109 2024-04-09 10:16:51.774507 mango_agents_assume-1.1.3.post1/mango/util/termination_detection.py
+-rw-r--r--   0        0        0     1325 2024-03-18 17:20:29.891957 mango_agents_assume-1.1.3.post1/pyproject.toml
+-rw-r--r--   0        0        0     7488 2023-11-08 08:44:41.520711 mango_agents_assume-1.1.3.post1/readme.md
+-rw-r--r--   0        0        0     8870 1970-01-01 00:00:00.000000 mango_agents_assume-1.1.3.post1/PKG-INFO
```

### Comparing `mango_agents_assume-1.1.1.post8/LICENSE` & `mango_agents_assume-1.1.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/agent/core.py` & `mango_agents_assume-1.1.3.post1/mango/agent/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module implements the base class for agents (:class:`Agent`).
 
 Every agent must live in a container. Containers are responsible for making
  connections to other agents.
 """
+
 import asyncio
 import logging
 from abc import ABC
 from datetime import datetime
 from typing import Any, Dict, Optional, Tuple, Union
 
 from ..container.core import Container
@@ -472,13 +473,19 @@
             self._stopped.set_result(True)
         self._context.deregister_agent(self.aid)
         try:
             # Shutdown reactive inbox task
             self._check_inbox_task.remove_done_callback(self.raise_exceptions)
             self._check_inbox_task.cancel()
             await self._check_inbox_task
-
+        except asyncio.CancelledError:
+            pass
+        try:
             await self._scheduler.stop()
         except asyncio.CancelledError:
             pass
+        try:
+            await self._scheduler.shutdown()
+        except asyncio.CancelledError:
+            pass
         finally:
             logger.info("Agent %s: Shutdown successful", self.aid)
```

### Comparing `mango_agents_assume-1.1.1.post8/mango/agent/role.py` & `mango_agents_assume-1.1.3.post1/mango/agent/role.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Furthermore there are two lifecycle methods to know about:
 * :func:`Role.setup` is called when the Role is added to the agent, so its the perfect place
                      for initialization and scheduling of tasks
 * :func:`Role.on_stop` is called when the container the agent lives in, is shut down
 """
 import asyncio
 from abc import ABC
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union, Callable
 
 from mango.agent.core import Agent, AgentContext, AgentDelegates
 from mango.util.scheduling import Scheduler
 
 
 class DataContainer:
     def __getitem__(self, key):
@@ -122,14 +122,15 @@
     def __init__(self, agent_context, scheduler):
         self._role_models = {}
         self._roles = []
         self._role_to_active = {}
         self._role_model_type_to_subs = {}
         self._message_subs = []
         self._send_msg_subs = {}
+        self._role_event_type_to_handler = {}
         self._agent_context = agent_context
         self._scheduler = scheduler
         self._data = DataContainer()
 
     def get_or_create_model(self, cls):
         """Creates or return (when already created) a central role model.
 
@@ -174,14 +175,23 @@
 
         Args:
             role ([type]): the role
         """
         self._roles.append(role)
         self._role_to_active[role] = True
 
+    def remove_role(self, role: Role) -> None:
+        """Remove a given role
+
+        Args:
+            role ([type]): the role
+        """
+        self._roles.remove(role)
+        del self._role_to_active[role]
+
     @property
     def roles(self) -> List[Role]:
         """Returns all roles
 
         Returns:
             List[Role]: the roles hold by this handler
         """
@@ -284,20 +294,31 @@
                 self._message_subs.insert(
                     i, (role, message_condition, method, priority)
                 )
                 break
             elif i == len(self._message_subs) - 1:
                 self._message_subs.append((role, message_condition, method, priority))
 
-    def subscribe_send(self, role, method):
+    def subscribe_send(self, role: Role, method: Callable):
         if role in self._send_msg_subs:
             self._send_msg_subs[role].append(method)
         else:
             self._send_msg_subs[role] = [method]
 
+    def emit_event(self, event: Any, event_source: Any = None):
+        subs = self._role_event_type_to_handler[type(event)]
+        for _, method in subs:
+            method(event, event_source)
+
+    def subscribe_event(self, role: Role, event_type: type, method: Callable):
+        if not event_type in self._role_event_type_to_handler:
+            self._role_event_type_to_handler[event_type] = []
+
+        self._role_event_type_to_handler[event_type] += [(role, method)]
+
 
 class RoleContext(AgentDelegates):
     """Implementation of the RoleContext."""
 
     def __init__(
         self,
         agent_context: AgentContext,
@@ -349,16 +370,29 @@
         self._role_handler.subscribe_send(role, method)
 
     def add_role(self, role: Role):
         """Add a role to the context.
 
         :param role: the Role
         """
+        role.bind(self)
         self._role_handler.add_role(role)
 
+        # Setup role
+        role.setup()
+
+    def remove_role(self, role: Role):
+        """Remove a role and call on_stop for clean up
+
+        :param role: the role to remove
+        :type role: Role
+        """
+        self._role_handler.remove_role(role)
+        asyncio.create_task(role.on_stop())
+
     def handle_message(self, content, meta: Dict[str, Any]):
         """Handle an incoming message, delegating it to all applicable subscribers
         for role, message_condition, method, _ in self._message_subs:
             if self._is_role_active(role) and message_condition(content, meta):
                 method(content, meta)
 
         :param content: content
@@ -394,14 +428,35 @@
             content=content,
             receiver_addr=receiver_addr,
             receiver_id=receiver_id,
             acl_metadata=acl_metadata,
             **kwargs
         )
 
+    def emit_event(self, event: Any, event_source: Any = None):
+        """Emit an custom event to other roles.
+
+        :param event: the event
+        :type event: Any
+        :param event_source: emitter of the event (mostly the emitting role), defaults to None
+        :type event_source: Any, optional
+        """
+        self._role_handler.emit_event(event, event_source)
+
+    def subscribe_event(self, role: Role, event_type: Any, handler_method: Callable):
+        """Subscribe to specific event types. The listener will be evaluated based
+        on their order of subscription
+
+        :param role: the role in which you want to handle the event
+        :type role: Role
+        :param event_type: the event type you want to handle
+        :type event_type: Any
+        """
+        self._role_handler.subscribe_event(role, event_type, handler_method)
+
     @property
     def addr(self):
         return self._agent_context.addr
 
     @property
     def aid(self):
         return self._aid
@@ -444,28 +499,23 @@
         )
 
     def add_role(self, role: Role):
         """Add a role to the agent. This will lead to the call of :func:`Role.setup`.
 
         :param role: the role to add
         """
-        role.bind(self._role_context)
         self._role_context.add_role(role)
 
-        # Setup role
-        role.setup()
-
     def remove_role(self, role: Role):
         """Remove a role permanently from the agent.
 
         :param role: [description]
         :type role: Role
         """
         self._role_context.remove_role(role)
-        asyncio.create_task(role.on_stop())
 
     @property
     def roles(self) -> List[Role]:
         """Returns list of roles
 
         :return: list of roles
         """
```

### Comparing `mango_agents_assume-1.1.1.post8/mango/container/core.py` & `mango_agents_assume-1.1.3.post1/mango/container/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,25 +349,27 @@
 
     def __init__(
         self,
         container,
     ) -> None:
         self._active = False
         self._container = container
+        self._mp_enabled = False
 
     def _init_mp(self):
         # For agent multiprocessing support
         self._agent_processes = []
         self._terminate_sub_processes = Event()
         self._pid_to_message_pipe = {}
         self._pid_to_pipe = {}
         self._pid_to_aids = {}
         self._handle_process_events_tasks: List[asyncio.Task] = []
         self._handle_sp_messages_tasks: List[asyncio.Task] = []
         self._main_queue = None
+        self._mp_enabled = True
 
     @property
     def aids(self):
         all_aids = []
         if self._active:
             for _, aids in self._pid_to_aids.items():
                 all_aids += aids
@@ -421,14 +423,16 @@
         target_inbox = None
         if self._active:
             target_inbox = self._find_sp_queue(receiver_id)
             default_meta["receiver_id"] = receiver_id
         return None, target_inbox
 
     def _find_sp_queue(self, aid):
+        if not self._mp_enabled:
+            return None
         for pid, aids in self._pid_to_aids.items():
             if aid in aids:
                 return PipeToWriteQueue(self._pid_to_message_pipe[pid])
         raise ValueError(f"The aid '{aid}' does not exist in any subprocess.")
 
     def create_agent_process(self, agent_creator, container, mirror_container_creator):
         if not self._active:
@@ -582,19 +586,25 @@
     def _reserve_aid(self, suggested_aid=None):
         aid = self._container_process_manager.pre_hook_reserve_aid(
             suggested_aid=suggested_aid
         )
         if aid is not None:
             return aid
 
-        if suggested_aid is None or not self.is_aid_available(suggested_aid):
-            aid = f"{AGENT_PATTERN_NAME_PRE}{self._aid_counter}"
-            self._aid_counter += 1
-        else:
-            aid = suggested_aid
+        if suggested_aid is not None:
+            if self.is_aid_available(suggested_aid):
+                return suggested_aid
+            else:
+                logger.warning(
+                    "The suggested aid could not be reserved, either it is not available or it is not allowed (pattern agentX);%s",
+                    suggested_aid,
+                )
+    
+        aid = f"{AGENT_PATTERN_NAME_PRE}{self._aid_counter}"
+        self._aid_counter += 1
         return aid
 
     def register_agent(self, agent, suggested_aid: str = None):
         """
         Register *agent* and return the agent id
         :param agent: The agent instance
         :param suggested_aid: (Optional) suggested aid, if the aid is already taken, a generated aid is used.
```

### Comparing `mango_agents_assume-1.1.1.post8/mango/container/external_coupling.py` & `mango_agents_assume-1.1.3.post1/mango/container/external_coupling.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/container/factory.py` & `mango_agents_assume-1.1.3.post1/mango/container/factory.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/container/mqtt.py` & `mango_agents_assume-1.1.3.post1/mango/container/mqtt.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/container/protocol.py` & `mango_agents_assume-1.1.3.post1/mango/container/protocol.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/container/tcp.py` & `mango_agents_assume-1.1.3.post1/mango/container/tcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains the abstract Container class and the subclasses
 TCPContainer and MQTTContainer
 """
+
 import asyncio
 import logging
 import time
 from typing import Optional, Tuple, Union
 
 from mango.container.core import Container, ContainerMirrorData
```

### Comparing `mango_agents_assume-1.1.1.post8/mango/messages/acl_message.proto` & `mango_agents_assume-1.1.3.post1/mango/messages/acl_message.proto`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/messages/acl_message_pb2.py` & `mango_agents_assume-1.1.3.post1/mango/messages/acl_message_pb2.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/messages/codecs.py` & `mango_agents_assume-1.1.3.post1/mango/messages/codecs.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/messages/message.py` & `mango_agents_assume-1.1.3.post1/mango/messages/message.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/messages/other_proto_msgs_pb2.py` & `mango_agents_assume-1.1.3.post1/mango/messages/other_proto_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/modules/base_module.py` & `mango_agents_assume-1.1.3.post1/mango/modules/base_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/modules/mqtt_module.py` & `mango_agents_assume-1.1.3.post1/mango/modules/mqtt_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/modules/rabbit_module.py` & `mango_agents_assume-1.1.3.post1/mango/modules/rabbit_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/modules/zero_module.py` & `mango_agents_assume-1.1.3.post1/mango/modules/zero_module.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/util/clock.py` & `mango_agents_assume-1.1.3.post1/mango/util/clock.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/util/distributed_clock.py` & `mango_agents_assume-1.1.3.post1/mango/util/distributed_clock.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/util/distributed_termination.py` & `mango_agents_assume-1.1.3.post1/mango/util/distributed_termination.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/util/multiprocessing.py` & `mango_agents_assume-1.1.3.post1/mango/util/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/mango/util/scheduling.py` & `mango_agents_assume-1.1.3.post1/mango/util/scheduling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,53 @@
 """
 Module for commonly used time based scheduled task executed inside one agent.
 """
+
 import asyncio
 import concurrent.futures
 import datetime
 from abc import abstractmethod
-from multiprocessing import Manager
+from multiprocessing import Manager, Event
 from typing import Any, List, Tuple
+from dataclasses import dataclass
+from multiprocessing.synchronize import Event as MultiprocessingEvent
 
 from dateutil.rrule import rrule
 
 from mango.util.clock import AsyncioClock, Clock, ExternalClock
+from asyncio import Future
+
+
+@dataclass
+class ScheduledProcessControl:
+    run_task_event: MultiprocessingEvent
+    kill_process_event: MultiprocessingEvent
+
+    def kill_process(self):
+        self.kill_process_event.set()
+
+    def init_process(self):
+        self.kill_process_event.clear()
+
+    def resume_task(self):
+        self.run_task_event.set()
+
+    def suspend_task(self):
+        self.run_task_event.clear()
 
 
 class Suspendable:
     """
     Wraps a coroutine, intercepting __await__ to add the functionality of suspending.
     """
 
-    def __init__(self, coro, ext_contr_event=None):
+    def __init__(self, coro, ext_contr_event=None, kill_event=None):
         self._coro = coro
 
+        self._kill_event = kill_event
         if ext_contr_event is not None:
             self._can_run = ext_contr_event
         else:
             self._can_run = asyncio.Event()
             self._can_run.set()
 
     def __await__(self):
@@ -39,14 +62,17 @@
                         # not allowed here as this is not an async method
                         yield from self._can_run.wait().__await__()
                     else:
                         self._can_run.wait()
             except BaseException as err:
                 send, message = iter_throw, err
 
+            if self._kill_event is not None and self._kill_event.is_set():
+                return None
+
             try:
                 # throw error or resume coroutine
                 signal = send(message)
             except StopIteration as err:
                 return err.value
             else:
                 send = iter_send
@@ -87,14 +113,21 @@
         """
         return self._coro
 
 
 # asyncio tasks
 
 
+def _close_coro(coro):
+    try:
+        coro.close()
+    except:
+        pass
+
+
 class ScheduledTask:
     """
     Base class for scheduled tasks in mango. Within this class it is possible to
     define what to do on execution and on stop. In most cases the logic should get
     passed as lambda while the scheduling logic is inside of class inheriting from this one.
     """
 
@@ -127,14 +160,19 @@
         """
         Called when the task is cancelled or finished.
         """
         if self._on_stop_hook_in is not None:
             self._on_stop_hook_in(fut)
         if self._is_observable:
             self._is_done.set_result(True)
+        self.close()
+
+    def close(self):
+        """Perform closing actions"""
+        pass
 
 
 class TimestampScheduledTask(ScheduledTask):
     """
     Timestamp based one-shot task. This task will get executed when a given unix timestamp is reached.
     """
 
@@ -151,14 +189,17 @@
         await sleep_future
         self.notify_running()
 
     async def run(self):
         await self._wait(self._timestamp)
         return await self._coro
 
+    def close(self):
+        _close_coro(self._coro)
+
 
 class AwaitingTask(ScheduledTask):
     """
     Awaiting task. This task will execute a given coroutine after another given coroutine has been awaited.
     Can be useful if you want to execute something after a Future has finished.
     """
 
@@ -171,27 +212,34 @@
 
     async def run(self):
         self.notify_sleeping()
         await self._awaited_coroutine
         self.notify_running()
         return await self._coroutine
 
+    def close(self):
+        _close_coro(self._awaited_coroutine)
+        _close_coro(self._coroutine)
+
 
 class InstantScheduledTask(TimestampScheduledTask):
     """
     One-shot task, which will get executed instantly.
     """
 
     def __init__(self, coroutine, clock: Clock = None, on_stop=None, observable=True):
         if clock is None:
             clock = AsyncioClock()
         super().__init__(
             coroutine, clock.time, clock=clock, on_stop=on_stop, observable=observable
         )
 
+    def close(self):
+        _close_coro(self._coro)
+
 
 class PeriodicScheduledTask(ScheduledTask):
     """
     Class for periodic scheduled tasks. It enables to create a task for an agent
     which will get executed periodically with a specified delay.
     """
 
@@ -270,14 +318,17 @@
         while not self._condition():
             sleep_future: asyncio.Future = self.clock.sleep(self._delay)
             self.notify_sleeping()
             await sleep_future
             self.notify_running()
         return await self._coro
 
+    def close(self):
+        _close_coro(self._coro)
+
 
 # process tasks
 
 
 class ScheduledProcessTask(ScheduledTask):
     # Mark class as task for an external process
 
@@ -403,25 +454,33 @@
         observable=True,
     ):
         # List of Tuples with asyncio.Future, ScheduledTask, Suspendable coro, Source
         self._scheduled_tasks: List[
             Tuple[ScheduledTask, asyncio.Future, Suspendable, Any]
         ] = []
         self.clock = clock if clock is not None else AsyncioClock()
-        self._scheduled_process_tasks = []
-        self._process_pool_exec = concurrent.futures.ProcessPoolExecutor(
-            max_workers=num_process_parallel, initializer=_create_asyncio_context
-        )
+        self._scheduled_process_tasks: List[
+            Tuple[ScheduledProcessTask, Future, ScheduledProcessControl, Any]
+        ] = []
+        self._manager = None
+        self._num_process_parallel = num_process_parallel
+        self._process_pool_exec = None
         self._suspendable = suspendable
         self._observable = observable
 
     @staticmethod
-    def _run_task_in_p_context(task, suspend_event):
+    def _run_task_in_p_context(
+        task, scheduled_process_control: ScheduledProcessControl
+    ):
         try:
-            coro = Suspendable(task.run(), ext_contr_event=suspend_event)
+            coro = Suspendable(
+                task.run(),
+                ext_contr_event=scheduled_process_control.run_task_event,
+                kill_event=scheduled_process_control.kill_process_event,
+            )
 
             return asyncio.get_event_loop().run_until_complete(coro)
         finally:
             pass
 
     async def sleep(self, t: float):
         """
@@ -615,26 +674,43 @@
         :type task: ScheduledProcessTask
         :return: future to check whether the task is done and to finally retrieve the result
         :rtype: _type_
         :param src: creator of the task
         :type src: Object
         """
 
+        if self._process_pool_exec is None:
+            self._process_pool_exec = concurrent.futures.ProcessPoolExecutor(
+                max_workers=self._num_process_parallel,
+                initializer=_create_asyncio_context,
+            )
         loop = asyncio.get_running_loop()
-        manager = Manager()
-        event = manager.Event()
-        event.set()
+        if self._manager is None:
+            self._manager = Manager()
+
+        scheduled_process_control = ScheduledProcessControl(
+            run_task_event=self._manager.Event(),
+            kill_process_event=self._manager.Event(),
+        )
+        scheduled_process_control.init_process()
+        scheduled_process_control.resume_task()
+
         l_task = asyncio.ensure_future(
             loop.run_in_executor(
-                self._process_pool_exec, Scheduler._run_task_in_p_context, task, event
+                self._process_pool_exec,
+                Scheduler._run_task_in_p_context,
+                task,
+                scheduled_process_control,
             )
         )
         l_task.add_done_callback(self._remove_process_task)
         l_task.add_done_callback(task.on_stop)
-        self._scheduled_process_tasks.append((task, l_task, event, src))
+        self._scheduled_process_tasks.append(
+            (task, l_task, scheduled_process_control, src)
+        )
         return l_task
 
     def schedule_timestamp_process_task(
         self, coroutine_creator, timestamp: float, on_stop=None, src=None
     ):
         """Schedule a task at specified unix timestamp dispatched to another process.
 
@@ -754,40 +830,41 @@
         """
         if not self._suspendable:
             raise Exception("The scheduler is configured as non-suspendable!")
 
         for _, _, coro, src in self._scheduled_tasks:
             if src == given_src and coro is not None:
                 coro.suspend()
-        for _, _, event, src in self._scheduled_process_tasks:
-            if src == given_src and event is not None:
-                event.clear()
+        for _, _, scheduled_process_control, src in self._scheduled_process_tasks:
+            if src == given_src:
+                scheduled_process_control.suspend_task()
 
     def resume(self, given_src):
         """Resume a set of tasks triggered by the given src object.
 
         :param given_src: the src object
         :type given_src: object
         """
         if not self._suspendable:
             raise Exception("The scheduler is configured as non-suspendable!")
 
         for _, _, coro, src in self._scheduled_tasks:
             if src == given_src and coro is not None:
                 coro.resume()
-        for _, _, event, src in self._scheduled_process_tasks:
-            if src == given_src and event is not None:
-                event.set()
+        for _, _, scheduled_process_control, src in self._scheduled_process_tasks:
+            if src == given_src:
+                scheduled_process_control.resume_task()
 
     def _remove_process_task(self, fut=asyncio.Future):
         for i in range(len(self._scheduled_process_tasks)):
-            _, task, event, _ = self._scheduled_process_tasks[i]
+            _, task, scheduled_process_control, _ = self._scheduled_process_tasks[i]
             if task == fut:
+                scheduled_process_control.resume_task()
+                scheduled_process_control.kill_process()
                 del self._scheduled_process_tasks[i]
-                event.set()
                 break
 
     # methods for removing tasks, stopping or shutting down
 
     def _remove_task(self, fut=asyncio.Future):
         self._remove_generic_task(self._scheduled_tasks, fut=fut)
 
@@ -838,16 +915,19 @@
                 if (
                     scheduled_task._is_sleeping.done()
                     and scheduled_task not in sleeping_tasks
                 ):
                     # we need to recognize how many sleeping tasks we have in order to find out if all tasks are done
                     sleeping_tasks.append(scheduled_task)
 
-    def shutdown(self):
+    async def shutdown(self):
         """
         Shutdown internal process executor pool.
         """
         # resume all process so they can get shutdown
-        for _, _, event, _ in self._scheduled_process_tasks:
-            if event is not None:
-                event.set()
-        self._process_pool_exec.shutdown()
+        for _, _, scheduled_process_control, _ in self._scheduled_process_tasks:
+            scheduled_process_control.kill_process()
+        for task, _, _, _ in self._scheduled_tasks:
+            task.close()
+        await self.stop()
+        if self._process_pool_exec is not None:
+            self._process_pool_exec.shutdown()
```

### Comparing `mango_agents_assume-1.1.1.post8/mango/util/termination_detection.py` & `mango_agents_assume-1.1.3.post1/mango/util/termination_detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,25 @@
             if scheduled_task._is_sleeping.done():
                 # we need to recognize how many sleeping tasks we have in order to find out if all tasks are done
                 sleeping_tasks.append(scheduled_task)
         unfinished_tasks += len(scheduled_tasks) - len(sleeping_tasks)
     return unfinished_tasks
 
 
-async def tasks_complete_or_sleeping(container: Container):
+async def tasks_complete_or_sleeping(container: Container, except_sources=["no_wait"]):
     sleeping_tasks = []
     task_list = []
     await container.inbox.join()
     for agent in container._agents.values():
         await agent.inbox.join()
         task_list.extend(agent._scheduler._scheduled_tasks)
         task_list.extend(agent._scheduler._scheduled_process_tasks)
 
     while len(task_list) > len(sleeping_tasks):
+        task_list = list(filter(lambda x: x[3] not in except_sources, task_list))
         await container.inbox.join()
         for scheduled_task, task, _, _ in task_list:
             await asyncio.wait(
                 [scheduled_task._is_sleeping, scheduled_task._is_done],
                 return_when=asyncio.FIRST_COMPLETED,
             )
             if (
```

### Comparing `mango_agents_assume-1.1.1.post8/pyproject.toml` & `mango_agents_assume-1.1.3.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mango-agents-assume"
-version = "1.1.1-8"
+version = "1.1.3-1"
 description = "Modular Python Agent Framework - Temporary Fork of mango for development purpose"
 authors = ["Mango Developers <mango@offis.de>", "Florian Maurer <fmaurer@disroot.org>"]
 license = "LICENSE"
 readme = "readme.md"
 
 homepage = "https://mango-agents.readthedocs.io/"
 repository = "https://gitlab.com/maurerle/mango"
```

### Comparing `mango_agents_assume-1.1.1.post8/readme.md` & `mango_agents_assume-1.1.3.post1/readme.md`

 * *Files identical despite different names*

### Comparing `mango_agents_assume-1.1.1.post8/PKG-INFO` & `mango_agents_assume-1.1.3.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-agents-assume
-Version: 1.1.1.post8
+Version: 1.1.3.post1
 Summary: Modular Python Agent Framework - Temporary Fork of mango for development purpose
 Home-page: https://mango-agents.readthedocs.io/
 License: LICENSE
 Keywords: agent based simulation,simulation
 Author: Mango Developers
 Author-email: mango@offis.de
 Requires-Python: >=3.7,<4.0
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dill (>=0.3.6)
 Requires-Dist: msgspec (>=0.14.2)
 Requires-Dist: paho-mqtt (>=1.5.1,<2.0.0)
 Requires-Dist: protobuf (>=3.20.3,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
```

