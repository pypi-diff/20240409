# Comparing `tmp/wireguard_tools-0.4.6.tar.gz` & `tmp/wireguard_tools-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireguard_tools-0.4.6.tar", max compression
+gzip compressed data, was "wireguard_tools-0.4.7.tar", max compression
```

## Comparing `wireguard_tools-0.4.6.tar` & `wireguard_tools-0.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1083 2022-12-14 04:23:20.284345 wireguard_tools-0.4.6/LICENSE
-drwxr-xr-x   0        0        0        0 2022-12-14 04:23:20.284345 wireguard_tools-0.4.6/LICENSES/
--rw-r--r--   0        0        0      643 2022-12-14 04:23:20.284345 wireguard_tools-0.4.6/LICENSES/0BSD.txt
--rw-r--r--   0        0        0     1593 2022-12-14 04:23:20.284345 wireguard_tools-0.4.6/LICENSES/CC-PDDC.txt
--rw-r--r--   0        0        0     1078 2022-12-14 04:23:20.284345 wireguard_tools-0.4.6/LICENSES/MIT.txt
--rw-r--r--   0        0        0     6958 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/README.md
--rw-r--r--   0        0        0     2183 2024-03-19 16:12:43.576606 wireguard_tools-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      394 2024-03-19 16:12:43.576606 wireguard_tools-0.4.6/src/wireguard_tools/__init__.py
--rw-r--r--   0        0        0      188 2022-12-14 04:23:20.288346 wireguard_tools-0.4.6/src/wireguard_tools/__main__.py
--rw-r--r--   0        0        0     7889 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/cli.py
--rw-r--r--   0        0        0     5736 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/curve25519.py
--rw-r--r--   0        0        0        0 2022-12-14 04:23:20.288346 wireguard_tools-0.4.6/src/wireguard_tools/py.typed
--rw-r--r--   0        0        0    12130 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/wireguard_config.py
--rw-r--r--   0        0        0     1276 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/wireguard_device.py
--rw-r--r--   0        0        0     2583 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/wireguard_key.py
--rw-r--r--   0        0        0     4494 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/wireguard_netlink.py
--rw-r--r--   0        0        0     6125 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/src/wireguard_tools/wireguard_uapi.py
--rw-r--r--   0        0        0        0 2022-12-14 04:23:20.288346 wireguard_tools-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0      215 2022-12-14 04:23:20.288346 wireguard_tools-0.4.6/tests/conftest.py
--rw-r--r--   0        0        0     8975 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/tests/test_curve25519.py
--rw-r--r--   0        0        0      257 2024-03-19 16:11:43.327460 wireguard_tools-0.4.6/tests/test_entrypoints.py
--rw-r--r--   0        0        0     3478 2024-03-19 16:09:40.517123 wireguard_tools-0.4.6/tests/test_wireguard_config.py
--rw-r--r--   0        0        0      661 2022-12-14 04:23:20.288346 wireguard_tools-0.4.6/tests/test_wireguard_key.py
--rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 wireguard_tools-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-13 17:55:51.419036 wireguard_tools-0.4.7/LICENSE
+drwxr-xr-x   0        0        0        0 2022-12-13 17:55:51.419036 wireguard_tools-0.4.7/LICENSES/
+-rw-r--r--   0        0        0      643 2022-12-13 17:55:51.419036 wireguard_tools-0.4.7/LICENSES/0BSD.txt
+-rw-r--r--   0        0        0     1593 2022-12-13 17:55:51.419036 wireguard_tools-0.4.7/LICENSES/CC-PDDC.txt
+-rw-r--r--   0        0        0     1078 2022-12-13 17:55:51.419036 wireguard_tools-0.4.7/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     6958 2024-03-19 15:56:41.129853 wireguard_tools-0.4.7/README.md
+-rw-r--r--   0        0        0     2212 2024-04-09 17:00:04.299995 wireguard_tools-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      394 2024-04-09 17:00:04.303995 wireguard_tools-0.4.7/src/wireguard_tools/__init__.py
+-rw-r--r--   0        0        0      188 2022-12-13 17:55:51.423036 wireguard_tools-0.4.7/src/wireguard_tools/__main__.py
+-rw-r--r--   0        0        0     7889 2024-03-19 15:54:13.165789 wireguard_tools-0.4.7/src/wireguard_tools/cli.py
+-rw-r--r--   0        0        0     5736 2024-03-19 14:54:00.408481 wireguard_tools-0.4.7/src/wireguard_tools/curve25519.py
+-rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.7/src/wireguard_tools/py.typed
+-rw-r--r--   0        0        0    12130 2024-03-19 15:55:00.779099 wireguard_tools-0.4.7/src/wireguard_tools/wireguard_config.py
+-rw-r--r--   0        0        0     1276 2024-03-19 15:55:26.083795 wireguard_tools-0.4.7/src/wireguard_tools/wireguard_device.py
+-rw-r--r--   0        0        0     2583 2024-03-19 15:55:38.580139 wireguard_tools-0.4.7/src/wireguard_tools/wireguard_key.py
+-rw-r--r--   0        0        0     4502 2024-04-09 16:37:57.778335 wireguard_tools-0.4.7/src/wireguard_tools/wireguard_netlink.py
+-rw-r--r--   0        0        0     6125 2024-03-19 15:55:56.740637 wireguard_tools-0.4.7/src/wireguard_tools/wireguard_uapi.py
+-rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.7/tests/__init__.py
+-rw-r--r--   0        0        0      215 2022-12-13 17:55:51.423036 wireguard_tools-0.4.7/tests/conftest.py
+-rw-r--r--   0        0        0     8975 2024-03-19 15:56:16.741186 wireguard_tools-0.4.7/tests/test_curve25519.py
+-rw-r--r--   0        0        0      257 2024-04-09 16:36:46.128306 wireguard_tools-0.4.7/tests/test_entrypoints.py
+-rw-r--r--   0        0        0     3478 2024-03-19 15:56:28.449506 wireguard_tools-0.4.7/tests/test_wireguard_config.py
+-rw-r--r--   0        0        0      661 2024-03-19 14:04:19.383947 wireguard_tools-0.4.7/tests/test_wireguard_key.py
+-rw-r--r--   0        0        0     8118 1970-01-01 00:00:00.000000 wireguard_tools-0.4.7/PKG-INFO
```

### Comparing `wireguard_tools-0.4.6/LICENSE` & `wireguard_tools-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/LICENSES/0BSD.txt` & `wireguard_tools-0.4.7/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/LICENSES/CC-PDDC.txt` & `wireguard_tools-0.4.7/LICENSES/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/LICENSES/MIT.txt` & `wireguard_tools-0.4.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/README.md` & `wireguard_tools-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/pyproject.toml` & `wireguard_tools-0.4.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022-2024 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "wireguard-tools"
-version = "0.4.6"
+version = "0.4.7"
 description = "Pure python reimplementation of wireguard-tools"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -33,15 +33,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 attrs = ">=22.1.0"
 pyroute2 = "^0.7.3"
 segno = "^1.5.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
+black = { version=">=24.3.0", python = "^3.8" }
 poethepoet = "^0.16.5"
 pre-commit = { version = "^3.5.0", python = "^3.8.1" }
 tbump = "^6.9.0"
 
 [tool.poetry.group.test.dependencies]
 mypy = "^0.991"
 pytest = "^6.2.5"
```

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/cli.py` & `wireguard_tools-0.4.7/src/wireguard_tools/cli.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/curve25519.py` & `wireguard_tools-0.4.7/src/wireguard_tools/curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/wireguard_config.py` & `wireguard_tools-0.4.7/src/wireguard_tools/wireguard_config.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/wireguard_device.py` & `wireguard_tools-0.4.7/src/wireguard_tools/wireguard_device.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/wireguard_key.py` & `wireguard_tools-0.4.7/src/wireguard_tools/wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/wireguard_netlink.py` & `wireguard_tools-0.4.7/src/wireguard_tools/wireguard_netlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 endpoint_port=peer_attrs.get("WGPEER_A_ENDPOINT", {}).get("port"),
                 persistent_keepalive=peer_attrs[
                     "WGPEER_A_PERSISTENT_KEEPALIVE_INTERVAL"
                 ]
                 or None,
                 allowed_ips=[
                     allowed_ip["addr"]
-                    for allowed_ip in peer_attrs["WGPEER_A_ALLOWEDIPS"]
+                    for allowed_ip in peer_attrs.get("WGPEER_A_ALLOWEDIPS", [])
                 ],
                 last_handshake=peer_attrs.get("WGPEER_A_LAST_HANDSHAKE_TIME", {}).get(
                     "tv_sec",
                 ),
                 rx_bytes=peer_attrs.get("WGPEER_A_RX_BYTES"),
                 tx_bytes=peer_attrs.get("WGPEER_A_TX_BYTES"),
             )
```

### Comparing `wireguard_tools-0.4.6/src/wireguard_tools/wireguard_uapi.py` & `wireguard_tools-0.4.7/src/wireguard_tools/wireguard_uapi.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/tests/test_curve25519.py` & `wireguard_tools-0.4.7/tests/test_curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/tests/test_wireguard_config.py` & `wireguard_tools-0.4.7/tests/test_wireguard_config.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/tests/test_wireguard_key.py` & `wireguard_tools-0.4.7/tests/test_wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.6/PKG-INFO` & `wireguard_tools-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wireguard-tools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Pure python reimplementation of wireguard-tools
 Home-page: https://github.com/cmusatyalab/wireguard-tools
 License: MIT
 Author: Carnegie Mellon University
 Author-email: satya+group@cs.cmu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: attrs (>=22.1.0)
 Requires-Dist: pyroute2 (>=0.7.3,<0.8.0)
 Requires-Dist: segno (>=1.5.2,<2.0.0)
 Project-URL: Repository, https://github.com/cmusatyalab/wireguard-tools
 Description-Content-Type: text/markdown
```

