# Comparing `tmp/agent-bdi-2.3.6.tar.gz` & `tmp/agent-bdi-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent-bdi-2.3.6.tar", last modified: Wed Mar 13 17:02:32 2024, max compression
+gzip compressed data, was "agent-bdi-2.4.0.tar", last modified: Tue Apr  9 08:36:20 2024, max compression
```

## Comparing `agent-bdi-2.3.6.tar` & `agent-bdi-2.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.778825 agent-bdi-2.3.6/
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/LICENSE.md
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3202 2024-03-13 17:02:32.777820 agent-bdi-2.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/README.md
--rw-rw-rw-   0        0        0       42 2024-03-13 17:02:32.778825 agent-bdi-2.3.6/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-03-13 17:02:17.000000 agent-bdi-2.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.718700 agent-bdi-2.3.6/src/
--rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.3.6/src/__init__.py
--rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.3.6/src/abdi_config.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.737211 agent-bdi-2.3.6/src/agent_bdi.egg-info/
--rw-rw-rw-   0        0        0     3202 2024-03-13 17:02:32.000000 agent-bdi-2.3.6/src/agent_bdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-03-13 17:02:32.000000 agent-bdi-2.3.6/src/agent_bdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 17:02:32.000000 agent-bdi-2.3.6/src/agent_bdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-03-13 17:02:32.000000 agent-bdi-2.3.6/src/agent_bdi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.747874 agent-bdi-2.3.6/src/broker/
--rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.3.6/src/broker/__init__.py
--rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.3.6/src/broker/broker_maker.py
--rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.3.6/src/broker/empty_broker.py
--rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.3.6/src/broker/message_broker.py
--rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.3.6/src/broker/mqtt_broker.py
--rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.3.6/src/broker/notifier.py
--rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.3.6/src/broker/redis_broker.py
--rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.3.6/src/broker/ros_broker.py
--rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.3.6/src/broker/ros_noetic_broker.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.751873 agent-bdi-2.3.6/src/core/
--rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.3.6/src/core/Agent.py
--rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/core/Belief.py
--rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/core/Desire.py
--rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/core/Intention.py
--rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.759875 agent-bdi-2.3.6/src/holon/
--rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/holon/Blackboard.py
--rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.3.6/src/holon/Heart.py
--rw-rw-rw-   0        0        0    10966 2024-03-13 16:08:32.000000 agent-bdi-2.3.6/src/holon/HolonicAgent.py
--rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/holon/HolonicDesire.py
--rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.3.6/src/holon/HolonicIntention.py
--rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.3.6/src/holon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.768388 agent-bdi-2.3.6/src/holon/logistics/
--rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.3.6/src/holon/logistics/__init__.py
--rw-rw-rw-   0        0        0      710 2024-02-24 14:56:32.000000 agent-bdi-2.3.6/src/holon/logistics/base_logistic.py
--rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.3.6/src/holon/logistics/broker_logistic.py
--rw-rw-rw-   0        0        0     5299 2024-02-26 10:20:43.000000 agent-bdi-2.3.6/src/holon/logistics/loading_coordinator.py
--rw-rw-rw-   0        0        0     6199 2024-02-24 17:44:27.000000 agent-bdi-2.3.6/src/holon/logistics/payload_wrapper.py
--rw-rw-rw-   0        0        0     3488 2024-02-24 20:30:24.000000 agent-bdi-2.3.6/src/holon/logistics/request_logistic.py
--rw-rw-rw-   0        0        0     2367 2024-02-24 20:21:15.000000 agent-bdi-2.3.6/src/holon/logistics/response_logistic.py
--rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.3.6/src/holon/payload.py
-drwxrwxrwx   0        0        0        0 2024-03-13 17:02:32.772391 agent-bdi-2.3.6/tests/
--rw-rw-rw-   0        0        0      762 2024-01-07 09:18:18.000000 agent-bdi-2.3.6/tests/test01.py
--rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.3.6/tests/test_loadingbal.py
--rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.3.6/tests/test_request.py
--rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.3.6/tests/test_send.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.339026 agent-bdi-2.4.0/
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/LICENSE.md
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3202 2024-04-09 08:36:20.338026 agent-bdi-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 08:36:20.339026 agent-bdi-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-04-09 08:36:11.000000 agent-bdi-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.287969 agent-bdi-2.4.0/src/
+-rw-rw-rw-   0        0        0        0 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/abdi_config.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.304458 agent-bdi-2.4.0/src/agent_bdi.egg-info/
+-rw-rw-rw-   0        0        0     3202 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 08:36:20.000000 agent-bdi-2.4.0/src/agent_bdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.313458 agent-bdi-2.4.0/src/broker/
+-rw-rw-rw-   0        0        0      134 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/__init__.py
+-rw-rw-rw-   0        0        0      964 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/broker_maker.py
+-rw-rw-rw-   0        0        0      943 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/empty_broker.py
+-rw-rw-rw-   0        0        0      645 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/message_broker.py
+-rw-rw-rw-   0        0        0     2186 2024-03-13 16:08:10.000000 agent-bdi-2.4.0/src/broker/mqtt_broker.py
+-rw-rw-rw-   0        0        0      383 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/broker/notifier.py
+-rw-rw-rw-   0        0        0      903 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/redis_broker.py
+-rw-rw-rw-   0        0        0      897 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/ros_broker.py
+-rw-rw-rw-   0        0        0     2651 2024-01-04 04:28:19.000000 agent-bdi-2.4.0/src/broker/ros_noetic_broker.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.318800 agent-bdi-2.4.0/src/core/
+-rw-rw-rw-   0        0        0      316 2023-05-22 15:55:38.000000 agent-bdi-2.4.0/src/core/Agent.py
+-rw-rw-rw-   0        0        0       58 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/Belief.py
+-rw-rw-rw-   0        0        0       52 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/Desire.py
+-rw-rw-rw-   0        0        0       55 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/Intention.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.326216 agent-bdi-2.4.0/src/holon/
+-rw-rw-rw-   0        0        0      116 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/holon/Blackboard.py
+-rw-rw-rw-   0        0        0      452 2023-05-28 19:59:05.000000 agent-bdi-2.4.0/src/holon/Heart.py
+-rw-rw-rw-   0        0        0    11104 2024-04-04 18:17:14.000000 agent-bdi-2.4.0/src/holon/HolonicAgent.py
+-rw-rw-rw-   0        0        0       72 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/holon/HolonicDesire.py
+-rw-rw-rw-   0        0        0       84 2023-04-25 11:32:48.000000 agent-bdi-2.4.0/src/holon/HolonicIntention.py
+-rw-rw-rw-   0        0        0        0 2023-12-25 14:17:27.000000 agent-bdi-2.4.0/src/holon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.331951 agent-bdi-2.4.0/src/holon/logistics/
+-rw-rw-rw-   0        0        0        0 2024-02-13 16:04:18.000000 agent-bdi-2.4.0/src/holon/logistics/__init__.py
+-rw-rw-rw-   0        0        0      710 2024-02-24 14:56:32.000000 agent-bdi-2.4.0/src/holon/logistics/base_logistic.py
+-rw-rw-rw-   0        0        0      356 2024-02-07 10:01:09.000000 agent-bdi-2.4.0/src/holon/logistics/broker_logistic.py
+-rw-rw-rw-   0        0        0     5299 2024-02-26 10:20:43.000000 agent-bdi-2.4.0/src/holon/logistics/loading_coordinator.py
+-rw-rw-rw-   0        0        0     6333 2024-04-04 18:40:47.000000 agent-bdi-2.4.0/src/holon/logistics/payload_wrapper.py
+-rw-rw-rw-   0        0        0     3570 2024-04-04 18:43:34.000000 agent-bdi-2.4.0/src/holon/logistics/request_logistic.py
+-rw-rw-rw-   0        0        0     2367 2024-02-24 20:21:15.000000 agent-bdi-2.4.0/src/holon/logistics/response_logistic.py
+-rw-rw-rw-   0        0        0       80 2024-01-05 16:48:07.000000 agent-bdi-2.4.0/src/holon/payload.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:36:20.337018 agent-bdi-2.4.0/tests/
+-rw-rw-rw-   0        0        0      762 2024-01-07 09:18:18.000000 agent-bdi-2.4.0/tests/test01.py
+-rw-rw-rw-   0        0        0     1837 2024-02-15 11:41:34.000000 agent-bdi-2.4.0/tests/test_loadingbal.py
+-rw-rw-rw-   0        0        0     2318 2024-01-06 16:12:29.000000 agent-bdi-2.4.0/tests/test_request.py
+-rw-rw-rw-   0        0        0     2754 2024-01-06 16:34:09.000000 agent-bdi-2.4.0/tests/test_send.py
```

### Comparing `agent-bdi-2.3.6/PKG-INFO` & `agent-bdi-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.3.6
+Version: 2.4.0
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.3.6/README.md` & `agent-bdi-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/setup.py` & `agent-bdi-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "agent-bdi",
-    version = "2.3.6",
+    version = "2.4.0",
     author = "Ming Fang Shiu",
     author_email='avatar.xu@gmail.com',
     description='Agent BDI framework',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mfshiu/abdi.git",
     project_urls = {
```

### Comparing `agent-bdi-2.3.6/src/abdi_config.py` & `agent-bdi-2.4.0/src/abdi_config.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/agent_bdi.egg-info/PKG-INFO` & `agent-bdi-2.4.0/src/agent_bdi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-bdi
-Version: 2.3.6
+Version: 2.4.0
 Summary: Agent BDI framework
 Home-page: https://github.com/mfshiu/abdi.git
 Author: Ming Fang Shiu
 Author-email: avatar.xu@gmail.com
 Project-URL: Bug Tracker, https://bugtracker.zoho.com/portal/avatardotxugmaildotcom#allprojects/1982079000000043717/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agent-bdi-2.3.6/src/agent_bdi.egg-info/SOURCES.txt` & `agent-bdi-2.4.0/src/agent_bdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/broker_maker.py` & `agent-bdi-2.4.0/src/broker/broker_maker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/empty_broker.py` & `agent-bdi-2.4.0/src/broker/empty_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/message_broker.py` & `agent-bdi-2.4.0/src/broker/message_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/mqtt_broker.py` & `agent-bdi-2.4.0/src/broker/mqtt_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/redis_broker.py` & `agent-bdi-2.4.0/src/broker/redis_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/ros_broker.py` & `agent-bdi-2.4.0/src/broker/ros_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/broker/ros_noetic_broker.py` & `agent-bdi-2.4.0/src/broker/ros_noetic_broker.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/holon/HolonicAgent.py` & `agent-bdi-2.4.0/src/holon/HolonicAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import inspect
+import logging
 from multiprocessing import Process
 import os
 import signal
 import sys
 import threading
 import time 
 from typing import final
 import uuid
 
 currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parentdir = os.path.dirname(currentdir)
 sys.path.insert(0, parentdir) 
 
-import hashlib
-import logging
-
 from abdi_config import AbdiConfig, LOGGER_NAME
 from broker.notifier import BrokerNotifier
 from broker.broker_maker import BrokerMaker
 from core.Agent import Agent
 from holon.Blackboard import Blackboard
 from holon.HolonicDesire import HolonicDesire
 from holon.HolonicIntention import HolonicIntention
 from holon.logistics.base_logistic import BaseLogistic
-# from holon.logistics.broker_logistic import BrokerLogistic
-from holon.payload import Payload
 
 
 logger = logging.getLogger(LOGGER_NAME)
 
 
-
 class HolonicAgent(Agent, BrokerNotifier) :
     def __init__(self, config:AbdiConfig=None, b:Blackboard=None, d:HolonicDesire=None, i: HolonicIntention=None):
         b = b or Blackboard()
         d = d or HolonicDesire()
         i = i or HolonicIntention()
         super().__init__(b, d, i)
         
@@ -292,22 +287,26 @@
             
             
     def on_connected(self):
         pass
 
 
     @final
-    def _on_message(self, topic:str, payload):
-        # logger.debug(f"topic: {topic}, payload: {payload}")
+    def _on_message(self, topic:str, payload, payload_info=None):
         if topic in self._topic_handlers:
-            # logger.debug(f"topic in self._topic_handlers")
-            self._topic_handlers[topic](topic, payload)
+            topic_handler = self._topic_handlers[topic]
+            if len(inspect.signature(topic_handler).parameters) == 2:
+                self._topic_handlers[topic](topic, payload)
+            else:
+                self._topic_handlers[topic](topic, payload, payload_info)
         else:
-            # logger.debug(f"on_message")
-            self.on_message(topic, payload)
+            if len(inspect.signature(self.on_message).parameters) == 2:
+                self.on_message(topic, payload)
+            else:
+                self.on_message(topic, payload, payload_info)
         
         
     # def _process_message(self, topic:str, payload):
     #     logger.debug(f"payload: {len(payload)}")
     #     if payload and self._request_logistic.is_request(payload):
     #         logger.debug("message is_request")
     #         threading.Thread(target=self._on_request, args=(topic, payload)).start()
@@ -319,15 +318,15 @@
     #         logger.debug(f"unmanaged payload")
     #         if topic in self._topic_handlers:
     #             self._topic_handlers[topic](topic, payload)
     #         else:
     #             self.on_message(topic, payload)
 
 
-    def on_message(self, topic:str, payload):
+    def on_message(self, topic:str, payload, payload_info=None):
         pass
 
 
 
 # ==================================
 #  Others operation 
 # ==================================
```

### Comparing `agent-bdi-2.3.6/src/holon/logistics/base_logistic.py` & `agent-bdi-2.4.0/src/holon/logistics/base_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/holon/logistics/loading_coordinator.py` & `agent-bdi-2.4.0/src/holon/logistics/loading_coordinator.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/src/holon/logistics/payload_wrapper.py` & `agent-bdi-2.4.0/src/holon/logistics/payload_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import pickle
+import uuid
 
 from abdi_config import LOGGER_NAME
 
 logger = logging.getLogger(LOGGER_NAME)
 VERSION = "0001"
 VERSION_BYTES = VERSION.encode('utf-8')
 # WRAPPER_HEAD = "950f7f7ba7c111eea5c4ff9ca9F3fcfd"
@@ -22,26 +23,28 @@
         self.agent_id = agent_id
         
         
     def create_response_json(self, response_payload, request_payload):
         response_json = {
             "version": VERSION,
             "request_id": request_payload["request_id"],
-            "receiver": request_payload["sender"]
+            "receiver": request_payload["sender"],
+            "request_token": request_payload["request_token"]
         }
         response_json["content"] = response_payload
         
         return response_json
         
         
     def create_request_json(self, payload, request_id):
         request_json = {
             "version": VERSION,
             "request_id": request_id,
-            "sender": self.agent_id
+            "sender": self.agent_id,
+            "request_token": str(uuid.uuid4()).replace("-", "")
         }
         request_json["content"] = payload
         
         return request_json
         
 
     def get_payload_wrapper(self, payload):
@@ -95,19 +98,19 @@
 
         return payload_resp
 
 
     def wrap_for_request(self, payload, request_id) -> str:
         wrapper = self.get_payload_wrapper(payload)
         if wrapper:
-            payload_resp = wrapper.wrap_for_request(payload, request_id)
+            payload_request, request_token = wrapper.wrap_for_request(payload, request_id)
         else:
             raise Exception("Unsupported payload type.")
 
-        return payload_resp
+        return payload_request, request_token
 
 
 
 class BinaryWrapper:
     def __init__(self, payload_wrapper:PayloadWrapper):
         self.payload_wrapper = payload_wrapper
         
@@ -126,15 +129,15 @@
         return payload_json
 
 
     def wrap_for_request(self, payload, request_id) -> bytes:
         request_json = self.payload_wrapper.create_request_json(payload, request_id)
         request_payload = WRAPPER_REQUEST_HEAD_BYTES + pickle.dumps(request_json)
         
-        return request_payload
+        return request_payload, request_json['request_token']
      
         
     def wrap_for_response(self, response_payload:bytes, managed_request_payload) -> bytes:
         response_json = self.payload_wrapper.create_response_json(response_payload, managed_request_payload)
         response_payload = WRAPPER_RESPONSE_HEAD_BYTES + pickle.dumps(response_json)
         
         return response_payload
@@ -157,28 +160,26 @@
                 acceptable = False
             
         return acceptable
 
         
     def unpack(self, payload:str):
         payload_text = payload.decode('utf-8')
-        # logger.debug(f"payload_text: {payload_text}")
         payload_json = json.loads(payload_text[len(WRAPPER_REQUEST_HEAD):])
         logger.debug(f"payload_json: {str(payload_json)[:300]}...")
         if VERSION != payload_json["version"]:
             raise Exception("Invalid payload version.")
         return payload_json
 
 
     def wrap_for_request(self, payload, request_id) -> str:
         request_json = self.payload_wrapper.create_request_json(payload, request_id)
-        # print(f"request_json: {request_json}")
         request_payload = f"{WRAPPER_REQUEST_HEAD}{json.dumps(request_json)}"
         
-        return request_payload
+        return request_payload, request_json['request_token']
                 
         
     def wrap_for_response(self, response_payload:str, managed_request_payload) -> str:
         response_json = self.payload_wrapper.create_response_json(response_payload, managed_request_payload)
         response_payload = f"{WRAPPER_RESPONSE_HEAD}{json.dumps(response_json)}"
         
         return response_payload
```

### Comparing `agent-bdi-2.3.6/src/holon/logistics/request_logistic.py` & `agent-bdi-2.4.0/src/holon/logistics/request_logistic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import uuid
 
 from abdi_config import LOGGER_NAME
 from holon.HolonicAgent import HolonicAgent
 from holon.logistics.base_logistic import BaseLogistic
 from holon.logistics.payload_wrapper import PayloadWrapper
 
 
@@ -23,18 +22,20 @@
         logger.debug(f"self, agent_id: {self.agent.agent_id}, short_id: {self.agent.short_id}, request_id: {self.request_id}")
         self._payload_wrapper = PayloadWrapper(self.agent.agent_id)
         
         
     def publish(self, topic, payload):
         logistic_topic = f"{PUBLISH_HEADER}.{topic}"
         logger.debug(f"agent_id: {self.agent.agent_id}, request_id: {self.request_id}")
-        packed_payload = self._payload_wrapper.wrap_for_request(payload, self.request_id)
+        packed_payload, request_token = self._payload_wrapper.wrap_for_request(payload, self.request_id)
         # logistic_topic, packed_payload = self.pack(topic, payload)
         logger.debug(f"logistic_topic: {logistic_topic}, packed_payload: {str(packed_payload)[:300]}")
         self.agent.publish(logistic_topic, packed_payload)
+        
+        return request_token
 
 
     def subscribe(self, topic, topic_handler=None, datatype="str"):
         response_topic = f"{self.response_topic_header}.{topic}"
         self.agent.subscribe(response_topic, datatype, self.handle_response)
         RequestLogistic.__handlers[self.response_topic_header] = topic_handler
 
@@ -42,15 +43,15 @@
     def handle_response(self, topic:str, payload):
         responsed_topic = topic[len(self.response_topic_header)+1:]
         unpacked = self._payload_wrapper.unpack(payload)
         logger.debug(f"topic: {topic}, unpacked: {str(unpacked)[:300]}")
 
         if topic_handler := RequestLogistic.__handlers[self.response_topic_header]:
             self.agent.set_topic_handler(responsed_topic, topic_handler)
-        self.agent._on_message(responsed_topic, unpacked["content"])
+        self.agent._on_message(responsed_topic, unpacked["content"], payload_info=unpacked["request_token"])
 
 
     # def handle_response(self, topic:str, payload):
     #     responsed_topic = topic[len(self.response_topic_header)+1:]
     #     # unpacked = self.unpack(payload)
     #     unpacked = self._payload_wrapper.unpack(payload)
     #     if unpacked["receiver"] == self.agent.agent_id:
```

### Comparing `agent-bdi-2.3.6/src/holon/logistics/response_logistic.py` & `agent-bdi-2.4.0/src/holon/logistics/response_logistic.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/tests/test01.py` & `agent-bdi-2.4.0/tests/test01.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/tests/test_loadingbal.py` & `agent-bdi-2.4.0/tests/test_loadingbal.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/tests/test_request.py` & `agent-bdi-2.4.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `agent-bdi-2.3.6/tests/test_send.py` & `agent-bdi-2.4.0/tests/test_send.py`

 * *Files identical despite different names*

