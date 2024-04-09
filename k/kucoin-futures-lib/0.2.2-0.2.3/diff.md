# Comparing `tmp/kucoin_futures_lib-0.2.2.tar.gz` & `tmp/kucoin_futures_lib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.2.2.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.2.3.tar", max compression
```

## Comparing `kucoin_futures_lib-0.2.2.tar` & `kucoin_futures_lib-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/LICENSE
--rw-r--r--   0        0        0       52 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/README.md
--rw-r--r--   0        0        0      719 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      251 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     1977 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2555 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     1419 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    12789 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     2732 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      455 2024-04-08 22:52:46.795708 kucoin_futures_lib-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/LICENSE
+-rw-r--r--   0        0        0       52 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/README.md
+-rw-r--r--   0        0        0      719 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      251 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     1977 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2554 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     1775 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    12789 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     2786 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      455 2024-04-09 14:47:34.106620 kucoin_futures_lib-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.2.3/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.2.2/LICENSE` & `kucoin_futures_lib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/handlers/oco.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.market_order_id = market_order_id
         self.instrument = instrument
         self._canceled = asyncio.Event()
         self._cancel_order = cancel_order
         self._topic = "/contractMarket/tradeOrders"
 
     def __repr__(self):
-        return f"TpSlHandler({self.limit_order_id}, {self.market_order_id}, {self.instrument})"
+        return f"OcoHandler({self.instrument}, {self.limit_order_id}, {self.market_order_id})"
 
     @property
     def topic(self) -> str:
         """Return the topic supported by the handler."""
         return f"{self._topic}:{self.instrument}"
 
     @property
```

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 """A collection of helper functions for the Kucoin wrapper."""
 
 import logging
 import math
+from decimal import Decimal
 
 logger = logging.getLogger(__name__)
 
 
 class KucoinFuturesHelper:
     """Kucoin Helpers mixin class."""
 
     @staticmethod
     def calculate_lots(
-        investment_amount: float, current_price: float, lot_size: float
+        lot_size: float, current_price: float, investment_amount: float,
     ) -> int:
         """Calculate the maximum number of lots to buy based on the investment amount, current price, and lot size.
-        :param investment_amount: The maximum amount to invest.
-        :param current_price: The current price of the instrument.
         :param lot_size: The lot size for the instrument. E.g. 0.001 for BTC/USDT.
+        :param current_price: The current price of the instrument.
+        :param investment_amount: The maximum amount to invest.
         :return: The maximum number of lots to buy.
         """
         logger.debug(
             "Calculating lots to buy with investment amount %s, current price %s, and lot size %s",
             investment_amount,
             current_price,
             lot_size,
         )
+
+        if lot_size == 0 or current_price == 0 or investment_amount == 0:
+            return 0
+
+        current_price = Decimal(str(current_price))
+        investment_amount = Decimal(str(investment_amount))
+        lot_size = Decimal(str(lot_size))
+
         lot_price = current_price * lot_size
-        lots = investment_amount // lot_price
+        lots = (investment_amount / lot_price).to_integral_value(rounding='ROUND_FLOOR')  # Use Decimal's floor rounding
         return int(lots)
 
     @staticmethod
     def calculate_precision(tick_size: float) -> int:
         """Calculate the precision of a tick size.
         :param tick_size: The tick size to calculate the precision of.
         :return: The precision of the tick size.
```

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.2.2/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.2.3/kucoin_futures_lib/websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,23 +57,23 @@
         handler = EntryRangeHandler(
             instrument=instrument, entry_high=entry_high, entry_low=entry_low
         )
         await self.subscribe(handler, timeout)
 
     async def tp_sl_cancel(
         self,
+        instrument: str,
         tp_order_id: str,
         sl_order_id: str,
-        instrument: str,
         cancel_order: Union[Callable[[str], None], Callable[[str], Awaitable[None]]],
     ) -> None:
         """Listen for take profit and stop loss orders and cancel the other order when one is done.
-        :param tp_order_id: Take profit order ID
-        :param sl_order_id: Stop loss order ID
         :param instrument: Instrument symbol
+        :param tp_order_id: Take profit order ID, must be a limit order.
+        :param sl_order_id: Stop loss order ID, must be a market stop order.
         :param cancel_order: Function to cancel the order
         """
         handler = OcoHandler(
             limit_order_id=tp_order_id,
             market_order_id=sl_order_id,
             instrument=instrument,
             cancel_order=cancel_order,
```

### Comparing `kucoin_futures_lib-0.2.2/PKG-INFO` & `kucoin_futures_lib-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

