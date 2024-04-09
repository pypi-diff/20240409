# Comparing `tmp/bitpapa_pay-0.1.2.tar.gz` & `tmp/bitpapa_pay-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpapa_pay-0.1.2.tar", max compression
+gzip compressed data, was "bitpapa_pay-0.1.3.tar", max compression
```

## Comparing `bitpapa_pay-0.1.2.tar` & `bitpapa_pay-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,9 @@
--rw-r--r--   0        0        0     1151 2024-03-19 14:47:17.270688 bitpapa_pay-0.1.2/README.md
--rw-r--r--   0        0        0      111 2024-03-19 11:11:57.253911 bitpapa_pay-0.1.2/bitpapa_pay/__init__.py
--rw-r--r--   0        0        0       50 2024-03-18 23:20:52.341865 bitpapa_pay-0.1.2/bitpapa_pay/clients/__init__.py
--rw-r--r--   0        0        0      860 2024-03-24 21:51:27.826030 bitpapa_pay-0.1.2/bitpapa_pay/clients/base.py
--rw-r--r--   0        0        0     4421 2024-03-24 21:51:02.865903 bitpapa_pay-0.1.2/bitpapa_pay/clients/client.py
--rw-r--r--   0        0        0       17 2024-03-19 14:42:56.391296 bitpapa_pay-0.1.2/bitpapa_pay/const.py
--rw-r--r--   0        0        0      145 2024-03-19 00:07:37.345891 bitpapa_pay-0.1.2/bitpapa_pay/exceptions.py
--rw-r--r--   0        0        0      351 2024-03-19 01:22:34.285815 bitpapa_pay-0.1.2/bitpapa_pay/methods/__init__.py
--rw-r--r--   0        0        0      148 2024-03-19 01:02:41.650275 bitpapa_pay-0.1.2/bitpapa_pay/methods/base.py
--rw-r--r--   0        0        0      470 2024-03-24 21:52:58.790484 bitpapa_pay-0.1.2/bitpapa_pay/methods/create_telegram_invoice.py
--rw-r--r--   0        0        0      295 2024-03-24 21:53:25.926617 bitpapa_pay-0.1.2/bitpapa_pay/methods/get_exchange_rates_all.py
--rw-r--r--   0        0        0      312 2024-03-24 21:53:36.654669 bitpapa_pay-0.1.2/bitpapa_pay/methods/get_telegram_invoices.py
--rw-r--r--   0        0        0      193 2024-03-15 10:15:43.411887 bitpapa_pay-0.1.2/bitpapa_pay/types/__init__.py
--rw-r--r--   0        0        0       84 2024-03-15 09:43:19.679765 bitpapa_pay-0.1.2/bitpapa_pay/types/exchange_rates.py
--rw-r--r--   0        0        0      456 2024-03-24 21:49:20.041369 bitpapa_pay-0.1.2/bitpapa_pay/types/telegram_invoice.py
--rw-r--r--   0        0        0      371 2024-03-24 22:02:15.176889 bitpapa_pay-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1151 2024-03-19 14:47:17.270688 bitpapa_pay-0.1.3/README.md
+-rw-r--r--   0        0        0       50 2024-04-09 08:50:44.260698 bitpapa_pay-0.1.3/bitpapa_pay/__init__.py
+-rw-r--r--   0        0        0     3562 2024-04-09 10:13:10.010388 bitpapa_pay-0.1.3/bitpapa_pay/client.py
+-rw-r--r--   0        0        0      473 2024-04-09 09:47:14.505171 bitpapa_pay-0.1.3/bitpapa_pay/methods/base.py
+-rw-r--r--   0        0        0      625 2024-04-09 09:55:00.185493 bitpapa_pay-0.1.3/bitpapa_pay/methods/exchange_rates.py
+-rw-r--r--   0        0        0     2325 2024-04-09 09:55:17.053511 bitpapa_pay-0.1.3/bitpapa_pay/methods/telegram.py
+-rw-r--r--   0        0        0       18 2024-04-09 10:09:42.228510 bitpapa_pay-0.1.3/bitpapa_pay/version.py
+-rw-r--r--   0        0        0      371 2024-04-09 10:02:17.386048 bitpapa_pay-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 bitpapa_pay-0.1.3/PKG-INFO
```

### Comparing `bitpapa_pay-0.1.2/README.md` & `bitpapa_pay-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bitpapa_pay-0.1.2/PKG-INFO` & `bitpapa_pay-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpapa-pay
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bitpapa Pay async python wrapper
 Author: VasilevAlexandr97
 Author-email: vasilev.alex.work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

