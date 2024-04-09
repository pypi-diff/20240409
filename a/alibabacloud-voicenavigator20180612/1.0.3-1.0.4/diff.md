# Comparing `tmp/alibabacloud_voicenavigator20180612-1.0.3.tar.gz` & `tmp/alibabacloud_voicenavigator20180612-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_voicenavigator20180612-1.0.3.tar", last modified: Sun Feb  4 17:12:31 2024, max compression
+gzip compressed data, was "dist/alibabacloud_voicenavigator20180612-1.0.4.tar", last modified: Tue Apr  9 17:15:42 2024, max compression
```

## Comparing `alibabacloud_voicenavigator20180612-1.0.3.tar` & `alibabacloud_voicenavigator20180612-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      231 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1224 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139039 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612/client.py
--rw-r--r--   0 root         (0) root         (0)   215904 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2666 2024-02-04 17:12:31.000000 alibabacloud_voicenavigator20180612-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      602 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139039 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612/client.py
+-rw-r--r--   0 root         (0) root         (0)   215904 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:15:42.000000 alibabacloud_voicenavigator20180612-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2666 2024-04-09 17:15:41.000000 alibabacloud_voicenavigator20180612-1.0.4/setup.py
```

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/LICENSE` & `alibabacloud_voicenavigator20180612-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/PKG-INFO` & `alibabacloud_voicenavigator20180612-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_voicenavigator20180612
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud VoiceNavigator (20180612) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/README-CN.md` & `alibabacloud_voicenavigator20180612-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/README.md` & `alibabacloud_voicenavigator20180612-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612/client.py` & `alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612/models.py` & `alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/alibabacloud_voicenavigator20180612.egg-info/PKG-INFO` & `alibabacloud_voicenavigator20180612-1.0.4/alibabacloud_voicenavigator20180612.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-voicenavigator20180612
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud VoiceNavigator (20180612) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_voicenavigator20180612-1.0.3/setup.py` & `alibabacloud_voicenavigator20180612-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_voicenavigator20180612.
 
-Created on 04/02/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_voicenavigator20180612"
 NAME = "alibabacloud_voicenavigator20180612" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud VoiceNavigator (20180612) SDK Library for Python"
```

