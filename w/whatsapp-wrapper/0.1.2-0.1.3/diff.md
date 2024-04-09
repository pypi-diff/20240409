# Comparing `tmp/whatsapp_wrapper-0.1.2.tar.gz` & `tmp/whatsapp_wrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_wrapper-0.1.2.tar", last modified: Tue Apr  9 05:12:40 2024, max compression
+gzip compressed data, was "whatsapp_wrapper-0.1.3.tar", last modified: Tue Apr  9 12:38:43 2024, max compression
```

## Comparing `whatsapp_wrapper-0.1.2.tar` & `whatsapp_wrapper-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/whatsapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/audio_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/media_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/message_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/whatsapp_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:38:43.086315 whatsapp_wrapper-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 12:38:43.082315 whatsapp_wrapper-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:38:43.086315 whatsapp_wrapper-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:38:43.082315 whatsapp_wrapper-0.1.3/whatsapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/audio_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/media_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/message_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/whatsapp_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:38:43.082315 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/top_level.txt
```

### Comparing `whatsapp_wrapper-0.1.2/LICENSE` & `whatsapp_wrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.2/PKG-INFO` & `whatsapp_wrapper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp_wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.
 Home-page: https://github.com/AntonioVentilii/whatsapp-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/whatsapp-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/whatsapp-wrapper/issues
```

### Comparing `whatsapp_wrapper-0.1.2/README.md` & `whatsapp_wrapper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.2/setup.py` & `whatsapp_wrapper-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='whatsapp_wrapper',
-    version='0.1.2',
+    version='0.1.3',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
     description='Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AntonioVentilii/whatsapp-wrapper',
```

### Comparing `whatsapp_wrapper-0.1.2/whatsapp_wrapper/audio_utilities.py` & `whatsapp_wrapper-0.1.3/whatsapp_wrapper/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.2/whatsapp_wrapper/core.py` & `whatsapp_wrapper-0.1.3/whatsapp_wrapper/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         if database_config is None:
             self._db = None
             txt = "Database configuration is not provided. Chats will not be saved."
             warnings.warn(txt, WhatsAppAPIWarning)
         else:
             self._db = configure_database(database_config)
         self.error_handler = self._custom_error_handler_factory(error_handler or _default_error_handler)
+        self._banned_users = []
 
     def _custom_error_handler_factory(self, external_error_handler):
         """Bind an external error handler to the current instance."""
 
         def error_handler(response: Response, data: dict):
             # Call the external error handler with self as the first argument
             external_error_handler(self, response, data)
@@ -52,14 +53,28 @@
         return error_handler
 
     @property
     def db(self) -> WhatsAppDB:
         return self._db
 
     @property
+    def banned_users(self) -> list[str]:
+        if self.db:
+            db_banned_users = self.db.list_banned_user_names()
+        else:
+            db_banned_users = []
+        ret = self._banned_users + db_banned_users
+        ret = list(set(ret))
+        return ret
+
+    @banned_users.setter
+    def banned_users(self, value: list[str]):
+        self._banned_users = value
+
+    @property
     def base_url(self):
         return f'{self.BASE_URL}/{self.version}'
 
     @property
     def mobile_url(self):
         return f'{self.base_url}/{self.mobile_id}'
```

### Comparing `whatsapp_wrapper-0.1.2/whatsapp_wrapper/media_utilities.py` & `whatsapp_wrapper-0.1.3/whatsapp_wrapper/media_utilities.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.2/whatsapp_wrapper/message_object.py` & `whatsapp_wrapper-0.1.3/whatsapp_wrapper/message_object.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.2/whatsapp_wrapper/whatsapp_db.py` & `whatsapp_wrapper-0.1.3/whatsapp_wrapper/whatsapp_db.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/PKG-INFO` & `whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.
 Home-page: https://github.com/AntonioVentilii/whatsapp-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/whatsapp-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/whatsapp-wrapper/issues
```

