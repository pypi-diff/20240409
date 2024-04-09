# Comparing `tmp/mypy-boto3-mediaconvert-1.34.33.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.34.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.34.33.tar", last modified: Thu Feb  1 20:47:06 2024, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.34.81.tar", last modified: Tue Apr  9 19:32:46 2024, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.34.33.tar` & `mypy-boto3-mediaconvert-1.34.81.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:47:06.660686 mypy-boto3-mediaconvert-1.34.33/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-02-01 20:47:06.660686 mypy-boto3-mediaconvert-1.34.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:47:06.660686 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22527 2024-02-01 20:46:50.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22524 2024-02-01 20:46:50.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    57849 2024-02-01 20:46:51.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    57849 2024-02-01 20:46:50.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-02-01 20:46:50.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-01 20:46:50.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   150688 2024-02-01 20:46:53.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   150688 2024-02-01 20:46:53.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 20:47:06.660686 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-02-01 20:47:06.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-01 20:47:06.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 20:47:06.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 20:47:06.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-01 20:47:06.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-01 20:47:06.000000 mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 20:47:06.660686 mypy-boto3-mediaconvert-1.34.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-02-01 20:46:49.000000 mypy-boto3-mediaconvert-1.34.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.356502 mypy-boto3-mediaconvert-1.34.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-09 19:32:46.356502 mypy-boto3-mediaconvert-1.34.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.356502 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22527 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22524 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    58068 2024-04-09 19:32:14.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58068 2024-04-09 19:32:13.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   151253 2024-04-09 19:32:16.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151253 2024-04-09 19:32:15.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.356502 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-09 19:32:46.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 19:32:46.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:46.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:46.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:32:46.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 19:32:46.000000 mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:32:46.356502 mypy-boto3-mediaconvert-1.34.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-09 19:32:12.000000 mypy-boto3-mediaconvert-1.34.81/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/LICENSE` & `mypy-boto3-mediaconvert-1.34.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/PKG-INFO` & `mypy-boto3-mediaconvert-1.34.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.34.33
-Summary: Type annotations for boto3.MediaConvert 1.34.33 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.81
+Summary: Type annotations for boto3.MediaConvert 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.34.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/README.md` & `mypy-boto3-mediaconvert-1.34.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.34.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.34.33\n"
-        "Version:         1.34.33\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.MediaConvert 1.34.81\n"
+        "Version:         1.34.81\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.33")
+    print("1.34.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,15 @@
     "M2tsEbpAudioIntervalType",
     "M2tsEbpPlacementType",
     "M2tsEsRateInPesType",
     "M2tsForceTsVideoEbpOrderType",
     "M2tsKlvMetadataType",
     "M2tsNielsenId3Type",
     "M2tsPcrControlType",
+    "M2tsPreventBufferUnderflowType",
     "M2tsRateModeType",
     "M2tsScte35SourceType",
     "M2tsSegmentationMarkersType",
     "M2tsSegmentationStyleType",
     "M3u8AudioDurationType",
     "M3u8DataPtsControlType",
     "M3u8NielsenId3Type",
@@ -1113,14 +1114,15 @@
 M2tsEbpAudioIntervalType = Literal["VIDEO_AND_FIXED_INTERVALS", "VIDEO_INTERVAL"]
 M2tsEbpPlacementType = Literal["VIDEO_AND_AUDIO_PIDS", "VIDEO_PID"]
 M2tsEsRateInPesType = Literal["EXCLUDE", "INCLUDE"]
 M2tsForceTsVideoEbpOrderType = Literal["DEFAULT", "FORCE"]
 M2tsKlvMetadataType = Literal["NONE", "PASSTHROUGH"]
 M2tsNielsenId3Type = Literal["INSERT", "NONE"]
 M2tsPcrControlType = Literal["CONFIGURED_PCR_PERIOD", "PCR_EVERY_PES_PACKET"]
+M2tsPreventBufferUnderflowType = Literal["DISABLED", "ENABLED"]
 M2tsRateModeType = Literal["CBR", "VBR"]
 M2tsScte35SourceType = Literal["NONE", "PASSTHROUGH"]
 M2tsSegmentationMarkersType = Literal[
     "EBP", "EBP_LEGACY", "NONE", "PSI_SEGSTART", "RAI_ADAPT", "RAI_SEGSTART"
 ]
 M2tsSegmentationStyleType = Literal["MAINTAIN_CADENCE", "RESET_CADENCE"]
 M3u8AudioDurationType = Literal["DEFAULT_CODEC_DURATION", "MATCH_VIDEO_DURATION"]
@@ -1393,14 +1395,15 @@
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
@@ -1411,14 +1414,15 @@
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
@@ -1436,14 +1440,15 @@
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
@@ -1456,24 +1461,26 @@
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
@@ -1534,15 +1541,14 @@
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
@@ -1722,14 +1728,15 @@
     "sts",
     "supplychain",
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
@@ -1776,13 +1783,14 @@
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,15 @@
     "M2tsEbpAudioIntervalType",
     "M2tsEbpPlacementType",
     "M2tsEsRateInPesType",
     "M2tsForceTsVideoEbpOrderType",
     "M2tsKlvMetadataType",
     "M2tsNielsenId3Type",
     "M2tsPcrControlType",
+    "M2tsPreventBufferUnderflowType",
     "M2tsRateModeType",
     "M2tsScte35SourceType",
     "M2tsSegmentationMarkersType",
     "M2tsSegmentationStyleType",
     "M3u8AudioDurationType",
     "M3u8DataPtsControlType",
     "M3u8NielsenId3Type",
@@ -1113,14 +1114,15 @@
 M2tsEbpAudioIntervalType = Literal["VIDEO_AND_FIXED_INTERVALS", "VIDEO_INTERVAL"]
 M2tsEbpPlacementType = Literal["VIDEO_AND_AUDIO_PIDS", "VIDEO_PID"]
 M2tsEsRateInPesType = Literal["EXCLUDE", "INCLUDE"]
 M2tsForceTsVideoEbpOrderType = Literal["DEFAULT", "FORCE"]
 M2tsKlvMetadataType = Literal["NONE", "PASSTHROUGH"]
 M2tsNielsenId3Type = Literal["INSERT", "NONE"]
 M2tsPcrControlType = Literal["CONFIGURED_PCR_PERIOD", "PCR_EVERY_PES_PACKET"]
+M2tsPreventBufferUnderflowType = Literal["DISABLED", "ENABLED"]
 M2tsRateModeType = Literal["CBR", "VBR"]
 M2tsScte35SourceType = Literal["NONE", "PASSTHROUGH"]
 M2tsSegmentationMarkersType = Literal[
     "EBP", "EBP_LEGACY", "NONE", "PSI_SEGSTART", "RAI_ADAPT", "RAI_SEGSTART"
 ]
 M2tsSegmentationStyleType = Literal["MAINTAIN_CADENCE", "RESET_CADENCE"]
 M3u8AudioDurationType = Literal["DEFAULT_CODEC_DURATION", "MATCH_VIDEO_DURATION"]
@@ -1393,14 +1395,15 @@
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
@@ -1411,14 +1414,15 @@
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
@@ -1436,14 +1440,15 @@
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
@@ -1456,24 +1461,26 @@
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
@@ -1534,15 +1541,14 @@
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
@@ -1722,14 +1728,15 @@
     "sts",
     "supplychain",
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
@@ -1776,13 +1783,14 @@
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,15 @@
     M2tsEbpAudioIntervalType,
     M2tsEbpPlacementType,
     M2tsEsRateInPesType,
     M2tsForceTsVideoEbpOrderType,
     M2tsKlvMetadataType,
     M2tsNielsenId3Type,
     M2tsPcrControlType,
+    M2tsPreventBufferUnderflowType,
     M2tsRateModeType,
     M2tsScte35SourceType,
     M2tsSegmentationMarkersType,
     M2tsSegmentationStyleType,
     M3u8AudioDurationType,
     M3u8DataPtsControlType,
     M3u8NielsenId3Type,
@@ -1003,14 +1004,18 @@
     {
         "Alignment": NotRequired[BurninSubtitleAlignmentType],
         "ApplyFontColor": NotRequired[BurninSubtitleApplyFontColorType],
         "BackgroundColor": NotRequired[BurninSubtitleBackgroundColorType],
         "BackgroundOpacity": NotRequired[int],
         "FallbackFont": NotRequired[BurninSubtitleFallbackFontType],
         "FontColor": NotRequired[BurninSubtitleFontColorType],
+        "FontFileBold": NotRequired[str],
+        "FontFileBoldItalic": NotRequired[str],
+        "FontFileItalic": NotRequired[str],
+        "FontFileRegular": NotRequired[str],
         "FontOpacity": NotRequired[int],
         "FontResolution": NotRequired[int],
         "FontScript": NotRequired[FontScriptType],
         "FontSize": NotRequired[int],
         "HexFontColor": NotRequired[str],
         "OutlineColor": NotRequired[BurninSubtitleOutlineColorType],
         "OutlineSize": NotRequired[int],
@@ -1038,14 +1043,18 @@
         "BackgroundColor": NotRequired[DvbSubtitleBackgroundColorType],
         "BackgroundOpacity": NotRequired[int],
         "DdsHandling": NotRequired[DvbddsHandlingType],
         "DdsXCoordinate": NotRequired[int],
         "DdsYCoordinate": NotRequired[int],
         "FallbackFont": NotRequired[DvbSubSubtitleFallbackFontType],
         "FontColor": NotRequired[DvbSubtitleFontColorType],
+        "FontFileBold": NotRequired[str],
+        "FontFileBoldItalic": NotRequired[str],
+        "FontFileItalic": NotRequired[str],
+        "FontFileRegular": NotRequired[str],
         "FontOpacity": NotRequired[int],
         "FontResolution": NotRequired[int],
         "FontScript": NotRequired[FontScriptType],
         "FontSize": NotRequired[int],
         "Height": NotRequired[int],
         "HexFontColor": NotRequired[str],
         "OutlineColor": NotRequired[DvbSubtitleOutlineColorType],
@@ -1383,18 +1392,18 @@
         "WaitMinutes": NotRequired[int],
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
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
@@ -2643,14 +2652,15 @@
         "NielsenId3": NotRequired[M2tsNielsenId3Type],
         "NullPacketBitrate": NotRequired[float],
         "PatInterval": NotRequired[int],
         "PcrControl": NotRequired[M2tsPcrControlType],
         "PcrPid": NotRequired[int],
         "PmtInterval": NotRequired[int],
         "PmtPid": NotRequired[int],
+        "PreventBufferUnderflow": NotRequired[M2tsPreventBufferUnderflowType],
         "PrivateMetadataPid": NotRequired[int],
         "ProgramNumber": NotRequired[int],
         "PtsOffset": NotRequired[int],
         "PtsOffsetMode": NotRequired[TsPtsOffsetType],
         "RateMode": NotRequired[M2tsRateModeType],
         "Scte35Esam": NotRequired[M2tsScte35EsamTypeDef],
         "Scte35Pid": NotRequired[int],
@@ -2689,14 +2699,15 @@
         "NielsenId3": NotRequired[M2tsNielsenId3Type],
         "NullPacketBitrate": NotRequired[float],
         "PatInterval": NotRequired[int],
         "PcrControl": NotRequired[M2tsPcrControlType],
         "PcrPid": NotRequired[int],
         "PmtInterval": NotRequired[int],
         "PmtPid": NotRequired[int],
+        "PreventBufferUnderflow": NotRequired[M2tsPreventBufferUnderflowType],
         "PrivateMetadataPid": NotRequired[int],
         "ProgramNumber": NotRequired[int],
         "PtsOffset": NotRequired[int],
         "PtsOffsetMode": NotRequired[TsPtsOffsetType],
         "RateMode": NotRequired[M2tsRateModeType],
         "Scte35Esam": NotRequired[M2tsScte35EsamTypeDef],
         "Scte35Pid": NotRequired[int],
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,15 @@
     M2tsEbpAudioIntervalType,
     M2tsEbpPlacementType,
     M2tsEsRateInPesType,
     M2tsForceTsVideoEbpOrderType,
     M2tsKlvMetadataType,
     M2tsNielsenId3Type,
     M2tsPcrControlType,
+    M2tsPreventBufferUnderflowType,
     M2tsRateModeType,
     M2tsScte35SourceType,
     M2tsSegmentationMarkersType,
     M2tsSegmentationStyleType,
     M3u8AudioDurationType,
     M3u8DataPtsControlType,
     M3u8NielsenId3Type,
@@ -1003,14 +1004,18 @@
     {
         "Alignment": NotRequired[BurninSubtitleAlignmentType],
         "ApplyFontColor": NotRequired[BurninSubtitleApplyFontColorType],
         "BackgroundColor": NotRequired[BurninSubtitleBackgroundColorType],
         "BackgroundOpacity": NotRequired[int],
         "FallbackFont": NotRequired[BurninSubtitleFallbackFontType],
         "FontColor": NotRequired[BurninSubtitleFontColorType],
+        "FontFileBold": NotRequired[str],
+        "FontFileBoldItalic": NotRequired[str],
+        "FontFileItalic": NotRequired[str],
+        "FontFileRegular": NotRequired[str],
         "FontOpacity": NotRequired[int],
         "FontResolution": NotRequired[int],
         "FontScript": NotRequired[FontScriptType],
         "FontSize": NotRequired[int],
         "HexFontColor": NotRequired[str],
         "OutlineColor": NotRequired[BurninSubtitleOutlineColorType],
         "OutlineSize": NotRequired[int],
@@ -1038,14 +1043,18 @@
         "BackgroundColor": NotRequired[DvbSubtitleBackgroundColorType],
         "BackgroundOpacity": NotRequired[int],
         "DdsHandling": NotRequired[DvbddsHandlingType],
         "DdsXCoordinate": NotRequired[int],
         "DdsYCoordinate": NotRequired[int],
         "FallbackFont": NotRequired[DvbSubSubtitleFallbackFontType],
         "FontColor": NotRequired[DvbSubtitleFontColorType],
+        "FontFileBold": NotRequired[str],
+        "FontFileBoldItalic": NotRequired[str],
+        "FontFileItalic": NotRequired[str],
+        "FontFileRegular": NotRequired[str],
         "FontOpacity": NotRequired[int],
         "FontResolution": NotRequired[int],
         "FontScript": NotRequired[FontScriptType],
         "FontSize": NotRequired[int],
         "Height": NotRequired[int],
         "HexFontColor": NotRequired[str],
         "OutlineColor": NotRequired[DvbSubtitleOutlineColorType],
@@ -1383,18 +1392,18 @@
         "WaitMinutes": NotRequired[int],
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
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
@@ -2643,14 +2652,15 @@
         "NielsenId3": NotRequired[M2tsNielsenId3Type],
         "NullPacketBitrate": NotRequired[float],
         "PatInterval": NotRequired[int],
         "PcrControl": NotRequired[M2tsPcrControlType],
         "PcrPid": NotRequired[int],
         "PmtInterval": NotRequired[int],
         "PmtPid": NotRequired[int],
+        "PreventBufferUnderflow": NotRequired[M2tsPreventBufferUnderflowType],
         "PrivateMetadataPid": NotRequired[int],
         "ProgramNumber": NotRequired[int],
         "PtsOffset": NotRequired[int],
         "PtsOffsetMode": NotRequired[TsPtsOffsetType],
         "RateMode": NotRequired[M2tsRateModeType],
         "Scte35Esam": NotRequired[M2tsScte35EsamTypeDef],
         "Scte35Pid": NotRequired[int],
@@ -2689,14 +2699,15 @@
         "NielsenId3": NotRequired[M2tsNielsenId3Type],
         "NullPacketBitrate": NotRequired[float],
         "PatInterval": NotRequired[int],
         "PcrControl": NotRequired[M2tsPcrControlType],
         "PcrPid": NotRequired[int],
         "PmtInterval": NotRequired[int],
         "PmtPid": NotRequired[int],
+        "PreventBufferUnderflow": NotRequired[M2tsPreventBufferUnderflowType],
         "PrivateMetadataPid": NotRequired[int],
         "ProgramNumber": NotRequired[int],
         "PtsOffset": NotRequired[int],
         "PtsOffsetMode": NotRequired[TsPtsOffsetType],
         "RateMode": NotRequired[M2tsRateModeType],
         "Scte35Esam": NotRequired[M2tsScte35EsamTypeDef],
         "Scte35Pid": NotRequired[int],
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.34.33
-Summary: Type annotations for boto3.MediaConvert 1.34.33 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.81
+Summary: Type annotations for boto3.MediaConvert 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconvert)](https://pepy.tech/project/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.34.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mediaconvert-1.34.33/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.34.81/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.34.33/setup.py` & `mypy-boto3-mediaconvert-1.34.81/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.34.33",
+    version="1.34.81",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.MediaConvert 1.34.33 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.MediaConvert 1.34.81 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

