# Comparing `tmp/easy_kite_methods-0.0.5.tar.gz` & `tmp/easy_kite_methods-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_kite_methods-0.0.5.tar", max compression
+gzip compressed data, was "easy_kite_methods-0.0.6.tar", max compression
```

## Comparing `easy_kite_methods-0.0.5.tar` & `easy_kite_methods-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.5/README.md
--rw-r--r--   0        0        0      510 2024-04-08 06:19:05.831494 easy_kite_methods-0.0.5/easy_kite_methods/__init__.py
--rw-r--r--   0        0        0     1627 2024-04-08 05:46:27.884702 easy_kite_methods-0.0.5/easy_kite_methods/kite_login.py
--rw-r--r--   0        0        0     9701 2024-04-08 10:54:32.982952 easy_kite_methods-0.0.5/easy_kite_methods/order_placement.py
--rw-r--r--   0        0        0      555 2024-04-08 10:54:45.341570 easy_kite_methods-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3640 2024-04-08 09:17:23.806185 easy_kite_methods-0.0.6/README.md
+-rw-r--r--   0        0        0      510 2024-04-09 06:07:05.486197 easy_kite_methods-0.0.6/easy_kite_methods/__init__.py
+-rw-r--r--   0        0        0     1627 2024-04-09 08:41:07.253656 easy_kite_methods-0.0.6/easy_kite_methods/kite_login.py
+-rw-r--r--   0        0        0    17907 2024-04-09 08:41:27.047322 easy_kite_methods-0.0.6/easy_kite_methods/order_placement.py
+-rw-r--r--   0        0        0      555 2024-04-09 08:42:47.851686 easy_kite_methods-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 easy_kite_methods-0.0.6/PKG-INFO
```

### Comparing `easy_kite_methods-0.0.5/README.md` & `easy_kite_methods-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.5/easy_kite_methods/kite_login.py` & `easy_kite_methods-0.0.6/easy_kite_methods/kite_login.py`

 * *Files identical despite different names*

### Comparing `easy_kite_methods-0.0.5/pyproject.toml` & `easy_kite_methods-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_kite_methods"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Vivek Patel <vivekkvhpatel@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

### Comparing `easy_kite_methods-0.0.5/PKG-INFO` & `easy_kite_methods-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_kite_methods
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Vivek Patel
 Author-email: vivekkvhpatel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

