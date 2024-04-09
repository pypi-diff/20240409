# Comparing `tmp/coinbase-advanced-py-1.2.1.tar.gz` & `tmp/coinbase-advanced-py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinbase-advanced-py-1.2.1.tar", last modified: Wed Mar 27 20:37:13 2024, max compression
+gzip compressed data, was "coinbase-advanced-py-1.2.2.tar", last modified: Tue Apr  9 20:55:52 2024, max compression
```

## Comparing `coinbase-advanced-py-1.2.1.tar` & `coinbase-advanced-py-1.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.318734 coinbase-advanced-py-1.2.1/
--rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.2.1/LICENSE.md
--rw-r--r--   0 urischwartz   (501) staff       (20)    15261 2024-03-27 20:37:13.318201 coinbase-advanced-py-1.2.1/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)    14147 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/README.md
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.303297 coinbase-advanced-py-1.2.1/coinbase/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.2.1/coinbase/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.1/coinbase/__version__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1986 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/coinbase/api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      746 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/coinbase/constants.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2411 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.308556 coinbase-advanced-py-1.2.1/coinbase/rest/
--rwxr-xr-x   0 urischwartz   (501) staff       (20)     2490 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.1/coinbase/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1331 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      641 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.1/coinbase/rest/common.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2974 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      927 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4033 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1684 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    59432 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.1/coinbase/rest/orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1280 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.1/coinbase/rest/payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2866 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4125 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3223 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/rest/products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6913 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.1/coinbase/rest/rest_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.309728 coinbase-advanced-py-1.2.1/coinbase/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/coinbase/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    15436 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.1/coinbase/websocket/channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    19199 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.1/coinbase/websocket/websocket_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.310780 coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/
--rw-r--r--   0 urischwartz   (501) staff       (20)    15261 2024-03-27 20:37:13.000000 coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-03-27 20:37:13.000000 coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/SOURCES.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-03-27 20:37:13.000000 coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/dependency_links.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-03-27 20:37:13.000000 coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/requires.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-03-27 20:37:13.000000 coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/top_level.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-03-27 20:37:13.318832 coinbase-advanced-py-1.2.1/setup.cfg
--rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.2.1/setup.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.311276 coinbase-advanced-py-1.2.1/tests/
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.315563 coinbase-advanced-py-1.2.1/tests/rest/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.2.1/tests/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1389 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/rest/test_accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      872 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.1/tests/rest/test_common.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/rest/test_convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/rest/test_fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3965 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/rest/test_futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/rest/test_market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    54821 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.1/tests/rest/test_orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.1/tests/rest/test_payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3268 2024-02-01 19:31:57.000000 coinbase-advanced-py-1.2.1/tests/rest/test_perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.2.1/tests/rest/test_portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/rest/test_products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6970 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.1/tests/rest/test_rest_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1936 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/test_api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1963 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/test_jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-03-27 20:37:13.316935 coinbase-advanced-py-1.2.1/tests/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/websocket/mock_ws_server.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/websocket/test_channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    13978 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.1/tests/websocket/test_websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.045608 coinbase-advanced-py-1.2.2/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.2.2/LICENSE.md
+-rw-r--r--   0 urischwartz   (501) staff       (20)    15261 2024-04-09 20:55:52.045219 coinbase-advanced-py-1.2.2/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)    14147 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/README.md
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.027150 coinbase-advanced-py-1.2.2/coinbase/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.2.2/coinbase/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/__version__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1986 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/coinbase/api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      746 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/coinbase/constants.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2350 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.032262 coinbase-advanced-py-1.2.2/coinbase/rest/
+-rwxr-xr-x   0 urischwartz   (501) staff       (20)     2514 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1331 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      641 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/coinbase/rest/common.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2974 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      927 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4806 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/rest/futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1684 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    59432 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/coinbase/rest/orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1280 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/coinbase/rest/payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2866 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4125 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     3223 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     6913 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/coinbase/rest/rest_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.033390 coinbase-advanced-py-1.2.2/coinbase/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/coinbase/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    15436 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/websocket/channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    19199 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/coinbase/websocket/websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.035090 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    15261 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/SOURCES.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/dependency_links.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/requires.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/top_level.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-04-09 20:55:52.045689 coinbase-advanced-py-1.2.2/setup.cfg
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.2.2/setup.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.035706 coinbase-advanced-py-1.2.2/tests/
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.042138 coinbase-advanced-py-1.2.2/tests/rest/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.2.2/tests/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1389 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      872 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/tests/rest/test_common.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5011 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/tests/rest/test_futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    54821 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/tests/rest/test_orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/tests/rest/test_payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     3268 2024-02-01 19:31:57.000000 coinbase-advanced-py-1.2.2/tests/rest/test_perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.2.2/tests/rest/test_portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     6970 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/tests/rest/test_rest_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1936 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/test_api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1749 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/tests/test_jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.043764 coinbase-advanced-py-1.2.2/tests/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/mock_ws_server.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/test_channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    13978 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/test_websocket_base.py
```

### Comparing `coinbase-advanced-py-1.2.1/LICENSE.md` & `coinbase-advanced-py-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/PKG-INFO` & `coinbase-advanced-py-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `coinbase-advanced-py-1.2.1/README.md` & `coinbase-advanced-py-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/api_base.py` & `coinbase-advanced-py-1.2.2/coinbase/api_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/constants.py` & `coinbase-advanced-py-1.2.2/coinbase/constants.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/jwt_generator.py` & `coinbase-advanced-py-1.2.2/coinbase/jwt_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import jwt
 from cryptography.hazmat.primitives import serialization
 
 from coinbase.constants import BASE_URL, REST_SERVICE, WS_SERVICE
 
 
-def build_jwt(key_var, secret_var, service, uri=None) -> str:
+def build_jwt(key_var, secret_var, uri=None) -> str:
     """
     :meta private:
     """
     try:
         private_key_bytes = secret_var.encode("utf-8")
         private_key = serialization.load_pem_private_key(
             private_key_bytes, password=None
@@ -24,15 +24,14 @@
         )
 
     jwt_data = {
         "sub": key_var,
         "iss": "coinbase-cloud",
         "nbf": int(time.time()),
         "exp": int(time.time()) + 120,
-        "aud": [service],
     }
 
     if uri:
         jwt_data["uri"] = uri
 
     jwt_token = jwt.encode(
         jwt_data,
@@ -57,15 +56,15 @@
 
     Parameters:
 
     - **uri (str)** - Formatted URI for the endpoint (e.g. "GET api.coinbase.com/api/v3/brokerage/accounts") Can be generated using ``format_jwt_uri``
     - **key_var (str)** - The API key
     - **secret_var (str)** - The API key secret
     """
-    return build_jwt(key_var, secret_var, REST_SERVICE, uri=uri)
+    return build_jwt(key_var, secret_var, uri=uri)
 
 
 def build_ws_jwt(key_var, secret_var) -> str:
     """
     **Build WebSocket JWT**
     __________
 
@@ -76,15 +75,15 @@
     __________
 
     Parameters:
 
     - **key_var (str)** - The API key
     - **secret_var (str)** - The API key secret
     """
-    return build_jwt(key_var, secret_var, WS_SERVICE)
+    return build_jwt(key_var, secret_var)
 
 
 def format_jwt_uri(method, path) -> str:
     """
     **Format JWT URI**
     __________
```

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/__init__.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class RESTClient(RESTBase):
     from .accounts import get_account, get_accounts
     from .common import get_unix_time
     from .convert import commit_convert_trade, create_convert_quote, get_convert_trade
     from .fees import get_transaction_summary
     from .futures import (
         cancel_pending_futures_sweep,
+        close_position,
         get_futures_balance_summary,
         get_futures_position,
         list_futures_positions,
         list_futures_sweeps,
         schedule_futures_sweep,
     )
     from .market_data import get_candles, get_market_trades
```

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/accounts.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/accounts.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/common.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/common.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/convert.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/fees.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/fees.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/futures.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/futures.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,38 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from coinbase.constants import API_PREFIX
 
 
+def close_position(
+    self, client_order_id: str, product_id: str, size: Optional[str] = None, **kwargs
+) -> Dict[str, Any]:
+    """
+    **Close Position**
+    _________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/close_position
+
+    __________
+
+    **Description:**
+
+    Places an order to close any open positions for a specified ``product_id``.
+
+    __________
+
+    **Read more on the official documentation:** `Close Position
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_closeposition>`_
+    """
+    endpoint = f"{API_PREFIX}/orders/close_position"
+    data = {"client_order_id": client_order_id, "product_id": product_id, "size": size}
+
+    return self.post(endpoint, data=data, **kwargs)
+
+
 def get_futures_balance_summary(self, **kwargs) -> Dict[str, Any]:
     """
     **Get Futures Balance Summary**
     _______________________________
 
     [GET] https://api.coinbase.com/api/v3/brokerage/cfm/balance_summary
```

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/market_data.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/market_data.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/orders.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/orders.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/payments.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/perpetuals.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/perpetuals.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/portfolios.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/portfolios.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/products.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/rest/rest_base.py` & `coinbase-advanced-py-1.2.2/coinbase/rest/rest_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/websocket/__init__.py` & `coinbase-advanced-py-1.2.2/coinbase/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/websocket/channels.py` & `coinbase-advanced-py-1.2.2/coinbase/websocket/channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase/websocket/websocket_base.py` & `coinbase-advanced-py-1.2.2/coinbase/websocket/websocket_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/PKG-INFO` & `coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `coinbase-advanced-py-1.2.1/coinbase_advanced_py.egg-info/SOURCES.txt` & `coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/setup.py` & `coinbase-advanced-py-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_accounts.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_accounts.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_common.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_common.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_convert.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_fees.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_fees.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_futures.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_futures.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,46 @@
 
 from coinbase.rest import RESTClient
 
 from ..constants import TEST_API_KEY, TEST_API_SECRET
 
 
 class FuturesTest(unittest.TestCase):
+    def test_close_position(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {
+            "client_order_id": "client_order_id_1",
+            "product_id": "product_id_1",
+        }
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/close_position",
+                json=expected_response,
+            )
+            closedOrder = client.close_position(
+                "client_order_id_1", "product_id_1", "100"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "size": "100",
+                },
+            )
+            self.assertEqual(closedOrder, expected_response)
+
     def test_get_futures_balance_summary(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
```

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_market_data.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_market_data.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_orders.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_orders.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_payments.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_perpetuals.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_perpetuals.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_portfolios.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_products.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/rest/test_rest_base.py` & `coinbase-advanced-py-1.2.2/tests/rest/test_rest_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/test_api_base.py` & `coinbase-advanced-py-1.2.2/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/test_jwt_generator.py` & `coinbase-advanced-py-1.2.2/tests/test_jwt_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,32 @@
 
 
 class JwtGeneratorTest(unittest.TestCase):
     def test_build_rest_jwt(self):
         uri = jwt_generator.format_jwt_uri("GET", "/api/v3/brokerage/accounts")
         result_jwt = jwt_generator.build_rest_jwt(uri, TEST_API_KEY, TEST_API_SECRET)
 
-        decoded_data = jwt.decode(
-            result_jwt, TEST_API_SECRET, algorithms=["ES256"], audience=[REST_SERVICE]
-        )
+        decoded_data = jwt.decode(result_jwt, TEST_API_SECRET, algorithms=["ES256"])
         header_bytes = base64.urlsafe_b64decode(str(result_jwt.split(".")[0] + "=="))
         decoded_header = json.loads(header_bytes.decode("utf-8"))
 
         self.assertEqual(decoded_data["sub"], TEST_API_KEY)
         self.assertEqual(decoded_data["iss"], "coinbase-cloud")
-        self.assertEqual(decoded_data["aud"], [REST_SERVICE])
         self.assertEqual(decoded_data["uri"], uri)
         self.assertEqual(decoded_header["kid"], TEST_API_KEY)
 
     def test_build_ws_jwt(self):
         result_jwt = jwt_generator.build_ws_jwt(TEST_API_KEY, TEST_API_SECRET)
 
-        decoded_data = jwt.decode(
-            result_jwt, TEST_API_SECRET, algorithms=["ES256"], audience=[WS_SERVICE]
-        )
+        decoded_data = jwt.decode(result_jwt, TEST_API_SECRET, algorithms=["ES256"])
         header_bytes = base64.urlsafe_b64decode(str(result_jwt.split(".")[0] + "=="))
         decoded_header = json.loads(header_bytes.decode("utf-8"))
 
         self.assertEqual(decoded_data["sub"], TEST_API_KEY)
         self.assertEqual(decoded_data["iss"], "coinbase-cloud")
-        self.assertEqual(decoded_data["aud"], [WS_SERVICE])
         self.assertNotIn("uri", decoded_data)
         self.assertEqual(decoded_header["kid"], TEST_API_KEY)
 
     def test_build_rest_jwt_error(self):
         with self.assertRaises(Exception):
             uri = jwt_generator.format_jwt_uri("GET", "/api/v3/brokerage/accounts")
             jwt_generator.build_rest_jwt(uri, TEST_API_KEY, "bad_secret")
```

### Comparing `coinbase-advanced-py-1.2.1/tests/websocket/mock_ws_server.py` & `coinbase-advanced-py-1.2.2/tests/websocket/mock_ws_server.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/websocket/test_channels.py` & `coinbase-advanced-py-1.2.2/tests/websocket/test_channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.1/tests/websocket/test_websocket_base.py` & `coinbase-advanced-py-1.2.2/tests/websocket/test_websocket_base.py`

 * *Files identical despite different names*

