# Comparing `tmp/kcwebplus-3.0.tar.gz` & `tmp/kcwebplus-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.tar", last modified: Mon Apr  8 15:14:16 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.1.tar", last modified: Mon Apr  8 15:22:40 2024, max compression
```

## Comparing `kcwebplus-3.0.tar` & `kcwebplus-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/common/
--rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/common/model.py
--rw-rw-rw-   0        0        0    18943 2024-04-04 04:18:15.000000 kcwebplus-3.0/kcwebplus/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/common/autoload.py
--rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/__init__.py
--rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/__init__.py
--rw-rw-rw-   0        0        0    12570 2024-04-08 15:11:11.000000 kcwebplus-3.0/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1014 2024-04-08 14:31:42.000000 kcwebplus-3.0/kcwebplus/server
--rw-rw-rw-   0        0        0      334 2024-04-04 03:14:17.000000 kcwebplus-3.0/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      354 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      141 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1480 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      450 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-3.0/LICENSE
--rw-rw-rw-   0        0        0      354 2024-04-08 15:14:16.000000 kcwebplus-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-08 15:12:36.000000 kcwebplus-3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 15:14:16.000000 kcwebplus-3.0/setup.cfg
--rw-rw-rw-   0        0        0     2641 2024-04-08 15:13:27.000000 kcwebplus-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/common/
+-rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/common/model.py
+-rw-rw-rw-   0        0        0    18943 2024-04-04 04:18:15.000000 kcwebplus-3.0.1/kcwebplus/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/common/autoload.py
+-rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/index/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/controller/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/kcwebplus/index/__init__.py
+-rw-rw-rw-   0        0        0    12570 2024-04-08 15:11:11.000000 kcwebplus-3.0.1/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1014 2024-04-08 14:31:42.000000 kcwebplus-3.0.1/kcwebplus/server
+-rw-rw-rw-   0        0        0      334 2024-04-08 15:21:11.000000 kcwebplus-3.0.1/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      358 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1480 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      450 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      358 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-08 15:20:26.000000 kcwebplus-3.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:22:40.000000 kcwebplus-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2643 2024-04-08 15:22:24.000000 kcwebplus-3.0.1/setup.py
```

### Comparing `kcwebplus-3.0/kcwebplus/common/model.py` & `kcwebplus-3.0.1/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/common/__init__.py` & `kcwebplus-3.0.1/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/config/__init__.py` & `kcwebplus-3.0.1/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0.1/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0.1/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/kcwebplus.py` & `kcwebplus-3.0.1/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus/server` & `kcwebplus-3.0.1/kcwebplus/server`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0.1/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/LICENSE` & `kcwebplus-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/README.md` & `kcwebplus-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0/setup.py` & `kcwebplus-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,130 +37,130 @@
 00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
 00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
 00000260: 6527 5d3d 276b 6377 6562 706c 7573 2720  e']='kcwebplus' 
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 2020 2020 23e9 a1b9              #...
 00000290: e79b aee7 9a84 e590 8de7 a7b0 200d 0a63  ............ ..c
 000002a0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000002b0: 5d3d 2733 2e30 2709 0909 0909 0909 23e9  ]='3.0'.......#.
-000002c0: a1b9 e79b aee7 8988 e69c ac0d 0a63 6f6e  .............con
-000002d0: 666b 6377 5b27 6465 7363 7269 7074 696f  fkcw['descriptio
-000002e0: 6e27 5d3d 27e8 afa5 e789 88e6 9cac e99c  n']='...........
-000002f0: 8070 7974 686f 6ee7 8988 e69c ac3e 3d33  .python......>=3
-00000300: 2e38 2720 2020 2020 2020 23e9 a1b9 e79b  .8'       #.....
-00000310: aee7 9a84 e7ae 80e5 8d95 e68f 8fe8 bfb0  ................
-00000320: 0d0a 636f 6e66 6b63 775b 276c 6f6e 675f  ..confkcw['long_
-00000330: 6465 7363 7269 7074 696f 6e27 5d3d 22e8  description']=".
-00000340: afa5 e789 88e6 9cac e99c 8070 7974 686f  ...........pytho
-00000350: 6ee7 8988 e69c ac3e 3d33 2e38 2220 2020  n......>=3.8"   
-00000360: 2020 23e9 a1b9 e79b aee8 afa6 e7bb 86e6    #.............
-00000370: 8f8f e8bf b00d 0a63 6f6e 666b 6377 5b27  .......confkcw['
-00000380: 6c69 6365 6e73 6527 5d3d 274d 4954 204c  license']='MIT L
-00000390: 6963 656e 7365 2720 2020 2020 2020 2020  icense'         
-000003a0: 2020 2020 2020 2020 2020 2023 e5bc 80e6             #....
-000003b0: ba90 e58d 8fe8 aeae 2020 206d 6974 e5bc  ........   mit..
-000003c0: 80e6 ba90 0d0a 636f 6e66 6b63 775b 2775  ......confkcw['u
-000003d0: 726c 275d 3d27 270d 0a63 6f6e 666b 6377  rl']=''..confkcw
-000003e0: 5b27 6175 7468 6f72 275d 3d27 e799 bee9  ['author']='....
-000003f0: 878c 2de5 9da4 e59d a427 2020 0909 0909  ..-......'  ....
-00000400: 0920 23e5 908d e5ad 970d 0a63 6f6e 666b  . #........confk
-00000410: 6377 5b27 6175 7468 6f72 5f65 6d61 696c  cw['author_email
-00000420: 275d 3d27 666b 3134 3032 3933 3635 3334  ']='fk1402936534
-00000430: 4071 712e 636f 6d27 2009 2020 2020 2023  @qq.com' .     #
-00000440: e982 aee4 bbb6 e59c b0e5 9d80 0d0a 636f  ..............co
-00000450: 6e66 6b63 775b 276d 6169 6e74 6169 6e65  nfkcw['maintaine
-00000460: 7227 5d3d 27e5 9da4 e59d a427 2009 0909  r']='......' ...
-00000470: 0909 0920 23e7 bbb4 e68a a4e4 baba e591  ... #...........
-00000480: 98e7 9a84 e590 8de5 ad97 0d0a 636f 6e66  ............conf
-00000490: 6b63 775b 276d 6169 6e74 6169 6e65 725f  kcw['maintainer_
-000004a0: 656d 6169 6c27 5d3d 2766 6b31 3430 3239  email']='fk14029
-000004b0: 3336 3533 3440 7171 2e63 6f6d 2720 2020  36534@qq.com'   
-000004c0: 2023 e7bb b4e6 8aa4 e4ba bae5 9198 e79a   #..............
-000004d0: 84e9 82ae e4bb b6e5 9cb0 e59d 800d 0a64  ...............d
-000004e0: 6566 2067 6574 5f66 696c 6528 666f 6c64  ef get_file(fold
-000004f0: 6572 3d27 2e2f 272c 6c69 7374 733d 5b5d  er='./',lists=[]
-00000500: 293a 0d0a 2020 2020 6c69 733d 6f73 2e6c  ):..    lis=os.l
-00000510: 6973 7464 6972 2866 6f6c 6465 7229 0d0a  istdir(folder)..
-00000520: 2020 2020 666f 7220 6669 6c65 7320 696e      for files in
-00000530: 206c 6973 3a0d 0a20 2020 2020 2020 2069   lis:..        i
-00000540: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
-00000550: 6669 6c65 2866 6f6c 6465 722b 222f 222b  file(folder+"/"+
-00000560: 6669 6c65 7329 3a0d 0a20 2020 2020 2020  files):..       
-00000570: 2020 2020 2069 6620 6669 6c65 733d 3d27       if files=='
-00000580: 5f5f 7079 6361 6368 655f 5f27 206f 7220  __pycache__' or 
-00000590: 6669 6c65 733d 3d27 2e67 6974 273a 0d0a  files=='.git':..
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
-000005c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000005d0: 2020 2020 2020 2020 206c 6973 7473 2e61           lists.a
-000005e0: 7070 656e 6428 666f 6c64 6572 2b22 2f22  ppend(folder+"/"
-000005f0: 2b66 696c 6573 290d 0a20 2020 2020 2020  +files)..       
-00000600: 2020 2020 2020 2020 2067 6574 5f66 696c           get_fil
-00000610: 6528 666f 6c64 6572 2b22 2f22 2b66 696c  e(folder+"/"+fil
-00000620: 6573 2c6c 6973 7473 290d 0a20 2020 2020  es,lists)..     
-00000630: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000640: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-00000650: 7265 7475 726e 206c 6973 7473 0d0a 623d  return lists..b=
-00000660: 6765 745f 6669 6c65 2822 6b63 7765 6270  get_file("kcwebp
-00000670: 6c75 7322 2c5b 276b 6377 6562 706c 7573  lus",['kcwebplus
-00000680: 275d 290d 0a73 6574 7570 280d 0a20 2020  '])..setup(..   
-00000690: 206e 616d 6520 3d20 636f 6e66 6b63 775b   name = confkcw[
-000006a0: 226e 616d 6522 5d2c 0d0a 2020 2020 7665  "name"],..    ve
-000006b0: 7273 696f 6e20 3d20 636f 6e66 6b63 775b  rsion = confkcw[
-000006c0: 2276 6572 7369 6f6e 225d 2c0d 0a20 2020  "version"],..   
-000006d0: 206b 6579 776f 7264 7320 3d20 226b 6377   keywords = "kcw
-000006e0: 6562 706c 7573 222b 636f 6e66 6b63 775b  ebplus"+confkcw[
-000006f0: 2776 6572 7369 6f6e 275d 2c0d 0a20 2020  'version'],..   
-00000700: 2064 6573 6372 6970 7469 6f6e 203d 2063   description = c
-00000710: 6f6e 666b 6377 5b22 6465 7363 7269 7074  onfkcw["descript
-00000720: 696f 6e22 5d2c 0d0a 2020 2020 6c6f 6e67  ion"],..    long
-00000730: 5f64 6573 6372 6970 7469 6f6e 203d 2063  _description = c
-00000740: 6f6e 666b 6377 5b22 6c6f 6e67 5f64 6573  onfkcw["long_des
-00000750: 6372 6970 7469 6f6e 225d 2c0d 0a20 2020  cription"],..   
-00000760: 206c 6963 656e 7365 203d 2063 6f6e 666b   license = confk
-00000770: 6377 5b22 6c69 6365 6e73 6522 5d2c 0d0a  cw["license"],..
-00000780: 2020 2020 6175 7468 6f72 203d 2063 6f6e      author = con
-00000790: 666b 6377 5b22 6175 7468 6f72 225d 2c0d  fkcw["author"],.
-000007a0: 0a20 2020 2061 7574 686f 725f 656d 6169  .    author_emai
-000007b0: 6c20 3d20 636f 6e66 6b63 775b 2261 7574  l = confkcw["aut
-000007c0: 686f 725f 656d 6169 6c22 5d2c 0d0a 2020  hor_email"],..  
-000007d0: 2020 6d61 696e 7461 696e 6572 203d 2063    maintainer = c
-000007e0: 6f6e 666b 6377 5b22 6d61 696e 7461 696e  onfkcw["maintain
-000007f0: 6572 225d 2c0d 0a20 2020 206d 6169 6e74  er"],..    maint
-00000800: 6169 6e65 725f 656d 6169 6c20 3d20 636f  ainer_email = co
-00000810: 6e66 6b63 775b 226d 6169 6e74 6169 6e65  nfkcw["maintaine
-00000820: 725f 656d 6169 6c22 5d2c 0d0a 2020 2020  r_email"],..    
-00000830: 7572 6c3d 636f 6e66 6b63 775b 2775 726c  url=confkcw['url
-00000840: 275d 2c0d 0a20 2020 2070 6163 6b61 6765  '],..    package
-00000850: 7320 3d20 2062 2c0d 0a20 2020 2023 2064  s =  b,..    # d
-00000860: 6174 615f 6669 6c65 733d 5b28 2753 6372  ata_files=[('Scr
-00000870: 6970 7473 272c 205b 276b 6377 6562 706c  ipts', ['kcwebpl
-00000880: 7573 2f62 696e 2f6b 6377 2e65 7865 275d  us/bin/kcw.exe']
-00000890: 295d 2c0d 0a20 2020 2069 6e73 7461 6c6c  )],..    install
-000008a0: 5f72 6571 7569 7265 7320 3d20 5b27 6b63  _requires = ['kc
-000008b0: 7765 623e 3d35 2e32 3727 2c27 7079 4f70  web>=5.27','pyOp
-000008c0: 656e 5353 4c3d 3d32 332e 322e 3027 2c27  enSSL==23.2.0','
-000008d0: 6368 6172 6465 743d 3d34 2e30 2e30 272c  chardet==4.0.0',
-000008e0: 2761 7073 6368 6564 756c 6572 3d3d 332e  'apscheduler==3.
-000008f0: 362e 3327 2c27 7172 636f 6465 3d3d 362e  6.3','qrcode==6.
-00000900: 3127 2c27 7069 6c6c 6f77 3d3d 382e 342e  1','pillow==8.4.
-00000910: 3027 2c27 7073 7574 696c 3d3d 352e 372e  0','psutil==5.7.
-00000920: 3027 2c27 6f73 7332 3d3d 322e 3132 2e31  0','oss2==2.12.1
-00000930: 272c 2777 6562 736f 636b 6574 2d63 6c69  ','websocket-cli
-00000940: 656e 743d 3d31 2e33 2e31 275d 2c20 23e7  ent==1.3.1'], #.
-00000950: acac e4b8 89e6 96b9 e58c 850d 0a20 2020  .............   
-00000960: 2070 6163 6b61 6765 5f64 6174 6120 3d20   package_data = 
-00000970: 7b0d 0a20 2020 2020 2020 2027 273a 205b  {..        '': [
-00000980: 272a 2e68 746d 6c27 2c20 272a 2e6a 7327  '*.html', '*.js'
-00000990: 2c27 2a2e 6373 7327 2c27 2a2e 6a70 6727  ,'*.css','*.jpg'
-000009a0: 2c27 2a2e 706e 6727 2c27 2a2e 6769 6627  ,'*.png','*.gif'
-000009b0: 2c27 7365 7276 6572 272c 2773 6572 7665  ,'server','serve
-000009c0: 722e 7368 275d 2c0d 0a20 2020 207d 2c0d  r.sh'],..    },.
-000009d0: 0a20 2020 2065 6e74 7279 5f70 6f69 6e74  .    entry_point
-000009e0: 7320 3d20 7b0d 0a20 2020 2020 2020 2027  s = {..        '
-000009f0: 636f 6e73 6f6c 655f 7363 7269 7074 7327  console_scripts'
-00000a00: 3a5b 0d0a 2020 2020 2020 2020 2020 2020  :[..            
-00000a10: 276b 6377 6562 706c 7573 203d 206b 6377  'kcwebplus = kcw
-00000a20: 6562 706c 7573 2e6b 6377 6562 706c 7573  ebplus.kcwebplus
-00000a30: 3a65 7865 6375 7461 626c 6527 0d0a 2020  :executable'..  
-00000a40: 2020 2020 2020 5d0d 0a20 2020 207d 0d0a        ]..    }..
-00000a50: 29                                       )
+000002b0: 5d3d 2733 2e30 2e31 2709 0909 0909 0909  ]='3.0.1'.......
+000002c0: 23e9 a1b9 e79b aee7 8988 e69c ac0d 0a63  #..............c
+000002d0: 6f6e 666b 6377 5b27 6465 7363 7269 7074  onfkcw['descript
+000002e0: 696f 6e27 5d3d 27e8 afa5 e789 88e6 9cac  ion']='.........
+000002f0: e99c 8070 7974 686f 6ee7 8988 e69c ac3e  ...python......>
+00000300: 3d33 2e38 2720 2020 2020 2020 23e9 a1b9  =3.8'       #...
+00000310: e79b aee7 9a84 e7ae 80e5 8d95 e68f 8fe8  ................
+00000320: bfb0 0d0a 636f 6e66 6b63 775b 276c 6f6e  ....confkcw['lon
+00000330: 675f 6465 7363 7269 7074 696f 6e27 5d3d  g_description']=
+00000340: 22e8 afa5 e789 88e6 9cac e99c 8070 7974  "............pyt
+00000350: 686f 6ee7 8988 e69c ac3e 3d33 2e38 2220  hon......>=3.8" 
+00000360: 2020 2020 23e9 a1b9 e79b aee8 afa6 e7bb      #...........
+00000370: 86e6 8f8f e8bf b00d 0a63 6f6e 666b 6377  .........confkcw
+00000380: 5b27 6c69 6365 6e73 6527 5d3d 274d 4954  ['license']='MIT
+00000390: 204c 6963 656e 7365 2720 2020 2020 2020   License'       
+000003a0: 2020 2020 2020 2020 2020 2020 2023 e5bc               #..
+000003b0: 80e6 ba90 e58d 8fe8 aeae 2020 206d 6974  ..........   mit
+000003c0: e5bc 80e6 ba90 0d0a 636f 6e66 6b63 775b  ........confkcw[
+000003d0: 2775 726c 275d 3d27 270d 0a63 6f6e 666b  'url']=''..confk
+000003e0: 6377 5b27 6175 7468 6f72 275d 3d27 e799  cw['author']='..
+000003f0: bee9 878c 2de5 9da4 e59d a427 2020 0909  ....-......'  ..
+00000400: 0909 0920 23e5 908d e5ad 970d 0a63 6f6e  ... #........con
+00000410: 666b 6377 5b27 6175 7468 6f72 5f65 6d61  fkcw['author_ema
+00000420: 696c 275d 3d27 666b 3134 3032 3933 3635  il']='fk14029365
+00000430: 3334 4071 712e 636f 6d27 2009 2020 2020  34@qq.com' .    
+00000440: 2023 e982 aee4 bbb6 e59c b0e5 9d80 0d0a   #..............
+00000450: 636f 6e66 6b63 775b 276d 6169 6e74 6169  confkcw['maintai
+00000460: 6e65 7227 5d3d 27e5 9da4 e59d a427 2009  ner']='......' .
+00000470: 0909 0909 0920 23e7 bbb4 e68a a4e4 baba  ..... #.........
+00000480: e591 98e7 9a84 e590 8de5 ad97 0d0a 636f  ..............co
+00000490: 6e66 6b63 775b 276d 6169 6e74 6169 6e65  nfkcw['maintaine
+000004a0: 725f 656d 6169 6c27 5d3d 2766 6b31 3430  r_email']='fk140
+000004b0: 3239 3336 3533 3440 7171 2e63 6f6d 2720  2936534@qq.com' 
+000004c0: 2020 2023 e7bb b4e6 8aa4 e4ba bae5 9198     #............
+000004d0: e79a 84e9 82ae e4bb b6e5 9cb0 e59d 800d  ................
+000004e0: 0a64 6566 2067 6574 5f66 696c 6528 666f  .def get_file(fo
+000004f0: 6c64 6572 3d27 2e2f 272c 6c69 7374 733d  lder='./',lists=
+00000500: 5b5d 293a 0d0a 2020 2020 6c69 733d 6f73  []):..    lis=os
+00000510: 2e6c 6973 7464 6972 2866 6f6c 6465 7229  .listdir(folder)
+00000520: 0d0a 2020 2020 666f 7220 6669 6c65 7320  ..    for files 
+00000530: 696e 206c 6973 3a0d 0a20 2020 2020 2020  in lis:..       
+00000540: 2069 6620 6e6f 7420 6f73 2e70 6174 682e   if not os.path.
+00000550: 6973 6669 6c65 2866 6f6c 6465 722b 222f  isfile(folder+"/
+00000560: 222b 6669 6c65 7329 3a0d 0a20 2020 2020  "+files):..     
+00000570: 2020 2020 2020 2069 6620 6669 6c65 733d         if files=
+00000580: 3d27 5f5f 7079 6361 6368 655f 5f27 206f  ='__pycache__' o
+00000590: 7220 6669 6c65 733d 3d27 2e67 6974 273a  r files=='.git':
+000005a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000005b0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+000005c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000005d0: 2020 2020 2020 2020 2020 206c 6973 7473             lists
+000005e0: 2e61 7070 656e 6428 666f 6c64 6572 2b22  .append(folder+"
+000005f0: 2f22 2b66 696c 6573 290d 0a20 2020 2020  /"+files)..     
+00000600: 2020 2020 2020 2020 2020 2067 6574 5f66             get_f
+00000610: 696c 6528 666f 6c64 6572 2b22 2f22 2b66  ile(folder+"/"+f
+00000620: 696c 6573 2c6c 6973 7473 290d 0a20 2020  iles,lists)..   
+00000630: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00000640: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+00000650: 2020 7265 7475 726e 206c 6973 7473 0d0a    return lists..
+00000660: 623d 6765 745f 6669 6c65 2822 6b63 7765  b=get_file("kcwe
+00000670: 6270 6c75 7322 2c5b 276b 6377 6562 706c  bplus",['kcwebpl
+00000680: 7573 275d 290d 0a73 6574 7570 280d 0a20  us'])..setup(.. 
+00000690: 2020 206e 616d 6520 3d20 636f 6e66 6b63     name = confkc
+000006a0: 775b 226e 616d 6522 5d2c 0d0a 2020 2020  w["name"],..    
+000006b0: 7665 7273 696f 6e20 3d20 636f 6e66 6b63  version = confkc
+000006c0: 775b 2276 6572 7369 6f6e 225d 2c0d 0a20  w["version"],.. 
+000006d0: 2020 206b 6579 776f 7264 7320 3d20 226b     keywords = "k
+000006e0: 6377 6562 706c 7573 222b 636f 6e66 6b63  cwebplus"+confkc
+000006f0: 775b 2776 6572 7369 6f6e 275d 2c0d 0a20  w['version'],.. 
+00000700: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
+00000710: 2063 6f6e 666b 6377 5b22 6465 7363 7269   confkcw["descri
+00000720: 7074 696f 6e22 5d2c 0d0a 2020 2020 6c6f  ption"],..    lo
+00000730: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00000740: 2063 6f6e 666b 6377 5b22 6c6f 6e67 5f64   confkcw["long_d
+00000750: 6573 6372 6970 7469 6f6e 225d 2c0d 0a20  escription"],.. 
+00000760: 2020 206c 6963 656e 7365 203d 2063 6f6e     license = con
+00000770: 666b 6377 5b22 6c69 6365 6e73 6522 5d2c  fkcw["license"],
+00000780: 0d0a 2020 2020 6175 7468 6f72 203d 2063  ..    author = c
+00000790: 6f6e 666b 6377 5b22 6175 7468 6f72 225d  onfkcw["author"]
+000007a0: 2c0d 0a20 2020 2061 7574 686f 725f 656d  ,..    author_em
+000007b0: 6169 6c20 3d20 636f 6e66 6b63 775b 2261  ail = confkcw["a
+000007c0: 7574 686f 725f 656d 6169 6c22 5d2c 0d0a  uthor_email"],..
+000007d0: 2020 2020 6d61 696e 7461 696e 6572 203d      maintainer =
+000007e0: 2063 6f6e 666b 6377 5b22 6d61 696e 7461   confkcw["mainta
+000007f0: 696e 6572 225d 2c0d 0a20 2020 206d 6169  iner"],..    mai
+00000800: 6e74 6169 6e65 725f 656d 6169 6c20 3d20  ntainer_email = 
+00000810: 636f 6e66 6b63 775b 226d 6169 6e74 6169  confkcw["maintai
+00000820: 6e65 725f 656d 6169 6c22 5d2c 0d0a 2020  ner_email"],..  
+00000830: 2020 7572 6c3d 636f 6e66 6b63 775b 2775    url=confkcw['u
+00000840: 726c 275d 2c0d 0a20 2020 2070 6163 6b61  rl'],..    packa
+00000850: 6765 7320 3d20 2062 2c0d 0a20 2020 2023  ges =  b,..    #
+00000860: 2064 6174 615f 6669 6c65 733d 5b28 2753   data_files=[('S
+00000870: 6372 6970 7473 272c 205b 276b 6377 6562  cripts', ['kcweb
+00000880: 706c 7573 2f62 696e 2f6b 6377 2e65 7865  plus/bin/kcw.exe
+00000890: 275d 295d 2c0d 0a20 2020 2069 6e73 7461  '])],..    insta
+000008a0: 6c6c 5f72 6571 7569 7265 7320 3d20 5b27  ll_requires = ['
+000008b0: 6b63 7765 623e 3d35 2e32 3727 2c27 7079  kcweb>=5.27','py
+000008c0: 4f70 656e 5353 4c3d 3d32 332e 322e 3027  OpenSSL==23.2.0'
+000008d0: 2c27 6368 6172 6465 743d 3d34 2e30 2e30  ,'chardet==4.0.0
+000008e0: 272c 2761 7073 6368 6564 756c 6572 3d3d  ','apscheduler==
+000008f0: 332e 362e 3327 2c27 7172 636f 6465 3d3d  3.6.3','qrcode==
+00000900: 362e 3127 2c27 7069 6c6c 6f77 3d3d 382e  6.1','pillow==8.
+00000910: 342e 3027 2c27 7073 7574 696c 3d3d 352e  4.0','psutil==5.
+00000920: 372e 3027 2c27 6f73 7332 3d3d 322e 3132  7.0','oss2==2.12
+00000930: 2e31 272c 2777 6562 736f 636b 6574 2d63  .1','websocket-c
+00000940: 6c69 656e 743d 3d31 2e33 2e31 275d 2c20  lient==1.3.1'], 
+00000950: 23e7 acac e4b8 89e6 96b9 e58c 850d 0a20  #.............. 
+00000960: 2020 2070 6163 6b61 6765 5f64 6174 6120     package_data 
+00000970: 3d20 7b0d 0a20 2020 2020 2020 2027 273a  = {..        '':
+00000980: 205b 272a 2e68 746d 6c27 2c20 272a 2e6a   ['*.html', '*.j
+00000990: 7327 2c27 2a2e 6373 7327 2c27 2a2e 6a70  s','*.css','*.jp
+000009a0: 6727 2c27 2a2e 706e 6727 2c27 2a2e 6769  g','*.png','*.gi
+000009b0: 6627 2c27 7365 7276 6572 272c 2773 6572  f','server','ser
+000009c0: 7665 722e 7368 275d 2c0d 0a20 2020 207d  ver.sh'],..    }
+000009d0: 2c0d 0a20 2020 2065 6e74 7279 5f70 6f69  ,..    entry_poi
+000009e0: 6e74 7320 3d20 7b0d 0a20 2020 2020 2020  nts = {..       
+000009f0: 2027 636f 6e73 6f6c 655f 7363 7269 7074   'console_script
+00000a00: 7327 3a5b 0d0a 2020 2020 2020 2020 2020  s':[..          
+00000a10: 2020 276b 6377 6562 706c 7573 203d 206b    'kcwebplus = k
+00000a20: 6377 6562 706c 7573 2e6b 6377 6562 706c  cwebplus.kcwebpl
+00000a30: 7573 3a65 7865 6375 7461 626c 6527 0d0a  us:executable'..
+00000a40: 2020 2020 2020 2020 5d0d 0a20 2020 207d          ]..    }
+00000a50: 0d0a 29                                  ..)
```

