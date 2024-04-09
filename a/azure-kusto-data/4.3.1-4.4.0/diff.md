# Comparing `tmp/azure-kusto-data-4.3.1.tar.gz` & `tmp/azure-kusto-data-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-data-4.3.1.tar", last modified: Mon Dec 18 15:33:57 2023, max compression
+gzip compressed data, was "dist/azure-kusto-data-4.4.0.tar", last modified: Tue Apr  9 05:14:46 2024, max compression
```

## Comparing `azure-kusto-data-4.3.1.tar` & `azure-kusto-data-4.4.0.tar`

### file list

```diff
@@ -1,52 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/azure/kusto/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_cloud_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/azure/kusto/data/aio/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/aio/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/aio/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/aio/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15224 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/client_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/client_request_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30943 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/kcsb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/kusto_trusted_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/azure/kusto/data/wellKnownKustoEndpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2023-12-18 15:33:56.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-12-18 15:33:56.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 15:33:56.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-18 15:33:56.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-18 15:33:56.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-18 15:33:56.000000 azure-kusto-data-4.3.1/azure_kusto_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:57.000000 azure-kusto-data-4.3.1/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15947 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/tests/aio/test_async_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2023-12-18 15:33:46.000000 azure-kusto-data-4.3.1/tests/aio/test_kusto_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/kusto/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_cloud_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_token_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client_request_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30943 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/kcsb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/kusto_trusted_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/wellKnownKustoEndpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/setup.py
```

### Comparing `azure-kusto-data-4.3.1/PKG-INFO` & `azure-kusto-data-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.3.1
+Version: 4.4.0
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.3.1/README.rst` & `azure-kusto-data-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/_cloud_settings.py` & `azure-kusto-data-4.4.0/azure/kusto/data/_cloud_settings.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/_converters.py` & `azure-kusto-data-4.4.0/azure/kusto/data/_converters.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/_models.py` & `azure-kusto-data-4.4.0/azure/kusto/data/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/_telemetry.py` & `azure-kusto-data-4.4.0/azure/kusto/data/_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/_token_providers.py` & `azure-kusto-data-4.4.0/azure/kusto/data/_token_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         if self._msi_auth_context is not None:
             self._msi_auth_context.close()
         if self._msi_auth_context is not None:
             raise KustoAsyncUsageError("Can't close async token provider with sync close", self.is_async)
 
     async def close_async(self):
         if self._msi_auth_context is not None:
-            sync_to_async(self._msi_auth_context.close())
+            await sync_to_async(self._msi_auth_context.close())
 
         if self._msi_auth_context_async is not None:
             await self._msi_auth_context_async.close()
 
 
 class AzCliTokenProvider(CloudInfoTokenProvider):
     """AzCli Token Provider obtains a refresh token from the AzCli cache and uses it to authenticate with MSAL"""
@@ -468,15 +468,15 @@
         if self._az_auth_context is not None:
             self._az_auth_context.close()
         if self._az_auth_context_async is not None:
             raise KustoAsyncUsageError("Can't close async token provider with sync close", self.is_async)
 
     async def close_async(self):
         if self._az_auth_context is not None:
-            sync_to_async(self._az_auth_context.close())
+            await sync_to_async(self._az_auth_context.close())
 
         if self._az_auth_context_async is not None:
             await self._az_auth_context_async.close()
 
 
 class UserPassTokenProvider(CloudInfoTokenProvider):
     """Acquire a token from MSAL with username and password"""
@@ -693,15 +693,15 @@
             self.credential_from_login_endpoint = None
 
     async def close_async(self):
         if self.credential is not None:
             if inspect.iscoroutinefunction(self.credential.close):
                 await self.credential.close()
             else:
-                sync_to_async(self.credential.close)()
+                await sync_to_async(self.credential.close)()
             self.credential = None
             self.credential_from_login_endpoint = None
 
 
 class DeviceLoginTokenProvider(AzureIdentityTokenCredentialProvider):
     """Acquire a token from MSAL with Device Login flow"""
```

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/aio/_models.py` & `azure-kusto-data-4.4.0/azure/kusto/data/aio/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/aio/client.py` & `azure-kusto-data-4.4.0/azure/kusto/data/aio/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,63 +47,109 @@
     @aio_documented_by(KustoClientSync.execute)
     async def execute(self, database: Optional[str], query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
         query = query.strip()
         if query.startswith("."):
             return await self.execute_mgmt(database, query, properties)
         return await self.execute_query(database, query, properties)
 
-    @distributed_trace_async(name_of_span="KustoClient.query_cmd", kind=SpanKind.CLIENT)
+    @distributed_trace_async(name_of_span="AioKustoClient.query_cmd", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_query)
     async def execute_query(self, database: str, query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
         database = self._get_database_or_default(database)
         Span.set_query_attributes(self._kusto_cluster, database, properties)
+        request = ExecuteRequestParams._from_query(
+            query,
+            database,
+            properties,
+            self._request_headers,
+            self._query_default_timeout,
+            self._mgmt_default_timeout,
+            self._client_server_delta,
+            self.client_details,
+        )
+        return await self._execute(self._query_endpoint, request, properties)
 
-        return await self._execute(self._query_endpoint, database, query, None, KustoClient._query_default_timeout, properties)
-
-    @distributed_trace_async(name_of_span="KustoClient.control_cmd", kind=SpanKind.CLIENT)
+    @distributed_trace_async(name_of_span="AioKustoClient.control_cmd", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_mgmt)
     async def execute_mgmt(self, database: str, query: str, properties: ClientRequestProperties = None) -> KustoResponseDataSet:
         database = self._get_database_or_default(database)
         Span.set_query_attributes(self._kusto_cluster, database, properties)
+        request = ExecuteRequestParams._from_query(
+            query,
+            database,
+            properties,
+            self._request_headers,
+            self._mgmt_default_timeout,
+            self._mgmt_default_timeout,
+            self._client_server_delta,
+            self.client_details,
+        )
+        return await self._execute(self._mgmt_endpoint, request, properties)
 
-        return await self._execute(self._mgmt_endpoint, database, query, None, KustoClient._mgmt_default_timeout, properties)
-
-    @distributed_trace_async(name_of_span="KustoClient.streaming_ingest", kind=SpanKind.CLIENT)
+    @distributed_trace_async(name_of_span="AioKustoClient.streaming_ingest", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_streaming_ingest)
     async def execute_streaming_ingest(
         self,
         database: Optional[str],
         table: str,
-        stream: io.IOBase,
+        stream: Optional[io.IOBase],
+        blob_url: Optional[str],
         stream_format: Union[DataFormat, str],
         properties: ClientRequestProperties = None,
         mapping_name: str = None,
     ):
         database = self._get_database_or_default(database)
-        Span.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
 
         stream_format = stream_format.kusto_value if isinstance(stream_format, DataFormat) else DataFormat[stream_format.upper()].kusto_value
         endpoint = self._streaming_ingest_endpoint + database + "/" + table + "?streamFormat=" + stream_format
         if mapping_name is not None:
             endpoint = endpoint + "&mappingName=" + mapping_name
 
-        await self._execute(endpoint, database, None, stream, self._streaming_ingest_default_timeout, properties)
+        if blob_url:
+            endpoint += "&sourceKind=uri"
+            request = ExecuteRequestParams._from_blob_url(
+                blob_url,
+                properties,
+                self._request_headers,
+                self._streaming_ingest_default_timeout,
+                self._mgmt_default_timeout,
+                self._client_server_delta,
+                self.client_details,
+            )
+        elif stream:
+            request = ExecuteRequestParams._from_stream(
+                stream,
+                properties,
+                self._request_headers,
+                self._streaming_ingest_default_timeout,
+                self._mgmt_default_timeout,
+                self._client_server_delta,
+                self.client_details,
+            )
+        else:
+            raise Exception("execute_streaming_ingest is expecting either a stream or blob url")
+
+        Span.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
+        await self._execute(endpoint, request, properties)
 
     @aio_documented_by(KustoClientSync._execute_streaming_query_parsed)
     async def _execute_streaming_query_parsed(
         self,
         database: Optional[str],
         query: str,
         timeout: timedelta = _KustoClientBase._query_default_timeout,
         properties: Optional[ClientRequestProperties] = None,
     ) -> StreamingDataSetEnumerator:
-        response = await self._execute(self._query_endpoint, database, query, None, timeout, properties, stream_response=True)
+        request = ExecuteRequestParams._from_query(
+            query, database, properties, self._request_headers, timeout, self._mgmt_default_timeout, self._client_server_delta, self.client_details
+        )
+        response = await self._execute(self._query_endpoint, request, properties, stream_response=True)
         return StreamingDataSetEnumerator(JsonTokenReader(response.content))
 
-    @distributed_trace_async(name_of_span="KustoClient.streaming_query", kind=SpanKind.CLIENT)
+    @distributed_trace_async(name_of_span="AioKustoClient.streaming_query", kind=SpanKind.CLIENT)
     @aio_documented_by(KustoClientSync.execute_streaming_query)
     async def execute_streaming_query(
         self,
         database: Optional[str],
         query: str,
         timeout: timedelta = _KustoClientBase._query_default_timeout,
         properties: Optional[ClientRequestProperties] = None,
@@ -114,49 +160,41 @@
         response = await self._execute_streaming_query_parsed(database, query, timeout, properties)
         return KustoStreamingResponseDataSet(response)
 
     @aio_documented_by(KustoClientSync._execute)
     async def _execute(
         self,
         endpoint: str,
-        database: Optional[str],
-        query: Optional[str],
-        payload: Optional[io.IOBase],
-        timeout: timedelta,
-        properties: ClientRequestProperties = None,
+        request: ExecuteRequestParams,
+        properties: Optional[ClientRequestProperties] = None,
         stream_response: bool = False,
     ) -> Union[KustoResponseDataSet, ClientResponse]:
         """Executes given query against this client"""
         if self._is_closed:
             raise KustoClosedError()
         self.validate_endpoint()
-        request_params = ExecuteRequestParams(
-            database,
-            payload,
-            properties,
-            query,
-            timeout,
-            self._request_headers,
-            self._mgmt_default_timeout,
-            self._client_server_delta,
-            self.client_details,
-        )
-        json_payload = request_params.json_payload
-        request_headers = request_params.request_headers
-        timeout = request_params.timeout
+
+        request_headers = request.request_headers
+        timeout = request.timeout
         if self._aad_helper:
             request_headers["Authorization"] = await self._aad_helper.acquire_authorization_header_async()
 
         invoker = lambda: self._session.post(
-            endpoint, headers=request_headers, json=json_payload, data=payload, timeout=timeout.seconds, proxy=self._proxy_url, allow_redirects=False
+            endpoint,
+            headers=request_headers,
+            json=request.json_payload,
+            data=request.payload,
+            timeout=timeout.seconds,
+            proxy=self._proxy_url,
+            allow_redirects=False,
         )
 
         try:
             response = await MonitoredActivity.invoke_async(
-                invoker, name_of_span="KustoClient.http_post", tracing_attributes=Span.create_http_attributes("POST", endpoint, request_headers)
+                invoker, name_of_span="AioKustoClient.http_post", tracing_attributes=Span.create_http_attributes("POST", endpoint, request_headers)
             )
         except Exception as e:
             raise KustoNetworkError(endpoint, None if properties is None else properties.client_request_id) from e
 
         if stream_response:
             try:
                 response.raise_for_status()
@@ -168,23 +206,23 @@
                     response_text = await response.text()
                 except Exception:
                     response_text = None
                 try:
                     response_json = await response.json()
                 except Exception:
                     response_json = None
-                raise self._handle_http_error(e, endpoint, payload, response, response.status, response_json, response_text)
+                raise self._handle_http_error(e, endpoint, request.payload, response, response.status, response_json, response_text)
 
         async with response:
             response_json = None
             try:
                 if 300 <= response.status < 400:
                     raise Exception("Unexpected redirection, got status code: " + str(response.status))
                 response_json = await response.json()
                 response.raise_for_status()
             except Exception as e:
                 try:
                     response_text = await response.text()
                 except Exception:
                     response_text = None
-                raise self._handle_http_error(e, endpoint, payload, response, response.status, response_json, response_text)
-            return MonitoredActivity.invoke(lambda: self._kusto_parse_by_endpoint(endpoint, response_json), name_of_span="KustoClient.processing_response")
+                raise self._handle_http_error(e, endpoint, request.payload, response, response.status, response_json, response_text)
+            return MonitoredActivity.invoke(lambda: self._kusto_parse_by_endpoint(endpoint, response_json), name_of_span="AioKustoClient.processing_response")
```

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/aio/response.py` & `azure-kusto-data-4.4.0/azure/kusto/data/aio/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/aio/streaming_response.py` & `azure-kusto-data-4.4.0/azure/kusto/data/aio/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/client.py` & `azure-kusto-data-4.4.0/azure/kusto/data/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,73 +171,119 @@
         :param str query: Query to be executed.
         :param azure.kusto.data.ClientRequestProperties properties: Optional additional properties.
         :return: Kusto response data set.
         :rtype: azure.kusto.data.response.KustoResponseDataSet
         """
         database = self._get_database_or_default(database)
         Span.set_query_attributes(self._kusto_cluster, database, properties)
-
-        return self._execute(self._query_endpoint, database, query, None, self._query_default_timeout, properties)
+        request = ExecuteRequestParams._from_query(
+            query,
+            database,
+            properties,
+            self._request_headers,
+            self._query_default_timeout,
+            self._mgmt_default_timeout,
+            self._client_server_delta,
+            self.client_details,
+        )
+        return self._execute(self._query_endpoint, request, properties)
 
     @distributed_trace(name_of_span="KustoClient.control_cmd", kind=SpanKind.CLIENT)
     def execute_mgmt(self, database: Optional[str], query: str, properties: Optional[ClientRequestProperties] = None) -> KustoResponseDataSet:
         """
         Execute a KQL control command.
         To learn more about KQL control commands go to  https://docs.microsoft.com/en-us/azure/kusto/management/
         :param Optional[str] database: Database against query will be executed. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str query: Query to be executed.
         :param azure.kusto.data.ClientRequestProperties properties: Optional additional properties.
         :return: Kusto response data set.
         :rtype: azure.kusto.data.response.KustoResponseDataSet
         """
         database = self._get_database_or_default(database)
         Span.set_query_attributes(self._kusto_cluster, database, properties)
-
-        return self._execute(self._mgmt_endpoint, database, query, None, self._mgmt_default_timeout, properties)
+        request = ExecuteRequestParams._from_query(
+            query,
+            database,
+            properties,
+            self._request_headers,
+            self._mgmt_default_timeout,
+            self._mgmt_default_timeout,
+            self._client_server_delta,
+            self.client_details,
+        )
+        return self._execute(self._mgmt_endpoint, request, properties)
 
     @distributed_trace(name_of_span="KustoClient.streaming_ingest", kind=SpanKind.CLIENT)
     def execute_streaming_ingest(
         self,
         database: Optional[str],
         table: str,
-        stream: IO[AnyStr],
+        stream: Optional[IO[AnyStr]],
+        blob_url: Optional[str],
         stream_format: Union[DataFormat, str],
         properties: Optional[ClientRequestProperties] = None,
         mapping_name: str = None,
     ):
         """
         Execute streaming ingest against this client
         If the Kusto service is not configured to allow streaming ingestion, this may raise an error
         To learn more about streaming ingestion go to:
         https://docs.microsoft.com/en-us/azure/data-explorer/ingest-data-streaming
         :param Optional[str] database: Target database. If not provided, will default to the "Initial Catalog" value in the connection string
         :param str table: Target table.
-        :param io.BaseIO stream: stream object which contains the data to ingest.
+        :param Optional[IO[AnyStr]] stream: a stream object or which contains the data to ingest.
+        :param Optional[str] blob_url: An url to a blob which contains the data to ingest. Provide either this or stream.
         :param DataFormat stream_format: Format of the data in the stream.
         :param ClientRequestProperties properties: additional request properties.
         :param str mapping_name: Pre-defined mapping of the table. Required when stream_format is json/avro.
         """
         database = self._get_database_or_default(database)
-        Span.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
 
         stream_format = stream_format.kusto_value if isinstance(stream_format, DataFormat) else DataFormat[stream_format.upper()].kusto_value
         endpoint = self._streaming_ingest_endpoint + database + "/" + table + "?streamFormat=" + stream_format
         if mapping_name is not None:
             endpoint = endpoint + "&mappingName=" + mapping_name
+        if blob_url:
+            endpoint += "&sourceKind=uri"
+            request = ExecuteRequestParams._from_blob_url(
+                blob_url,
+                properties,
+                self._request_headers,
+                self._streaming_ingest_default_timeout,
+                self._mgmt_default_timeout,
+                self._client_server_delta,
+                self.client_details,
+            )
+        elif stream:
+            request = ExecuteRequestParams._from_stream(
+                stream,
+                properties,
+                self._request_headers,
+                self._streaming_ingest_default_timeout,
+                self._mgmt_default_timeout,
+                self._client_server_delta,
+                self.client_details,
+            )
+        else:
+            raise Exception("execute_streaming_ingest is expecting either a stream or blob url")
 
-        self._execute(endpoint, database, None, stream, self._streaming_ingest_default_timeout, properties)
+        Span.set_streaming_ingest_attributes(self._kusto_cluster, database, table, properties)
+        self._execute(endpoint, request, properties)
 
     def _execute_streaming_query_parsed(
         self,
         database: Optional[str],
         query: str,
         timeout: timedelta = _KustoClientBase._query_default_timeout,
         properties: Optional[ClientRequestProperties] = None,
     ) -> StreamingDataSetEnumerator:
-        response = self._execute(self._query_endpoint, database, query, None, timeout, properties, stream_response=True)
+        request = ExecuteRequestParams._from_query(
+            query, database, properties, self._request_headers, timeout, self._mgmt_default_timeout, self._client_server_delta, self.client_details
+        )
+        response = self._execute(self._query_endpoint, request, properties, stream_response=True)
         response.raw.decode_content = True
         return StreamingDataSetEnumerator(JsonTokenReader(response.raw))
 
     @distributed_trace(name_of_span="KustoClient.streaming_query", kind=SpanKind.CLIENT)
     def execute_streaming_query(
         self,
         database: Optional[str],
@@ -258,49 +304,34 @@
         Span.set_query_attributes(self._kusto_cluster, database, properties)
 
         return KustoStreamingResponseDataSet(self._execute_streaming_query_parsed(database, query, timeout, properties))
 
     def _execute(
         self,
         endpoint: str,
-        database: Optional[str],
-        query: Optional[str],
-        payload: Optional[IO[AnyStr]],
-        timeout: timedelta,
+        request: ExecuteRequestParams,
         properties: Optional[ClientRequestProperties] = None,
         stream_response: bool = False,
     ) -> Union[KustoResponseDataSet, Response]:
         """Executes given query against this client"""
         if self._is_closed:
             raise KustoClosedError()
         self.validate_endpoint()
-        request_params = ExecuteRequestParams(
-            database,
-            payload,
-            properties,
-            query,
-            timeout,
-            self._request_headers,
-            self._mgmt_default_timeout,
-            self._client_server_delta,
-            self.client_details,
-        )
-        json_payload = request_params.json_payload
-        request_headers = request_params.request_headers
-        timeout = request_params.timeout
+
+        request_headers = request.request_headers
         if self._aad_helper:
             request_headers["Authorization"] = self._aad_helper.acquire_authorization_header()
 
         # trace http post call for response
         invoker = lambda: self._session.post(
             endpoint,
             headers=request_headers,
-            json=json_payload,
-            data=payload,
-            timeout=timeout.seconds,
+            json=request.json_payload,
+            data=request.payload,
+            timeout=request.timeout.seconds,
             stream=stream_response,
             allow_redirects=False,
         )
 
         try:
             response = MonitoredActivity.invoke(
                 invoker, name_of_span="KustoClient.http_post", tracing_attributes=Span.create_http_attributes("POST", endpoint, request_headers)
@@ -320,10 +351,10 @@
         response_json = None
         try:
             if 300 <= response.status_code < 400:
                 raise Exception("Unexpected redirection, got status code: " + str(response.status))
             response_json = response.json()
             response.raise_for_status()
         except Exception as e:
-            raise self._handle_http_error(e, endpoint, payload, response, response.status_code, response_json, response.text)
+            raise self._handle_http_error(e, endpoint, request.payload, response, response.status_code, response_json, response.text)
         # trace response processing
         return MonitoredActivity.invoke(lambda: self._kusto_parse_by_endpoint(endpoint, response_json), name_of_span="KustoClient.processing_response")
```

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/client_base.py` & `azure-kusto-data-4.4.0/azure/kusto/data/client_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -121,44 +121,90 @@
         if response_text:
             raise KustoServiceError(response_text, response) from exception
 
         raise KustoServiceError("Server error response contains no data.", response) from exception
 
 
 class ExecuteRequestParams:
-    def __init__(
-        self,
-        database: str,
-        payload: Optional[io.IOBase],
+    @staticmethod
+    def _from_stream(
+        stream: io.IOBase,
         properties: ClientRequestProperties,
+        request_headers: Any,
+        timeout: timedelta,
+        mgmt_default_timeout: timedelta,
+        client_server_delta: timedelta,
+        client_details: ClientDetails,
+    ):
+        # Before 3.0 it was KPC.execute_streaming_ingest, but was changed to align with the other SDKs
+        client_request_id_prefix = "KPC.executeStreamingIngest;"
+        request_headers = request_headers.copy()
+        request_headers["Content-Encoding"] = "gzip"
+        if properties:
+            request_headers.update(json.loads(properties.to_json())["Options"])
+
+        return ExecuteRequestParams(
+            stream, None, request_headers, client_request_id_prefix, properties, timeout, mgmt_default_timeout, client_server_delta, client_details
+        )
+
+    @staticmethod
+    def _from_query(
         query: str,
+        database: str,
+        properties: ClientRequestProperties,
+        request_headers: Any,
         timeout: timedelta,
-        request_headers: dict,
         mgmt_default_timeout: timedelta,
         client_server_delta: timedelta,
         client_details: ClientDetails,
     ):
-        request_headers = copy(request_headers)
-        request_headers["Connection"] = "Keep-Alive"
-        json_payload = None
-        if not payload:
-            json_payload = {"db": database, "csl": query}
-            if properties:
-                json_payload["properties"] = properties.to_json()
-
-            client_request_id_prefix = "KPC.execute;"
-            request_headers["Content-Type"] = "application/json; charset=utf-8"
-        else:
-            if properties:
-                request_headers.update(json.loads(properties.to_json())["Options"])
-
-            # Before 3.0 it was KPC.execute_streaming_ingest, but was changed to align with the other SDKs
-            client_request_id_prefix = "KPC.executeStreamingIngest;"
-            request_headers["Content-Encoding"] = "gzip"
+        json_payload = {"db": database, "csl": query}
+        if properties:
+            json_payload["properties"] = properties.to_json()
+
+        client_request_id_prefix = "KPC.execute;"
+        request_headers = request_headers.copy()
+        request_headers["Content-Type"] = "application/json; charset=utf-8"
+
+        return ExecuteRequestParams(
+            None, json_payload, request_headers, client_request_id_prefix, properties, timeout, mgmt_default_timeout, client_server_delta, client_details
+        )
+
+    @staticmethod
+    def _from_blob_url(
+        blob: str,
+        properties: ClientRequestProperties,
+        request_headers: Any,
+        timeout: timedelta,
+        mgmt_default_timeout: timedelta,
+        client_server_delta: timedelta,
+        client_details: ClientDetails,
+    ):
+        json_payload = {"sourceUri": blob}
+        client_request_id_prefix = "KPC.executeStreamingIngestFromBlob;"
+        request_headers = request_headers.copy()
+        request_headers["Content-Type"] = "application/json; charset=utf-8"
+        if properties:
+            request_headers.update(json.loads(properties.to_json())["Options"])
+        return ExecuteRequestParams(
+            None, json_payload, request_headers, client_request_id_prefix, properties, timeout, mgmt_default_timeout, client_server_delta, client_details
+        )
 
+    def __init__(
+        self,
+        payload,
+        json_payload,
+        request_headers,
+        client_request_id_prefix,
+        properties: ClientRequestProperties,
+        timeout: timedelta,
+        mgmt_default_timeout: timedelta,
+        client_server_delta: timedelta,
+        client_details: ClientDetails,
+    ):
         special_headers = [
             {
                 "name": "x-ms-client-request-id",
                 "value": client_request_id_prefix + str(uuid.uuid4()),
                 "property": lambda p: p.client_request_id,
             },
             {
@@ -197,7 +243,8 @@
                 timeout = properties.get_option(ClientRequestProperties.request_timeout_option_name, timeout)
 
         timeout = (timeout or mgmt_default_timeout) + client_server_delta
 
         self.json_payload = json_payload
         self.request_headers = request_headers
         self.timeout = timeout
+        self.payload = payload
```

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/client_details.py` & `azure-kusto-data-4.4.0/azure/kusto/data/client_details.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/client_request_properties.py` & `azure-kusto-data-4.4.0/azure/kusto/data/client_request_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/data_format.py` & `azure-kusto-data-4.4.0/azure/kusto/data/data_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     SOHSV = ("sohsv", IngestionMappingKind.CSV, True)
     PSV = ("psv", IngestionMappingKind.CSV, True)
     TXT = ("txt", IngestionMappingKind.CSV, True)
     TSVE = ("tsve", IngestionMappingKind.CSV, True)
     JSON = ("json", IngestionMappingKind.JSON, True)
     SINGLEJSON = ("singlejson", IngestionMappingKind.JSON, True)
     MULTIJSON = ("multijson", IngestionMappingKind.JSON, True)
-    AVRO = ("avro", IngestionMappingKind.AVRO, True)
-    APACHEAVRO = ("apacheavro", IngestionMappingKind.APACHEAVRO, True)
+    AVRO = ("avro", IngestionMappingKind.AVRO, False)
+    APACHEAVRO = ("apacheavro", IngestionMappingKind.APACHEAVRO, False)
     PARQUET = ("parquet", IngestionMappingKind.PARQUET, False)
     SSTREAM = ("sstream", IngestionMappingKind.SSTREAM, False)
     ORC = ("orc", IngestionMappingKind.ORC, False)
     RAW = ("raw", IngestionMappingKind.CSV, True)
     W3CLOGFILE = ("w3clogfile", IngestionMappingKind.W3CLOGFILE, True)
 
     def __init__(self, kusto_value: str, ingestion_mapping_kind: IngestionMappingKind, compressible: bool):
```

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/env_utils.py` & `azure-kusto-data-4.4.0/azure/kusto/data/env_utils.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/exceptions.py` & `azure-kusto-data-4.4.0/azure/kusto/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/helpers.py` & `azure-kusto-data-4.4.0/azure/kusto/data/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         raise TypeError("Expected KustoResultTable or KustoStreamingResultTable got {}".format(type(table).__name__))
 
     columns = [col.column_name for col in table.columns]
     frame = pd.DataFrame(table.raw_rows, columns=columns)
 
     # fix types
     for col in table.columns:
+        if col.column_type == "string" and hasattr(pd, "StringDType"):
+            frame[col.column_name] = frame[col.column_name].astype(pd.StringDType())
         if col.column_type == "bool":
             frame[col.column_name] = frame[col.column_name].astype(pd.BooleanDtype() if nullable_bools else bool)
         elif col.column_type == "int":
             frame[col.column_name] = frame[col.column_name].astype(pd.Int32Dtype())
         elif col.column_type == "long":
             frame[col.column_name] = frame[col.column_name].astype(pd.Int64Dtype())
         elif col.column_type == "real" or col.column_type == "decimal":
```

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/kcsb.py` & `azure-kusto-data-4.4.0/azure/kusto/data/kcsb.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/kusto_trusted_endpoints.py` & `azure-kusto-data-4.4.0/azure/kusto/data/kusto_trusted_endpoints.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/response.py` & `azure-kusto-data-4.4.0/azure/kusto/data/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/security.py` & `azure-kusto-data-4.4.0/azure/kusto/data/security.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/streaming_response.py` & `azure-kusto-data-4.4.0/azure/kusto/data/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure/kusto/data/wellKnownKustoEndpoints.json` & `azure-kusto-data-4.4.0/azure/kusto/data/wellKnownKustoEndpoints.json`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.3.1/azure_kusto_data.egg-info/PKG-INFO` & `azure-kusto-data-4.4.0/azure_kusto_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.3.1
+Version: 4.4.0
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.3.1/azure_kusto_data.egg-info/SOURCES.txt` & `azure-kusto-data-4.4.0/azure_kusto_data.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,11 +33,8 @@
 azure/kusto/data/aio/response.py
 azure/kusto/data/aio/streaming_response.py
 azure_kusto_data.egg-info/PKG-INFO
 azure_kusto_data.egg-info/SOURCES.txt
 azure_kusto_data.egg-info/dependency_links.txt
 azure_kusto_data.egg-info/namespace_packages.txt
 azure_kusto_data.egg-info/requires.txt
-azure_kusto_data.egg-info/top_level.txt
-tests/aio/__init__.py
-tests/aio/test_async_token_providers.py
-tests/aio/test_kusto_client.py
+azure_kusto_data.egg-info/top_level.txt
```

### Comparing `azure-kusto-data-4.3.1/setup.py` & `azure-kusto-data-4.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,13 +40,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     namespace_packages=["azure"],
     keywords="kusto wrapper client library",
-    packages=find_packages(exclude=["azure", "tests"]),
+    packages=find_packages(exclude=["azure", "*tests*", "*tests.*"]),
     package_data={"": ["wellKnownKustoEndpoints.json"]},
     include_package_data=True,
     install_requires=["python-dateutil>=2.8.0", "requests>=2.13.0", "azure-identity>=1.5.0,<2", "msal>=1.9.0,<2", "ijson~=3.1", "azure-core>=1.11.0,<2"],
     extras_require={"pandas": ["pandas"], "aio": ["aiohttp>=3.8.0,<4", "asgiref>=3.2.3,<4"]},
 )
```

