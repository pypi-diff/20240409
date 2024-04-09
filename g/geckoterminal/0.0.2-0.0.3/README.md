# Comparing `tmp/geckoterminal-0.0.2.tar.gz` & `tmp/geckoterminal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geckoterminal-0.0.2.tar", last modified: Sun Dec 17 04:23:54 2023, max compression
+gzip compressed data, was "geckoterminal-0.0.3.tar", last modified: Tue Apr  9 18:51:51 2024, max compression
```

## Comparing `geckoterminal-0.0.2.tar` & `geckoterminal-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2023-12-17 04:23:54.649878 geckoterminal-0.0.2/
--rw-r--r--   0 samuel     (501) staff       (20)     1063 2023-10-27 20:26:39.000000 geckoterminal-0.0.2/LICENSE
--rw-r--r--   0 samuel     (501) staff       (20)      732 2023-12-17 04:23:54.649499 geckoterminal-0.0.2/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      529 2023-11-02 14:15:07.000000 geckoterminal-0.0.2/README.md
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2023-12-17 04:23:54.646536 geckoterminal-0.0.2/geckoterminal/
--rw-r--r--   0 samuel     (501) staff       (20)       18 2023-10-25 20:20:39.000000 geckoterminal-0.0.2/geckoterminal/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     3217 2023-10-27 20:15:02.000000 geckoterminal-0.0.2/geckoterminal/api.py
--rw-r--r--   0 samuel     (501) staff       (20)      640 2023-10-23 03:46:08.000000 geckoterminal-0.0.2/geckoterminal/client.py
--rw-r--r--   0 samuel     (501) staff       (20)      141 2023-07-24 16:10:03.000000 geckoterminal-0.0.2/geckoterminal/config.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2023-12-17 04:23:54.648374 geckoterminal-0.0.2/geckoterminal.egg-info/
--rw-r--r--   0 samuel     (501) staff       (20)      732 2023-12-17 04:23:54.000000 geckoterminal-0.0.2/geckoterminal.egg-info/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      323 2023-12-17 04:23:54.000000 geckoterminal-0.0.2/geckoterminal.egg-info/SOURCES.txt
--rw-r--r--   0 samuel     (501) staff       (20)        1 2023-12-17 04:23:54.000000 geckoterminal-0.0.2/geckoterminal.egg-info/dependency_links.txt
--rw-r--r--   0 samuel     (501) staff       (20)       30 2023-12-17 04:23:54.000000 geckoterminal-0.0.2/geckoterminal.egg-info/requires.txt
--rw-r--r--   0 samuel     (501) staff       (20)       14 2023-12-17 04:23:54.000000 geckoterminal-0.0.2/geckoterminal.egg-info/top_level.txt
--rw-r--r--   0 samuel     (501) staff       (20)       38 2023-12-17 04:23:54.649944 geckoterminal-0.0.2/setup.cfg
--rw-r--r--   0 samuel     (501) staff       (20)      383 2023-12-17 04:23:16.000000 geckoterminal-0.0.2/setup.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2023-12-17 04:23:54.648798 geckoterminal-0.0.2/tests/
--rw-r--r--   0 samuel     (501) staff       (20)     1522 2023-10-30 17:15:15.000000 geckoterminal-0.0.2/tests/test_api.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.986448 geckoterminal-0.0.3/
+-rw-r--r--   0 samuel     (501) staff       (20)     1063 2023-10-27 20:26:39.000000 geckoterminal-0.0.3/LICENSE
+-rw-r--r--   0 samuel     (501) staff       (20)      693 2024-04-09 18:51:51.986171 geckoterminal-0.0.3/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)      490 2024-04-09 18:47:29.000000 geckoterminal-0.0.3/README.md
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.982237 geckoterminal-0.0.3/geckoterminal/
+-rw-r--r--   0 samuel     (501) staff       (20)       18 2023-10-25 20:20:39.000000 geckoterminal-0.0.3/geckoterminal/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     3217 2023-10-27 20:15:02.000000 geckoterminal-0.0.3/geckoterminal/api.py
+-rw-r--r--   0 samuel     (501) staff       (20)      640 2023-10-23 03:46:08.000000 geckoterminal-0.0.3/geckoterminal/client.py
+-rw-r--r--   0 samuel     (501) staff       (20)      141 2023-07-24 16:10:03.000000 geckoterminal-0.0.3/geckoterminal/config.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.984969 geckoterminal-0.0.3/geckoterminal.egg-info/
+-rw-r--r--   0 samuel     (501) staff       (20)      693 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)      323 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel     (501) staff       (20)        1 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       30 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/requires.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       14 2024-04-09 18:51:51.000000 geckoterminal-0.0.3/geckoterminal.egg-info/top_level.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       38 2024-04-09 18:51:51.986510 geckoterminal-0.0.3/setup.cfg
+-rw-r--r--   0 samuel     (501) staff       (20)      383 2024-04-09 18:51:29.000000 geckoterminal-0.0.3/setup.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-04-09 18:51:51.985623 geckoterminal-0.0.3/tests/
+-rw-r--r--   0 samuel     (501) staff       (20)     1522 2023-10-30 17:15:15.000000 geckoterminal-0.0.3/tests/test_api.py
```

### Comparing `geckoterminal-0.0.2/LICENSE` & `geckoterminal-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geckoterminal-0.0.2/PKG-INFO` & `geckoterminal-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: geckoterminal
-Version: 0.0.2
+Version: 0.0.3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.0.0
 Requires-Dist: pandas>=2.0.0
 
 # GeckoTerminal
 
 Python wrapper for GeckoTerminal's API.
 
 ## Installation
 ```
-pip3 install git+https://github.com/samuel-poon/geckoterminal.git
+pip3 install geckoterminal
 ```
 
 ## GeckoTerminal Docs
 
 https://www.geckoterminal.com/dex-api
 
 ## Quick Start
```

### Comparing `geckoterminal-0.0.2/README.md` & `geckoterminal-0.0.3/geckoterminal.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+Metadata-Version: 2.1
+Name: geckoterminal
+Version: 0.0.3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.0.0
+Requires-Dist: pandas>=2.0.0
+
 # GeckoTerminal
 
 Python wrapper for GeckoTerminal's API.
 
 ## Installation
 ```
-pip3 install git+https://github.com/samuel-poon/geckoterminal.git
+pip3 install geckoterminal
 ```
 
 ## GeckoTerminal Docs
 
 https://www.geckoterminal.com/dex-api
 
 ## Quick Start
```

### Comparing `geckoterminal-0.0.2/geckoterminal/api.py` & `geckoterminal-0.0.3/geckoterminal/api.py`

 * *Files identical despite different names*

### Comparing `geckoterminal-0.0.2/geckoterminal/client.py` & `geckoterminal-0.0.3/geckoterminal/client.py`

 * *Files identical despite different names*

### Comparing `geckoterminal-0.0.2/tests/test_api.py` & `geckoterminal-0.0.3/tests/test_api.py`

 * *Files identical despite different names*

