# Comparing `tmp/pycv_crossvalidation-0.0.2.tar.gz` & `tmp/pycv_crossvalidation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycv_crossvalidation-0.0.2.tar", last modified: Thu Mar 21 12:33:59 2024, max compression
+gzip compressed data, was "pycv_crossvalidation-0.0.3.tar", last modified: Tue Apr  9 05:27:56 2024, max compression
```

## Comparing `pycv_crossvalidation-0.0.2.tar` & `pycv_crossvalidation-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 12:33:59.382240 pycv_crossvalidation-0.0.2/
--rw-rw-rw-   0        0        0      457 2024-03-21 12:33:59.382240 pycv_crossvalidation-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-21 12:20:54.000000 pycv_crossvalidation-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 12:33:59.363348 pycv_crossvalidation-0.0.2/pycv_crossvalidation/
--rw-rw-rw-   0        0        0    29056 2024-02-24 18:02:35.000000 pycv_crossvalidation-0.0.2/pycv_crossvalidation/CrossValidation.py
--rw-rw-rw-   0        0        0        0 2024-03-21 12:32:53.000000 pycv_crossvalidation-0.0.2/pycv_crossvalidation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:33:59.381026 pycv_crossvalidation-0.0.2/pycv_crossvalidation.egg-info/
--rw-rw-rw-   0        0        0      457 2024-03-21 12:33:59.000000 pycv_crossvalidation-0.0.2/pycv_crossvalidation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-03-21 12:33:59.000000 pycv_crossvalidation-0.0.2/pycv_crossvalidation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 12:33:59.000000 pycv_crossvalidation-0.0.2/pycv_crossvalidation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-03-21 12:33:59.000000 pycv_crossvalidation-0.0.2/pycv_crossvalidation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      157 2024-03-21 12:20:22.000000 pycv_crossvalidation-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      580 2024-03-21 12:33:59.384247 pycv_crossvalidation-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 05:27:56.163022 pycv_crossvalidation-0.0.3/
+-rw-rw-rw-   0        0        0     1103 2024-04-09 05:21:21.000000 pycv_crossvalidation-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     7144 2024-04-09 05:27:56.163022 pycv_crossvalidation-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6679 2024-04-09 05:17:23.000000 pycv_crossvalidation-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:27:56.145382 pycv_crossvalidation-0.0.3/pycv_crossvalidation/
+-rw-rw-rw-   0        0        0    29056 2024-02-24 18:02:35.000000 pycv_crossvalidation-0.0.3/pycv_crossvalidation/CrossValidation.py
+-rw-rw-rw-   0        0        0        0 2024-03-21 12:32:53.000000 pycv_crossvalidation-0.0.3/pycv_crossvalidation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:27:56.162014 pycv_crossvalidation-0.0.3/pycv_crossvalidation.egg-info/
+-rw-rw-rw-   0        0        0     7144 2024-04-09 05:27:56.000000 pycv_crossvalidation-0.0.3/pycv_crossvalidation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-04-09 05:27:56.000000 pycv_crossvalidation-0.0.3/pycv_crossvalidation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:27:56.000000 pycv_crossvalidation-0.0.3/pycv_crossvalidation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-09 05:27:56.000000 pycv_crossvalidation-0.0.3/pycv_crossvalidation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      157 2024-03-21 12:20:22.000000 pycv_crossvalidation-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      559 2024-04-09 05:27:56.165415 pycv_crossvalidation-0.0.3/setup.cfg
```

### Comparing `pycv_crossvalidation-0.0.2/pycv_crossvalidation/CrossValidation.py` & `pycv_crossvalidation-0.0.3/pycv_crossvalidation/CrossValidation.py`

 * *Files identical despite different names*

### Comparing `pycv_crossvalidation-0.0.2/setup.cfg` & `pycv_crossvalidation-0.0.3/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 765f 6372 6f73 7376 616c   = pycv_crossval
 00000020: 6964 6174 696f 6e0d 0a76 6572 7369 6f6e  idation..version
-00000030: 203d 2030 2e30 2e32 0d0a 6175 7468 6f72   = 0.0.2..author
+00000030: 203d 2030 2e30 2e33 0d0a 6175 7468 6f72   = 0.0.3..author
 00000040: 203d 2044 696f 676f 2041 706f 7374 6f6c   = Diogo Apostol
 00000050: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000060: 3d20 6f67 6f69 642e 3437 3840 676d 6169  = ogoid.478@gmai
 00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000080: 6f6e 203d 2050 7974 686f 6e20 5061 636b  on = Python Pack
 00000090: 6167 6520 666f 7220 4372 6f73 7320 5661  age for Cross Va
 000000a0: 6c69 6461 7469 6f6e 0d0a 6c6f 6e67 5f64  lidation..long_d
@@ -17,21 +17,19 @@
 00000100: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 00000110: 622e 636f 6d2f 4469 6f67 6f41 706f 7374  b.com/DiogoApost
 00000120: 6f6c 6f2f 7079 6376 0d0a 636c 6173 7369  olo/pycv..classi
 00000130: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
 00000140: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000150: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
 00000160: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000170: 4170 7072 6f76 6564 203a 3a20 474e 5520  Approved :: GNU 
-00000180: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000190: 6963 656e 7365 2028 4750 4c29 0d0a 094f  icense (GPL)...O
-000001a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000001b0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000001c0: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-000001d0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-000001e0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-000001f0: 7320 3d20 3e3d 332e 370d 0a69 6e63 6c75  s = >=3.7..inclu
-00000200: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000210: 3d20 5472 7565 0d0a 0d0a 5b65 6767 5f69  = True....[egg_i
-00000220: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000230: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000240: 0d0a 0d0a                                ....
+00000170: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000180: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000190: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001a0: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
+000001b0: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+000001c0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+000001d0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000001e0: 3d33 2e37 0d0a 696e 636c 7564 655f 7061  =3.7..include_pa
+000001f0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+00000200: 650d 0a0d 0a5b 6567 675f 696e 666f 5d0d  e....[egg_info].
+00000210: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000220: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

