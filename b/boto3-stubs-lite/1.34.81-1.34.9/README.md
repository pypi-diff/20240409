# Comparing `tmp/boto3-stubs-lite-1.34.81.tar.gz` & `tmp/boto3-stubs-lite-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-stubs-lite-1.34.81.tar", last modified: Tue Apr  9 19:32:45 2024, max compression
+gzip compressed data, was "boto3-stubs-lite-1.34.9.tar", last modified: Wed Dec 27 20:32:17 2023, max compression
```

## Comparing `boto3-stubs-lite-1.34.81.tar` & `boto3-stubs-lite-1.34.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.444497 boto3-stubs-lite-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:32:03.000000 boto3-stubs-lite-1.34.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   141535 2024-04-09 19:32:45.444497 boto3-stubs-lite-1.34.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    71195 2024-04-09 19:32:03.000000 boto3-stubs-lite-1.34.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.344497 boto3-stubs-lite-1.34.81/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/crt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.344497 boto3-stubs-lite-1.34.81/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.344497 boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.344497 boto3-stubs-lite-1.34.81/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:03.000000 boto3-stubs-lite-1.34.81/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.344497 boto3-stubs-lite-1.34.81/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.344497 boto3-stubs-lite-1.34.81/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/s3/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 19:32:02.000000 boto3-stubs-lite-1.34.81/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:45.348497 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   141535 2024-04-09 19:32:45.000000 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-09 19:32:45.000000 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:45.000000 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:45.000000 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-09 19:32:45.000000 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 19:32:45.000000 boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:32:45.444497 boto3-stubs-lite-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    50292 2024-04-09 19:32:03.000000 boto3-stubs-lite-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-27 20:32:04.000000 boto3-stubs-lite-1.34.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    82528 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    70270 2023-12-27 20:32:04.000000 boto3-stubs-lite-1.34.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/crt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:04.000000 boto3-stubs-lite-1.34.9/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    82528 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    35996 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    49544 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/setup.py
```

### Comparing `boto3-stubs-lite-1.34.81/LICENSE` & `boto3-stubs-lite-1.34.9/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `boto3-stubs-lite-1.34.81/README.md` & `boto3-stubs-lite-1.34.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/1.34.81/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -384,15 +384,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `boto3-stubs-lite[all]` - Type annotations for all 382 services.
+- `boto3-stubs-lite[all]` - Type annotations for all 376 services.
 - `boto3-stubs-lite[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/),
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/),
   [EC2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/),
   [Lambda](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/),
   [RDS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/),
   [S3](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/) and
@@ -468,17 +468,14 @@
   service.
 - `boto3-stubs-lite[appsync]` - Type annotations for
   [AppSync](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
   service.
 - `boto3-stubs-lite[arc-zonal-shift]` - Type annotations for
   [ARCZonalShift](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
   service.
-- `boto3-stubs-lite[artifact]` - Type annotations for
-  [Artifact](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_artifact/)
-  service.
 - `boto3-stubs-lite[athena]` - Type annotations for
   [Athena](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
   service.
 - `boto3-stubs-lite[auditmanager]` - Type annotations for
   [AuditManager](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
   service.
 - `boto3-stubs-lite[autoscaling]` - Type annotations for
@@ -524,17 +521,14 @@
   service.
 - `boto3-stubs-lite[budgets]` - Type annotations for
   [Budgets](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
   service.
 - `boto3-stubs-lite[ce]` - Type annotations for
   [CostExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
   service.
-- `boto3-stubs-lite[chatbot]` - Type annotations for
-  [Chatbot](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/)
-  service.
 - `boto3-stubs-lite[chime]` - Type annotations for
   [Chime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
   service.
 - `boto3-stubs-lite[chime-sdk-identity]` - Type annotations for
   [ChimeSDKIdentity](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
   service.
 - `boto3-stubs-lite[chime-sdk-media-pipelines]` - Type annotations for
@@ -602,17 +596,14 @@
   service.
 - `boto3-stubs-lite[codecatalyst]` - Type annotations for
   [CodeCatalyst](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
   service.
 - `boto3-stubs-lite[codecommit]` - Type annotations for
   [CodeCommit](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
   service.
-- `boto3-stubs-lite[codeconnections]` - Type annotations for
-  [CodeConnections](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeconnections/)
-  service.
 - `boto3-stubs-lite[codedeploy]` - Type annotations for
   [CodeDeploy](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
   service.
 - `boto3-stubs-lite[codeguru-reviewer]` - Type annotations for
   [CodeGuruReviewer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
   service.
 - `boto3-stubs-lite[codeguru-security]` - Type annotations for
@@ -665,17 +656,14 @@
   service.
 - `boto3-stubs-lite[connectcases]` - Type annotations for
   [ConnectCases](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
   service.
 - `boto3-stubs-lite[connectparticipant]` - Type annotations for
   [ConnectParticipant](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
   service.
-- `boto3-stubs-lite[controlcatalog]` - Type annotations for
-  [ControlCatalog](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controlcatalog/)
-  service.
 - `boto3-stubs-lite[controltower]` - Type annotations for
   [ControlTower](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
   service.
 - `boto3-stubs-lite[cost-optimization-hub]` - Type annotations for
   [CostOptimizationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cost_optimization_hub/)
   service.
 - `boto3-stubs-lite[cur]` - Type annotations for
@@ -697,17 +685,14 @@
   [DataSync](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
   service.
 - `boto3-stubs-lite[datazone]` - Type annotations for
   [DataZone](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
   service.
 - `boto3-stubs-lite[dax]` - Type annotations for
   [DAX](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/) service.
-- `boto3-stubs-lite[deadline]` - Type annotations for
-  [DeadlineCloud](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_deadline/)
-  service.
 - `boto3-stubs-lite[detective]` - Type annotations for
   [Detective](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
   service.
 - `boto3-stubs-lite[devicefarm]` - Type annotations for
   [DeviceFarm](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
   service.
 - `boto3-stubs-lite[devops-guru]` - Type annotations for
@@ -889,14 +874,17 @@
   [IoT](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/) service.
 - `boto3-stubs-lite[iot-data]` - Type annotations for
   [IoTDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
   service.
 - `boto3-stubs-lite[iot-jobs-data]` - Type annotations for
   [IoTJobsDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/)
   service.
+- `boto3-stubs-lite[iot-roborunner]` - Type annotations for
+  [IoTRoboRunner](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
+  service.
 - `boto3-stubs-lite[iot1click-devices]` - Type annotations for
   [IoT1ClickDevicesService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
   service.
 - `boto3-stubs-lite[iot1click-projects]` - Type annotations for
   [IoT1ClickProjects](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
   service.
 - `boto3-stubs-lite[iotanalytics]` - Type annotations for
@@ -1416,34 +1404,28 @@
   [SFN](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
   service.
 - `boto3-stubs-lite[storagegateway]` - Type annotations for
   [StorageGateway](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
   service.
 - `boto3-stubs-lite[sts]` - Type annotations for
   [STS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/) service.
-- `boto3-stubs-lite[supplychain]` - Type annotations for
-  [SupplyChain](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/)
-  service.
 - `boto3-stubs-lite[support]` - Type annotations for
   [Support](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
   service.
 - `boto3-stubs-lite[support-app]` - Type annotations for
   [SupportApp](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support_app/)
   service.
 - `boto3-stubs-lite[swf]` - Type annotations for
   [SWF](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/) service.
 - `boto3-stubs-lite[synthetics]` - Type annotations for
   [Synthetics](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
   service.
 - `boto3-stubs-lite[textract]` - Type annotations for
   [Textract](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
   service.
-- `boto3-stubs-lite[timestream-influxdb]` - Type annotations for
-  [TimestreamInfluxDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_influxdb/)
-  service.
 - `boto3-stubs-lite[timestream-query]` - Type annotations for
   [TimestreamQuery](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
   service.
 - `boto3-stubs-lite[timestream-write]` - Type annotations for
   [TimestreamWrite](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
   service.
 - `boto3-stubs-lite[tnb]` - Type annotations for
```

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/__init__.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/crt.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/docs/utils.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/conditions.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/table.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/transform.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/dynamodb/types.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/exceptions.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/resources/action.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/resources/base.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/resources/collection.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/resources/model.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/resources/params.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/resources/response.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/s3/inject.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/s3/transfer.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/session.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3-stubs/utils.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/SOURCES.txt` & `boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.81/boto3_stubs_lite.egg-info/requires.txt` & `boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 mypy-boto3-application-insights<1.35.0,>=1.34.0
 mypy-boto3-applicationcostprofiler<1.35.0,>=1.34.0
 mypy-boto3-appmesh<1.35.0,>=1.34.0
 mypy-boto3-apprunner<1.35.0,>=1.34.0
 mypy-boto3-appstream<1.35.0,>=1.34.0
 mypy-boto3-appsync<1.35.0,>=1.34.0
 mypy-boto3-arc-zonal-shift<1.35.0,>=1.34.0
-mypy-boto3-artifact<1.35.0,>=1.34.0
 mypy-boto3-athena<1.35.0,>=1.34.0
 mypy-boto3-auditmanager<1.35.0,>=1.34.0
 mypy-boto3-autoscaling<1.35.0,>=1.34.0
 mypy-boto3-autoscaling-plans<1.35.0,>=1.34.0
 mypy-boto3-b2bi<1.35.0,>=1.34.0
 mypy-boto3-backup<1.35.0,>=1.34.0
 mypy-boto3-backup-gateway<1.35.0,>=1.34.0
@@ -60,15 +59,14 @@
 mypy-boto3-bedrock-agent<1.35.0,>=1.34.0
 mypy-boto3-bedrock-agent-runtime<1.35.0,>=1.34.0
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 mypy-boto3-braket<1.35.0,>=1.34.0
 mypy-boto3-budgets<1.35.0,>=1.34.0
 mypy-boto3-ce<1.35.0,>=1.34.0
-mypy-boto3-chatbot<1.35.0,>=1.34.0
 mypy-boto3-chime<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-identity<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-media-pipelines<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-meetings<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-messaging<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-voice<1.35.0,>=1.34.0
 mypy-boto3-cleanrooms<1.35.0,>=1.34.0
@@ -86,15 +84,14 @@
 mypy-boto3-cloudtrail<1.35.0,>=1.34.0
 mypy-boto3-cloudtrail-data<1.35.0,>=1.34.0
 mypy-boto3-cloudwatch<1.35.0,>=1.34.0
 mypy-boto3-codeartifact<1.35.0,>=1.34.0
 mypy-boto3-codebuild<1.35.0,>=1.34.0
 mypy-boto3-codecatalyst<1.35.0,>=1.34.0
 mypy-boto3-codecommit<1.35.0,>=1.34.0
-mypy-boto3-codeconnections<1.35.0,>=1.34.0
 mypy-boto3-codedeploy<1.35.0,>=1.34.0
 mypy-boto3-codeguru-reviewer<1.35.0,>=1.34.0
 mypy-boto3-codeguru-security<1.35.0,>=1.34.0
 mypy-boto3-codeguruprofiler<1.35.0,>=1.34.0
 mypy-boto3-codepipeline<1.35.0,>=1.34.0
 mypy-boto3-codestar<1.35.0,>=1.34.0
 mypy-boto3-codestar-connections<1.35.0,>=1.34.0
@@ -107,26 +104,24 @@
 mypy-boto3-compute-optimizer<1.35.0,>=1.34.0
 mypy-boto3-config<1.35.0,>=1.34.0
 mypy-boto3-connect<1.35.0,>=1.34.0
 mypy-boto3-connect-contact-lens<1.35.0,>=1.34.0
 mypy-boto3-connectcampaigns<1.35.0,>=1.34.0
 mypy-boto3-connectcases<1.35.0,>=1.34.0
 mypy-boto3-connectparticipant<1.35.0,>=1.34.0
-mypy-boto3-controlcatalog<1.35.0,>=1.34.0
 mypy-boto3-controltower<1.35.0,>=1.34.0
 mypy-boto3-cost-optimization-hub<1.35.0,>=1.34.0
 mypy-boto3-cur<1.35.0,>=1.34.0
 mypy-boto3-customer-profiles<1.35.0,>=1.34.0
 mypy-boto3-databrew<1.35.0,>=1.34.0
 mypy-boto3-dataexchange<1.35.0,>=1.34.0
 mypy-boto3-datapipeline<1.35.0,>=1.34.0
 mypy-boto3-datasync<1.35.0,>=1.34.0
 mypy-boto3-datazone<1.35.0,>=1.34.0
 mypy-boto3-dax<1.35.0,>=1.34.0
-mypy-boto3-deadline<1.35.0,>=1.34.0
 mypy-boto3-detective<1.35.0,>=1.34.0
 mypy-boto3-devicefarm<1.35.0,>=1.34.0
 mypy-boto3-devops-guru<1.35.0,>=1.34.0
 mypy-boto3-directconnect<1.35.0,>=1.34.0
 mypy-boto3-discovery<1.35.0,>=1.34.0
 mypy-boto3-dlm<1.35.0,>=1.34.0
 mypy-boto3-dms<1.35.0,>=1.34.0
@@ -187,14 +182,15 @@
 mypy-boto3-inspector<1.35.0,>=1.34.0
 mypy-boto3-inspector-scan<1.35.0,>=1.34.0
 mypy-boto3-inspector2<1.35.0,>=1.34.0
 mypy-boto3-internetmonitor<1.35.0,>=1.34.0
 mypy-boto3-iot<1.35.0,>=1.34.0
 mypy-boto3-iot-data<1.35.0,>=1.34.0
 mypy-boto3-iot-jobs-data<1.35.0,>=1.34.0
+mypy-boto3-iot-roborunner<1.35.0,>=1.34.0
 mypy-boto3-iot1click-devices<1.35.0,>=1.34.0
 mypy-boto3-iot1click-projects<1.35.0,>=1.34.0
 mypy-boto3-iotanalytics<1.35.0,>=1.34.0
 mypy-boto3-iotdeviceadvisor<1.35.0,>=1.34.0
 mypy-boto3-iotevents<1.35.0,>=1.34.0
 mypy-boto3-iotevents-data<1.35.0,>=1.34.0
 mypy-boto3-iotfleethub<1.35.0,>=1.34.0
@@ -368,21 +364,19 @@
 mypy-boto3-ssm-sap<1.35.0,>=1.34.0
 mypy-boto3-sso<1.35.0,>=1.34.0
 mypy-boto3-sso-admin<1.35.0,>=1.34.0
 mypy-boto3-sso-oidc<1.35.0,>=1.34.0
 mypy-boto3-stepfunctions<1.35.0,>=1.34.0
 mypy-boto3-storagegateway<1.35.0,>=1.34.0
 mypy-boto3-sts<1.35.0,>=1.34.0
-mypy-boto3-supplychain<1.35.0,>=1.34.0
 mypy-boto3-support<1.35.0,>=1.34.0
 mypy-boto3-support-app<1.35.0,>=1.34.0
 mypy-boto3-swf<1.35.0,>=1.34.0
 mypy-boto3-synthetics<1.35.0,>=1.34.0
 mypy-boto3-textract<1.35.0,>=1.34.0
-mypy-boto3-timestream-influxdb<1.35.0,>=1.34.0
 mypy-boto3-timestream-query<1.35.0,>=1.34.0
 mypy-boto3-timestream-write<1.35.0,>=1.34.0
 mypy-boto3-tnb<1.35.0,>=1.34.0
 mypy-boto3-transcribe<1.35.0,>=1.34.0
 mypy-boto3-transfer<1.35.0,>=1.34.0
 mypy-boto3-translate<1.35.0,>=1.34.0
 mypy-boto3-trustedadvisor<1.35.0,>=1.34.0
@@ -459,17 +453,14 @@
 
 [appsync]
 mypy-boto3-appsync<1.35.0,>=1.34.0
 
 [arc-zonal-shift]
 mypy-boto3-arc-zonal-shift<1.35.0,>=1.34.0
 
-[artifact]
-mypy-boto3-artifact<1.35.0,>=1.34.0
-
 [athena]
 mypy-boto3-athena<1.35.0,>=1.34.0
 
 [auditmanager]
 mypy-boto3-auditmanager<1.35.0,>=1.34.0
 
 [autoscaling]
@@ -508,29 +499,26 @@
 [bedrock-runtime]
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 
 [billingconductor]
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 
 [boto3]
-boto3==1.34.81
-botocore==1.34.81
+boto3==1.34.9
+botocore==1.34.9
 
 [braket]
 mypy-boto3-braket<1.35.0,>=1.34.0
 
 [budgets]
 mypy-boto3-budgets<1.35.0,>=1.34.0
 
 [ce]
 mypy-boto3-ce<1.35.0,>=1.34.0
 
-[chatbot]
-mypy-boto3-chatbot<1.35.0,>=1.34.0
-
 [chime]
 mypy-boto3-chime<1.35.0,>=1.34.0
 
 [chime-sdk-identity]
 mypy-boto3-chime-sdk-identity<1.35.0,>=1.34.0
 
 [chime-sdk-media-pipelines]
@@ -598,17 +586,14 @@
 
 [codecatalyst]
 mypy-boto3-codecatalyst<1.35.0,>=1.34.0
 
 [codecommit]
 mypy-boto3-codecommit<1.35.0,>=1.34.0
 
-[codeconnections]
-mypy-boto3-codeconnections<1.35.0,>=1.34.0
-
 [codedeploy]
 mypy-boto3-codedeploy<1.35.0,>=1.34.0
 
 [codeguru-reviewer]
 mypy-boto3-codeguru-reviewer<1.35.0,>=1.34.0
 
 [codeguru-security]
@@ -661,17 +646,14 @@
 
 [connectcases]
 mypy-boto3-connectcases<1.35.0,>=1.34.0
 
 [connectparticipant]
 mypy-boto3-connectparticipant<1.35.0,>=1.34.0
 
-[controlcatalog]
-mypy-boto3-controlcatalog<1.35.0,>=1.34.0
-
 [controltower]
 mypy-boto3-controltower<1.35.0,>=1.34.0
 
 [cost-optimization-hub]
 mypy-boto3-cost-optimization-hub<1.35.0,>=1.34.0
 
 [cur]
@@ -694,17 +676,14 @@
 
 [datazone]
 mypy-boto3-datazone<1.35.0,>=1.34.0
 
 [dax]
 mypy-boto3-dax<1.35.0,>=1.34.0
 
-[deadline]
-mypy-boto3-deadline<1.35.0,>=1.34.0
-
 [detective]
 mypy-boto3-detective<1.35.0,>=1.34.0
 
 [devicefarm]
 mypy-boto3-devicefarm<1.35.0,>=1.34.0
 
 [devops-guru]
@@ -910,14 +889,17 @@
 
 [iot-data]
 mypy-boto3-iot-data<1.35.0,>=1.34.0
 
 [iot-jobs-data]
 mypy-boto3-iot-jobs-data<1.35.0,>=1.34.0
 
+[iot-roborunner]
+mypy-boto3-iot-roborunner<1.35.0,>=1.34.0
+
 [iot1click-devices]
 mypy-boto3-iot1click-devices<1.35.0,>=1.34.0
 
 [iot1click-projects]
 mypy-boto3-iot1click-projects<1.35.0,>=1.34.0
 
 [iotanalytics]
@@ -1453,17 +1435,14 @@
 
 [storagegateway]
 mypy-boto3-storagegateway<1.35.0,>=1.34.0
 
 [sts]
 mypy-boto3-sts<1.35.0,>=1.34.0
 
-[supplychain]
-mypy-boto3-supplychain<1.35.0,>=1.34.0
-
 [support]
 mypy-boto3-support<1.35.0,>=1.34.0
 
 [support-app]
 mypy-boto3-support-app<1.35.0,>=1.34.0
 
 [swf]
@@ -1471,17 +1450,14 @@
 
 [synthetics]
 mypy-boto3-synthetics<1.35.0,>=1.34.0
 
 [textract]
 mypy-boto3-textract<1.35.0,>=1.34.0
 
-[timestream-influxdb]
-mypy-boto3-timestream-influxdb<1.35.0,>=1.34.0
-
 [timestream-query]
 mypy-boto3-timestream-query<1.35.0,>=1.34.0
 
 [timestream-write]
 mypy-boto3-timestream-write<1.35.0,>=1.34.0
 
 [tnb]
```

### Comparing `boto3-stubs-lite-1.34.81/setup.py` & `boto3-stubs-lite-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs-lite",
-    version="1.34.81",
+    version="1.34.9",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.81 generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3 1.34.9 generated with mypy-boto3-builder 7.23.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -74,15 +74,14 @@
             "mypy-boto3-application-insights>=1.34.0, <1.35.0",
             "mypy-boto3-applicationcostprofiler>=1.34.0, <1.35.0",
             "mypy-boto3-appmesh>=1.34.0, <1.35.0",
             "mypy-boto3-apprunner>=1.34.0, <1.35.0",
             "mypy-boto3-appstream>=1.34.0, <1.35.0",
             "mypy-boto3-appsync>=1.34.0, <1.35.0",
             "mypy-boto3-arc-zonal-shift>=1.34.0, <1.35.0",
-            "mypy-boto3-artifact>=1.34.0, <1.35.0",
             "mypy-boto3-athena>=1.34.0, <1.35.0",
             "mypy-boto3-auditmanager>=1.34.0, <1.35.0",
             "mypy-boto3-autoscaling>=1.34.0, <1.35.0",
             "mypy-boto3-autoscaling-plans>=1.34.0, <1.35.0",
             "mypy-boto3-b2bi>=1.34.0, <1.35.0",
             "mypy-boto3-backup>=1.34.0, <1.35.0",
             "mypy-boto3-backup-gateway>=1.34.0, <1.35.0",
@@ -93,15 +92,14 @@
             "mypy-boto3-bedrock-agent>=1.34.0, <1.35.0",
             "mypy-boto3-bedrock-agent-runtime>=1.34.0, <1.35.0",
             "mypy-boto3-bedrock-runtime>=1.34.0, <1.35.0",
             "mypy-boto3-billingconductor>=1.34.0, <1.35.0",
             "mypy-boto3-braket>=1.34.0, <1.35.0",
             "mypy-boto3-budgets>=1.34.0, <1.35.0",
             "mypy-boto3-ce>=1.34.0, <1.35.0",
-            "mypy-boto3-chatbot>=1.34.0, <1.35.0",
             "mypy-boto3-chime>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-identity>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-media-pipelines>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-meetings>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-messaging>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-voice>=1.34.0, <1.35.0",
             "mypy-boto3-cleanrooms>=1.34.0, <1.35.0",
@@ -119,15 +117,14 @@
             "mypy-boto3-cloudtrail>=1.34.0, <1.35.0",
             "mypy-boto3-cloudtrail-data>=1.34.0, <1.35.0",
             "mypy-boto3-cloudwatch>=1.34.0, <1.35.0",
             "mypy-boto3-codeartifact>=1.34.0, <1.35.0",
             "mypy-boto3-codebuild>=1.34.0, <1.35.0",
             "mypy-boto3-codecatalyst>=1.34.0, <1.35.0",
             "mypy-boto3-codecommit>=1.34.0, <1.35.0",
-            "mypy-boto3-codeconnections>=1.34.0, <1.35.0",
             "mypy-boto3-codedeploy>=1.34.0, <1.35.0",
             "mypy-boto3-codeguru-reviewer>=1.34.0, <1.35.0",
             "mypy-boto3-codeguru-security>=1.34.0, <1.35.0",
             "mypy-boto3-codeguruprofiler>=1.34.0, <1.35.0",
             "mypy-boto3-codepipeline>=1.34.0, <1.35.0",
             "mypy-boto3-codestar>=1.34.0, <1.35.0",
             "mypy-boto3-codestar-connections>=1.34.0, <1.35.0",
@@ -140,26 +137,24 @@
             "mypy-boto3-compute-optimizer>=1.34.0, <1.35.0",
             "mypy-boto3-config>=1.34.0, <1.35.0",
             "mypy-boto3-connect>=1.34.0, <1.35.0",
             "mypy-boto3-connect-contact-lens>=1.34.0, <1.35.0",
             "mypy-boto3-connectcampaigns>=1.34.0, <1.35.0",
             "mypy-boto3-connectcases>=1.34.0, <1.35.0",
             "mypy-boto3-connectparticipant>=1.34.0, <1.35.0",
-            "mypy-boto3-controlcatalog>=1.34.0, <1.35.0",
             "mypy-boto3-controltower>=1.34.0, <1.35.0",
             "mypy-boto3-cost-optimization-hub>=1.34.0, <1.35.0",
             "mypy-boto3-cur>=1.34.0, <1.35.0",
             "mypy-boto3-customer-profiles>=1.34.0, <1.35.0",
             "mypy-boto3-databrew>=1.34.0, <1.35.0",
             "mypy-boto3-dataexchange>=1.34.0, <1.35.0",
             "mypy-boto3-datapipeline>=1.34.0, <1.35.0",
             "mypy-boto3-datasync>=1.34.0, <1.35.0",
             "mypy-boto3-datazone>=1.34.0, <1.35.0",
             "mypy-boto3-dax>=1.34.0, <1.35.0",
-            "mypy-boto3-deadline>=1.34.0, <1.35.0",
             "mypy-boto3-detective>=1.34.0, <1.35.0",
             "mypy-boto3-devicefarm>=1.34.0, <1.35.0",
             "mypy-boto3-devops-guru>=1.34.0, <1.35.0",
             "mypy-boto3-directconnect>=1.34.0, <1.35.0",
             "mypy-boto3-discovery>=1.34.0, <1.35.0",
             "mypy-boto3-dlm>=1.34.0, <1.35.0",
             "mypy-boto3-dms>=1.34.0, <1.35.0",
@@ -220,14 +215,15 @@
             "mypy-boto3-inspector>=1.34.0, <1.35.0",
             "mypy-boto3-inspector-scan>=1.34.0, <1.35.0",
             "mypy-boto3-inspector2>=1.34.0, <1.35.0",
             "mypy-boto3-internetmonitor>=1.34.0, <1.35.0",
             "mypy-boto3-iot>=1.34.0, <1.35.0",
             "mypy-boto3-iot-data>=1.34.0, <1.35.0",
             "mypy-boto3-iot-jobs-data>=1.34.0, <1.35.0",
+            "mypy-boto3-iot-roborunner>=1.34.0, <1.35.0",
             "mypy-boto3-iot1click-devices>=1.34.0, <1.35.0",
             "mypy-boto3-iot1click-projects>=1.34.0, <1.35.0",
             "mypy-boto3-iotanalytics>=1.34.0, <1.35.0",
             "mypy-boto3-iotdeviceadvisor>=1.34.0, <1.35.0",
             "mypy-boto3-iotevents>=1.34.0, <1.35.0",
             "mypy-boto3-iotevents-data>=1.34.0, <1.35.0",
             "mypy-boto3-iotfleethub>=1.34.0, <1.35.0",
@@ -401,21 +397,19 @@
             "mypy-boto3-ssm-sap>=1.34.0, <1.35.0",
             "mypy-boto3-sso>=1.34.0, <1.35.0",
             "mypy-boto3-sso-admin>=1.34.0, <1.35.0",
             "mypy-boto3-sso-oidc>=1.34.0, <1.35.0",
             "mypy-boto3-stepfunctions>=1.34.0, <1.35.0",
             "mypy-boto3-storagegateway>=1.34.0, <1.35.0",
             "mypy-boto3-sts>=1.34.0, <1.35.0",
-            "mypy-boto3-supplychain>=1.34.0, <1.35.0",
             "mypy-boto3-support>=1.34.0, <1.35.0",
             "mypy-boto3-support-app>=1.34.0, <1.35.0",
             "mypy-boto3-swf>=1.34.0, <1.35.0",
             "mypy-boto3-synthetics>=1.34.0, <1.35.0",
             "mypy-boto3-textract>=1.34.0, <1.35.0",
-            "mypy-boto3-timestream-influxdb>=1.34.0, <1.35.0",
             "mypy-boto3-timestream-query>=1.34.0, <1.35.0",
             "mypy-boto3-timestream-write>=1.34.0, <1.35.0",
             "mypy-boto3-tnb>=1.34.0, <1.35.0",
             "mypy-boto3-transcribe>=1.34.0, <1.35.0",
             "mypy-boto3-transfer>=1.34.0, <1.35.0",
             "mypy-boto3-translate>=1.34.0, <1.35.0",
             "mypy-boto3-trustedadvisor>=1.34.0, <1.35.0",
@@ -441,15 +435,15 @@
             "mypy-boto3-dynamodb>=1.34.0, <1.35.0",
             "mypy-boto3-ec2>=1.34.0, <1.35.0",
             "mypy-boto3-lambda>=1.34.0, <1.35.0",
             "mypy-boto3-rds>=1.34.0, <1.35.0",
             "mypy-boto3-s3>=1.34.0, <1.35.0",
             "mypy-boto3-sqs>=1.34.0, <1.35.0",
         ],
-        "boto3": ["boto3==1.34.81", "botocore==1.34.81"],
+        "boto3": ["boto3==1.34.9", "botocore==1.34.9"],
         "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.34.0, <1.35.0"],
         "account": ["mypy-boto3-account>=1.34.0, <1.35.0"],
         "acm": ["mypy-boto3-acm>=1.34.0, <1.35.0"],
         "acm-pca": ["mypy-boto3-acm-pca>=1.34.0, <1.35.0"],
         "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.34.0, <1.35.0"],
         "amp": ["mypy-boto3-amp>=1.34.0, <1.35.0"],
         "amplify": ["mypy-boto3-amplify>=1.34.0, <1.35.0"],
@@ -467,15 +461,14 @@
         "application-insights": ["mypy-boto3-application-insights>=1.34.0, <1.35.0"],
         "applicationcostprofiler": ["mypy-boto3-applicationcostprofiler>=1.34.0, <1.35.0"],
         "appmesh": ["mypy-boto3-appmesh>=1.34.0, <1.35.0"],
         "apprunner": ["mypy-boto3-apprunner>=1.34.0, <1.35.0"],
         "appstream": ["mypy-boto3-appstream>=1.34.0, <1.35.0"],
         "appsync": ["mypy-boto3-appsync>=1.34.0, <1.35.0"],
         "arc-zonal-shift": ["mypy-boto3-arc-zonal-shift>=1.34.0, <1.35.0"],
-        "artifact": ["mypy-boto3-artifact>=1.34.0, <1.35.0"],
         "athena": ["mypy-boto3-athena>=1.34.0, <1.35.0"],
         "auditmanager": ["mypy-boto3-auditmanager>=1.34.0, <1.35.0"],
         "autoscaling": ["mypy-boto3-autoscaling>=1.34.0, <1.35.0"],
         "autoscaling-plans": ["mypy-boto3-autoscaling-plans>=1.34.0, <1.35.0"],
         "b2bi": ["mypy-boto3-b2bi>=1.34.0, <1.35.0"],
         "backup": ["mypy-boto3-backup>=1.34.0, <1.35.0"],
         "backup-gateway": ["mypy-boto3-backup-gateway>=1.34.0, <1.35.0"],
@@ -486,15 +479,14 @@
         "bedrock-agent": ["mypy-boto3-bedrock-agent>=1.34.0, <1.35.0"],
         "bedrock-agent-runtime": ["mypy-boto3-bedrock-agent-runtime>=1.34.0, <1.35.0"],
         "bedrock-runtime": ["mypy-boto3-bedrock-runtime>=1.34.0, <1.35.0"],
         "billingconductor": ["mypy-boto3-billingconductor>=1.34.0, <1.35.0"],
         "braket": ["mypy-boto3-braket>=1.34.0, <1.35.0"],
         "budgets": ["mypy-boto3-budgets>=1.34.0, <1.35.0"],
         "ce": ["mypy-boto3-ce>=1.34.0, <1.35.0"],
-        "chatbot": ["mypy-boto3-chatbot>=1.34.0, <1.35.0"],
         "chime": ["mypy-boto3-chime>=1.34.0, <1.35.0"],
         "chime-sdk-identity": ["mypy-boto3-chime-sdk-identity>=1.34.0, <1.35.0"],
         "chime-sdk-media-pipelines": ["mypy-boto3-chime-sdk-media-pipelines>=1.34.0, <1.35.0"],
         "chime-sdk-meetings": ["mypy-boto3-chime-sdk-meetings>=1.34.0, <1.35.0"],
         "chime-sdk-messaging": ["mypy-boto3-chime-sdk-messaging>=1.34.0, <1.35.0"],
         "chime-sdk-voice": ["mypy-boto3-chime-sdk-voice>=1.34.0, <1.35.0"],
         "cleanrooms": ["mypy-boto3-cleanrooms>=1.34.0, <1.35.0"],
@@ -512,15 +504,14 @@
         "cloudtrail": ["mypy-boto3-cloudtrail>=1.34.0, <1.35.0"],
         "cloudtrail-data": ["mypy-boto3-cloudtrail-data>=1.34.0, <1.35.0"],
         "cloudwatch": ["mypy-boto3-cloudwatch>=1.34.0, <1.35.0"],
         "codeartifact": ["mypy-boto3-codeartifact>=1.34.0, <1.35.0"],
         "codebuild": ["mypy-boto3-codebuild>=1.34.0, <1.35.0"],
         "codecatalyst": ["mypy-boto3-codecatalyst>=1.34.0, <1.35.0"],
         "codecommit": ["mypy-boto3-codecommit>=1.34.0, <1.35.0"],
-        "codeconnections": ["mypy-boto3-codeconnections>=1.34.0, <1.35.0"],
         "codedeploy": ["mypy-boto3-codedeploy>=1.34.0, <1.35.0"],
         "codeguru-reviewer": ["mypy-boto3-codeguru-reviewer>=1.34.0, <1.35.0"],
         "codeguru-security": ["mypy-boto3-codeguru-security>=1.34.0, <1.35.0"],
         "codeguruprofiler": ["mypy-boto3-codeguruprofiler>=1.34.0, <1.35.0"],
         "codepipeline": ["mypy-boto3-codepipeline>=1.34.0, <1.35.0"],
         "codestar": ["mypy-boto3-codestar>=1.34.0, <1.35.0"],
         "codestar-connections": ["mypy-boto3-codestar-connections>=1.34.0, <1.35.0"],
@@ -533,26 +524,24 @@
         "compute-optimizer": ["mypy-boto3-compute-optimizer>=1.34.0, <1.35.0"],
         "config": ["mypy-boto3-config>=1.34.0, <1.35.0"],
         "connect": ["mypy-boto3-connect>=1.34.0, <1.35.0"],
         "connect-contact-lens": ["mypy-boto3-connect-contact-lens>=1.34.0, <1.35.0"],
         "connectcampaigns": ["mypy-boto3-connectcampaigns>=1.34.0, <1.35.0"],
         "connectcases": ["mypy-boto3-connectcases>=1.34.0, <1.35.0"],
         "connectparticipant": ["mypy-boto3-connectparticipant>=1.34.0, <1.35.0"],
-        "controlcatalog": ["mypy-boto3-controlcatalog>=1.34.0, <1.35.0"],
         "controltower": ["mypy-boto3-controltower>=1.34.0, <1.35.0"],
         "cost-optimization-hub": ["mypy-boto3-cost-optimization-hub>=1.34.0, <1.35.0"],
         "cur": ["mypy-boto3-cur>=1.34.0, <1.35.0"],
         "customer-profiles": ["mypy-boto3-customer-profiles>=1.34.0, <1.35.0"],
         "databrew": ["mypy-boto3-databrew>=1.34.0, <1.35.0"],
         "dataexchange": ["mypy-boto3-dataexchange>=1.34.0, <1.35.0"],
         "datapipeline": ["mypy-boto3-datapipeline>=1.34.0, <1.35.0"],
         "datasync": ["mypy-boto3-datasync>=1.34.0, <1.35.0"],
         "datazone": ["mypy-boto3-datazone>=1.34.0, <1.35.0"],
         "dax": ["mypy-boto3-dax>=1.34.0, <1.35.0"],
-        "deadline": ["mypy-boto3-deadline>=1.34.0, <1.35.0"],
         "detective": ["mypy-boto3-detective>=1.34.0, <1.35.0"],
         "devicefarm": ["mypy-boto3-devicefarm>=1.34.0, <1.35.0"],
         "devops-guru": ["mypy-boto3-devops-guru>=1.34.0, <1.35.0"],
         "directconnect": ["mypy-boto3-directconnect>=1.34.0, <1.35.0"],
         "discovery": ["mypy-boto3-discovery>=1.34.0, <1.35.0"],
         "dlm": ["mypy-boto3-dlm>=1.34.0, <1.35.0"],
         "dms": ["mypy-boto3-dms>=1.34.0, <1.35.0"],
@@ -613,14 +602,15 @@
         "inspector": ["mypy-boto3-inspector>=1.34.0, <1.35.0"],
         "inspector-scan": ["mypy-boto3-inspector-scan>=1.34.0, <1.35.0"],
         "inspector2": ["mypy-boto3-inspector2>=1.34.0, <1.35.0"],
         "internetmonitor": ["mypy-boto3-internetmonitor>=1.34.0, <1.35.0"],
         "iot": ["mypy-boto3-iot>=1.34.0, <1.35.0"],
         "iot-data": ["mypy-boto3-iot-data>=1.34.0, <1.35.0"],
         "iot-jobs-data": ["mypy-boto3-iot-jobs-data>=1.34.0, <1.35.0"],
+        "iot-roborunner": ["mypy-boto3-iot-roborunner>=1.34.0, <1.35.0"],
         "iot1click-devices": ["mypy-boto3-iot1click-devices>=1.34.0, <1.35.0"],
         "iot1click-projects": ["mypy-boto3-iot1click-projects>=1.34.0, <1.35.0"],
         "iotanalytics": ["mypy-boto3-iotanalytics>=1.34.0, <1.35.0"],
         "iotdeviceadvisor": ["mypy-boto3-iotdeviceadvisor>=1.34.0, <1.35.0"],
         "iotevents": ["mypy-boto3-iotevents>=1.34.0, <1.35.0"],
         "iotevents-data": ["mypy-boto3-iotevents-data>=1.34.0, <1.35.0"],
         "iotfleethub": ["mypy-boto3-iotfleethub>=1.34.0, <1.35.0"],
@@ -810,21 +800,19 @@
         "ssm-sap": ["mypy-boto3-ssm-sap>=1.34.0, <1.35.0"],
         "sso": ["mypy-boto3-sso>=1.34.0, <1.35.0"],
         "sso-admin": ["mypy-boto3-sso-admin>=1.34.0, <1.35.0"],
         "sso-oidc": ["mypy-boto3-sso-oidc>=1.34.0, <1.35.0"],
         "stepfunctions": ["mypy-boto3-stepfunctions>=1.34.0, <1.35.0"],
         "storagegateway": ["mypy-boto3-storagegateway>=1.34.0, <1.35.0"],
         "sts": ["mypy-boto3-sts>=1.34.0, <1.35.0"],
-        "supplychain": ["mypy-boto3-supplychain>=1.34.0, <1.35.0"],
         "support": ["mypy-boto3-support>=1.34.0, <1.35.0"],
         "support-app": ["mypy-boto3-support-app>=1.34.0, <1.35.0"],
         "swf": ["mypy-boto3-swf>=1.34.0, <1.35.0"],
         "synthetics": ["mypy-boto3-synthetics>=1.34.0, <1.35.0"],
         "textract": ["mypy-boto3-textract>=1.34.0, <1.35.0"],
-        "timestream-influxdb": ["mypy-boto3-timestream-influxdb>=1.34.0, <1.35.0"],
         "timestream-query": ["mypy-boto3-timestream-query>=1.34.0, <1.35.0"],
         "timestream-write": ["mypy-boto3-timestream-write>=1.34.0, <1.35.0"],
         "tnb": ["mypy-boto3-tnb>=1.34.0, <1.35.0"],
         "transcribe": ["mypy-boto3-transcribe>=1.34.0, <1.35.0"],
         "transfer": ["mypy-boto3-transfer>=1.34.0, <1.35.0"],
         "translate": ["mypy-boto3-translate>=1.34.0, <1.35.0"],
         "trustedadvisor": ["mypy-boto3-trustedadvisor>=1.34.0, <1.35.0"],
```
