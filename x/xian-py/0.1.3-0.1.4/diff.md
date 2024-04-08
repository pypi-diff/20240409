# Comparing `tmp/xian_py-0.1.3.tar.gz` & `tmp/xian_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xian_py-0.1.3.tar", max compression
+gzip compressed data, was "xian_py-0.1.4.tar", max compression
```

## Comparing `xian_py-0.1.3.tar` & `xian_py-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4472 2024-02-21 22:59:58.766214 xian_py-0.1.3/README.md
--rw-r--r--   0        0        0      344 2024-03-20 14:43:11.530508 xian_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4755 2024-02-21 22:59:58.766680 xian_py-0.1.3/xian_py/encoding.py
--rw-r--r--   0        0        0     2320 2024-02-21 22:59:58.766767 xian_py-0.1.3/xian_py/formating.py
--rw-r--r--   0        0        0     3683 2024-03-20 14:43:11.533780 xian_py-0.1.3/xian_py/transactions.py
--rw-r--r--   0        0        0      387 2024-02-21 22:59:58.766926 xian_py-0.1.3/xian_py/utils.py
--rw-r--r--   0        0        0     1906 2024-02-21 22:59:58.767011 xian_py-0.1.3/xian_py/wallet.py
--rw-r--r--   0        0        0     6291 2024-03-20 14:29:49.515671 xian_py-0.1.3/xian_py/xian.py
--rw-r--r--   0        0        0     7299 2024-02-21 22:59:58.767235 xian_py-0.1.3/xian_py/xian_datetime.py
--rw-r--r--   0        0        0     4683 2024-02-21 22:59:58.767344 xian_py-0.1.3/xian_py/xian_decimal.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 xian_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4472 2024-02-21 22:59:58.766214 xian_py-0.1.4/README.md
+-rw-r--r--   0        0        0      344 2024-04-08 22:25:42.732388 xian_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4755 2024-02-21 22:59:58.766680 xian_py-0.1.4/xian_py/encoding.py
+-rw-r--r--   0        0        0     2320 2024-02-21 22:59:58.766767 xian_py-0.1.4/xian_py/formating.py
+-rw-r--r--   0        0        0     3683 2024-04-08 21:58:17.489646 xian_py-0.1.4/xian_py/transactions.py
+-rw-r--r--   0        0        0      387 2024-04-08 21:58:01.758197 xian_py-0.1.4/xian_py/utils.py
+-rw-r--r--   0        0        0     1906 2024-02-21 22:59:58.767011 xian_py-0.1.4/xian_py/wallet.py
+-rw-r--r--   0        0        0     6593 2024-04-08 22:25:24.966190 xian_py-0.1.4/xian_py/xian.py
+-rw-r--r--   0        0        0     7299 2024-02-21 22:59:58.767235 xian_py-0.1.4/xian_py/xian_datetime.py
+-rw-r--r--   0        0        0     4683 2024-02-21 22:59:58.767344 xian_py-0.1.4/xian_py/xian_decimal.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 xian_py-0.1.4/PKG-INFO
```

### Comparing `xian_py-0.1.3/README.md` & `xian_py-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/xian_py/encoding.py` & `xian_py-0.1.4/xian_py/encoding.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/xian_py/formating.py` & `xian_py-0.1.4/xian_py/formating.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/xian_py/transactions.py` & `xian_py-0.1.4/xian_py/transactions.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/xian_py/wallet.py` & `xian_py-0.1.4/xian_py/wallet.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/xian_py/xian.py` & `xian_py-0.1.4/xian_py/xian.py`

 * *Files 7% similar despite different names*

```diff
@@ -198,7 +198,20 @@
         :returns:
         - success - Boolean. True if successful
         - data - String. Transaction hash
         """
 
         kwargs = {"name": name, "code": code}
         return self.send_tx('submission', 'submit_contract', kwargs, stamps, chain_id)
+
+    def get_nodes(self) -> list:
+        """ Retrieve list of nodes from the network """
+
+        r = requests.post(f'{self.node_url}/net_info')
+        peers = r.json()['result']['peers']
+
+        ips = list()
+
+        for peer in peers:
+            ips.append(peer['remote_ip'])
+
+        return ips
```

### Comparing `xian_py-0.1.3/xian_py/xian_datetime.py` & `xian_py-0.1.4/xian_py/xian_datetime.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/xian_py/xian_decimal.py` & `xian_py-0.1.4/xian_py/xian_decimal.py`

 * *Files identical despite different names*

### Comparing `xian_py-0.1.3/PKG-INFO` & `xian_py-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xian-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python tools to interact with the Xian blockchain
 License: MIT
 Author: endogen
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

