# Comparing `tmp/alibabacloud_eventbridge20200401-4.0.0.tar.gz` & `tmp/alibabacloud_eventbridge20200401-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eventbridge20200401-4.0.0.tar", last modified: Thu Mar 14 10:11:08 2024, max compression
+gzip compressed data, was "dist/alibabacloud_eventbridge20200401-4.0.1.tar", last modified: Tue Apr  9 17:14:50 2024, max compression
```

## Comparing `alibabacloud_eventbridge20200401-4.0.0.tar` & `alibabacloud_eventbridge20200401-4.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     1308 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194399 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401/client.py
--rw-r--r--   0 root         (0) root         (0)   963497 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-14 10:11:08.000000 alibabacloud_eventbridge20200401-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194635 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401/client.py
+-rw-r--r--   0 root         (0) root         (0)   966849 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:14:50.000000 alibabacloud_eventbridge20200401-4.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-09 17:14:49.000000 alibabacloud_eventbridge20200401-4.0.1/setup.py
```

### Comparing `alibabacloud_eventbridge20200401-4.0.0/LICENSE` & `alibabacloud_eventbridge20200401-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-4.0.0/PKG-INFO` & `alibabacloud_eventbridge20200401-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eventbridge20200401
-Version: 4.0.0
+Version: 4.0.1
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-4.0.0/README-CN.md` & `alibabacloud_eventbridge20200401-4.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-4.0.0/README.md` & `alibabacloud_eventbridge20200401-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401/client.py` & `alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1199,14 +1199,16 @@
         
         @param request: DeleteEventSourceRequest
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
@@ -1234,14 +1236,16 @@
         
         @param request: DeleteEventSourceRequest
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

### Comparing `alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401/models.py` & `alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5834,18 +5834,20 @@
 
 class CreateEventStreamingRequestSourceSourcePrometheusParameters(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         data_type: str = None,
         labels: str = None,
+        region_id: str = None,
     ):
         self.cluster_id = cluster_id
         self.data_type = data_type
         self.labels = labels
+        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -5854,24 +5856,28 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
@@ -7015,20 +7021,22 @@
         return self
 
 
 class CreateServiceLinkedRoleForProductResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
+        http_code: int = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         # The returned response code. The value Success indicates that the request is successful. Other values indicate that the request failed. For more information about error codes, see Error codes.
         self.code = code
+        self.http_code = http_code
         # The returned message. If the request is successful, success is returned.
         self.message = message
         # The request ID.
         self.request_id = request_id
         # Indicates whether the request is successful. Valid values: true and false.
         self.success = success
 
@@ -7039,26 +7047,30 @@
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -7444,34 +7456,40 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteEventSourceRequest(TeaModel):
     def __init__(
         self,
+        event_bus_name: str = None,
         event_source_name: str = None,
     ):
+        self.event_bus_name = event_bus_name
         # The name of the event source.
         self.event_source_name = event_source_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.event_bus_name is not None:
+            result['EventBusName'] = self.event_bus_name
         if self.event_source_name is not None:
             result['EventSourceName'] = self.event_source_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('EventBusName') is not None:
+            self.event_bus_name = m.get('EventBusName')
         if m.get('EventSourceName') is not None:
             self.event_source_name = m.get('EventSourceName')
         return self
 
 
 class DeleteEventSourceResponseBody(TeaModel):
     def __init__(
@@ -12069,18 +12087,20 @@
 
 class GetEventStreamingResponseBodyDataSourceSourcePrometheusParameters(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         data_type: str = None,
         labels: str = None,
+        region_id: str = None,
     ):
         self.cluster_id = cluster_id
         self.data_type = data_type
         self.labels = labels
+        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -12089,24 +12109,28 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
@@ -17283,14 +17307,59 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
+class ListEventStreamingsResponseBodyDataEventStreamingsSourceSourcePrometheusParameters(TeaModel):
+    def __init__(
+        self,
+        cluster_id: str = None,
+        data_type: str = None,
+        labels: str = None,
+        region_id: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.data_type = data_type
+        self.labels = labels
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
         queue_name: str = None,
         region_id: str = None,
         virtual_host_name: str = None,
@@ -17531,26 +17600,28 @@
 class ListEventStreamingsResponseBodyDataEventStreamingsSource(TeaModel):
     def __init__(
         self,
         source_dtsparameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceDTSParameters = None,
         source_kafka_parameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceKafkaParameters = None,
         source_mnsparameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceMNSParameters = None,
         source_mqttparameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceMQTTParameters = None,
+        source_prometheus_parameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourcePrometheusParameters = None,
         source_rabbit_mqparameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRabbitMQParameters = None,
         source_rocket_mqparameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceRocketMQParameters = None,
         source_slsparameters: ListEventStreamingsResponseBodyDataEventStreamingsSourceSourceSLSParameters = None,
     ):
         # The parameters that are returned if Data Transmission Service (DTS) is specified as the event source.
         self.source_dtsparameters = source_dtsparameters
         # The parameters that are returned if Message Queue for Apache Kafka is specified as the event source.
         self.source_kafka_parameters = source_kafka_parameters
         # The parameters that are returned if Message Service (MNS) is specified as the event source.
         self.source_mnsparameters = source_mnsparameters
         # The parameters that are returned if Message Queue for MQTT is specified as the event source.
         self.source_mqttparameters = source_mqttparameters
+        self.source_prometheus_parameters = source_prometheus_parameters
         # The parameters that are returned if Message Queue for RabbitMQ is specified as the event source.
         self.source_rabbit_mqparameters = source_rabbit_mqparameters
         # Source RocketMQ Parameters
         self.source_rocket_mqparameters = source_rocket_mqparameters
         # The parameters that are returned if Log Service is specified as the event source.
         self.source_slsparameters = source_slsparameters
 
@@ -17559,14 +17630,16 @@
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
 
@@ -17580,14 +17653,16 @@
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
@@ -17602,14 +17677,17 @@
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
@@ -26071,18 +26149,20 @@
 
 class UpdateEventStreamingRequestSourceSourcePrometheusParameters(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         data_type: str = None,
         labels: str = None,
+        region_id: str = None,
     ):
         self.cluster_id = cluster_id
         self.data_type = data_type
         self.labels = labels
+        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -26091,24 +26171,28 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
```

### Comparing `alibabacloud_eventbridge20200401-4.0.0/alibabacloud_eventbridge20200401.egg-info/PKG-INFO` & `alibabacloud_eventbridge20200401-4.0.1/alibabacloud_eventbridge20200401.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eventbridge20200401
-Version: 4.0.0
+Version: 4.0.1
 Summary: Alibaba Cloud eventbridge (20200401) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eventbridge20200401-4.0.0/setup.py` & `alibabacloud_eventbridge20200401-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eventbridge20200401.
 
-Created on 14/03/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eventbridge20200401"
 NAME = "alibabacloud_eventbridge20200401" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eventbridge (20200401) SDK Library for Python"
```

