# Comparing `tmp/kcwebplus-3.0.6.tar.gz` & `tmp/kcwebplus-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.6.tar", last modified: Tue Apr  9 16:00:14 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.7.tar", last modified: Tue Apr  9 16:19:15 2024, max compression
```

## Comparing `kcwebplus-3.0.6.tar` & `kcwebplus-3.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.934946 kcwebplus-3.0.6/
--rw-rw-rw-   0        0        0      344 2024-04-09 16:00:14.934008 kcwebplus-3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.906901 kcwebplus-3.0.6/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.917428 kcwebplus-3.0.6/kcwebplus/common/
--rw-rw-rw-   0        0        0    18682 2024-04-09 15:47:58.000000 kcwebplus-3.0.6/kcwebplus/common/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/common/model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.918429 kcwebplus-3.0.6/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.918429 kcwebplus-3.0.6/kcwebplus/index/
--rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.921476 kcwebplus-3.0.6/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/common/__init__.py
--rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/common/autoload.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.922467 kcwebplus-3.0.6/kcwebplus/index/controller/
--rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.924199 kcwebplus-3.0.6/kcwebplus/index/controller/index/
--rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.927432 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.901801 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.929432 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/server
--rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.913424 kcwebplus-3.0.6/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      177 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      450 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:00:14.935881 kcwebplus-3.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2683 2024-04-09 16:00:10.000000 kcwebplus-3.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.085853 kcwebplus-3.0.7/
+-rw-rw-rw-   0        0        0      344 2024-04-09 16:19:15.084853 kcwebplus-3.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.060856 kcwebplus-3.0.7/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.065913 kcwebplus-3.0.7/kcwebplus/common/
+-rw-rw-rw-   0        0        0    18682 2024-04-09 15:47:58.000000 kcwebplus-3.0.7/kcwebplus/common/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/common/model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.070356 kcwebplus-3.0.7/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.071356 kcwebplus-3.0.7/kcwebplus/index/
+-rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.072355 kcwebplus-3.0.7/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/common/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/common/autoload.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.073355 kcwebplus-3.0.7/kcwebplus/index/controller/
+-rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.075356 kcwebplus-3.0.7/kcwebplus/index/controller/index/
+-rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.077356 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.054928 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.081854 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/server
+-rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.065913 kcwebplus-3.0.7/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      163 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      450 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:19:15.085853 kcwebplus-3.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2746 2024-04-09 16:18:27.000000 kcwebplus-3.0.7/setup.py
```

### Comparing `kcwebplus-3.0.6/README.md` & `kcwebplus-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/common/__init__.py` & `kcwebplus-3.0.7/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/common/model.py` & `kcwebplus-3.0.7/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/config/__init__.py` & `kcwebplus-3.0.7/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0.7/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/kcwebplus.py` & `kcwebplus-3.0.7/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus/server` & `kcwebplus-3.0.7/kcwebplus/server`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0.7/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.6/setup.py` & `kcwebplus-3.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,168 +1,172 @@
-00000000: 0d0a 2320 7079 7468 6f6e 2073 6574 7570  ..# python setup
-00000010: 2e70 7920 7364 6973 7420 7570 6c6f 6164  .py sdist upload
-00000020: 0d0a 2320 7477 696e 6520 7570 6c6f 6164  ..# twine upload
-00000030: 202d 2d72 6570 6f73 6974 6f72 792d 7572   --repository-ur
-00000040: 6c20 6874 7470 733a 2f2f 7465 7374 2e70  l https://test.p
-00000050: 7970 692e 6f72 672f 6c65 6761 6379 2f20  ypi.org/legacy/ 
-00000060: 6469 7374 2f2a 2023 e4b8 8ae4 bca0 e588  dist/* #........
-00000070: b0e6 b58b e8af 950d 0a23 2070 6970 2069  .........# pip i
-00000080: 6e73 7461 6c6c 202d 2d69 6e64 6578 2d75  nstall --index-u
-00000090: 726c 2068 7474 7073 3a2f 2f70 7970 692e  rl https://pypi.
-000000a0: 6f72 672f 7369 6d70 6c65 2f20 6b63 7765  org/simple/ kcwe
-000000b0: 6220 2020 23e5 ae89 e8a3 85e6 b58b e8af  b   #...........
-000000c0: 95e6 9c8d e58a a1e4 b88a e79a 846b 6377  .............kcw
-000000d0: 6562 2070 6970 3320 696e 7374 616c 6c20  eb pip3 install 
-000000e0: 6b63 7765 623d 3d34 2e31 322e 3420 2d69  kcweb==4.12.4 -i
-000000f0: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
-00000100: 672f 7369 6d70 6c65 2f0d 0a23 2323 2323  g/simple/..#####
-00000110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000130: 2323 2323 2323 2323 200d 0a66 726f 6d20  ######## ..from 
-00000140: 7365 7475 7074 6f6f 6c73 2069 6d70 6f72  setuptools impor
-00000150: 7420 7365 7475 702c 2066 696e 645f 7061  t setup, find_pa
-00000160: 636b 6167 6573 2c45 7874 656e 7369 6f6e  ckages,Extension
-00000170: 0d0a 696d 706f 7274 206f 730d 0a64 6566  ..import os..def
-00000180: 2066 696c 655f 6765 745f 636f 6e74 656e   file_get_conten
-00000190: 7428 6b29 3a0d 0a20 2020 2022 e88e b7e5  t(k):..    "....
-000001a0: 8f96 e696 87e4 bbb6 e586 85e5 aeb9 220d  ..............".
-000001b0: 0a20 2020 2069 6620 6f73 2e70 6174 682e  .    if os.path.
-000001c0: 6973 6669 6c65 286b 293a 0d0a 2020 2020  isfile(k):..    
-000001d0: 2020 2020 663d 6f70 656e 286b 2c27 7227      f=open(k,'r'
-000001e0: 2c65 6e63 6f64 696e 673d 2275 7466 2d38  ,encoding="utf-8
-000001f0: 2229 0d0a 2020 2020 2020 2020 636f 6e3d  ")..        con=
-00000200: 662e 7265 6164 2829 0d0a 2020 2020 2020  f.read()..      
-00000210: 2020 662e 636c 6f73 6528 290d 0a20 2020    f.close()..   
-00000220: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000230: 636f 6e3d 2727 0d0a 2020 2020 7265 7475  con=''..    retu
-00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
-00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
-00000260: 6527 5d3d 276b 6377 6562 706c 7573 2720  e']='kcwebplus' 
-00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000280: 2020 2020 2020 2020 2020 2020 23e9 a1b9              #...
-00000290: e79b aee7 9a84 e590 8de7 a7b0 200d 0a63  ............ ..c
-000002a0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000002b0: 5d3d 2733 2e30 2e36 2709 0909 0909 0909  ]='3.0.6'.......
-000002c0: 23e9 a1b9 e79b aee7 8988 e69c ac0d 0a63  #..............c
-000002d0: 6f6e 666b 6377 5b27 6465 7363 7269 7074  onfkcw['descript
-000002e0: 696f 6e27 5d3d 27e8 afa5 e789 88e6 9cac  ion']='.........
-000002f0: e99c 8070 7974 686f 6ee7 8988 e69c ac3e  ...python......>
-00000300: 3d33 2e38 2720 2020 2020 2020 23e9 a1b9  =3.8'       #...
-00000310: e79b aee7 9a84 e7ae 80e5 8d95 e68f 8fe8  ................
-00000320: bfb0 0d0a 636f 6e66 6b63 775b 276c 6f6e  ....confkcw['lon
-00000330: 675f 6465 7363 7269 7074 696f 6e27 5d3d  g_description']=
-00000340: 22e8 afa5 e789 88e6 9cac e99c 8070 7974  "............pyt
-00000350: 686f 6ee7 8988 e69c ac3e 3d33 2e38 2220  hon......>=3.8" 
-00000360: 2020 2020 23e9 a1b9 e79b aee8 afa6 e7bb      #...........
-00000370: 86e6 8f8f e8bf b00d 0a63 6f6e 666b 6377  .........confkcw
-00000380: 5b27 6c69 6365 6e73 6527 5d3d 274d 4954  ['license']='MIT
-00000390: 204c 6963 656e 7365 2720 2020 2020 2020   License'       
-000003a0: 2020 2020 2020 2020 2020 2020 2023 e5bc               #..
-000003b0: 80e6 ba90 e58d 8fe8 aeae 2020 206d 6974  ..........   mit
-000003c0: e5bc 80e6 ba90 0d0a 636f 6e66 6b63 775b  ........confkcw[
-000003d0: 2775 726c 275d 3d27 270d 0a63 6f6e 666b  'url']=''..confk
-000003e0: 6377 5b27 6175 7468 6f72 275d 3d27 e799  cw['author']='..
-000003f0: bee9 878c 2de5 9da4 e59d a427 2020 0909  ....-......'  ..
-00000400: 0909 0920 23e5 908d e5ad 970d 0a63 6f6e  ... #........con
-00000410: 666b 6377 5b27 6175 7468 6f72 5f65 6d61  fkcw['author_ema
-00000420: 696c 275d 3d27 666b 3134 3032 3933 3635  il']='fk14029365
-00000430: 3334 4071 712e 636f 6d27 2009 2020 2020  34@qq.com' .    
-00000440: 2023 e982 aee4 bbb6 e59c b0e5 9d80 0d0a   #..............
-00000450: 636f 6e66 6b63 775b 276d 6169 6e74 6169  confkcw['maintai
-00000460: 6e65 7227 5d3d 27e5 9da4 e59d a427 2009  ner']='......' .
-00000470: 0909 0909 0920 23e7 bbb4 e68a a4e4 baba  ..... #.........
-00000480: e591 98e7 9a84 e590 8de5 ad97 0d0a 636f  ..............co
-00000490: 6e66 6b63 775b 276d 6169 6e74 6169 6e65  nfkcw['maintaine
-000004a0: 725f 656d 6169 6c27 5d3d 2766 6b31 3430  r_email']='fk140
-000004b0: 3239 3336 3533 3440 7171 2e63 6f6d 2720  2936534@qq.com' 
-000004c0: 2020 2023 e7bb b4e6 8aa4 e4ba bae5 9198     #............
-000004d0: e79a 84e9 82ae e4bb b6e5 9cb0 e59d 800d  ................
-000004e0: 0a64 6566 2067 6574 5f66 696c 6528 666f  .def get_file(fo
-000004f0: 6c64 6572 3d27 2e2f 272c 6c69 7374 733d  lder='./',lists=
-00000500: 5b5d 293a 0d0a 2020 2020 6c69 733d 6f73  []):..    lis=os
-00000510: 2e6c 6973 7464 6972 2866 6f6c 6465 7229  .listdir(folder)
-00000520: 0d0a 2020 2020 666f 7220 6669 6c65 7320  ..    for files 
-00000530: 696e 206c 6973 3a0d 0a20 2020 2020 2020  in lis:..       
-00000540: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
-00000550: 6973 6669 6c65 2866 6f6c 6465 722b 222f  isfile(folder+"/
-00000560: 222b 6669 6c65 7329 3a0d 0a20 2020 2020  "+files):..     
-00000570: 2020 2020 2020 2069 6620 6669 6c65 733d         if files=
-00000580: 3d27 5f5f 7079 6361 6368 655f 5f27 206f  ='__pycache__' o
-00000590: 7220 6669 6c65 733d 3d27 2e67 6974 273a  r files=='.git':
-000005a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000005b0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-000005c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000005d0: 2020 2020 2020 2020 2020 206c 6973 7473             lists
-000005e0: 2e61 7070 656e 6428 666f 6c64 6572 2b22  .append(folder+"
-000005f0: 2f22 2b66 696c 6573 290d 0a20 2020 2020  /"+files)..     
-00000600: 2020 2020 2020 2020 2020 2067 6574 5f66             get_f
-00000610: 696c 6528 666f 6c64 6572 2b22 2f22 2b66  ile(folder+"/"+f
-00000620: 696c 6573 2c6c 6973 7473 290d 0a20 2020  iles,lists)..   
-00000630: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000640: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-00000650: 2020 7265 7475 726e 206c 6973 7473 0d0a    return lists..
-00000660: 623d 6765 745f 6669 6c65 2822 6b63 7765  b=get_file("kcwe
-00000670: 6270 6c75 7322 2c5b 276b 6377 6562 706c  bplus",['kcwebpl
-00000680: 7573 275d 290d 0a73 6574 7570 280d 0a20  us'])..setup(.. 
-00000690: 2020 206e 616d 6520 3d20 636f 6e66 6b63     name = confkc
-000006a0: 775b 226e 616d 6522 5d2c 0d0a 2020 2020  w["name"],..    
-000006b0: 7665 7273 696f 6e20 3d20 636f 6e66 6b63  version = confkc
-000006c0: 775b 2276 6572 7369 6f6e 225d 2c0d 0a20  w["version"],.. 
-000006d0: 2020 206b 6579 776f 7264 7320 3d20 226b     keywords = "k
-000006e0: 6377 6562 706c 7573 222b 636f 6e66 6b63  cwebplus"+confkc
-000006f0: 775b 2776 6572 7369 6f6e 275d 2c0d 0a20  w['version'],.. 
-00000700: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
-00000710: 2063 6f6e 666b 6377 5b22 6465 7363 7269   confkcw["descri
-00000720: 7074 696f 6e22 5d2c 0d0a 2020 2020 6c6f  ption"],..    lo
-00000730: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-00000740: 2063 6f6e 666b 6377 5b22 6c6f 6e67 5f64   confkcw["long_d
-00000750: 6573 6372 6970 7469 6f6e 225d 2c0d 0a20  escription"],.. 
-00000760: 2020 206c 6963 656e 7365 203d 2063 6f6e     license = con
-00000770: 666b 6377 5b22 6c69 6365 6e73 6522 5d2c  fkcw["license"],
-00000780: 0d0a 2020 2020 6175 7468 6f72 203d 2063  ..    author = c
-00000790: 6f6e 666b 6377 5b22 6175 7468 6f72 225d  onfkcw["author"]
-000007a0: 2c0d 0a20 2020 2061 7574 686f 725f 656d  ,..    author_em
-000007b0: 6169 6c20 3d20 636f 6e66 6b63 775b 2261  ail = confkcw["a
-000007c0: 7574 686f 725f 656d 6169 6c22 5d2c 0d0a  uthor_email"],..
-000007d0: 2020 2020 6d61 696e 7461 696e 6572 203d      maintainer =
-000007e0: 2063 6f6e 666b 6377 5b22 6d61 696e 7461   confkcw["mainta
-000007f0: 696e 6572 225d 2c0d 0a20 2020 206d 6169  iner"],..    mai
-00000800: 6e74 6169 6e65 725f 656d 6169 6c20 3d20  ntainer_email = 
-00000810: 636f 6e66 6b63 775b 226d 6169 6e74 6169  confkcw["maintai
-00000820: 6e65 725f 656d 6169 6c22 5d2c 0d0a 2020  ner_email"],..  
-00000830: 2020 7572 6c3d 636f 6e66 6b63 775b 2775    url=confkcw['u
-00000840: 726c 275d 2c0d 0a20 2020 2070 6163 6b61  rl'],..    packa
-00000850: 6765 7320 3d20 2062 2c0d 0a20 2020 2023  ges =  b,..    #
-00000860: 2064 6174 615f 6669 6c65 733d 5b28 2753   data_files=[('S
-00000870: 6372 6970 7473 272c 205b 276b 6377 6562  cripts', ['kcweb
-00000880: 706c 7573 2f62 696e 2f6b 6377 2e65 7865  plus/bin/kcw.exe
-00000890: 275d 295d 2c0d 0a20 2020 2069 6e73 7461  '])],..    insta
-000008a0: 6c6c 5f72 6571 7569 7265 7320 3d20 5b27  ll_requires = ['
-000008b0: 6b63 7765 623e 3d35 2e32 3827 2c27 7069  kcweb>=5.28','pi
-000008c0: 6c6c 6f77 3d3d 3130 2e33 2e30 272c 2770  llow==10.3.0','p
-000008d0: 794f 7065 6e53 534c 3d3d 3233 2e32 2e30  yOpenSSL==23.2.0
-000008e0: 272c 2763 6861 7264 6574 3d3d 342e 302e  ','chardet==4.0.
-000008f0: 3027 2c27 6170 7363 6865 6475 6c65 723d  0','apscheduler=
-00000900: 3d33 2e36 2e33 272c 2771 7263 6f64 653d  =3.6.3','qrcode=
-00000910: 3d36 2e31 272c 2770 696c 6c6f 773d 3d39  =6.1','pillow==9
-00000920: 2e30 2e30 272c 2770 7375 7469 6c3e 3d35  .0.0','psutil>=5
-00000930: 2e38 2e30 272c 276f 7373 323e 3d32 2e31  .8.0','oss2>=2.1
-00000940: 322e 3127 2c27 7765 6273 6f63 6b65 742d  2.1','websocket-
-00000950: 636c 6965 6e74 3d3d 312e 332e 3127 2c27  client==1.3.1','
-00000960: 6372 7970 746f 6772 6170 6879 3d3d 3431  cryptography==41
-00000970: 2e30 2e37 275d 2c20 23e7 acac e4b8 89e6  .0.7'], #.......
-00000980: 96b9 e58c 850d 0a20 2020 2070 6163 6b61  .......    packa
-00000990: 6765 5f64 6174 6120 3d20 7b0d 0a20 2020  ge_data = {..   
-000009a0: 2020 2020 2027 273a 205b 272a 2e68 746d       '': ['*.htm
-000009b0: 6c27 2c20 272a 2e6a 7327 2c27 2a2e 6373  l', '*.js','*.cs
-000009c0: 7327 2c27 2a2e 6a70 6727 2c27 2a2e 706e  s','*.jpg','*.pn
-000009d0: 6727 2c27 2a2e 6769 6627 2c27 7365 7276  g','*.gif','serv
-000009e0: 6572 272c 2773 6572 7665 722e 7368 275d  er','server.sh']
-000009f0: 2c0d 0a20 2020 207d 2c0d 0a20 2020 2065  ,..    },..    e
-00000a00: 6e74 7279 5f70 6f69 6e74 7320 3d20 7b0d  ntry_points = {.
-00000a10: 0a20 2020 2020 2020 2027 636f 6e73 6f6c  .        'consol
-00000a20: 655f 7363 7269 7074 7327 3a5b 0d0a 2020  e_scripts':[..  
-00000a30: 2020 2020 2020 2020 2020 276b 6377 6562            'kcweb
-00000a40: 706c 7573 203d 206b 6377 6562 706c 7573  plus = kcwebplus
-00000a50: 2e6b 6377 6562 706c 7573 3a65 7865 6375  .kcwebplus:execu
-00000a60: 7461 626c 6527 0d0a 2020 2020 2020 2020  table'..        
-00000a70: 5d0d 0a20 2020 207d 0d0a 29              ]..    }..)
+00000000: 0d0a 2320 e689 93e5 8c85 e4b8 8ae4 bca0  ..# ............
+00000010: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000020: 2073 6469 7374 2075 706c 6f61 640d 0a23   sdist upload..#
+00000030: 20e6 8993 e58c 8520 7079 7468 6f6e 2073   ...... python s
+00000040: 6574 7570 2e70 7920 7364 6973 740d 0a23  etup.py sdist..#
+00000050: 2074 7769 6e65 2075 706c 6f61 6420 2d2d   twine upload --
+00000060: 7265 706f 7369 746f 7279 2d75 726c 2068  repository-url h
+00000070: 7474 7073 3a2f 2f74 6573 742e 7079 7069  ttps://test.pypi
+00000080: 2e6f 7267 2f6c 6567 6163 792f 2064 6973  .org/legacy/ dis
+00000090: 742f 2a20 23e4 b88a e4bc a0e5 88b0 e6b5  t/* #...........
+000000a0: 8be8 af95 0d0a 2320 7069 7020 696e 7374  ......# pip inst
+000000b0: 616c 6c20 2d2d 696e 6465 782d 7572 6c20  all --index-url 
+000000c0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000000d0: 2f73 696d 706c 652f 206b 6377 6562 2020  /simple/ kcweb  
+000000e0: 2023 e5ae 89e8 a385 e6b5 8be8 af95 e69c   #..............
+000000f0: 8de5 8aa1 e4b8 8ae7 9a84 6b63 7765 6220  ..........kcweb 
+00000100: 7069 7033 2069 6e73 7461 6c6c 206b 6377  pip3 install kcw
+00000110: 6562 3d3d 342e 3132 2e34 202d 6920 6874  eb==4.12.4 -i ht
+00000120: 7470 733a 2f2f 7079 7069 2e6f 7267 2f73  tps://pypi.org/s
+00000130: 696d 706c 652f 0d0a 2320 e5ae 89e8 a385  imple/..# ......
+00000140: 2070 7974 686f 6e20 7365 7475 702e 7079   python setup.py
+00000150: 2069 6e73 7461 6c6c 0d0a 2323 2323 2323   install..######
+00000160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000180: 2323 2323 2323 2320 0d0a 6672 6f6d 2073  ####### ..from s
+00000190: 6574 7570 746f 6f6c 7320 696d 706f 7274  etuptools import
+000001a0: 2073 6574 7570 2c20 6669 6e64 5f70 6163   setup, find_pac
+000001b0: 6b61 6765 732c 4578 7465 6e73 696f 6e0d  kages,Extension.
+000001c0: 0a69 6d70 6f72 7420 6f73 0d0a 6465 6620  .import os..def 
+000001d0: 6669 6c65 5f67 6574 5f63 6f6e 7465 6e74  file_get_content
+000001e0: 286b 293a 0d0a 2020 2020 22e8 8eb7 e58f  (k):..    ".....
+000001f0: 96e6 9687 e4bb b6e5 8685 e5ae b922 0d0a  ............."..
+00000200: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+00000210: 7366 696c 6528 6b29 3a0d 0a20 2020 2020  sfile(k):..     
+00000220: 2020 2066 3d6f 7065 6e28 6b2c 2772 272c     f=open(k,'r',
+00000230: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00000240: 290d 0a20 2020 2020 2020 2063 6f6e 3d66  )..        con=f
+00000250: 2e72 6561 6428 290d 0a20 2020 2020 2020  .read()..       
+00000260: 2066 2e63 6c6f 7365 2829 0d0a 2020 2020   f.close()..    
+00000270: 656c 7365 3a0d 0a20 2020 2020 2020 2063  else:..        c
+00000280: 6f6e 3d27 270d 0a20 2020 2072 6574 7572  on=''..    retur
+00000290: 6e20 636f 6e0d 0a63 6f6e 666b 6377 3d7b  n con..confkcw={
+000002a0: 7d0d 0a63 6f6e 666b 6377 5b27 6e61 6d65  }..confkcw['name
+000002b0: 275d 3d27 6b63 7765 6270 6c75 7327 2020  ']='kcwebplus'  
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 2020 2020 2020 2020 2020 2023 e9a1 b9e7             #....
+000002e0: 9bae e79a 84e5 908d e7a7 b020 0d0a 636f  ........... ..co
+000002f0: 6e66 6b63 775b 2776 6572 7369 6f6e 275d  nfkcw['version']
+00000300: 3d27 332e 302e 3727 0909 0909 0909 0923  ='3.0.7'.......#
+00000310: e9a1 b9e7 9bae e789 88e6 9cac 0d0a 636f  ..............co
+00000320: 6e66 6b63 775b 2764 6573 6372 6970 7469  nfkcw['descripti
+00000330: 6f6e 275d 3d27 e8af a5e7 8988 e69c ace9  on']='..........
+00000340: 9c80 7079 7468 6f6e e789 88e6 9cac 3e3d  ..python......>=
+00000350: 332e 3827 2020 2020 2020 2023 e9a1 b9e7  3.8'       #....
+00000360: 9bae e79a 84e7 ae80 e58d 95e6 8f8f e8bf  ................
+00000370: b00d 0a63 6f6e 666b 6377 5b27 6c6f 6e67  ...confkcw['long
+00000380: 5f64 6573 6372 6970 7469 6f6e 275d 3d22  _description']="
+00000390: e8af a5e7 8988 e69c ace9 9c80 7079 7468  ............pyth
+000003a0: 6f6e e789 88e6 9cac 3e3d 332e 3822 2020  on......>=3.8"  
+000003b0: 2020 2023 e9a1 b9e7 9bae e8af a6e7 bb86     #............
+000003c0: e68f 8fe8 bfb0 0d0a 636f 6e66 6b63 775b  ........confkcw[
+000003d0: 276c 6963 656e 7365 275d 3d27 4d49 5420  'license']='MIT 
+000003e0: 4c69 6365 6e73 6527 2020 2020 2020 2020  License'        
+000003f0: 2020 2020 2020 2020 2020 2020 23e5 bc80              #...
+00000400: e6ba 90e5 8d8f e8ae ae20 2020 6d69 74e5  .........   mit.
+00000410: bc80 e6ba 900d 0a63 6f6e 666b 6377 5b27  .......confkcw['
+00000420: 7572 6c27 5d3d 2727 0d0a 636f 6e66 6b63  url']=''..confkc
+00000430: 775b 2761 7574 686f 7227 5d3d 27e7 99be  w['author']='...
+00000440: e987 8c2d e59d a4e5 9da4 2720 2009 0909  ...-......'  ...
+00000450: 0909 2023 e590 8de5 ad97 0d0a 636f 6e66  .. #........conf
+00000460: 6b63 775b 2761 7574 686f 725f 656d 6169  kcw['author_emai
+00000470: 6c27 5d3d 2766 6b31 3430 3239 3336 3533  l']='fk140293653
+00000480: 3440 7171 2e63 6f6d 2720 0920 2020 2020  4@qq.com' .     
+00000490: 23e9 82ae e4bb b6e5 9cb0 e59d 800d 0a63  #..............c
+000004a0: 6f6e 666b 6377 5b27 6d61 696e 7461 696e  onfkcw['maintain
+000004b0: 6572 275d 3d27 e59d a4e5 9da4 2720 0909  er']='......' ..
+000004c0: 0909 0909 2023 e7bb b4e6 8aa4 e4ba bae5  .... #..........
+000004d0: 9198 e79a 84e5 908d e5ad 970d 0a63 6f6e  .............con
+000004e0: 666b 6377 5b27 6d61 696e 7461 696e 6572  fkcw['maintainer
+000004f0: 5f65 6d61 696c 275d 3d27 666b 3134 3032  _email']='fk1402
+00000500: 3933 3635 3334 4071 712e 636f 6d27 2020  936534@qq.com'  
+00000510: 2020 23e7 bbb4 e68a a4e4 baba e591 98e7    #.............
+00000520: 9a84 e982 aee4 bbb6 e59c b0e5 9d80 0d0a  ................
+00000530: 6465 6620 6765 745f 6669 6c65 2866 6f6c  def get_file(fol
+00000540: 6465 723d 272e 2f27 2c6c 6973 7473 3d5b  der='./',lists=[
+00000550: 5d29 3a0d 0a20 2020 206c 6973 3d6f 732e  ]):..    lis=os.
+00000560: 6c69 7374 6469 7228 666f 6c64 6572 290d  listdir(folder).
+00000570: 0a20 2020 2066 6f72 2066 696c 6573 2069  .    for files i
+00000580: 6e20 6c69 733a 0d0a 2020 2020 2020 2020  n lis:..        
+00000590: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
+000005a0: 7366 696c 6528 666f 6c64 6572 2b22 2f22  sfile(folder+"/"
+000005b0: 2b66 696c 6573 293a 0d0a 2020 2020 2020  +files):..      
+000005c0: 2020 2020 2020 6966 2066 696c 6573 3d3d        if files==
+000005d0: 275f 5f70 7963 6163 6865 5f5f 2720 6f72  '__pycache__' or
+000005e0: 2066 696c 6573 3d3d 272e 6769 7427 3a0d   files=='.git':.
+000005f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000600: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
+00000610: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000620: 2020 2020 2020 2020 2020 6c69 7374 732e            lists.
+00000630: 6170 7065 6e64 2866 6f6c 6465 722b 222f  append(folder+"/
+00000640: 222b 6669 6c65 7329 0d0a 2020 2020 2020  "+files)..      
+00000650: 2020 2020 2020 2020 2020 6765 745f 6669            get_fi
+00000660: 6c65 2866 6f6c 6465 722b 222f 222b 6669  le(folder+"/"+fi
+00000670: 6c65 732c 6c69 7374 7329 0d0a 2020 2020  les,lists)..    
+00000680: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000690: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
+000006a0: 2072 6574 7572 6e20 6c69 7374 730d 0a62   return lists..b
+000006b0: 3d67 6574 5f66 696c 6528 226b 6377 6562  =get_file("kcweb
+000006c0: 706c 7573 222c 5b27 6b63 7765 6270 6c75  plus",['kcwebplu
+000006d0: 7327 5d29 0d0a 7365 7475 7028 0d0a 2020  s'])..setup(..  
+000006e0: 2020 6e61 6d65 203d 2063 6f6e 666b 6377    name = confkcw
+000006f0: 5b22 6e61 6d65 225d 2c0d 0a20 2020 2076  ["name"],..    v
+00000700: 6572 7369 6f6e 203d 2063 6f6e 666b 6377  ersion = confkcw
+00000710: 5b22 7665 7273 696f 6e22 5d2c 0d0a 2020  ["version"],..  
+00000720: 2020 6b65 7977 6f72 6473 203d 2022 6b63    keywords = "kc
+00000730: 7765 6270 6c75 7322 2b63 6f6e 666b 6377  webplus"+confkcw
+00000740: 5b27 7665 7273 696f 6e27 5d2c 0d0a 2020  ['version'],..  
+00000750: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
+00000760: 636f 6e66 6b63 775b 2264 6573 6372 6970  confkcw["descrip
+00000770: 7469 6f6e 225d 2c0d 0a20 2020 206c 6f6e  tion"],..    lon
+00000780: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+00000790: 636f 6e66 6b63 775b 226c 6f6e 675f 6465  confkcw["long_de
+000007a0: 7363 7269 7074 696f 6e22 5d2c 0d0a 2020  scription"],..  
+000007b0: 2020 6c69 6365 6e73 6520 3d20 636f 6e66    license = conf
+000007c0: 6b63 775b 226c 6963 656e 7365 225d 2c0d  kcw["license"],.
+000007d0: 0a20 2020 2061 7574 686f 7220 3d20 636f  .    author = co
+000007e0: 6e66 6b63 775b 2261 7574 686f 7222 5d2c  nfkcw["author"],
+000007f0: 0d0a 2020 2020 6175 7468 6f72 5f65 6d61  ..    author_ema
+00000800: 696c 203d 2063 6f6e 666b 6377 5b22 6175  il = confkcw["au
+00000810: 7468 6f72 5f65 6d61 696c 225d 2c0d 0a20  thor_email"],.. 
+00000820: 2020 206d 6169 6e74 6169 6e65 7220 3d20     maintainer = 
+00000830: 636f 6e66 6b63 775b 226d 6169 6e74 6169  confkcw["maintai
+00000840: 6e65 7222 5d2c 0d0a 2020 2020 6d61 696e  ner"],..    main
+00000850: 7461 696e 6572 5f65 6d61 696c 203d 2063  tainer_email = c
+00000860: 6f6e 666b 6377 5b22 6d61 696e 7461 696e  onfkcw["maintain
+00000870: 6572 5f65 6d61 696c 225d 2c0d 0a20 2020  er_email"],..   
+00000880: 2075 726c 3d63 6f6e 666b 6377 5b27 7572   url=confkcw['ur
+00000890: 6c27 5d2c 0d0a 2020 2020 7061 636b 6167  l'],..    packag
+000008a0: 6573 203d 2020 622c 0d0a 2020 2020 2320  es =  b,..    # 
+000008b0: 6461 7461 5f66 696c 6573 3d5b 2827 5363  data_files=[('Sc
+000008c0: 7269 7074 7327 2c20 5b27 6b63 7765 6270  ripts', ['kcwebp
+000008d0: 6c75 732f 6269 6e2f 6b63 772e 6578 6527  lus/bin/kcw.exe'
+000008e0: 5d29 5d2c 0d0a 2020 2020 696e 7374 616c  ])],..    instal
+000008f0: 6c5f 7265 7175 6972 6573 203d 205b 276b  l_requires = ['k
+00000900: 6377 6562 3e3d 352e 3330 272c 2770 794f  cweb>=5.30','pyO
+00000910: 7065 6e53 534c 3d3d 3233 2e32 2e30 272c  penSSL==23.2.0',
+00000920: 2763 6861 7264 6574 3d3d 342e 302e 3027  'chardet==4.0.0'
+00000930: 2c27 6170 7363 6865 6475 6c65 723d 3d33  ,'apscheduler==3
+00000940: 2e36 2e33 272c 2771 7263 6f64 653d 3d36  .6.3','qrcode==6
+00000950: 2e31 272c 2770 696c 6c6f 773d 3d31 302e  .1','pillow==10.
+00000960: 302e 3027 2c27 7073 7574 696c 3d3d 352e  0.0','psutil==5.
+00000970: 382e 3027 2c27 6f73 7332 3e3d 322e 3132  8.0','oss2>=2.12
+00000980: 2e31 272c 2777 6562 736f 636b 6574 2d63  .1','websocket-c
+00000990: 6c69 656e 743d 3d31 2e33 2e31 272c 2763  lient==1.3.1','c
+000009a0: 7279 7074 6f67 7261 7068 793d 3d34 312e  ryptography==41.
+000009b0: 302e 3727 5d2c 2023 e7ac ace4 b889 e696  0.7'], #........
+000009c0: b9e5 8c85 0d0a 2020 2020 7061 636b 6167  ......    packag
+000009d0: 655f 6461 7461 203d 207b 0d0a 2020 2020  e_data = {..    
+000009e0: 2020 2020 2727 3a20 5b27 2a2e 6874 6d6c      '': ['*.html
+000009f0: 272c 2027 2a2e 6a73 272c 272a 2e63 7373  ', '*.js','*.css
+00000a00: 272c 272a 2e6a 7067 272c 272a 2e70 6e67  ','*.jpg','*.png
+00000a10: 272c 272a 2e67 6966 272c 2773 6572 7665  ','*.gif','serve
+00000a20: 7227 2c27 7365 7276 6572 2e73 6827 5d2c  r','server.sh'],
+00000a30: 0d0a 2020 2020 7d2c 0d0a 2020 2020 656e  ..    },..    en
+00000a40: 7472 795f 706f 696e 7473 203d 207b 0d0a  try_points = {..
+00000a50: 2020 2020 2020 2020 2763 6f6e 736f 6c65          'console
+00000a60: 5f73 6372 6970 7473 273a 5b0d 0a20 2020  _scripts':[..   
+00000a70: 2020 2020 2020 2020 2027 6b63 7765 6270           'kcwebp
+00000a80: 6c75 7320 3d20 6b63 7765 6270 6c75 732e  lus = kcwebplus.
+00000a90: 6b63 7765 6270 6c75 733a 6578 6563 7574  kcwebplus:execut
+00000aa0: 6162 6c65 270d 0a20 2020 2020 2020 205d  able'..        ]
+00000ab0: 0d0a 2020 2020 7d0d 0a29                 ..    }..)
```

