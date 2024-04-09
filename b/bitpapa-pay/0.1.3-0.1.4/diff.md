# Comparing `tmp/bitpapa_pay-0.1.3.tar.gz` & `tmp/bitpapa_pay-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpapa_pay-0.1.3.tar", max compression
+gzip compressed data, was "bitpapa_pay-0.1.4.tar", max compression
```

## Comparing `bitpapa_pay-0.1.3.tar` & `bitpapa_pay-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1151 2024-03-19 14:47:17.270688 bitpapa_pay-0.1.3/README.md
--rw-r--r--   0        0        0       50 2024-04-09 08:50:44.260698 bitpapa_pay-0.1.3/bitpapa_pay/__init__.py
--rw-r--r--   0        0        0     3562 2024-04-09 10:13:10.010388 bitpapa_pay-0.1.3/bitpapa_pay/client.py
--rw-r--r--   0        0        0      473 2024-04-09 09:47:14.505171 bitpapa_pay-0.1.3/bitpapa_pay/methods/base.py
--rw-r--r--   0        0        0      625 2024-04-09 09:55:00.185493 bitpapa_pay-0.1.3/bitpapa_pay/methods/exchange_rates.py
--rw-r--r--   0        0        0     2325 2024-04-09 09:55:17.053511 bitpapa_pay-0.1.3/bitpapa_pay/methods/telegram.py
--rw-r--r--   0        0        0       18 2024-04-09 10:09:42.228510 bitpapa_pay-0.1.3/bitpapa_pay/version.py
--rw-r--r--   0        0        0      371 2024-04-09 10:02:17.386048 bitpapa_pay-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1155 2024-04-09 10:23:59.770129 bitpapa_pay-0.1.4/README.md
+-rw-r--r--   0        0        0       50 2024-04-09 08:50:44.260698 bitpapa_pay-0.1.4/bitpapa_pay/__init__.py
+-rw-r--r--   0        0        0     3562 2024-04-09 10:22:00.217588 bitpapa_pay-0.1.4/bitpapa_pay/client.py
+-rw-r--r--   0        0        0      473 2024-04-09 09:47:14.505171 bitpapa_pay-0.1.4/bitpapa_pay/methods/base.py
+-rw-r--r--   0        0        0      625 2024-04-09 09:55:00.185493 bitpapa_pay-0.1.4/bitpapa_pay/methods/exchange_rates.py
+-rw-r--r--   0        0        0     2325 2024-04-09 09:55:17.053511 bitpapa_pay-0.1.4/bitpapa_pay/methods/telegram.py
+-rw-r--r--   0        0        0       18 2024-04-09 10:25:31.978520 bitpapa_pay-0.1.4/bitpapa_pay/version.py
+-rw-r--r--   0        0        0      371 2024-04-09 10:25:28.650506 bitpapa_pay-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.4/PKG-INFO
```

### Comparing `bitpapa_pay-0.1.3/README.md` & `bitpapa_pay-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 ```
     
 ## Usage/Examples
 
 ```python
 import asyncio
 
-from bitpapa_pay import BitpapaPay
+from bitpapa_pay import TelegramBitpapaPay
 
 
 async def main():
-    bitpapa = BitpapaPay(api_token="wDSJlwtszc-MsrdRSbyo")
-    result = await bitpapa.create_telegram_invoice("USDT", 100)
+    bitpapa_pay = TelegramBitpapaPay(api_token="api_token")
+    result = await bitpapa_pay.create_invoice("USDT", -100)
     print(result.model_dump())
     print(
         result.invoice.id,
         result.invoice.currency_code,
         result.invoice.amount,
         result.invoice.status,
         result.invoice.created_at,
         result.invoice.updated_at,
         result.invoice.url
     )
-    result = await bitpapa.get_telegram_invoices()
+    result = await bitpapa_pay.get_invoices()
     for invoice in result.invoices:
         print(
             invoice.id,
             invoice.currency_code,
             invoice.amount,
             invoice.status,
             invoice.created_at,
             invoice.updated_at,
             invoice.url
         )
-    result = await bitpapa.get_exchange_rates_all()
+    result = await bitpapa_pay.get_exchange_rates_all()
     print(result)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `bitpapa_pay-0.1.3/bitpapa_pay/client.py` & `bitpapa_pay-0.1.4/bitpapa_pay/client.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.3/bitpapa_pay/methods/exchange_rates.py` & `bitpapa_pay-0.1.4/bitpapa_pay/methods/exchange_rates.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.3/bitpapa_pay/methods/telegram.py` & `bitpapa_pay-0.1.4/bitpapa_pay/methods/telegram.py`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.3/PKG-INFO` & `bitpapa_pay-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpapa-pay
-Version: 0.1.3
+Version: 0.1.4
 Summary: Bitpapa Pay async python wrapper
 Author: VasilevAlexandr97
 Author-email: vasilev.alex.work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,42 +32,42 @@
 ```
     
 ## Usage/Examples
 
 ```python
 import asyncio
 
-from bitpapa_pay import BitpapaPay
+from bitpapa_pay import TelegramBitpapaPay
 
 
 async def main():
-    bitpapa = BitpapaPay(api_token="wDSJlwtszc-MsrdRSbyo")
-    result = await bitpapa.create_telegram_invoice("USDT", 100)
+    bitpapa_pay = TelegramBitpapaPay(api_token="api_token")
+    result = await bitpapa_pay.create_invoice("USDT", -100)
     print(result.model_dump())
     print(
         result.invoice.id,
         result.invoice.currency_code,
         result.invoice.amount,
         result.invoice.status,
         result.invoice.created_at,
         result.invoice.updated_at,
         result.invoice.url
     )
-    result = await bitpapa.get_telegram_invoices()
+    result = await bitpapa_pay.get_invoices()
     for invoice in result.invoices:
         print(
             invoice.id,
             invoice.currency_code,
             invoice.amount,
             invoice.status,
             invoice.created_at,
             invoice.updated_at,
             invoice.url
         )
-    result = await bitpapa.get_exchange_rates_all()
+    result = await bitpapa_pay.get_exchange_rates_all()
     print(result)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

