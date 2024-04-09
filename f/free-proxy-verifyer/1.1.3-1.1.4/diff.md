# Comparing `tmp/free_proxy_verifyer-1.1.3.tar.gz` & `tmp/free_proxy_verifyer-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free_proxy_verifyer-1.1.3.tar", last modified: Thu Mar 14 12:53:21 2024, max compression
+gzip compressed data, was "free_proxy_verifyer-1.1.4.tar", last modified: Tue Apr  9 15:38:08 2024, max compression
```

## Comparing `free_proxy_verifyer-1.1.3.tar` & `free_proxy_verifyer-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:53:21.011818 free_proxy_verifyer-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-14 12:53:09.000000 free_proxy_verifyer-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-14 12:53:21.011818 free_proxy_verifyer-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-14 12:53:09.000000 free_proxy_verifyer-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:53:21.007818 free_proxy_verifyer-1.1.3/free_proxy_verifyer/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-14 12:53:09.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-14 12:53:09.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer/free_proxy_verifyer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 12:53:21.011818 free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-14 12:53:20.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-14 12:53:20.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 12:53:20.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 12:53:20.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-14 12:53:20.000000 free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 12:53:21.011818 free_proxy_verifyer-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-14 12:53:09.000000 free_proxy_verifyer-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:38:08.081691 free_proxy_verifyer-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 15:37:59.000000 free_proxy_verifyer-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-09 15:38:08.081691 free_proxy_verifyer-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-09 15:37:59.000000 free_proxy_verifyer-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:38:08.081691 free_proxy_verifyer-1.1.4/free_proxy_verifyer/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 15:37:59.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-09 15:37:59.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer/free_proxy_verifyer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:38:08.081691 free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-09 15:38:08.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 15:38:08.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:38:08.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 15:38:08.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 15:38:08.000000 free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:38:08.081691 free_proxy_verifyer-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 15:37:59.000000 free_proxy_verifyer-1.1.4/setup.py
```

### Comparing `free_proxy_verifyer-1.1.3/LICENSE.txt` & `free_proxy_verifyer-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `free_proxy_verifyer-1.1.3/PKG-INFO` & `free_proxy_verifyer-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: free_proxy_verifyer
-Version: 1.1.3
+Version: 1.1.4
 Summary: A simple package to verify http and https working proxies.
 Home-page: https://github.com/mominurr/free_proxy_verifyer
 Author: Mominur Rahman
 Author-email: mominurr518@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,16 @@
 - [checkip.amazonaws.com](https://checkip.amazonaws.com)
 - [ipify.org](https://api.ipify.org/)
 - [httpbin.org](https://httpbin.org/ip)
 - [icanhazip.com](https://www.icanhazip.com/)
 - [jsonip.com](https://jsonip.com/)
 - [SeeIP](https://api.seeip.org/jsonip)
 - [SmartProxy](https://ip.smartproxy.com/json)
+- [ip-api.com](https://ip-api.com/)
+- [ip.nf](https://ip.nf/me.json)
 
 
 # Installation
 
 You can install free_proxy_verifyer via pip:
 
 ```
```

### Comparing `free_proxy_verifyer-1.1.3/README.md` & `free_proxy_verifyer-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 - [checkip.amazonaws.com](https://checkip.amazonaws.com)
 - [ipify.org](https://api.ipify.org/)
 - [httpbin.org](https://httpbin.org/ip)
 - [icanhazip.com](https://www.icanhazip.com/)
 - [jsonip.com](https://jsonip.com/)
 - [SeeIP](https://api.seeip.org/jsonip)
 - [SmartProxy](https://ip.smartproxy.com/json)
+- [ip-api.com](https://ip-api.com/)
+- [ip.nf](https://ip.nf/me.json)
 
 
 # Installation
 
 You can install free_proxy_verifyer via pip:
 
 ```
```

### Comparing `free_proxy_verifyer-1.1.3/free_proxy_verifyer/free_proxy_verifyer.py` & `free_proxy_verifyer-1.1.4/free_proxy_verifyer/free_proxy_verifyer.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,16 @@
             "https://checkip.amazonaws.com",
             "https://api.ipify.org/",
             "https://httpbin.org/ip",
             "https://www.icanhazip.com/",
             "https://jsonip.com/",
             "https://api.seeip.org/jsonip",
             "https://ip.smartproxy.com/json",
+            "https://ip-api.com/",
+            "https://ip.nf/me.json"
         ]
         self.url=None
 
 
     def verify_proxy(self,proxy,timeout=(5,5)):
         """
         Verify if the proxy is working or not.
```

### Comparing `free_proxy_verifyer-1.1.3/free_proxy_verifyer.egg-info/PKG-INFO` & `free_proxy_verifyer-1.1.4/free_proxy_verifyer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: free-proxy-verifyer
-Version: 1.1.3
+Version: 1.1.4
 Summary: A simple package to verify http and https working proxies.
 Home-page: https://github.com/mominurr/free_proxy_verifyer
 Author: Mominur Rahman
 Author-email: mominurr518@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,16 @@
 - [checkip.amazonaws.com](https://checkip.amazonaws.com)
 - [ipify.org](https://api.ipify.org/)
 - [httpbin.org](https://httpbin.org/ip)
 - [icanhazip.com](https://www.icanhazip.com/)
 - [jsonip.com](https://jsonip.com/)
 - [SeeIP](https://api.seeip.org/jsonip)
 - [SmartProxy](https://ip.smartproxy.com/json)
+- [ip-api.com](https://ip-api.com/)
+- [ip.nf](https://ip.nf/me.json)
 
 
 # Installation
 
 You can install free_proxy_verifyer via pip:
 
 ```
```

### Comparing `free_proxy_verifyer-1.1.3/setup.py` & `free_proxy_verifyer-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='free_proxy_verifyer',
-    version='1.1.3',
+    version='1.1.4',
     author='Mominur Rahman',
     author_email='mominurr518@email.com',
     description='A simple package to verify http and https working proxies.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/mominurr/free_proxy_verifyer',
     packages=find_packages(),
```

