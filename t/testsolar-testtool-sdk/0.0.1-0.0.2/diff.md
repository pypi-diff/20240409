# Comparing `tmp/testsolar-testtool-sdk-0.0.1.tar.gz` & `tmp/testsolar-testtool-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.0.1.tar", last modified: Mon Apr  8 11:26:27 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.0.2.tar", last modified: Mon Apr  8 12:21:58 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.0.1.tar` & `testsolar-testtool-sdk-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:26:27.131436 testsolar-testtool-sdk-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 11:26:27.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 11:26:27.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:26:27.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 11:26:27.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 11:26:27.000000 testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:26:27.135436 testsolar-testtool-sdk-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-08 11:25:59.000000 testsolar-testtool-sdk-0.0.1/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.278031 testsolar-testtool-sdk-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.278031 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.0.1/LICENSE` & `testsolar-testtool-sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/reporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import os
 import struct
+import logging
 from enum import Enum
 from typing import Optional, BinaryIO
 
 import portalocker
-from loguru import logger
 from pydantic import BaseModel
 
 from .model.load import LoadResult
 from .model.testresult import TestResult
 
 # 跟TestSolar uniSDK约定的管道上报魔数，避免乱序导致后续数据全部无法上报
 MAGIC_NUMBER = 0x1234ABCD
@@ -70,22 +70,22 @@
 
         # 将 JSON 数据的长度写入管道
         self.pipe_io.write(struct.pack("<I", length))
 
         # 将 JSON 数据本身写入管道
         self.pipe_io.write(data)
 
-        logger.debug(f"Sending {length} bytes to pipe {PIPE_WRITER}")
+        logging.debug(f"Sending {length} bytes to pipe {PIPE_WRITER}")
 
         self.pipe_io.flush()
 
     def _write_load_file(self, load_result: LoadResult) -> None:
         with open(os.path.join(self.report_path, 'result.json'), "wb") as f:
-            logger.debug(f"Writing load results to {self.report_path}")
+            logging.debug(f"Writing load results to {self.report_path}")
             f.write(load_result.model_dump_json(by_alias=True, indent=2).encode('utf-8'))
 
     def _write_case_result(self, case_result: TestResult) -> None:
         retry_id = case_result.test.attrs.get('retry', '0')
         filename = hashlib.md5(f"{case_result.test.name}.{retry_id}".encode('utf-8')).hexdigest() + ".json"
         with open(os.path.join(self.report_path, filename), "wb") as f:
-            logger.debug(f"Writing case results to {self.report_path}")
+            logging.debug(f"Writing case results to {self.report_path}")
             f.write(case_result.model_dump_json(by_alias=True, indent=2).encode('utf-8'))
```

### Comparing `testsolar-testtool-sdk-0.0.1/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.0.1/tests/test_report.py` & `testsolar-testtool-sdk-0.0.2/tests/test_report.py`

 * *Files identical despite different names*

