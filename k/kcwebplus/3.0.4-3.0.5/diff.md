# Comparing `tmp/kcwebplus-3.0.4.tar.gz` & `tmp/kcwebplus-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.4.tar", last modified: Tue Apr  9 14:07:11 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.5.tar", last modified: Tue Apr  9 14:22:17 2024, max compression
```

## Comparing `kcwebplus-3.0.4.tar` & `kcwebplus-3.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.509375 kcwebplus-3.0.4/
--rw-rw-rw-   0        0        0      344 2024-04-09 14:07:11.507372 kcwebplus-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.473374 kcwebplus-3.0.4/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.487376 kcwebplus-3.0.4/kcwebplus/common/
--rw-rw-rw-   0        0        0    18943 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/common/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/common/model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.488374 kcwebplus-3.0.4/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.489375 kcwebplus-3.0.4/kcwebplus/index/
--rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.492373 kcwebplus-3.0.4/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/common/__init__.py
--rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/common/autoload.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.493374 kcwebplus-3.0.4/kcwebplus/index/controller/
--rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.495373 kcwebplus-3.0.4/kcwebplus/index/controller/index/
--rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.499374 kcwebplus-3.0.4/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.467375 kcwebplus-3.0.4/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.502374 kcwebplus-3.0.4/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/server
--rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.4/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 14:07:11.484450 kcwebplus-3.0.4/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 14:07:11.000000 kcwebplus-3.0.4/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2024-04-09 14:07:11.000000 kcwebplus-3.0.4/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:07:11.000000 kcwebplus-3.0.4/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-09 14:07:11.000000 kcwebplus-3.0.4/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      162 2024-04-09 14:07:11.000000 kcwebplus-3.0.4/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      450 2024-04-09 14:07:11.000000 kcwebplus-3.0.4/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 14:07:11.510375 kcwebplus-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2666 2024-04-09 14:07:09.000000 kcwebplus-3.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.082233 kcwebplus-3.0.5/
+-rw-rw-rw-   0        0        0      344 2024-04-09 14:22:17.081233 kcwebplus-3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.046233 kcwebplus-3.0.5/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.060232 kcwebplus-3.0.5/kcwebplus/common/
+-rw-rw-rw-   0        0        0    18943 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/common/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/common/model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.061270 kcwebplus-3.0.5/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.064233 kcwebplus-3.0.5/kcwebplus/index/
+-rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.066234 kcwebplus-3.0.5/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/common/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/common/autoload.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.067235 kcwebplus-3.0.5/kcwebplus/index/controller/
+-rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.070233 kcwebplus-3.0.5/kcwebplus/index/controller/index/
+-rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.074233 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.040233 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.077232 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/server
+-rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.056234 kcwebplus-3.0.5/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-04-09 14:22:17.000000 kcwebplus-3.0.5/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      162 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      450 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:22:17.082233 kcwebplus-3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2666 2024-04-09 14:22:14.000000 kcwebplus-3.0.5/setup.py
```

### Comparing `kcwebplus-3.0.4/README.md` & `kcwebplus-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/common/__init__.py` & `kcwebplus-3.0.5/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/common/model.py` & `kcwebplus-3.0.5/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/config/__init__.py` & `kcwebplus-3.0.5/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0.5/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/kcwebplus.py` & `kcwebplus-3.0.5/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus/server` & `kcwebplus-3.0.5/kcwebplus/server`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0.5/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.4/setup.py` & `kcwebplus-3.0.5/setup.py`

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
-000002b0: 5d3d 2733 2e30 2e34 2709 0909 0909 0909  ]='3.0.4'.......
+000002b0: 5d3d 2733 2e30 2e35 2709 0909 0909 0909  ]='3.0.5'.......
 000002c0: 23e9 a1b9 e79b aee7 8988 e69c ac0d 0a63  #..............c
 000002d0: 6f6e 666b 6377 5b27 6465 7363 7269 7074  onfkcw['descript
 000002e0: 696f 6e27 5d3d 27e8 afa5 e789 88e6 9cac  ion']='.........
 000002f0: e99c 8070 7974 686f 6ee7 8988 e69c ac3e  ...python......>
 00000300: 3d33 2e38 2720 2020 2020 2020 23e9 a1b9  =3.8'       #...
 00000310: e79b aee7 9a84 e7ae 80e5 8d95 e68f 8fe8  ................
 00000320: bfb0 0d0a 636f 6e66 6b63 775b 276c 6f6e  ....confkcw['lon
@@ -143,16 +143,16 @@
 000008e0: 272c 2761 7073 6368 6564 756c 6572 3d3d  ','apscheduler==
 000008f0: 332e 362e 3327 2c27 7172 636f 6465 3d3d  3.6.3','qrcode==
 00000900: 362e 3127 2c27 7069 6c6c 6f77 3d3d 382e  6.1','pillow==8.
 00000910: 342e 3027 2c27 7073 7574 696c 3d3d 352e  4.0','psutil==5.
 00000920: 372e 3027 2c27 6f73 7332 3d3d 322e 3132  7.0','oss2==2.12
 00000930: 2e31 272c 2777 6562 736f 636b 6574 2d63  .1','websocket-c
 00000940: 6c69 656e 743d 3d31 2e33 2e31 272c 2763  lient==1.3.1','c
-00000950: 7279 7074 6f67 7261 7068 793d 3d34 322e  ryptography==42.
-00000960: 302e 3527 5d2c 2023 e7ac ace4 b889 e696  0.5'], #........
+00000950: 7279 7074 6f67 7261 7068 793d 3d34 312e  ryptography==41.
+00000960: 302e 3727 5d2c 2023 e7ac ace4 b889 e696  0.7'], #........
 00000970: b9e5 8c85 0d0a 2020 2020 7061 636b 6167  ......    packag
 00000980: 655f 6461 7461 203d 207b 0d0a 2020 2020  e_data = {..    
 00000990: 2020 2020 2727 3a20 5b27 2a2e 6874 6d6c      '': ['*.html
 000009a0: 272c 2027 2a2e 6a73 272c 272a 2e63 7373  ', '*.js','*.css
 000009b0: 272c 272a 2e6a 7067 272c 272a 2e70 6e67  ','*.jpg','*.png
 000009c0: 272c 272a 2e67 6966 272c 2773 6572 7665  ','*.gif','serve
 000009d0: 7227 2c27 7365 7276 6572 2e73 6827 5d2c  r','server.sh'],
```

