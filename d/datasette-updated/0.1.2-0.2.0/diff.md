# Comparing `tmp/datasette-updated-0.1.2.tar.gz` & `tmp/datasette-updated-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-updated-0.1.2.tar", last modified: Sun Dec 17 15:39:19 2023, max compression
+gzip compressed data, was "datasette-updated-0.2.0.tar", last modified: Tue Apr  9 14:38:21 2024, max compression
```

## Comparing `datasette-updated-0.1.2.tar` & `datasette-updated-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-17 15:39:07.000000 datasette-updated-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-12-17 15:39:07.000000 datasette-updated-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/datasette_updated/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-17 15:39:07.000000 datasette-updated-0.1.2/datasette_updated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/datasette_updated/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-17 15:39:07.000000 datasette-updated-0.1.2/datasette_updated/templates/_footer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/datasette_updated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-17 15:39:19.000000 datasette-updated-0.1.2/datasette_updated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-17 15:39:19.000000 datasette-updated-0.1.2/datasette_updated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 15:39:19.000000 datasette-updated-0.1.2/datasette_updated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-17 15:39:19.000000 datasette-updated-0.1.2/datasette_updated.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-17 15:39:19.000000 datasette-updated-0.1.2/datasette_updated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-17 15:39:19.000000 datasette-updated-0.1.2/datasette_updated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-17 15:39:07.000000 datasette-updated-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 15:39:19.529749 datasette-updated-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2023-12-17 15:39:07.000000 datasette-updated-0.1.2/tests/test_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:38:21.185113 datasette-updated-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 14:38:06.000000 datasette-updated-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-09 14:38:21.185113 datasette-updated-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-09 14:38:06.000000 datasette-updated-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:38:21.181113 datasette-updated-0.2.0/datasette_updated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-09 14:38:06.000000 datasette-updated-0.2.0/datasette_updated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:38:21.185113 datasette-updated-0.2.0/datasette_updated/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-09 14:38:06.000000 datasette-updated-0.2.0/datasette_updated/templates/_footer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:38:21.185113 datasette-updated-0.2.0/datasette_updated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-09 14:38:21.000000 datasette-updated-0.2.0/datasette_updated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 14:38:21.000000 datasette-updated-0.2.0/datasette_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:38:21.000000 datasette-updated-0.2.0/datasette_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 14:38:21.000000 datasette-updated-0.2.0/datasette_updated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 14:38:21.000000 datasette-updated-0.2.0/datasette_updated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 14:38:21.000000 datasette-updated-0.2.0/datasette_updated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 14:38:06.000000 datasette-updated-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:38:21.185113 datasette-updated-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:38:21.185113 datasette-updated-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-09 14:38:06.000000 datasette-updated-0.2.0/tests/test_updated.py
```

### Comparing `datasette-updated-0.1.2/LICENSE` & `datasette-updated-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-updated-0.1.2/PKG-INFO` & `datasette-updated-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-updated
-Version: 0.1.2
+Version: 0.2.0
 Summary: Display the date your data was updated
 Author-email: Ryan Caught <rcaught@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rcaught/datasette-updated
 Project-URL: Changelog, https://github.com/rcaught/datasette-updated/releases
 Project-URL: Issues, https://github.com/rcaught/datasette-updated/issues
 Project-URL: CI, https://github.com/rcaught/datasette-updated/actions
@@ -71,15 +71,15 @@
 echo '{
   "plugins": {
     "datasette-updated": {
       "updated": "'"$(date -Iseconds)"'"
     }
   }
 }' > plugins/datasette-updated/metadata.json && \
-datasette publish --plugins-dir=plugins ...
+datasette publish --plugins-dir=plugins --install=datasette-updated ...
 ```
 
 ### Combined metadata configuration
 You can combine base metadata and plugin metadata configuration, but be aware that the base `metadata.(json|yml)` will always win if there is a duplicate configuration value.
 
 ### Extra configuration
 The base / instance level metadata can accept the following extra configuration (that will apply to all levels):
@@ -117,15 +117,15 @@
 {% endif %}
 ```
 
 - **If you have your own custom footer template, you will need to add the above code**, as your base template will take precedence.
 - Look at [local_time](https://github.com/basecamp/local_time/tree/main#example) for extra configuration options (just ignore the Ruby parts).
 
 ## Screenshot and Demo
-![screenshot](screenshot.png?raw=true)
+![screenshot](https://github.com/rcaught/datasette-updated/raw/master/screenshot.png)
 - Example site: https://querydata.io/
 - The Javascript component converts time elements from UTC to the browser's local time.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
```

### Comparing `datasette-updated-0.1.2/README.md` & `datasette-updated-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 echo '{
   "plugins": {
     "datasette-updated": {
       "updated": "'"$(date -Iseconds)"'"
     }
   }
 }' > plugins/datasette-updated/metadata.json && \
-datasette publish --plugins-dir=plugins ...
+datasette publish --plugins-dir=plugins --install=datasette-updated ...
 ```
 
 ### Combined metadata configuration
 You can combine base metadata and plugin metadata configuration, but be aware that the base `metadata.(json|yml)` will always win if there is a duplicate configuration value.
 
 ### Extra configuration
 The base / instance level metadata can accept the following extra configuration (that will apply to all levels):
@@ -95,15 +95,15 @@
 {% endif %}
 ```
 
 - **If you have your own custom footer template, you will need to add the above code**, as your base template will take precedence.
 - Look at [local_time](https://github.com/basecamp/local_time/tree/main#example) for extra configuration options (just ignore the Ruby parts).
 
 ## Screenshot and Demo
-![screenshot](screenshot.png?raw=true)
+![screenshot](https://github.com/rcaught/datasette-updated/raw/master/screenshot.png)
 - Example site: https://querydata.io/
 - The Javascript component converts time elements from UTC to the browser's local time.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
```

### Comparing `datasette-updated-0.1.2/datasette_updated/__init__.py` & `datasette-updated-0.2.0/datasette_updated/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     return {"datasette_updated": always_merger.merge(base_config, specific_config)}
 
 
 @hookimpl
 def extra_js_urls():
     return [
         {
-            "url": "https://cdn.jsdelivr.net/npm/local-time@2.1.0/app/assets/javascripts/local-time.min.js",
-            "sri": "sha384-vjSE5N9a5zc42mPRxkfhAoktbmiiZ6AIEk0mEJxR3w9SWxQdzLTQx8Y+FubMepSl",
+            "url": "https://cdn.jsdelivr.net/npm/local-time@3.0.2/app/assets/javascripts/local-time.es2017-umd.js",
+            "sri": "sha384-l4PZDWQdg3uX/iY4bmkakiAYpcvOOarVJY77JwQ7edY2+c2IdUro71pKH2029xvq",
         }
     ]
 
 
 @hookimpl
 def extra_body_script():
     return {
```

### Comparing `datasette-updated-0.1.2/datasette_updated/templates/_footer.html` & `datasette-updated-0.2.0/datasette_updated/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `datasette-updated-0.1.2/datasette_updated.egg-info/PKG-INFO` & `datasette-updated-0.2.0/datasette_updated.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-updated
-Version: 0.1.2
+Version: 0.2.0
 Summary: Display the date your data was updated
 Author-email: Ryan Caught <rcaught@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rcaught/datasette-updated
 Project-URL: Changelog, https://github.com/rcaught/datasette-updated/releases
 Project-URL: Issues, https://github.com/rcaught/datasette-updated/issues
 Project-URL: CI, https://github.com/rcaught/datasette-updated/actions
@@ -71,15 +71,15 @@
 echo '{
   "plugins": {
     "datasette-updated": {
       "updated": "'"$(date -Iseconds)"'"
     }
   }
 }' > plugins/datasette-updated/metadata.json && \
-datasette publish --plugins-dir=plugins ...
+datasette publish --plugins-dir=plugins --install=datasette-updated ...
 ```
 
 ### Combined metadata configuration
 You can combine base metadata and plugin metadata configuration, but be aware that the base `metadata.(json|yml)` will always win if there is a duplicate configuration value.
 
 ### Extra configuration
 The base / instance level metadata can accept the following extra configuration (that will apply to all levels):
@@ -117,15 +117,15 @@
 {% endif %}
 ```
 
 - **If you have your own custom footer template, you will need to add the above code**, as your base template will take precedence.
 - Look at [local_time](https://github.com/basecamp/local_time/tree/main#example) for extra configuration options (just ignore the Ruby parts).
 
 ## Screenshot and Demo
-![screenshot](screenshot.png?raw=true)
+![screenshot](https://github.com/rcaught/datasette-updated/raw/master/screenshot.png)
 - Example site: https://querydata.io/
 - The Javascript component converts time elements from UTC to the browser's local time.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
```

### Comparing `datasette-updated-0.1.2/pyproject.toml` & `datasette-updated-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-updated"
-version = "0.1.2"
+version = "0.2.0"
 description = "Display the date your data was updated"
 readme = "README.md"
 authors = [{ name = "Ryan Caught", email = "rcaught@gmail.com" }]
 license = { text = "Apache-2.0" }
 classifiers = [
   "Framework :: Datasette",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `datasette-updated-0.1.2/tests/test_updated.py` & `datasette-updated-0.2.0/tests/test_updated.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     assert "datasette-updated" in installed_plugins
 
 
 @pytest.fixture
 def db_and_path(tmpdir):
     path = str(tmpdir / "data.db")
     db = sqlite_utils.Database(path)
-    db["cities"].insert_all(
+    db.table("cities").insert_all(
         [
             {
                 "id": "nyc",
                 "name": "New York City",
             },
             {
                 "id": "london",
```

