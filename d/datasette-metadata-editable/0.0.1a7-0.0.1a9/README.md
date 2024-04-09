# Comparing `tmp/datasette-metadata-editable-0.0.1a7.tar.gz` & `tmp/datasette-metadata-editable-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-metadata-editable-0.0.1a7.tar", last modified: Thu Oct 26 18:46:45 2023, max compression
+gzip compressed data, was "datasette-metadata-editable-0.0.1a9.tar", last modified: Thu Oct 26 19:39:15 2023, max compression
```

## Comparing `datasette-metadata-editable-0.0.1a7.tar` & `datasette-metadata-editable-0.0.1a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:45.616631 datasette-metadata-editable-0.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-26 18:46:45.616631 datasette-metadata-editable-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:45.612630 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/internal_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:45.612630 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/static/plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:45.612630 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/templates/edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:45.612630 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-26 18:46:45.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-26 18:46:45.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 18:46:45.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-26 18:46:45.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-26 18:46:45.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-26 18:46:45.000000 datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 18:46:45.616631 datasette-metadata-editable-0.0.1a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 18:46:45.612630 datasette-metadata-editable-0.0.1a7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-10-26 18:46:21.000000 datasette-metadata-editable-0.0.1a7/tests/test_metadata_editable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 19:39:15.194440 datasette-metadata-editable-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-26 19:39:15.194440 datasette-metadata-editable-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 19:39:15.186440 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/internal_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 19:39:15.190440 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/static/plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 19:39:15.190440 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/templates/edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 19:39:15.190440 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-26 19:39:15.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-26 19:39:15.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 19:39:15.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-26 19:39:15.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-26 19:39:15.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-26 19:39:15.000000 datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 19:39:15.194440 datasette-metadata-editable-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 19:39:15.190440 datasette-metadata-editable-0.0.1a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-10-26 19:38:54.000000 datasette-metadata-editable-0.0.1a9/tests/test_metadata_editable.py
```

### Comparing `datasette-metadata-editable-0.0.1a7/LICENSE` & `datasette-metadata-editable-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-metadata-editable-0.0.1a7/PKG-INFO` & `datasette-metadata-editable-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-metadata-editable
-Version: 0.0.1a7
+Version: 0.0.1a9
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-metadata-editable
 Project-URL: Changelog, https://github.com/datasette/datasette-metadata-editable/releases
 Project-URL: Issues, https://github.com/datasette/datasette-metadata-editable/issues
 Project-URL: CI, https://github.com/datasette/datasette-metadata-editable/actions
 Classifier: Framework :: Datasette
```

### Comparing `datasette-metadata-editable-0.0.1a7/README.md` & `datasette-metadata-editable-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/__init__.py` & `datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,41 @@
 import json
 import sqlite3
 
 import markdown2
 import nh3
-from datasette import Response, hookimpl
+from datasette import Response, hookimpl, Permission, Forbidden
 from sqlite_utils import Database
 from typing import Optional
 
 from .internal_migrations import internal_migrations
+from functools import wraps
+
+PERMISSION_EDIT_METADATA = "datasette-metadata-editable-edit"
 
 cache = {}
 
 
+# decorator for routes, to ensure the proper permissions are checked
+def check_permission():
+    def decorator(func):
+        @wraps(func)
+        async def wrapper(scope, receive, datasette, request):
+            result = await datasette.permission_allowed(
+                request.actor, PERMISSION_EDIT_METADATA, default=False
+            )
+            if not result:
+                raise Forbidden("Permission denied for datasette-comments")
+            return await func(scope, receive, datasette, request)
+
+        return wrapper
+
+    return decorator
+
+
 def md_to_html(md: str):
     raw_html = markdown2.markdown(md)
     return nh3.clean(raw_html)
 
 
 async def insert_index_entry(db, cache, key, value):
     return await insert_entry(db, cache, "index", None, None, None, key, value)
@@ -80,14 +100,15 @@
             "key": key,
             "value": value,
         },
     )
 
 
 class Routes:
+    @check_permission()
     async def edit_page(scope, receive, datasette, request):
         db = request.args.get("db")
         table = request.args.get("table")
         column = request.args.get("column")
 
         if db and not table:
             target_type = "database"
@@ -121,14 +142,15 @@
                     "table": table,
                     "column": column,
                 },
                 request=request,
             )
         )
 
+    @check_permission()
     async def api_edit(scope, receive, datasette, request):
         assert request.method == "POST"
         data = await request.post_vars()
         internal_db = datasette.get_internal_database()
 
         target_type = data.get("target_type")
         if target_type == "index":
@@ -190,14 +212,28 @@
                 f"Exception while sourcing from datasette_metadata_editable_entries at startup: {e}"
             )
 
     return inner
 
 
 @hookimpl
+def register_permissions(datasette):
+    return [
+        Permission(
+            name=PERMISSION_EDIT_METADATA,
+            abbr=None,
+            description="Ability to edit metadata",
+            takes_database=False,
+            takes_resource=False,
+            default=False,
+        ),
+    ]
+
+
+@hookimpl
 def get_metadata(datasette, key, database, table):
     return cache
 
 
 @hookimpl
 def register_routes():
     return [
@@ -206,20 +242,20 @@
     ]
 
 
 @hookimpl
 async def extra_body_script(
     template, database, table, columns, view_name, request, datasette
 ):
-    if view_name in ("index", "database", "table"):
+    if not request or not await datasette.permission_allowed(
+        request.actor, PERMISSION_EDIT_METADATA, default=False
+    ):
+        return ""
+    if view_name == "index":
         url = "/-/datasette-metadata-editable/edit?"
-        if view_name in ["database", "table"]:
-            url += f"&db={database}"
-        if view_name in ["table"]:
-            url += f"&table={table}"
         return f"""
           const editMetadata = document.createElement("a")
           editMetadata.textContent = "Edit metadata"
           editMetadata.setAttribute('href', {json.dumps(url)})
 
           const metadataElement = document.querySelector('.metadata-description');
           if(metadataElement)
@@ -234,7 +270,45 @@
 def extra_js_urls(template, database, table, columns, view_name, request, datasette):
     if view_name in {"table", "query", "database"}:
         return [
             datasette.urls.path(
                 "/-/static-plugins/datasette-metadata-editable/plugin.js"
             )
         ]
+
+
+@hookimpl
+def database_actions(datasette, actor, database):
+    async def inner():
+        if not await datasette.permission_allowed(
+            actor, PERMISSION_EDIT_METADATA, default=False
+        ):
+            return []
+        return [
+            {
+                "href": datasette.urls.path(
+                    f"/-/datasette-metadata-editable/edit?db={database}"
+                ),
+                "label": "Edit database metadata",
+            }
+        ]
+
+    return inner
+
+
+@hookimpl
+def table_actions(datasette, actor, database, table):
+    async def inner():
+        if not await datasette.permission_allowed(
+            actor, PERMISSION_EDIT_METADATA, default=False
+        ):
+            return []
+        return [
+            {
+                "href": datasette.urls.path(
+                    f"/-/datasette-metadata-editable/edit?db={database}&table={table}"
+                ),
+                "label": "Edit table metadata",
+            }
+        ]
+
+    return inner
```

### Comparing `datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/schema.sql` & `datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/schema.sql`

 * *Files identical despite different names*

### Comparing `datasette-metadata-editable-0.0.1a7/datasette_metadata_editable/templates/edit.html` & `datasette-metadata-editable-0.0.1a9/datasette_metadata_editable/templates/edit.html`

 * *Files identical despite different names*

### Comparing `datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/PKG-INFO` & `datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-metadata-editable
-Version: 0.0.1a7
+Version: 0.0.1a9
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-metadata-editable
 Project-URL: Changelog, https://github.com/datasette/datasette-metadata-editable/releases
 Project-URL: Issues, https://github.com/datasette/datasette-metadata-editable/issues
 Project-URL: CI, https://github.com/datasette/datasette-metadata-editable/actions
 Classifier: Framework :: Datasette
```

### Comparing `datasette-metadata-editable-0.0.1a7/datasette_metadata_editable.egg-info/SOURCES.txt` & `datasette-metadata-editable-0.0.1a9/datasette_metadata_editable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-metadata-editable-0.0.1a7/pyproject.toml` & `datasette-metadata-editable-0.0.1a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-metadata-editable"
-version = "0.0.1a7"
+version = "0.0.1a9"
 description = ""
 readme = "README.md"
 authors = [{name = "Alex Garcia"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette-metadata-editable-0.0.1a7/tests/test_metadata_editable.py` & `datasette-metadata-editable-0.0.1a9/tests/test_metadata_editable.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,32 @@
     assert response.status_code == 200
     installed_plugins = {p["name"] for p in response.json()}
     assert "datasette-metadata-editable" in installed_plugins
 
 
 @pytest.mark.asyncio
 async def test_basic(snapshot):
-    datasette = Datasette(memory=True)
+    datasette = Datasette(
+        memory=True,
+        metadata={
+            "permissions": {"datasette-metadata-editable-edit": {"id": ["root"]}}
+        },
+    )
     assert datasette.metadata("title") is None
 
     cookies = {"ds_actor": datasette.sign({"a": {"id": "root"}}, "actor")}
     response = await datasette.client.get(
         "/-/datasette-metadata-editable/edit", cookies=cookies
     )
     csrftoken = response.cookies["ds_csrftoken"]
     cookies["ds_csrftoken"] = csrftoken
 
     await datasette.client.post(
         "/-/datasette-metadata-editable/api/edit",
+        cookies=cookies,
         data={"csrftoken": csrftoken, "target_type": "index", "title": "yo"},
     )
 
     async def all_entries():
         return [
             dict(row)
             for row in (
@@ -39,11 +45,12 @@
         ]
 
     assert datasette.metadata("title") == "yo"
     assert await all_entries() == snapshot(name="entry rows initial")
 
     await datasette.client.post(
         "/-/datasette-metadata-editable/api/edit",
+        cookies=cookies,
         data={"csrftoken": csrftoken, "target_type": "index", "title": "yo2"},
     )
     assert datasette.metadata("title") == "yo2"
     assert await all_entries() == snapshot(name="entry rows updated")
```

