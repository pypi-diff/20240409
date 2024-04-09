# Comparing `tmp/cascadis-0.0.4.tar.gz` & `tmp/cascadis-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cascadis-0.0.4.tar", last modified: Fri Mar 22 11:11:40 2024, max compression
+gzip compressed data, was "cascadis-0.1.0.tar", last modified: Tue Apr  9 14:17:08 2024, max compression
```

## Comparing `cascadis-0.0.4.tar` & `cascadis-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 11:11:40.896646 cascadis-0.0.4/
--rw-r--r--   0 Hailong    (502) staff       (20)       84 2024-03-15 13:30:10.000000 cascadis-0.0.4/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1171 2024-03-22 11:11:40.896019 cascadis-0.0.4/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      239 2024-03-22 11:03:46.000000 cascadis-0.0.4/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 11:11:40.888925 cascadis-0.0.4/cascadis/
--rw-r--r--   0 Hailong    (502) staff       (20)       22 2024-03-22 11:11:14.000000 cascadis-0.0.4/cascadis/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)      411 2024-03-16 03:00:19.000000 cascadis-0.0.4/cascadis/__main__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2156 2024-03-15 13:30:10.000000 cascadis-0.0.4/cascadis/api.py
--rw-r--r--   0 Hailong    (502) staff       (20)      646 2024-03-22 09:32:31.000000 cascadis-0.0.4/cascadis/atx.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3074 2024-03-22 09:36:07.000000 cascadis-0.0.4/cascadis/auth.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 11:11:40.894294 cascadis-0.0.4/cascadis/cli/
--rw-r--r--   0 Hailong    (502) staff       (20)       74 2024-03-16 01:57:43.000000 cascadis-0.0.4/cascadis/cli/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2065 2024-03-22 09:34:33.000000 cascadis-0.0.4/cascadis/cli/get.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1800 2024-03-22 09:34:33.000000 cascadis-0.0.4/cascadis/cli/put.py
--rw-r--r--   0 Hailong    (502) staff       (20)      304 2024-03-22 09:34:33.000000 cascadis-0.0.4/cascadis/cli/shell.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2269 2024-03-22 09:32:31.000000 cascadis-0.0.4/cascadis/environ.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1088 2024-03-22 09:32:31.000000 cascadis-0.0.4/cascadis/misc.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3249 2024-03-22 09:32:31.000000 cascadis-0.0.4/cascadis/solutions.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 11:11:40.895364 cascadis-0.0.4/cascadis/templates/
--rw-r--r--   0 Hailong    (502) staff       (20)      432 2024-03-15 13:30:10.000000 cascadis-0.0.4/cascadis/templates/login.html
--rw-r--r--   0 Hailong    (502) staff       (20)      336 2024-03-15 13:30:10.000000 cascadis-0.0.4/cascadis/templates/upload.html
--rw-r--r--   0 Hailong    (502) staff       (20)      322 2024-03-16 01:25:48.000000 cascadis-0.0.4/cascadis/utils.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3898 2024-03-21 13:14:22.000000 cascadis-0.0.4/cascadis/views.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1350 2024-03-22 09:32:31.000000 cascadis-0.0.4/cascadis/viewutils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 11:11:40.891211 cascadis-0.0.4/cascadis.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1171 2024-03-22 11:11:40.000000 cascadis-0.0.4/cascadis.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      628 2024-03-22 11:11:40.000000 cascadis-0.0.4/cascadis.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-03-22 11:11:40.000000 cascadis-0.0.4/cascadis.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       89 2024-03-22 11:11:40.000000 cascadis-0.0.4/cascadis.egg-info/entry_points.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-03-15 13:35:31.000000 cascadis-0.0.4/cascadis.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)      181 2024-03-22 11:11:40.000000 cascadis-0.0.4/cascadis.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        9 2024-03-22 11:11:40.000000 cascadis-0.0.4/cascadis.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)      181 2024-03-15 14:10:33.000000 cascadis-0.0.4/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-03-22 11:11:40.896781 cascadis-0.0.4/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2141 2024-03-22 11:11:14.000000 cascadis-0.0.4/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:17:08.159444 cascadis-0.1.0/
+-rw-r--r--   0 Hailong    (502) staff       (20)       84 2024-03-15 13:30:10.000000 cascadis-0.1.0/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1199 2024-04-09 14:17:08.158792 cascadis-0.1.0/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      282 2024-04-09 14:16:23.000000 cascadis-0.1.0/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:17:08.144578 cascadis-0.1.0/cascadis/
+-rw-r--r--   0 Hailong    (502) staff       (20)       22 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      411 2024-03-16 03:00:19.000000 cascadis-0.1.0/cascadis/__main__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2156 2024-03-15 13:30:10.000000 cascadis-0.1.0/cascadis/api.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      646 2024-03-22 09:32:31.000000 cascadis-0.1.0/cascadis/atx.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3074 2024-03-22 09:36:07.000000 cascadis-0.1.0/cascadis/auth.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      425 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/cas.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:17:08.151912 cascadis-0.1.0/cascadis/cli/
+-rw-r--r--   0 Hailong    (502) staff       (20)       74 2024-03-16 01:57:43.000000 cascadis-0.1.0/cascadis/cli/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2065 2024-03-22 09:34:33.000000 cascadis-0.1.0/cascadis/cli/get.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2021 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/cli/put.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      356 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/cli/shell.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2265 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/environ.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1088 2024-03-22 09:32:31.000000 cascadis-0.1.0/cascadis/misc.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:17:08.155439 cascadis-0.1.0/cascadis/solutions/
+-rw-r--r--   0 Hailong    (502) staff       (20)     2968 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/solutions/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1010 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/solutions/inference.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1356 2024-04-02 15:36:40.000000 cascadis-0.1.0/cascadis/solutions/legacy.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      130 2024-04-03 01:14:20.000000 cascadis-0.1.0/cascadis/solutions/migrations.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1930 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/solutions/sessions.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:17:08.157187 cascadis-0.1.0/cascadis/templates/
+-rw-r--r--   0 Hailong    (502) staff       (20)      432 2024-03-15 13:30:10.000000 cascadis-0.1.0/cascadis/templates/login.html
+-rw-r--r--   0 Hailong    (502) staff       (20)      336 2024-03-15 13:30:10.000000 cascadis-0.1.0/cascadis/templates/upload.html
+-rw-r--r--   0 Hailong    (502) staff       (20)      322 2024-03-16 01:25:48.000000 cascadis-0.1.0/cascadis/utils.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4254 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/views.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1538 2024-04-09 14:16:23.000000 cascadis-0.1.0/cascadis/viewutils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:17:08.158067 cascadis-0.1.0/cascadis.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1199 2024-04-09 14:17:08.000000 cascadis-0.1.0/cascadis.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      778 2024-04-09 14:17:08.000000 cascadis-0.1.0/cascadis.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-09 14:17:08.000000 cascadis-0.1.0/cascadis.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       89 2024-04-09 14:17:08.000000 cascadis-0.1.0/cascadis.egg-info/entry_points.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-03-15 13:35:31.000000 cascadis-0.1.0/cascadis.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)      202 2024-04-09 14:17:08.000000 cascadis-0.1.0/cascadis.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        9 2024-04-09 14:17:08.000000 cascadis-0.1.0/cascadis.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)      201 2024-04-09 14:16:23.000000 cascadis-0.1.0/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-09 14:17:08.159571 cascadis-0.1.0/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2091 2024-04-09 14:16:23.000000 cascadis-0.1.0/setup.py
```

### Comparing `cascadis-0.0.4/PKG-INFO` & `cascadis-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: cascadis
-Version: 0.0.4
+Version: 0.1.0
 Summary: A simple content-addressed storage service.
 Home-page: https://github.com/frozflame/cascadis
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
 Requires-Dist: flask~=3.0.2
 Requires-Dist: joker-cast~=0.5.2
-Requires-Dist: joker-filesys~=0.2.1
+Requires-Dist: joker-filesys~=0.2.2
 Requires-Dist: joker-flasky~=0.6.0
 Requires-Dist: joker~=0.3.3
 Requires-Dist: pymongo~=4.6.2
 Requires-Dist: redis~=5.0.2
 Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=68.2.0
 Requires-Dist: volkanic~=0.5.1
 Requires-Dist: werkzeug~=3.0.1
+Requires-Dist: python-magic~=0.4.27
 
 Cascadis
 =========
 
-A simple content-addressed storage service.
+A content-addressed storage service.
+
+This project is currently at experimental stage.
 
 Install with `pip`:
 
     pip install cascadis
 
 For deployment, you may want to use `gunicorn`:
```

### Comparing `cascadis-0.0.4/cascadis/api.py` & `cascadis-0.1.0/cascadis/api.py`

 * *Files identical despite different names*

### Comparing `cascadis-0.0.4/cascadis/atx.py` & `cascadis-0.1.0/cascadis/atx.py`

 * *Files identical despite different names*

### Comparing `cascadis-0.0.4/cascadis/auth.py` & `cascadis-0.1.0/cascadis/auth.py`

 * *Files identical despite different names*

### Comparing `cascadis-0.0.4/cascadis/cli/get.py` & `cascadis-0.1.0/cascadis/cli/get.py`

 * *Files identical despite different names*

### Comparing `cascadis-0.0.4/cascadis/cli/put.py` & `cascadis-0.1.0/cascadis/cli/put.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,31 @@
 gi = GlobalInterface()
 
 
 class _CommandContext:
     def __init__(self, delete=False):
         self.delete = delete
 
-    def put_file_into_cas(self, path):
+    def _put_file_into_cas(self, path: str):
+        if self.delete and os.stat(path).st_dev == os.stat(gi.files).st_dev:
+            return gi.cas.seize(path)
         with open(path, "rb") as fin:
             content = fin.read()
             cid = gi.cas.save([content])
-            path = os.path.abspath(path)
-            print(cid, path)
-        register_cli_upload(cid, path)
         if self.delete:
             os.remove(path)
         return cid
 
+    def put_file_into_cas(self, path: str):
+        path = os.path.abspath(path)
+        cid = self._put_file_into_cas(path)
+        print(cid, path)
+        register_cli_upload(cid, path)
+        return cid
+
     def put_files_in_dir_into_cas(self, dirpath):
         executor = ThreadPoolExecutor(max_workers=10)
         paths = find_regular_files(dirpath)
         for batch in chunkwize(1000, paths):
             executor.map(self.put_file_into_cas, batch)
```

### Comparing `cascadis-0.0.4/cascadis/environ.py` & `cascadis-0.1.0/cascadis/environ.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 import logging
 import os
 from functools import cached_property
 from pathlib import Path
 
 import volkanic
-from joker.filesys.cas import ContentAddressedStorage
 from joker.redis import ErrorInterface
 from pymongo import MongoClient
 from pymongo.database import Database
 from redis import Redis
 from volkanic.utils import ignore_arguments, indented_json_print
 
+from cascadis.cas import ContentAddressedStorage
+
 _logger = logging.getLogger(__name__)
 
 
 class GlobalInterface(volkanic.GlobalInterface):
     package_name = "cascadis"
     default_config = {
         "cache_ttl": 0,
```

### Comparing `cascadis-0.0.4/cascadis/misc.py` & `cascadis-0.1.0/cascadis/misc.py`

 * *Files identical despite different names*

### Comparing `cascadis-0.0.4/cascadis/solutions.py` & `cascadis-0.1.0/cascadis/solutions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 #!/usr/bin/env python3
 # coding: utf-8
 from __future__ import annotations
 
 import datetime
-import os
+import logging
 import mimetypes
+import os
 from typing import Iterable, TypedDict
 
-import subprocess
 import pymongo.errors
 from flask import request
 
 from cascadis.environ import GlobalInterface
+from cascadis.solutions.inference import get_or_infer_content_type
+from cascadis.solutions.legacy import (
+    infer_mimetype_from_upload,
+    infer_mimetype_with_file_command,
+)
 
 gi = GlobalInterface()
+_logger = logging.getLogger(__name__)
 
 
 def query_by_file_id(file_id):
     coll = gi.mongodb.get_collection("file_registry")
     cursor = coll.find({"file_id": file_id})
     return list(cursor)
 
@@ -96,34 +102,14 @@
         "filename": filename,
     }
     coll.insert_one(record)
     if mimetype:
         register_object(cid, mimetype)
 
 
-def infer_mimetype_from_upload(cid: str) -> str:
-    coll = gi.mongodb["uploads"]
-    record = coll.find_one(
-        {"cid": cid},
-        sort=[("_id", -1)],
-        projection=["mimetype"],
-    )
-    if record:
-        return record["mimetype"]
-
-
-def infer_mimetype_with_file_command(cid: str) -> str:
-    path = gi.cas.locate(cid)
-    cmd = ["file", "--mime-type", str(path)]
-    proc = subprocess.run(cmd, capture_output=True, text=True)
-    return proc.stdout.split()[-1]
-
-
-# def update_
-
 if __name__ == "__main__":
     print(
         infer_mimetype_with_file_command(
             "3543069d447f8ef042b5f0500e36a9b787f9288a064dd38905f4147169f9c476"
         )
     )
     print(
```

### Comparing `cascadis-0.0.4/cascadis/views.py` & `cascadis-0.1.0/cascadis/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 import logging
 import mimetypes
 import os.path
 
 import flask
 from flask import Blueprint, request, Response
 
-from cascadis.auth import set_protection_level, LoginInterface, login_required
+from cascadis.auth import set_protection_level, LoginInterface
 from cascadis.environ import GlobalInterface
 from cascadis.solutions import register_http_upload
-from cascadis.viewutils import Proxy, fmt_content_disposition_attachment
+from cascadis.solutions.sessions import Session
+from cascadis.viewutils import (
+    Proxy, fmt_content_disposition
+)
 
 gi = GlobalInterface()
 bp = Blueprint("cas", __name__)
 _logger = logging.getLogger(__name__)
 
 
 def _read_uploading_file_in_chunks(chunksize=16384):
@@ -51,21 +54,14 @@
     LoginInterface.install_builtin_users()
     username = request.form["username"]
     password = request.form["password"]
     li = LoginInterface.login(username, password)
     return {"code": 0, "data": li.userinfo}
 
 
-@bp.route("/help")
-@set_protection_level(2)
-@login_required
-def api_help():
-    return "help"
-
-
 @bp.route("/cas/files", methods=["GET", "POST"])
 @bp.route("/cascadis/files", methods=["GET", "POST"])
 @set_protection_level(2)
 def api_upload():
     # if request.method == "GET":
     #     return pages.respond_upload_page()
     # chunks = read_uploading_file()
@@ -89,14 +85,16 @@
     }
     resp.headers.update(headers)
     return resp
 
 
 @bp.route("/cas/files/<cname>")
 @bp.route("/cascadis/files/<cname>")
+@bp.route("/cas/c/<cname>")
+@bp.route("/cascadis/content/<cname>")
 @set_protection_level(1)
 def api_download(cname: str):
     # TODO: support Content-Length on GET/HEAD
     # TODO: use HEAD method on HEAD proxy
     cid, ext = os.path.splitext(cname)
     if len(cid) != 64:
         return flask.abort(404)
@@ -115,10 +113,22 @@
     else:
         chunks = gi.cas.load(cid)
     # https://flask.palletsprojects.com/en/2.1.x/patterns/streaming/#basic-usage
     resp = Response(chunks, mimetype=mimetype)
     if mimetype == default_mimetype:
         resp.headers["Content-Disposition"] = "inline"
     elif filename != cname:
-        content_dispos = fmt_content_disposition_attachment(filename)
+        content_dispos = fmt_content_disposition(filename, attachment=True)
         resp.headers["Content-Disposition"] = content_dispos
     return resp
+
+
+@bp.route("/cas/s/<session_id>")
+@bp.route("/cascadis/session/<session_id>")
+def view_public(session_id):
+    try:
+        session = Session.load(session_id)
+    except FileNotFoundError:
+        return flask.abort(404)
+    chunks = gi.cas.load(session.cid)
+    print(session, "----")
+    return Response(chunks, content_type=session.content_type)
```

### Comparing `cascadis-0.0.4/cascadis/viewutils.py` & `cascadis-0.1.0/cascadis/viewutils.py`

 * *Files 27% similar despite different names*

```diff
@@ -38,10 +38,15 @@
             content_type=resp.headers["Content-Type"],
         )
         if disposition := resp.headers.get("Content-Disposition"):
             ret_resp.headers["Content-Disposition"] = disposition
         return ret_resp
 
 
-def fmt_content_disposition_attachment(filename: str):
+def fmt_content_disposition(filename: str, attachment=False) -> str:
     quoted = urllib.parse.quote(filename)
-    return f'''attachment; filename="{quoted}"; filename*="UTF-8''{quoted}"'''
+    kind = "attachment" if attachment else "inline"
+    return f'''{kind}; filename="{quoted}"; filename*="UTF-8''{quoted}"'''
+
+
+def fmt_content_disposition_attachment(filename: str) -> str:
+    return fmt_content_disposition(filename, attachment=True)
```

### Comparing `cascadis-0.0.4/cascadis.egg-info/PKG-INFO` & `cascadis-0.1.0/cascadis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: cascadis
-Version: 0.0.4
+Version: 0.1.0
 Summary: A simple content-addressed storage service.
 Home-page: https://github.com/frozflame/cascadis
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
 Requires-Dist: flask~=3.0.2
 Requires-Dist: joker-cast~=0.5.2
-Requires-Dist: joker-filesys~=0.2.1
+Requires-Dist: joker-filesys~=0.2.2
 Requires-Dist: joker-flasky~=0.6.0
 Requires-Dist: joker~=0.3.3
 Requires-Dist: pymongo~=4.6.2
 Requires-Dist: redis~=5.0.2
 Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=68.2.0
 Requires-Dist: volkanic~=0.5.1
 Requires-Dist: werkzeug~=3.0.1
+Requires-Dist: python-magic~=0.4.27
 
 Cascadis
 =========
 
-A simple content-addressed storage service.
+A content-addressed storage service.
+
+This project is currently at experimental stage.
 
 Install with `pip`:
 
     pip install cascadis
 
 For deployment, you may want to use `gunicorn`:
```

### Comparing `cascadis-0.0.4/cascadis.egg-info/SOURCES.txt` & `cascadis-0.1.0/cascadis.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 requirements.txt
 setup.py
 cascadis/__init__.py
 cascadis/__main__.py
 cascadis/api.py
 cascadis/atx.py
 cascadis/auth.py
+cascadis/cas.py
 cascadis/environ.py
 cascadis/misc.py
-cascadis/solutions.py
 cascadis/utils.py
 cascadis/views.py
 cascadis/viewutils.py
 cascadis.egg-info/PKG-INFO
 cascadis.egg-info/SOURCES.txt
 cascadis.egg-info/dependency_links.txt
 cascadis.egg-info/entry_points.txt
 cascadis.egg-info/not-zip-safe
 cascadis.egg-info/requires.txt
 cascadis.egg-info/top_level.txt
 cascadis/cli/__init__.py
 cascadis/cli/get.py
 cascadis/cli/put.py
 cascadis/cli/shell.py
+cascadis/solutions/__init__.py
+cascadis/solutions/inference.py
+cascadis/solutions/legacy.py
+cascadis/solutions/migrations.py
+cascadis/solutions/sessions.py
 cascadis/templates/login.html
 cascadis/templates/upload.html
```

### Comparing `cascadis-0.0.4/setup.py` & `cascadis-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
             'cas = cascadis.__main__:registry',
             'cascadis = cascadis.__main__:registry',
         ]
     },
     'classifiers': [
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: 3.13',
     ],
     # ensure copy static file to runtime directory
     'include_package_data': True,
     'long_description': read('README.md'),
```

