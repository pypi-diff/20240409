# Comparing `tmp/vents-0.4.0.tar.gz` & `tmp/vents-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.4.0.tar", last modified: Wed Nov 29 13:10:54 2023, max compression
+gzip compressed data, was "vents-0.4.1.tar", last modified: Tue Apr  9 10:58:32 2024, max compression
```

## Comparing `vents-0.4.0.tar` & `vents-0.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.925463 vents-0.4.0/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-11-29 13:09:54.000000 vents-0.4.0/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1725 2023-11-29 13:10:54.925383 vents-0.4.0/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-11-29 13:10:54.925838 vents-0.4.0/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-11-29 13:09:54.000000 vents-0.4.0/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.920865 vents-0.4.0/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-11-29 13:09:54.000000 vents-0.4.0/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     5003 2023-11-29 13:09:54.000000 vents-0.4.0/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.922178 vents-0.4.0/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      335 2023-11-29 13:09:54.000000 vents-0.4.0/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2501 2023-11-29 13:09:54.000000 vents-0.4.0/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     3858 2023-11-29 13:09:54.000000 vents-0.4.0/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)      529 2023-11-29 13:09:54.000000 vents-0.4.0/vents/connections/connection_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)     3505 2023-11-29 13:09:54.000000 vents-0.4.0/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-11-29 13:09:54.000000 vents-0.4.0/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.923316 vents-0.4.0/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-11-29 13:09:54.000000 vents-0.4.0/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      246 2023-11-29 13:09:54.000000 vents-0.4.0/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.923710 vents-0.4.0/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.924196 vents-0.4.0/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1650 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.924675 vents-0.4.0/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1636 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.925144 vents-0.4.0/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-11-29 13:09:54.000000 vents-0.4.0/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-11-29 13:09:54.000000 vents-0.4.0/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-11-29 13:09:54.000000 vents-0.4.0/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-11-29 13:10:54.921494 vents-0.4.0/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1725 2023-11-29 13:10:54.000000 vents-0.4.0/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-11-29 13:10:54.000000 vents-0.4.0/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-11-29 13:10:54.000000 vents-0.4.0/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       69 2023-11-29 13:10:54.000000 vents-0.4.0/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-11-29 13:10:54.000000 vents-0.4.0/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.026483 vents-0.4.1/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2024-04-09 10:56:34.000000 vents-0.4.1/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1725 2024-04-09 10:58:32.026416 vents-0.4.1/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2024-04-09 10:58:32.026874 vents-0.4.1/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2024-04-09 10:56:34.000000 vents-0.4.1/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.021208 vents-0.4.1/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2024-04-09 10:56:34.000000 vents-0.4.1/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5003 2024-04-09 10:56:34.000000 vents-0.4.1/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.022769 vents-0.4.1/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      335 2024-04-09 10:56:34.000000 vents-0.4.1/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2501 2024-04-09 10:56:34.000000 vents-0.4.1/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3932 2024-04-09 10:56:34.000000 vents-0.4.1/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)      529 2024-04-09 10:56:34.000000 vents-0.4.1/vents/connections/connection_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3505 2024-04-09 10:56:34.000000 vents-0.4.1/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2024-04-09 10:56:34.000000 vents-0.4.1/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.024123 vents-0.4.1/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2024-04-09 10:56:34.000000 vents-0.4.1/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      246 2024-04-09 10:56:34.000000 vents-0.4.1/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.024529 vents-0.4.1/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.025066 vents-0.4.1/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1650 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.025591 vents-0.4.1/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1636 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.026129 vents-0.4.1/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2024-04-09 10:56:34.000000 vents-0.4.1/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2024-04-09 10:56:34.000000 vents-0.4.1/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2024-04-09 10:56:34.000000 vents-0.4.1/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2024-04-09 10:58:32.021966 vents-0.4.1/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1725 2024-04-09 10:58:31.000000 vents-0.4.1/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1216 2024-04-09 10:58:31.000000 vents-0.4.1/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2024-04-09 10:58:31.000000 vents-0.4.1/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       69 2024-04-09 10:58:31.000000 vents-0.4.1/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2024-04-09 10:58:31.000000 vents-0.4.1/vents.egg-info/top_level.txt
```

### Comparing `vents-0.4.0/PKG-INFO` & `vents-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.4.0
+Version: 0.4.1
 Summary: Open source connections, integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.4.0/setup.cfg` & `vents-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/setup.py` & `vents-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/config.py` & `vents-0.4.1/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/connections/catalog.py` & `vents-0.4.1/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/connections/connection.py` & `vents-0.4.1/vents/connections/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, ClassVar
 from typing_extensions import Literal
 
 from clipped.compact.pydantic import Field, StrictStr
 from clipped.config.schema import BaseSchemaModel
 from clipped.types.ref_or_obj import RefField
 
 from vents.connections.connection_resource import ConnectionResource
@@ -11,14 +11,15 @@
 
 
 class Connection(BaseSchemaModel):
     _IDENTIFIER = "connection"
 
     name: StrictStr
     kind: ProviderKind
+    is_alias: ClassVar[Optional[bool]] = Field(alias="isAlias")
     description: Optional[StrictStr]
     tags: Optional[Union[List[StrictStr], RefField]]
     schema_: Optional[ConnectionSchema] = Field(alias="schema")
     secret: Optional[Union[ConnectionResource, RefField]]
     config_map: Optional[Union[ConnectionResource, RefField]] = Field(alias="configMap")
     env: Optional[Union[List[Dict], RefField]]
     annotations: Optional[Union[Dict, RefField]]
```

### Comparing `vents-0.4.0/vents/connections/connection_resource.py` & `vents-0.4.1/vents/connections/connection_resource.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/connections/connection_schema.py` & `vents-0.4.1/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/__init__.py` & `vents-0.4.1/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/base.py` & `vents-0.4.1/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/discord_webhook.py` & `vents-0.4.1/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/hipchat_webhook.py` & `vents-0.4.1/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/mattermost_webhook.py` & `vents-0.4.1/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/pagerduty_webhook.py` & `vents-0.4.1/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/slack_webhook.py` & `vents-0.4.1/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/notifiers/webhook.py` & `vents-0.4.1/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/aws/base.py` & `vents-0.4.1/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/aws/s3.py` & `vents-0.4.1/vents/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/aws/service.py` & `vents-0.4.1/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/azure/base.py` & `vents-0.4.1/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/azure/blob_storage.py` & `vents-0.4.1/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/azure/service.py` & `vents-0.4.1/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/base.py` & `vents-0.4.1/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/gcp/base.py` & `vents-0.4.1/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/gcp/gcs.py` & `vents-0.4.1/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/gcp/service.py` & `vents-0.4.1/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents/providers/kinds.py` & `vents-0.4.1/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.4.0/vents.egg-info/PKG-INFO` & `vents-0.4.1/vents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.4.0
+Version: 0.4.1
 Summary: Open source connections, integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.4.0/vents.egg-info/SOURCES.txt` & `vents-0.4.1/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

