# Comparing `tmp/pelican-nginx-alias-map-1.0.1.tar.gz` & `tmp/pelican_nginx_alias_map-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-nginx-alias-map-1.0.1.tar", max compression
+gzip compressed data, was "pelican_nginx_alias_map-2.0.0.tar", max compression
```

## Comparing `pelican-nginx-alias-map-1.0.1.tar` & `pelican_nginx_alias_map-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1150 2021-08-28 22:25:11.059101 pelican-nginx-alias-map-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3709 2021-08-29 10:35:36.422192 pelican-nginx-alias-map-1.0.1/README.md
--rw-r--r--   0        0        0       39 2021-08-29 10:35:23.306835 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/__init__.py
--rw-r--r--   0        0        0     3101 2021-08-29 10:35:23.307274 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/nginx_alias_map.py
--rw-r--r--   0        0        0      245 2021-08-29 10:35:23.307686 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/test_data/alias_map.expected
--rw-r--r--   0        0        0      119 2021-08-29 10:35:23.308064 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/test_data/test_no_alias.md
--rw-r--r--   0        0        0      143 2021-08-29 10:35:23.308384 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/test_data/test_one_alias.md
--rw-r--r--   0        0        0      156 2021-08-29 10:35:23.308765 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/test_data/test_two_alias.md
--rw-r--r--   0        0        0     1206 2021-12-04 11:51:54.051524 pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/test_nginx_alias_map.py
--rw-r--r--   0        0        0     2014 2021-12-04 12:05:45.677814 pelican-nginx-alias-map-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4799 2021-12-04 12:42:20.232215 pelican-nginx-alias-map-1.0.1/setup.py
--rw-r--r--   0        0        0     5166 2021-12-04 12:42:20.232485 pelican-nginx-alias-map-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1150 2021-08-28 22:25:11.059101 pelican_nginx_alias_map-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3709 2021-08-29 10:35:36.422192 pelican_nginx_alias_map-2.0.0/README.md
+-rw-r--r--   0        0        0       39 2021-08-29 10:35:23.306835 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/__init__.py
+-rw-r--r--   0        0        0     3105 2024-04-09 18:45:23.680399 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/nginx_alias_map.py
+-rw-r--r--   0        0        0      245 2021-08-29 10:35:23.307686 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/test_data/alias_map.expected
+-rw-r--r--   0        0        0      119 2021-08-29 10:35:23.308064 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/test_data/test_no_alias.md
+-rw-r--r--   0        0        0      143 2021-08-29 10:35:23.308384 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/test_data/test_one_alias.md
+-rw-r--r--   0        0        0      156 2021-08-29 10:35:23.308765 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/test_data/test_two_alias.md
+-rw-r--r--   0        0        0     1206 2021-12-04 11:51:54.051524 pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/test_nginx_alias_map.py
+-rw-r--r--   0        0        0     2081 2024-04-09 18:48:46.179648 pelican_nginx_alias_map-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5217 1970-01-01 00:00:00.000000 pelican_nginx_alias_map-2.0.0/PKG-INFO
```

### Comparing `pelican-nginx-alias-map-1.0.1/LICENSE.txt` & `pelican_nginx_alias_map-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pelican-nginx-alias-map-1.0.1/README.md` & `pelican_nginx_alias_map-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/nginx_alias_map.py` & `pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/nginx_alias_map.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             + self.context.get("hidden_pages", [])
         )
 
         query_aliases = []
         noquery_aliases = []
         for page in pages:
             aliases = page.metadata.get("alias", [])
-            if type(aliases) != list:
+            if not isinstance(aliases, list):
                 aliases = aliases.split(self.alias_delimiter)
             for alias in aliases:
                 alias = alias.strip()
                 if "?" in alias:
                     query_aliases += [(page, alias)]
                     logger.info("[alias] Saving query alias %s" % alias)
                 else:
@@ -58,24 +58,24 @@
             if len(noquery_aliases) > 0:
                 if len(query_aliases) > 0:
                     default_variable = self.alias_map_temp
                     fd.write("map $uri $%s {\n" % default_variable)
                 else:
                     fd.write("map $uri $%s {\n" % self.alias_map)
 
-                for (page, alias) in noquery_aliases:
+                for page, alias in noquery_aliases:
                     logger.info("[alias] Processing quoted alias %s" % alias)
                     self.create_alias(page, alias, fd)
                 fd.write("  }\n")
 
             if len(query_aliases) > 0:
                 fd.write("\nmap $request_uri $%s {\n" % self.alias_map)
                 if default_variable:
                     fd.write("\tdefault $%s;\n" % default_variable)
-                for (page, alias) in query_aliases:
+                for page, alias in query_aliases:
                     logger.info("[alias] Processing quoted alias %s" % alias)
                     self.create_alias(page, alias, fd)
                 fd.write("  }\n")
 
 
 def get_generators(generators):
     return NginxAliasMapGenerator
```

### Comparing `pelican-nginx-alias-map-1.0.1/pelican/plugins/nginx_alias_map/test_nginx_alias_map.py` & `pelican_nginx_alias_map-2.0.0/pelican/plugins/nginx_alias_map/test_nginx_alias_map.py`

 * *Files identical despite different names*

### Comparing `pelican-nginx-alias-map-1.0.1/pyproject.toml` & `pelican_nginx_alias_map-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-nginx-alias-map"
-version = "1.0.1"
+version = "2.0.0"
 description = "This Pelican plugin creates an nginx-compatible map between the final page locations and prior locations, defined in the `Alias` attribute for any article or page."
 authors = ["Gaige B. Paulsen <gaige@cluetrust.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pelican", "plugin"]
 repository = "https://github.com/gaige/nginx_alias_map"
 documentation = "https://docs.getpelican.com"
@@ -23,41 +23,45 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/gaige/nginx_alias_map/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.8,<4.0"
 pelican = ">=4.5"
 markdown = {version = ">=3.2, != 3.3.5", optional = true}
 
 [tool.poetry.dev-dependencies]
-black = {version = "^21.5b0", allow-prereleases = true}
+black = {version = "^24.3"}
 flake8 = "^4.0"
-flake8-black = "^0.2"
-invoke = "^1.3"
+flake8-black = "^0.3"
+invoke = "^2.2"
 isort = "^5.4"
 livereload = "^2.6"
 markdown = "^3.2, != 3.3.5"
-pytest = "^6.0"
+pytest = "^7.3.2"
 pytest-cov = "^3.0"
 pytest-pythonpath = "^0.7"
-pytest-sugar = "^0.9"
-Werkzeug = "^2.0"
+pytest-sugar = "^1.0"
+Werkzeug = "^3.0"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
 
 [tool.autopub]
 project-name = "nginx_alias_map"
 git-username = "botpub"
 git-email = "botpub@autopub.rocks"
 append-github-contributor = true
 
+[tool.commitizen]
+version_provider = "poetry"
+tag_format = "v$major.$minor.$patch$prerelease"
+
 [tool.isort]
 # Maintain compatibility with Black
 profile = "black"
 multi_line_output = 3
 
 # Sort imports within their section independent of the import type
 force_sort_within_sections = true
```

### Comparing `pelican-nginx-alias-map-1.0.1/setup.py` & `pelican_nginx_alias_map-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,128 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-nginx-alias-map
+Version: 2.0.0
+Summary: This Pelican plugin creates an nginx-compatible map between the final page locations and prior locations, defined in the `Alias` attribute for any article or page.
+Home-page: https://github.com/gaige/nginx_alias_map
+License: MIT
+Keywords: pelican,plugin
+Author: Gaige B. Paulsen
+Author-email: gaige@cluetrust.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Plugins
+Classifier: Framework :: Pelican
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: markdown
+Requires-Dist: markdown (>=3.2,!=3.3.5) ; extra == "markdown"
+Requires-Dist: pelican (>=4.5)
+Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Issue Tracker, https://github.com/gaige/nginx_alias_map/issues
+Project-URL: Repository, https://github.com/gaige/nginx_alias_map
+Description-Content-Type: text/markdown
+
+nginx_alias_map: A Plugin for Pelican
+====================================================
+
+[![Build Status](https://img.shields.io/github/workflow/status/gaige/nginx_alias_map/build)](https://github.com/gaige/nginx_alias_map/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-nginx-alias-map)](https://pypi.org/project/pelican-nginx-alias-map/)
+![License](https://img.shields.io/pypi/l/pelican-nginx-alias-map?color=blue)
+
+
+This Pelican plugin creates an nginx-compatible map between the final page locations
+and prior locations, defined in the "Alias" attribute for any article or page.
+
+Loosely based on [pelican-alias](https://github.com/Nitron/pelican-alias) by Chris Williams,
+which itself was inspired by jekyll_alias_generator.
+
+Installation
+------------
+
+This plugin can be installed via:
+
+    python -m pip install pelican-nginx-alias-map
+
+Usage
+-----
+
+Add the directory to the base plugins directory to `PLUGIN_PATHS` in
+`pelicanconf.py`, and then add `nginx_alias_map` to the `PLUGINS` list. For example,
+
+    PLUGIN_PATHS = ["plugins"]
+    PLUGINS = ['nginx_alias_map']
+
+Definable parameters (with defaults in brackets) allow some configuration of the output
+of the plugin.
+
+There are two definable parameters, one from Chris's code (`ALIAS_DELIMITER`), which
+defines the delimiter for multiple aliases for the same item; and `ALIAS_FILE`, which
+defines the final name of the output file containing the map; and
+
+    ALIAS_DELIMITER : Delimeter between multiple aliases for the same item [","]
+    ALIAS_FILE : Name of map file to be placed in `output` ['alias_map.txt']
+    ALIAS_MAP : Name of the map used in the alias file ['redirect_uri']
+    ALIAS_MAP_TEMP: Name of the map used in the alias file when 2-stage lookup is needed ['redirect_uri_1']
+
+### Support for URLs with query strings
+
+In the event that you need to redirect a URI that contains a query string, a separate
+map block will be created to map the `$request_uri` against an re.escaped version of your
+alias that contains the `?` character. Otherwise, when no query string is present, the
+test is made against `$uri`, which has much more processing done with it (query string
+removal, removal of unnecessary '/'s, and so forth).
+
+### NGINX configuration
+
+The resulting file (stored in `output/$(ALIAS_FILE)`) is ready to be included into
+your nginx configuration file (in an http stanza). Once the map is created, use the
+`ALIAS_MAP` variable in your processing.
+
+    include /opt/web/output/alias_map.txt;
+
+    server {
+      listen       *:80 ssl;
+      server_name  example.server;
+
+
+        # Redirection logic
+        if ( $redirect_uri ) {
+            return 301 $redirect_uri;
+        }
+
+        location / {
+            alias /opt/web/output;
+        }
+    }
+
+This configuration uses the evil `if` statement, but it's concise.  If you have a better
+approach, please create a pull request, and I'll add it to this doc (or replace it if it
+makes more sense).
+
+I've chosen to use a 301 redirect here, because I'm confident of the permanency.  During
+testing, you may want to use a 302.
+
+Contributing
+------------
+
+Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
+
+To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
-packages = \
-['pelican', 'pelican.plugins.nginx_alias_map']
+[existing issues]: https://github.com/gaige/nginx_alias_map/issues
+[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
-package_data = \
-{'': ['*'], 'pelican.plugins.nginx_alias_map': ['test_data/*']}
+License
+-------
 
-install_requires = \
-['pelican>=4.5']
-
-extras_require = \
-{'markdown': ['markdown>=3.2,!=3.3.5']}
-
-setup_kwargs = {
-    'name': 'pelican-nginx-alias-map',
-    'version': '1.0.1',
-    'description': 'This Pelican plugin creates an nginx-compatible map between the final page locations and prior locations, defined in the `Alias` attribute for any article or page.',
-    'long_description': 'nginx_alias_map: A Plugin for Pelican\n====================================================\n\n[![Build Status](https://img.shields.io/github/workflow/status/gaige/nginx_alias_map/build)](https://github.com/gaige/nginx_alias_map/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/pelican-nginx-alias-map)](https://pypi.org/project/pelican-nginx-alias-map/)\n![License](https://img.shields.io/pypi/l/pelican-nginx-alias-map?color=blue)\n\n\nThis Pelican plugin creates an nginx-compatible map between the final page locations\nand prior locations, defined in the "Alias" attribute for any article or page.\n\nLoosely based on [pelican-alias](https://github.com/Nitron/pelican-alias) by Chris Williams,\nwhich itself was inspired by jekyll_alias_generator.\n\nInstallation\n------------\n\nThis plugin can be installed via:\n\n    python -m pip install pelican-nginx-alias-map\n\nUsage\n-----\n\nAdd the directory to the base plugins directory to `PLUGIN_PATHS` in\n`pelicanconf.py`, and then add `nginx_alias_map` to the `PLUGINS` list. For example,\n\n    PLUGIN_PATHS = ["plugins"]\n    PLUGINS = [\'nginx_alias_map\']\n\nDefinable parameters (with defaults in brackets) allow some configuration of the output\nof the plugin.\n\nThere are two definable parameters, one from Chris\'s code (`ALIAS_DELIMITER`), which\ndefines the delimiter for multiple aliases for the same item; and `ALIAS_FILE`, which\ndefines the final name of the output file containing the map; and\n\n    ALIAS_DELIMITER : Delimeter between multiple aliases for the same item [","]\n    ALIAS_FILE : Name of map file to be placed in `output` [\'alias_map.txt\']\n    ALIAS_MAP : Name of the map used in the alias file [\'redirect_uri\']\n    ALIAS_MAP_TEMP: Name of the map used in the alias file when 2-stage lookup is needed [\'redirect_uri_1\']\n\n### Support for URLs with query strings\n\nIn the event that you need to redirect a URI that contains a query string, a separate\nmap block will be created to map the `$request_uri` against an re.escaped version of your\nalias that contains the `?` character. Otherwise, when no query string is present, the\ntest is made against `$uri`, which has much more processing done with it (query string\nremoval, removal of unnecessary \'/\'s, and so forth).\n\n### NGINX configuration\n\nThe resulting file (stored in `output/$(ALIAS_FILE)`) is ready to be included into\nyour nginx configuration file (in an http stanza). Once the map is created, use the\n`ALIAS_MAP` variable in your processing.\n\n    include /opt/web/output/alias_map.txt;\n\n    server {\n      listen       *:80 ssl;\n      server_name  example.server;\n\n\n        # Redirection logic\n        if ( $redirect_uri ) {\n            return 301 $redirect_uri;\n        }\n\n        location / {\n            alias /opt/web/output;\n        }\n    }\n\nThis configuration uses the evil `if` statement, but it\'s concise.  If you have a better\napproach, please create a pull request, and I\'ll add it to this doc (or replace it if it\nmakes more sense).\n\nI\'ve chosen to use a 301 redirect here, because I\'m confident of the permanency.  During\ntesting, you may want to use a 302.\n\nContributing\n------------\n\nContributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[existing issues]: https://github.com/gaige/nginx_alias_map/issues\n[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html\n\nLicense\n-------\n\nThis project is licensed under the MIT license.\n',
-    'author': 'Gaige B. Paulsen',
-    'author_email': 'gaige@cluetrust.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gaige/nginx_alias_map',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.2,<4.0',
-}
+This project is licensed under the MIT license.
 
-
-setup(**setup_kwargs)
```

