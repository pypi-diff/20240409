# Comparing `tmp/kcwebplus-3.0.1.tar.gz` & `tmp/kcwebplus-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.1.tar", last modified: Mon Apr  8 15:22:40 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.2.tar", last modified: Tue Apr  9 12:10:11 2024, max compression
```

## Comparing `kcwebplus-3.0.1.tar` & `kcwebplus-3.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/common/
--rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/common/model.py
--rw-rw-rw-   0        0        0    18943 2024-04-04 04:18:15.000000 kcwebplus-3.0.1/kcwebplus/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/common/autoload.py
--rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/__init__.py
--rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/__init__.py
--rw-rw-rw-   0        0        0    12570 2024-04-08 15:11:11.000000 kcwebplus-3.0.1/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1014 2024-04-08 14:31:42.000000 kcwebplus-3.0.1/kcwebplus/server
--rw-rw-rw-   0        0        0      334 2024-04-08 15:21:11.000000 kcwebplus-3.0.1/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      358 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      141 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1480 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      450 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/LICENSE
--rw-rw-rw-   0        0        0      358 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-08 15:20:26.000000 kcwebplus-3.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2643 2024-04-08 15:22:24.000000 kcwebplus-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/common/
+-rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/common/model.py
+-rw-rw-rw-   0        0        0    18943 2024-04-04 04:18:15.000000 kcwebplus-3.0.2/kcwebplus/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/common/autoload.py
+-rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/controller/
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/index/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/controller/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/kcwebplus/index/__init__.py
+-rw-rw-rw-   0        0        0    12570 2024-04-08 15:11:11.000000 kcwebplus-3.0.2/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1014 2024-04-08 14:31:42.000000 kcwebplus-3.0.2/kcwebplus/server
+-rw-rw-rw-   0        0        0      334 2024-04-08 15:21:11.000000 kcwebplus-3.0.2/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-09 12:10:10.000000 kcwebplus-3.0.2/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-09 12:10:10.000000 kcwebplus-3.0.2/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      358 2024-04-09 12:10:10.000000 kcwebplus-3.0.2/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2024-04-09 12:10:10.000000 kcwebplus-3.0.2/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1480 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      450 2024-04-09 12:10:10.000000 kcwebplus-3.0.2/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0      358 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-08 15:20:26.000000 kcwebplus-3.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 12:10:11.000000 kcwebplus-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2643 2024-04-09 12:10:03.000000 kcwebplus-3.0.2/setup.py
```

### Comparing `kcwebplus-3.0.1/kcwebplus/common/model.py` & `kcwebplus-3.0.2/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/common/__init__.py` & `kcwebplus-3.0.2/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/config/__init__.py` & `kcwebplus-3.0.2/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0.2/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0.2/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0.2/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/kcwebplus.py` & `kcwebplus-3.0.2/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus/server` & `kcwebplus-3.0.2/kcwebplus/server`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0.2/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/LICENSE` & `kcwebplus-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/README.md` & `kcwebplus-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.1/setup.py` & `kcwebplus-3.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
 00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
 00000260: 6527 5d3d 276b 6377 6562 706c 7573 2720  e']='kcwebplus' 
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 2020 2020 23e9 a1b9              #...
 00000290: e79b aee7 9a84 e590 8de7 a7b0 200d 0a63  ............ ..c
 000002a0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000002b0: 5d3d 2733 2e30 2e31 2709 0909 0909 0909  ]='3.0.1'.......
+000002b0: 5d3d 2733 2e30 2e32 2709 0909 0909 0909  ]='3.0.2'.......
 000002c0: 23e9 a1b9 e79b aee7 8988 e69c ac0d 0a63  #..............c
 000002d0: 6f6e 666b 6377 5b27 6465 7363 7269 7074  onfkcw['descript
 000002e0: 696f 6e27 5d3d 27e8 afa5 e789 88e6 9cac  ion']='.........
 000002f0: e99c 8070 7974 686f 6ee7 8988 e69c ac3e  ...python......>
 00000300: 3d33 2e38 2720 2020 2020 2020 23e9 a1b9  =3.8'       #...
 00000310: e79b aee7 9a84 e7ae 80e5 8d95 e68f 8fe8  ................
 00000320: bfb0 0d0a 636f 6e66 6b63 775b 276c 6f6e  ....confkcw['lon
@@ -133,15 +133,15 @@
 00000840: 726c 275d 2c0d 0a20 2020 2070 6163 6b61  rl'],..    packa
 00000850: 6765 7320 3d20 2062 2c0d 0a20 2020 2023  ges =  b,..    #
 00000860: 2064 6174 615f 6669 6c65 733d 5b28 2753   data_files=[('S
 00000870: 6372 6970 7473 272c 205b 276b 6377 6562  cripts', ['kcweb
 00000880: 706c 7573 2f62 696e 2f6b 6377 2e65 7865  plus/bin/kcw.exe
 00000890: 275d 295d 2c0d 0a20 2020 2069 6e73 7461  '])],..    insta
 000008a0: 6c6c 5f72 6571 7569 7265 7320 3d20 5b27  ll_requires = ['
-000008b0: 6b63 7765 623e 3d35 2e32 3727 2c27 7079  kcweb>=5.27','py
+000008b0: 6b63 7765 623e 3d35 2e32 3827 2c27 7079  kcweb>=5.28','py
 000008c0: 4f70 656e 5353 4c3d 3d32 332e 322e 3027  OpenSSL==23.2.0'
 000008d0: 2c27 6368 6172 6465 743d 3d34 2e30 2e30  ,'chardet==4.0.0
 000008e0: 272c 2761 7073 6368 6564 756c 6572 3d3d  ','apscheduler==
 000008f0: 332e 362e 3327 2c27 7172 636f 6465 3d3d  3.6.3','qrcode==
 00000900: 362e 3127 2c27 7069 6c6c 6f77 3d3d 382e  6.1','pillow==8.
 00000910: 342e 3027 2c27 7073 7574 696c 3d3d 352e  4.0','psutil==5.
 00000920: 372e 3027 2c27 6f73 7332 3d3d 322e 3132  7.0','oss2==2.12
```

