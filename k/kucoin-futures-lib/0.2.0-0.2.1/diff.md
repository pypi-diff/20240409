# Comparing `tmp/kucoin_futures_lib-0.2.0.tar.gz` & `tmp/kucoin_futures_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.2.0.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.2.1.tar", max compression
```

## Comparing `kucoin_futures_lib-0.2.0.tar` & `kucoin_futures_lib-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/LICENSE
--rw-r--r--   0        0        0       52 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/README.md
--rw-r--r--   0        0        0      719 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      251 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1920 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2499 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1419 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-08 18:45:50.312869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12864 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     2732 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-08 18:45:50.316869 kucoin_futures_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 19:47:51.564344 kucoin_futures_lib-0.2.1/LICENSE
+-rw-r--r--   0        0        0       52 2024-04-08 19:47:51.564344 kucoin_futures_lib-0.2.1/README.md
+-rw-r--r--   0        0        0      719 2024-04-08 19:47:51.564344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1977 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2555 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1419 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    12864 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     2732 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-08 19:47:51.568344 kucoin_futures_lib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.1/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.2.0/LICENSE` & `kucoin_futures_lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,19 +41,24 @@
         return False
 
     async def handle(self, msg):
         """Handle the trade order message from
         :param msg: The trade order message.
         https://www.kucoin.com/docs/websocket/futures-trading/public-channels/get-ticker-v2
         """
+
+        if self._entered.is_set():
+            return
+
         ticker = msg.get("data", {})
         best_bid_price = float(ticker.get("bestBidPrice", 0))
         best_ask_price = float(ticker.get("bestAskPrice", 0))
         if best_bid_price >= self.entry_low and best_ask_price <= self.entry_high:
+            self._entered.set()
             logger.info(
                 "Instrument %s has reached the entry range: %s <= %s <= %s",
                 self.instrument,
                 self.entry_low,
                 best_bid_price,
                 self.entry_high,
             )
-            self._entered.set()
+
```

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/handlers/oco.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         return self._canceled
 
     async def handle(self, msg: Dict):
         """Handle the trade order message from
         :param msg: The trade order message.
         https://www.kucoin.com/docs/websocket/futures-trading/private-channels/trade-orders
         """
+        if self._canceled.is_set():
+            return
+
         trade_order = msg.get("data", {})
         order_id = trade_order.get("orderId", "")
         status = trade_order.get("status", "")
 
         if status == "done":
             if order_id == self.limit_order_id:
                 logger.info("Limit order %s is done.", self.limit_order_id)
```

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.0/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.2.1/kucoin_futures_lib/websocket.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,32 @@
                 await handler.done.wait()
         except asyncio.TimeoutError:
             logger.warning("Timeout reached. Unsubscribing from %s", handler.topic)
             handler.done.set()
         finally:
             await ws_client.unsubscribe(handler.topic)
 
+    async def listen_for_entry(
+        self,
+        instrument: str,
+        entry_high: float,
+        entry_low: float,
+        timeout: float = 60 * 60 * 12,
+    ) -> None:
+        """Listen for the entry price range.
+        :param instrument: Instrument symbol
+        :param entry_high: Entry high price
+        :param entry_low: Entry low price
+        :param timeout: timeout in seconds. Default is 12 hours
+        """
+        handler = EntryRangeHandler(
+            instrument=instrument, entry_high=entry_high, entry_low=entry_low
+        )
+        await self.subscribe(handler, timeout)
+
     async def tp_sl_cancel(
         self,
         tp_order_id: str,
         sl_order_id: str,
         instrument: str,
         cancel_order: Union[Callable[[str], None], Callable[[str], Awaitable[None]]],
     ) -> None:
@@ -57,25 +75,7 @@
         handler = OcoHandler(
             limit_order_id=tp_order_id,
             market_order_id=sl_order_id,
             instrument=instrument,
             cancel_order=cancel_order,
         )
         await self.subscribe(handler, None)
-
-    async def listen_for_entry(
-        self,
-        instrument: str,
-        entry_high: float,
-        entry_low: float,
-        timeout: float = 60 * 60 * 12,
-    ) -> None:
-        """Listen for the entry price range.
-        :param instrument: Instrument symbol
-        :param entry_high: Entry high price
-        :param entry_low: Entry low price
-        :param timeout: timeout in seconds. Default is 12 hours
-        """
-        handler = EntryRangeHandler(
-            instrument=instrument, entry_high=entry_high, entry_low=entry_low
-        )
-        await self.subscribe(handler, timeout)
```

### Comparing `kucoin_futures_lib-0.2.0/PKG-INFO` & `kucoin_futures_lib-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

