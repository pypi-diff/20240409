# Comparing `tmp/temsah-2.1.2.tar.gz` & `tmp/temsah-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temsah-2.1.2.tar", last modified: Tue Mar 26 23:28:08 2024, max compression
+gzip compressed data, was "temsah-2.1.3.tar", last modified: Tue Apr  9 18:15:14 2024, max compression
```

## Comparing `temsah-2.1.2.tar` & `temsah-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 23:28:08.660641 temsah-2.1.2/
--rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      268 2024-03-26 23:28:08.659649 temsah-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2024-02-23 01:03:41.000000 temsah-2.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 23:28:08.661639 temsah-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-03-26 23:27:11.000000 temsah-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 23:28:08.649860 temsah-2.1.2/temsah/
--rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.2/temsah/__init__.py
--rw-rw-rw-   0        0        0    14576 2024-03-26 23:24:14.000000 temsah-2.1.2/temsah/data_extractor.py
--rw-rw-rw-   0        0        0     1616 2024-02-28 11:44:26.000000 temsah-2.1.2/temsah/main.py
-drwxrwxrwx   0        0        0        0 2024-03-26 23:28:08.657649 temsah-2.1.2/temsah.egg-info/
--rw-rw-rw-   0        0        0      268 2024-03-26 23:28:08.000000 temsah-2.1.2/temsah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-03-26 23:28:08.000000 temsah-2.1.2/temsah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 23:28:08.000000 temsah-2.1.2/temsah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-26 23:28:08.000000 temsah-2.1.2/temsah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-26 23:28:08.000000 temsah-2.1.2/temsah.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 18:15:14.968891 temsah-2.1.3/
+-rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      268 2024-04-09 18:15:14.960914 temsah-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2024-02-23 01:03:41.000000 temsah-2.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:15:14.969888 temsah-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-04-09 18:14:16.000000 temsah-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:15:14.920500 temsah-2.1.3/temsah/
+-rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.3/temsah/__init__.py
+-rw-rw-rw-   0        0        0     1656 2024-04-09 18:12:37.000000 temsah-2.1.3/temsah/currency.py
+-rw-rw-rw-   0        0        0    14576 2024-03-26 23:24:14.000000 temsah-2.1.3/temsah/data_extractor.py
+-rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.3/temsah/main.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:15:14.955405 temsah-2.1.3/temsah.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 18:15:14.000000 temsah-2.1.3/temsah.egg-info/top_level.txt
```

### Comparing `temsah-2.1.2/LICENSE.txt` & `temsah-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temsah-2.1.2/README.md` & `temsah-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `temsah-2.1.2/temsah/data_extractor.py` & `temsah-2.1.3/temsah/data_extractor.py`

 * *Files identical despite different names*

### Comparing `temsah-2.1.2/temsah/main.py` & `temsah-2.1.3/temsah/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 from bs4 import BeautifulSoup
 import chardet
 from .data_extractor import *
+from .currency import *
 
 
 # ---------------------------
 
 class Temsah:
 
     def __init__(self, url):
@@ -44,7 +45,14 @@
 
             scraper.product.url = url
 
             return scraper.product
 
         else:
             print(f"page.status_code:{page.status_code}")
+            
+
+        
+    
+        
+    
+
```

