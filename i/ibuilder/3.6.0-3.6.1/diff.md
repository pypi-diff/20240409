# Comparing `tmp/ibuilder-3.6.0.tar.gz` & `tmp/ibuilder-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibuilder-3.6.0.tar", max compression
+gzip compressed data, was "ibuilder-3.6.1.tar", max compression
```

## Comparing `ibuilder-3.6.0.tar` & `ibuilder-3.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.6.0/LICENSE
--rw-r--r--   0        0        0     5130 2024-04-05 09:24:54.705266 ibuilder-3.6.0/README.md
--rw-r--r--   0        0        0        0 2024-01-06 11:55:51.913157 ibuilder-3.6.0/ibuilder/__init__.py
--rw-r--r--   0        0        0       43 2024-01-06 11:55:51.916490 ibuilder-3.6.0/ibuilder/__main__.py
--rw-r--r--   0        0        0     4231 2024-01-06 11:55:51.919824 ibuilder-3.6.0/ibuilder/config/config.py
--rw-r--r--   0        0        0     2124 2024-04-04 20:37:02.132422 ibuilder-3.6.0/ibuilder/config/models.py
--rwxr-xr-x   0        0        0     5877 2024-04-05 09:16:29.587532 ibuilder-3.6.0/ibuilder/history.py
--rwxr-xr-x   0        0        0     3748 2024-01-06 12:03:11.386576 ibuilder-3.6.0/ibuilder/images.py
--rwxr-xr-x   0        0        0    14079 2024-04-05 09:19:24.556372 ibuilder-3.6.0/ibuilder/main.py
--rw-r--r--   0        0        0     1564 2024-04-05 09:15:56.066470 ibuilder-3.6.0/ibuilder/models.py
--rw-r--r--   0        0        0    15058 2024-01-06 11:55:51.909823 ibuilder-3.6.0/ibuilder/utils.py
--rw-r--r--   0        0        0      890 2024-04-04 18:58:11.184246 ibuilder-3.6.0/pyproject.toml
--rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 ibuilder-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.6.1/LICENSE
+-rw-r--r--   0        0        0     5130 2024-04-05 09:24:54.705266 ibuilder-3.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-01-06 11:55:51.913157 ibuilder-3.6.1/ibuilder/__init__.py
+-rw-r--r--   0        0        0       43 2024-01-06 11:55:51.916490 ibuilder-3.6.1/ibuilder/__main__.py
+-rw-r--r--   0        0        0     4231 2024-01-06 11:55:51.919824 ibuilder-3.6.1/ibuilder/config/config.py
+-rw-r--r--   0        0        0     2146 2024-04-09 15:47:47.718510 ibuilder-3.6.1/ibuilder/config/models.py
+-rwxr-xr-x   0        0        0     6005 2024-04-05 09:31:38.769033 ibuilder-3.6.1/ibuilder/history.py
+-rwxr-xr-x   0        0        0     3748 2024-01-06 12:03:11.386576 ibuilder-3.6.1/ibuilder/images.py
+-rwxr-xr-x   0        0        0    13936 2024-04-05 09:40:19.536378 ibuilder-3.6.1/ibuilder/main.py
+-rw-r--r--   0        0        0     1564 2024-04-05 09:15:56.066470 ibuilder-3.6.1/ibuilder/models.py
+-rw-r--r--   0        0        0    15058 2024-01-06 11:55:51.909823 ibuilder-3.6.1/ibuilder/utils.py
+-rw-r--r--   0        0        0      890 2024-04-09 15:39:16.076014 ibuilder-3.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 ibuilder-3.6.1/PKG-INFO
```

### Comparing `ibuilder-3.6.0/LICENSE` & `ibuilder-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.0/README.md` & `ibuilder-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.0/ibuilder/config/config.py` & `ibuilder-3.6.1/ibuilder/config/config.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.0/ibuilder/config/models.py` & `ibuilder-3.6.1/ibuilder/config/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 class PushRegistry(BaseModel):
     """
     Push registry components such as url, username, etc.
     """
 
     url: str | None
     username: str | None
-    password: str | None
-    email: str | None
+    password: Optional[str] | None
+    # email: Optional[str] | None
 
 
 class Push(BaseModel):
     """
     Push components such as the image, registry, and docker config path.
     """
```

### Comparing `ibuilder-3.6.0/ibuilder/history.py` & `ibuilder-3.6.1/ibuilder/history.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,20 +43,28 @@
     table.add_column("Calling Params")
     table.add_column("B/L/S/P")
     table.add_column("Version")
 
     history = db.table("history").all()
     if history:
         for r in history:
-            r['doc_id'] = str(r.doc_id)
-            r['build_logs'] = '' if not 'build_logs' in r else r['build_logs']
-            r['tag_source_logs'] = '' if not 'tag_source_logs' in r else r['tag_source_logs']
-            r['tag_source_push_logs'] = '' if not 'tag_source_push_logs' in r else r['tag_source_push_logs']
-            r['image_push_logs'] = '' if not 'image_push_logs' in r else r['image_push_logs']
-            r['image_push_latest_logs'] = '' if not 'image_push_latest_logs' in r else r['image_push_latest_logs']
+            r["doc_id"] = str(r.doc_id)
+            r["build_logs"] = "" if "build_logs" not in r else r["build_logs"]
+            r["tag_source_logs"] = (
+                "" if "tag_source_logs" not in r else r["tag_source_logs"]
+            )
+            r["tag_source_push_logs"] = (
+                "" if "tag_source_push_logs" not in r else r["tag_source_push_logs"]
+            )
+            r["image_push_logs"] = (
+                "" if "image_push_logs" not in r else r["image_push_logs"]
+            )
+            r["image_push_latest_logs"] = (
+                "" if "image_push_latest_logs" not in r else r["image_push_latest_logs"]
+            )
             h = HistoryOnDB(**r)
             blsp = []
             ver = ""
             if h.run_params:
                 blsp.append(completed(h.run_params["build"]["image"]))
                 blsp.append(completed(h.run_params["build"]["tag_image_latest"]))
                 blsp.append(completed(h.run_params["source"]["tag"]))
@@ -77,15 +85,15 @@
     return False
 
 
 def history_detail(db, id):
     """Show history detail (all info for a specific history item)."""
 
     r = db.table("history").get(doc_id=id)
-    r['doc_id'] = str(id)
+    r["doc_id"] = str(id)
     h = HistoryOnDB(**r)
 
     brief = Table(
         title="History Detail",
         show_header=True,
         show_edge=True,
         show_lines=True,
```

### Comparing `ibuilder-3.6.0/ibuilder/images.py` & `ibuilder-3.6.1/ibuilder/images.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.0/ibuilder/main.py` & `ibuilder-3.6.1/ibuilder/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
 #  Copyright 2023 drad <sa@adercon.com>
 
 import logging
-import tomli
 from datetime import datetime
 from os import getenv
 from typing import List, Optional
 
 import typer
 from rich import print
 from rich.console import Console
@@ -40,15 +39,15 @@
 logger_base = logging.getLogger("default")
 logger_base.setLevel(logging.getLevelName(getenv("LOG_LEVEL", "INFO")))
 logger_base.addHandler(logging.StreamHandler())
 logger = logging.LoggerAdapter(logging.getLogger("default"))
 
 app = typer.Typer(
     pretty_exceptions_enable=False,
-    help="build, tag, and push images\n\nNOTE: set LOG_LEVEL environment variable to adjust logging (e.g. $ LOG_LEVEL=DEBUG ib build -i minor)"
+    help="build, tag, and push images\n\nNOTE: set LOG_LEVEL environment variable to adjust logging (e.g. $ LOG_LEVEL=DEBUG ib build -i minor)",
 )
 app.add_typer(ibuilder.history.app, name="history")
 app.add_typer(ibuilder.images.app, name="images")
 
 _prj = None
 _db = None
 
@@ -337,21 +336,20 @@
         logger.debug(f"- sign image flag is: {_sign}")
         image_repush(r, _sign)
 
 
 def version_callback(value: bool):
     """
     Show version.
-    NOTICE: we load the pyproject.toml here (rather than a config) so its not loaded on normal app usage as it is not needed then.
     """
 
     import importlib.metadata
 
     if value:
-        _meta = importlib.metadata.metadata('ibuilder')
+        _meta = importlib.metadata.metadata("ibuilder")
         _name = _meta["Name"]
         _version = _meta["Version"]
         typer.echo(f"{_name} {_version}")
         raise typer.Exit()
 
 
 @app.callback()
```

### Comparing `ibuilder-3.6.0/ibuilder/models.py` & `ibuilder-3.6.1/ibuilder/models.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.0/ibuilder/utils.py` & `ibuilder-3.6.1/ibuilder/utils.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.0/pyproject.toml` & `ibuilder-3.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [internal]
 created = 2019-06-15
 modified = 2024-01-06
 
 [tool.poetry]
 name = "ibuilder"
-version = "3.6.0"
+version = "3.6.1"
 description = "build, tag, push, and sign docker images"
 authors = ["drad <sa@adercon.com>"]
 maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/ibuilder"
 repository = "https://gitlab.com/drad/ibuilder"
```

### Comparing `ibuilder-3.6.0/PKG-INFO` & `ibuilder-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibuilder
-Version: 3.6.0
+Version: 3.6.1
 Summary: build, tag, push, and sign docker images
 Home-page: https://gitlab.com/drad/ibuilder
 License: GPL-3.0-only
 Keywords: cli,docker,containers,build,ci,cd,image,tag,git,push,sign,cosign
 Author: drad
 Author-email: sa@adercon.com
 Maintainer: drad
```

