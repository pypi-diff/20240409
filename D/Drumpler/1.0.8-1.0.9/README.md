# Comparing `tmp/Drumpler-1.0.8.tar.gz` & `tmp/Drumpler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.8.tar", last modified: Mon Apr  8 20:51:13 2024, max compression
+gzip compressed data, was "Drumpler-1.0.9.tar", last modified: Tue Apr  9 19:26:38 2024, max compression
```

## Comparing `Drumpler-1.0.8.tar` & `Drumpler-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.566760 Drumpler-1.0.8/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.565359 Drumpler-1.0.8/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-08 20:51:13.000000 Drumpler-1.0.8/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.8/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-08 20:51:13.566139 Drumpler-1.0.8/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.8/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.560543 Drumpler-1.0.8/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.8/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.8/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     6945 2024-04-08 20:50:43.000000 Drumpler-1.0.8/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.8/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.8/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-08 20:51:13.566880 Drumpler-1.0.8/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-08 20:50:49.000000 Drumpler-1.0.8/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-08 20:51:13.564461 Drumpler-1.0.8/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.8/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.968396 Drumpler-1.0.9/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.966868 Drumpler-1.0.9/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.9/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 19:26:38.967625 Drumpler-1.0.9/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.9/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.961568 Drumpler-1.0.9/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.9/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.9/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     7118 2024-04-09 19:26:03.000000 Drumpler-1.0.9/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.9/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.9/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-09 19:26:38.968562 Drumpler-1.0.9/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-09 19:26:14.000000 Drumpler-1.0.9/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.965921 Drumpler-1.0.9/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.9/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.8/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.0.9/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.8/LICENSE` & `Drumpler-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.8/PKG-INFO` & `Drumpler-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.8/README.md` & `Drumpler-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.8/drumpler/constants.py` & `Drumpler-1.0.9/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.8/drumpler/drumpler.py` & `Drumpler-1.0.9/drumpler/drumpler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 from flask import Flask, request, jsonify
 from .constants import DRUMPLER_HOST, DRUMPLER_PORT, DRUMPLER_DEBUG, DATABASE_URI, AUTHORIZATION_KEY
 import json
 from flask_sqlalchemy import SQLAlchemy
 from .request import Request as BaseRequest
+from sqlalchemy import func
 
 app = Flask(__name__)
 app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
 app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 db = SQLAlchemy(app)
 
 class Request(db.Model, BaseRequest):
@@ -79,17 +80,21 @@
         db.session.add(new_request)
         db.session.commit()
         return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
     
     def __get_next_unhandled_request(self):
         with db.session.begin():
             unhandled_request = db.session.query(Request)\
-                .filter_by(is_handled=0, is_being_processed=False)\
-                .order_by(Request.id)\
-                .with_for_update(skip_locked=True).first()
+                .filter(
+                    Request.is_handled == 0, 
+                    Request.is_being_processed == False,
+                    Request.request_url.like(func.concat(self.host, '%'))
+                )\
+            .order_by(Request.id)\
+            .with_for_update(skip_locked=True).first()
 
             if unhandled_request:
                 # Prepare data before committing the transaction
                 request_data = {
                     "id": unhandled_request.id,
                     "timestamp": unhandled_request.timestamp.isoformat(),
                     "source_ip": unhandled_request.source_ip,
```

### Comparing `Drumpler-1.0.8/drumpler/mammoth.py` & `Drumpler-1.0.9/drumpler/mammoth.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.8/drumpler/request.py` & `Drumpler-1.0.9/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.8/setup.py` & `Drumpler-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.8',
+    version='1.0.9',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.8/test/test_drumpler.py` & `Drumpler-1.0.9/test/test_drumpler.py`

 * *Files identical despite different names*

