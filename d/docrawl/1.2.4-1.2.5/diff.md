# Comparing `tmp/docrawl-1.2.4.tar.gz` & `tmp/docrawl-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.2.4.tar", last modified: Thu Mar 14 09:35:33 2024, max compression
+gzip compressed data, was "docrawl-1.2.5.tar", last modified: Tue Apr  9 10:47:51 2024, max compression
```

## Comparing `docrawl-1.2.4.tar` & `docrawl-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 09:35:33.952692 docrawl-1.2.4/
--rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.2.4/LICENSE
--rw-rw-rw-   0        0        0      527 2024-03-14 09:35:33.952692 docrawl-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 09:35:33.931260 docrawl-1.2.4/docrawl/
--rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.2.4/docrawl/__init__.py
--rw-rw-rw-   0        0        0    12433 2024-03-14 09:31:31.000000 docrawl-1.2.4/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    42925 2024-03-14 09:32:09.000000 docrawl-1.2.4/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.2.4/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.2.4/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.2.4/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2024-03-14 09:35:33.951626 docrawl-1.2.4/docrawl.egg-info/
--rw-rw-rw-   0        0        0      527 2024-03-14 09:35:33.000000 docrawl-1.2.4/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-03-14 09:35:33.000000 docrawl-1.2.4/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 09:35:33.000000 docrawl-1.2.4/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-03-14 09:35:33.000000 docrawl-1.2.4/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 09:35:33.000000 docrawl-1.2.4/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 09:35:33.952692 docrawl-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      834 2024-03-14 09:33:27.000000 docrawl-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:47:51.711438 docrawl-1.2.5/
+-rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-04-09 10:47:51.711438 docrawl-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 10:47:51.685599 docrawl-1.2.5/docrawl/
+-rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    12654 2024-03-18 17:46:30.000000 docrawl-1.2.5/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    42925 2024-03-14 09:32:09.000000 docrawl-1.2.5/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.2.5/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:47:51.709837 docrawl-1.2.5/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 10:47:51.000000 docrawl-1.2.5/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:47:51.711438 docrawl-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      834 2024-04-09 10:47:33.000000 docrawl-1.2.5/setup.py
```

### Comparing `docrawl-1.2.4/LICENSE` & `docrawl-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.4/PKG-INFO` & `docrawl-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.2.4
+Version: 1.2.5
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.2.4/docrawl/docrawl_client.py` & `docrawl-1.2.5/docrawl/docrawl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,27 @@
     headless: bool
     last_function: str
 
 
 class DocrawlClient:
     id_iter = itertools.count()
 
-    def __init__(self, kv_redis=KeepVariableDummyRedisServer(), kv_redis_keys=None, number_of_spawn_browsers=0):
+    def __init__(self, kv_redis=KeepVariableDummyRedisServer(), kv_redis_keys=None, number_of_spawn_browsers=0, redis_key_prefix=""):
         """number of spawn browsers = how many browser processes are ready in standby mode to not initialize + close the browser, currently support 0 and 1"""
         self._client_id = next(self.id_iter)
 
         self.kv_redis = kv_redis
         self.kv_redis_keys = kv_redis_keys or dict()
+        self.redis_key_prefix = redis_key_prefix
 
-        self._kv_redis_key_browser_metadata = self.kv_redis_keys.get('browser_meta_data', 'browser_meta_data')
-        self._kv_redis_key_scanned_elements = self.kv_redis_keys.get('elements', 'elements')
-        self._kv_redis_key_screenshot = self.kv_redis_keys.get('screenshot', 'screenshot')
-
+        self._kv_redis_key_browser_metadata = self.kv_redis_keys.get(self.redis_key_prefix+'browser_meta_data', self.redis_key_prefix+'browser_meta_data')
+        self._kv_redis_key_scanned_elements = self.kv_redis_keys.get(self.redis_key_prefix+'elements', self.redis_key_prefix+'elements')
+        self._kv_redis_key_screenshot = self.kv_redis_keys.get(self.redis_key_prefix+'screenshot', self.redis_key_prefix+'screenshot')
+        
+        
         docrawl_logger.info(f'Initialised DocrawlClient with ID {self._client_id}')
         
         if number_of_spawn_browsers > 0: #TODO: increase number of spawned browsers, support just 1 standby browser at this moment
             self.run_spider()
 
     def set_browser_meta_data(self, browser_meta_data: dict):
         self.kv_redis.set(key=self._kv_redis_key_browser_metadata, value=browser_meta_data)
```

### Comparing `docrawl-1.2.4/docrawl/docrawl_core.py` & `docrawl-1.2.5/docrawl/docrawl_core.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.4/docrawl/docrawl_launcher.py` & `docrawl-1.2.5/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.4/docrawl/docrawl_logger.py` & `docrawl-1.2.5/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.4/docrawl/elements.py` & `docrawl-1.2.5/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.2.4/docrawl.egg-info/PKG-INFO` & `docrawl-1.2.5/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.2.4
+Version: 1.2.5
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.2.4/setup.py` & `docrawl-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.2.4',
+    version='1.2.5',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

