# Comparing `tmp/chainbench-0.6.5.tar.gz` & `tmp/chainbench-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.6.5.tar", max compression
+gzip compressed data, was "chainbench-0.6.6.tar", max compression
```

## Comparing `chainbench-0.6.5.tar` & `chainbench-0.6.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2024-02-16 07:31:38.567934 chainbench-0.6.5/LICENSE
--rw-r--r--   0        0        0    12165 2024-02-16 07:31:38.567934 chainbench-0.6.5/README.md
--rw-r--r--   0        0        0        0 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/__main__.py
--rw-r--r--   0        0        0    14999 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/main.py
--rw-r--r--   0        0        0        0 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3731 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2759 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     1157 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/ethereum/consensus.py
--rw-r--r--   0        0        0     2703 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      344 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/evm/all.py
--rw-r--r--   0        0        0     1272 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/evm/debug_trace.py
--rw-r--r--   0        0        0      427 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4251 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1654 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1931 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2896 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0     3513 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/solana/general.py
--rw-r--r--   0        0        0     2222 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/profile/starknet/wallet.py
--rw-r--r--   0        0        0      599 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     6482 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/test_data/blockchain.py
--rw-r--r--   0        0        0     5985 2024-02-16 07:31:38.567934 chainbench-0.6.5/chainbench/test_data/ethereum.py
--rw-r--r--   0        0        0    11721 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/test_data/evm.py
--rw-r--r--   0        0        0     5443 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/test_data/solana.py
--rw-r--r--   0        0        0     2284 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/test_data/starknet.py
--rw-r--r--   0        0        0       24 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/tools/__init__.py
--rw-r--r--   0        0        0       18 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/tools/discovery/__init__.py
--rw-r--r--   0        0        0      977 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/tools/discovery/clients.json
--rw-r--r--   0        0        0    55080 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/tools/discovery/methods.json
--rw-r--r--   0        0        0     5499 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/tools/discovery/rpc.py
--rw-r--r--   0        0        0      416 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/__init__.py
--rw-r--r--   0        0        0     2895 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/ethereum.py
--rw-r--r--   0        0        0     4622 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/evm.py
--rw-r--r--   0        0        0     4632 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/http.py
--rw-r--r--   0        0        0      799 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/methods/__init__.py
--rw-r--r--   0        0        0      516 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/methods/common.py
--rw-r--r--   0        0        0     9075 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/methods/ethereum.py
--rw-r--r--   0        0        0     8591 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/methods/evm.py
--rw-r--r--   0        0        0     2885 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/solana.py
--rw-r--r--   0        0        0     3680 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/user/starknet.py
--rw-r--r--   0        0        0        0 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/__init__.py
--rw-r--r--   0        0        0     6218 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/cli.py
--rw-r--r--   0        0        0    12931 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/event.py
--rw-r--r--   0        0        0     5766 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/http.py
--rw-r--r--   0        0        0     2419 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3453 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/notify.py
--rw-r--r--   0        0        0      870 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/rng.py
--rw-r--r--   0        0        0      337 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/rpc.py
--rw-r--r--   0        0        0      455 2024-02-16 07:31:38.571934 chainbench-0.6.5/chainbench/util/timer.py
--rw-r--r--   0        0        0      948 2024-02-16 07:31:38.571934 chainbench-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    12756 1970-01-01 00:00:00.000000 chainbench-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 05:42:16.689645 chainbench-0.6.6/LICENSE
+-rw-r--r--   0        0        0    12165 2024-04-09 05:42:16.689645 chainbench-0.6.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/__main__.py
+-rw-r--r--   0        0        0    15103 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3732 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2760 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     1158 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/ethereum/consensus.py
+-rw-r--r--   0        0        0     2776 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      344 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/all.py
+-rw-r--r--   0        0        0     1272 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/debug_trace.py
+-rw-r--r--   0        0        0      427 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4252 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1655 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1931 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2897 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0     3514 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0     2223 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/profile/starknet/wallet.py
+-rw-r--r--   0        0        0      599 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6482 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/blockchain.py
+-rw-r--r--   0        0        0     5934 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/ethereum.py
+-rw-r--r--   0        0        0    12501 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     5443 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0     2284 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/test_data/starknet.py
+-rw-r--r--   0        0        0       24 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/__init__.py
+-rw-r--r--   0        0        0      977 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/clients.json
+-rw-r--r--   0        0        0    55080 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/methods.json
+-rw-r--r--   0        0        0     5499 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/tools/discovery/rpc.py
+-rw-r--r--   0        0        0      416 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     2895 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/ethereum.py
+-rw-r--r--   0        0        0     4622 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/evm.py
+-rw-r--r--   0        0        0     4672 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/http.py
+-rw-r--r--   0        0        0      799 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/common.py
+-rw-r--r--   0        0        0     9082 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/ethereum.py
+-rw-r--r--   0        0        0    10003 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/methods/evm.py
+-rw-r--r--   0        0        0     2885 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/solana.py
+-rw-r--r--   0        0        0     3680 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/user/starknet.py
+-rw-r--r--   0        0        0        0 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     6218 2024-04-09 05:42:16.689645 chainbench-0.6.6/chainbench/util/cli.py
+-rw-r--r--   0        0        0    12953 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/event.py
+-rw-r--r--   0        0        0     5766 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/http.py
+-rw-r--r--   0        0        0     2419 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3453 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/notify.py
+-rw-r--r--   0        0        0      870 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/rng.py
+-rw-r--r--   0        0        0      337 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      455 2024-04-09 05:42:16.693645 chainbench-0.6.6/chainbench/util/timer.py
+-rw-r--r--   0        0        0      953 2024-04-09 05:42:16.693645 chainbench-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    12756 1970-01-01 00:00:00.000000 chainbench-0.6.6/PKG-INFO
```

### Comparing `chainbench-0.6.5/LICENSE` & `chainbench-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/README.md` & `chainbench-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/main.py` & `chainbench-0.6.6/chainbench/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,17 @@
         sys.exit(1)
 
     custom_exclude_tags: list[str] = []
     if exclude_tags:
         for tag in exclude_tags:
             custom_exclude_tags.append(tag)
 
+    if not debug_trace_methods:
+        custom_exclude_tags = custom_exclude_tags + ["trace", "debug"]
+
     locust_options = LocustOptions(
         profile_path=profile_path,
         host=host,
         port=port,
         test_time=test_time,
         users=users,
         spawn_rate=spawn_rate,
```

### Comparing `chainbench-0.6.5/chainbench/profile/avalanche/general.py` & `chainbench-0.6.6/chainbench/profile/avalanche/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "eth_getTransactionReceipt" : 17
     "eth_chainId" : 15
     "eth_blockNumber" : 15
     "eth_getBalance" : 11
     "Others" : 28
 ```
 """
+
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
 class AvalancheProfile(EvmUser):
```

### Comparing `chainbench-0.6.5/chainbench/profile/bsc/general.py` & `chainbench-0.6.6/chainbench/profile/bsc/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "eth_getLogs" : 36
     "eth_blockNumber" : 28
     "eth_chainId" : 18
     "eth_getBlockByNumber" : 13
     "Others" : 20
 ```
 """
+
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
 class BscProfile(EvmUser):
```

### Comparing `chainbench-0.6.5/chainbench/profile/ethereum/consensus.py` & `chainbench-0.6.6/chainbench/profile/ethereum/consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Ethereum Beacon profile.
 """
+
 from locust import constant_pacing
 
 from chainbench.user.methods.ethereum import EthBeaconMethods
 
 # mypy: ignore_errors
```

### Comparing `chainbench-0.6.5/chainbench/profile/ethereum/general.py` & `chainbench-0.6.6/chainbench/profile/ethereum/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "eth_getBalance" : 12
     "eth_chainId" : 11
     "eth_getBlockByNumber" : 9
     "eth_getTransactionByHash" : 8
     "Others" : 12
 ```
 """
+
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
 class EthereumProfile(EvmUser):
@@ -81,14 +82,15 @@
 
     @tag("debug")
     @task(3)
     def trace_transaction_task(self):
         self.make_rpc_call(
             name="trace_transaction",
             method="debug_traceTransaction",
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(2)
     def client_version_task(self):
         self.make_rpc_call(
             name="client_version",
             method="web3_clientVersion",
```

### Comparing `chainbench-0.6.5/chainbench/profile/evm/debug_trace.py` & `chainbench-0.6.6/chainbench/profile/evm/debug_trace.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/profile/evm/heavy.py` & `chainbench-0.6.6/chainbench/profile/evm/heavy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 EVM profile (heavy mode).
 """
+
 from random import randint
 
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
```

### Comparing `chainbench-0.6.5/chainbench/profile/evm/light.py` & `chainbench-0.6.6/chainbench/profile/evm/light.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 EVM profile (light mode).
 """
+
 from locust import constant_pacing, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
 class EvmLightProfile(EvmUser):
```

### Comparing `chainbench-0.6.5/chainbench/profile/oasis/general.py` & `chainbench-0.6.6/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/profile/polygon/general.py` & `chainbench-0.6.6/chainbench/profile/polygon/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "eth_getBlockByNumber" : 17
     "eth_blockNumber" : 16
     "eth_getTransactionByHash" : 11
     "eth_getLogs" : 11
     "Others" : 9
 ```
 """
+
 from locust import constant_pacing, tag, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
 
 class PolygonGeneral(EvmUser):
```

### Comparing `chainbench-0.6.5/chainbench/profile/solana/general.py` & `chainbench-0.6.6/chainbench/profile/solana/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "getTransaction" : 7
     "getSignaturesForAddress" : 4
     "getLatestBlockhash" : 4
     "getBalance" : 4
     "Others" : 3
 ```
 """
+
 from locust import constant_pacing, tag, task
 
 from chainbench.user import SolanaUser
 from chainbench.util.rng import get_rng
 
 
 class SolanaProfile(SolanaUser):
```

### Comparing `chainbench-0.6.5/chainbench/profile/starknet/wallet.py` & `chainbench-0.6.6/chainbench/profile/starknet/wallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "starknet_call" : 54
     "starket_chainId" : 25
     "starknet_getClassHashAt" : 17
     "starknet_getTransactionReceipt" : 3
     "Others" : 1
 ```
 """
+
 from locust import constant_pacing, task
 
 from chainbench.user import StarkNetUser
 from chainbench.util.rng import get_rng
 
 
 class StarkNetWalletProfile(StarkNetUser):
```

### Comparing `chainbench-0.6.5/chainbench/test_data/__init__.py` & `chainbench-0.6.6/chainbench/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/test_data/blockchain.py` & `chainbench-0.6.6/chainbench/test_data/blockchain.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/test_data/ethereum.py` & `chainbench-0.6.6/chainbench/test_data/ethereum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import typing as t
 from argparse import Namespace
 from dataclasses import dataclass
 
-from tenacity import retry, stop_after_attempt
+from tenacity import retry, stop_after_attempt, wait_fixed
 
 from chainbench.test_data.blockchain import (
     Block,
     BlockNotFoundError,
     BlockNumber,
     BlockRange,
     TestData,
@@ -116,27 +116,24 @@
         if isinstance(block_id, str):
             if (block_id := block_id.lower()) not in (
                 "head",
                 "genesis",
                 "finalized",
             ):
                 raise ValueError("Invalid block identifier")
-        try:
-            slot = int(self.fetch_block_header(block_id)["slot"])
+        slot = int(self.fetch_block_header(block_id)["slot"])
 
-            committees_response = self.client.get(f"/eth/v1/beacon/states/{block_id}/committees", params={"slot": slot})
-            return EthBeaconBlock.from_response(slot, committees_response.json)
-        except BlockNotFoundError:
-            return self.fetch_latest_block()
+        committees_response = self.client.get(f"/eth/v1/beacon/states/{block_id}/committees", params={"slot": slot})
+        return EthBeaconBlock.from_response(slot, committees_response.json)
 
-    @retry(reraise=True, stop=stop_after_attempt(5))
+    @retry(reraise=True, stop=stop_after_attempt(20), wait=wait_fixed(1))
     def fetch_latest_block(self) -> EthBeaconBlock:
         return self.fetch_block("head")
 
-    @retry(reraise=True, stop=stop_after_attempt(5))
+    @retry(reraise=True, stop=stop_after_attempt(20), wait=wait_fixed(1))
     def fetch_latest_block_number(self) -> BlockNumber:
         return int(self.fetch_block_header("head")["slot"])
 
     def _get_start_and_end_blocks(self, parsed_options: Namespace) -> BlockRange:
         end_block_number = self.fetch_latest_block_number()
         if parsed_options.use_latest_blocks:
             start_block_number = end_block_number - self.data.size.blocks_len + 1
```

### Comparing `chainbench-0.6.5/chainbench/test_data/evm.py` & `chainbench-0.6.6/chainbench/test_data/evm.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,30 @@
                 "0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599",
                 "0x95aD61b0a150d79219dCF64E1E6Cc01f0B64C4cE",
                 "0x7D1AfA7B718fb893dB30A3aBc0Cfc608AaCfeBB0",
                 "0x6B175474E89094C44Da98b954EedeAC495271d0F",
                 "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984",
             ],
         },
+        11155111: {
+            "name": "ethereum-sepolia-testnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x7451ee8EeCf3b8534FA07B15b4B5ceE4bCc88778",
+                "0x3593B75e2a849DFDACb7e1ADdA24cB836670532b",
+                "0xFd57b4ddBf88a4e07fF4e34C487b99af2Fe82a05",
+                "0x397a59aA02eB65702E5DAdDd5967bbe1979F9aC3",
+                "0x466D489b6d36E7E3b824ef491C225F5830E81cC1",
+                "0x26fb2eee2F48d6EB3111e5aF0b3F11E6694296a8",
+                "0xc132ec2e4B6130273AE6C6eD0a1B8bEE2C3815a0",
+                "0x1c7D4B196Cb0C7B01d743Fbc6116a902379C7238",
+                "0x4c16D8C078eF6B56700C1BE19a336915962df072",
+                "0x097D90c9d3E0B50Ca60e1ae45F6A81010f9FB534",
+            ],
+        },
         56: {
             "name": "bsc-mainnet",
             "start_block": 20000000,
             "contract_addresses": [
                 "0x2170Ed0880ac9A755fd29B2688956BD959F933F8",
                 "0x55d398326f99059fF775485246999027B3197955",
                 "0xbb4CdB9CBd36B01bD1cBaEBF2De08d9173bc095c",
```

### Comparing `chainbench-0.6.5/chainbench/test_data/solana.py` & `chainbench-0.6.6/chainbench/test_data/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/test_data/starknet.py` & `chainbench-0.6.6/chainbench/test_data/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/tools/discovery/clients.json` & `chainbench-0.6.6/chainbench/tools/discovery/clients.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/tools/discovery/methods.json` & `chainbench-0.6.6/chainbench/tools/discovery/methods.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/tools/discovery/rpc.py` & `chainbench-0.6.6/chainbench/tools/discovery/rpc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/user/ethereum.py` & `chainbench-0.6.6/chainbench/user/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/user/evm.py` & `chainbench-0.6.6/chainbench/user/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/user/http.py` & `chainbench-0.6.6/chainbench/user/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         if response.status_code != 200:
             self.logger.info(f"Request failed with {response.status_code} code")
             self.logger.debug(
                 f"Request to {response.url} failed with HTTP Error {response.status_code} code: {response.text}"
             )
             self.check_fatal(response)
             response.failure(f"Request failed with {response.status_code} code")
+            response.raise_for_status()
 
     def post(
         self, name: str, data: t.Optional[dict] = None, params: t.Optional[dict] = None, path: str = ""
     ) -> ResponseContextManager:
         with self.client.request("POST", path, json=data, params=params, name=name, catch_response=True) as response:
             self.check_http_error(response)
             return response
```

### Comparing `chainbench-0.6.5/chainbench/user/methods/__init__.py` & `chainbench-0.6.6/chainbench/user/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/user/methods/common.py` & `chainbench-0.6.6/chainbench/user/methods/common.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/user/methods/ethereum.py` & `chainbench-0.6.6/chainbench/user/methods/ethereum.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             name="eth_v1_beacon_states_validators_random_ids",
             state_id=block.block_number,
             validator_ids=block.get_random_validator_indexes(validator_count, self.rng.get_rng()),
         )
 
     def eth_v1_beacon_states_random_state_id_finality_checkpoints_task(self):
         self.get(
-            name="eth_v1_beacon_states_finality_checkpoints",
+            name="eth_v1_beacon_random_states_finality_checkpoints",
             path=f"/eth/v1/beacon/states/"
             f"{self.test_data.get_random_block(self.rng.get_rng()).block_number}/finality_checkpoints",
         )
 
     def eth_v1_validator_duties_proposer_random_epoch_task(self):
         self.get(
             name="eth_v1_validator_duties_proposer_random_epoch",
```

### Comparing `chainbench-0.6.5/chainbench/user/methods/evm.py` & `chainbench-0.6.6/chainbench/user/methods/evm.py`

 * *Files 14% similar despite different names*

```diff
@@ -177,14 +177,55 @@
         )
 
     def eth_syncing_task(self) -> None:
         self.make_rpc_call(
             method="eth_syncing",
         )
 
+    def debug_get_bad_blocks_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_getBadBlocks",
+        )
+
+    def debug_get_raw_block_by_number_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_getRawBlock",
+            params=[hex(self.test_data.get_random_block_number(self.rng.get_rng()))],
+        )
+
+    def debug_get_raw_header_by_number_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_getRawHeader",
+            params=[hex(self.test_data.get_random_block_number(self.rng.get_rng()))],
+        )
+
+    def debug_get_raw_receipts_by_number_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_getRawReceipts",
+            params=[hex(self.test_data.get_random_block_number(self.rng.get_rng()))],
+        )
+
+    def debug_get_raw_transaction_by_hash_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_getRawTransaction",
+            params=[self.test_data.get_random_tx_hash(self.rng.get_rng())],
+        )
+
+    def debug_trace_bad_block_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_traceBadBlock",
+            params=[self.test_data.get_random_block_hash(self.rng.get_rng())],
+        )
+
+    def debug_trace_block_task(self) -> None:
+        self.make_rpc_call(
+            method="debug_traceBlock",
+            params=self._block_params_factory(),
+        )
+
     def debug_trace_block_by_hash_task(self) -> None:
         self.make_rpc_call(
             method="debug_traceBlockByHash",
             params=self._debug_trace_block_by_hash_params_factory(self.rng.get_rng()),
         )
 
     def debug_trace_block_by_number_task(self) -> None:
```

### Comparing `chainbench-0.6.5/chainbench/user/solana.py` & `chainbench-0.6.6/chainbench/user/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/user/starknet.py` & `chainbench-0.6.6/chainbench/user/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/util/cli.py` & `chainbench-0.6.6/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/util/event.py` & `chainbench-0.6.6/chainbench/util/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                     continue
                 if (
                     latest_block_number not in user.test_data.data.block_numbers
                     and latest_block_number not in invalid_blocks
                 ):
                     try:
                         block = user.test_data.fetch_block(latest_block_number)
-                    except InvalidBlockError:
+                    except (InvalidBlockError, BlockNotFoundError):
                         invalid_blocks.append(latest_block_number)
                         continue
                     user.test_data.data.push_block(block)
                     blocks[test_data_class_name] = block.to_json()
                     print(f"Block {block.block_number} fetched and updated in test data")
         if len(blocks) > 0:
             send_msg_to_workers(master_runner, "block_data", blocks)
```

### Comparing `chainbench-0.6.5/chainbench/util/http.py` & `chainbench-0.6.6/chainbench/util/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/util/monitor.py` & `chainbench-0.6.6/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/util/notify.py` & `chainbench-0.6.6/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/chainbench/util/rng.py` & `chainbench-0.6.6/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.5/pyproject.toml` & `chainbench-0.6.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.6.5"
+version = "0.6.6"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
 packages = [{include = "chainbench"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-locust = "^2.22.0"
+locust = "^2.24.1"
 click = "^8.1.6"
-locust-plugins = {extras = ["dashboards"], version = "^4.3.4"}
+locust-plugins = {extras = ["dashboards"], version = "^4.4.2"}
 tenacity = "^8.2.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = ">=23.1,<25.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 flake8-pyproject = "^1.2.3"
 
 [tool.poetry.scripts]
```

### Comparing `chainbench-0.6.5/PKG-INFO` & `chainbench-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.6.5
+Version: 0.6.6
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.6,<9.0.0)
-Requires-Dist: locust (>=2.22.0,<3.0.0)
-Requires-Dist: locust-plugins[dashboards] (>=4.3.4,<5.0.0)
+Requires-Dist: locust (>=2.24.1,<3.0.0)
+Requires-Dist: locust-plugins[dashboards] (>=4.4.2,<5.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
  <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
```

