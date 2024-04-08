# Comparing `tmp/coinpaprika_async-3.0.2.tar.gz` & `tmp/coinpaprika_async-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-3.0.2.tar", last modified: Tue Jun 20 23:41:22 2023, max compression
+gzip compressed data, was "coinpaprika_async-3.0.3.tar", last modified: Mon Apr  8 22:52:53 2024, max compression
```

## Comparing `coinpaprika_async-3.0.2.tar` & `coinpaprika_async-3.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:22.070850 coinpaprika_async-3.0.2/
--rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.2/LICENSE
--rw-rw-rw-   0        0        0     2169 2023-06-20 23:41:22.070850 coinpaprika_async-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.2/README.md
--rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      139 2023-06-20 23:41:22.072852 coinpaprika_async-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-06-20 23:40:59.000000 coinpaprika_async-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.697865 coinpaprika_async-3.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.775852 coinpaprika_async-3.0.2/src/coinpaprika_async/
--rw-rw-rw-   0        0        0      481 2023-06-20 23:37:28.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/__init__.py
--rw-rw-rw-   0        0        0      125 2023-06-20 21:46:00.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/_version__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.843851 coinpaprika_async-3.0.2/src/coinpaprika_async/api/
--rw-rw-rw-   0        0        0      245 2023-06-20 18:10:10.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/__init__.py
--rw-rw-rw-   0        0        0      235 2023-06-18 16:35:59.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coinpaprika_api.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.849850 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/__init__.py
--rw-rw-rw-   0        0        0     3882 2023-06-20 19:23:07.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/api.py
--rw-rw-rw-   0        0        0     3033 2023-06-20 18:29:31.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.859854 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:33:51.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/__init__.py
--rw-rw-rw-   0        0        0      612 2023-06-18 16:34:24.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/api.py
--rw-rw-rw-   0        0        0        0 2023-06-18 16:34:04.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/exchanges/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.869916 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:50.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/__init__.py
--rw-rw-rw-   0        0        0      828 2023-06-20 20:00:00.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/api.py
--rw-rw-rw-   0        0        0      351 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.903852 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:39.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/__init__.py
--rw-rw-rw-   0        0        0      307 2023-06-18 14:55:02.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/api.py
--rw-rw-rw-   0        0        0      408 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/market/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.914851 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/__init__.py
--rw-rw-rw-   0        0        0     3198 2023-06-20 20:00:40.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/api.py
--rw-rw-rw-   0        0        0     1457 2023-06-20 17:52:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.924852 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/
--rw-rw-rw-   0        0        0       62 2023-06-18 14:49:03.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/__init__.py
--rw-rw-rw-   0        0        0     2683 2023-06-20 17:03:43.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/http_async_client.py
--rw-rw-rw-   0        0        0      217 2023-06-20 17:03:37.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/http_models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.951878 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-06-20 20:01:10.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/api.py
--rw-rw-rw-   0        0        0      569 2023-06-20 18:13:19.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.987853 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/
--rw-rw-rw-   0        0        0       43 2023-06-18 16:37:29.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/__init__.py
--rw-rw-rw-   0        0        0      769 2023-06-20 20:05:47.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/api.py
--rw-rw-rw-   0        0        0      241 2023-06-20 20:03:04.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/models.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:22.016854 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/
--rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/__init__.py
--rw-rw-rw-   0        0        0     2482 2023-06-20 18:32:49.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/api.py
--rw-rw-rw-   0        0        0     1056 2023-06-20 17:15:14.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/models.py
--rw-rw-rw-   0        0        0     1314 2023-06-20 21:30:06.000000 coinpaprika_async-3.0.2/src/coinpaprika_async/coinpaprika_async_client.py
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:21.834850 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/
--rw-rw-rw-   0        0        0     2169 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1688 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 23:41:21.000000 coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 23:41:22.025854 coinpaprika_async-3.0.2/tests/
--rw-rw-rw-   0        0        0     1893 2023-06-20 18:16:17.000000 coinpaprika_async-3.0.2/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.458334 coinpaprika_async-3.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2191 2024-04-08 22:52:53.457336 coinpaprika_async-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.3/README.md
+-rw-rw-rw-   0        0        0      364 2024-04-08 22:09:42.000000 coinpaprika_async-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      139 2024-04-08 22:52:53.460336 coinpaprika_async-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-04-08 22:17:29.000000 coinpaprika_async-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.324319 coinpaprika_async-3.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.357296 coinpaprika_async-3.0.3/src/coinpaprika_async/
+-rw-rw-rw-   0        0        0      485 2024-04-08 22:14:45.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-08 22:06:50.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.373290 coinpaprika_async-3.0.3/src/coinpaprika_async/api/
+-rw-rw-rw-   0        0        0      245 2023-06-20 18:10:10.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-18 16:35:59.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coinpaprika_api.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.381394 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/__init__.py
+-rw-rw-rw-   0        0        0     5954 2023-06-21 22:20:04.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/api.py
+-rw-rw-rw-   0        0        0     3033 2023-06-20 18:29:31.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.392600 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:33:51.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/__init__.py
+-rw-rw-rw-   0        0        0      897 2024-04-08 22:40:55.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/api.py
+-rw-rw-rw-   0        0        0     1322 2024-04-08 22:41:52.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/exchanges/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.400392 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:50.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/__init__.py
+-rw-rw-rw-   0        0        0      828 2023-06-20 20:00:00.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/api.py
+-rw-rw-rw-   0        0        0      351 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.406419 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:39.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/__init__.py
+-rw-rw-rw-   0        0        0      307 2023-06-18 14:55:02.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/api.py
+-rw-rw-rw-   0        0        0      408 2023-06-20 16:48:12.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/market/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.414399 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/__init__.py
+-rw-rw-rw-   0        0        0     3200 2024-04-08 22:06:10.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/api.py
+-rw-rw-rw-   0        0        0     1457 2023-06-20 17:52:21.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.430347 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/
+-rw-rw-rw-   0        0        0       62 2023-06-18 14:49:03.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/__init__.py
+-rw-rw-rw-   0        0        0     2683 2023-06-20 17:03:43.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/http_async_client.py
+-rw-rw-rw-   0        0        0      217 2023-06-20 17:03:37.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/http_models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.435332 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:28:26.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-06-20 20:01:10.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/api.py
+-rw-rw-rw-   0        0        0      569 2023-06-20 18:13:19.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.442332 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/
+-rw-rw-rw-   0        0        0       43 2023-06-18 16:37:29.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-06-20 20:05:47.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/api.py
+-rw-rw-rw-   0        0        0      241 2023-06-20 20:03:04.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/models.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.448347 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/
+-rw-rw-rw-   0        0        0       43 2023-06-17 19:19:52.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/__init__.py
+-rw-rw-rw-   0        0        0     2482 2023-06-20 18:32:49.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/api.py
+-rw-rw-rw-   0        0        0     1056 2023-06-20 17:15:14.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/models.py
+-rw-rw-rw-   0        0        0     1478 2024-04-08 22:10:59.000000 coinpaprika_async-3.0.3/src/coinpaprika_async/coinpaprika_async_client.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.455334 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/
+-rw-rw-rw-   0        0        0     2191 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1693 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-08 22:52:53.000000 coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 22:52:53.450332 coinpaprika_async-3.0.3/src/tests/
+-rw-rw-rw-   0        0        0     2289 2024-04-08 22:37:24.000000 coinpaprika_async-3.0.3/src/tests/test_client.py
```

### Comparing `coinpaprika_async-3.0.2/LICENSE` & `coinpaprika_async-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/PKG-INFO` & `coinpaprika_async-3.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: coinpaprika_async
-Version: 3.0.2
+Version: 3.0.3
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
-Keywords: coinpaprika_async api cryptocurrency async httpx client
+Keywords: coinpaprika_async,api,cryptocurrency,async,httpx,client
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
 
 <div align="center">
 <h1 style="font-size:50px;">Coinpaprika Async Client</h1>
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
```

### Comparing `coinpaprika_async-3.0.2/README.md` & `coinpaprika_async-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/setup.py` & `coinpaprika_async-3.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from setuptools import setup
 
 setup(
     name="coinpaprika_async",
-    version="3.0.2",
+    version="3.0.3",
     author="DroidZed",
     author_email="droid.zed77@outlook.com",
     description="An asynchronous client for the coinpaprika API.",
     url="https://github.com/DroidZed/coinpaprika-async-client.git",
     license="MIT",
     install_requires=["httpx"],
-    keywords="coinpaprika_async api cryptocurrency async httpx client",
+    keywords=[
+        "coinpaprika_async",
+        "api",
+        "cryptocurrency",
+        "async",
+        "httpx",
+        "client",
+    ],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/coins/models.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/coins/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/key/api.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/key/api.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/api.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Any, Dict, List
 from ..coinpaprika_api import CoinpaprikaAPI
 from .models import *
 
 
-class MiscelanousEndpoints(CoinpaprikaAPI):
+class MiscellaneousEndpoints(CoinpaprikaAPI):
     async def people(self, person_id: str):
         res = await self.internal.call_api(f"people/{person_id}")
 
         if res.Error:
             return res.Error
 
         data: List[Dict[str, Any]] = res.Data
```

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/misc/models.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/misc/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/networking_layer/http_async_client.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/networking_layer/http_async_client.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/api.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/api.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/people/models.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/people/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/tags/api.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/tags/api.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/api.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/api.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/api/tickers/models.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/api/tickers/models.py`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async/coinpaprika_async_client.py` & `coinpaprika_async-3.0.3/src/coinpaprika_async/coinpaprika_async_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-from typing import Optional
+from typing import Optional, Any
 
 from .api.networking_layer import HttpAsyncClient
 
 
 class CoinPaprikaAsyncClient:
-
     """
     ### An async client for interacting with Coinpaprika's API backend.
 
     """
 
     __FREE_API_URL = "https://api.coinpaprika.com/v1"
 
     __PRO_API_URL = "https://api-pro.coinpaprika.com/v1"
 
-    def __init__(self, http: HttpAsyncClient = HttpAsyncClient(), api_key: Optional[str] = None):
+    def __init__(
+        self,
+        http: HttpAsyncClient = HttpAsyncClient(),
+        api_key: Optional[str] = None,
+    ):
         self._http_client = http
         self._is_paid = api_key != None
         self._api_key = api_key
 
     async def call_api(self, path: str, **query_params):
         uri = self.__create_api_uri(path)
         headers = self.__create_headers()
 
-        return await self._http_client.get(uri, headers=headers, url_params=query_params, timeout=20)
+        return await self._http_client.get(
+            uri, headers=headers, url_params=query_params, timeout=20
+        )
 
     def __create_api_uri(self, path: str):
-        return f"{self.__FREE_API_URL}/{path}" if not self._is_paid else f"{self.__PRO_API_URL}/{path}"
+        return (
+            f"{self.__FREE_API_URL}/{path}"
+            if not self._is_paid
+            else f"{self.__PRO_API_URL}/{path}"
+        )
 
     def __create_headers(self):
         if self._is_paid:
             return {
                 "Accept": "application/json",
                 "User-Agent": "coinpaprika_async-async/python",
                 "Authorization": self._api_key,
             }
         else:
-            return {"Accept": "application/json", "User-Agent": "coinpaprika_async-async/python"}
+            return {
+                "Accept": "application/json",
+                "User-Agent": "coinpaprika_async-async/python",
+            }
```

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/PKG-INFO` & `coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: coinpaprika-async
-Version: 3.0.2
+Name: coinpaprika_async
+Version: 3.0.3
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
-Keywords: coinpaprika_async api cryptocurrency async httpx client
+Keywords: coinpaprika_async,api,cryptocurrency,async,httpx,client
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
 
 <div align="center">
 <h1 style="font-size:50px;">Coinpaprika Async Client</h1>
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
```

### Comparing `coinpaprika_async-3.0.2/src/coinpaprika_async.egg-info/SOURCES.txt` & `coinpaprika_async-3.0.3/src/coinpaprika_async.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/coinpaprika_async/__init__.py
-src/coinpaprika_async/_version__.py
+src/coinpaprika_async/__version__.py
 src/coinpaprika_async/coinpaprika_async_client.py
 src/coinpaprika_async.egg-info/PKG-INFO
 src/coinpaprika_async.egg-info/SOURCES.txt
 src/coinpaprika_async.egg-info/dependency_links.txt
 src/coinpaprika_async.egg-info/requires.txt
 src/coinpaprika_async.egg-info/top_level.txt
 src/coinpaprika_async/api/__init__.py
@@ -36,8 +36,8 @@
 src/coinpaprika_async/api/people/models.py
 src/coinpaprika_async/api/tags/__init__.py
 src/coinpaprika_async/api/tags/api.py
 src/coinpaprika_async/api/tags/models.py
 src/coinpaprika_async/api/tickers/__init__.py
 src/coinpaprika_async/api/tickers/api.py
 src/coinpaprika_async/api/tickers/models.py
-tests/test_client.py
+src/tests/test_client.py
```

### Comparing `coinpaprika_async-3.0.2/tests/test_client.py` & `coinpaprika_async-3.0.3/src/tests/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,84 @@
 import pytest
 from pytest_httpx import HTTPXMock
 
-from coinpaprika_async import MiscelanousEndpoints, CoinsEndpoint, ApiError
+from src.coinpaprika_async import (
+    CoinsEndpoint,
+    ExchangesEndpoint,
+    MiscellaneousEndpoints,
+    ApiError,
+)
 
 
 class TestClient:
     @pytest.mark.asyncio
     async def test_mock_async_price_conv(self, httpx_mock: HTTPXMock):
-        params = {"base_currency_id": "btc-bitcoin", "quote_currency_id": "usd-us-dollars", "amount": 1337}
+        params = {
+            "base_currency_id": "btc-bitcoin",
+            "quote_currency_id": "usd-us-dollars",
+            "amount": 1337,
+        }
 
         json = {
             "base_currency_id": "btc-bitcoin",
             "base_currency_name": "Bitcoin",
             "base_price_last_updated": "2022-01-16T23:46:14Z",
             "quote_currency_id": "xmr-monero",
             "quote_currency_name": "Monero",
             "quote_price_last_updated": "2022-01-16T23:46:14Z",
             "amount": 12.2,
             "price": 2336.6037613108747,
         }
 
-        api = MiscelanousEndpoints()
+        api = MiscellaneousEndpoints()
 
         httpx_mock.add_response(json=json)
 
         response = await api.price_converter(**params)
 
         assert not isinstance(response, ApiError)
 
     @pytest.mark.asyncio
     async def test_should_give_proper_coins(self):
         coins_api = CoinsEndpoint()
 
-        resp = await coins_api.coins()
+        resp = await coins_api.get_all()
 
         if isinstance(resp, ApiError):
             assert False
 
         assert len(resp) != 0
 
     @pytest.mark.asyncio
     async def test_failed_api_call(self, httpx_mock: HTTPXMock):
         json_obj = {"error": "id not found"}
 
         coins_api = CoinsEndpoint()
 
         httpx_mock.add_response(json=json_obj, status_code=404)
 
-        response = await coins_api.coin("eth")
+        response = await coins_api.coin_by_id("eth")
 
         if response.Error:
             assert response.Error.error == json_obj["error"]
 
     @pytest.mark.asyncio
     async def test_for_markets(self):
         coins_api = CoinsEndpoint()
 
-        response = await coins_api.markets("btc-bitcoin")
+        response = await coins_api.markets_of_coin("btc-bitcoin")
+
+        if isinstance(response, ApiError):
+            assert False
+
+        assert len(response)
+
+    @pytest.mark.asyncio
+    async def test_for_exchanges(self):
+        exchanges_api = ExchangesEndpoint()
+
+        response = await exchanges_api.exchange_list()
 
         if isinstance(response, ApiError):
             assert False
 
         assert len(response)
```

