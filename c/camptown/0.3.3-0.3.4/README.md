# Comparing `tmp/camptown-0.3.3.tar.gz` & `tmp/camptown-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camptown-0.3.3.tar", max compression
+gzip compressed data, was "camptown-0.3.4.tar", max compression
```

## Comparing `camptown-0.3.3.tar` & `camptown-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-10-29 02:26:23.894789 camptown-0.3.3/LICENSE
--rw-r--r--   0        0        0      411 2023-10-30 21:51:00.824614 camptown-0.3.3/README.md
--rw-r--r--   0        0        0     7152 2023-11-04 03:18:18.136875 camptown-0.3.3/camptown/__init__.py
--rw-r--r--   0        0        0     2015 2023-10-31 23:28:41.076267 camptown-0.3.3/camptown/__main__.py
--rw-r--r--   0        0        0       57 2024-03-06 08:53:08.107583 camptown-0.3.3/camptown/__version__.py
--rw-r--r--   0        0        0     4567 2024-03-06 08:48:11.943562 camptown-0.3.3/camptown/templates/index.html
--rw-r--r--   0        0        0     7490 2023-11-03 05:40:15.255213 camptown-0.3.3/camptown/templates/player.css
--rw-r--r--   0        0        0     5793 2023-10-31 22:45:25.531318 camptown-0.3.3/camptown/templates/player.js
--rw-r--r--   0        0        0      652 2024-03-06 08:52:36.283639 camptown-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 camptown-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-10-29 02:26:23.894789 camptown-0.3.4/LICENSE
+-rw-r--r--   0        0        0      411 2023-10-30 21:51:00.824614 camptown-0.3.4/README.md
+-rw-r--r--   0        0        0     7307 2024-04-09 19:10:07.219908 camptown-0.3.4/camptown/__init__.py
+-rw-r--r--   0        0        0     2015 2023-10-31 23:28:41.076267 camptown-0.3.4/camptown/__main__.py
+-rw-r--r--   0        0        0       57 2024-04-09 19:14:07.495710 camptown-0.3.4/camptown/__version__.py
+-rw-r--r--   0        0        0     4567 2024-03-06 08:48:11.943562 camptown-0.3.4/camptown/templates/index.html
+-rw-r--r--   0        0        0     7708 2024-04-09 19:05:33.563695 camptown-0.3.4/camptown/templates/player.css
+-rw-r--r--   0        0        0     5793 2023-10-31 22:45:25.531318 camptown-0.3.4/camptown/templates/player.js
+-rw-r--r--   0        0        0      652 2024-04-09 19:12:24.126150 camptown-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 camptown-0.3.4/PKG-INFO
```

### Comparing `camptown-0.3.3/LICENSE` & `camptown-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `camptown-0.3.3/camptown/__init__.py` & `camptown-0.3.4/camptown/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,21 +195,24 @@
         loader=jinja2.FileSystemLoader(os.path.join(os.path.dirname(__file__), 'templates')))
     env.filters['markdown'] = markdown(output_dir, file_callback, outfiles)
     env.filters['lyrics'] = lyrics
     env.filters['artwork_img'] = artwork_img
     env.filters['timestamp'] = seconds_timestamp
     env.filters['datetime'] = seconds_datetime
 
-    urls = [(CAMPTOWN_URL, 'Camptown')]
-    if footer_urls:
-        urls += footer_urls
+    if 'theme' in album and 'footer_text' in album['theme']:
+        footer_text = Markup(album['theme']['footer_text'])
+    else:
+        urls = [(CAMPTOWN_URL, 'Camptown')]
+        if footer_urls:
+            urls += footer_urls
 
-    footer_text = Markup("Made with " + ' + '.join([
-        f'<a href="{url}" target="_blank" rel="noopener">{text}</a>'
-        for url, text in urls]))
+        footer_text = Markup("Made with " + ' + '.join([
+            f'<a href="{url}" target="_blank" rel="noopener">{text}</a>'
+            for url, text in urls]))
 
     for tmpl in ('index.html', 'player.js', 'player.css'):
         LOGGER.info("Writing %s", tmpl)
         template = env.get_template(tmpl)
         with open(os.path.join(output_dir, tmpl), 'w', encoding='utf8') as outfile:
             outfile.write(template.render(album=album,
                                           theme=album.get('theme', {}),
```

### Comparing `camptown-0.3.3/camptown/__main__.py` & `camptown-0.3.4/camptown/__main__.py`

 * *Files identical despite different names*

### Comparing `camptown-0.3.3/camptown/templates/index.html` & `camptown-0.3.4/camptown/templates/index.html`

 * *Files identical despite different names*

### Comparing `camptown-0.3.3/camptown/templates/player.css` & `camptown-0.3.4/camptown/templates/player.css`

 * *Files 2% similar despite different names*

```diff
@@ -125,34 +125,45 @@
 }
 
 .player {
     display: flex;
     align-items: center;
     column-gap: 1ex;
     padding-right: 1ex;
+    height: 36px;
 }
 
 .player button {
-    width: 3em;
-    height: 3em;
+    height: 100%;
+    aspect-ratio: 1 / 1;
     border: solid var(--foreground) 1px;
     border-radius: 4px;
     background-color: white;
     color: black;
     background-position: center center;
     background-size: 90%;
     background-repeat: no-repeat;
+    box-sizing: border-box;
 }
 .player button:hover {
     border: solid var(--highlight) 1px;
     background-color: color-mix(in srgb, var(--highlight) 10%, white);
 }
 
 audio {
     flex-grow: 1;
+    height: 100%;
+    vertical-align: middle;
+    margin: 0;
+    padding: 0;
+}
+
+audio::-webkit-media-controls-enclosure {
+    border-radius: 0;
+    height: 100%;
 }
 
 .track img {
     display: none;
 }
 
 input[type="checkbox"] { display: none; }
```

### Comparing `camptown-0.3.3/camptown/templates/player.js` & `camptown-0.3.4/camptown/templates/player.js`

 * *Files identical despite different names*

### Comparing `camptown-0.3.3/pyproject.toml` & `camptown-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "camptown"
-version = "0.3.3"
+version = "0.3.4"
 description = "Semantic-HTML player engine"
 authors = ["fluffy <fluffy@beesbuzz.biz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fluffy-critter/camptown"
 documentation = "https://camptown.readthedocs.io"
 include = [
     "camptown/__version__.py"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Jinja2 = "^3.1.2"
+Jinja2 = "^3.1.3"
 mistune = "^3.0.2"
 markupsafe = "^2.1.3"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.1"
 pylint = "^3.0.2"
 autopep8 = "^2.0.4"
```

### Comparing `camptown-0.3.3/PKG-INFO` & `camptown-0.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: camptown
-Version: 0.3.3
+Version: 0.3.4
 Summary: Semantic-HTML player engine
 Home-page: https://github.com/fluffy-critter/camptown
 License: MIT
 Author: fluffy
 Author-email: fluffy@beesbuzz.biz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: mistune (>=3.0.2,<4.0.0)
 Project-URL: Documentation, https://camptown.readthedocs.io
 Project-URL: Repository, https://github.com/fluffy-critter/camptown
 Description-Content-Type: text/markdown
 
 # Camptown
```

