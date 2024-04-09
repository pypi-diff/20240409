# Comparing `tmp/moonworm-0.8.0.tar.gz` & `tmp/moonworm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonworm-0.8.0.tar", last modified: Wed Nov  8 20:17:16 2023, max compression
+gzip compressed data, was "moonworm-0.9.0.tar", last modified: Tue Apr  9 17:15:30 2024, max compression
```

## Comparing `moonworm-0.8.0.tar` & `moonworm-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-08 20:16:49.000000 moonworm-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-08 20:16:49.000000 moonworm-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-11-08 20:17:16.876969 moonworm-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2023-11-08 20:16:49.000000 moonworm-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.864969 moonworm-0.8.0/moonworm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.868969 moonworm-0.8.0/moonworm/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-11-08 20:16:55.000000 moonworm-0.8.0/moonworm/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-11-08 20:16:55.000000 moonworm-0.8.0/moonworm/__pycache__/version.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14812 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.872969 moonworm-0.8.0/moonworm/crawler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/ethereum_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/function_call_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/log_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/moonstream_ethereum_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.872969 moonworm-0.8.0/moonworm/crawler/state/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/state/event_scanner_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/state/json_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/state/moonstream_event_state.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/crawler/state/sqlite_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.860969 moonworm-0.8.0/moonworm/fixture/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.872969 moonworm-0.8.0/moonworm/fixture/abis/
--rw-r--r--   0 runner    (1001) docker     (127)    43620 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/CUContract.json
--rw-r--r--   0 runner    (1001) docker     (127)    27178 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/CULands.json
--rw-r--r--   0 runner    (1001) docker     (127)    24823 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/CryptoKitties.json
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/DiamondCutFacet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/Greeter.json
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OpenseaDAOProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    28432 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OpenseaExchange.json
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OpenseaProxyRegistry.json
--rw-r--r--   0 runner    (1001) docker     (127)    16598 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OpenseaToken.json
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OwnableERC1155.json
--rw-r--r--   0 runner    (1001) docker     (127)     8742 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OwnableERC20.json
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/abis/OwnableERC721.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/fixture/bytecodes/
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/Greeter.bin
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaDAOProxy.bin
--rw-r--r--   0 runner    (1001) docker     (127)    39806 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaExchange.bin
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaProxyRegistry.bin
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaToken.bin
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OwnableERC1155.bin
--rw-r--r--   0 runner    (1001) docker     (127)     8108 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OwnableERC20.bin
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/bytecodes/OwnableERC721.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/fixture/events_abi/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/events_abi/events.sample.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/fixture/smart_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/smart_contracts/Greeter.sol
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/smart_contracts/OwnableERC1155.sol
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/smart_contracts/OwnableERC20.sol
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/smart_contracts/OwnableERC721.sol
--rwxr-xr-x   0 runner    (1001) docker     (127)      350 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/fixture/smart_contracts/compile.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    36670 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/brownie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/brownie_contract.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/brownie_contract_foundry.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/brownie_contract_prod.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/cli.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/generators/contract.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/tests/crawler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/crawler/test_function_call_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/crawler/test_function_call_crawler_mainnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.876969 moonworm-0.8.0/moonworm/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/generators/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/test_tester_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/tests/test_testnet.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2023-11-08 20:16:49.000000 moonworm-0.8.0/moonworm/web3_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 20:17:16.868969 moonworm-0.8.0/moonworm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-11-08 20:17:16.000000 moonworm-0.8.0/moonworm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2023-11-08 20:17:16.000000 moonworm-0.8.0/moonworm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 20:17:16.000000 moonworm-0.8.0/moonworm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-08 20:17:16.000000 moonworm-0.8.0/moonworm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-08 20:17:16.000000 moonworm-0.8.0/moonworm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-08 20:17:16.000000 moonworm-0.8.0/moonworm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 20:17:16.876969 moonworm-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-11-08 20:16:49.000000 moonworm-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.424749 moonworm-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 17:15:09.000000 moonworm-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 17:15:09.000000 moonworm-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-09 17:15:30.420749 moonworm-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-09 17:15:09.000000 moonworm-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.412748 moonworm-0.9.0/moonworm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.416749 moonworm-0.9.0/moonworm/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-09 17:15:12.000000 moonworm-0.9.0/moonworm/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 17:15:12.000000 moonworm-0.9.0/moonworm/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14812 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.416749 moonworm-0.9.0/moonworm/crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/ethereum_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/function_call_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/log_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/moonstream_ethereum_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.416749 moonworm-0.9.0/moonworm/crawler/state/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/state/event_scanner_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/state/json_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/state/moonstream_event_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/crawler/state/sqlite_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.412748 moonworm-0.9.0/moonworm/fixture/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.416749 moonworm-0.9.0/moonworm/fixture/abis/
+-rw-r--r--   0 runner    (1001) docker     (127)    43620 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/CUContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27178 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/CULands.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24823 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/CryptoKitties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/DiamondCutFacet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/Greeter.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OpenseaDAOProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28432 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OpenseaExchange.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OpenseaProxyRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16598 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OpenseaToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OwnableERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OwnableERC20.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/abis/OwnableERC721.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/fixture/bytecodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/Greeter.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaDAOProxy.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    39806 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaExchange.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaProxyRegistry.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaToken.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OwnableERC1155.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OwnableERC20.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/bytecodes/OwnableERC721.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/fixture/events_abi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/events_abi/events.sample.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/fixture/smart_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/smart_contracts/Greeter.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/smart_contracts/OwnableERC1155.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/smart_contracts/OwnableERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/smart_contracts/OwnableERC721.sol
+-rwxr-xr-x   0 runner    (1001) docker     (127)      350 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/fixture/smart_contracts/compile.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36935 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/brownie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/brownie_contract.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/brownie_contract_foundry.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/brownie_contract_prod.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/cli.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/generators/contract.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/tests/crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/crawler/test_function_call_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/crawler/test_function_call_crawler_mainnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.420749 moonworm-0.9.0/moonworm/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/generators/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/test_tester_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/tests/test_testnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-09 17:15:09.000000 moonworm-0.9.0/moonworm/web3_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:15:30.416749 moonworm-0.9.0/moonworm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-09 17:15:30.000000 moonworm-0.9.0/moonworm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-09 17:15:30.000000 moonworm-0.9.0/moonworm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:15:30.000000 moonworm-0.9.0/moonworm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 17:15:30.000000 moonworm-0.9.0/moonworm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 17:15:30.000000 moonworm-0.9.0/moonworm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:15:30.000000 moonworm-0.9.0/moonworm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:15:30.424749 moonworm-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-09 17:15:09.000000 moonworm-0.9.0/setup.py
```

### Comparing `moonworm-0.8.0/LICENSE` & `moonworm-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/PKG-INFO` & `moonworm-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonworm
-Version: 0.8.0
+Version: 0.9.0
 Summary: moonworm: Generate a command line interface to any Ethereum smart contract
 Home-page: https://github.com/moonstream-to/moonworm/
 Author: Moonstream
 Author-email: engineering@moonstream.to
 License: UNKNOWN
 Description: ## What is moonworm?
```

### Comparing `moonworm-0.8.0/README.md` & `moonworm-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/abi.py` & `moonworm-0.9.0/moonworm/abi.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/cli.py` & `moonworm-0.9.0/moonworm/cli.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/contracts.py` & `moonworm-0.9.0/moonworm/contracts.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/ethereum_state_provider.py` & `moonworm-0.9.0/moonworm/crawler/ethereum_state_provider.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/example.py` & `moonworm-0.9.0/moonworm/crawler/example.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/function_call_crawler.py` & `moonworm-0.9.0/moonworm/crawler/function_call_crawler.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/log_scanner.py` & `moonworm-0.9.0/moonworm/crawler/log_scanner.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/moonstream_ethereum_state_provider.py` & `moonworm-0.9.0/moonworm/crawler/moonstream_ethereum_state_provider.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/networks.py` & `moonworm-0.9.0/moonworm/crawler/networks.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/state/event_scanner_state.py` & `moonworm-0.9.0/moonworm/crawler/state/event_scanner_state.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/state/json_state.py` & `moonworm-0.9.0/moonworm/crawler/state/json_state.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/crawler/state/moonstream_event_state.py` & `moonworm-0.9.0/moonworm/crawler/state/moonstream_event_state.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/deployment.py` & `moonworm-0.9.0/moonworm/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Allows users to inspect the conditions under which a smart contract was deployed.
 
 The entrypoint for this functionality is [`find_deployment_block`][moonworm.deployment.find_deployment_block].
 """
+
 import logging
 import os
 import time
 from typing import Dict, Optional
 
 from eth_typing.evm import ChecksumAddress
 from web3 import Web3
```

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/CUContract.json` & `moonworm-0.9.0/moonworm/fixture/abis/CUContract.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/CULands.json` & `moonworm-0.9.0/moonworm/fixture/abis/CULands.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/CryptoKitties.json` & `moonworm-0.9.0/moonworm/fixture/abis/CryptoKitties.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/DiamondCutFacet.json` & `moonworm-0.9.0/moonworm/fixture/abis/DiamondCutFacet.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/Greeter.json` & `moonworm-0.9.0/moonworm/fixture/abis/Greeter.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OpenseaDAOProxy.json` & `moonworm-0.9.0/moonworm/fixture/abis/OpenseaDAOProxy.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OpenseaExchange.json` & `moonworm-0.9.0/moonworm/fixture/abis/OpenseaExchange.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OpenseaProxyRegistry.json` & `moonworm-0.9.0/moonworm/fixture/abis/OpenseaProxyRegistry.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OpenseaToken.json` & `moonworm-0.9.0/moonworm/fixture/abis/OpenseaToken.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OwnableERC1155.json` & `moonworm-0.9.0/moonworm/fixture/abis/OwnableERC1155.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OwnableERC20.json` & `moonworm-0.9.0/moonworm/fixture/abis/OwnableERC20.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/abis/OwnableERC721.json` & `moonworm-0.9.0/moonworm/fixture/abis/OwnableERC721.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/Greeter.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/Greeter.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaDAOProxy.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaDAOProxy.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaExchange.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaExchange.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaProxyRegistry.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaProxyRegistry.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OpenseaToken.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OpenseaToken.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OwnableERC1155.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OwnableERC1155.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OwnableERC20.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OwnableERC20.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/bytecodes/OwnableERC721.bin` & `moonworm-0.9.0/moonworm/fixture/bytecodes/OwnableERC721.bin`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/events_abi/events.sample.json` & `moonworm-0.9.0/moonworm/fixture/events_abi/events.sample.json`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/smart_contracts/OwnableERC1155.sol` & `moonworm-0.9.0/moonworm/fixture/smart_contracts/OwnableERC1155.sol`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/smart_contracts/OwnableERC20.sol` & `moonworm-0.9.0/moonworm/fixture/smart_contracts/OwnableERC20.sol`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/fixture/smart_contracts/OwnableERC721.sol` & `moonworm-0.9.0/moonworm/fixture/smart_contracts/OwnableERC721.sol`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/generators/basic.py` & `moonworm-0.9.0/moonworm/generators/basic.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/generators/brownie.py` & `moonworm-0.9.0/moonworm/generators/brownie.py`

 * *Files 1% similar despite different names*

```diff
@@ -835,14 +835,21 @@
             elif param["type"] == "tuple":
                 call_args.append(
                     cst.Arg(
                         keyword=cst.Name(value="type"),
                         value=cst.parse_expression("eval"),
                     ),
                 )
+            elif param["type"] == "tuple[]":
+                call_args.append(
+                    cst.Arg(
+                        keyword=cst.Name(value="type"),
+                        value=cst.parse_expression("eval"),
+                    ),
+                )
             elif param["type"] == "Any":
                 # In general case, we just use a Python `eval` to parse the input from the command line.
                 # This is similar to the way we handle `tuple` arguments.
                 call_args.append(
                     cst.Arg(
                         keyword=cst.Name(value="type"),
                         value=cst.parse_expression("eval"),
```

### Comparing `moonworm-0.8.0/moonworm/generators/brownie_contract.py.template` & `moonworm-0.9.0/moonworm/generators/brownie_contract.py.template`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/generators/brownie_contract_foundry.py.template` & `moonworm-0.9.0/moonworm/generators/brownie_contract_foundry.py.template`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/generators/brownie_contract_prod.py.template` & `moonworm-0.9.0/moonworm/generators/brownie_contract_prod.py.template`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/generators/cli.py.template` & `moonworm-0.9.0/moonworm/generators/cli.py.template`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/generators/contract.py.template` & `moonworm-0.9.0/moonworm/generators/contract.py.template`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/manage.py` & `moonworm-0.9.0/moonworm/manage.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/tests/crawler/test_function_call_crawler.py` & `moonworm-0.9.0/moonworm/tests/crawler/test_function_call_crawler.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/tests/crawler/test_function_call_crawler_mainnet.py` & `moonworm-0.9.0/moonworm/tests/crawler/test_function_call_crawler_mainnet.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/tests/generators/test_basic.py` & `moonworm-0.9.0/moonworm/tests/generators/test_basic.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/tests/test_tester_provider.py` & `moonworm-0.9.0/moonworm/tests/test_tester_provider.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/tests/test_testnet.py` & `moonworm-0.9.0/moonworm/tests/test_testnet.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/watch.py` & `moonworm-0.9.0/moonworm/watch.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm/web3_util.py` & `moonworm-0.9.0/moonworm/web3_util.py`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/moonworm.egg-info/PKG-INFO` & `moonworm-0.9.0/moonworm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonworm
-Version: 0.8.0
+Version: 0.9.0
 Summary: moonworm: Generate a command line interface to any Ethereum smart contract
 Home-page: https://github.com/moonstream-to/moonworm/
 Author: Moonstream
 Author-email: engineering@moonstream.to
 License: UNKNOWN
 Description: ## What is moonworm?
```

### Comparing `moonworm-0.8.0/moonworm.egg-info/SOURCES.txt` & `moonworm-0.9.0/moonworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moonworm-0.8.0/setup.py` & `moonworm-0.9.0/setup.py`

 * *Files identical despite different names*

