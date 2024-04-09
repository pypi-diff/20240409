# Comparing `tmp/easy_kite_methods-0.0.6.tar.gz` & `tmp/easy_kite_methods-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_kite_methods-0.0.6.tar", max compression
+gzip compressed data, was "easy_kite_methods-0.0.7.tar", max compression
```

## Comparing `easy_kite_methods-0.0.6.tar` & `easy_kite_methods-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.6/README.md
--rw-r--r--   0        0        0      510 2024-04-09 06:07:05.486197 easy_kite_methods-0.0.6/easy_kite_methods/__init__.py
--rw-r--r--   0        0        0     1627 2024-04-09 08:41:07.253656 easy_kite_methods-0.0.6/easy_kite_methods/kite_login.py
--rw-r--r--   0        0        0    17907 2024-04-09 08:41:27.047322 easy_kite_methods-0.0.6/easy_kite_methods/order_placement.py
--rw-r--r--   0        0        0      555 2024-04-09 08:42:47.851686 easy_kite_methods-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.7/README.md
+-rw-r--r--   0        0        0      510 2024-04-09 06:07:05.486197 easy_kite_methods-0.0.7/easy_kite_methods/__init__.py
+-rw-r--r--   0        0        0     1627 2024-04-09 08:41:07.253656 easy_kite_methods-0.0.7/easy_kite_methods/kite_login.py
+-rw-r--r--   0        0        0    17430 2024-04-09 08:45:49.597761 easy_kite_methods-0.0.7/easy_kite_methods/order_placement.py
+-rw-r--r--   0        0        0      555 2024-04-09 08:46:14.411967 easy_kite_methods-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.7/PKG-INFO
```

### Comparing `easy_kite_methods-0.0.6/README.md` & `easy_kite_methods-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.6/easy_kite_methods/kite_login.py` & `easy_kite_methods-0.0.7/easy_kite_methods/kite_login.py`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.6/easy_kite_methods/order_placement.py` & `easy_kite_methods-0.0.7/easy_kite_methods/order_placement.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,17 +238,14 @@
             if variety.upper() is "CO":
                 order_id = kite.modify_order(variety=kite.VARIETY_CO, order_id=order_id,
                                              quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
 
             if variety.upper() is "AMO":
                 order_id = kite.modify_order(variety=kite.VARIETY_AMO, order_id=order_id,
                                              quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
-            if variety.upper() is "BO":
-                order_id = kite.modify_order(variety=kite.VARIETY_BO, order_id=order_id,
-                                             quantity=quantity, order_type=kite.ORDER_TYPE_MARKET)
             break
         except (
                 NetworkException, DataException, KeyError, ReadTimeout,
                 ConnectionError, ConnectionResetError, ConnectionAbortedError,
                 ConnectionRefusedError, ConnectTimeoutError):
             tried += 1
             sleep(WAIT_BEFORE_RETRY)
@@ -272,17 +269,14 @@
 
             if variety.upper() is "CO":
                 variety = kite.VARIETY_CO
 
             if variety.upper() is "AMO":
                 variety = kite.VARIETY_AMO
 
-            if variety.upper() is "BO":
-                variety = kite.VARIETY_BO
-
             order_id = kite.modify_order(variety=variety, order_id=order_id,
                                          price=price, order_type=kite.ORDER_TYPE_MARKET)
             break
         except (
                 NetworkException, DataException, KeyError, ReadTimeout,
                 ConnectionError, ConnectionResetError, ConnectionAbortedError,
                 ConnectionRefusedError, ConnectTimeoutError):
@@ -307,17 +301,14 @@
 
             if variety.upper() is "CO":
                 variety = kite.VARIETY_CO
 
             if variety.upper() is "AMO":
                 variety = kite.VARIETY_AMO
 
-            if variety.upper() is "BO":
-                variety = kite.VARIETY_BO
-
             order_id = kite.modify_order(
                 variety=variety, order_id=order_id, order_type=kite.TRANSACTION_TYPE_SELL)
             break
         except (
                 NetworkException, DataException, KeyError, ReadTimeout,
                 ConnectionError, ConnectionResetError, ConnectionAbortedError,
                 ConnectionRefusedError, ConnectTimeoutError):
@@ -342,17 +333,14 @@
 
             if variety.upper() is "CO":
                 variety = kite.VARIETY_CO
 
             if variety.upper() is "AMO":
                 variety = kite.VARIETY_AMO
 
-            if variety.upper() is "BO":
-                variety = kite.VARIETY_BO
-
             order_id = kite.modify_order(
                 variety=variety, order_id=order_id, order_type=kite.TRANSACTION_TYPE_BUY)
             break
         except (
                 NetworkException, DataException, KeyError, ReadTimeout,
                 ConnectionError, ConnectionResetError, ConnectionAbortedError,
                 ConnectionRefusedError, ConnectTimeoutError):
```

### Comparing `easy_kite_methods-0.0.6/pyproject.toml` & `easy_kite_methods-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_kite_methods"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Vivek Patel <vivekkvhpatel@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

### Comparing `easy_kite_methods-0.0.6/PKG-INFO` & `easy_kite_methods-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_kite_methods
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Vivek Patel
 Author-email: vivekkvhpatel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

