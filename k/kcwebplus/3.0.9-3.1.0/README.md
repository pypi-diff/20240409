# Comparing `tmp/kcwebplus-3.0.9.tar.gz` & `tmp/kcwebplus-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.9.tar", last modified: Tue Apr  9 16:43:03 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.1.0.tar", last modified: Tue Apr  9 19:51:52 2024, max compression
```

## Comparing `kcwebplus-3.0.9.tar` & `kcwebplus-3.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.116831 kcwebplus-3.0.9/
--rw-rw-rw-   0        0        0      344 2024-04-09 16:43:03.115875 kcwebplus-3.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.084795 kcwebplus-3.0.9/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.095795 kcwebplus-3.0.9/kcwebplus/common/
--rw-rw-rw-   0        0        0    18682 2024-04-09 16:36:59.000000 kcwebplus-3.0.9/kcwebplus/common/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/common/model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.096795 kcwebplus-3.0.9/kcwebplus/config/
--rw-rw-rw-   0        0        0      646 2024-04-09 16:40:19.000000 kcwebplus-3.0.9/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.098795 kcwebplus-3.0.9/kcwebplus/index/
--rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.100796 kcwebplus-3.0.9/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/common/__init__.py
--rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/common/autoload.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.102800 kcwebplus-3.0.9/kcwebplus/index/controller/
--rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.104796 kcwebplus-3.0.9/kcwebplus/index/controller/index/
--rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.108797 kcwebplus-3.0.9/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.079807 kcwebplus-3.0.9/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.111798 kcwebplus-3.0.9/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.9/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1014 2024-04-09 16:23:31.000000 kcwebplus-3.0.9/kcwebplus/server
--rw-rw-rw-   0        0        0      334 2024-04-09 16:23:25.000000 kcwebplus-3.0.9/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 16:43:03.091795 kcwebplus-3.0.9/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 16:43:03.000000 kcwebplus-3.0.9/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2024-04-09 16:43:03.000000 kcwebplus-3.0.9/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:43:03.000000 kcwebplus-3.0.9/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-09 16:43:03.000000 kcwebplus-3.0.9/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      163 2024-04-09 16:43:03.000000 kcwebplus-3.0.9/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      450 2024-04-09 16:43:03.000000 kcwebplus-3.0.9/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:43:03.116831 kcwebplus-3.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2746 2024-04-09 16:40:07.000000 kcwebplus-3.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.827155 kcwebplus-3.1.0/
+-rw-rw-rw-   0        0        0      344 2024-04-09 19:51:52.826158 kcwebplus-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.791163 kcwebplus-3.1.0/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.803156 kcwebplus-3.1.0/kcwebplus/common/
+-rw-rw-rw-   0        0        0    18682 2024-04-09 16:36:59.000000 kcwebplus-3.1.0/kcwebplus/common/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/common/model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.805157 kcwebplus-3.1.0/kcwebplus/config/
+-rw-rw-rw-   0        0        0      646 2024-04-09 19:51:49.000000 kcwebplus-3.1.0/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.805157 kcwebplus-3.1.0/kcwebplus/index/
+-rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.810155 kcwebplus-3.1.0/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/common/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/common/autoload.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.811156 kcwebplus-3.1.0/kcwebplus/index/controller/
+-rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.814156 kcwebplus-3.1.0/kcwebplus/index/controller/index/
+-rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.819158 kcwebplus-3.1.0/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.784155 kcwebplus-3.1.0/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.822158 kcwebplus-3.1.0/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.1.0/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1014 2024-04-09 16:23:31.000000 kcwebplus-3.1.0/kcwebplus/server
+-rw-rw-rw-   0        0        0      334 2024-04-09 16:23:25.000000 kcwebplus-3.1.0/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:52.800205 kcwebplus-3.1.0/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 19:51:52.000000 kcwebplus-3.1.0/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-04-09 19:51:52.000000 kcwebplus-3.1.0/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 19:51:52.000000 kcwebplus-3.1.0/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-09 19:51:52.000000 kcwebplus-3.1.0/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      151 2024-04-09 19:51:52.000000 kcwebplus-3.1.0/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      450 2024-04-09 19:51:52.000000 kcwebplus-3.1.0/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 19:51:52.827155 kcwebplus-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2732 2024-04-09 19:51:40.000000 kcwebplus-3.1.0/setup.py
```

### Comparing `kcwebplus-3.0.9/README.md` & `kcwebplus-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/common/__init__.py` & `kcwebplus-3.1.0/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/common/model.py` & `kcwebplus-3.1.0/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/config/__init__.py` & `kcwebplus-3.1.0/kcwebplus/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from kcweb.config import *
 kcwebplus={}
 kcwebplus['name']='kcwebplus'                             #项目的名称
-kcwebplus['version']='3.0.9'							#项目版本
+kcwebplus['version']='3.1.0'							#项目版本
 kcwebplus['description']=''       #项目的简单描述
 kcwebplus['long_description']=''     #项目详细描述
 kcwebplus['license']='MIT'                    #开源协议   mit开源
 kcwebplus['url']=''
 kcwebplus['author']='百里-坤坤'  					 #名字
 kcwebplus['author_email']='fk1402936534@qq.com' 	     #邮件地址
 kcwebplus['maintainer']='坤坤' 						 #维护人员的名字
```

### Comparing `kcwebplus-3.0.9/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.1.0/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.1.0/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.1.0/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/kcwebplus.py` & `kcwebplus-3.1.0/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus/server` & `kcwebplus-3.1.0/kcwebplus/server`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.1.0/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.9/setup.py` & `kcwebplus-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 00000290: 6e20 636f 6e0d 0a63 6f6e 666b 6377 3d7b  n con..confkcw={
 000002a0: 7d0d 0a63 6f6e 666b 6377 5b27 6e61 6d65  }..confkcw['name
 000002b0: 275d 3d27 6b63 7765 6270 6c75 7327 2020  ']='kcwebplus'  
 000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002d0: 2020 2020 2020 2020 2020 2023 e9a1 b9e7             #....
 000002e0: 9bae e79a 84e5 908d e7a7 b020 0d0a 636f  ........... ..co
 000002f0: 6e66 6b63 775b 2776 6572 7369 6f6e 275d  nfkcw['version']
-00000300: 3d27 332e 302e 3927 0909 0909 0909 0923  ='3.0.9'.......#
+00000300: 3d27 332e 312e 3027 0909 0909 0909 0923  ='3.1.0'.......#
 00000310: e9a1 b9e7 9bae e789 88e6 9cac 0d0a 636f  ..............co
 00000320: 6e66 6b63 775b 2764 6573 6372 6970 7469  nfkcw['descripti
 00000330: 6f6e 275d 3d27 e8af a5e7 8988 e69c ace9  on']='..........
 00000340: 9c80 7079 7468 6f6e e789 88e6 9cac 3e3d  ..python......>=
 00000350: 332e 3827 2020 2020 2020 2023 e9a1 b9e7  3.8'       #....
 00000360: 9bae e79a 84e7 ae80 e58d 95e6 8f8f e8bf  ................
 00000370: b00d 0a63 6f6e 666b 6377 5b27 6c6f 6e67  ...confkcw['long
@@ -142,31 +142,30 @@
 000008d0: 6c75 732f 6269 6e2f 6b63 772e 6578 6527  lus/bin/kcw.exe'
 000008e0: 5d29 5d2c 0d0a 2020 2020 696e 7374 616c  ])],..    instal
 000008f0: 6c5f 7265 7175 6972 6573 203d 205b 276b  l_requires = ['k
 00000900: 6377 6562 3e3d 352e 3330 272c 2770 794f  cweb>=5.30','pyO
 00000910: 7065 6e53 534c 3d3d 3233 2e32 2e30 272c  penSSL==23.2.0',
 00000920: 2763 6861 7264 6574 3d3d 342e 302e 3027  'chardet==4.0.0'
 00000930: 2c27 6170 7363 6865 6475 6c65 723d 3d33  ,'apscheduler==3
-00000940: 2e36 2e33 272c 2771 7263 6f64 653d 3d36  .6.3','qrcode==6
-00000950: 2e31 272c 2770 696c 6c6f 773d 3d31 302e  .1','pillow==10.
-00000960: 302e 3027 2c27 7073 7574 696c 3d3d 352e  0.0','psutil==5.
-00000970: 382e 3027 2c27 6f73 7332 3e3d 322e 3132  8.0','oss2>=2.12
-00000980: 2e31 272c 2777 6562 736f 636b 6574 2d63  .1','websocket-c
-00000990: 6c69 656e 743d 3d31 2e33 2e31 272c 2763  lient==1.3.1','c
-000009a0: 7279 7074 6f67 7261 7068 793d 3d34 312e  ryptography==41.
-000009b0: 302e 3727 5d2c 2023 e7ac ace4 b889 e696  0.7'], #........
-000009c0: b9e5 8c85 0d0a 2020 2020 7061 636b 6167  ......    packag
-000009d0: 655f 6461 7461 203d 207b 0d0a 2020 2020  e_data = {..    
-000009e0: 2020 2020 2727 3a20 5b27 2a2e 6874 6d6c      '': ['*.html
-000009f0: 272c 2027 2a2e 6a73 272c 272a 2e63 7373  ', '*.js','*.css
-00000a00: 272c 272a 2e6a 7067 272c 272a 2e70 6e67  ','*.jpg','*.png
-00000a10: 272c 272a 2e67 6966 272c 2773 6572 7665  ','*.gif','serve
-00000a20: 7227 2c27 7365 7276 6572 2e73 6827 5d2c  r','server.sh'],
-00000a30: 0d0a 2020 2020 7d2c 0d0a 2020 2020 656e  ..    },..    en
-00000a40: 7472 795f 706f 696e 7473 203d 207b 0d0a  try_points = {..
-00000a50: 2020 2020 2020 2020 2763 6f6e 736f 6c65          'console
-00000a60: 5f73 6372 6970 7473 273a 5b0d 0a20 2020  _scripts':[..   
-00000a70: 2020 2020 2020 2020 2027 6b63 7765 6270           'kcwebp
-00000a80: 6c75 7320 3d20 6b63 7765 6270 6c75 732e  lus = kcwebplus.
-00000a90: 6b63 7765 6270 6c75 733a 6578 6563 7574  kcwebplus:execut
-00000aa0: 6162 6c65 270d 0a20 2020 2020 2020 205d  able'..        ]
-00000ab0: 0d0a 2020 2020 7d0d 0a29                 ..    }..)
+00000940: 2e36 2e33 272c 2770 696c 6c6f 773e 3d31  .6.3','pillow>=1
+00000950: 302e 302e 3027 2c27 7073 7574 696c 3d3d  0.0.0','psutil==
+00000960: 352e 382e 3027 2c27 6f73 7332 3e3d 322e  5.8.0','oss2>=2.
+00000970: 3132 2e31 272c 2777 6562 736f 636b 6574  12.1','websocket
+00000980: 2d63 6c69 656e 743d 3d31 2e33 2e31 272c  -client==1.3.1',
+00000990: 2763 7279 7074 6f67 7261 7068 793d 3d34  'cryptography==4
+000009a0: 312e 302e 3727 5d2c 2023 e7ac ace4 b889  1.0.7'], #......
+000009b0: e696 b9e5 8c85 0d0a 2020 2020 7061 636b  ........    pack
+000009c0: 6167 655f 6461 7461 203d 207b 0d0a 2020  age_data = {..  
+000009d0: 2020 2020 2020 2727 3a20 5b27 2a2e 6874        '': ['*.ht
+000009e0: 6d6c 272c 2027 2a2e 6a73 272c 272a 2e63  ml', '*.js','*.c
+000009f0: 7373 272c 272a 2e6a 7067 272c 272a 2e70  ss','*.jpg','*.p
+00000a00: 6e67 272c 272a 2e67 6966 272c 2773 6572  ng','*.gif','ser
+00000a10: 7665 7227 2c27 7365 7276 6572 2e73 6827  ver','server.sh'
+00000a20: 5d2c 0d0a 2020 2020 7d2c 0d0a 2020 2020  ],..    },..    
+00000a30: 656e 7472 795f 706f 696e 7473 203d 207b  entry_points = {
+00000a40: 0d0a 2020 2020 2020 2020 2763 6f6e 736f  ..        'conso
+00000a50: 6c65 5f73 6372 6970 7473 273a 5b0d 0a20  le_scripts':[.. 
+00000a60: 2020 2020 2020 2020 2020 2027 6b63 7765             'kcwe
+00000a70: 6270 6c75 7320 3d20 6b63 7765 6270 6c75  bplus = kcwebplu
+00000a80: 732e 6b63 7765 6270 6c75 733a 6578 6563  s.kcwebplus:exec
+00000a90: 7574 6162 6c65 270d 0a20 2020 2020 2020  utable'..       
+00000aa0: 205d 0d0a 2020 2020 7d0d 0a29             ]..    }..)
```

