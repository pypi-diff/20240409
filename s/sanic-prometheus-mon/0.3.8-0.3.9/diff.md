# Comparing `tmp/sanic-prometheus-mon-0.3.8.tar.gz` & `tmp/sanic-prometheus-mon-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sanic-prometheus-mon-0.3.8.tar", last modified: Fri Sep  2 12:07:46 2022, max compression
+gzip compressed data, was "sanic-prometheus-mon-0.3.9.tar", last modified: Tue Apr  9 12:23:38 2024, max compression
```

## Comparing `sanic-prometheus-mon-0.3.8.tar` & `sanic-prometheus-mon-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 velisay  (775908382) SBERNED\Пользователи (116889197)        0 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)      915 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/PKG-INFO
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)     5207 2022-02-20 09:18:24.000000 sanic-prometheus-mon-0.3.8/README.rst
-drwxr-xr-x   0 velisay  (775908382) SBERNED\Пользователи (116889197)        0 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus/
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)     5778 2021-09-22 14:04:56.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus/__init__.py
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)     1003 2021-09-22 14:04:56.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus/endpoint.py
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)       51 2021-09-22 14:04:56.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus/exceptions.py
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)     2899 2022-09-02 12:07:24.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus/metrics.py
-drwxr-xr-x   0 velisay  (775908382) SBERNED\Пользователи (116889197)        0 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)      915 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/PKG-INFO
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)      408 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/SOURCES.txt
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)        1 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/dependency_links.txt
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)        1 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/not-zip-safe
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)       53 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/requires.txt
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)       17 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/top_level.txt
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)       62 2022-09-02 12:07:46.000000 sanic-prometheus-mon-0.3.8/setup.cfg
--rw-r--r--   0 velisay  (775908382) SBERNED\Пользователи (116889197)     1164 2022-09-02 12:07:24.000000 sanic-prometheus-mon-0.3.8/setup.py
+drwxr-xr-x   0 hairspray   (501) staff       (20)        0 2024-04-09 12:23:38.719780 sanic-prometheus-mon-0.3.9/
+-rw-r--r--   0 hairspray   (501) staff       (20)     1070 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/LICENSE
+-rw-r--r--   0 hairspray   (501) staff       (20)      916 2024-04-09 12:23:38.719858 sanic-prometheus-mon-0.3.9/PKG-INFO
+-rw-r--r--   0 hairspray   (501) staff       (20)     5207 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/README.rst
+drwxr-xr-x   0 hairspray   (501) staff       (20)        0 2024-04-09 12:23:38.718395 sanic-prometheus-mon-0.3.9/sanic_prometheus/
+-rw-r--r--   0 hairspray   (501) staff       (20)     5778 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus/__init__.py
+-rw-r--r--   0 hairspray   (501) staff       (20)     1003 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus/endpoint.py
+-rw-r--r--   0 hairspray   (501) staff       (20)       51 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus/exceptions.py
+-rw-r--r--   0 hairspray   (501) staff       (20)     3203 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus/metrics.py
+drwxr-xr-x   0 hairspray   (501) staff       (20)        0 2024-04-09 12:23:38.719308 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/
+-rw-r--r--   0 hairspray   (501) staff       (20)      916 2024-04-09 12:23:38.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/PKG-INFO
+-rw-r--r--   0 hairspray   (501) staff       (20)      461 2024-04-09 12:23:38.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/SOURCES.txt
+-rw-r--r--   0 hairspray   (501) staff       (20)        1 2024-04-09 12:23:38.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/dependency_links.txt
+-rw-r--r--   0 hairspray   (501) staff       (20)        1 2024-04-09 12:23:38.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/not-zip-safe
+-rw-r--r--   0 hairspray   (501) staff       (20)       53 2024-04-09 12:23:38.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/requires.txt
+-rw-r--r--   0 hairspray   (501) staff       (20)       17 2024-04-09 12:23:38.000000 sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/top_level.txt
+-rw-r--r--   0 hairspray   (501) staff       (20)       62 2024-04-09 12:23:38.720237 sanic-prometheus-mon-0.3.9/setup.cfg
+-rw-r--r--   0 hairspray   (501) staff       (20)     1164 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/setup.py
+drwxr-xr-x   0 hairspray   (501) staff       (20)        0 2024-04-09 12:23:38.719614 sanic-prometheus-mon-0.3.9/tests/
+-rw-r--r--   0 hairspray   (501) staff       (20)     1714 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/tests/test_endpoint.py
+-rw-r--r--   0 hairspray   (501) staff       (20)      531 2024-04-09 12:22:58.000000 sanic-prometheus-mon-0.3.9/tests/test_metrics.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sanic-prometheus-mon-0.3.8/PKG-INFO` & `sanic-prometheus-mon-0.3.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sanic-prometheus-mon
-Version: 0.3.8
+Version: 0.3.9
 Summary: Exposes Prometheus monitoring metrics of Sanic apps.
 Home-page: https://github.com/valerylisay/sanic-prometheus-mon
 Author: Dan Kruchinin
 Author-email: dan.kruchinin@gmail.com
 Maintainer: Valeriy Lisay
 Maintainer-email: valery@lisay.ru
 License: MIT
-Description: UNKNOWN
 Keywords: python sanic prometheus monitoring metrics
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
```

### Comparing `sanic-prometheus-mon-0.3.8/README.rst` & `sanic-prometheus-mon-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `sanic-prometheus-mon-0.3.8/sanic_prometheus/__init__.py` & `sanic-prometheus-mon-0.3.9/sanic_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `sanic-prometheus-mon-0.3.8/sanic_prometheus/endpoint.py` & `sanic-prometheus-mon-0.3.9/sanic_prometheus/endpoint.py`

 * *Files identical despite different names*

### Comparing `sanic-prometheus-mon-0.3.8/sanic_prometheus/metrics.py` & `sanic-prometheus-mon-0.3.9/sanic_prometheus/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import http
 import time
 import typing as tp
 
 import psutil
 from prometheus_client import Counter, Histogram, Gauge
 
 
@@ -50,20 +51,35 @@
         app.metrics['PROC_RSS_MEM_PERC'].set(p.memory_percent())
 
 
 def before_request_handler(request):
     _set_start_time_compat(request, time.perf_counter())
 
 
+def _convert_status_to_int(
+        response_status: tp.Union[int, str, http.HTTPStatus]
+) -> int:
+    """
+    Converts http.HTTPStatus, str, int to int value.
+
+    If error returns 0.
+    """
+    try:
+        response_status = int(response_status)
+    except (TypeError, ValueError):
+        response_status = 0
+
+    return response_status
+
+
 def after_request_handler(request, response, get_endpoint_fn):
     # Note, that some handlers can ignore response logic,
     # for example, websocket handler
     response_status = response.status if response else 200
-    if not isinstance(response_status, int):
-        response_status = int(response_status)  # HTTPStatus -> int
+    response_status = _convert_status_to_int(response_status)
 
     endpoint = get_endpoint_fn(request)
 
     req_start_time = _get_start_time_compat(request)
     if req_start_time:
         latency = time.perf_counter() - req_start_time
```

### Comparing `sanic-prometheus-mon-0.3.8/sanic_prometheus_mon.egg-info/PKG-INFO` & `sanic-prometheus-mon-0.3.9/sanic_prometheus_mon.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sanic-prometheus-mon
-Version: 0.3.8
+Version: 0.3.9
 Summary: Exposes Prometheus monitoring metrics of Sanic apps.
 Home-page: https://github.com/valerylisay/sanic-prometheus-mon
 Author: Dan Kruchinin
 Author-email: dan.kruchinin@gmail.com
 Maintainer: Valeriy Lisay
 Maintainer-email: valery@lisay.ru
 License: MIT
-Description: UNKNOWN
 Keywords: python sanic prometheus monitoring metrics
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
```

### Comparing `sanic-prometheus-mon-0.3.8/setup.py` & `sanic-prometheus-mon-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='sanic-prometheus-mon',
-    version='0.3.8',
+    version='0.3.9',
     description='Exposes Prometheus monitoring metrics of Sanic apps.',
     url='https://github.com/valerylisay/sanic-prometheus-mon',
     author='Dan Kruchinin',
     author_email='dan.kruchinin@gmail.com',
     maintainer='Valeriy Lisay',
     maintainer_email='valery@lisay.ru',
     license='MIT',
```

