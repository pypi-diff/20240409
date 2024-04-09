# Comparing `tmp/hscan-3.3.4.tar.gz` & `tmp/hscan-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscan-3.3.4.tar", last modified: Mon Mar 25 02:42:10 2024, max compression
+gzip compressed data, was "hscan-3.3.5.tar", last modified: Tue Apr  9 02:57:56 2024, max compression
```

## Comparing `hscan-3.3.4.tar` & `hscan-3.3.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-03-25 02:42:10.804515 hscan-3.3.4/
--rw-r--r--   0 jyanghe    (501) staff       (20)      517 2024-03-25 02:42:10.804037 hscan-3.3.4/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)       95 2024-03-19 07:49:57.000000 hscan-3.3.4/README.md
--rw-r--r--   0 jyanghe    (501) staff       (20)     1114 2024-03-25 02:38:49.000000 hscan-3.3.4/Setup.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-03-25 02:42:10.785558 hscan-3.3.4/hscan.egg-info/
--rw-r--r--   0 jyanghe    (501) staff       (20)      517 2024-03-25 02:42:10.000000 hscan-3.3.4/hscan.egg-info/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)      652 2024-03-25 02:42:10.000000 hscan-3.3.4/hscan.egg-info/SOURCES.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        1 2024-03-25 02:42:10.000000 hscan-3.3.4/hscan.egg-info/dependency_links.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)      276 2024-03-25 02:42:10.000000 hscan-3.3.4/hscan.egg-info/requires.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        5 2024-03-25 02:42:10.000000 hscan-3.3.4/hscan.egg-info/top_level.txt
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-03-25 02:42:10.792452 hscan-3.3.4/scan/
--rw-r--r--   0 jyanghe    (501) staff       (20)      255 2023-11-21 07:57:54.000000 hscan-3.3.4/scan/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-3.3.4/scan/common.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-3.3.4/scan/config.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1523 2023-12-21 02:40:02.000000 hscan-3.3.4/scan/crawl.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-03-25 02:42:10.801362 hscan-3.3.4/scan/database/
--rw-r--r--   0 jyanghe    (501) staff       (20)      353 2024-03-25 02:39:35.000000 hscan-3.3.4/scan/database/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     5654 2024-01-17 02:08:19.000000 hscan-3.3.4/scan/database/aior2.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-3.3.4/scan/database/kafka.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-3.3.4/scan/database/mongodb.py
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-3.3.4/scan/database/mysql.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-3.3.4/scan/database/oss.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-3.3.4/scan/database/pg.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     3610 2023-08-23 03:23:21.000000 hscan-3.3.4/scan/database/r2.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     8218 2024-03-19 08:09:15.000000 hscan-3.3.4/scan/database/rabbitmq.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-3.3.4/scan/database/redis.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     7536 2024-03-25 02:38:14.000000 hscan-3.3.4/scan/database/wasabi.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-03-25 02:42:10.803021 hscan-3.3.4/scan/downloade/
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-3.3.4/scan/downloade/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2880 2023-11-21 08:29:57.000000 hscan-3.3.4/scan/downloade/aiohttp_downloader.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     7569 2023-11-23 09:30:46.000000 hscan-3.3.4/scan/downloade/downloader.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1089 2023-11-15 08:19:41.000000 hscan-3.3.4/scan/log.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-3.3.4/scan/monitor.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-3.3.4/scan/response.py
--rw-r--r--   0 jyanghe    (501) staff       (20)    12677 2023-11-09 08:38:43.000000 hscan-3.3.4/scan/spider.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-3.3.4/scan/util.py
--rw-r--r--   0 jyanghe    (501) staff       (20)       38 2024-03-25 02:42:10.804626 hscan-3.3.4/setup.cfg
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-04-09 02:57:56.276007 hscan-3.3.5/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      517 2024-04-09 02:57:56.275414 hscan-3.3.5/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)       95 2024-03-19 07:49:57.000000 hscan-3.3.5/README.md
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1114 2024-04-09 02:56:04.000000 hscan-3.3.5/Setup.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-04-09 02:57:56.254378 hscan-3.3.5/hscan.egg-info/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      517 2024-04-09 02:57:56.000000 hscan-3.3.5/hscan.egg-info/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)      652 2024-04-09 02:57:56.000000 hscan-3.3.5/hscan.egg-info/SOURCES.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        1 2024-04-09 02:57:56.000000 hscan-3.3.5/hscan.egg-info/dependency_links.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)      276 2024-04-09 02:57:56.000000 hscan-3.3.5/hscan.egg-info/requires.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        5 2024-04-09 02:57:56.000000 hscan-3.3.5/hscan.egg-info/top_level.txt
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-04-09 02:57:56.262081 hscan-3.3.5/scan/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      255 2023-11-21 07:57:54.000000 hscan-3.3.5/scan/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-3.3.5/scan/common.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-3.3.5/scan/config.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1524 2024-04-09 02:55:48.000000 hscan-3.3.5/scan/crawl.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-04-09 02:57:56.271679 hscan-3.3.5/scan/database/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      353 2024-03-25 02:39:35.000000 hscan-3.3.5/scan/database/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     5654 2024-01-17 02:08:19.000000 hscan-3.3.5/scan/database/aior2.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-3.3.5/scan/database/kafka.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-3.3.5/scan/database/mongodb.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-3.3.5/scan/database/mysql.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-3.3.5/scan/database/oss.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-3.3.5/scan/database/pg.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     3610 2023-08-23 03:23:21.000000 hscan-3.3.5/scan/database/r2.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     8218 2024-03-19 08:09:15.000000 hscan-3.3.5/scan/database/rabbitmq.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-3.3.5/scan/database/redis.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     7536 2024-03-25 02:38:14.000000 hscan-3.3.5/scan/database/wasabi.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2024-04-09 02:57:56.274211 hscan-3.3.5/scan/downloade/
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-3.3.5/scan/downloade/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2880 2023-11-21 08:29:57.000000 hscan-3.3.5/scan/downloade/aiohttp_downloader.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     7569 2023-11-23 09:30:46.000000 hscan-3.3.5/scan/downloade/downloader.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1089 2023-11-15 08:19:41.000000 hscan-3.3.5/scan/log.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-3.3.5/scan/monitor.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-3.3.5/scan/response.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)    12677 2023-11-09 08:38:43.000000 hscan-3.3.5/scan/spider.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-3.3.5/scan/util.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)       38 2024-04-09 02:57:56.276149 hscan-3.3.5/setup.cfg
```

### Comparing `hscan-3.3.4/PKG-INFO` & `hscan-3.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscan
-Version: 3.3.4
+Version: 3.3.5
 Summary: A python framework
 Home-page: https://github.com/jyangHe/hscan
 Author: jyanghe
 Author-email: jyanghe1023@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hscan-3.3.4/Setup.py` & `hscan-3.3.5/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hscan",
-    version="3.3.4",
+    version="3.3.5",
     author="jyanghe",
     author_email="jyanghe1023@gmail.com",
     description="A python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jyangHe/hscan",
     packages=setuptools.find_packages(),
```

### Comparing `hscan-3.3.4/hscan.egg-info/PKG-INFO` & `hscan-3.3.5/hscan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscan
-Version: 3.3.4
+Version: 3.3.5
 Summary: A python framework
 Home-page: https://github.com/jyangHe/hscan
 Author: jyanghe
 Author-email: jyanghe1023@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hscan-3.3.4/hscan.egg-info/SOURCES.txt` & `hscan-3.3.5/hscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/config.py` & `hscan-3.3.5/scan/config.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/crawl.py` & `hscan-3.3.5/scan/crawl.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Crawl:
     def __init__(self):
         self.downloader = Downloader()
         self.aiohttp_downloader = AioHttpDownloader()
 
     async def fetch(self,  url, params=None, data=None, files=None, json=None, content=None, headers=None, cookies=None,
                     verify=True, http2=False, auth=None, proxies=None, allow_redirects=True, stream=False,
-                    session=True, timeout=30, cycle=1, tls=False, use_aiohttp=False):
+                    session=False, timeout=30, cycle=1, tls=False, use_aiohttp=False):
         if use_aiohttp:
             res = await self.aiohttp_downloader.request(
                 url, params=params, data=data, files=files, json=json, content=content, headers=headers,
                 proxies=proxies,
                 verify=verify, http2=http2, cookies=cookies, auth=auth, allow_redirects=allow_redirects,
                 timeout=timeout,
                 cycle=cycle, stream=stream, tls=tls, session=session
```

### Comparing `hscan-3.3.4/scan/database/aior2.py` & `hscan-3.3.5/scan/database/aior2.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/kafka.py` & `hscan-3.3.5/scan/database/kafka.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/mongodb.py` & `hscan-3.3.5/scan/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/pg.py` & `hscan-3.3.5/scan/database/pg.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/r2.py` & `hscan-3.3.5/scan/database/r2.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/rabbitmq.py` & `hscan-3.3.5/scan/database/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/redis.py` & `hscan-3.3.5/scan/database/redis.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/database/wasabi.py` & `hscan-3.3.5/scan/database/wasabi.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/downloade/aiohttp_downloader.py` & `hscan-3.3.5/scan/downloade/aiohttp_downloader.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/downloade/downloader.py` & `hscan-3.3.5/scan/downloade/downloader.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/log.py` & `hscan-3.3.5/scan/log.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/monitor.py` & `hscan-3.3.5/scan/monitor.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/response.py` & `hscan-3.3.5/scan/response.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/spider.py` & `hscan-3.3.5/scan/spider.py`

 * *Files identical despite different names*

### Comparing `hscan-3.3.4/scan/util.py` & `hscan-3.3.5/scan/util.py`

 * *Files identical despite different names*

