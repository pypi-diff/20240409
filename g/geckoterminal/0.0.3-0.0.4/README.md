# Comparing `tmp/geckoterminal-0.0.3.tar.gz` & `tmp/geckoterminal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geckoterminal-0.0.3.tar", last modified: Tue Apr  9 18:51:51 2024, max compression
+gzip compressed data, was "geckoterminal-0.0.4.tar", last modified: Tue Apr  9 19:24:05 2024, max compression
```

## Comparing `geckoterminal-0.0.3.tar` & `geckoterminal-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.986448 geckoterminal-0.0.3/
--rw-r--r--   0 samuel     (501) staff       (20)     1063 2023-10-27 20:26:39.000000 geckoterminal-0.0.3/LICENSE
--rw-r--r--   0 samuel     (501) staff       (20)      693 2024-04-09 18:51:51.986171 geckoterminal-0.0.3/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      490 2024-04-09 18:47:29.000000 geckoterminal-0.0.3/README.md
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.982237 geckoterminal-0.0.3/geckoterminal/
--rw-r--r--   0 samuel     (501) staff       (20)       18 2023-10-25 20:20:39.000000 geckoterminal-0.0.3/geckoterminal/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     3217 2023-10-27 20:15:02.000000 geckoterminal-0.0.3/geckoterminal/api.py
--rw-r--r--   0 samuel     (501) staff       (20)      640 2023-10-23 03:46:08.000000 geckoterminal-0.0.3/geckoterminal/client.py
--rw-r--r--   0 samuel     (501) staff       (20)      141 2023-07-24 16:10:03.000000 geckoterminal-0.0.3/geckoterminal/config.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.984969 geckoterminal-0.0.3/geckoterminal.egg-info/
--rw-r--r--   0 samuel     (501) staff       (20)      693 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      323 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/SOURCES.txt
--rw-r--r--   0 samuel     (501) staff       (20)        1 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/dependency_links.txt
--rw-r--r--   0 samuel     (501) staff       (20)       30 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/requires.txt
--rw-r--r--   0 samuel     (501) staff       (20)       14 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/top_level.txt
--rw-r--r--   0 samuel     (501) staff       (20)       38 2024-04-09 18:51:51.986510 geckoterminal-0.0.3/setup.cfg
--rw-r--r--   0 samuel     (501) staff       (20)      383 2024-04-09 18:51:29.000000 geckoterminal-0.0.3/setup.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.985623 geckoterminal-0.0.3/tests/
--rw-r--r--   0 samuel     (501) staff       (20)     1522 2023-10-30 17:15:15.000000 geckoterminal-0.0.3/tests/test_api.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 19:24:05.117874 geckoterminal-0.0.4/
+-rw-r--r--   0 samuel     (501) staff       (20)     1063 2023-10-27 20:26:39.000000 geckoterminal-0.0.4/LICENSE
+-rw-r--r--   0 samuel     (501) staff       (20)      894 2024-04-09 19:24:05.117616 geckoterminal-0.0.4/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)      691 2024-04-09 19:18:58.000000 geckoterminal-0.0.4/README.md
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 19:24:05.113311 geckoterminal-0.0.4/geckoterminal/
+-rw-r--r--   0 samuel     (501) staff       (20)       18 2023-10-25 20:20:39.000000 geckoterminal-0.0.4/geckoterminal/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     3546 2024-04-09 19:14:39.000000 geckoterminal-0.0.4/geckoterminal/api.py
+-rw-r--r--   0 samuel     (501) staff       (20)      640 2023-10-23 03:46:08.000000 geckoterminal-0.0.4/geckoterminal/client.py
+-rw-r--r--   0 samuel     (501) staff       (20)      141 2023-07-24 16:10:03.000000 geckoterminal-0.0.4/geckoterminal/config.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 19:24:05.116304 geckoterminal-0.0.4/geckoterminal.egg-info/
+-rw-r--r--   0 samuel     (501) staff       (20)      894 2024-04-09 19:24:05.000000 geckoterminal-0.0.4/geckoterminal.egg-info/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)      323 2024-04-09 19:24:05.000000 geckoterminal-0.0.4/geckoterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel     (501) staff       (20)        1 2024-04-09 19:24:05.000000 geckoterminal-0.0.4/geckoterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       30 2024-04-09 19:24:05.000000 geckoterminal-0.0.4/geckoterminal.egg-info/requires.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       14 2024-04-09 19:24:05.000000 geckoterminal-0.0.4/geckoterminal.egg-info/top_level.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       38 2024-04-09 19:24:05.117927 geckoterminal-0.0.4/setup.cfg
+-rw-r--r--   0 samuel     (501) staff       (20)      383 2024-04-09 19:14:52.000000 geckoterminal-0.0.4/setup.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 19:24:05.116826 geckoterminal-0.0.4/tests/
+-rw-r--r--   0 samuel     (501) staff       (20)     1522 2023-10-30 17:15:15.000000 geckoterminal-0.0.4/tests/test_api.py
```

### Comparing `geckoterminal-0.0.3/LICENSE` & `geckoterminal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geckoterminal-0.0.3/PKG-INFO` & `geckoterminal-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: geckoterminal
-Version: 0.0.3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.0.0
-Requires-Dist: pandas>=2.0.0
-
 # GeckoTerminal
 
 Python wrapper for GeckoTerminal's API.
 
 ## Installation
 ```
 pip3 install geckoterminal
@@ -22,10 +13,15 @@
 
 ## Quick Start
 ```python
 import geckoterminal
 
 networks = geckoterminal.get_networks()
 dexes = geckoterminal.get_dexes(network='eth')
-weth_usdc = geckoterminal.get_pool(network='eth', pool_address='0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640')
+weth_usdc = geckoterminal.get_pool(network='eth', pool_address='0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640') # WETH/USDC Uniswap v3 0.05%
 polygon_top_pools = geckoterminal.get_top_pools(network='polygon_pos')
+weth_usdc_trades = geckoterminal.get_trades(
+    network='eth',
+    pool_address='0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640',
+    trade_volume_in_usd_greater_than=10000
+)
 ```
```

### Comparing `geckoterminal-0.0.3/geckoterminal/api.py` & `geckoterminal-0.0.4/geckoterminal/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,8 +106,17 @@
 
     response = client.request(f'/networks/{network}/pools/{pool_address}/ohlcv/{timeframe}', params=params)
 
     if df:
         ohlcv_list = response['data']['attributes']['ohlcv_list']
         return pd.DataFrame(ohlcv_list, columns=config.OHLCV_COLUMNS)
 
-    return response
+    return response
+
+def get_trades(network, pool_address, trade_volume_in_usd_greater_than=0):
+    # Returns last 300 trades in past 24 hours from pool
+    
+    params = {
+        'trade_volume_in_usd_greater_than':trade_volume_in_usd_greater_than
+    }
+
+    return client.request(f'/networks/{network}/pools/{pool_address}/trades', params=params)
```

### Comparing `geckoterminal-0.0.3/geckoterminal/client.py` & `geckoterminal-0.0.4/geckoterminal/client.py`

 * *Files identical despite different names*

### Comparing `geckoterminal-0.0.3/tests/test_api.py` & `geckoterminal-0.0.4/tests/test_api.py`

 * *Files identical despite different names*

