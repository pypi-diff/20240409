# Comparing `tmp/alibabacloud_umeng-apm20220214-1.1.0.tar.gz` & `tmp/alibabacloud_umeng-apm20220214-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_umeng-apm20220214-1.1.0.tar", last modified: Fri Aug 11 09:51:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud_umeng-apm20220214-1.1.1.tar", last modified: Tue Apr  9 02:18:34 2024, max compression
```

## Comparing `alibabacloud_umeng-apm20220214-1.1.0.tar` & `alibabacloud_umeng-apm20220214-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 09:51:48.000000 alibabacloud_umeng-apm20220214-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      471 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-08-11 09:51:48.000000 alibabacloud_umeng-apm20220214-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 09:51:48.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41744 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214/client.py
--rw-r--r--   0 root         (0) root         (0)    58752 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 09:51:48.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-11 09:51:48.000000 alibabacloud_umeng-apm20220214-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2834 2023-08-11 09:51:47.000000 alibabacloud_umeng-apm20220214-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41744 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/client.py
+-rw-r--r--   0 root         (0) root         (0)    57226 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-04-09 02:18:34.000000 alibabacloud_umeng-apm20220214-1.1.1/setup.py
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/LICENSE` & `alibabacloud_umeng-apm20220214-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/PKG-INFO` & `alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_umeng-apm20220214
-Version: 1.1.0
+Name: alibabacloud-umeng-apm20220214
+Version: 1.1.1
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/umeng-apm-20220214/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/README-CN.md` & `alibabacloud_umeng-apm20220214-1.1.1/README-CN.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/umeng-apm-20220214/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/README.md` & `alibabacloud_umeng-apm20220214-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/umeng-apm-20220214/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214/client.py` & `alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214/models.py` & `alibabacloud_umeng-apm20220214-1.1.1/alibabacloud_umeng_apm20220214/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,17 +269,14 @@
         body: GetH5PageTrendResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -480,17 +477,14 @@
         body: GetLaunchTrendResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -679,17 +673,14 @@
         body: GetNativePageTrendResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -878,17 +869,14 @@
         body: GetNetworkTrendResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -965,17 +953,17 @@
         return self
 
 
 class GetStatTrendResponseBodyData(TeaModel):
     def __init__(
         self,
         affected_user_count: int = None,
-        affected_user_rate: int = None,
+        affected_user_rate: float = None,
         error_count: int = None,
-        error_rate: int = None,
+        error_rate: float = None,
         time_point: str = None,
     ):
         self.affected_user_count = affected_user_count
         self.affected_user_rate = affected_user_rate
         self.error_count = error_count
         self.error_rate = error_rate
         self.time_point = time_point
@@ -1077,17 +1065,14 @@
         body: GetStatTrendResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1284,17 +1269,14 @@
         body: GetSymUploadParamResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1471,17 +1453,14 @@
         body: GetTodayStatTrendResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1593,17 +1572,14 @@
         body: UpdateAlertPlanResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1804,17 +1780,14 @@
         body: UploadSymbolFileResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO` & `alibabacloud_umeng-apm20220214-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-umeng-apm20220214
-Version: 1.1.0
+Name: alibabacloud_umeng-apm20220214
+Version: 1.1.1
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/umeng-apm-20220214/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.0/setup.py` & `alibabacloud_umeng-apm20220214-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_umeng-apm20220214.
 
-Created on 11/08/2023
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_umeng_apm20220214"
 NAME = "alibabacloud_umeng-apm20220214" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud umeng-apm (20220214) SDK Library for Python"
@@ -38,15 +38,15 @@
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

