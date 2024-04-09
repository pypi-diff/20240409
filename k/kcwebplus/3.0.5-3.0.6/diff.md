# Comparing `tmp/kcwebplus-3.0.5.tar.gz` & `tmp/kcwebplus-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.5.tar", last modified: Tue Apr  9 14:22:17 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.6.tar", last modified: Tue Apr  9 16:00:14 2024, max compression
```

## Comparing `kcwebplus-3.0.5.tar` & `kcwebplus-3.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.082233 kcwebplus-3.0.5/
--rw-rw-rw-   0        0        0      344 2024-04-09 14:22:17.081233 kcwebplus-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.046233 kcwebplus-3.0.5/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.060232 kcwebplus-3.0.5/kcwebplus/common/
--rw-rw-rw-   0        0        0    18943 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/common/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/common/model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.061270 kcwebplus-3.0.5/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.064233 kcwebplus-3.0.5/kcwebplus/index/
--rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.066234 kcwebplus-3.0.5/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/common/__init__.py
--rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/common/autoload.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.067235 kcwebplus-3.0.5/kcwebplus/index/controller/
--rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.070233 kcwebplus-3.0.5/kcwebplus/index/controller/index/
--rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.074233 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.040233 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.077232 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/server
--rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.5/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 14:22:17.056234 kcwebplus-3.0.5/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2024-04-09 14:22:17.000000 kcwebplus-3.0.5/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      162 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      450 2024-04-09 14:22:16.000000 kcwebplus-3.0.5/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 14:22:17.082233 kcwebplus-3.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2666 2024-04-09 14:22:14.000000 kcwebplus-3.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.934946 kcwebplus-3.0.6/
+-rw-rw-rw-   0        0        0      344 2024-04-09 16:00:14.934008 kcwebplus-3.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.906901 kcwebplus-3.0.6/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.917428 kcwebplus-3.0.6/kcwebplus/common/
+-rw-rw-rw-   0        0        0    18682 2024-04-09 15:47:58.000000 kcwebplus-3.0.6/kcwebplus/common/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/common/model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.918429 kcwebplus-3.0.6/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.918429 kcwebplus-3.0.6/kcwebplus/index/
+-rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.921476 kcwebplus-3.0.6/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/common/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/common/autoload.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.922467 kcwebplus-3.0.6/kcwebplus/index/controller/
+-rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.924199 kcwebplus-3.0.6/kcwebplus/index/controller/index/
+-rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.927432 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.901801 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.929432 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/server
+-rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.6/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:14.913424 kcwebplus-3.0.6/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      450 2024-04-09 16:00:14.000000 kcwebplus-3.0.6/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:00:14.935881 kcwebplus-3.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2683 2024-04-09 16:00:10.000000 kcwebplus-3.0.6/setup.py
```

### Comparing `kcwebplus-3.0.5/README.md` & `kcwebplus-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/common/__init__.py` & `kcwebplus-3.0.6/kcwebplus/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     param={}
     for i in sorted (params) : 
         param[i]=params[i]
     i=0
     strs=""
     for k in param:
         if k:
-            use mysql;flush privileges;update user set host = '%' where user ='root';ALTER USER 'root'@'%' IDENTIFIED BY 'resgsgrsegrgesr' PASSWORD EXPIRE NEVER;ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY 'resgsgrsegrgesr';flush privileges;
             if isinstance(k,dict):
                 k=json_encode(k)
                 k=k.replace('"', '')
                 k=k.replace("'", '')
             if param[k]:
                 if i==0:
                     strs+=str(k)+"="+str(param[k])
```

### Comparing `kcwebplus-3.0.5/kcwebplus/common/model.py` & `kcwebplus-3.0.6/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/config/__init__.py` & `kcwebplus-3.0.6/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0.6/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0.6/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/kcwebplus.py` & `kcwebplus-3.0.6/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus/server` & `kcwebplus-3.0.6/kcwebplus/server`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0.6/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.5/setup.py` & `kcwebplus-3.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
 00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
 00000260: 6527 5d3d 276b 6377 6562 706c 7573 2720  e']='kcwebplus' 
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 2020 2020 23e9 a1b9              #...
 00000290: e79b aee7 9a84 e590 8de7 a7b0 200d 0a63  ............ ..c
 000002a0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000002b0: 5d3d 2733 2e30 2e35 2709 0909 0909 0909  ]='3.0.5'.......
+000002b0: 5d3d 2733 2e30 2e36 2709 0909 0909 0909  ]='3.0.6'.......
 000002c0: 23e9 a1b9 e79b aee7 8988 e69c ac0d 0a63  #..............c
 000002d0: 6f6e 666b 6377 5b27 6465 7363 7269 7074  onfkcw['descript
 000002e0: 696f 6e27 5d3d 27e8 afa5 e789 88e6 9cac  ion']='.........
 000002f0: e99c 8070 7974 686f 6ee7 8988 e69c ac3e  ...python......>
 00000300: 3d33 2e38 2720 2020 2020 2020 23e9 a1b9  =3.8'       #...
 00000310: e79b aee7 9a84 e7ae 80e5 8d95 e68f 8fe8  ................
 00000320: bfb0 0d0a 636f 6e66 6b63 775b 276c 6f6e  ....confkcw['lon
@@ -133,35 +133,36 @@
 00000840: 726c 275d 2c0d 0a20 2020 2070 6163 6b61  rl'],..    packa
 00000850: 6765 7320 3d20 2062 2c0d 0a20 2020 2023  ges =  b,..    #
 00000860: 2064 6174 615f 6669 6c65 733d 5b28 2753   data_files=[('S
 00000870: 6372 6970 7473 272c 205b 276b 6377 6562  cripts', ['kcweb
 00000880: 706c 7573 2f62 696e 2f6b 6377 2e65 7865  plus/bin/kcw.exe
 00000890: 275d 295d 2c0d 0a20 2020 2069 6e73 7461  '])],..    insta
 000008a0: 6c6c 5f72 6571 7569 7265 7320 3d20 5b27  ll_requires = ['
-000008b0: 6b63 7765 623e 3d35 2e32 3827 2c27 7079  kcweb>=5.28','py
-000008c0: 4f70 656e 5353 4c3d 3d32 332e 322e 3027  OpenSSL==23.2.0'
-000008d0: 2c27 6368 6172 6465 743d 3d34 2e30 2e30  ,'chardet==4.0.0
-000008e0: 272c 2761 7073 6368 6564 756c 6572 3d3d  ','apscheduler==
-000008f0: 332e 362e 3327 2c27 7172 636f 6465 3d3d  3.6.3','qrcode==
-00000900: 362e 3127 2c27 7069 6c6c 6f77 3d3d 382e  6.1','pillow==8.
-00000910: 342e 3027 2c27 7073 7574 696c 3d3d 352e  4.0','psutil==5.
-00000920: 372e 3027 2c27 6f73 7332 3d3d 322e 3132  7.0','oss2==2.12
-00000930: 2e31 272c 2777 6562 736f 636b 6574 2d63  .1','websocket-c
-00000940: 6c69 656e 743d 3d31 2e33 2e31 272c 2763  lient==1.3.1','c
-00000950: 7279 7074 6f67 7261 7068 793d 3d34 312e  ryptography==41.
-00000960: 302e 3727 5d2c 2023 e7ac ace4 b889 e696  0.7'], #........
-00000970: b9e5 8c85 0d0a 2020 2020 7061 636b 6167  ......    packag
-00000980: 655f 6461 7461 203d 207b 0d0a 2020 2020  e_data = {..    
-00000990: 2020 2020 2727 3a20 5b27 2a2e 6874 6d6c      '': ['*.html
-000009a0: 272c 2027 2a2e 6a73 272c 272a 2e63 7373  ', '*.js','*.css
-000009b0: 272c 272a 2e6a 7067 272c 272a 2e70 6e67  ','*.jpg','*.png
-000009c0: 272c 272a 2e67 6966 272c 2773 6572 7665  ','*.gif','serve
-000009d0: 7227 2c27 7365 7276 6572 2e73 6827 5d2c  r','server.sh'],
-000009e0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 656e  ..    },..    en
-000009f0: 7472 795f 706f 696e 7473 203d 207b 0d0a  try_points = {..
-00000a00: 2020 2020 2020 2020 2763 6f6e 736f 6c65          'console
-00000a10: 5f73 6372 6970 7473 273a 5b0d 0a20 2020  _scripts':[..   
-00000a20: 2020 2020 2020 2020 2027 6b63 7765 6270           'kcwebp
-00000a30: 6c75 7320 3d20 6b63 7765 6270 6c75 732e  lus = kcwebplus.
-00000a40: 6b63 7765 6270 6c75 733a 6578 6563 7574  kcwebplus:execut
-00000a50: 6162 6c65 270d 0a20 2020 2020 2020 205d  able'..        ]
-00000a60: 0d0a 2020 2020 7d0d 0a29                 ..    }..)
+000008b0: 6b63 7765 623e 3d35 2e32 3827 2c27 7069  kcweb>=5.28','pi
+000008c0: 6c6c 6f77 3d3d 3130 2e33 2e30 272c 2770  llow==10.3.0','p
+000008d0: 794f 7065 6e53 534c 3d3d 3233 2e32 2e30  yOpenSSL==23.2.0
+000008e0: 272c 2763 6861 7264 6574 3d3d 342e 302e  ','chardet==4.0.
+000008f0: 3027 2c27 6170 7363 6865 6475 6c65 723d  0','apscheduler=
+00000900: 3d33 2e36 2e33 272c 2771 7263 6f64 653d  =3.6.3','qrcode=
+00000910: 3d36 2e31 272c 2770 696c 6c6f 773d 3d39  =6.1','pillow==9
+00000920: 2e30 2e30 272c 2770 7375 7469 6c3e 3d35  .0.0','psutil>=5
+00000930: 2e38 2e30 272c 276f 7373 323e 3d32 2e31  .8.0','oss2>=2.1
+00000940: 322e 3127 2c27 7765 6273 6f63 6b65 742d  2.1','websocket-
+00000950: 636c 6965 6e74 3d3d 312e 332e 3127 2c27  client==1.3.1','
+00000960: 6372 7970 746f 6772 6170 6879 3d3d 3431  cryptography==41
+00000970: 2e30 2e37 275d 2c20 23e7 acac e4b8 89e6  .0.7'], #.......
+00000980: 96b9 e58c 850d 0a20 2020 2070 6163 6b61  .......    packa
+00000990: 6765 5f64 6174 6120 3d20 7b0d 0a20 2020  ge_data = {..   
+000009a0: 2020 2020 2027 273a 205b 272a 2e68 746d       '': ['*.htm
+000009b0: 6c27 2c20 272a 2e6a 7327 2c27 2a2e 6373  l', '*.js','*.cs
+000009c0: 7327 2c27 2a2e 6a70 6727 2c27 2a2e 706e  s','*.jpg','*.pn
+000009d0: 6727 2c27 2a2e 6769 6627 2c27 7365 7276  g','*.gif','serv
+000009e0: 6572 272c 2773 6572 7665 722e 7368 275d  er','server.sh']
+000009f0: 2c0d 0a20 2020 207d 2c0d 0a20 2020 2065  ,..    },..    e
+00000a00: 6e74 7279 5f70 6f69 6e74 7320 3d20 7b0d  ntry_points = {.
+00000a10: 0a20 2020 2020 2020 2027 636f 6e73 6f6c  .        'consol
+00000a20: 655f 7363 7269 7074 7327 3a5b 0d0a 2020  e_scripts':[..  
+00000a30: 2020 2020 2020 2020 2020 276b 6377 6562            'kcweb
+00000a40: 706c 7573 203d 206b 6377 6562 706c 7573  plus = kcwebplus
+00000a50: 2e6b 6377 6562 706c 7573 3a65 7865 6375  .kcwebplus:execu
+00000a60: 7461 626c 6527 0d0a 2020 2020 2020 2020  table'..        
+00000a70: 5d0d 0a20 2020 207d 0d0a 29              ]..    }..)
```

