# Comparing `tmp/alibabacloud_eventbridge20200401_py2-3.0.0.tar.gz` & `tmp/alibabacloud_eventbridge20200401_py2-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eventbridge20200401_py2-3.0.0.tar", last modified: Thu Mar 14 10:10:53 2024, max compression
+gzip compressed data, was "dist/alibabacloud_eventbridge20200401_py2-3.0.1.tar", last modified: Tue Apr  9 17:13:27 2024, max compression
```

## Comparing `alibabacloud_eventbridge20200401_py2-3.0.0.tar` & `alibabacloud_eventbridge20200401_py2-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      747 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84239 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401/client.py
--rw-r--r--   0 root         (0) root         (0)   979045 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 10:10:53.000000 alibabacloud_eventbridge20200401_py2-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2943 2024-03-14 10:10:52.000000 alibabacloud_eventbridge20200401_py2-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1436 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84357 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401/client.py
+-rw-r--r--   0 root         (0) root         (0)   982442 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-09 17:13:27.000000 alibabacloud_eventbridge20200401_py2-3.0.1/setup.py
```

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/ChangeLog.md` & `alibabacloud_eventbridge20200401_py2-3.0.1/ChangeLog.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+2024-03-14 Version: 3.0.0
+- Update API CreateEventStreaming: update param Sink.
+- Update API CreateEventStreaming: update param Source.
+- Update API CreateRule: update param EventTargets.
+- Update API DeleteEventStreaming: update response param.
+- Update API DisableRule: update response param.
+- Update API EnableRule: update response param.
+- Update API GetEventStreaming: update response param.
+- Update API ListUserDefinedEventSources: update response param.
+- Update API PauseEventStreaming: update response param.
+- Update API StartEventStreaming: update response param.
+- Update API UpdateEventStreaming: update param Sink.
+- Update API UpdateEventStreaming: update param Source.
+
+
 2024-02-28 Version: 2.0.0
 - Update API CreateEventStreaming: update param Sink.
 - Update API CreateEventStreaming: update param Source.
 - Update API DisableRule: update response param.
 - Update API EnableRule: update response param.
 - Update API GetEventStreaming: update response param.
 - Update API ListUserDefinedEventSources: update response param.
```

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/LICENSE` & `alibabacloud_eventbridge20200401_py2-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/PKG-INFO` & `alibabacloud_eventbridge20200401_py2-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eventbridge20200401_py2
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/README-CN.md` & `alibabacloud_eventbridge20200401_py2-3.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/README.md` & `alibabacloud_eventbridge20200401_py2-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401/client.py` & `alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401/client.py`

 * *Files identical despite different names*

```diff
@@ -593,14 +593,16 @@
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteEventSourceResponse
         """
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.event_bus_name):
+            body['EventBusName'] = request.event_bus_name
         if not UtilClient.is_unset(request.event_source_name):
             body['EventSourceName'] = request.event_source_name
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteEventSource',
```

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401/models.py` & `alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5182,18 +5182,19 @@
             self.region_id = m.get('RegionId')
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
 class CreateEventStreamingRequestSourceSourcePrometheusParameters(TeaModel):
-    def __init__(self, cluster_id=None, data_type=None, labels=None):
+    def __init__(self, cluster_id=None, data_type=None, labels=None, region_id=None):
         self.cluster_id = cluster_id  # type: str
         self.data_type = data_type  # type: str
         self.labels = labels  # type: str
+        self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateEventStreamingRequestSourceSourcePrometheusParameters, self).to_map()
         if _map is not None:
@@ -5202,24 +5203,28 @@
         result = dict()
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
         if self.data_type is not None:
             result['DataType'] = self.data_type
         if self.labels is not None:
             result['Labels'] = self.labels
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         if m.get('DataType') is not None:
             self.data_type = m.get('DataType')
         if m.get('Labels') is not None:
             self.labels = m.get('Labels')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
         return self
 
 
 class CreateEventStreamingRequestSourceSourceRabbitMQParameters(TeaModel):
     def __init__(self, instance_id=None, queue_name=None, region_id=None, virtual_host_name=None):
         # The ID of the Message Queue for RabbitMQ instance.
         self.instance_id = instance_id  # type: str
@@ -6237,17 +6242,18 @@
         m = m or dict()
         if m.get('ProductName') is not None:
             self.product_name = m.get('ProductName')
         return self
 
 
 class CreateServiceLinkedRoleForProductResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, success=None):
+    def __init__(self, code=None, http_code=None, message=None, request_id=None, success=None):
         # The returned response code. The value Success indicates that the request is successful. Other values indicate that the request failed. For more information about error codes, see Error codes.
         self.code = code  # type: str
+        self.http_code = http_code  # type: int
         # The returned message. If the request is successful, success is returned.
         self.message = message  # type: str
         # The request ID.
         self.request_id = request_id  # type: str
         # Indicates whether the request is successful. Valid values: true and false.
         self.success = success  # type: bool
 
@@ -6258,26 +6264,30 @@
         _map = super(CreateServiceLinkedRoleForProductResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.http_code is not None:
+            result['HttpCode'] = self.http_code
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.success is not None:
             result['Success'] = self.success
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('HttpCode') is not None:
+            self.http_code = m.get('HttpCode')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
@@ -6616,33 +6626,38 @@
         if m.get('body') is not None:
             temp_model = DeleteEventBusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteEventSourceRequest(TeaModel):
-    def __init__(self, event_source_name=None):
+    def __init__(self, event_bus_name=None, event_source_name=None):
+        self.event_bus_name = event_bus_name  # type: str
         # The name of the event source.
         self.event_source_name = event_source_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteEventSourceRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.event_bus_name is not None:
+            result['EventBusName'] = self.event_bus_name
         if self.event_source_name is not None:
             result['EventSourceName'] = self.event_source_name
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('EventBusName') is not None:
+            self.event_bus_name = m.get('EventBusName')
         if m.get('EventSourceName') is not None:
             self.event_source_name = m.get('EventSourceName')
         return self
 
 
 class DeleteEventSourceResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, success=None):
@@ -10718,18 +10733,19 @@
             self.region_id = m.get('RegionId')
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
 class GetEventStreamingResponseBodyDataSourceSourcePrometheusParameters(TeaModel):
-    def __init__(self, cluster_id=None, data_type=None, labels=None):
+    def __init__(self, cluster_id=None, data_type=None, labels=None, region_id=None):
         self.cluster_id = cluster_id  # type: str
         self.data_type = data_type  # type: str
         self.labels = labels  # type: str
+        self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetEventStreamingResponseBodyDataSourceSourcePrometheusParameters, self).to_map()
         if _map is not None:
@@ -10738,24 +10754,28 @@
         result = dict()
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
         if self.data_type is not None:
             result['DataType'] = self.data_type
         if self.labels is not None:
             result['Labels'] = self.labels
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         if m.get('DataType') is not None:
             self.data_type = m.get('DataType')
         if m.get('Labels') is not None:
             self.labels = m.get('Labels')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
         return self
 
 
 class GetEventStreamingResponseBodyDataSourceSourceRabbitMQParameters(TeaModel):
     def __init__(self, instance_id=None, queue_name=None, region_id=None, virtual_host_name=None):
         # The ID of the Message Queue for RabbitMQ instance.
         self.instance_id = instance_id  # type: str
@@ -15358,14 +15378,53 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
+class ListEventStreamingsResponseBodyDataEventStreamingsSourceSourcePrometheusParameters(TeaModel):
+    def __init__(self, cluster_id=None, data_type=None, labels=None, region_id=None):
+        self.cluster_id = cluster_id  # type: str
+        self.data_type = data_type  # type: str
+        self.labels = labels  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListEventStreamingsResponseBodyDataEventStreamingsSourceSourcePrometheusParameters, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.data_type is not None:
+            result['DataType'] = self.data_type
+        if self.labels is not None:
+            result['Labels'] = self.labels
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('DataType') is not None:
+            self.data_type = m.get('DataType')
+        if m.get('Labels') is not None:
+            self.labels = m.get('Labels')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
 class ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRabbitMQParameters(TeaModel):
     def __init__(self, instance_id=None, queue_name=None, region_id=None, virtual_host_name=None):
         # The ID of the Message Queue for RabbitMQ instance.
         self.instance_id = instance_id  # type: str
         # The name of the queue on the Message Queue for RabbitMQ instance.
         self.queue_name = queue_name  # type: str
         # The ID of the region where the Message Queue for RabbitMQ instance resides.
@@ -15573,24 +15632,25 @@
         if m.get('RoleName') is not None:
             self.role_name = m.get('RoleName')
         return self
 
 
 class ListEventStreamingsResponseBodyDataEventStreamingsSource(TeaModel):
     def __init__(self, source_dtsparameters=None, source_kafka_parameters=None, source_mnsparameters=None,
-                 source_mqttparameters=None, source_rabbit_mqparameters=None, source_rocket_mqparameters=None,
-                 source_slsparameters=None):
+                 source_mqttparameters=None, source_prometheus_parameters=None, source_rabbit_mqparameters=None,
+                 source_rocket_mqparameters=None, source_slsparameters=None):
         # The parameters that are returned if Data Transmission Service (DTS) is specified as the event source.
         self.source_dtsparameters = source_dtsparameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceDTSParameters
         # The parameters that are returned if Message Queue for Apache Kafka is specified as the event source.
         self.source_kafka_parameters = source_kafka_parameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceKafkaParameters
         # The parameters that are returned if Message Service (MNS) is specified as the event source.
         self.source_mnsparameters = source_mnsparameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceMNSParameters
         # The parameters that are returned if Message Queue for MQTT is specified as the event source.
         self.source_mqttparameters = source_mqttparameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceMQTTParameters
+        self.source_prometheus_parameters = source_prometheus_parameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourcePrometheusParameters
         # The parameters that are returned if Message Queue for RabbitMQ is specified as the event source.
         self.source_rabbit_mqparameters = source_rabbit_mqparameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRabbitMQParameters
         # Source RocketMQ Parameters
         self.source_rocket_mqparameters = source_rocket_mqparameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRocketMQParameters
         # The parameters that are returned if Log Service is specified as the event source.
         self.source_slsparameters = source_slsparameters  # type: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceSLSParameters
 
@@ -15599,14 +15659,16 @@
             self.source_dtsparameters.validate()
         if self.source_kafka_parameters:
             self.source_kafka_parameters.validate()
         if self.source_mnsparameters:
             self.source_mnsparameters.validate()
         if self.source_mqttparameters:
             self.source_mqttparameters.validate()
+        if self.source_prometheus_parameters:
+            self.source_prometheus_parameters.validate()
         if self.source_rabbit_mqparameters:
             self.source_rabbit_mqparameters.validate()
         if self.source_rocket_mqparameters:
             self.source_rocket_mqparameters.validate()
         if self.source_slsparameters:
             self.source_slsparameters.validate()
 
@@ -15620,14 +15682,16 @@
             result['SourceDTSParameters'] = self.source_dtsparameters.to_map()
         if self.source_kafka_parameters is not None:
             result['SourceKafkaParameters'] = self.source_kafka_parameters.to_map()
         if self.source_mnsparameters is not None:
             result['SourceMNSParameters'] = self.source_mnsparameters.to_map()
         if self.source_mqttparameters is not None:
             result['SourceMQTTParameters'] = self.source_mqttparameters.to_map()
+        if self.source_prometheus_parameters is not None:
+            result['SourcePrometheusParameters'] = self.source_prometheus_parameters.to_map()
         if self.source_rabbit_mqparameters is not None:
             result['SourceRabbitMQParameters'] = self.source_rabbit_mqparameters.to_map()
         if self.source_rocket_mqparameters is not None:
             result['SourceRocketMQParameters'] = self.source_rocket_mqparameters.to_map()
         if self.source_slsparameters is not None:
             result['SourceSLSParameters'] = self.source_slsparameters.to_map()
         return result
@@ -15642,14 +15706,17 @@
             self.source_kafka_parameters = temp_model.from_map(m['SourceKafkaParameters'])
         if m.get('SourceMNSParameters') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceMNSParameters()
             self.source_mnsparameters = temp_model.from_map(m['SourceMNSParameters'])
         if m.get('SourceMQTTParameters') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceMQTTParameters()
             self.source_mqttparameters = temp_model.from_map(m['SourceMQTTParameters'])
+        if m.get('SourcePrometheusParameters') is not None:
+            temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSourceSourcePrometheusParameters()
+            self.source_prometheus_parameters = temp_model.from_map(m['SourcePrometheusParameters'])
         if m.get('SourceRabbitMQParameters') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRabbitMQParameters()
             self.source_rabbit_mqparameters = temp_model.from_map(m['SourceRabbitMQParameters'])
         if m.get('SourceRocketMQParameters') is not None:
             temp_model = ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRocketMQParameters()
             self.source_rocket_mqparameters = temp_model.from_map(m['SourceRocketMQParameters'])
         if m.get('SourceSLSParameters') is not None:
@@ -23160,18 +23227,19 @@
             self.region_id = m.get('RegionId')
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
 class UpdateEventStreamingRequestSourceSourcePrometheusParameters(TeaModel):
-    def __init__(self, cluster_id=None, data_type=None, labels=None):
+    def __init__(self, cluster_id=None, data_type=None, labels=None, region_id=None):
         self.cluster_id = cluster_id  # type: str
         self.data_type = data_type  # type: str
         self.labels = labels  # type: str
+        self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateEventStreamingRequestSourceSourcePrometheusParameters, self).to_map()
         if _map is not None:
@@ -23180,24 +23248,28 @@
         result = dict()
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
         if self.data_type is not None:
             result['DataType'] = self.data_type
         if self.labels is not None:
             result['Labels'] = self.labels
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         if m.get('DataType') is not None:
             self.data_type = m.get('DataType')
         if m.get('Labels') is not None:
             self.labels = m.get('Labels')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
         return self
 
 
 class UpdateEventStreamingRequestSourceSourceRabbitMQParameters(TeaModel):
     def __init__(self, instance_id=None, queue_name=None, region_id=None, virtual_host_name=None):
         # The ID of the Message Queue for RabbitMQ instance.
         self.instance_id = instance_id  # type: str
```

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/alibabacloud_eventbridge20200401_py2.egg-info/PKG-INFO` & `alibabacloud_eventbridge20200401_py2-3.0.1/alibabacloud_eventbridge20200401_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eventbridge20200401-py2
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401_py2-3.0.0/setup.py` & `alibabacloud_eventbridge20200401_py2-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eventbridge20200401_py2.
 
-Created on 14/03/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eventbridge20200401"
 NAME = "alibabacloud_eventbridge20200401_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eventbridge (20200401) SDK Library for Python2"
```

