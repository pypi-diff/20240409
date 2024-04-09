# Comparing `tmp/flask-simplebook-0.6.0.tar.gz` & `tmp/flask-simplebook-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-simplebook-0.6.0.tar", last modified: Wed Apr  3 23:04:26 2024, max compression
+gzip compressed data, was "flask-simplebook-0.6.1.tar", last modified: Tue Apr  9 12:29:14 2024, max compression
```

## Comparing `flask-simplebook-0.6.0.tar` & `flask-simplebook-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-03 23:04:26.711934 flask-simplebook-0.6.0/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2476 2024-04-03 23:04:26.711934 flask-simplebook-0.6.0/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1987 2022-10-17 17:05:23.000000 flask-simplebook-0.6.0/README.md
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-03 23:04:26.707934 flask-simplebook-0.6.0/flask_simplebook.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2476 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      281 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        9 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       11 2024-04-03 23:04:26.000000 flask-simplebook-0.6.0/flask_simplebook.egg-info/top_level.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-04-03 23:04:26.711934 flask-simplebook-0.6.0/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      862 2024-04-03 23:02:07.000000 flask-simplebook-0.6.0/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-03 23:04:26.707934 flask-simplebook-0.6.0/simplebook/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3061 2022-10-24 16:24:31.000000 flask-simplebook-0.6.0/simplebook/app.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      272 2022-05-26 16:17:02.000000 flask-simplebook-0.6.0/simplebook/worker.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       73 2022-05-26 16:17:02.000000 flask-simplebook-0.6.0/simplebook/wsgi.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-09 12:29:14.831194 flask-simplebook-0.6.1/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    70267 2024-04-09 12:28:47.000000 flask-simplebook-0.6.1/LICENSE.md
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2501 2024-04-09 12:29:14.831194 flask-simplebook-0.6.1/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1987 2022-10-17 17:05:23.000000 flask-simplebook-0.6.1/README.md
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-09 12:29:14.831194 flask-simplebook-0.6.1/flask_simplebook.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2501 2024-04-09 12:29:14.000000 flask-simplebook-0.6.1/flask_simplebook.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      292 2024-04-09 12:29:14.000000 flask-simplebook-0.6.1/flask_simplebook.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2024-04-09 12:29:14.000000 flask-simplebook-0.6.1/flask_simplebook.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        9 2024-04-09 12:29:14.000000 flask-simplebook-0.6.1/flask_simplebook.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       11 2024-04-09 12:29:14.000000 flask-simplebook-0.6.1/flask_simplebook.egg-info/top_level.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2024-04-09 12:29:14.831194 flask-simplebook-0.6.1/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      862 2024-04-09 12:28:39.000000 flask-simplebook-0.6.1/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2024-04-09 12:29:14.831194 flask-simplebook-0.6.1/simplebook/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3061 2022-10-24 16:24:31.000000 flask-simplebook-0.6.1/simplebook/app.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      272 2022-05-26 16:17:02.000000 flask-simplebook-0.6.1/simplebook/worker.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       73 2022-05-26 16:17:02.000000 flask-simplebook-0.6.1/simplebook/wsgi.py
```

### Comparing `flask-simplebook-0.6.0/PKG-INFO` & `flask-simplebook-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: flask-simplebook
-Version: 0.6.0
+Version: 0.6.1
 Summary: flask app for SimpleBook
 Home-page: https://code.librehq.com/ots/mediawiki/SimpleBook
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: flask
 Requires-Dist: rq
 
 # flask-simplebook
 
 This is the flask companion application to the SimpleBook MediaWiki extension.
```

### Comparing `flask-simplebook-0.6.0/README.md` & `flask-simplebook-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-simplebook-0.6.0/flask_simplebook.egg-info/PKG-INFO` & `flask-simplebook-0.6.1/flask_simplebook.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: flask-simplebook
-Version: 0.6.0
+Version: 0.6.1
 Summary: flask app for SimpleBook
 Home-page: https://code.librehq.com/ots/mediawiki/SimpleBook
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: flask
 Requires-Dist: rq
 
 # flask-simplebook
 
 This is the flask companion application to the SimpleBook MediaWiki extension.
```

### Comparing `flask-simplebook-0.6.0/setup.py` & `flask-simplebook-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="flask-simplebook",
-    version="0.6.0",
+    version="0.6.1",
     description="flask app for SimpleBook",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Open Tech Strategies, LLC",
     author_email="frankduncan@opentechstrategies.com",  # For now, this works
     url="https://code.librehq.com/ots/mediawiki/SimpleBook",
     classifiers=[
```

### Comparing `flask-simplebook-0.6.0/simplebook/app.py` & `flask-simplebook-0.6.1/simplebook/app.py`

 * *Files identical despite different names*

