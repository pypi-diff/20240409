# Comparing `tmp/alibabacloud_sysom20231230_py2-1.0.0.tar.gz` & `tmp/alibabacloud_sysom20231230_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sysom20231230_py2-1.0.0.tar", last modified: Mon Jan 29 06:23:33 2024, max compression
+gzip compressed data, was "dist/alibabacloud_sysom20231230_py2-1.0.1.tar", last modified: Tue Apr  9 07:25:54 2024, max compression
```

## Comparing `alibabacloud_sysom20231230_py2-1.0.0.tar` & `alibabacloud_sysom20231230_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4843 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230/client.py
--rw-r--r--   0 root         (0) root         (0)    14255 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2024-01-29 06:23:33.000000 alibabacloud_sysom20231230_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230/client.py
+-rw-r--r--   0 root         (0) root         (0)    14255 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2024-04-09 07:25:54.000000 alibabacloud_sysom20231230_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/LICENSE` & `alibabacloud_sysom20231230_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/PKG-INFO` & `alibabacloud_sysom20231230_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sysom20231230_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud SysOM (20231230) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/README-CN.md` & `alibabacloud_sysom20231230_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/README.md` & `alibabacloud_sysom20231230_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230/client.py` & `alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230/models.py` & `alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/alibabacloud_sysom20231230_py2.egg-info/PKG-INFO` & `alibabacloud_sysom20231230_py2-1.0.1/alibabacloud_sysom20231230_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sysom20231230-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud SysOM (20231230) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sysom20231230_py2-1.0.0/setup.py` & `alibabacloud_sysom20231230_py2-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sysom20231230_py2.
 
-Created on 29/01/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sysom20231230"
 NAME = "alibabacloud_sysom20231230_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud SysOM (20231230) SDK Library for Python2"
```

