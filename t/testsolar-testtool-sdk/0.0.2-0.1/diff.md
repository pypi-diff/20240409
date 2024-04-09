# Comparing `tmp/testsolar-testtool-sdk-0.0.2.tar.gz` & `tmp/testsolar-testtool-sdk-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.0.2.tar", last modified: Mon Apr  8 12:21:58 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.1.tar", last modified: Tue Apr  9 08:36:49 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.0.2.tar` & `testsolar-testtool-sdk-0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.278031 testsolar-testtool-sdk-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.278031 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 12:21:58.000000 testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:21:58.282031 testsolar-testtool-sdk-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-08 12:21:30.000000 testsolar-testtool-sdk-0.0.2/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.147272 testsolar-testtool-sdk-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.147272 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.0.2/LICENSE` & `testsolar-testtool-sdk-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.0.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/testsolar_testtool_sdk/__init__.py
+src/testsolar_testtool_sdk/pipe_reader.py
 src/testsolar_testtool_sdk/reporter.py
 src/testsolar_testtool_sdk.egg-info/PKG-INFO
 src/testsolar_testtool_sdk.egg-info/SOURCES.txt
 src/testsolar_testtool_sdk.egg-info/dependency_links.txt
 src/testsolar_testtool_sdk.egg-info/requires.txt
 src/testsolar_testtool_sdk.egg-info/top_level.txt
 src/testsolar_testtool_sdk/model/__init__.py
```

### Comparing `testsolar-testtool-sdk-0.0.2/tests/test_report.py` & `testsolar-testtool-sdk-0.1/tests/test_report.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import concurrent.futures
 import io
+import logging
 import random
-import struct
-import time
 from datetime import datetime, timedelta
+from typing import BinaryIO
+from functools import partial
 
 from src.testsolar_testtool_sdk.model.load import LoadResult, LoadError
 from src.testsolar_testtool_sdk.model.test import TestCase
 from src.testsolar_testtool_sdk.model.testresult import ResultType, LogLevel
 from src.testsolar_testtool_sdk.model.testresult import (
     TestResult,
     TestCaseStep,
     TestCaseAssertError,
     TestCaseLog,
 )
-from src.testsolar_testtool_sdk.reporter import Reporter, MAGIC_NUMBER, ReportType
+from src.testsolar_testtool_sdk.pipe_reader import read_load_result, read_test_result
+from src.testsolar_testtool_sdk.reporter import Reporter, ReportType
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
 
 
 def _format_datetime(t: datetime) -> str:
     return t.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
 
 
 def generate_demo_load_result() -> LoadResult:
@@ -56,15 +62,15 @@
     start: datetime = datetime.utcnow() - timedelta(seconds=40)
     _tr = TestResult(
         Test=TestCase(Name=f"mumu/mu.py/test_case_name_{index}_p1", Attributes={}),
         StartTime=_format_datetime(start),
         EndTime=_format_datetime(datetime.utcnow()),
         ResultType=ResultType.SUCCEED,
         Message="ファイルが見つかりません。ファイルパスを確認して、もう一度試してください。",
-        Steps=[generate_testcase_step(f"{index}_{x}") for x in range(40)],
+        Steps=[generate_testcase_step(f"{index}_{x}") for x in range(10)],
     )
 
     return _tr
 
 
 def generate_testcase_log(index: str) -> TestCaseLog:
     start: datetime = datetime.utcnow() - timedelta(seconds=15)
@@ -88,15 +94,15 @@
 
 def generate_testcase_step(index: str) -> TestCaseStep:
     start: datetime = datetime.utcnow() - timedelta(seconds=10)
     return TestCaseStep(
         StartTime=_format_datetime(start),
         EndTime=_format_datetime(datetime.utcnow()),
         Title=get_random_unicode(100),
-        Logs=[generate_testcase_log(f"{index}_{x}") for x in range(1000)],
+        Logs=[generate_testcase_log(f"{index}_{x}") for x in range(100)],
     )
 
 
 def get_random_unicode(length) -> str:
     get_char = chr
 
     # Update this to include code point ranges to be sampled
@@ -133,55 +139,43 @@
     load_result = generate_demo_load_result()
 
     # 调用report_load_result方法
     reporter.report_load_result(load_result)
 
     # 检查管道中的魔数
     pipe_io.seek(0)
-    magic_number = struct.unpack("<I", pipe_io.read(4))[0]
-    assert magic_number == MAGIC_NUMBER, "Magic number does not match"
 
-    # 检查管道中的数据长度
-    real_load_result = load_result.model_dump_json(by_alias=True).encode("utf-8")
-    length = struct.unpack("<I", pipe_io.read(4))[0]
-    assert length == len(real_load_result), "Data length does not match"
-
-    # 检查管道中的数据
-    expected_load_result = pipe_io.read(length)
-    assert real_load_result == expected_load_result, "Data load result does not much"
+    loaded = read_load_result(pipe_io)
+    assert loaded == load_result
+
+
+def send_test_result(pipe_io: BinaryIO):
+    reporter = Reporter(reporter_type=ReportType.Pipeline, pipe_io=pipe_io)
+    test_results = []
+    run_case_result = generate_test_result(0)
+    test_results.append(run_case_result)
+    reporter.report_run_case_result(run_case_result)
 
 
 def test_report_run_case_result():
     # 创建一个Reporter实例
     pipe_io = io.BytesIO()
-    reporter = Reporter(reporter_type=ReportType.Pipeline, pipe_io=pipe_io)
 
-    test_results = []
+    send_action = partial(send_test_result, pipe_io)
 
-    # 创建五个LoadResult实例并调用report_run_case_result方法
-    for i in range(5):
-        run_case_result = generate_test_result(i)
-        test_results.append(run_case_result)
-        reporter.report_run_case_result(run_case_result)
-        time.sleep(1)
+    # 创建五个LoadResult实例并发调用report_run_case_result方法
+    with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
+        for i in range(5):
+            executor.submit(send_action)
 
     # 检查管道中的数据，确保每个用例的魔数和数据长度还有数据正确
     pipe_io.seek(0)
-    for test_result in test_results:
-        index = test_results.index(test_result)
-        magic_number = struct.unpack("<I", pipe_io.read(4))[0]
-        assert (
-            magic_number == MAGIC_NUMBER
-        ), f"Magic number does not match for case {index}"
-
-        length = struct.unpack("<I", pipe_io.read(4))[0]
-
-        expected_result_data = test_result.model_dump_json(by_alias=True).encode(
-            "utf-8"
-        )
-        expected_length = len(expected_result_data)
-        assert length == expected_length, f"Data length does not match for case {index}"
-
-        result_data = pipe_io.read(length)
-        assert (
-            result_data == expected_result_data
-        ), f"Result data does not match for case {index}"
+    r1: TestResult = read_test_result(pipe_io)
+    assert r1.result_type == ResultType.SUCCEED
+    r2 = read_test_result(pipe_io)
+    assert r2.result_type == ResultType.SUCCEED
+    r3 = read_test_result(pipe_io)
+    assert r3.result_type == ResultType.SUCCEED
+    r4 = read_test_result(pipe_io)
+    assert r4.result_type == ResultType.SUCCEED
+    r5 = read_test_result(pipe_io)
+    assert r5.result_type == ResultType.SUCCEED
```

