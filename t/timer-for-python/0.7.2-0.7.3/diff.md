# Comparing `tmp/timer-for-python-0.7.2.tar.gz` & `tmp/timer-for-python-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-for-python-0.7.2.tar", last modified: Sun Dec  3 12:32:06 2023, max compression
+gzip compressed data, was "timer-for-python-0.7.3.tar", last modified: Mon Apr  8 23:37:48 2024, max compression
```

## Comparing `timer-for-python-0.7.2.tar` & `timer-for-python-0.7.3.tar`

### file list

```diff
@@ -1,60 +1,44 @@
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.560757 timer-for-python-0.7.2/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1085 2023-06-27 14:27:46.000000 timer-for-python-0.7.2/LICENSE.md
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      193 2023-12-02 06:34:23.000000 timer-for-python-0.7.2/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     6838 2023-12-03 12:32:06.560403 timer-for-python-0.7.2/PKG-INFO
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     4171 2023-12-03 12:30:50.000000 timer-for-python-0.7.2/README.md
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      108 2023-12-03 12:09:24.000000 timer-for-python-0.7.2/pyproject.toml
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1841 2023-12-03 12:32:06.562238 timer-for-python-0.7.2/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.330913 timer-for-python-0.7.2/src/
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.347315 timer-for-python-0.7.2/src/timer/
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.351416 timer-for-python-0.7.2/src/timer/.pytest_cache/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       37 2022-05-08 17:22:45.000000 timer-for-python-0.7.2/src/timer/.pytest_cache/.gitignore
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2022-05-08 17:22:45.000000 timer-for-python-0.7.2/src/timer/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      302 2022-05-08 17:22:45.000000 timer-for-python-0.7.2/src/timer/.pytest_cache/README.md
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.325519 timer-for-python-0.7.2/src/timer/.pytest_cache/v/
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.399712 timer-for-python-0.7.2/src/timer/.pytest_cache/v/cache/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:45.000000 timer-for-python-0.7.2/src/timer/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:45.000000 timer-for-python-0.7.2/src/timer/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      161 2023-03-13 10:40:21.000000 timer-for-python-0.7.2/src/timer/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.432176 timer-for-python-0.7.2/src/timer/constant/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       67 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/constant/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       53 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/constant/decimals.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/constant/various.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.444109 timer-for-python-0.7.2/src/timer/controller/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1662 2022-05-08 17:31:17.000000 timer-for-python-0.7.2/src/timer/controller/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.448189 timer-for-python-0.7.2/src/timer/decorator/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      378 2023-08-03 14:43:30.000000 timer-for-python-0.7.2/src/timer/decorator/benchmark.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.486029 timer-for-python-0.7.2/src/timer/error/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1185 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/error/__init__.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.514964 timer-for-python-0.7.2/src/timer/helper/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1568 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/helper/decimals.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1641 2022-05-08 17:31:17.000000 timer-for-python-0.7.2/src/timer/helper/output.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.517109 timer-for-python-0.7.2/src/timer/helper/thread/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      471 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/helper/thread/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1474 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/helper/thread/list.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1083 2022-05-08 17:31:17.000000 timer-for-python-0.7.2/src/timer/helper/time_fractions.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.526923 timer-for-python-0.7.2/src/timer/model/
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.541092 timer-for-python-0.7.2/src/timer/model/.pytest_cache/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       37 2022-05-08 17:22:29.000000 timer-for-python-0.7.2/src/timer/model/.pytest_cache/.gitignore
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2022-05-08 17:22:29.000000 timer-for-python-0.7.2/src/timer/model/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      302 2022-05-08 17:22:29.000000 timer-for-python-0.7.2/src/timer/model/.pytest_cache/README.md
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.330023 timer-for-python-0.7.2/src/timer/model/.pytest_cache/v/
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.543455 timer-for-python-0.7.2/src/timer/model/.pytest_cache/v/cache/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:29.000000 timer-for-python-0.7.2/src/timer/model/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:29.000000 timer-for-python-0.7.2/src/timer/model/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      145 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/model/__init__.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      282 2022-05-08 08:29:07.000000 timer-for-python-0.7.2/src/timer/model/elapsed_time_fractions.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      212 2022-05-08 08:29:07.000000 timer-for-python-0.7.2/src/timer/model/thread_item.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1298 2022-05-08 17:31:17.000000 timer-for-python-0.7.2/src/timer/model/time_fractions.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     7017 2023-12-03 06:09:45.000000 timer-for-python-0.7.2/src/timer/model/timer.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      557 2022-05-08 08:29:07.000000 timer-for-python-0.7.2/src/timer/model/timer_base.py
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2022-04-27 16:25:41.000000 timer-for-python-0.7.2/src/timer/py.typed
--rw-r--r--   0 jakobbagterp   (502) staff       (20)       80 2023-12-03 12:30:57.000000 timer-for-python-0.7.2/src/timer/version.py
-drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-12-03 12:32:06.552039 timer-for-python-0.7.2/src/timer_for_python.egg-info/
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     6838 2023-12-03 12:32:06.000000 timer-for-python-0.7.2/src/timer_for_python.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (502) staff       (20)     1349 2023-12-03 12:32:06.000000 timer-for-python-0.7.2/src/timer_for_python.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2023-12-03 12:32:06.000000 timer-for-python-0.7.2/src/timer_for_python.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2022-05-08 08:41:50.000000 timer-for-python-0.7.2/src/timer_for_python.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (502) staff       (20)      127 2023-12-03 12:32:06.000000 timer-for-python-0.7.2/src/timer_for_python.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (502) staff       (20)        6 2023-12-03 12:32:06.000000 timer-for-python-0.7.2/src/timer_for_python.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.009327 timer-for-python-0.7.3/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1085 2023-04-02 09:26:54.000000 timer-for-python-0.7.3/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      193 2023-10-19 11:12:04.000000 timer-for-python-0.7.3/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     6838 2024-04-08 23:37:48.009225 timer-for-python-0.7.3/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4171 2024-04-08 23:33:25.000000 timer-for-python-0.7.3/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      108 2024-01-04 23:11:47.000000 timer-for-python-0.7.3/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1841 2024-04-08 23:37:48.009694 timer-for-python-0.7.3/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.001254 timer-for-python-0.7.3/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.002640 timer-for-python-0.7.3/src/timer/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      161 2023-01-27 23:59:28.000000 timer-for-python-0.7.3/src/timer/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.003533 timer-for-python-0.7.3/src/timer/constant/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       67 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/constant/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       53 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/constant/decimals.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/constant/various.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.003700 timer-for-python-0.7.3/src/timer/controller/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1662 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/controller/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.003863 timer-for-python-0.7.3/src/timer/decorator/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      378 2023-01-27 23:59:28.000000 timer-for-python-0.7.3/src/timer/decorator/benchmark.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.004163 timer-for-python-0.7.3/src/timer/error/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1185 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/error/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.004767 timer-for-python-0.7.3/src/timer/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1568 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/helper/decimals.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1641 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/helper/output.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.005083 timer-for-python-0.7.3/src/timer/helper/thread/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      471 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/helper/thread/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1474 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/helper/thread/list.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1083 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/helper/time_fractions.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.006098 timer-for-python-0.7.3/src/timer/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      145 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/model/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      282 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/model/elapsed_time_fractions.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      212 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/model/thread_item.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/model/time_fractions.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     7017 2024-01-04 23:11:45.000000 timer-for-python-0.7.3/src/timer/model/timer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      557 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/model/timer_base.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:59:39.000000 timer-for-python-0.7.3/src/timer/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2024-04-08 23:33:46.000000 timer-for-python-0.7.3/src/timer/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:48.008467 timer-for-python-0.7.3/src/timer_for_python.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     6838 2024-04-08 23:37:47.000000 timer-for-python-0.7.3/src/timer_for_python.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      945 2024-04-08 23:37:47.000000 timer-for-python-0.7.3/src/timer_for_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2024-04-08 23:37:47.000000 timer-for-python-0.7.3/src/timer_for_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:26:38.000000 timer-for-python-0.7.3/src/timer_for_python.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      127 2024-04-08 23:37:47.000000 timer-for-python-0.7.3/src/timer_for_python.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        6 2024-04-08 23:37:47.000000 timer-for-python-0.7.3/src/timer_for_python.egg-info/top_level.txt
```

### Comparing `timer-for-python-0.7.2/LICENSE.md` & `timer-for-python-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/PKG-INFO` & `timer-for-python-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-for-python
-Version: 0.7.2
+Version: 0.7.3
 Summary: Timer for Python
 Home-page: https://jakob-bagterp.github.io/timer-for-python/
 Download-URL: https://pypi.org/project/timer-for-python/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
@@ -20,25 +20,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: colorist==1.7.0
+Requires-Dist: colorist==1.7.1
 Provides-Extra: testing
-Requires-Dist: coverage==7.3.2; extra == "testing"
-Requires-Dist: flake8==6.1.0; extra == "testing"
-Requires-Dist: mypy==1.7.1; extra == "testing"
-Requires-Dist: numpy==1.26.2; extra == "testing"
-Requires-Dist: pytest==7.4.3; extra == "testing"
-Requires-Dist: pytest-cov==4.1.0; extra == "testing"
-Requires-Dist: tox==4.11.3; extra == "testing"
+Requires-Dist: coverage==7.4.4; extra == "testing"
+Requires-Dist: flake8==7.0.0; extra == "testing"
+Requires-Dist: mypy==1.9.0; extra == "testing"
+Requires-Dist: numpy==1.26.4; extra == "testing"
+Requires-Dist: pytest==8.1.1; extra == "testing"
+Requires-Dist: pytest-cov==5.0.0; extra == "testing"
+Requires-Dist: tox==4.14.2; extra == "testing"
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.2&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.3&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
 [![Python 3.10 | 3.11 | 3.12+](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/timer-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/timer-for-python/branch/master/graph/badge.svg?token=P4IT8WQO0R)](https://codecov.io/gh/jakob-bagterp/timer-for-python)
 [![CodeQL](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/timer-for-python)](https://pepy.tech/project/timer-for-python)
```

### Comparing `timer-for-python-0.7.2/README.md` & `timer-for-python-0.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.2&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.3&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
 [![Python 3.10 | 3.11 | 3.12+](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/timer-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/timer-for-python/branch/master/graph/badge.svg?token=P4IT8WQO0R)](https://codecov.io/gh/jakob-bagterp/timer-for-python)
 [![CodeQL](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/timer-for-python)](https://pepy.tech/project/timer-for-python)
```

### Comparing `timer-for-python-0.7.2/setup.cfg` & `timer-for-python-0.7.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = timer-for-python
-version = 0.7.2
+version = 0.7.3
 author = Jakob Bagterp
 author_email = jakob_bagterp@hotmail.com
 maintainer = Jakob Bagterp
 maintainer_email = jakob_bagterp@hotmail.com
 description = Timer for Python
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
@@ -31,29 +31,29 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 setup_requires = 
-	colorist==1.7.0
+	colorist==1.7.1
 install_requires = 
-	colorist==1.7.0
+	colorist==1.7.1
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage==7.3.2
-	flake8==6.1.0
-	mypy==1.7.1
-	numpy==1.26.2
-	pytest==7.4.3
-	pytest-cov==4.1.0
-	tox==4.11.3
+	coverage==7.4.4
+	flake8==7.0.0
+	mypy==1.9.0
+	numpy==1.26.4
+	pytest==8.1.1
+	pytest-cov==5.0.0
+	tox==4.14.2
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `timer-for-python-0.7.2/src/timer/controller/__init__.py` & `timer-for-python-0.7.3/src/timer/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/error/__init__.py` & `timer-for-python-0.7.3/src/timer/error/__init__.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/helper/decimals.py` & `timer-for-python-0.7.3/src/timer/helper/decimals.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/helper/output.py` & `timer-for-python-0.7.3/src/timer/helper/output.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/helper/thread/list.py` & `timer-for-python-0.7.3/src/timer/helper/thread/list.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/helper/time_fractions.py` & `timer-for-python-0.7.3/src/timer/helper/time_fractions.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/model/time_fractions.py` & `timer-for-python-0.7.3/src/timer/model/time_fractions.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/model/timer.py` & `timer-for-python-0.7.3/src/timer/model/timer.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer/model/timer_base.py` & `timer-for-python-0.7.3/src/timer/model/timer_base.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.2/src/timer_for_python.egg-info/PKG-INFO` & `timer-for-python-0.7.3/src/timer_for_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-for-python
-Version: 0.7.2
+Version: 0.7.3
 Summary: Timer for Python
 Home-page: https://jakob-bagterp.github.io/timer-for-python/
 Download-URL: https://pypi.org/project/timer-for-python/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
@@ -20,25 +20,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: colorist==1.7.0
+Requires-Dist: colorist==1.7.1
 Provides-Extra: testing
-Requires-Dist: coverage==7.3.2; extra == "testing"
-Requires-Dist: flake8==6.1.0; extra == "testing"
-Requires-Dist: mypy==1.7.1; extra == "testing"
-Requires-Dist: numpy==1.26.2; extra == "testing"
-Requires-Dist: pytest==7.4.3; extra == "testing"
-Requires-Dist: pytest-cov==4.1.0; extra == "testing"
-Requires-Dist: tox==4.11.3; extra == "testing"
+Requires-Dist: coverage==7.4.4; extra == "testing"
+Requires-Dist: flake8==7.0.0; extra == "testing"
+Requires-Dist: mypy==1.9.0; extra == "testing"
+Requires-Dist: numpy==1.26.4; extra == "testing"
+Requires-Dist: pytest==8.1.1; extra == "testing"
+Requires-Dist: pytest-cov==5.0.0; extra == "testing"
+Requires-Dist: tox==4.14.2; extra == "testing"
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.2&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.3&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
 [![Python 3.10 | 3.11 | 3.12+](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/timer-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/timer-for-python/branch/master/graph/badge.svg?token=P4IT8WQO0R)](https://codecov.io/gh/jakob-bagterp/timer-for-python)
 [![CodeQL](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/timer-for-python)](https://pepy.tech/project/timer-for-python)
```

