# Comparing `tmp/azure-kusto-ingest-4.3.1.tar.gz` & `tmp/azure-kusto-ingest-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-ingest-4.3.1.tar", last modified: Mon Dec 18 15:33:57 2023, max compression
+gzip compressed data, was "dist/azure-kusto-ingest-4.4.0.tar", last modified: Tue Apr  9 05:14:47 2024, max compression
```

## Comparing `azure-kusto-ingest-4.3.1.tar` & `azure-kusto-ingest-4.4.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_ingest_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_ranked_storage_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_status_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_storage_account_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_stream_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/base_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/ingestion_blob_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/ingestion_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/managed_streaming_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/azure/kusto/ingest/streaming_ingest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-18 15:33:57.000000 azure-kusto-ingest-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-18 15:33:46.000000 azure-kusto-ingest-4.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ingest_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ranked_storage_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_status_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_storage_account_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_stream_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/base_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_blob_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/managed_streaming_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/streaming_ingest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/setup.py
```

### Comparing `azure-kusto-ingest-4.3.1/PKG-INFO` & `azure-kusto-ingest-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.3.1
+Version: 4.4.0
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.3.1/README.rst` & `azure-kusto-ingest-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/__init__.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/_ingest_telemetry.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ingest_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/_ranked_storage_account.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ranked_storage_account.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/_resource_manager.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_resource_manager.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/_status_q.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_status_q.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/_storage_account_set.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_storage_account_set.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/_stream_extensions.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_stream_extensions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/base_ingest_client.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/base_ingest_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+import ipaddress
 import os
 import tempfile
 import time
 import uuid
 from abc import ABCMeta, abstractmethod
 from copy import copy
 from enum import Enum
 from io import TextIOWrapper
 from typing import TYPE_CHECKING, Union, IO, AnyStr, Optional, Tuple
+from urllib.parse import urlparse
 
 from azure.kusto.data.data_format import DataFormat
 from azure.kusto.data.exceptions import KustoClosedError
 
 from .descriptors import FileDescriptor, StreamDescriptor
 from .ingestion_properties import IngestionProperties
 
 
 if TYPE_CHECKING:
     import pandas
 
+INGEST_PREFIX = "ingest-"
+PROTOCOL_SUFFIX = "://"
+
 
 class IngestionStatus(Enum):
     """
     The ingestion was queued.
     """
 
     QUEUED = "QUEUED"
@@ -165,7 +170,34 @@
         self._is_closed = True
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
+
+    @staticmethod
+    def get_ingestion_endpoint(cluster_url: str) -> str:
+        if INGEST_PREFIX in cluster_url or not cluster_url or BaseIngestClient.is_reserved_hostname(cluster_url):
+            return cluster_url
+        else:
+            return cluster_url.replace(PROTOCOL_SUFFIX, PROTOCOL_SUFFIX + INGEST_PREFIX, 1)
+
+    @staticmethod
+    def get_query_endpoint(cluster_url: str) -> str:
+        if INGEST_PREFIX in cluster_url:
+            return cluster_url.replace(INGEST_PREFIX, "", 1)
+        else:
+            return cluster_url
+
+    @staticmethod
+    def is_reserved_hostname(raw_uri: str) -> bool:
+        url = urlparse(raw_uri)
+        if not url.netloc:
+            return True
+        authority = url.netloc.split(":")[0]  # removes port if exists
+        try:
+            is_ip = ipaddress.ip_address(authority)
+        except ValueError:
+            is_ip = False
+        is_localhost = "localhost" in authority
+        return is_localhost or is_ip or authority.lower() == "onebox.dev.kusto.windows.net"
```

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/descriptors.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/descriptors.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import uuid
 from copy import copy
 from gzip import GzipFile
 from io import BytesIO, SEEK_END
 from typing import Union, Optional, AnyStr, IO, List, Dict
 from zipfile import ZipFile
 
+from azure.storage.blob import BlobClient
+
 OptionalUUID = Optional[Union[str, uuid.UUID]]
 
 
 def ensure_uuid(maybe_uuid: OptionalUUID) -> uuid.UUID:
     if not maybe_uuid:
         return uuid.uuid4()
 
@@ -146,14 +148,18 @@
 
     def get_tracing_attributes(self) -> dict:
         # Remove query parameters from self.path, if exists
         if self.path:
             obfuscated_path = self.path.split("?")[0].split(";")[0]
         return {self._BLOB_URI: obfuscated_path, self._SOURCE_ID: str(self.source_id)}
 
+    def fill_size(self):
+        if not self.size:
+            self.size = BlobClient.from_blob_url(self.path).get_blob_properties().size
+
 
 class StreamDescriptor(DescriptorBase):
     """StreamDescriptor is used to describe a stream that will be used as ingestion source"""
 
     _STREAM_NAME = "stream_name"
 
     # TODO: currently we always assume that streams are gz compressed (will get compressed before sending), should we expand that?
```

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/exceptions.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/ingest_client.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingest_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,30 +28,35 @@
     """
     Queued ingest client provides methods to allow queued ingestion into kusto (ADX).
     To learn more about the different types of ingestions and when to use each, visit:
     https://docs.microsoft.com/en-us/azure/data-explorer/ingest-data-overview#ingestion-methods
     """
 
     _INGEST_PREFIX = "ingest-"
-    _EXPECTED_SERVICE_TYPE = "DataManagement"
     _SERVICE_CLIENT_TIMEOUT_SECONDS = 10 * 60
     _MAX_RETRIES = 3
 
-    def __init__(self, kcsb: Union[str, KustoConnectionStringBuilder]):
+    def __init__(self, kcsb: Union[str, KustoConnectionStringBuilder], auto_correct_endpoint: bool = True):
         """Kusto Ingest Client constructor.
         :param kcsb: The connection string to initialize KustoClient.
         """
         super().__init__()
         if not isinstance(kcsb, KustoConnectionStringBuilder):
             kcsb = KustoConnectionStringBuilder(kcsb)
+
+        if auto_correct_endpoint:
+            kcsb["Data Source"] = BaseIngestClient.get_ingestion_endpoint(kcsb.data_source)
+
         self._proxy_dict: Optional[Dict[str, str]] = None
         self._connection_datasource = kcsb.data_source
         self._resource_manager = _ResourceManager(KustoClient(kcsb))
         self._endpoint_service_type = None
         self._suggested_endpoint_uri = None
+        self.application_for_tracing = kcsb.client_details.application_for_tracing
+        self.client_version_for_tracing = kcsb.client_details.version_for_tracing
 
     def close(self) -> None:
         self._resource_manager.close()
         super().close()
 
     def set_proxy(self, proxy_url: str):
         self._resource_manager.set_proxy(proxy_url)
@@ -121,22 +126,24 @@
         :param azure.kusto.ingest.IngestionProperties ingestion_properties: Ingestion properties.
         """
         IngestTracingAttributes.set_ingest_descriptor_attributes(blob_descriptor, ingestion_properties)
 
         if self._is_closed:
             raise KustoClosedError()
 
-        try:
-            queues = self._resource_manager.get_ingestion_queues()
-        except KustoServiceError as ex:
-            self._validate_endpoint_service_type()
-            raise ex
+        queues = self._resource_manager.get_ingestion_queues()
 
         authorization_context = self._resource_manager.get_authorization_context()
-        ingestion_blob_info = IngestionBlobInfo(blob_descriptor, ingestion_properties=ingestion_properties, auth_context=authorization_context)
+        ingestion_blob_info = IngestionBlobInfo(
+            blob_descriptor,
+            ingestion_properties=ingestion_properties,
+            auth_context=authorization_context,
+            application_for_tracing=self.application_for_tracing,
+            client_version_for_tracing=self.client_version_for_tracing,
+        )
         ingestion_blob_info_json = ingestion_blob_info.to_json()
         retries_left = min(self._MAX_RETRIES, len(queues))
         for queue in queues:
             try:
                 with QueueServiceClient(queue.account_uri, proxies=self._proxy_dict) as queue_service:
                     with queue_service.get_queue_client(queue=queue.object_name, message_encode_policy=TextBase64EncodePolicy()) as queue_client:
                         # trace enqueuing of blob for ingestion
@@ -152,54 +159,15 @@
                 retries_left = retries_left - 1
                 # TODO: log the retry once we have a proper logging system
                 self._resource_manager.report_resource_usage_result(queue.storage_account_name, False)
                 if retries_left == 0:
                     raise KustoQueueError() from e
 
     def _get_containers(self) -> List[_ResourceUri]:
-        try:
-            containers = self._resource_manager.get_containers()
-        except KustoServiceError as ex:
-            self._validate_endpoint_service_type()
-            raise ex
-        return containers
-
-    def _validate_endpoint_service_type(self):
-        if not self._hostname_starts_with_ingest(self._connection_datasource):
-            if not self._endpoint_service_type:
-                self._endpoint_service_type = self._retrieve_service_type()
-
-            if self._EXPECTED_SERVICE_TYPE != self._endpoint_service_type:
-                if not self._suggested_endpoint_uri:
-                    self._suggested_endpoint_uri = self._generate_endpoint_suggestion(self._connection_datasource)
-                    if not self._suggested_endpoint_uri:
-                        raise KustoInvalidEndpointError(self._EXPECTED_SERVICE_TYPE, self._endpoint_service_type)
-                raise KustoInvalidEndpointError(self._EXPECTED_SERVICE_TYPE, self._endpoint_service_type, self._suggested_endpoint_uri)
-
-    def _retrieve_service_type(self) -> str:
-        return self._resource_manager.retrieve_service_type()
-
-    def _generate_endpoint_suggestion(self, datasource: str) -> Optional[str]:
-        """The default is not passing a suggestion to the exception String"""
-        endpoint_uri_to_suggest_str = None
-        if datasource.strip():
-            try:
-                endpoint_uri_to_suggest = urlparse(datasource)  # Standardize URL formatting
-                endpoint_uri_to_suggest = urlparse(endpoint_uri_to_suggest.scheme + "://" + self._INGEST_PREFIX + endpoint_uri_to_suggest.hostname)
-                endpoint_uri_to_suggest_str = endpoint_uri_to_suggest.geturl()
-            except Exception:
-                # TODO: Add logging infrastructure so we can tell the user as a warning:
-                #   "Couldn't generate suggested endpoint due to problem parsing datasource, with exception: {ex}. The correct endpoint is usually the Engine endpoint with '{self._INGEST_PREFIX}' prepended to the hostname."
-                pass
-        return endpoint_uri_to_suggest_str
-
-    def _hostname_starts_with_ingest(self, datasource: str) -> bool:
-        datasource_uri = urlparse(datasource)
-        hostname = datasource_uri.hostname
-        return hostname and hostname.startswith(self._INGEST_PREFIX)
+        return self._resource_manager.get_containers()
 
     def upload_blob(
         self,
         containers: List[_ResourceUri],
         descriptor: Union[FileDescriptor, "StreamDescriptor"],
         database: str,
         table: str,
```

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/ingestion_blob_info.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_blob_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,37 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from azure.kusto.ingest import BlobDescriptor, IngestionProperties
 
 
 class IngestionBlobInfo:
-    def __init__(self, blob_descriptor: "BlobDescriptor", ingestion_properties: "IngestionProperties", auth_context=None):
+    def __init__(
+        self,
+        blob_descriptor: "BlobDescriptor",
+        ingestion_properties: "IngestionProperties",
+        auth_context=None,
+        application_for_tracing=None,
+        client_version_for_tracing=None,
+    ):
         self.properties = dict()
         self.properties["BlobPath"] = blob_descriptor.path
         if blob_descriptor.size:
             self.properties["RawDataSize"] = blob_descriptor.size
         self.properties["DatabaseName"] = ingestion_properties.database
         self.properties["TableName"] = ingestion_properties.table
         self.properties["RetainBlobOnSuccess"] = True
         self.properties["FlushImmediately"] = ingestion_properties.flush_immediately
         self.properties["IgnoreSizeLimit"] = False
         self.properties["ReportLevel"] = ingestion_properties.report_level.value
         self.properties["ReportMethod"] = ingestion_properties.report_method.value
         self.properties["SourceMessageCreationTime"] = datetime.utcnow().isoformat()
         self.properties["Id"] = str(blob_descriptor.source_id)
+        self.properties["ApplicationForTracing"] = application_for_tracing
+        self.properties["ClientVersionForTracing"] = client_version_for_tracing
 
         additional_properties = ingestion_properties.additional_properties or {}
         additional_properties["authorizationContext"] = auth_context
 
         tags = []
         if ingestion_properties.additional_tags:
             tags.extend(ingestion_properties.additional_tags)
```

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/ingestion_properties.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/managed_streaming_ingest_client.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/managed_streaming_ingest_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import uuid
 from io import SEEK_SET
-from typing import AnyStr, IO, TYPE_CHECKING, Union
+from typing import AnyStr, IO, TYPE_CHECKING, Union, Optional
 
+from azure.kusto.ingest.descriptors import DescriptorBase
 from tenacity import Retrying, _utils, stop_after_attempt, wait_random_exponential
 
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing import SpanKind
 
 from azure.kusto.data import KustoConnectionStringBuilder
 from azure.kusto.data.exceptions import KustoApiError, KustoClosedError
 from azure.kusto.data._telemetry import MonitoredActivity
 
-
 from . import BlobDescriptor, FileDescriptor, IngestionProperties, StreamDescriptor
 from ._ingest_telemetry import IngestTracingAttributes
 from ._stream_extensions import chain_streams, read_until_size_or_end
 from .base_ingest_client import BaseIngestClient, IngestionResult
 from .ingest_client import QueuedIngestClient
 from .streaming_ingest_client import KustoStreamingIngestClient
 
@@ -33,46 +33,23 @@
         - Multiple transient errors were encountered when trying to do streaming ingestion
         - The ingestion is too large for streaming ingestion (over 4MB)
         - The ingestion is directly from a blob
     """
 
     MAX_STREAMING_SIZE_IN_BYTES = 4 * 1024 * 1024
 
-    @staticmethod
-    def from_engine_kcsb(engine_kcsb: Union[KustoConnectionStringBuilder, str]) -> "ManagedStreamingIngestClient":
-        """
-        Create a ManagedStreamingIngestClient from a KustoConnectionStringBuilder for the engine.
-        This Connection String is used for the streaming ingest client.
-        This method will infer the dm connection string (by using the same authentication and adding the ingest- prefix)
-        For advanced use cases, use the constructor directly.
-        :param engine_kcsb: KustoConnectionStringBuilder for the engine.
-        :return: ManagedStreamingIngestClient
-        """
-        kcsb = repr(engine_kcsb) if type(engine_kcsb) == KustoConnectionStringBuilder else engine_kcsb
-        dm_kcsb = KustoConnectionStringBuilder(kcsb.replace("https://", "https://ingest-"))
-        return ManagedStreamingIngestClient(engine_kcsb, dm_kcsb)
-
-    @staticmethod
-    def from_dm_kcsb(dm_kcsb: Union[KustoConnectionStringBuilder, str]) -> "ManagedStreamingIngestClient":
-        """
-        Create a ManagedStreamingIngestClient from a KustoConnectionStringBuilder for the dm.
-        This Connection String is used for the queued ingest client.
-        This method will infer the engine connection string (by using the same authentication and removing the ingest- prefix)
-        For advanced use cases, use the constructor directly.
-        :param dm_kcsb: KustoConnectionStringBuilder for the dm.
-        :return: ManagedStreamingIngestClient
-        """
-        kcsb = repr(dm_kcsb) if type(dm_kcsb) == KustoConnectionStringBuilder else dm_kcsb
-        engine_kcsb = KustoConnectionStringBuilder(kcsb.replace("https://ingest-", "https://"))
-        return ManagedStreamingIngestClient(engine_kcsb, dm_kcsb)
-
-    def __init__(self, engine_kcsb: Union[KustoConnectionStringBuilder, str], dm_kcsb: Union[KustoConnectionStringBuilder, str]):
+    def __init__(
+        self,
+        engine_kcsb: Union[KustoConnectionStringBuilder, str],
+        dm_kcsb: Union[KustoConnectionStringBuilder, str, None] = None,
+        auto_correct_endpoint: bool = True,
+    ):
         super().__init__()
-        self.queued_client = QueuedIngestClient(dm_kcsb)
-        self.streaming_client = KustoStreamingIngestClient(engine_kcsb)
+        self.queued_client = QueuedIngestClient(dm_kcsb if dm_kcsb is not None else engine_kcsb, auto_correct_endpoint)
+        self.streaming_client = KustoStreamingIngestClient(engine_kcsb, auto_correct_endpoint)
         self._set_retry_settings()
 
     def close(self) -> None:
         if not self._is_closed:
             self.queued_client.close()
             self.streaming_client.close()
         super().close()
@@ -104,38 +81,28 @@
 
         super().ingest_from_stream(stream_descriptor, ingestion_properties)
 
         stream_descriptor = BaseIngestClient._prepare_stream(stream_descriptor, ingestion_properties)
         stream = stream_descriptor.stream
 
         buffered_stream = read_until_size_or_end(stream, self.MAX_STREAMING_SIZE_IN_BYTES + 1)
-
-        if len(buffered_stream.getbuffer()) > self.MAX_STREAMING_SIZE_IN_BYTES:
-            stream_descriptor.stream = chain_streams([buffered_stream, stream])
-            return self.queued_client.ingest_from_stream(stream_descriptor, ingestion_properties)
+        length = len(buffered_stream.getbuffer())
 
         stream_descriptor.stream = buffered_stream
 
         try:
-            for attempt in Retrying(
-                stop=stop_after_attempt(self._num_of_attempts), wait=wait_random_exponential(max=self._max_seconds_per_retry), reraise=True
-            ):
-                with attempt:
-                    stream.seek(0, SEEK_SET)
-                    client_request_id = ManagedStreamingIngestClient._get_request_id(stream_descriptor.source_id, attempt.retry_state.attempt_number - 1)
-                    # trace attempt to ingest from stream
-                    invoker = lambda: self.streaming_client._ingest_from_stream_with_client_request_id(
-                        stream_descriptor, ingestion_properties, client_request_id
-                    )
-                    return MonitoredActivity.invoke(invoker, name_of_span="ManagedStreamingIngestClient.ingest_from_stream_attempt")
-
+            res = self._stream_with_retries(length, stream_descriptor, ingestion_properties)
+            if res:
+                return res
+            stream_descriptor.stream = chain_streams([buffered_stream, stream])
         except KustoApiError as ex:
             error = ex.get_api_error()
             if error.permanent:
                 raise
+            buffered_stream.seek(0, SEEK_SET)
 
         return self.queued_client.ingest_from_stream(stream_descriptor, ingestion_properties)
 
     @distributed_trace(kind=SpanKind.CLIENT)
     def ingest_from_blob(self, blob_descriptor: BlobDescriptor, ingestion_properties: IngestionProperties):
         """
         Enqueue an ingest command from azure blobs.
@@ -147,13 +114,46 @@
         :param azure.kusto.ingest.BlobDescriptor blob_descriptor: An object that contains a description of the blob to be ingested.
         :param azure.kusto.ingest.IngestionProperties ingestion_properties: Ingestion properties.
         """
         IngestTracingAttributes.set_ingest_descriptor_attributes(blob_descriptor, ingestion_properties)
 
         if self._is_closed:
             raise KustoClosedError()
+        blob_descriptor.fill_size()
+        try:
+            res = self._stream_with_retries(blob_descriptor.size, blob_descriptor, ingestion_properties)
+            if res:
+                return res
+        except KustoApiError as ex:
+            error = ex.get_api_error()
+            if error.permanent:
+                raise
 
         return self.queued_client.ingest_from_blob(blob_descriptor, ingestion_properties)
 
+    def _stream_with_retries(
+        self,
+        length: int,
+        descriptor: DescriptorBase,
+        props: IngestionProperties,
+    ) -> Optional[IngestionResult]:
+        from_stream = isinstance(descriptor, StreamDescriptor)
+        if length > self.MAX_STREAMING_SIZE_IN_BYTES:
+            return None
+        for attempt in Retrying(stop=stop_after_attempt(self._num_of_attempts), wait=wait_random_exponential(max=self._max_seconds_per_retry), reraise=True):
+            with attempt:
+                client_request_id = ManagedStreamingIngestClient._get_request_id(descriptor.source_id, attempt.retry_state.attempt_number - 1)
+                # trace attempt to ingest from stream
+                if from_stream:
+                    descriptor.stream.seek(0, SEEK_SET)
+                    invoker = lambda: self.streaming_client._ingest_from_stream_with_client_request_id(descriptor, props, client_request_id)
+                else:
+                    invoker = lambda: self.streaming_client.ingest_from_blob(descriptor, props, client_request_id)
+                return MonitoredActivity.invoke(
+                    invoker,
+                    name_of_span="ManagedStreamingIngestClient.ingest_from_stream_attempt",
+                    tracing_attributes={"attemptNumber": attempt, "sourceIsStream": from_stream},
+                )
+
     @staticmethod
     def _get_request_id(source_id: uuid.UUID, attempt: int):
         return f"KPC.executeManagedStreamingIngest;{source_id};{attempt}"
```

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/status.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/status.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.3.1/azure/kusto/ingest/streaming_ingest_client.py` & `azure-kusto-ingest-4.4.0/azure/kusto/ingest/streaming_ingest_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,30 +6,36 @@
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing import SpanKind
 
 from azure.kusto.data import KustoClient, KustoConnectionStringBuilder, ClientRequestProperties
 
 from ._ingest_telemetry import IngestTracingAttributes
 from .base_ingest_client import BaseIngestClient, IngestionResult, IngestionStatus
-from .descriptors import FileDescriptor, StreamDescriptor
+from .descriptors import FileDescriptor, StreamDescriptor, BlobDescriptor
 from .ingestion_properties import IngestionProperties
 
 
 class KustoStreamingIngestClient(BaseIngestClient):
     """Kusto streaming ingest client for Python.
     KustoStreamingIngestClient works with both 2.x and 3.x flavors of Python.
     All primitive types are supported.
     Tests are run using pytest.
     """
 
-    def __init__(self, kcsb: Union[KustoConnectionStringBuilder, str]):
+    def __init__(self, kcsb: Union[KustoConnectionStringBuilder, str], auto_correct_endpoint: bool = True):
         """Kusto Streaming Ingest Client constructor.
         :param KustoConnectionStringBuilder kcsb: The connection string to initialize KustoClient.
         """
         super().__init__()
+
+        if isinstance(kcsb, str):
+            kcsb = KustoConnectionStringBuilder(kcsb)
+
+        if auto_correct_endpoint:
+            kcsb["Data Source"] = BaseIngestClient.get_query_endpoint(kcsb.data_source)
         self._kusto_client = KustoClient(kcsb)
 
     def close(self):
         if not self._is_closed:
             self._kusto_client.close()
         super().close()
 
@@ -75,13 +81,34 @@
             additional_properties = ClientRequestProperties()
             additional_properties.client_request_id = client_request_id
 
         self._kusto_client.execute_streaming_ingest(
             ingestion_properties.database,
             ingestion_properties.table,
             stream_descriptor.stream,
+            None,
             ingestion_properties.format.name,
             additional_properties,
             mapping_name=ingestion_properties.ingestion_mapping_reference,
         )
 
         return IngestionResult(IngestionStatus.SUCCESS, ingestion_properties.database, ingestion_properties.table, stream_descriptor.source_id)
+
+    def ingest_from_blob(
+        self, blob_descriptor: BlobDescriptor, ingestion_properties: IngestionProperties, client_request_id: Optional[str] = None
+    ) -> IngestionResult:
+        IngestTracingAttributes.set_ingest_descriptor_attributes(blob_descriptor, ingestion_properties)
+        additional_properties = None
+        if client_request_id:
+            additional_properties = ClientRequestProperties()
+            additional_properties.client_request_id = client_request_id
+
+        self._kusto_client.execute_streaming_ingest(
+            ingestion_properties.database,
+            ingestion_properties.table,
+            None,
+            blob_descriptor.path,
+            ingestion_properties.format.name,
+            additional_properties,
+            mapping_name=ingestion_properties.ingestion_mapping_reference,
+        )
+        return IngestionResult(IngestionStatus.SUCCESS, ingestion_properties.database, ingestion_properties.table, blob_descriptor.source_id)
```

### Comparing `azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/PKG-INFO` & `azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.3.1
+Version: 4.4.0
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.3.1/azure_kusto_ingest.egg-info/SOURCES.txt` & `azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 azure/kusto/__init__.py
 azure/kusto/ingest/__init__.py
 azure/kusto/ingest/_ingest_telemetry.py
 azure/kusto/ingest/_ranked_storage_account.py
```

### Comparing `azure-kusto-ingest-4.3.1/setup.py` & `azure-kusto-ingest-4.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,11 +38,11 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
-    packages=find_packages(exclude=["azure", "tests"]),
+    packages=find_packages(exclude=["azure", "*tests*", "*tests.*"]),
     install_requires=["azure-kusto-data=={}".format(VERSION), "azure-storage-blob>=12,<13", "azure-storage-queue>=12,<13", "tenacity>=8.0.0"],
     extras_require={"pandas": ["pandas"], "aio": []},
 )
```

