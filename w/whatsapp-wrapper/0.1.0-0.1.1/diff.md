# Comparing `tmp/whatsapp_wrapper-0.1.0.tar.gz` & `tmp/whatsapp_wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_wrapper-0.1.0.tar", last modified: Mon Apr  8 17:34:54 2024, max compression
+gzip compressed data, was "whatsapp_wrapper-0.1.1.tar", last modified: Mon Apr  8 18:42:54 2024, max compression
```

## Comparing `whatsapp_wrapper-0.1.0.tar` & `whatsapp_wrapper-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:34:54.975346 whatsapp_wrapper-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 17:34:54.975346 whatsapp_wrapper-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:34:54.975346 whatsapp_wrapper-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:34:54.975346 whatsapp_wrapper-0.1.0/whatsapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/media_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/message_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-08 17:34:35.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper/whatsapp_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:34:54.975346 whatsapp_wrapper-0.1.0/whatsapp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 17:34:54.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:34:54.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:34:54.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 17:34:54.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 17:34:54.000000 whatsapp_wrapper-0.1.0/whatsapp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/whatsapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/media_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/message_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/whatsapp_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/top_level.txt
```

### Comparing `whatsapp_wrapper-0.1.0/LICENSE` & `whatsapp_wrapper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.0/setup.py` & `whatsapp_wrapper-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='whatsapp_wrapper',
-    version='0.1.0',
+    version='0.1.1',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
     description='Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AntonioVentilii/whatsapp-wrapper',
@@ -25,15 +25,18 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='WhatsApp, Firestore, API, integration, messaging',
     install_requires=[
         'requests',
-        'firestore-wrapper'
+        'firestore-wrapper',
+        'pydub',
+        'ffmpeg-downloader',
+        'ffmpeg-python',
     ],
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
         ],
     },
 )
```

### Comparing `whatsapp_wrapper-0.1.0/whatsapp_wrapper/core.py` & `whatsapp_wrapper-0.1.1/whatsapp_wrapper/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from __future__ import annotations
 
 import time
 import warnings
-from typing import Any, Callable, Optional
 
 import requests
 from requests import Response
 
 from .configs import BASE_URL, LAST_API_VERSION
 from .exceptions import WhatsAppAPIWarning
 from .media_utilities import check_media_type_supported, save_media_to_temp_cache
 from .message_object import MessageObject
 from .whatsapp_db import DatabaseConfig, WhatsAppDB, configure_database
 
-ErrorHandlerType = Callable[[Response, dict], Optional[Any]]
 
-
-def _default_error_handler(response: Response, data: dict):
+def _default_error_handler(_, response: Response, data: dict):
     status_code = response.status_code
     error_message = (
         f"Request was failed with status code: {status_code}."
         f" Data: {data}"
     )
     raise Exception(error_message)
 
@@ -29,25 +26,34 @@
     BASE_URL = BASE_URL
     DEFAULT_API_VERSION = LAST_API_VERSION
 
     _MESSAGE_URI = 'messages'
     _MEDIA_URI = 'media'
 
     def __init__(self, mobile_id: str, api_token: str, version: str = LAST_API_VERSION,
-                 database_config: DatabaseConfig = None, error_handler: ErrorHandlerType = None):
+                 database_config: DatabaseConfig = None, error_handler=None):
         self.mobile_id = mobile_id
         self.bearer_token = api_token
         self.version = version or self.DEFAULT_API_VERSION
         if database_config is None:
             self._db = None
             txt = "Database configuration is not provided. Chats will not be saved."
             warnings.warn(txt, WhatsAppAPIWarning)
         else:
             self._db = configure_database(database_config)
-        self.error_handler: Callable[[Response, dict | None], Any | None] = error_handler or _default_error_handler
+        self.error_handler = self._custom_error_handler_factory(error_handler or _default_error_handler)
+
+    def _custom_error_handler_factory(self, external_error_handler):
+        """Bind an external error handler to the current instance."""
+
+        def error_handler(response: Response, data: dict):
+            # Call the external error handler with self as the first argument
+            external_error_handler(self, response, data)
+
+        return error_handler
 
     @property
     def db(self) -> WhatsAppDB:
         return self._db
 
     @property
     def base_url(self):
```

### Comparing `whatsapp_wrapper-0.1.0/whatsapp_wrapper/media_utilities.py` & `whatsapp_wrapper-0.1.1/whatsapp_wrapper/media_utilities.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.0/whatsapp_wrapper/message_object.py` & `whatsapp_wrapper-0.1.1/whatsapp_wrapper/message_object.py`

 * *Files identical despite different names*

