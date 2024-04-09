# Comparing `tmp/butler-connect-0.8.5.tar.gz` & `tmp/butler-connect-0.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.8.5.tar", last modified: Thu Feb  1 08:53:10 2024, max compression
+gzip compressed data, was "butler-connect-0.9.0b0.tar", last modified: Tue Apr  9 11:18:14 2024, max compression
```

## Comparing `butler-connect-0.8.5.tar` & `butler-connect-0.9.0b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 08:53:10.508324 butler-connect-0.8.5/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.8.5/LICENSE
--rw-rw-rw-   0        0        0     3670 2024-02-01 08:53:10.507373 butler-connect-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     1573 2024-02-01 08:52:39.000000 butler-connect-0.8.5/README.md
--rw-rw-rw-   0        0        0      738 2024-02-01 08:50:48.000000 butler-connect-0.8.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-01 08:53:10.508324 butler-connect-0.8.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-01 08:53:10.463881 butler-connect-0.8.5/src/
-drwxrwxrwx   0        0        0        0 2024-02-01 08:53:10.466866 butler-connect-0.8.5/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.8.5/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18875 2023-12-29 13:47:52.000000 butler-connect-0.8.5/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2024-02-01 08:53:10.480931 butler-connect-0.8.5/src/butlerDescription/
--rw-rw-rw-   0        0        0      229 2023-11-22 09:46:59.000000 butler-connect-0.8.5/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.8.5/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.8.5/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0     1411 2024-02-01 08:52:12.000000 butler-connect-0.8.5/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     3238 2024-02-01 08:51:24.000000 butler-connect-0.8.5/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2024-02-01 08:53:10.506323 butler-connect-0.8.5/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     3670 2024-02-01 08:53:10.000000 butler-connect-0.8.5/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-02-01 08:53:10.000000 butler-connect-0.8.5/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 08:53:10.000000 butler-connect-0.8.5/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-02-01 08:53:10.000000 butler-connect-0.8.5/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2024-02-01 08:53:10.000000 butler-connect-0.8.5/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.616445 butler-connect-0.9.0b0/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.9.0b0/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-09 11:18:14.615446 butler-connect-0.9.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1759 2024-04-09 11:18:02.000000 butler-connect-0.9.0b0/README.md
+-rw-rw-rw-   0        0        0      743 2024-04-09 10:28:26.000000 butler-connect-0.9.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 11:18:14.616445 butler-connect-0.9.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.588840 butler-connect-0.9.0b0/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.590840 butler-connect-0.9.0b0/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.9.0b0/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    20896 2024-04-09 11:17:10.000000 butler-connect-0.9.0b0/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.593840 butler-connect-0.9.0b0/src/butlerDescription/
+-rw-rw-rw-   0        0        0      229 2023-11-22 09:46:59.000000 butler-connect-0.9.0b0/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.9.0b0/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.9.0b0/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0     1411 2024-02-01 08:52:12.000000 butler-connect-0.9.0b0/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     3238 2024-02-01 08:51:24.000000 butler-connect-0.9.0b0/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.614434 butler-connect-0.9.0b0/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.8.5/LICENSE` & `butler-connect-0.9.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.8.5/PKG-INFO` & `butler-connect-0.9.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.8.5
+Version: 0.9.0b0
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -91,7 +91,12 @@
 - add GroupOptionType_labels to __init__
 ### 0.8.3
 - bugfix in GroupOptionType.agent.building
 ### 0.8.4
 - bugfix automatic destory of connection on BasicBrokerThreadingConnection on class destroy
 ### 0.8.5
 - add heating_sub_system to signal and group
+### 0.9.0
+- add some internal functions to pikaButler for mor stability
+- better loghandling in pikaBulter with the gobale Vars': 
+-- logInfoMessages = False
+-- logInfoConnection = True
```

### Comparing `butler-connect-0.8.5/README.md` & `butler-connect-0.9.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,8 +46,13 @@
 ### 0.8.2
 - add GroupOptionType_labels to __init__
 ### 0.8.3
 - bugfix in GroupOptionType.agent.building
 ### 0.8.4
 - bugfix automatic destory of connection on BasicBrokerThreadingConnection on class destroy
 ### 0.8.5
-- add heating_sub_system to signal and group
+- add heating_sub_system to signal and group
+### 0.9.0
+- add some internal functions to pikaButler for mor stability
+- better loghandling in pikaBulter with the gobale Vars': 
+-- logInfoMessages = False
+-- logInfoConnection = True
```

### Comparing `butler-connect-0.8.5/src/butlerConnect/pikaButler.py` & `butler-connect-0.9.0b0/src/butlerConnect/pikaButler.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 import threading
 
 import ssl
 
 default_heartbeat = 600
 default_blocked_connection_timeout = 300
 
+logInfoMessages = False
+logInfoConnection = True
+
+MAX_RECONNECT_ATTEMPTS = 5  # Maximale Anzahl von Wiederverbindungsversuchen
+MAX_RECONNECT_DELAY = 32  # Maximale Verzögerung in Sekunden (2^5 = 32)
+
 class BasicPikaConnection(object):
     EXCHANGE_TYPE = ExchangeType.fanout
     def __init__(self,host,port,user,password,connectionName,callbackData,callbackControl,component,ssl_activate=False,ca_certificate=None,client_certificate=None,client_key=None,certificate_password='',virtual_host='/'):
         self.virtual_host = virtual_host
         self.ssl_activate = ssl_activate
         
         self.ca_certificate = ca_certificate
@@ -39,54 +45,71 @@
         self._channelPublish = None
         # In production, experiment with higher prefetch values
         # for higher consumer throughput
         self.consumerRun = False
         self.publisherRun = False
         self.reconnectingTimeout = 10.0
         self.queSendData = queue.Queue()
+        self.queSize = 250
+    def __enter__(self):
+        # Initialisieren Sie Verbindungen und Ressourcen
+        return self
+    
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        # Bereinigen Sie alle Verbindungen und Ressourcen
+        self.stop()
 
     def bindExchangeConsumer(self,exchange,callback):
         queue_name =  f'{self.connectionName}_{exchange}'
         result = self._channelConsumer.queue_declare(queue=queue_name, exclusive=False)
         self._channelConsumer.exchange_declare(exchange=exchange,  exchange_type='fanout')
         self._channelConsumer.queue_bind(exchange=exchange, queue=queue_name)
         self._channelConsumer.basic_consume(queue=queue_name,
                             auto_ack=True,
                             on_message_callback=callback)
     
     def publish(self,topic,msg):
-        LOG.info(f'{topic}=>{msg}')
+        if logInfoMessages:
+            LOG.info(f'{topic}=>{msg}')
+        if self.queSendData.qsize() > self.queSize:
+            LOG.error(f'Queue is full. Skip message {topic}=>{msg} [size={self.queSendData.qsize()}]')
+            raise Exception('Queue is full')
+            
         self.queSendData.put_nowait({topic:msg})
     
     def publishData(self,msg):
         topic = f'component.{self.component}.data.input'
         self.publish(topic=topic,msg=msg)
 
     def publishControl(self,msg):
         topic = f'component.{self.component}.control.input'
         self.publish(topic=topic,msg=msg)
             
-            
-    
     def startPublisher(self):
-        # Bestimmte Fehlerbeahndlung not notwendig
         self.publisherRun = True
-        while self.publisherRun :
+        reconnect_attempts = 0
+        while self.publisherRun:
             try:
                 self.runPublisher()
+                reconnect_attempts = 0  # Reset reconnect attempts after successful connection
             except (pika.exceptions.IncompatibleProtocolError, pika.exceptions.StreamLostError):
-                desc = f'Loosing Connection from {self.host}:{self.port}'
-                LOG.warning(desc)
+                LOG.warning(f'Loosing Connection from {self.host}:{self.port}')
+                reconnect_attempts += 1
             except Exception as e:
                 if self.publisherRun:
-                    desc = f'Exception Connection from {self.host}:{self.port} '
-                    LOG.exception(desc)
-                #self.publisherRun = False
-            time.sleep(self.reconnectingTimeout )
-            LOG.info(f'Try to reconnect!')
+                    LOG.exception(f'Exception Connection from {self.host}:{self.port}')
+                reconnect_attempts += 1
+
+            if self.publisherRun and reconnect_attempts < MAX_RECONNECT_ATTEMPTS:
+                wait_time = min(2 ** reconnect_attempts, MAX_RECONNECT_DELAY)
+                LOG.info(f'Attempting to reconnect in {wait_time} seconds...')
+                time.sleep(wait_time)
+            elif reconnect_attempts >= MAX_RECONNECT_ATTEMPTS:
+                LOG.error('Max reconnect attempts reached, handling as needed...')
+                break  # or other error handling
         
     def getSSLOptions(self):
         try:
             ca_certificate = os.path.abspath(self.ca_certificate)
             client_certificate = os.path.abspath(self.client_certificate)
             client_key = os.path.abspath(self.client_key)
             context = ssl.create_default_context(cafile=ca_certificate)
@@ -102,29 +125,31 @@
     def ConnectionParameters(self):
         if self.ssl_activate:
             return pika.ConnectionParameters(host=self.host,port=self.port,credentials=self.credentials,ssl_options=self.getSSLOptions(),heartbeat=default_heartbeat,blocked_connection_timeout=default_blocked_connection_timeout,virtual_host=self.virtual_host)
         else:
             return pika.ConnectionParameters(host=self.host,port=self.port,credentials=self.credentials,heartbeat=default_heartbeat,blocked_connection_timeout=default_blocked_connection_timeout,virtual_host=self.virtual_host)
     
     def runPublisher(self):
-        LOG.info(f'Create pika Publish-Connection with: host={self.host}, post={self.port}')
+        if logInfoConnection:
+            LOG.info(f'Create pika Publish-Connection with: host={self.host}, post={self.port}')
         self._connectionPublisher = pika.BlockingConnection(self.ConnectionParameters())
         self._channelPublish = self._connectionPublisher.channel()
         self._channelPublish.confirm_delivery()
         
         while self.publisherRun :
             try:
                 item = self.queSendData.get(block=True,timeout=default_heartbeat/2)
             except queue.Empty:
                 item = {}
             if item != {}:
                 try:
                     for topic in item.keys():
                         msg = item[topic]
-                        LOG.info(f'publish data {topic}@{msg}')
+                        if logInfoMessages:
+                            LOG.info(f'publish data {topic}@{msg}')
                         try:
                             self._channelPublish .basic_publish(exchange=topic,
                                     routing_key='',
                                     body=msg,properties=pika.BasicProperties(content_type='text/plain',
                                                           delivery_mode=pika.DeliveryMode.Transient),
                                     mandatory=True)
                         except (pika.exceptions.UnroutableError, pika.exceptions.ChannelClosedByBroker) as e:
@@ -135,50 +160,59 @@
                 except Exception as e:
                     self.que.put(item)
                     raise e
             # sending heartbeat
             else:
                 # do a pika heartbeat
                 self._connectionPublisher.process_data_events(time_limit=0.1) 
-     
-                
+        
     def runConsumer(self):
-        LOG.info(f'Create pika Consumer-Connection with: host={self.host}, post={self.port}')
+        if logInfoConnection:
+            LOG.info(f'Create pika Consumer-Connection with: host={self.host}, post={self.port}')
         self._connectionConsumer = pika.BlockingConnection(self.ConnectionParameters())
         self._channelConsumer = self._connectionConsumer.channel()
         topicData = f'component.{self.component}.data.output'
         topicControl = f'component.{self.component}.control.output'
         self.bindExchangeConsumer(exchange=topicData,callback=self.callbackData)
         self.bindExchangeConsumer(exchange=topicControl,callback=self.callbackControl)
-        LOG.info('self._channel.start_consuming()')
+        if logInfoConnection:
+            LOG.info('self._channel.start_consuming()')
         self._channelConsumer.start_consuming()
         
-
     def startConsumer(self):
         self.consumerRun = True
-        while self.consumerRun :
+        reconnect_attempts = 0
+        while self.consumerRun:
             try:
                 self.runConsumer()
+                reconnect_attempts = 0
             except (pika.exceptions.IncompatibleProtocolError, pika.exceptions.StreamLostError):
-                desc = f'Loosing Connection from {self.host}:{self.port}'
-                LOG.warning(desc)
+                LOG.warning(f'Loosing Connection from {self.host}:{self.port}')
+                reconnect_attempts += 1
             except Exception as e:
                 if self.consumerRun:
-                    desc = f'Exception Connection from {self.host}:{self.port}'
-                    LOG.exception(desc)
-                #self.consumerRun = False
-            time.sleep(self.reconnectingTimeout )
-            LOG.info(f'Try to reconnect!')
-        
-        
+                    LOG.exception(f'Exception Connection from {self.host}:{self.port}')
+                reconnect_attempts += 1
+
+            if self.consumerRun and reconnect_attempts < MAX_RECONNECT_ATTEMPTS:
+                wait_time = min(2 ** reconnect_attempts, MAX_RECONNECT_DELAY)
+                LOG.info(f'Attempting to reconnect in {wait_time} seconds...')
+                time.sleep(wait_time)
+            elif reconnect_attempts >= MAX_RECONNECT_ATTEMPTS:
+                LOG.error('Max reconnect attempts reached, handling as needed...')
+                break  # or other error handling
+             
     def stop(self):
         self.consumerRun = False
         self.publisherRun = False
         self._channelConsumer.stop_consuming()
-        pass
+        if self._connectionConsumer:
+            self._connectionConsumer.close()
+        if self._connectionPublisher:
+            self._connectionPublisher.close()
         
         
 def basicConsumerCallback(ch, method, properties, body):
         pass
       
     
 class basicConnection(object):
@@ -210,30 +244,32 @@
                 LOG.warning(f'Loosing connection. Do a reset!')
             except Exception as e:
                 if self.isRunning:
                     desc = f'Exception Connection from {self.topic}@{self.connectionParameter}'
                     LOG.exception(desc)
             if self.isRunning:
                 time.sleep(self.reconnectingTimeout )
-                LOG.info(f'Try to reconnect!')
+                if logInfoConnection:
+                    LOG.info(f'Try to reconnect!')
     
     def run(self):
         pass
 
 class basicConsumer(basicConnection):
     def __init__(self,connectionName,topic,callback,connectionParameter:pika.ConnectionParameters=None,createExchangeIfNotExists=False,exclusive=False,createExchangeType:ExchangeType=ExchangeType.fanout,routing_key=None,reconnectingCallback=None) -> None:
         super().__init__(connectionName=connectionName,topic=topic,callback=callback,connectionParameter=connectionParameter)
         self.createExchangeIfNotExists = createExchangeIfNotExists
         self.createExchangeType = createExchangeType
         self.exclusive = exclusive
         self.routing_key = routing_key
         self.reconnectingCallback = reconnectingCallback
     
     def run(self):
-        LOG.info(f'Create pika Consumer-Connection for {self.topic} with: {self.connectionParameter}')
+        if logInfoConnection:
+            LOG.info(f'Create pika Consumer-Connection for {self.topic} with: {self.connectionParameter}')
         self.connection = pika.BlockingConnection(self.connectionParameter)
         self.channel = self.connection.channel()
         
         
         queue_name =  f'{self.connectionName}' #_consume_{self.topic}'
         if self.routing_key is not None:
             queue_name = f'{queue_name}_{self.routing_key}'
@@ -268,15 +304,16 @@
     def __init__(self,connectionName,connectionParameter:pika.ConnectionParameters=None) -> None:
         super().__init__(connectionName=connectionName,connectionParameter=connectionParameter)
         self.que = queue.Queue()
         self.connection = None
         self.channel = None
         self.throwUnroutableError = False
     def run(self):
-        LOG.info(f'Create pika Publish-Connection with: {self.connectionParameter}')
+        if logInfoConnection:
+            LOG.info(f'Create pika Publish-Connection with: {self.connectionParameter}')
         self.connection = pika.BlockingConnection(self.connectionParameter)
         self.channel:pika.adapters.blocking_connection.BlockingChannel = self.connection.channel()
         self.channel.confirm_delivery()
         
         while self.isRunning :
             try:
                 item = self.que.get(block=True,timeout=default_heartbeat/4)
@@ -285,15 +322,16 @@
             if item != {}:
                 try:
                     for topic in item.keys():
                         d = item[topic]
                         msg = d.get('msg')
                         routing_key = d.get('routing_key',None)
                         if routing_key == None: routing_key = ''
-                        LOG.info(f'publish data {topic}@{msg}')
+                        if logInfoMessages:
+                            LOG.info(f'publish data {topic}@{msg}')
                         try:
                             self.channel.basic_publish(exchange=topic,
                                 routing_key=routing_key,
                                 body=msg,properties=pika.BasicProperties(content_type='text/plain',
                                                           delivery_mode=pika.DeliveryMode.Transient),
                           mandatory=True)
                         except pika.exceptions.ChannelClosedByBroker as e:
@@ -311,15 +349,16 @@
                     raise e
             else:
                 # do a pika heartbeat
                 self.connection.process_data_events(time_limit=0.1) 
 
             
     def publish(self,topic,msg,routing_key=None):
-        LOG.info(f'publish {topic}=>{msg} with routing_key={routing_key}')
+        if logInfoMessages:
+            LOG.info(f'publish {topic}=>{msg} with routing_key={routing_key}')
         self.que.put_nowait({topic:{'msg':msg,'routing_key':routing_key}})
     def stop(self):
         super().stop()   
         self.que.put({})
         #self.channel.close()
         #self.connection.close()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `butler-connect-0.8.5/src/butlerDescription/control.py` & `butler-connect-0.9.0b0/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.8.5/src/butlerDescription/group.py` & `butler-connect-0.9.0b0/src/butlerDescription/group.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.8.5/src/butlerDescription/signal.py` & `butler-connect-0.9.0b0/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.8.5/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.9.0b0/src/butler_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.8.5
+Version: 0.9.0b0
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -91,7 +91,12 @@
 - add GroupOptionType_labels to __init__
 ### 0.8.3
 - bugfix in GroupOptionType.agent.building
 ### 0.8.4
 - bugfix automatic destory of connection on BasicBrokerThreadingConnection on class destroy
 ### 0.8.5
 - add heating_sub_system to signal and group
+### 0.9.0
+- add some internal functions to pikaButler for mor stability
+- better loghandling in pikaBulter with the gobale Vars': 
+-- logInfoMessages = False
+-- logInfoConnection = True
```

