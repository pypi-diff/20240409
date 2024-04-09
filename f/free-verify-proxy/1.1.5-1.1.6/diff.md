# Comparing `tmp/free_verify_proxy-1.1.5.tar.gz` & `tmp/free_verify_proxy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free_verify_proxy-1.1.5.tar", last modified: Wed Mar 20 15:59:19 2024, max compression
+gzip compressed data, was "free_verify_proxy-1.1.6.tar", last modified: Tue Apr  9 15:40:35 2024, max compression
```

## Comparing `free_verify_proxy-1.1.5.tar` & `free_verify_proxy-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:59:19.081915 free_verify_proxy-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-20 15:59:19.081915 free_verify_proxy-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:59:19.081915 free_verify_proxy-1.1.5/free_verify_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/free_verify_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/free_verify_proxy/free_proxy_verifyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/free_verify_proxy/free_verify_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/free_verify_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:59:19.081915 free_verify_proxy-1.1.5/free_verify_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-20 15:59:19.000000 free_verify_proxy-1.1.5/free_verify_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-20 15:59:19.000000 free_verify_proxy-1.1.5/free_verify_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:59:19.000000 free_verify_proxy-1.1.5/free_verify_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 15:59:19.000000 free_verify_proxy-1.1.5/free_verify_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-20 15:59:19.000000 free_verify_proxy-1.1.5/free_verify_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 15:59:19.081915 free_verify_proxy-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-20 15:59:07.000000 free_verify_proxy-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:40:35.932864 free_verify_proxy-1.1.6/free_verify_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/free_proxy_verifyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/free_verify_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/setup.py
```

### Comparing `free_verify_proxy-1.1.5/LICENSE.txt` & `free_verify_proxy-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `free_verify_proxy-1.1.5/PKG-INFO` & `free_verify_proxy-1.1.6/free_verify_proxy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: free_verify_proxy
-Version: 1.1.5
+Name: free-verify-proxy
+Version: 1.1.6
 Summary: A simple package to provide http and https working proxy lists.
 Home-page: https://github.com/mominurr/free_verify_proxy
 Author: Mominur Rahman
 Author-email: mominurr518@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,14 +49,16 @@
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
 
 You can install free_verify_proxy via pip:
```

### Comparing `free_verify_proxy-1.1.5/README.md` & `free_verify_proxy-1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: free_verify_proxy
+Version: 1.1.6
+Summary: A simple package to provide http and https working proxy lists.
+Home-page: https://github.com/mominurr/free_verify_proxy
+Author: Mominur Rahman
+Author-email: mominurr518@email.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # free_verify_proxy
 
 free_verify_proxy is a Python library that collects free proxy from different sources and verifies whether the proxy is working or not. It checks the functionality of given proxies by making requests to various proxy detection servers. This library is useful for anyone who needs to ensure the reliability of proxies for their applications.
 
 
 # Proxy Sources
 
@@ -36,14 +49,16 @@
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
 
 You can install free_verify_proxy via pip:
 
@@ -75,8 +90,8 @@
 
 # Contributing
 
 Contributions are welcome! If you have any ideas, suggestions, or improvements, feel free to open an issue or create a pull request on GitHub.
 
 # License
 
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `free_verify_proxy-1.1.5/free_verify_proxy/free_proxy_verifyer.py` & `free_verify_proxy-1.1.6/free_verify_proxy/free_proxy_verifyer.py`

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

### Comparing `free_verify_proxy-1.1.5/free_verify_proxy/free_verify_proxy.py` & `free_verify_proxy-1.1.6/free_verify_proxy/free_verify_proxy.py`

 * *Files identical despite different names*

### Comparing `free_verify_proxy-1.1.5/free_verify_proxy/proxy.py` & `free_verify_proxy-1.1.6/free_verify_proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `free_verify_proxy-1.1.5/free_verify_proxy.egg-info/PKG-INFO` & `free_verify_proxy-1.1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: free-verify-proxy
-Version: 1.1.5
-Summary: A simple package to provide http and https working proxy lists.
-Home-page: https://github.com/mominurr/free_verify_proxy
-Author: Mominur Rahman
-Author-email: mominurr518@email.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # free_verify_proxy
 
 free_verify_proxy is a Python library that collects free proxy from different sources and verifies whether the proxy is working or not. It checks the functionality of given proxies by making requests to various proxy detection servers. This library is useful for anyone who needs to ensure the reliability of proxies for their applications.
 
 
 # Proxy Sources
 
@@ -49,14 +36,16 @@
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
 
 You can install free_verify_proxy via pip:
 
@@ -88,8 +77,8 @@
 
 # Contributing
 
 Contributions are welcome! If you have any ideas, suggestions, or improvements, feel free to open an issue or create a pull request on GitHub.
 
 # License
 
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `free_verify_proxy-1.1.5/setup.py` & `free_verify_proxy-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='free_verify_proxy',
-    version='1.1.5',
+    version='1.1.6',
     author='Mominur Rahman',
     author_email='mominurr518@email.com',
     description='A simple package to provide http and https working proxy lists.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/mominurr/free_verify_proxy',
     packages=find_packages(),
```

