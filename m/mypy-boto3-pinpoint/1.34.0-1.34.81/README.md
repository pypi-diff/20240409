# Comparing `tmp/mypy-boto3-pinpoint-1.34.0.tar.gz` & `tmp/mypy-boto3-pinpoint-1.34.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-1.34.0.tar", last modified: Wed Dec 13 21:23:30 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-1.34.81.tar", last modified: Tue Apr  9 19:32:46 2024, max compression
```

## Comparing `mypy-boto3-pinpoint-1.34.0.tar` & `mypy-boto3-pinpoint-1.34.81.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:30.351319 mypy-boto3-pinpoint-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2023-12-13 21:23:30.351319 mypy-boto3-pinpoint-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:30.351319 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80195 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    80192 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   139160 2023-12-13 21:15:25.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   139159 2023-12-13 21:15:23.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:30.351319 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2023-12-13 21:23:30.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-13 21:23:30.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:30.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:30.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:30.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-13 21:23:30.000000 mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:30.351319 mypy-boto3-pinpoint-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-13 21:15:22.000000 mypy-boto3-pinpoint-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80216 2024-04-09 19:32:21.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80213 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-09 19:32:21.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-09 19:32:21.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   139262 2024-04-09 19:32:24.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139262 2024-04-09 19:32:23.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 19:32:46.000000 mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:32:46.708504 mypy-boto3-pinpoint-1.34.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 19:32:20.000000 mypy-boto3-pinpoint-1.34.81/setup.py
```

### Comparing `mypy-boto3-pinpoint-1.34.0/LICENSE` & `mypy-boto3-pinpoint-1.34.81/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-pinpoint-1.34.0/PKG-INFO` & `mypy-boto3-pinpoint-1.34.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.34.0
-Summary: Type annotations for boto3.Pinpoint 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.81
+Summary: Type annotations for boto3.Pinpoint 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-1.34.0/README.md` & `mypy-boto3-pinpoint-1.34.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/__main__.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pinpoint 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Pinpoint 1.34.81\n"
+        "Version:         1.34.81\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/client.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#create_journey)
         """
 
     def create_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
-        TemplateName: str
+        TemplateName: str,
     ) -> CreatePushTemplateResponseTypeDef:
         """
         Creates a message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_push_template)
@@ -675,15 +675,15 @@
         self,
         *,
         ApplicationId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetApplicationDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)
@@ -743,15 +743,15 @@
         *,
         ApplicationId: str,
         CampaignId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetCampaignDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to a
         campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_campaign_date_range_kpi)
@@ -930,15 +930,15 @@
         *,
         ApplicationId: str,
         JourneyId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetJourneyDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard engagement metric that
         applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)
@@ -948,15 +948,15 @@
     def get_journey_execution_activity_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard execution metric that
         applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_activity_metrics)
@@ -979,15 +979,15 @@
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_activity_metrics)
@@ -997,15 +997,15 @@
     def get_journey_run_execution_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_metrics)
@@ -1213,15 +1213,15 @@
 
     def list_templates(
         self,
         *,
         NextToken: str = ...,
         PageSize: str = ...,
         Prefix: str = ...,
-        TemplateType: str = ...
+        TemplateType: str = ...,
     ) -> ListTemplatesResponseTypeDef:
         """
         Retrieves information about all the message templates that are associated with
         your Amazon Pinpoint
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_templates)
@@ -1263,15 +1263,15 @@
         """
 
     def remove_attributes(
         self,
         *,
         ApplicationId: str,
         AttributeType: str,
-        UpdateAttributesRequest: UpdateAttributesRequestTypeDef
+        UpdateAttributesRequest: UpdateAttributesRequestTypeDef,
     ) -> RemoveAttributesResponseTypeDef:
         """
         Removes one or more custom attributes, of the same attribute type, from the
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.remove_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#remove_attributes)
@@ -1287,15 +1287,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_messages)
         """
 
     def send_otp_message(
         self,
         *,
         ApplicationId: str,
-        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef
+        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef,
     ) -> SendOTPMessageResponseTypeDef:
         """
         Send an OTP message See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/SendOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_otp_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_otp_message)
@@ -1383,30 +1383,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_apns_voip_channel)
         """
 
     def update_apns_voip_sandbox_channel(
         self,
         *,
         APNSVoipSandboxChannelRequest: APNSVoipSandboxChannelRequestTypeDef,
-        ApplicationId: str
+        ApplicationId: str,
     ) -> UpdateApnsVoipSandboxChannelResponseTypeDef:
         """
         Enables the APNs VoIP sandbox channel for an application or updates the status
         and settings of the APNs VoIP sandbox channel for an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_voip_sandbox_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_apns_voip_sandbox_channel)
         """
 
     def update_application_settings(
         self,
         *,
         ApplicationId: str,
-        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef
+        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef,
     ) -> UpdateApplicationSettingsResponseTypeDef:
         """
         Updates the settings for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_application_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_application_settings)
         """
@@ -1424,15 +1424,15 @@
         """
 
     def update_campaign(
         self,
         *,
         ApplicationId: str,
         CampaignId: str,
-        WriteCampaignRequest: WriteCampaignRequestTypeDef
+        WriteCampaignRequest: WriteCampaignRequestTypeDef,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates the configuration and other settings for a campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_campaign)
         """
@@ -1451,15 +1451,15 @@
 
     def update_email_template(
         self,
         *,
         EmailTemplateRequest: EmailTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateEmailTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         email
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_email_template)
@@ -1504,15 +1504,15 @@
 
     def update_in_app_template(
         self,
         *,
         InAppTemplateRequest: InAppTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateInAppTemplateResponseTypeDef:
         """
         Updates an existing message template for messages sent through the in-app
         message
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_in_app_template)
@@ -1541,30 +1541,30 @@
 
     def update_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdatePushTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_push_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_push_template)
         """
 
     def update_recommender_configuration(
         self,
         *,
         RecommenderId: str,
-        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef
+        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef,
     ) -> UpdateRecommenderConfigurationResponseTypeDef:
         """
         Updates an Amazon Pinpoint configuration for a recommender model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_recommender_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_recommender_configuration)
         """
@@ -1595,30 +1595,30 @@
 
     def update_sms_template(
         self,
         *,
         SMSTemplateRequest: SMSTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateSmsTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the SMS
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_sms_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_sms_template)
         """
 
     def update_template_active_version(
         self,
         *,
         TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,
         TemplateName: str,
-        TemplateType: str
+        TemplateType: str,
     ) -> UpdateTemplateActiveVersionResponseTypeDef:
         """
         Changes the status of a specific version of a message template to *active*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_template_active_version)
         """
@@ -1637,30 +1637,30 @@
 
     def update_voice_template(
         self,
         *,
         TemplateName: str,
         VoiceTemplateRequest: VoiceTemplateRequestTypeDef,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateVoiceTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         voice
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_voice_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_voice_template)
         """
 
     def verify_otp_message(
         self,
         *,
         ApplicationId: str,
-        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef
+        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef,
     ) -> VerifyOTPMessageResponseTypeDef:
         """
         Verify an OTP See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/VerifyOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.verify_otp_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#verify_otp_message)
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/client.pyi` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#create_journey)
         """
 
     def create_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
-        TemplateName: str
+        TemplateName: str,
     ) -> CreatePushTemplateResponseTypeDef:
         """
         Creates a message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.create_push_template)
@@ -672,15 +672,15 @@
         self,
         *,
         ApplicationId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetApplicationDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to
         an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_application_date_range_kpi)
@@ -740,15 +740,15 @@
         *,
         ApplicationId: str,
         CampaignId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetCampaignDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard metric that applies to a
         campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_campaign_date_range_kpi)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#get_campaign_date_range_kpi)
@@ -927,15 +927,15 @@
         *,
         ApplicationId: str,
         JourneyId: str,
         KpiName: str,
         EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: str = ...,
-        StartTime: TimestampTypeDef = ...
+        StartTime: TimestampTypeDef = ...,
     ) -> GetJourneyDateRangeKpiResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard engagement metric that
         applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_date_range_kpi)
@@ -945,15 +945,15 @@
     def get_journey_execution_activity_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard execution metric that
         applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_execution_activity_metrics)
@@ -976,15 +976,15 @@
         self,
         *,
         ApplicationId: str,
         JourneyActivityId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionActivityMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a journey
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_activity_metrics)
@@ -994,15 +994,15 @@
     def get_journey_run_execution_metrics(
         self,
         *,
         ApplicationId: str,
         JourneyId: str,
         RunId: str,
         NextToken: str = ...,
-        PageSize: str = ...
+        PageSize: str = ...,
     ) -> GetJourneyRunExecutionMetricsResponseTypeDef:
         """
         Retrieves (queries) pre-aggregated data for a standard run execution metric
         that applies to a
         journey.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.get_journey_run_execution_metrics)
@@ -1210,15 +1210,15 @@
 
     def list_templates(
         self,
         *,
         NextToken: str = ...,
         PageSize: str = ...,
         Prefix: str = ...,
-        TemplateType: str = ...
+        TemplateType: str = ...,
     ) -> ListTemplatesResponseTypeDef:
         """
         Retrieves information about all the message templates that are associated with
         your Amazon Pinpoint
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.list_templates)
@@ -1260,15 +1260,15 @@
         """
 
     def remove_attributes(
         self,
         *,
         ApplicationId: str,
         AttributeType: str,
-        UpdateAttributesRequest: UpdateAttributesRequestTypeDef
+        UpdateAttributesRequest: UpdateAttributesRequestTypeDef,
     ) -> RemoveAttributesResponseTypeDef:
         """
         Removes one or more custom attributes, of the same attribute type, from the
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.remove_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#remove_attributes)
@@ -1284,15 +1284,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_messages)
         """
 
     def send_otp_message(
         self,
         *,
         ApplicationId: str,
-        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef
+        SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef,
     ) -> SendOTPMessageResponseTypeDef:
         """
         Send an OTP message See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/SendOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.send_otp_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#send_otp_message)
@@ -1380,30 +1380,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_apns_voip_channel)
         """
 
     def update_apns_voip_sandbox_channel(
         self,
         *,
         APNSVoipSandboxChannelRequest: APNSVoipSandboxChannelRequestTypeDef,
-        ApplicationId: str
+        ApplicationId: str,
     ) -> UpdateApnsVoipSandboxChannelResponseTypeDef:
         """
         Enables the APNs VoIP sandbox channel for an application or updates the status
         and settings of the APNs VoIP sandbox channel for an
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_apns_voip_sandbox_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_apns_voip_sandbox_channel)
         """
 
     def update_application_settings(
         self,
         *,
         ApplicationId: str,
-        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef
+        WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef,
     ) -> UpdateApplicationSettingsResponseTypeDef:
         """
         Updates the settings for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_application_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_application_settings)
         """
@@ -1421,15 +1421,15 @@
         """
 
     def update_campaign(
         self,
         *,
         ApplicationId: str,
         CampaignId: str,
-        WriteCampaignRequest: WriteCampaignRequestTypeDef
+        WriteCampaignRequest: WriteCampaignRequestTypeDef,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates the configuration and other settings for a campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_campaign)
         """
@@ -1448,15 +1448,15 @@
 
     def update_email_template(
         self,
         *,
         EmailTemplateRequest: EmailTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateEmailTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         email
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_email_template)
@@ -1501,15 +1501,15 @@
 
     def update_in_app_template(
         self,
         *,
         InAppTemplateRequest: InAppTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateInAppTemplateResponseTypeDef:
         """
         Updates an existing message template for messages sent through the in-app
         message
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_in_app_template)
@@ -1538,30 +1538,30 @@
 
     def update_push_template(
         self,
         *,
         PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdatePushTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through a push
         notification
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_push_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_push_template)
         """
 
     def update_recommender_configuration(
         self,
         *,
         RecommenderId: str,
-        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef
+        UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef,
     ) -> UpdateRecommenderConfigurationResponseTypeDef:
         """
         Updates an Amazon Pinpoint configuration for a recommender model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_recommender_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_recommender_configuration)
         """
@@ -1592,30 +1592,30 @@
 
     def update_sms_template(
         self,
         *,
         SMSTemplateRequest: SMSTemplateRequestTypeDef,
         TemplateName: str,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateSmsTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the SMS
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_sms_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_sms_template)
         """
 
     def update_template_active_version(
         self,
         *,
         TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,
         TemplateName: str,
-        TemplateType: str
+        TemplateType: str,
     ) -> UpdateTemplateActiveVersionResponseTypeDef:
         """
         Changes the status of a specific version of a message template to *active*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_template_active_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_template_active_version)
         """
@@ -1634,30 +1634,30 @@
 
     def update_voice_template(
         self,
         *,
         TemplateName: str,
         VoiceTemplateRequest: VoiceTemplateRequestTypeDef,
         CreateNewVersion: bool = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateVoiceTemplateResponseTypeDef:
         """
         Updates an existing message template for messages that are sent through the
         voice
         channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.update_voice_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#update_voice_template)
         """
 
     def verify_otp_message(
         self,
         *,
         ApplicationId: str,
-        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef
+        VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef,
     ) -> VerifyOTPMessageResponseTypeDef:
         """
         Verify an OTP See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-2016-12-01/VerifyOTPMessage).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint.Client.verify_otp_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/client/#verify_otp_message)
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/literals.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionType",
     "AlignmentType",
     "AttributeTypeType",
     "ButtonActionType",
     "CampaignStatusType",
     "ChannelTypeType",
@@ -51,15 +50,14 @@
     "TypeType",
     "PinpointServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionType = Literal["DEEP_LINK", "OPEN_APP", "URL"]
 AlignmentType = Literal["CENTER", "LEFT", "RIGHT"]
 AttributeTypeType = Literal[
     "AFTER", "BEFORE", "BETWEEN", "CONTAINS", "EXCLUSIVE", "INCLUSIVE", "ON"
 ]
 ButtonActionType = Literal["CLOSE", "DEEP_LINK", "LINK"]
 CampaignStatusType = Literal[
@@ -161,14 +159,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -179,14 +178,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -204,14 +204,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -224,24 +225,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -302,15 +305,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -382,17 +384,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -482,19 +486,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/literals.pyi` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -177,14 +178,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -202,14 +204,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -222,24 +225,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -300,15 +305,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -380,17 +384,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -480,19 +486,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/type_defs.py` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ADMChannelRequestTypeDef",
     "ADMChannelResponseTypeDef",
     "ADMMessageTypeDef",
     "APNSChannelRequestTypeDef",
     "APNSChannelResponseTypeDef",
     "APNSMessageTypeDef",
@@ -948,18 +947,18 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": NotRequired[str],
         "HtmlPart": NotRequired[str],
@@ -1174,14 +1173,15 @@
         "Id": NotRequired[str],
         "Identity": NotRequired[str],
         "IsArchived": NotRequired[bool],
         "LastModifiedBy": NotRequired[str],
         "LastModifiedDate": NotRequired[str],
         "MessagesPerSecond": NotRequired[int],
         "RoleArn": NotRequired[str],
+        "OrchestrationSendingRoleArn": NotRequired[str],
         "Version": NotRequired[int],
     },
 )
 DeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "DeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1395,14 +1395,15 @@
     "EmailChannelRequestTypeDef",
     {
         "FromAddress": str,
         "Identity": str,
         "ConfigurationSet": NotRequired[str],
         "Enabled": NotRequired[bool],
         "RoleArn": NotRequired[str],
+        "OrchestrationSendingRoleArn": NotRequired[str],
     },
 )
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": NotRequired[str],
     },
@@ -3172,17 +3173,15 @@
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
-        "JourneyRunExecutionActivityMetricsResponse": (
-            JourneyRunExecutionActivityMetricsResponseTypeDef
-        ),
+        "JourneyRunExecutionActivityMetricsResponse": JourneyRunExecutionActivityMetricsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint/type_defs.pyi` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -947,18 +947,18 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 EmailTemplateRequestTypeDef = TypedDict(
     "EmailTemplateRequestTypeDef",
     {
         "DefaultSubstitutions": NotRequired[str],
         "HtmlPart": NotRequired[str],
@@ -1173,14 +1173,15 @@
         "Id": NotRequired[str],
         "Identity": NotRequired[str],
         "IsArchived": NotRequired[bool],
         "LastModifiedBy": NotRequired[str],
         "LastModifiedDate": NotRequired[str],
         "MessagesPerSecond": NotRequired[int],
         "RoleArn": NotRequired[str],
+        "OrchestrationSendingRoleArn": NotRequired[str],
         "Version": NotRequired[int],
     },
 )
 DeleteEmailTemplateRequestRequestTypeDef = TypedDict(
     "DeleteEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1394,14 +1395,15 @@
     "EmailChannelRequestTypeDef",
     {
         "FromAddress": str,
         "Identity": str,
         "ConfigurationSet": NotRequired[str],
         "Enabled": NotRequired[bool],
         "RoleArn": NotRequired[str],
+        "OrchestrationSendingRoleArn": NotRequired[str],
     },
 )
 JourneyEmailMessageTypeDef = TypedDict(
     "JourneyEmailMessageTypeDef",
     {
         "FromAddress": NotRequired[str],
     },
@@ -3171,17 +3173,15 @@
         "JourneyExecutionMetricsResponse": JourneyExecutionMetricsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetJourneyRunExecutionActivityMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionActivityMetricsResponseTypeDef",
     {
-        "JourneyRunExecutionActivityMetricsResponse": (
-            JourneyRunExecutionActivityMetricsResponseTypeDef
-        ),
+        "JourneyRunExecutionActivityMetricsResponse": JourneyRunExecutionActivityMetricsResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetJourneyRunExecutionMetricsResponseTypeDef = TypedDict(
     "GetJourneyRunExecutionMetricsResponseTypeDef",
     {
         "JourneyRunExecutionMetricsResponse": JourneyRunExecutionMetricsResponseTypeDef,
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint
-Version: 1.34.0
-Summary: Type annotations for boto3.Pinpoint 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.81
+Summary: Type annotations for boto3.Pinpoint 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-pinpoint"></a>
 
 # mypy-boto3-pinpoint
 
 [![PyPI - mypy-boto3-pinpoint](https://img.shields.io/pypi/v/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint)](https://pepy.tech/project/mypy-boto3-pinpoint)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pinpoint 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
+[boto3.Pinpoint 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pinpoint docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-pinpoint-1.34.0/mypy_boto3_pinpoint.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-1.34.81/mypy_boto3_pinpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-1.34.0/setup.py` & `mypy-boto3-pinpoint-1.34.81/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint",
-    version="1.34.0",
+    version="1.34.81",
     packages=["mypy_boto3_pinpoint"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Pinpoint 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.Pinpoint 1.34.81 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 pinpoint type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pinpoint": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

