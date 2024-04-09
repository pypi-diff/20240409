# Comparing `tmp/pelican-markdown-it-reader-1.0.1.tar.gz` & `tmp/pelican_markdown_it_reader-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-markdown-it-reader-1.0.1.tar", max compression
+gzip compressed data, was "pelican_markdown_it_reader-2.0.0.tar", max compression
```

## Comparing `pelican-markdown-it-reader-1.0.1.tar` & `pelican_markdown_it_reader-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1799 2021-08-29 10:37:28.668076 pelican-markdown-it-reader-1.0.1/README.md
--rw-r--r--   0        0        0       42 2021-03-27 11:45:48.498426 pelican-markdown-it-reader-1.0.1/pelican/plugins/markdown_it_reader/__init__.py
--rw-r--r--   0        0        0     4271 2021-08-26 09:49:51.452027 pelican-markdown-it-reader-1.0.1/pelican/plugins/markdown_it_reader/markdown_it_reader.py
--rw-r--r--   0        0        0      495 2021-08-26 10:29:23.653647 pelican-markdown-it-reader-1.0.1/pelican/plugins/markdown_it_reader/test_markdown_it_reader.py
--rw-r--r--   0        0        0     1968 2021-12-04 13:10:14.863556 pelican-markdown-it-reader-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2763 2021-12-04 13:13:42.140513 pelican-markdown-it-reader-1.0.1/setup.py
--rw-r--r--   0        0        0     3331 2021-12-04 13:13:42.140770 pelican-markdown-it-reader-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1799 2024-04-09 18:56:13.009470 pelican_markdown_it_reader-2.0.0/README.md
+-rw-r--r--   0        0        0       42 2024-04-09 18:56:13.009715 pelican_markdown_it_reader-2.0.0/pelican/plugins/markdown_it_reader/__init__.py
+-rw-r--r--   0        0        0     4271 2024-04-09 18:56:13.009847 pelican_markdown_it_reader-2.0.0/pelican/plugins/markdown_it_reader/markdown_it_reader.py
+-rw-r--r--   0        0        0      495 2024-04-09 18:56:13.009940 pelican_markdown_it_reader-2.0.0/pelican/plugins/markdown_it_reader/test_markdown_it_reader.py
+-rw-r--r--   0        0        0     2046 2024-04-09 19:23:15.220119 pelican_markdown_it_reader-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 pelican_markdown_it_reader-2.0.0/PKG-INFO
```

### Comparing `pelican-markdown-it-reader-1.0.1/README.md` & `pelican_markdown_it_reader-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican-markdown-it-reader-1.0.1/pelican/plugins/markdown_it_reader/markdown_it_reader.py` & `pelican_markdown_it_reader-2.0.0/pelican/plugins/markdown_it_reader/markdown_it_reader.py`

 * *Files identical despite different names*

### Comparing `pelican-markdown-it-reader-1.0.1/pyproject.toml` & `pelican_markdown_it_reader-2.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-markdown-it-reader"
-version = "1.0.1"
+version = "2.0.0"
 description = "Reader plugin for Markdown-IT-py replacement"
 authors = ["Gaige B. Paulsen <gaige@cluetrust.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pelican", "plugin"]
 repository = "https://github.com/gaige/markdown-it-reader"
 documentation = "https://docs.getpelican.com"
@@ -23,44 +23,48 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/gaige/markdown-it-reader/issues"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-pelican = "^4.5"
+python = ">=3.8,<4.0"
+pelican = ">=4.5"
 Pygments = "^2.6"
 markdown-it-py = ">=1.1,<3.0"
 markdown = {version = "^3.2.2", optional = true}
 mdit-py-plugins = ">=0.2.8,<0.4.0"
 
 [tool.poetry.dev-dependencies]
-black = {version = "^20.8b1", allow-prereleases = true}
+black = {version = "^24.3"}
 flake8 = "^4.0"
-flake8-black = "^0.2.0"
-invoke = "^1.3"
+flake8-black = "^0.3"
+invoke = "^2.2"
 isort = "^5.4"
 livereload = "^2.6"
-markdown = "^3.2.2"
-pytest = "^6.2"
+markdown = "^3.2, != 3.3.5"
+pytest = "^7.3.2"
 pytest-cov = "^3.0"
-pytest-pythonpath = "^0.7.3"
-pytest-sugar = "^0.9.4"
-Werkzeug = "^2.0"
+pytest-pythonpath = "^0.7"
+pytest-sugar = "^1.0"
+Werkzeug = "^3.0"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
 
 [tool.autopub]
 project-name = "Markdown-IT reader"
 git-username = "gaige"
 git-email = "gaige@cluetrust.com"
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

### Comparing `pelican-markdown-it-reader-1.0.1/setup.py` & `pelican_markdown_it_reader-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-markdown-it-reader
+Version: 2.0.0
+Summary: Reader plugin for Markdown-IT-py replacement
+Home-page: https://github.com/gaige/markdown-it-reader
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
+Requires-Dist: Pygments (>=2.6,<3.0)
+Requires-Dist: markdown (>=3.2.2,<4.0.0) ; extra == "markdown"
+Requires-Dist: markdown-it-py (>=1.1,<3.0)
+Requires-Dist: mdit-py-plugins (>=0.2.8,<0.4.0)
+Requires-Dist: pelican (>=4.5)
+Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Issue Tracker, https://github.com/gaige/markdown-it-reader/issues
+Project-URL: Repository, https://github.com/gaige/markdown-it-reader
+Description-Content-Type: text/markdown
+
+Markdown-IT reader: A Plugin for Pelican
+====================================================
+
+[![Build Status](https://img.shields.io/github/workflow/status/gaige/markdown-it-reader/build)](https://github.com/gaige/markdown-it-reader/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-markdown-it-reader)](https://pypi.org/project/pelican-markdown-it-reader/)
+![License](https://img.shields.io/pypi/l/pelican-markdown-it-reader?color=blue)
+
+Reader plugin for Markdown-IT-py replacement
+
+This is double-opinionated, in that it's opinionated using Markdown-IT
+and again because we add in some additions; in particular:
+
+- Tables
+- footnotes
+- Pygment-based syntax highlighting
+
+Installation
+------------
+
+This plugin can be installed via:
+
+    python -m pip install pelican-markdown-it-reader
+
+
+Usage
+-----
+
+There are currently no configuration items.
+
+Once installed it takes over responsibility for reading the following file extensions:
+
+ - `md`
+ - `markdown`
+ - `mkd`
+ - `mdown`
+
+By taking over `link_open` and `image` render rules, the plugin handles replacing the
+pelican link placeholders with appropriate `href` items which are then rendered to html.
+
+Contributing
+------------
+
+Contributions are welcome and much appreciated. Every little bit helps.
+You can contribute by improving the documentation, adding missing features,
+and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
+
+To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
-packages = \
-['pelican', 'pelican.plugins.markdown_it_reader']
+[existing issues]: https://github.com/gaige/markdown-it-reader/issues
+[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
-package_data = \
-{'': ['*']}
+License
+-------
 
-install_requires = \
-['Pygments>=2.6,<3.0',
- 'markdown-it-py>=1.1,<3.0',
- 'mdit-py-plugins>=0.2.8,<0.4.0',
- 'pelican>=4.5,<5.0']
-
-extras_require = \
-{'markdown': ['markdown>=3.2.2,<4.0.0']}
-
-setup_kwargs = {
-    'name': 'pelican-markdown-it-reader',
-    'version': '1.0.1',
-    'description': 'Reader plugin for Markdown-IT-py replacement',
-    'long_description': "Markdown-IT reader: A Plugin for Pelican\n====================================================\n\n[![Build Status](https://img.shields.io/github/workflow/status/gaige/markdown-it-reader/build)](https://github.com/gaige/markdown-it-reader/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/pelican-markdown-it-reader)](https://pypi.org/project/pelican-markdown-it-reader/)\n![License](https://img.shields.io/pypi/l/pelican-markdown-it-reader?color=blue)\n\nReader plugin for Markdown-IT-py replacement\n\nThis is double-opinionated, in that it's opinionated using Markdown-IT\nand again because we add in some additions; in particular:\n\n- Tables\n- footnotes\n- Pygment-based syntax highlighting\n\nInstallation\n------------\n\nThis plugin can be installed via:\n\n    python -m pip install pelican-markdown-it-reader\n\n\nUsage\n-----\n\nThere are currently no configuration items.\n\nOnce installed it takes over responsibility for reading the following file extensions:\n\n - `md`\n - `markdown`\n - `mkd`\n - `mdown`\n\nBy taking over `link_open` and `image` render rules, the plugin handles replacing the\npelican link placeholders with appropriate `href` items which are then rendered to html.\n\nContributing\n------------\n\nContributions are welcome and much appreciated. Every little bit helps.\nYou can contribute by improving the documentation, adding missing features,\nand fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[existing issues]: https://github.com/gaige/markdown-it-reader/issues\n[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html\n\nLicense\n-------\n\nThis project is licensed under the MIT license.\n",
-    'author': 'Gaige B. Paulsen',
-    'author_email': 'gaige@cluetrust.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gaige/markdown-it-reader',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
-}
+This project is licensed under the MIT license.
 
-
-setup(**setup_kwargs)
```

