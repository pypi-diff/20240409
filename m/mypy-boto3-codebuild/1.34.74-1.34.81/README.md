# Comparing `tmp/mypy-boto3-codebuild-1.34.74.tar.gz` & `tmp/mypy-boto3-codebuild-1.34.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codebuild-1.34.74.tar", last modified: Fri Mar 29 19:18:23 2024, max compression
+gzip compressed data, was "mypy-boto3-codebuild-1.34.81.tar", last modified: Tue Apr  9 19:32:46 2024, max compression
```

## Comparing `mypy-boto3-codebuild-1.34.74.tar` & `mypy-boto3-codebuild-1.34.81.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:23.000138 mypy-boto3-codebuild-1.34.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-03-29 19:18:23.000138 mypy-boto3-codebuild-1.34.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:23.000138 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44830 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44827 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    58133 2024-03-29 19:17:43.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    58133 2024-03-29 19:17:43.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:18:23.000138 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-03-29 19:18:22.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 19:18:22.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:18:22.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:18:22.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 19:18:22.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-29 19:18:22.000000 mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:18:23.000138 mypy-boto3-codebuild-1.34.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-29 19:17:42.000000 mypy-boto3-codebuild-1.34.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.020500 mypy-boto3-codebuild-1.34.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-04-09 19:32:46.020500 mypy-boto3-codebuild-1.34.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.020500 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44830 2024-04-09 19:32:06.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44827 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-09 19:32:06.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-09 19:32:06.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-09 19:32:06.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-09 19:32:06.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    58133 2024-04-09 19:32:07.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58133 2024-04-09 19:32:07.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:46.020500 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-04-09 19:32:45.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-09 19:32:45.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:45.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:45.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:32:45.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 19:32:45.000000 mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:32:46.020500 mypy-boto3-codebuild-1.34.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-09 19:32:05.000000 mypy-boto3-codebuild-1.34.81/setup.py
```

### Comparing `mypy-boto3-codebuild-1.34.74/LICENSE` & `mypy-boto3-codebuild-1.34.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/PKG-INFO` & `mypy-boto3-codebuild-1.34.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.34.74
-Summary: Type annotations for boto3.CodeBuild 1.34.74 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.81
+Summary: Type annotations for boto3.CodeBuild 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codebuild-1.34.74/README.md` & `mypy-boto3-codebuild-1.34.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/__init__.py` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/__init__.pyi` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/__main__.py` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeBuild 1.34.74\n"
-        "Version:         1.34.74\n"
+        "Type annotations for boto3.CodeBuild 1.34.81\n"
+        "Version:         1.34.81\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.74")
+    print("1.34.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/client.py` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/client.pyi` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/literals.py` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,23 @@
     "GITLAB_SELF_MANAGED",
     "NO_SOURCE",
     "S3",
 ]
 StatusTypeType = Literal["FAILED", "FAULT", "IN_PROGRESS", "STOPPED", "SUCCEEDED", "TIMED_OUT"]
 WebhookBuildTypeType = Literal["BUILD", "BUILD_BATCH"]
 WebhookFilterTypeType = Literal[
-    "ACTOR_ACCOUNT_ID", "BASE_REF", "COMMIT_MESSAGE", "EVENT", "FILE_PATH", "HEAD_REF"
+    "ACTOR_ACCOUNT_ID",
+    "BASE_REF",
+    "COMMIT_MESSAGE",
+    "EVENT",
+    "FILE_PATH",
+    "HEAD_REF",
+    "RELEASE_NAME",
+    "TAG_NAME",
+    "WORKFLOW_NAME",
 ]
 CodeBuildServiceName = Literal["codebuild"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -302,24 +310,26 @@
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
```

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/literals.pyi` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,23 @@
     "GITLAB_SELF_MANAGED",
     "NO_SOURCE",
     "S3",
 ]
 StatusTypeType = Literal["FAILED", "FAULT", "IN_PROGRESS", "STOPPED", "SUCCEEDED", "TIMED_OUT"]
 WebhookBuildTypeType = Literal["BUILD", "BUILD_BATCH"]
 WebhookFilterTypeType = Literal[
-    "ACTOR_ACCOUNT_ID", "BASE_REF", "COMMIT_MESSAGE", "EVENT", "FILE_PATH", "HEAD_REF"
+    "ACTOR_ACCOUNT_ID",
+    "BASE_REF",
+    "COMMIT_MESSAGE",
+    "EVENT",
+    "FILE_PATH",
+    "HEAD_REF",
+    "RELEASE_NAME",
+    "TAG_NAME",
+    "WORKFLOW_NAME",
 ]
 CodeBuildServiceName = Literal["codebuild"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -302,24 +310,26 @@
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
```

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/paginator.py` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/paginator.pyi` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/type_defs.py` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild/type_defs.pyi` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/PKG-INFO` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.34.74
-Summary: Type annotations for boto3.CodeBuild 1.34.74 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.81
+Summary: Type annotations for boto3.CodeBuild 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.34.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codebuild-1.34.74/mypy_boto3_codebuild.egg-info/SOURCES.txt` & `mypy-boto3-codebuild-1.34.81/mypy_boto3_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.34.74/setup.py` & `mypy-boto3-codebuild-1.34.81/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codebuild",
-    version="1.34.74",
+    version="1.34.81",
     packages=["mypy_boto3_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CodeBuild 1.34.74 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CodeBuild 1.34.81 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

