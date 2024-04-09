# Comparing `tmp/whatsapp_wrapper-0.1.3.tar.gz` & `tmp/whatsapp_wrapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_wrapper-0.1.3.tar", last modified: Tue Apr  9 12:38:43 2024, max compression
+gzip compressed data, was "whatsapp_wrapper-0.1.4.tar", last modified: Tue Apr  9 13:25:30 2024, max compression
```

## Comparing `whatsapp_wrapper-0.1.3.tar` & `whatsapp_wrapper-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:38:43.086315 whatsapp_wrapper-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 12:38:43.082315 whatsapp_wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:38:43.086315 whatsapp_wrapper-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:38:43.082315 whatsapp_wrapper-0.1.3/whatsapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/audio_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/media_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/message_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-09 12:38:31.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper/whatsapp_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:38:43.082315 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 12:38:43.000000 whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:25:30.480734 whatsapp_wrapper-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 13:25:30.480734 whatsapp_wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:25:30.480734 whatsapp_wrapper-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:25:30.480734 whatsapp_wrapper-0.1.4/whatsapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/audio_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/media_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/message_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-09 13:25:22.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper/whatsapp_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:25:30.480734 whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 13:25:30.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 13:25:30.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:25:30.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 13:25:30.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 13:25:30.000000 whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/top_level.txt
```

### Comparing `whatsapp_wrapper-0.1.3/LICENSE` & `whatsapp_wrapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.3/PKG-INFO` & `whatsapp_wrapper-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp_wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.
 Home-page: https://github.com/AntonioVentilii/whatsapp-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/whatsapp-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/whatsapp-wrapper/issues
```

### Comparing `whatsapp_wrapper-0.1.3/README.md` & `whatsapp_wrapper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.3/setup.py` & `whatsapp_wrapper-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='whatsapp_wrapper',
-    version='0.1.3',
+    version='0.1.4',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
     description='Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AntonioVentilii/whatsapp-wrapper',
```

### Comparing `whatsapp_wrapper-0.1.3/whatsapp_wrapper/audio_utilities.py` & `whatsapp_wrapper-0.1.4/whatsapp_wrapper/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.3/whatsapp_wrapper/core.py` & `whatsapp_wrapper-0.1.4/whatsapp_wrapper/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
     def mark_as_read(self, message_id: str) -> dict:
         data = {
             "messaging_product": "whatsapp",
             "status": "read",
             "message_id": message_id,
         }
-        ret = self._send_message(data)
+        ret = self._send_message(data, save_to_db=False)
         return ret
 
     def send_text(self, to: str, message: str, preview_url: bool = False,
                   reply_to_message_id: str = None, save_to_db: bool = True) -> dict:
         message_obj = MessageObject(to, reply_to_message_id=reply_to_message_id)
         payload = message_obj.text(message, preview_url=preview_url)
         ret = self._send_message(payload, save_to_db=save_to_db)
```

### Comparing `whatsapp_wrapper-0.1.3/whatsapp_wrapper/media_utilities.py` & `whatsapp_wrapper-0.1.4/whatsapp_wrapper/media_utilities.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.3/whatsapp_wrapper/message_object.py` & `whatsapp_wrapper-0.1.4/whatsapp_wrapper/message_object.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.3/whatsapp_wrapper/whatsapp_db.py` & `whatsapp_wrapper-0.1.4/whatsapp_wrapper/whatsapp_db.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.3/whatsapp_wrapper.egg-info/PKG-INFO` & `whatsapp_wrapper-0.1.4/whatsapp_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.
 Home-page: https://github.com/AntonioVentilii/whatsapp-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/whatsapp-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/whatsapp-wrapper/issues
```

