# Comparing `tmp/kcwebplus-3.0.7.tar.gz` & `tmp/kcwebplus-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-3.0.7.tar", last modified: Tue Apr  9 16:19:15 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.8.tar", last modified: Tue Apr  9 16:23:48 2024, max compression
```

## Comparing `kcwebplus-3.0.7.tar` & `kcwebplus-3.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.085853 kcwebplus-3.0.7/
--rw-rw-rw-   0        0        0      344 2024-04-09 16:19:15.084853 kcwebplus-3.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.060856 kcwebplus-3.0.7/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.065913 kcwebplus-3.0.7/kcwebplus/common/
--rw-rw-rw-   0        0        0    18682 2024-04-09 15:47:58.000000 kcwebplus-3.0.7/kcwebplus/common/__init__.py
--rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/common/model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.070356 kcwebplus-3.0.7/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.071356 kcwebplus-3.0.7/kcwebplus/index/
--rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.072355 kcwebplus-3.0.7/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/common/__init__.py
--rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/common/autoload.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.073355 kcwebplus-3.0.7/kcwebplus/index/controller/
--rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.075356 kcwebplus-3.0.7/kcwebplus/index/controller/index/
--rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.077356 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.054928 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.081854 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1048 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/server
--rw-rw-rw-   0        0        0      339 2024-04-09 13:38:53.000000 kcwebplus-3.0.7/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 16:19:15.065913 kcwebplus-3.0.7/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1472 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      163 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      450 2024-04-09 16:19:15.000000 kcwebplus-3.0.7/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:19:15.085853 kcwebplus-3.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2746 2024-04-09 16:18:27.000000 kcwebplus-3.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.626504 kcwebplus-3.0.8/
+-rw-rw-rw-   0        0        0      344 2024-04-09 16:23:48.625518 kcwebplus-3.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.597506 kcwebplus-3.0.8/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.609506 kcwebplus-3.0.8/kcwebplus/common/
+-rw-rw-rw-   0        0        0    18682 2024-04-09 15:47:58.000000 kcwebplus-3.0.8/kcwebplus/common/__init__.py
+-rw-rw-rw-   0        0        0       41 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/common/model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.610506 kcwebplus-3.0.8/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.611505 kcwebplus-3.0.8/kcwebplus/index/
+-rw-rw-rw-   0        0        0       24 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.613506 kcwebplus-3.0.8/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       48 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/common/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/common/autoload.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.614506 kcwebplus-3.0.8/kcwebplus/index/controller/
+-rw-rw-rw-   0        0        0       21 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.616505 kcwebplus-3.0.8/kcwebplus/index/controller/index/
+-rw-rw-rw-   0        0        0       19 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.618504 kcwebplus-3.0.8/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       45 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0       36 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0     1386 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.592507 kcwebplus-3.0.8/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.621508 kcwebplus-3.0.8/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0    12570 2024-04-09 13:38:53.000000 kcwebplus-3.0.8/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1014 2024-04-09 16:23:31.000000 kcwebplus-3.0.8/kcwebplus/server
+-rw-rw-rw-   0        0        0      334 2024-04-09 16:23:25.000000 kcwebplus-3.0.8/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 16:23:48.605504 kcwebplus-3.0.8/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-09 16:23:48.000000 kcwebplus-3.0.8/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1472 2024-04-09 16:23:48.000000 kcwebplus-3.0.8/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:23:48.000000 kcwebplus-3.0.8/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-09 16:23:48.000000 kcwebplus-3.0.8/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      163 2024-04-09 16:23:48.000000 kcwebplus-3.0.8/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      450 2024-04-09 16:23:48.000000 kcwebplus-3.0.8/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:23:48.626504 kcwebplus-3.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2746 2024-04-09 16:23:46.000000 kcwebplus-3.0.8/setup.py
```

### Comparing `kcwebplus-3.0.7/README.md` & `kcwebplus-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/common/__init__.py` & `kcwebplus-3.0.8/kcwebplus/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/common/model.py` & `kcwebplus-3.0.8/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/config/__init__.py` & `kcwebplus-3.0.8/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0.8/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0.8/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0.8/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus/kcwebplus.py` & `kcwebplus-3.0.8/kcwebplus/kcwebplus.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0.8/kcwebplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcwebplus-3.0.7/setup.py` & `kcwebplus-3.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 00000290: 6e20 636f 6e0d 0a63 6f6e 666b 6377 3d7b  n con..confkcw={
 000002a0: 7d0d 0a63 6f6e 666b 6377 5b27 6e61 6d65  }..confkcw['name
 000002b0: 275d 3d27 6b63 7765 6270 6c75 7327 2020  ']='kcwebplus'  
 000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000002d0: 2020 2020 2020 2020 2020 2023 e9a1 b9e7             #....
 000002e0: 9bae e79a 84e5 908d e7a7 b020 0d0a 636f  ........... ..co
 000002f0: 6e66 6b63 775b 2776 6572 7369 6f6e 275d  nfkcw['version']
-00000300: 3d27 332e 302e 3727 0909 0909 0909 0923  ='3.0.7'.......#
+00000300: 3d27 332e 302e 3827 0909 0909 0909 0923  ='3.0.8'.......#
 00000310: e9a1 b9e7 9bae e789 88e6 9cac 0d0a 636f  ..............co
 00000320: 6e66 6b63 775b 2764 6573 6372 6970 7469  nfkcw['descripti
 00000330: 6f6e 275d 3d27 e8af a5e7 8988 e69c ace9  on']='..........
 00000340: 9c80 7079 7468 6f6e e789 88e6 9cac 3e3d  ..python......>=
 00000350: 332e 3827 2020 2020 2020 2023 e9a1 b9e7  3.8'       #....
 00000360: 9bae e79a 84e7 ae80 e58d 95e6 8f8f e8bf  ................
 00000370: b00d 0a63 6f6e 666b 6377 5b27 6c6f 6e67  ...confkcw['long
```

