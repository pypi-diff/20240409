# Comparing `tmp/whatsapp_wrapper-0.1.1.tar.gz` & `tmp/whatsapp_wrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_wrapper-0.1.1.tar", last modified: Mon Apr  8 18:42:54 2024, max compression
+gzip compressed data, was "whatsapp_wrapper-0.1.2.tar", last modified: Tue Apr  9 05:12:40 2024, max compression
```

## Comparing `whatsapp_wrapper-0.1.1.tar` & `whatsapp_wrapper-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/whatsapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/media_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/message_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-04-08 18:42:44.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper/whatsapp_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:42:54.263351 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 18:42:54.000000 whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/whatsapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/audio_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/media_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/message_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-09 05:12:32.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper/whatsapp_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:12:40.534100 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 05:12:40.000000 whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/top_level.txt
```

### Comparing `whatsapp_wrapper-0.1.1/LICENSE` & `whatsapp_wrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.1/PKG-INFO` & `whatsapp_wrapper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp_wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.
 Home-page: https://github.com/AntonioVentilii/whatsapp-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/whatsapp-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/whatsapp-wrapper/issues
```

### Comparing `whatsapp_wrapper-0.1.1/README.md` & `whatsapp_wrapper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.1/setup.py` & `whatsapp_wrapper-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='whatsapp_wrapper',
-    version='0.1.1',
+    version='0.1.2',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
     description='Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AntonioVentilii/whatsapp-wrapper',
```

### Comparing `whatsapp_wrapper-0.1.1/whatsapp_wrapper/core.py` & `whatsapp_wrapper-0.1.2/whatsapp_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.1/whatsapp_wrapper/media_utilities.py` & `whatsapp_wrapper-0.1.2/whatsapp_wrapper/media_utilities.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.1/whatsapp_wrapper/message_object.py` & `whatsapp_wrapper-0.1.2/whatsapp_wrapper/message_object.py`

 * *Files identical despite different names*

### Comparing `whatsapp_wrapper-0.1.1/whatsapp_wrapper/whatsapp_db.py` & `whatsapp_wrapper-0.1.2/whatsapp_wrapper/whatsapp_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,19 +42,20 @@
         raise ValueError(f'Credentials file {file} not found')
     return encoded_json
 
 
 def clean_chat_data(messages: dict) -> list[dict]:
     cleaned_messages = [
         {
-            'body': message['text']['body'],
+            'body': message.get('text', {}).get('body'),
             'from': message.get('from'),
             'to': message.get('to'),
             'timestamp': message['timestamp'],
-        } for message in messages.values() if message.get('type') == 'text'
+        } for message in messages.values()
+        if message.get('type') is not None and message.get('text') is not None
     ]
     return cleaned_messages
 
 
 def find_message_chain(messages: dict, message_id: str) -> list[dict]:
     """
     Recursively finds a message chain based on message IDs in a context field, starting from the specified message ID.
```

### Comparing `whatsapp_wrapper-0.1.1/whatsapp_wrapper.egg-info/PKG-INFO` & `whatsapp_wrapper-0.1.2/whatsapp_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Integration layer for WhatsApp Cloud API with Firestore for easy message storage and management.
 Home-page: https://github.com/AntonioVentilii/whatsapp-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/whatsapp-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/whatsapp-wrapper/issues
```

