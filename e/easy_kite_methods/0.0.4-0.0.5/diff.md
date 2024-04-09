# Comparing `tmp/easy_kite_methods-0.0.4.tar.gz` & `tmp/easy_kite_methods-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_kite_methods-0.0.4.tar", max compression
+gzip compressed data, was "easy_kite_methods-0.0.5.tar", max compression
```

## Comparing `easy_kite_methods-0.0.4.tar` & `easy_kite_methods-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.4/README.md
--rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.4/easy_kite_methods/__init__.py
--rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.4/easy_kite_methods/kite_login.py
--rw-r--r--   0        0        0     9668 2024-04-08 09:23:48.842896 easy_kite_methods-0.0.4/easy_kite_methods/order_placement.py
--rw-r--r--   0        0        0      555 2024-04-08 09:24:23.753792 easy_kite_methods-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.5/README.md
+-rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.5/easy_kite_methods/__init__.py
+-rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.5/easy_kite_methods/kite_login.py
+-rw-r--r--   0        0        0     9701 2024-04-08 10:54:32.982952 easy_kite_methods-0.0.5/easy_kite_methods/order_placement.py
+-rw-r--r--   0        0        0      555 2024-04-08 10:54:45.341570 easy_kite_methods-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.5/PKG-INFO
```

### Comparing `easy_kite_methods-0.0.4/README.md` & `easy_kite_methods-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.4/easy_kite_methods/kite_login.py` & `easy_kite_methods-0.0.5/easy_kite_methods/kite_login.py`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.4/easy_kite_methods/order_placement.py` & `easy_kite_methods-0.0.5/easy_kite_methods/order_placement.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,34 +47,36 @@
 def get_fno_price(fno_name: str):
     """
     name -> This is the name of the option instrument
     It can be either futures / options
     """
     while True:
         try:
+            fno_name.upper()
             value = kite.quote("NSE:" + fno_name)
             if (value[fno_name]['last_price'] >= 0):
                 break
         except (
                 NetworkException, DataException, KeyError, ReadTimeout,
                 ConnectionError, ConnectionResetError, ConnectionAbortedError,
                 ConnectionRefusedError, ConnectTimeoutError):
             pass
     return value
 
 
-def get_fno_instrument_token(stock_name: str):
+def get_fno_instrument_token(fno_name: str):
     """
     name -> This is the name of the option instrument
     It can be either futures / options
     """
     while True:
         try:
-            value = kite.quote("NFO:" + stock_name)
-            if (value[stock_name]['instrument_token'] >= 0):
+            fno_name.upper()
+            value = kite.quote("NFO:" + fno_name)
+            if (value[fno_name]['instrument_token'] >= 0):
                 break
         except (
                 NetworkException, DataException, KeyError, ReadTimeout,
                 ConnectionError, ConnectionResetError, ConnectionAbortedError,
                 ConnectionRefusedError, ConnectTimeoutError):
             pass
     return value
@@ -139,93 +141,93 @@
     quantity : Total number of orders
     """
 
     order_id = None
 
     if variety.upper() is "REGULAR":
         order_id = kite.modify_order(variety=kite.VARIETY_REGULAR, order_id=order_id,
-                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+                                     quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
 
     if variety.upper() is "CO":
-         order_id = kite.modify_order(variety=kite.VARIETY_CO, order_id=order_id,
-                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+        order_id = kite.modify_order(variety=kite.VARIETY_CO, order_id=order_id,
+                                     quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
 
     if variety.upper() is "AMO":
-         order_id = kite.modify_order(variety=kite.VARIETY_AMO, order_id=order_id,
-                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+        order_id = kite.modify_order(variety=kite.VARIETY_AMO, order_id=order_id,
+                                     quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
     if variety.upper() is "BO":
-         order_id = kite.modify_order(variety=kite.VARIETY_BO, order_id=order_id,
-                                 quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
+        order_id = kite.modify_order(variety=kite.VARIETY_BO, order_id=order_id,
+                                     quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
     return order_id
 
 
 def modify_order_price(variety, order_id, price):
     """
     order_id : This is the id of order executed
     variety : Variety can be [VARIETY_AMO
                             VARIETY_REGULAR ]
     price : Modified price of order
     """
     if variety.upper() is "REGULAR":
-         variety = kite.VARIETY_REGULAR
+        variety = kite.VARIETY_REGULAR
 
     if variety.upper() is "CO":
-         variety = kite.VARIETY_CO
+        variety = kite.VARIETY_CO
 
     if variety.upper() is "AMO":
         variety = kite.VARIETY_AMO
 
-    if variety.upper() is "BO" :
+    if variety.upper() is "BO":
         variety = kite.VARIETY_BO
-         
+
     order_id = kite.modify_order(variety=variety, order_id=order_id,
                                  price=price, order_type=kite.ORDER_TYPE_MARKET)
     return order_id
 
 
 def modify_order_to_sell(variety, order_id):
     """
     order_id : This is the id of order executed
     variety : Variety can be [VARIETY_AMO 
                             VARIETY_REGULAR ]                    
     """
-    if variety.upper() is "REGULAR" :
-         variety = kite.VARIETY_REGULAR
+    if variety.upper() is "REGULAR":
+        variety = kite.VARIETY_REGULAR
 
-    if variety.upper() is "CO" :
-         variety = kite.VARIETY_CO
-  
-    if variety.upper() is "AMO" :
+    if variety.upper() is "CO":
+        variety = kite.VARIETY_CO
+
+    if variety.upper() is "AMO":
         variety = kite.VARIETY_AMO
 
-    if variety.upper() is "BO" :
+    if variety.upper() is "BO":
         variety = kite.VARIETY_BO
 
     order_id = kite.modify_order(
         variety=variety, order_id=order_id, order_type=kite.TRANSACTION_TYPE_SELL)
-    
+
     return order_id
 
 
 def modify_order_to_buy(variety, order_id):
     """
     order_id : This is the id of order executed
     variety : Variety can be [VARIETY_AMO 
                             VARIETY_REGULAR ]                    
     """
-    if variety.upper() is "REGULAR" :
-         variety = kite.VARIETY_REGULAR
+    if variety.upper() is "REGULAR":
+        variety = kite.VARIETY_REGULAR
+
+    if variety.upper() is "CO":
+        variety = kite.VARIETY_CO
 
-    if variety.upper() is "CO" :
-         variety = kite.VARIETY_CO
-  
-    if variety.upper() is "AMO" :
+    if variety.upper() is "AMO":
         variety = kite.VARIETY_AMO
 
-    if variety.upper() is "BO" :
+    if variety.upper() is "BO":
         variety = kite.VARIETY_BO
 
     order_id = kite.modify_order(
         variety=variety, order_id=order_id, order_type=kite.TRANSACTION_TYPE_BUY)
     return order_id
```

### Comparing `easy_kite_methods-0.0.4/pyproject.toml` & `easy_kite_methods-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_kite_methods"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Vivek Patel <vivekkvhpatel@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

### Comparing `easy_kite_methods-0.0.4/PKG-INFO` & `easy_kite_methods-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_kite_methods
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Vivek Patel
 Author-email: vivekkvhpatel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

