# Comparing `tmp/line-web-0.0.3.tar.gz` & `tmp/line-web-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-web-0.0.3.tar", last modified: Tue Apr  9 03:54:31 2024, max compression
+gzip compressed data, was "line-web-0.0.4.tar", last modified: Tue Apr  9 07:05:51 2024, max compression
```

## Comparing `line-web-0.0.3.tar` & `line-web-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:54:31.798410 line-web-0.0.3/
--rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 line-web-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 line-web-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1661 2024-04-09 03:54:31.798410 line-web-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      960 2024-04-03 10:07:33.000000 line-web-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 03:54:31.782635 line-web-0.0.3/line/
--rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 line-web-0.0.3/line/__init__.py
--rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 line-web-0.0.3/line/authentications.py
--rw-rw-rw-   0        0        0    33330 2024-04-09 03:53:25.000000 line-web-0.0.3/line/core.py
--rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 line-web-0.0.3/line/exceptions.py
--rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 line-web-0.0.3/line/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:54:31.782635 line-web-0.0.3/line_web.egg-info/
--rw-rw-rw-   0        0        0     1661 2024-04-09 03:54:31.000000 line-web-0.0.3/line_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-09 03:54:31.000000 line-web-0.0.3/line_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:54:31.000000 line-web-0.0.3/line_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-09 03:54:31.000000 line-web-0.0.3/line_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-09 03:54:31.000000 line-web-0.0.3/line_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 03:54:31.798410 line-web-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3899 2024-04-09 03:53:52.000000 line-web-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:05:51.262975 line-web-0.0.4/
+-rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 line-web-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 line-web-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1661 2024-04-09 07:05:51.262975 line-web-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2024-04-03 10:07:33.000000 line-web-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:05:51.262975 line-web-0.0.4/line/
+-rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 line-web-0.0.4/line/__init__.py
+-rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 line-web-0.0.4/line/authentications.py
+-rw-rw-rw-   0        0        0    33340 2024-04-09 07:05:22.000000 line-web-0.0.4/line/core.py
+-rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 line-web-0.0.4/line/exceptions.py
+-rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 line-web-0.0.4/line/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:05:51.262975 line-web-0.0.4/line_web.egg-info/
+-rw-rw-rw-   0        0        0     1661 2024-04-09 07:05:51.000000 line-web-0.0.4/line_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-09 07:05:51.000000 line-web-0.0.4/line_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:05:51.000000 line-web-0.0.4/line_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-09 07:05:51.000000 line-web-0.0.4/line_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-09 07:05:51.000000 line-web-0.0.4/line_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 07:05:51.262975 line-web-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3899 2024-04-09 07:05:22.000000 line-web-0.0.4/setup.py
```

### Comparing `line-web-0.0.3/LICENSE` & `line-web-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `line-web-0.0.3/PKG-INFO` & `line-web-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-web
-Version: 0.0.3
+Version: 0.0.4
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-web
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `line-web-0.0.3/README.md` & `line-web-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `line-web-0.0.3/line/authentications.py` & `line-web-0.0.4/line/authentications.py`

 * *Files identical despite different names*

### Comparing `line-web-0.0.3/line/core.py` & `line-web-0.0.4/line/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ORDER_BY = typing.Literal["ASC", "DESC"]
 
 
 class Line:
 
     def __init__(
         self,
-        authentication: CookieAuthentication | BusinessAuthentication | BrowserAuthentication,
+        authentication: typing.Union[CookieAuthentication|BusinessAuthentication|BrowserAuthentication],
         bot: str,
         client_type: typing.Optional[str] = "PC",
         device_type: typing.Optional[str] = "",
         ping_secs: typing.Optional[int] = 60,
         streaming_token_retries: typing.Optional[int] = 0.5,
         __x_oa_chat_client_version: typing.Optional[str] = "20230404142351"
     ):
```

### Comparing `line-web-0.0.3/line_web.egg-info/PKG-INFO` & `line-web-0.0.4/line_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-web
-Version: 0.0.3
+Version: 0.0.4
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-web
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `line-web-0.0.3/setup.py` & `line-web-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'line-web'
 DESCRIPTION = 'Line chatbot framework.'
 URL = 'https://github.com/miloira/line-web'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'loguru',
     'pyee'
 ]
```

