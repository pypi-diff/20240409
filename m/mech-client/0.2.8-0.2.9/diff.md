# Comparing `tmp/mech_client-0.2.8.tar.gz` & `tmp/mech_client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.2.8.tar", max compression
+gzip compressed data, was "mech_client-0.2.9.tar", max compression
```

## Comparing `mech_client-0.2.8.tar` & `mech_client-0.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11339 2023-11-30 12:19:05.090563 mech_client-0.2.8/LICENSE
--rw-r--r--   0        0        0     4049 2023-11-30 12:19:05.090563 mech_client-0.2.8/README.md
--rw-r--r--   0        0        0       42 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/__init__.py
--rw-r--r--   0        0        0     5790 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/acn.py
--rw-r--r--   0        0        0     3359 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/cli.py
--rw-r--r--   0        0        0     1028 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/helpers/__init__.py
--rw-r--r--   0        0        0     1641 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/README.md
--rw-r--r--   0        0        0     1141 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/__init__.py
--rw-r--r--   0        0        0     1543 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/acn.proto
--rw-r--r--   0        0        0     4350 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/acn_pb2.py
--rw-r--r--   0        0        0     7982 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/custom_types.py
--rw-r--r--   0        0        0     4443 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/dialogues.py
--rw-r--r--   0        0        0    10272 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/message.py
--rw-r--r--   0        0        0     1233 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/protocol.yaml
--rw-r--r--   0        0        0     6592 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/serialization.py
--rw-r--r--   0        0        0      847 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/tests/__init__.py
--rw-r--r--   0        0        0     8965 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/tests/test_acn.py
--rw-r--r--   0        0        0     1964 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/tests/test_acn_dialogues.py
--rw-r--r--   0        0        0     4332 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/acn/tests/test_acn_messages.py
--rw-r--r--   0        0        0      577 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/README.md
--rw-r--r--   0        0        0     1219 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/__init__.py
--rw-r--r--   0        0        0      271 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/acn_data_share.proto
--rw-r--r--   0        0        0     1475 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
--rw-r--r--   0        0        0     4078 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/dialogues.py
--rw-r--r--   0        0        0     7742 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/message.py
--rw-r--r--   0        0        0     1052 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/protocol.yaml
--rw-r--r--   0        0        0     4617 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/serialization.py
--rw-r--r--   0        0        0     1835 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
--rw-r--r--   0        0        0     2021 2023-11-30 12:19:47.718271 mech_client-0.2.8/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
--rw-r--r--   0        0        0      631 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/README.md
--rw-r--r--   0        0        0      879 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/__init__.py
--rw-r--r--   0        0        0    27887 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/connection.py
--rw-r--r--   0        0        0     1763 2023-11-30 12:19:47.714271 mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/connection.yaml
--rw-r--r--   0        0        0    11558 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/interact.py
--rw-r--r--   0        0        0     2250 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     2059 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0     1815 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/subgraph.py
--rw-r--r--   0        0        0     2581 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/to_png.py
--rw-r--r--   0        0        0     6826 2023-11-30 12:19:05.090563 mech_client-0.2.8/mech_client/wss.py
--rw-r--r--   0        0        0     1477 2023-11-30 12:19:05.090563 mech_client-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-12-06 13:50:26.778873 mech_client-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4049 2023-12-06 13:50:26.778873 mech_client-0.2.9/README.md
+-rw-r--r--   0        0        0       42 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/__init__.py
+-rw-r--r--   0        0        0     5790 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/acn.py
+-rw-r--r--   0        0        0     3897 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/cli.py
+-rw-r--r--   0        0        0     1028 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/helpers/__init__.py
+-rw-r--r--   0        0        0     1641 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/README.md
+-rw-r--r--   0        0        0     1141 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/__init__.py
+-rw-r--r--   0        0        0     1543 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/acn.proto
+-rw-r--r--   0        0        0     4350 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/acn_pb2.py
+-rw-r--r--   0        0        0     7982 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/custom_types.py
+-rw-r--r--   0        0        0     4443 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/dialogues.py
+-rw-r--r--   0        0        0    10272 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/message.py
+-rw-r--r--   0        0        0     1233 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/protocol.yaml
+-rw-r--r--   0        0        0     6592 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/serialization.py
+-rw-r--r--   0        0        0      847 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/tests/__init__.py
+-rw-r--r--   0        0        0     8965 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/tests/test_acn.py
+-rw-r--r--   0        0        0     1964 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/tests/test_acn_dialogues.py
+-rw-r--r--   0        0        0     4332 2023-12-06 13:51:12.079260 mech_client-0.2.9/mech_client/helpers/acn/tests/test_acn_messages.py
+-rw-r--r--   0        0        0      577 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/README.md
+-rw-r--r--   0        0        0     1219 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/__init__.py
+-rw-r--r--   0        0        0      271 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/acn_data_share.proto
+-rw-r--r--   0        0        0     1475 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
+-rw-r--r--   0        0        0     4078 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/dialogues.py
+-rw-r--r--   0        0        0     7742 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/message.py
+-rw-r--r--   0        0        0     1052 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/protocol.yaml
+-rw-r--r--   0        0        0     4617 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/serialization.py
+-rw-r--r--   0        0        0     1835 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
+-rw-r--r--   0        0        0     2021 2023-12-06 13:51:12.083260 mech_client-0.2.9/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
+-rw-r--r--   0        0        0      631 2023-12-06 13:51:12.075260 mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/README.md
+-rw-r--r--   0        0        0      879 2023-12-06 13:51:12.075260 mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/__init__.py
+-rw-r--r--   0        0        0    27887 2023-12-06 13:51:12.075260 mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/connection.py
+-rw-r--r--   0        0        0     1763 2023-12-06 13:51:12.075260 mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/connection.yaml
+-rw-r--r--   0        0        0    14791 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/interact.py
+-rw-r--r--   0        0        0     2250 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     2059 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0     1815 2023-12-06 13:50:26.778873 mech_client-0.2.9/mech_client/subgraph.py
+-rw-r--r--   0        0        0     2581 2023-12-06 13:50:26.782873 mech_client-0.2.9/mech_client/to_png.py
+-rw-r--r--   0        0        0     7353 2023-12-06 13:50:26.782873 mech_client-0.2.9/mech_client/wss.py
+-rw-r--r--   0        0        0     1475 2023-12-06 13:50:26.782873 mech_client-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.9/PKG-INFO
```

### Comparing `mech_client-0.2.8/LICENSE` & `mech_client-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/README.md` & `mech_client-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/acn.py` & `mech_client-0.2.9/mech_client/acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/cli.py` & `mech_client-0.2.9/mech_client/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,33 +53,54 @@
 @click.option(
     "--confirm",
     type=click.Choice(
         choices=(ConfirmationType.OFF_CHAIN.value, ConfirmationType.ON_CHAIN.value)
     ),
     help="Data verification method (on-chain/off-chain)",
 )
-def interact(
+@click.option(
+    "--retries",
+    type=int,
+    help="Number of retries for sending a transaction",
+)
+@click.option(
+    "--timeout",
+    type=float,
+    help="Timeout to wait for the transaction",
+)
+@click.option(
+    "--sleep",
+    type=float,
+    help="Amount of sleep before retrying the transaction",
+)
+def interact(  # pylint: disable=too-many-arguments
     prompt: str,
     agent_id: int,
     tool: Optional[str],
     key: Optional[str],
     confirm: Optional[str] = None,
+    retries: Optional[int] = None,
+    timeout: Optional[float] = None,
+    sleep: Optional[float] = None,
 ) -> None:
     """Interact with a mech specifying a prompt and tool."""
     try:
         interact_(
             prompt=prompt,
             agent_id=agent_id,
             private_key_path=key,
             tool=tool,
             confirmation_type=(
                 ConfirmationType(confirm)
                 if confirm is not None
                 else ConfirmationType.WAIT_FOR_BOTH
             ),
+            retries=retries,
+            timeout=timeout,
+            sleep=sleep,
         )
     except (ValueError, FileNotFoundError) as e:
         raise click.ClickException(str(e)) from e
 
 
 @click.command()
 @click.argument("prompt")
```

### Comparing `mech_client-0.2.8/mech_client/helpers/__init__.py` & `mech_client-0.2.9/mech_client/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/README.md` & `mech_client-0.2.9/mech_client/helpers/acn/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/__init__.py` & `mech_client-0.2.9/mech_client/helpers/acn/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/acn.proto` & `mech_client-0.2.9/mech_client/helpers/acn/acn.proto`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/acn_pb2.py` & `mech_client-0.2.9/mech_client/helpers/acn/acn_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/custom_types.py` & `mech_client-0.2.9/mech_client/helpers/acn/custom_types.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/dialogues.py` & `mech_client-0.2.9/mech_client/helpers/acn/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/message.py` & `mech_client-0.2.9/mech_client/helpers/acn/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/protocol.yaml` & `mech_client-0.2.9/mech_client/helpers/acn/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/serialization.py` & `mech_client-0.2.9/mech_client/helpers/acn/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/tests/__init__.py` & `mech_client-0.2.9/mech_client/helpers/acn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/tests/test_acn.py` & `mech_client-0.2.9/mech_client/helpers/acn/tests/test_acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/tests/test_acn_dialogues.py` & `mech_client-0.2.9/mech_client/helpers/acn/tests/test_acn_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn/tests/test_acn_messages.py` & `mech_client-0.2.9/mech_client/helpers/acn/tests/test_acn_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/README.md` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/__init__.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/acn_data_share_pb2.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/acn_data_share_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/dialogues.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/message.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/protocol.yaml` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/serialization.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py` & `mech_client-0.2.9/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/README.md` & `mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/__init__.py` & `mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/connection.py` & `mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/connection.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/helpers/p2p_libp2p_client/connection.yaml` & `mech_client-0.2.9/mech_client/helpers/p2p_libp2p_client/connection.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/interact.py` & `mech_client-0.2.9/mech_client/interact.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,23 +24,26 @@
 
 python client.py <prompt> <tool>
 """
 
 import asyncio
 import json
 import os
+import time
 import warnings
+from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Any, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 import websocket
 from aea.crypto.base import Crypto
 from aea_ledger_ethereum import EthereumApi, EthereumCrypto
+from web3 import Web3
 from web3.contract import Contract as Web3Contract
 
 from mech_client.acn import (
     watch_for_data_url_from_mech,
     watch_for_data_url_from_mech_sync,
 )
 from mech_client.prompt_to_ipfs import push_metadata_to_ipfs
@@ -59,49 +62,88 @@
     "https://rpc.eu-central-2.gateway.fm/v4/gnosis/non-archival/mainnet",
 )
 LEDGER_CONFIG = {
     "address": MECHX_CHAIN_RPC,
     "chain_id": 100,
     "poa_chain": False,
     "default_gas_price_strategy": "eip1559",
+    "is_gas_estimation_enabled": True,
 }
 PRIVATE_KEY_FILE_PATH = "ethereum_private_key.txt"
 
 WSS_ENDPOINT = os.getenv(
     "WEBSOCKET_ENDPOINT",
     "wss://rpc.eu-central-2.gateway.fm/ws/v4/gnosis/non-archival/mainnet",
 )
 GNOSISSCAN_API_URL = "https://api.gnosisscan.io/api?module=contract&action=getabi&address={contract_address}"
 
+MAX_RETRIES = 3
+WAIT_SLEEP = 3.0
+TIMEOUT = 60.0
+
 # Ignore a specific warning message
 warnings.filterwarnings("ignore", "The log with transaction hash.*")
 
 
 class ConfirmationType(Enum):
     """Verification type."""
 
     ON_CHAIN = "on-chain"
     OFF_CHAIN = "off-chain"
     WAIT_FOR_BOTH = "wait-for-both"
 
 
-def get_contract(contract_address: str, ledger_api: EthereumApi) -> Web3Contract:
+def calculate_topic_id(event: Dict) -> str:
+    """Caclulate topic ID"""
+    text = event["name"]
+    text += "("
+    for inp in event["inputs"]:
+        text += inp["type"]
+        text += ","
+    text = text[:-1]
+    text += ")"
+    return Web3.keccak(text=text).hex()
+
+
+def get_event_signatures(abi: List) -> Tuple[str, str]:
+    """Calculate `Request` and `Deliver` event topics"""
+    request, deliver = "", ""
+    for obj in abi:
+        if obj["type"] != "event":
+            continue
+        if obj["name"] == "Deliver":
+            deliver = calculate_topic_id(event=obj)
+        if obj["name"] == "Request":
+            request = calculate_topic_id(event=obj)
+    return request, deliver
+
+
+def get_abi(contract_address: str) -> List:
+    """Get contract abi"""
+    abi_request_url = GNOSISSCAN_API_URL.format(contract_address=contract_address)
+    response = requests.get(abi_request_url).json()
+    return json.loads(response["result"])
+
+
+def get_contract(
+    contract_address: str, abi: List, ledger_api: EthereumApi
+) -> Web3Contract:
     """
     Returns a contract instance.
 
     :param contract_address: The address of the contract.
     :type contract_address: str
+    :param abi: ABI Object
+    :type abi: List
     :param ledger_api: The Ethereum API used for interacting with the ledger.
     :type ledger_api: EthereumApi
     :return: The contract instance.
     :rtype: Web3Contract
     """
-    abi_request_url = GNOSISSCAN_API_URL.format(contract_address=contract_address)
-    response = requests.get(abi_request_url).json()
-    abi = json.loads(response["result"])
+
     return ledger_api.get_contract_instance(
         {"abi": abi, "bytecode": "0x"}, contract_address
     )
 
 
 def _tool_selector_prompt(available_tools: List[str]) -> str:
     """
@@ -168,28 +210,33 @@
         return tool
     return _tool_selector_prompt(available_tools=available_tools)
 
 
 def fetch_tools(agent_id: int, ledger_api: EthereumApi) -> List[str]:
     """Fetch tools for specified agent ID."""
     mech_registry = get_contract(
-        contract_address=AGENT_REGISTRY_CONTRACT, ledger_api=ledger_api
+        contract_address=AGENT_REGISTRY_CONTRACT,
+        abi=get_abi(AGENT_REGISTRY_CONTRACT),
+        ledger_api=ledger_api,
     )
     token_uri = mech_registry.functions.tokenURI(agent_id).call()
     response = requests.get(token_uri).json()
     return response["tools"]
 
 
-def send_request(  # pylint: disable=too-many-arguments
+def send_request(  # pylint: disable=too-many-arguments,too-many-locals
     crypto: EthereumCrypto,
     ledger_api: EthereumApi,
     mech_contract: Web3Contract,
     prompt: str,
     tool: str,
     price: int = 10_000_000_000_000_000,
+    retries: Optional[int] = None,
+    timeout: Optional[float] = None,
+    sleep: Optional[float] = None,
 ) -> None:
     """
     Sends a request to the mech.
 
     :param crypto: The Ethereum crypto object.
     :type crypto: EthereumCrypto
     :param ledger_api: The Ethereum API used for interacting with the ledger.
@@ -198,62 +245,91 @@
     :type mech_contract: Web3Contract
     :param prompt: The request prompt.
     :type prompt: str
     :param tool: The requested tool.
     :type tool: str
     :param price: The price for the request (default: 10_000_000_000_000_000).
     :type price: int
+    :param retries: Number of retries for sending a transaction
+    :type retries: int
+    :param timeout: Timeout to wait for the transaction
+    :type timeout: float
+    :param sleep: Amount of sleep before retrying the transaction
+    :type sleep: float
     """
     v1_file_hash_hex_truncated, v1_file_hash_hex = push_metadata_to_ipfs(prompt, tool)
     print(f"Prompt uploaded: https://gateway.autonolas.tech/ipfs/{v1_file_hash_hex}")
     method_name = "request"
     methord_args = {"data": v1_file_hash_hex_truncated}
     tx_args = {"sender_address": crypto.address, "value": price}
-    raw_transaction = ledger_api.build_transaction(
-        contract_instance=mech_contract,
-        method_name=method_name,
-        method_args=methord_args,
-        tx_args=tx_args,
-    )
-    raw_transaction["gas"] = 50_000
-    signed_transaction = crypto.sign_transaction(raw_transaction)
-    transaction_digest = ledger_api.send_signed_transaction(signed_transaction)
-    print(f"Transaction sent: https://gnosisscan.io/tx/{transaction_digest}")
+
+    tries = 0
+    retries = retries or MAX_RETRIES
+    timeout = timeout or TIMEOUT
+    sleep = sleep or WAIT_SLEEP
+    deadline = datetime.now().timestamp() + timeout
+
+    while tries < retries and datetime.now().timestamp() < deadline:
+        tries += 1
+        try:
+            raw_transaction = ledger_api.build_transaction(
+                contract_instance=mech_contract,
+                method_name=method_name,
+                method_args=methord_args,
+                tx_args=tx_args,
+                raise_on_try=True,
+            )
+            signed_transaction = crypto.sign_transaction(raw_transaction)
+            transaction_digest = ledger_api.send_signed_transaction(
+                signed_transaction,
+                raise_on_try=True,
+            )
+            print(f"Transaction sent: https://gnosisscan.io/tx/{transaction_digest}")
+            return
+        except Exception as e:  # pylint: disable=broad-except
+            print(
+                f"Error occured while sending the transaction: {e}; Retrying in {sleep}"
+            )
+            time.sleep(sleep)
 
 
-def wait_for_data_url(
+def wait_for_data_url(  # pylint: disable=too-many-arguments
     request_id: str,
     wss: websocket.WebSocket,
     mech_contract: Web3Contract,
+    deliver_signature: str,
     ledger_api: EthereumApi,
     crypto: Crypto,
 ) -> Any:
     """
     Wait for data from on-chain/off-chain.
 
     :param request_id: The ID of the request.
     :type request_id: str
     :param wss: The WebSocket connection object.
     :type wss: websocket.WebSocket
     :param mech_contract: The mech contract instance.
     :type mech_contract: Web3Contract
+    :param deliver_signature: Topic signature for Deliver event
+    :type deliver_signature: str
     :param ledger_api: The Ethereum API used for interacting with the ledger.
     :type ledger_api: EthereumApi
     :param crypto: The cryptographic object.
     :type crypto: Crypto
     :return: The data received from on-chain/off-chain.
     :rtype: Any
     """
     loop = asyncio.new_event_loop()
     off_chain_task = loop.create_task(watch_for_data_url_from_mech(crypto=crypto))
     on_chain_task = loop.create_task(
         watch_for_data_url_from_wss(
             request_id=request_id,
             wss=wss,
             mech_contract=mech_contract,
+            deliver_signature=deliver_signature,
             ledger_api=ledger_api,
             loop=loop,
         )
     )
 
     async def _wait_for_tasks() -> Any:  # type: ignore
         """Wait for tasks to finish."""
@@ -265,20 +341,23 @@
         await asyncio.wait(unfinished)
         return finished.result()
 
     result = loop.run_until_complete(_wait_for_tasks())
     return result
 
 
-def interact(
+def interact(  # pylint: disable=too-many-arguments,too-many-locals
     prompt: str,
     agent_id: int,
     tool: Optional[str] = None,
     private_key_path: Optional[str] = None,
     confirmation_type: ConfirmationType = ConfirmationType.WAIT_FOR_BOTH,
+    retries: Optional[int] = None,
+    timeout: Optional[float] = None,
+    sleep: Optional[float] = None,
 ) -> Any:
     """
     Interact with agent mech contract.
 
     :param prompt: The interaction prompt.
     :type prompt: str
     :param agent_id: The ID of the agent.
@@ -286,14 +365,20 @@
     :param tool: The tool to interact with (optional).
     :type tool: Optional[str]
     :param private_key_path: The path to the private key file (optional).
     :type private_key_path: Optional[str]
     :param confirmation_type: The confirmation type for the interaction (default: ConfirmationType.WAIT_FOR_BOTH).
     :type confirmation_type: ConfirmationType
     :return: The data received from on-chain/off-chain.
+    :param retries: Number of retries for sending a transaction
+    :type retries: int
+    :param timeout: Timeout to wait for the transaction
+    :type timeout: float
+    :param sleep: Amount of sleep before retrying the transaction
+    :type sleep: float
     :rtype: Any
     """
     contract_address = query_agent_address(agent_id=agent_id)
     if contract_address is None:
         raise ValueError(f"Agent with ID {agent_id} does not exist!")
 
     private_key_path = private_key_path or PRIVATE_KEY_FILE_PATH
@@ -303,43 +388,59 @@
         )
 
     wss = websocket.create_connection(WSS_ENDPOINT)
     crypto = EthereumCrypto(private_key_path=private_key_path)
     ledger_api = EthereumApi(**LEDGER_CONFIG)
 
     tool = verify_or_retrieve_tool(agent_id=agent_id, ledger_api=ledger_api, tool=tool)
+    abi = get_abi(contract_address=contract_address)
     mech_contract = get_contract(
-        contract_address=contract_address, ledger_api=ledger_api
+        contract_address=contract_address, abi=abi, ledger_api=ledger_api
+    )
+    request_event_signature, deliver_event_signature = get_event_signatures(abi=abi)
+    register_event_handlers(
+        wss=wss,
+        contract_address=contract_address,
+        crypto=crypto,
+        request_signature=request_event_signature,
+        deliver_signature=deliver_event_signature,
     )
-    register_event_handlers(wss=wss, contract_address=contract_address, crypto=crypto)
     send_request(
         crypto=crypto,
         ledger_api=ledger_api,
         mech_contract=mech_contract,
         prompt=prompt,
         tool=tool,
+        retries=retries,
+        timeout=timeout,
+        sleep=sleep,
     )
     request_id = watch_for_request_id(
-        wss=wss, mech_contract=mech_contract, ledger_api=ledger_api
+        wss=wss,
+        mech_contract=mech_contract,
+        ledger_api=ledger_api,
+        request_signature=request_event_signature,
     )
     print(f"Created on-chain request with ID {request_id}")
     if confirmation_type == ConfirmationType.OFF_CHAIN:
         data_url = watch_for_data_url_from_mech_sync(crypto=crypto)
     elif confirmation_type == ConfirmationType.ON_CHAIN:
         data_url = watch_for_data_url_from_wss_sync(
             request_id=request_id,
             wss=wss,
+            deliver_signature=deliver_event_signature,
             mech_contract=mech_contract,
             ledger_api=ledger_api,
         )
     else:
         data_url = wait_for_data_url(
             request_id=request_id,
             wss=wss,
             mech_contract=mech_contract,
+            deliver_signature=deliver_event_signature,
             ledger_api=ledger_api,
             crypto=crypto,
         )
     print(f"Data arrived: {data_url}")
     data = requests.get(f"{data_url}/{request_id}").json()
     print(f"Data from agent: {data}")
     return data
```

### Comparing `mech_client-0.2.8/mech_client/prompt_to_ipfs.py` & `mech_client-0.2.9/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/push_to_ipfs.py` & `mech_client-0.2.9/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/subgraph.py` & `mech_client-0.2.9/mech_client/subgraph.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/to_png.py` & `mech_client-0.2.9/mech_client/to_png.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.8/mech_client/wss.py` & `mech_client-0.2.9/mech_client/wss.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,46 +27,46 @@
 
 import websocket
 from aea.crypto.base import Crypto
 from aea_ledger_ethereum import EthereumApi
 from web3.contract import Contract as Web3Contract
 
 
-EVENT_SIGNATURE_REQUEST = (
-    "0x4bda649efe6b98b0f9c1d5e859c29e20910f45c66dabfe6fad4a4881f7faf9cc"
-)
-EVENT_SIGNATURE_DELIVER = (
-    "0x3ec84da2cdc1ce60c063642b69ff2e65f3b69787a2b90443457ba274e51e7c72"
-)
-
-
 def register_event_handlers(
-    wss: websocket.WebSocket, contract_address: str, crypto: Crypto
+    wss: websocket.WebSocket,
+    contract_address: str,
+    crypto: Crypto,
+    request_signature: str,
+    deliver_signature: str,
 ) -> None:
     """
     Register event handlers.
 
     :param wss: The WebSocket connection object.
     :type wss: websocket.WebSocket
     :param contract_address: The address of the contract.
     :type contract_address: str
     :param crypto: The cryptographic object.
     :type crypto: Crypto
+    :param request_signature: Topic signature for Request event
+    :type request_signature: str
+    :param deliver_signature: Topic signature for Deliver event
+    :type deliver_signature: str
     """
 
     subscription_request = {
         "jsonrpc": "2.0",
         "id": 1,
         "method": "eth_subscribe",
         "params": [
             "logs",
             {
                 "address": contract_address,
                 "topics": [
-                    EVENT_SIGNATURE_REQUEST,
+                    request_signature,
                     ["0x" + "0" * 24 + crypto.address[2:]],
                 ],
             },
         ],
     }
     content = bytes(json.dumps(subscription_request), "utf-8")
     wss.send(content)
@@ -75,15 +75,15 @@
     _ = wss.recv()
     subscription_deliver = {
         "jsonrpc": "2.0",
         "id": 1,
         "method": "eth_subscribe",
         "params": [
             "logs",
-            {"address": contract_address, "topics": [EVENT_SIGNATURE_DELIVER]},
+            {"address": contract_address, "topics": [deliver_signature]},
         ],
     }
     content = bytes(json.dumps(subscription_deliver), "utf-8")
     wss.send(content)
 
     # registration confirmation
     _ = wss.recv()
@@ -105,61 +105,67 @@
             return ledger_api._api.eth.get_transaction_receipt(  # pylint: disable=protected-access
                 tx_hash
             )
         except Exception:  # pylint: disable=broad-except
             time.sleep(1)
 
 
-def watch_for_request_id(
+def watch_for_request_id(  # pylint: disable=too-many-arguments
     wss: websocket.WebSocket,
     mech_contract: Web3Contract,
     ledger_api: EthereumApi,
+    request_signature: str,
 ) -> str:
     """
     Watches for events on mech.
 
     :param wss: The WebSocket connection object.
     :type wss: websocket.WebSocket
     :param mech_contract: The mech contract instance.
     :type mech_contract: Web3Contract
     :param ledger_api: The Ethereum API used for interacting with the ledger.
     :type ledger_api: EthereumApi
     :return: The requested ID.
+    :param request_signature: Topic signature for Request event
+    :type request_signature: str
     :rtype: str
     """
     while True:
         msg = wss.recv()
         data = json.loads(msg)
         tx_hash = data["params"]["result"]["transactionHash"]
         tx_receipt = wait_for_receipt(tx_hash=tx_hash, ledger_api=ledger_api)
         event_signature = tx_receipt["logs"][0]["topics"][0].hex()
-        if event_signature != EVENT_SIGNATURE_REQUEST:
+        if event_signature != request_signature:
             continue
 
         rich_logs = mech_contract.events.Request().process_receipt(tx_receipt)
         request_id = str(rich_logs[0]["args"]["requestId"])
         return request_id
 
 
-async def watch_for_data_url_from_wss(
+async def watch_for_data_url_from_wss(  # pylint: disable=too-many-arguments
     request_id: str,
     wss: websocket.WebSocket,
     mech_contract: Web3Contract,
+    deliver_signature: str,
     ledger_api: EthereumApi,
     loop: asyncio.AbstractEventLoop,
 ) -> Any:
     """
     Watches for data on-chain.
 
     :param request_id: The ID of the request.
     :type request_id: str
     :param wss: The WebSocket connection object.
     :type wss: websocket.WebSocket
     :param mech_contract: The mech contract instance.
     :type mech_contract: Web3Contract
+    :param deliver_signature: Topic signature for Deliver event
+    :type deliver_signature: str
     :param ledger_api: The Ethereum API used for interacting with the ledger.
     :type ledger_api: EthereumApi
     :param loop: The event loop used for asynchronous operations.
     :type loop: asyncio.AbstractEventLoop
     :return: The data received from on-chain.
     :rtype: Any
     """
@@ -168,49 +174,53 @@
             msg = await loop.run_in_executor(executor=executor, func=wss.recv)
             data = json.loads(msg)
             tx_hash = data["params"]["result"]["transactionHash"]
             tx_receipt = await loop.run_in_executor(
                 executor, wait_for_receipt, tx_hash, ledger_api
             )
             event_signature = tx_receipt["logs"][0]["topics"][0].hex()
-            if event_signature != EVENT_SIGNATURE_DELIVER:
+            if event_signature != deliver_signature:
                 continue
 
             rich_logs = mech_contract.events.Deliver().process_receipt(tx_receipt)
             data = cast(bytes, rich_logs[0]["args"]["data"])
             if request_id != str(rich_logs[0]["args"]["requestId"]):
                 continue
             return f"https://gateway.autonolas.tech/ipfs/f01701220{data.hex()}"
 
 
 def watch_for_data_url_from_wss_sync(
     request_id: str,
     wss: websocket.WebSocket,
     mech_contract: Web3Contract,
+    deliver_signature: str,
     ledger_api: EthereumApi,
 ) -> Any:
     """
     Watches for data on-chain.
 
     :param request_id: The ID of the request.
     :type request_id: str
     :param wss: The WebSocket connection object.
     :type wss: websocket.WebSocket
     :param mech_contract: The mech contract instance.
     :type mech_contract: Web3Contract
+    :param deliver_signature: Topic signature for Deliver event
+    :type deliver_signature: str
     :param ledger_api: The Ethereum API used for interacting with the ledger.
     :type ledger_api: EthereumApi
     :return: The data received from on-chain.
     :rtype: Any
     """
     loop = asyncio.new_event_loop()
     task = loop.create_task(
         watch_for_data_url_from_wss(
             request_id=request_id,
             wss=wss,
             mech_contract=mech_contract,
+            deliver_signature=deliver_signature,
             ledger_api=ledger_api,
             loop=loop,
         )
     )
     loop.run_until_complete(task)
     return task.result()
```

### Comparing `mech_client-0.2.8/pyproject.toml` & `mech_client-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.2.8"
+version = "0.2.9"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 license = "Apache-2.0"
 include = [
     "mech_client/helpers/acn/*",
@@ -22,25 +22,25 @@
     "mech_client/helpers/p2p_libp2p_client/*.yaml",
     "mech_client/helpers/p2p_libp2p_client/*.proto",
     "mech_client/helpers/p2p_libp2p_client/tests/*",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-open-aea = {version = ">=1.42.0", extras = ["cli"]}
-open-aea-ledger-ethereum = ">=1.42.0"
-open-aea-cli-ipfs = ">=1.42.0"
+open-aea = {version = "==1.42.0", extras = ["cli"]}
+open-aea-ledger-ethereum = "==1.42.0"
+open-aea-cli-ipfs = "==1.42.0"
 websocket-client = ">=0.32.0,<1"
 gql = ">=3.4.1"
 asn1crypto = ">=1.4.0,<1.5.0"
-open-aea-ledger-cosmos = ">=1.42.0"
+open-aea-ledger-cosmos = "==1.42.0"
 
 [tool.poetry.scripts]
 mechx = "mech_client.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
-open-autonomy = "==0.13.6"
-tomte = {extras = ["tox"], version = "==0.2.14"}
+open-autonomy = "==0.13.8"
+tomte = {version = "0.2.15", extras = ["tox"]}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mech_client-0.2.8/PKG-INFO` & `mech_client-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: Basic client to interact with a mech
 License: Apache-2.0
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asn1crypto (>=1.4.0,<1.5.0)
 Requires-Dist: gql (>=3.4.1)
-Requires-Dist: open-aea-cli-ipfs (>=1.42.0)
-Requires-Dist: open-aea-ledger-cosmos (>=1.42.0)
-Requires-Dist: open-aea-ledger-ethereum (>=1.42.0)
-Requires-Dist: open-aea[cli] (>=1.42.0)
+Requires-Dist: open-aea-cli-ipfs (==1.42.0)
+Requires-Dist: open-aea-ledger-cosmos (==1.42.0)
+Requires-Dist: open-aea-ledger-ethereum (==1.42.0)
+Requires-Dist: open-aea[cli] (==1.42.0)
 Requires-Dist: websocket-client (>=0.32.0,<1)
 Description-Content-Type: text/markdown
 
 # mech-client
 Basic client to interact with a mech
 
 > **Warning**<br />
```

