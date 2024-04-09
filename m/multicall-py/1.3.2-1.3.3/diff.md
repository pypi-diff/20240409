# Comparing `tmp/multicall-py-1.3.2.tar.gz` & `tmp/multicall-py-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall-py-1.3.2.tar", last modified: Thu Sep 14 03:11:20 2023, max compression
+gzip compressed data, was "multicall-py-1.3.3.tar", last modified: Tue Apr  9 03:26:32 2024, max compression
```

## Comparing `multicall-py-1.3.2.tar` & `multicall-py-1.3.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2023-09-14 03:11:20.398312 multicall-py-1.3.2/
--rw-r--r--   0 jsvisa     (501) staff       (20)     1064 2023-03-16 12:45:05.000000 multicall-py-1.3.2/LICENSE
--rw-r--r--   0 jsvisa     (501) staff       (20)       30 2023-03-16 12:45:05.000000 multicall-py-1.3.2/MANIFEST.in
--rw-r--r--   0 jsvisa     (501) staff       (20)     3328 2023-09-14 03:11:20.398180 multicall-py-1.3.2/PKG-INFO
--rw-r--r--   0 jsvisa     (501) staff       (20)     2227 2023-08-28 11:12:52.000000 multicall-py-1.3.2/README.md
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2023-09-14 03:11:20.395666 multicall-py-1.3.2/multicall/
--rw-r--r--   0 jsvisa     (501) staff       (20)      211 2023-09-14 03:10:21.000000 multicall-py-1.3.2/multicall/__init__.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2023-09-14 03:11:20.396391 multicall-py-1.3.2/multicall/__pycache__/
--rw-r--r--   0 jsvisa     (501) staff       (20)      378 2023-08-29 08:59:55.000000 multicall-py-1.3.2/multicall/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     1787 2023-08-29 08:59:55.000000 multicall-py-1.3.2/multicall/__pycache__/balance_call.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     2379 2023-08-29 08:59:55.000000 multicall-py-1.3.2/multicall/__pycache__/call.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     3672 2023-08-29 08:59:55.000000 multicall-py-1.3.2/multicall/__pycache__/eth_decode.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     4878 2023-08-29 08:59:55.000000 multicall-py-1.3.2/multicall/__pycache__/multicall.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     2917 2023-08-29 08:59:55.000000 multicall-py-1.3.2/multicall/__pycache__/signature.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     1638 2023-09-14 03:07:50.000000 multicall-py-1.3.2/multicall/balance_call.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     2572 2023-09-12 08:34:46.000000 multicall-py-1.3.2/multicall/call.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3862 2023-09-12 08:15:04.000000 multicall-py-1.3.2/multicall/eth_decode.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     5058 2023-08-28 11:13:06.000000 multicall-py-1.3.2/multicall/multicall.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2023-09-14 03:11:20.397203 multicall-py-1.3.2/multicall/service/
--rw-r--r--   0 jsvisa     (501) staff       (20)      276 2023-03-16 12:45:05.000000 multicall-py-1.3.2/multicall/service/__init__.py
--rw-r--r--   0 jsvisa     (501) staff       (20)      708 2023-09-14 03:09:22.000000 multicall-py-1.3.2/multicall/service/base_token_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     4257 2023-03-16 12:45:05.000000 multicall-py-1.3.2/multicall/service/erc1155_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     2321 2023-03-16 12:45:05.000000 multicall-py-1.3.2/multicall/service/erc20_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3033 2023-03-16 12:45:05.000000 multicall-py-1.3.2/multicall/service/erc721_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     2933 2023-09-14 03:08:16.000000 multicall-py-1.3.2/multicall/service/ether_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3668 2023-03-16 12:45:05.000000 multicall-py-1.3.2/multicall/service/token_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3726 2023-09-12 09:45:50.000000 multicall-py-1.3.2/multicall/signature.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2023-09-14 03:11:20.397753 multicall-py-1.3.2/multicall_py.egg-info/
--rw-r--r--   0 jsvisa     (501) staff       (20)     3328 2023-09-14 03:11:20.000000 multicall-py-1.3.2/multicall_py.egg-info/PKG-INFO
--rw-r--r--   0 jsvisa     (501) staff       (20)      936 2023-09-14 03:11:20.000000 multicall-py-1.3.2/multicall_py.egg-info/SOURCES.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)        1 2023-09-14 03:11:20.000000 multicall-py-1.3.2/multicall_py.egg-info/dependency_links.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)       24 2023-09-14 03:11:20.000000 multicall-py-1.3.2/multicall_py.egg-info/requires.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)       10 2023-09-14 03:11:20.000000 multicall-py-1.3.2/multicall_py.egg-info/top_level.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)       38 2023-09-14 03:11:20.398345 multicall-py-1.3.2/setup.cfg
--rw-r--r--   0 jsvisa     (501) staff       (20)     1470 2023-09-14 03:10:16.000000 multicall-py-1.3.2/setup.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2023-09-14 03:11:20.398016 multicall-py-1.3.2/tests/
--rw-r--r--   0 jsvisa     (501) staff       (20)    16859 2023-09-08 03:13:01.000000 multicall-py-1.3.2/tests/test_eth_decode.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3080 2023-09-12 09:45:50.000000 multicall-py-1.3.2/tests/test_signature.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.435272 multicall-py-1.3.3/
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1064 2023-03-16 12:45:05.000000 multicall-py-1.3.3/LICENSE
+-rw-r--r--   0 jsvisa     (501) staff       (20)       30 2023-03-16 12:45:05.000000 multicall-py-1.3.3/MANIFEST.in
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3328 2024-04-09 03:26:32.435006 multicall-py-1.3.3/PKG-INFO
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2227 2023-08-28 11:12:52.000000 multicall-py-1.3.3/README.md
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.427590 multicall-py-1.3.3/multicall/
+-rw-r--r--   0 jsvisa     (501) staff       (20)      211 2024-04-09 03:24:37.000000 multicall-py-1.3.3/multicall/__init__.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.429871 multicall-py-1.3.3/multicall/__pycache__/
+-rw-r--r--   0 jsvisa     (501) staff       (20)      378 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1791 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/balance_call.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2379 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/call.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3672 2023-08-29 08:59:55.000000 multicall-py-1.3.3/multicall/__pycache__/eth_decode.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     4878 2023-08-29 08:59:55.000000 multicall-py-1.3.3/multicall/__pycache__/multicall.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3453 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/signature.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1638 2023-10-31 02:03:51.000000 multicall-py-1.3.3/multicall/balance_call.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2572 2023-09-12 08:34:46.000000 multicall-py-1.3.3/multicall/call.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3862 2023-09-12 08:15:04.000000 multicall-py-1.3.3/multicall/eth_decode.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     5009 2024-04-09 03:24:28.000000 multicall-py-1.3.3/multicall/multicall.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.432093 multicall-py-1.3.3/multicall/service/
+-rw-r--r--   0 jsvisa     (501) staff       (20)      276 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/__init__.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)      708 2023-09-14 03:09:22.000000 multicall-py-1.3.3/multicall/service/base_token_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     4257 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/erc1155_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2321 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/erc20_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3033 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/erc721_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2933 2023-09-14 03:08:16.000000 multicall-py-1.3.3/multicall/service/ether_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3668 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/token_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3726 2023-09-12 09:45:50.000000 multicall-py-1.3.3/multicall/signature.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.433677 multicall-py-1.3.3/multicall_py.egg-info/
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3328 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/PKG-INFO
+-rw-r--r--   0 jsvisa     (501) staff       (20)      936 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)        1 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)       24 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/requires.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)       10 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/top_level.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)       38 2024-04-09 03:26:32.435499 multicall-py-1.3.3/setup.cfg
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1470 2024-04-09 03:24:44.000000 multicall-py-1.3.3/setup.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.434490 multicall-py-1.3.3/tests/
+-rw-r--r--   0 jsvisa     (501) staff       (20)    16859 2023-09-08 03:13:01.000000 multicall-py-1.3.3/tests/test_eth_decode.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3080 2023-09-12 09:45:50.000000 multicall-py-1.3.3/tests/test_signature.py
```

### Comparing `multicall-py-1.3.2/LICENSE` & `multicall-py-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/PKG-INFO` & `multicall-py-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicall-py
-Version: 1.3.2
+Version: 1.3.3
 Summary: Ethereum multiple contract/rpc calls
 Home-page: https://github.com/jsvisa/multicall.py
 Author: Wenbiao Zheng
 Author-email: delweng@gmail.com
 License: MIT
 Keywords: ethereum jsonrpc contract
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `multicall-py-1.3.2/README.md` & `multicall-py-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/__pycache__/balance_call.cpython-310.pyc` & `multicall-py-1.3.3/multicall/__pycache__/balance_call.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 16 12:45:05 2023 UTC, .py size: 1633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 510f 1364 6106 0000  o.......Q..da...
+00000000: 6f0d 0d0a 0000 0000 8760 4065 6606 0000  o........`@ef...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6404 6c07 6d08 5a08 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6508 8303 5a09 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 e900 0000 0029 04da 084f 7074  S.)......)...Opt
@@ -50,63 +50,63 @@
 00000310: 6f64 655f 6461 7461 da04 6172 6773 2901  ode_data..args).
 00000320: 7211 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
 00000330: 1300 0000 da08 6361 6c6c 6461 7461 1700  ......calldata..
 00000340: 0000 7302 0000 000e 027a 1442 616c 616e  ..s......z.Balan
 00000350: 6365 4361 6c6c 2e63 616c 6c64 6174 61da  ceCall.calldata.
 00000360: 0772 7063 5f72 6573 da06 7265 7475 726e  .rpc_res..return
 00000370: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
-00000380: 000a 0000 0043 0000 0073 6600 0000 6401  .....C...sf...d.
-00000390: 7c01 7600 720d 7c00 6a00 7209 7c01 5300  |.v.r.|.j.r.|.S.
-000003a0: 7401 7c01 8301 8201 7a0a 7402 7c01 6402  t.|.....z.t.|.d.
-000003b0: 1900 6403 8302 7d03 5700 7c03 5300 0400  ..d...}.W.|.S...
-000003c0: 7403 7932 0100 7d04 0100 7a0f 7c02 6404  t.y2..}...z.|.d.
-000003d0: 7500 722a 5700 5900 6400 7d04 7e04 6400  u.r*W.Y.d.}.~.d.
-000003e0: 5300 7403 7c04 8301 8201 6400 7d04 7e04  S.t.|.....d.}.~.
-000003f0: 7701 7700 2905 4eda 0565 7272 6f72 da06  w.w.).N..error..
-00000400: 7265 7375 6c74 e910 0000 0054 2904 720f  result.....T).r.
-00000410: 0000 00da 0a56 616c 7565 4572 726f 72da  .....ValueError.
-00000420: 0369 6e74 da09 4578 6365 7074 696f 6e29  .int..Exception)
-00000430: 0572 1100 0000 7219 0000 0072 0f00 0000  .r....r....r....
-00000440: da07 6261 6c61 6e63 65da 0165 7212 0000  ..balance..er...
-00000450: 0072 1200 0000 7213 0000 00da 0664 6563  .r....r......dec
-00000460: 6f64 651b 0000 0073 1a00 0000 0801 0601  ode....s........
-00000470: 0401 0802 0202 1001 0405 0efc 0801 0e01  ................
-00000480: 0801 0880 02fd 7a12 4261 6c61 6e63 6543  ......z.BalanceC
-00000490: 616c 6c2e 6465 636f 6465 6303 0000 0000  all.decodec.....
-000004a0: 0000 0000 0000 0004 0000 0006 0000 0043  ...............C
-000004b0: 0000 0073 3600 0000 7c01 7006 7c00 6a00  ...s6...|.p.|.j.
-000004c0: 7006 6401 7d03 6402 6403 7c00 6a01 7402  p.d.}.d.d.|.j.t.
-000004d0: 7c03 7403 8302 7214 7404 7c03 8301 6e01  |.t...r.t.|...n.
-000004e0: 7c03 6702 7c00 6a05 6404 9c04 5300 2905  |.g.|.j.d...S.).
-000004f0: 4e72 0a00 0000 7a03 322e 30da 0e65 7468  Nr....z.2.0..eth
-00000500: 5f67 6574 4261 6c61 6e63 6529 04da 076a  _getBalance)...j
-00000510: 736f 6e72 7063 da06 6d65 7468 6f64 da06  sonrpc..method..
-00000520: 7061 7261 6d73 da02 6964 2906 720d 0000  params..id).r...
-00000530: 0072 0b00 0000 da0a 6973 696e 7374 616e  .r......isinstan
-00000540: 6365 721f 0000 00da 0368 6578 720c 0000  cer......hexr...
-00000550: 0029 0472 1100 0000 720d 0000 0072 0e00  .).r....r....r..
-00000560: 0000 da05 626c 6f63 6b72 1200 0000 7212  ....blockr....r.
-00000570: 0000 0072 1300 0000 da08 5f5f 6361 6c6c  ...r......__call
-00000580: 5f5f 2a00 0000 7310 0000 000e 0502 0202  __*...s.........
-00000590: 0104 0214 0102 fe04 0406 f97a 1442 616c  ...........z.Bal
-000005a0: 616e 6365 4361 6c6c 2e5f 5f63 616c 6c5f  anceCall.__call_
-000005b0: 5f29 044e 720a 0000 004e 4629 0146 2902  _).Nr....NF).F).
-000005c0: 4e4e 290f da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
-000005d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000005e0: 616c 6e61 6d65 5f5f da03 7374 7272 0200  alname__..strr..
-000005f0: 0000 7203 0000 0072 1f00 0000 da04 626f  ..r....r......bo
-00000600: 6f6c 7214 0000 00da 0870 726f 7065 7274  olr......propert
-00000610: 7972 1800 0000 7204 0000 0072 0500 0000  yr....r....r....
-00000620: 7223 0000 0072 2c00 0000 7212 0000 0072  r#...r,...r....r
-00000630: 1200 0000 7212 0000 0072 1300 0000 7209  ....r....r....r.
-00000640: 0000 0006 0000 0073 3400 0000 0800 0204  .......s4.......
-00000650: 0201 0201 0201 04fa 0202 02fe 0e03 02fd  ................
-00000660: 0a04 02fc 0605 02fb 0206 0afa 0210 0a01  ................
-00000670: 1803 0211 0201 04fd 0e02 02fe 0603 0efd  ................
-00000680: 7209 0000 004e 290a da06 7479 7069 6e67  r....N)...typing
-00000690: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-000006a0: 0500 0000 5a11 6574 685f 7574 696c 732e  ....Z.eth_utils.
-000006b0: 6164 6472 6573 7372 0600 0000 da04 6361  addressr......ca
-000006c0: 6c6c 7208 0000 0072 0900 0000 7212 0000  llr....r....r...
-000006d0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000006e0: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-000006f0: 0000 0018 000c 010c 0114 03              ...........
+00000380: 000a 0000 0043 0000 0073 6a00 0000 6401  .....C...sj...d.
+00000390: 7c01 7600 720f 7c00 6a00 6402 7500 720b  |.v.r.|.j.d.u.r.
+000003a0: 6400 5300 7401 7c01 8301 8201 7a0a 7402  d.S.t.|.....z.t.
+000003b0: 7c01 6403 1900 6404 8302 7d03 5700 7c03  |.d...d...}.W.|.
+000003c0: 5300 0400 7403 7934 0100 7d04 0100 7a0f  S...t.y4..}...z.
+000003d0: 7c02 6402 7500 722c 5700 5900 6400 7d04  |.d.u.r,W.Y.d.}.
+000003e0: 7e04 6400 5300 7403 7c04 8301 8201 6400  ~.d.S.t.|.....d.
+000003f0: 7d04 7e04 7701 7700 2905 4eda 0565 7272  }.~.w.w.).N..err
+00000400: 6f72 54da 0672 6573 756c 74e9 1000 0000  orT..result.....
+00000410: 2904 720f 0000 00da 0a56 616c 7565 4572  ).r......ValueEr
+00000420: 726f 72da 0369 6e74 da09 4578 6365 7074  ror..int..Except
+00000430: 696f 6e29 0572 1100 0000 7219 0000 0072  ion).r....r....r
+00000440: 0f00 0000 da07 6261 6c61 6e63 65da 0165  ......balance..e
+00000450: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000460: 0664 6563 6f64 651b 0000 0073 1a00 0000  .decode....s....
+00000470: 0801 0a01 0401 0802 0202 1001 0405 0efc  ................
+00000480: 0801 0e01 0801 0880 02fd 7a12 4261 6c61  ..........z.Bala
+00000490: 6e63 6543 616c 6c2e 6465 636f 6465 6303  nceCall.decodec.
+000004a0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+000004b0: 0000 0043 0000 0073 3600 0000 7c01 7006  ...C...s6...|.p.
+000004c0: 7c00 6a00 7006 6401 7d03 6402 6403 7c00  |.j.p.d.}.d.d.|.
+000004d0: 6a01 7402 7c03 7403 8302 7214 7404 7c03  j.t.|.t...r.t.|.
+000004e0: 8301 6e01 7c03 6702 7c00 6a05 6404 9c04  ..n.|.g.|.j.d...
+000004f0: 5300 2905 4e72 0a00 0000 7a03 322e 30da  S.).Nr....z.2.0.
+00000500: 0e65 7468 5f67 6574 4261 6c61 6e63 6529  .eth_getBalance)
+00000510: 04da 076a 736f 6e72 7063 da06 6d65 7468  ...jsonrpc..meth
+00000520: 6f64 da06 7061 7261 6d73 da02 6964 2906  od..params..id).
+00000530: 720d 0000 0072 0b00 0000 da0a 6973 696e  r....r......isin
+00000540: 7374 616e 6365 721f 0000 00da 0368 6578  stancer......hex
+00000550: 720c 0000 0029 0472 1100 0000 720d 0000  r....).r....r...
+00000560: 0072 0e00 0000 da05 626c 6f63 6b72 1200  .r......blockr..
+00000570: 0000 7212 0000 0072 1300 0000 da08 5f5f  ..r....r......__
+00000580: 6361 6c6c 5f5f 2a00 0000 7310 0000 000e  call__*...s.....
+00000590: 0502 0202 0104 0214 0102 fe04 0406 f97a  ...............z
+000005a0: 1442 616c 616e 6365 4361 6c6c 2e5f 5f63  .BalanceCall.__c
+000005b0: 616c 6c5f 5f29 044e 720a 0000 004e 4629  all__).Nr....NF)
+000005c0: 0146 2902 4e4e 290f da08 5f5f 6e61 6d65  .F).NN)...__name
+000005d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000005e0: 5f5f 7175 616c 6e61 6d65 5f5f da03 7374  __qualname__..st
+000005f0: 7272 0200 0000 7203 0000 0072 1f00 0000  rr....r....r....
+00000600: da04 626f 6f6c 7214 0000 00da 0870 726f  ..boolr......pro
+00000610: 7065 7274 7972 1800 0000 7204 0000 0072  pertyr....r....r
+00000620: 0500 0000 7223 0000 0072 2c00 0000 7212  ....r#...r,...r.
+00000630: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00000640: 0000 7209 0000 0006 0000 0073 3400 0000  ..r........s4...
+00000650: 0800 0204 0201 0201 0201 04fa 0202 02fe  ................
+00000660: 0e03 02fd 0a04 02fc 0605 02fb 0206 0afa  ................
+00000670: 0210 0a01 1803 0211 0201 04fd 0e02 02fe  ................
+00000680: 0603 0efd 7209 0000 004e 290a da06 7479  ....r....N)...ty
+00000690: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
+000006a0: 0000 0072 0500 0000 5a11 6574 685f 7574  ...r....Z.eth_ut
+000006b0: 696c 732e 6164 6472 6573 7372 0600 0000  ils.addressr....
+000006c0: da04 6361 6c6c 7208 0000 0072 0900 0000  ..callr....r....
+000006d0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+000006e0: 1300 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000006f0: 0000 7308 0000 0018 000c 010c 0114 03    ..s............
```

### Comparing `multicall-py-1.3.2/multicall/__pycache__/call.cpython-310.pyc` & `multicall-py-1.3.3/multicall/__pycache__/call.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 16 12:45:05 2023 UTC, .py size: 2572 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 510f 1364 0c0a 0000  o.......Q..d....
+00000000: 6f0d 0d0a 0000 0000 a622 0065 0c0a 0000  o........".e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6403 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6404 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 8302 5a0c  ..G.d.d...d...Z.
```

### Comparing `multicall-py-1.3.2/multicall/__pycache__/eth_decode.cpython-310.pyc` & `multicall-py-1.3.3/multicall/__pycache__/eth_decode.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/__pycache__/multicall.cpython-310.pyc` & `multicall-py-1.3.3/multicall/__pycache__/multicall.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/balance_call.py` & `multicall-py-1.3.3/multicall/balance_call.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/call.py` & `multicall-py-1.3.3/multicall/call.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/eth_decode.py` & `multicall-py-1.3.3/multicall/eth_decode.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/multicall.py` & `multicall-py-1.3.3/multicall/multicall.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ):
         self.provider_uri = provider_uri
         if session is None:
             retry = Retry(
                 total=3,
                 backoff_factor=2,
                 status_forcelist=[429, 500, 502, 503, 504],
-                allowed_methods=["POST", "GET"],
                 respect_retry_after_header=False,
             )
             adapter = requests.adapters.HTTPAdapter(max_retries=retry)
             session = Session()
             session.mount("http://", adapter)
             session.mount("https://", adapter)
```

### Comparing `multicall-py-1.3.2/multicall/service/base_token_service.py` & `multicall-py-1.3.3/multicall/service/base_token_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/service/erc1155_service.py` & `multicall-py-1.3.3/multicall/service/erc1155_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/service/erc20_service.py` & `multicall-py-1.3.3/multicall/service/erc20_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/service/erc721_service.py` & `multicall-py-1.3.3/multicall/service/erc721_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/service/ether_service.py` & `multicall-py-1.3.3/multicall/service/ether_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/service/token_service.py` & `multicall-py-1.3.3/multicall/service/token_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall/signature.py` & `multicall-py-1.3.3/multicall/signature.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/multicall_py.egg-info/PKG-INFO` & `multicall-py-1.3.3/multicall_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicall-py
-Version: 1.3.2
+Version: 1.3.3
 Summary: Ethereum multiple contract/rpc calls
 Home-page: https://github.com/jsvisa/multicall.py
 Author: Wenbiao Zheng
 Author-email: delweng@gmail.com
 License: MIT
 Keywords: ethereum jsonrpc contract
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `multicall-py-1.3.2/multicall_py.egg-info/SOURCES.txt` & `multicall-py-1.3.3/multicall_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/setup.py` & `multicall-py-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 setup(
     name="multicall-py",
-    version="1.3.2",
+    version="1.3.3",
     description="Ethereum multiple contract/rpc calls",
     long_description=open(os.path.join(here, "README.md")).read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `multicall-py-1.3.2/tests/test_eth_decode.py` & `multicall-py-1.3.3/tests/test_eth_decode.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.2/tests/test_signature.py` & `multicall-py-1.3.3/tests/test_signature.py`

 * *Files identical despite different names*

