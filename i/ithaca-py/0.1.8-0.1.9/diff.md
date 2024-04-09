# Comparing `tmp/ithaca_py-0.1.8.tar.gz` & `tmp/ithaca_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.1.8.tar", max compression
+gzip compressed data, was "ithaca_py-0.1.9.tar", max compression
```

## Comparing `ithaca_py-0.1.8.tar` & `ithaca_py-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-04 10:51:20.167172 ithaca_py-0.1.8/README.md
--rw-r--r--   0        0        0     5147 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/calculation.py
--rw-r--r--   0        0        0     2921 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/market.py
--rw-r--r--   0        0        0     6451 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-04 10:51:20.171172 ithaca_py-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-09 06:25:17.930162 ithaca_py-0.1.9/README.md
+-rw-r--r--   0        0        0     5147 2024-04-09 06:25:17.930162 ithaca_py-0.1.9/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-09 06:25:17.930162 ithaca_py-0.1.9/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-04-09 06:25:17.930162 ithaca_py-0.1.9/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/calculation.py
+-rw-r--r--   0        0        0     2921 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/market.py
+-rw-r--r--   0        0        0     6650 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/protocol.py
+-rw-r--r--   0        0        0     2210 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/ithaca/socket.py
+-rw-r--r--   0        0        0      948 2024-04-09 06:25:17.934162 ithaca_py-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 ithaca_py-0.1.9/PKG-INFO
```

### Comparing `ithaca_py-0.1.8/README.md` & `ithaca_py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/__init__.py` & `ithaca_py-0.1.9/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/analytics.py` & `ithaca_py-0.1.9/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/auth.py` & `ithaca_py-0.1.9/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/calculation.py` & `ithaca_py-0.1.9/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/client.py` & `ithaca_py-0.1.9/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/constants.py` & `ithaca_py-0.1.9/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/fundlock.py` & `ithaca_py-0.1.9/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/market.py` & `ithaca_py-0.1.9/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/orders.py` & `ithaca_py-0.1.9/ithaca/orders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Orders Module."""
 
 from datetime import datetime, timezone
 
 
-def create_client_order_id(value=101) -> int:
-    """Create a 'random' client order id."""
-    return int(
-        (datetime.now().astimezone(timezone.utc).timestamp() * 2**10 + value) * 1000
-    )
-
-
 class Orders:
     """Orders class."""
 
     def __init__(self, parent):
         """Class constructor."""
         self.parent = parent
 
+    def create_client_order_id(self, value=101) -> int:
+        """Create a 'random' client order id."""
+        return int(
+            (datetime.now().astimezone(timezone.utc).timestamp() * 2 ** 10 + value) * 1000
+        )
+
     def sign_order(self, order):
         """Sign Order."""
         raw_order = {
             "types": {
                 "EIP712Domain": [
                     {"name": "name", "type": "string"},
                     {"name": "version", "type": "string"},
@@ -61,21 +60,22 @@
                 "contractId": contract_id,
                 "side": side,
                 "quantity": f"{qty:.4f}",
             }
         return self.parent.auth.sign_message(raw_order)
 
     def new_order(
-        self,
-        legs,
-        price,
-        order_type="LIMIT",
-        time_in_force="GOOD_TILL_CANCEL",
-        request_single_price=True,
-        order_descr="",
+            self,
+            legs,
+            price,
+            client_order_id=None,
+            order_type="LIMIT",
+            time_in_force="GOOD_TILL_CANCEL",
+            request_single_price=True,
+            order_descr="",
     ):
         """Send new order request to Ithaca backend.
 
         Args:
             legs (list): list of legs as
                      (contractId: int, side: 'BUY' | 'SELL', quantity: float)
             price (float): Order limit for the conditional order
@@ -87,15 +87,16 @@
         Example:
             legs: [(5559, "SELL", 1), (5563, "BUY", 1)]
 
         Returns:
             json: {'result': 'OK', 'details': '', 'clientOrderId': 1742473240341423}
         """
         legs = sorted(legs, key=lambda x: x[0])
-        client_order_id = create_client_order_id()
+        if client_order_id is None:
+            client_order_id = self.create_client_order_id()
 
         order = {
             "clientOrderId": client_order_id,
             "totalNetPrice": f"{price:.4f}",
             "legs": legs,
             "orderType": order_type,
             "timeInForce": time_in_force,
@@ -124,17 +125,18 @@
             return {**res, "clientOrderId": client_order_id}
         except TypeError:
             return {"result": "ERROR", "clientOrderId": client_order_id}
 
     def new_orders(self, orders, order_descr=""):
         """Send new orders request to Ithaca backend."""
         payload = []
-        for legs, price in orders:
+        for legs, price,client_order_id in orders:
             legs = sorted(legs, key=lambda x: x[0])
-            client_order_id = create_client_order_id()
+            if client_order_id is None:
+                client_order_id = self.create_client_order_id()
 
             order = {
                 "clientOrderId": client_order_id,
                 "totalNetPrice": f"{price:.4f}",
                 "legs": legs,
                 "orderType": "LIMIT",
                 "timeInForce": "GOOD_TILL_CANCEL",
```

### Comparing `ithaca_py-0.1.8/ithaca/protocol.py` & `ithaca_py-0.1.9/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/ithaca/socket.py` & `ithaca_py-0.1.9/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.8/pyproject.toml` & `ithaca_py-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.1.8"
+version = "0.1.9"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,14 +14,15 @@
 eth-account = "^0.10.0"
 pandas = "^2.1.4"
 scipy = "^1.11.4"
 pydantic = "^2.5.3"
 websocket-client = "^1.7.0"
 web3 = "^6.13.0"
 cryptography = "^42.0.5"
+jupyter = "^1.0.0"
 
 
 [tool.poetry.group.lint.dependencies]
 flake8 = "^6.1.0"
 black = ">=23.12.1,<25.0.0"
 isort = "^5.13.2"
 mypy = "^1.8.0"
```

### Comparing `ithaca_py-0.1.8/PKG-INFO` & `ithaca_py-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: eth-account (>=0.10.0,<0.11.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pre-commit (>=3.6.0,<4.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: web3 (>=6.13.0,<7.0.0)
```

