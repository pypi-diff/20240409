# Comparing `tmp/pycol_complexity-0.0.3.tar.gz` & `tmp/pycol_complexity-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycol_complexity-0.0.3.tar", last modified: Thu Mar 21 06:41:51 2024, max compression
+gzip compressed data, was "pycol_complexity-0.0.4.tar", last modified: Tue Apr  9 05:30:16 2024, max compression
```

## Comparing `pycol_complexity-0.0.3.tar` & `pycol_complexity-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 06:41:51.143656 pycol_complexity-0.0.3/
--rw-rw-rw-   0        0        0     5563 2024-03-21 06:41:51.142660 pycol_complexity-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5104 2024-03-21 06:37:06.000000 pycol_complexity-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 06:41:51.097174 pycol_complexity-0.0.3/pycol_complexity/
--rw-rw-rw-   0        0        0        0 2024-03-21 03:21:50.000000 pycol_complexity-0.0.3/pycol_complexity/__init__.py
--rw-rw-rw-   0        0        0    93388 2024-03-21 04:47:59.000000 pycol_complexity-0.0.3/pycol_complexity/complexity.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:41:51.141658 pycol_complexity-0.0.3/pycol_complexity.egg-info/
--rw-rw-rw-   0        0        0     5563 2024-03-21 06:41:50.000000 pycol_complexity-0.0.3/pycol_complexity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-03-21 06:41:51.000000 pycol_complexity-0.0.3/pycol_complexity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 06:41:50.000000 pycol_complexity-0.0.3/pycol_complexity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-21 06:41:50.000000 pycol_complexity-0.0.3/pycol_complexity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2024-03-21 04:48:10.000000 pycol_complexity-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      580 2024-03-21 06:41:51.146002 pycol_complexity-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 05:30:16.000533 pycol_complexity-0.0.4/
+-rw-rw-rw-   0        0        0     1103 2024-04-09 05:21:21.000000 pycol_complexity-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5569 2024-04-09 05:30:15.999533 pycol_complexity-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2024-03-21 06:37:06.000000 pycol_complexity-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:30:15.983136 pycol_complexity-0.0.4/pycol_complexity/
+-rw-rw-rw-   0        0        0        0 2024-03-21 03:21:50.000000 pycol_complexity-0.0.4/pycol_complexity/__init__.py
+-rw-rw-rw-   0        0        0    93388 2024-03-21 04:47:59.000000 pycol_complexity-0.0.4/pycol_complexity/complexity.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:30:15.999533 pycol_complexity-0.0.4/pycol_complexity.egg-info/
+-rw-rw-rw-   0        0        0     5569 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      215 2024-03-21 04:48:10.000000 pycol_complexity-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      559 2024-04-09 05:30:16.001963 pycol_complexity-0.0.4/setup.cfg
```

### Comparing `pycol_complexity-0.0.3/PKG-INFO` & `pycol_complexity-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pycol_complexity
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Package for complexity measures
 Home-page: https://github.com/DiogoApostolo/pycol
 Author: Diogo Apostolo
 Author-email: ogoid.478@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 # pycol: Python Class Overlap Library
 
 The Python Class Overlap Library (`pycol`) assembles a set of data complexity measures associated to the problem of class overlap.
```

### Comparing `pycol_complexity-0.0.3/README.md` & `pycol_complexity-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pycol_complexity-0.0.3/pycol_complexity/complexity.py` & `pycol_complexity-0.0.4/pycol_complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `pycol_complexity-0.0.3/pycol_complexity.egg-info/PKG-INFO` & `pycol_complexity-0.0.4/pycol_complexity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pycol_complexity
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Package for complexity measures
 Home-page: https://github.com/DiogoApostolo/pycol
 Author: Diogo Apostolo
 Author-email: ogoid.478@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 # pycol: Python Class Overlap Library
 
 The Python Class Overlap Library (`pycol`) assembles a set of data complexity measures associated to the problem of class overlap.
```

### Comparing `pycol_complexity-0.0.3/setup.cfg` & `pycol_complexity-0.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 6f6c 5f63 6f6d 706c 6578   = pycol_complex
 00000020: 6974 790d 0a76 6572 7369 6f6e 203d 2030  ity..version = 0
-00000030: 2e30 2e33 0d0a 6175 7468 6f72 203d 2044  .0.3..author = D
+00000030: 2e30 2e34 0d0a 6175 7468 6f72 203d 2044  .0.4..author = D
 00000040: 696f 676f 2041 706f 7374 6f6c 6f0d 0a61  iogo Apostolo..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6f67  uthor_email = og
 00000060: 6f69 642e 3437 3840 676d 6169 6c2e 636f  oid.478@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2050 7974 686f 6e20 5061 636b 6167 6520   Python Package 
 00000090: 666f 7220 636f 6d70 6c65 7869 7479 206d  for complexity m
 000000a0: 6561 7375 7265 730d 0a6c 6f6e 675f 6465  easures..long_de
@@ -17,21 +17,19 @@
 00000100: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
 00000110: 2e63 6f6d 2f44 696f 676f 4170 6f73 746f  .com/DiogoAposto
 00000120: 6c6f 2f70 7963 6f6c 0d0a 636c 6173 7369  lo/pycol..classi
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

