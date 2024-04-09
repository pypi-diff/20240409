# Comparing `tmp/kucoin_futures_lib-0.2.1.tar.gz` & `tmp/kucoin_futures_lib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.2.1.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.2.2.tar", max compression
```

## Comparing `kucoin_futures_lib-0.2.1.tar` & `kucoin_futures_lib-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-08 19:47:51.564344 kucoin_futures_lib-0.2.1/LICENSE
--rw-r--r--   0        0        0       52 2024-04-08 19:47:51.564344 kucoin_futures_lib-0.2.1/README.md
--rw-r--r--   0        0        0      719 2024-04-08 19:47:51.564344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      251 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1977 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2555 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1419 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12864 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     2732 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/LICENSE
+-rw-r--r--   0        0        0       52 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/README.md
+-rw-r--r--   0        0        0      719 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1977 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2555 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1419 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    12789 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     2732 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.2/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.2.1/LICENSE` & `kucoin_futures_lib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/oco.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/trade.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,14 @@
             recent_fills = self.client.get_recent_fills()
             logger.debug("Recent fills: %s", json.dumps(recent_fills))
             if isinstance(recent_fills, list):
                 for fill in recent_fills:
                     if isinstance(fill, dict) and fill.get("orderId", "") == order_id:
                         logger.info("Order %s has been filled.", order_id)
                         return fill
-                logger.info("Order %s has not been filled yet.", order_id)
             else:
                 logger.warning("Unexpected recent fills response: %s", recent_fills)
             attempt += 1
             logger.info(
                 "Order %s has not been filled yet. Attempt %s/%s",
                 order_id,
                 attempt,
```

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.2.2/kucoin_futures_lib/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.1/PKG-INFO` & `kucoin_futures_lib-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

