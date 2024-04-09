# Comparing `tmp/datasette-public-0.2.2.tar.gz` & `tmp/datasette-public-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-public-0.2.2.tar", last modified: Fri Dec  2 21:10:07 2022, max compression
+gzip compressed data, was "datasette-public-0.2.3.tar", last modified: Tue Apr  9 20:28:04 2024, max compression
```

## Comparing `datasette-public-0.2.2.tar` & `datasette-public-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 21:10:07.521091 datasette-public-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-02 21:09:51.000000 datasette-public-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2022-12-02 21:10:07.517091 datasette-public-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2022-12-02 21:09:51.000000 datasette-public-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 21:10:07.517091 datasette-public-0.2.2/datasette_public/
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2022-12-02 21:09:51.000000 datasette-public-0.2.2/datasette_public/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 21:10:07.517091 datasette-public-0.2.2/datasette_public/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2022-12-02 21:09:51.000000 datasette-public-0.2.2/datasette_public/templates/public_table_change_privacy.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 21:10:07.517091 datasette-public-0.2.2/datasette_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2022-12-02 21:10:07.000000 datasette-public-0.2.2/datasette_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-02 21:10:07.000000 datasette-public-0.2.2/datasette_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 21:10:07.000000 datasette-public-0.2.2/datasette_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 21:10:07.000000 datasette-public-0.2.2/datasette_public.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-02 21:10:07.000000 datasette-public-0.2.2/datasette_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-02 21:10:07.000000 datasette-public-0.2.2/datasette_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 21:10:07.521091 datasette-public-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-12-02 21:09:51.000000 datasette-public-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:04.220275 datasette-public-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 20:27:54.000000 datasette-public-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 20:28:04.220275 datasette-public-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-09 20:27:54.000000 datasette-public-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:04.220275 datasette-public-0.2.3/datasette_public/
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-09 20:27:54.000000 datasette-public-0.2.3/datasette_public/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:04.220275 datasette-public-0.2.3/datasette_public/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-09 20:27:54.000000 datasette-public-0.2.3/datasette_public/templates/public_table_change_privacy.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:04.220275 datasette-public-0.2.3/datasette_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 20:28:04.000000 datasette-public-0.2.3/datasette_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 20:28:04.000000 datasette-public-0.2.3/datasette_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:28:04.000000 datasette-public-0.2.3/datasette_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:28:04.000000 datasette-public-0.2.3/datasette_public.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 20:28:04.000000 datasette-public-0.2.3/datasette_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 20:28:04.000000 datasette-public-0.2.3/datasette_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:28:04.220275 datasette-public-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 20:27:54.000000 datasette-public-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:28:04.220275 datasette-public-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-09 20:27:54.000000 datasette-public-0.2.3/tests/test_public.py
```

### Comparing `datasette-public-0.2.2/LICENSE` & `datasette-public-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-public-0.2.2/PKG-INFO` & `datasette-public-0.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: datasette-public
-Version: 0.2.2
+Version: 0.2.3
 Summary: Make specific Datasette tables visible to the public
 Home-page: https://github.com/simonw/datasette-public
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-public/issues
 Project-URL: CI, https://github.com/simonw/datasette-public/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-public/releases
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: datasette>=0.63
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 
 # datasette-public
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-public.svg)](https://pypi.org/project/datasette-public/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-public?include_prereleases&label=changelog)](https://github.com/simonw/datasette-public/releases)
 [![Tests](https://github.com/simonw/datasette-public/workflows/Test/badge.svg)](https://github.com/simonw/datasette-public/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-public/blob/main/LICENSE)
```

### Comparing `datasette-public-0.2.2/README.md` & `datasette-public-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datasette-public-0.2.2/datasette_public/__init__.py` & `datasette-public-0.2.3/datasette_public/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,19 @@
                 {
                     "href": datasette.urls.path(
                         "/-/public-table/{}/{}".format(database, quote_plus(table))
                     ),
                     "label": "Make {} {}".format(
                         noun, "public" if is_private else "private"
                     ),
+                    "description": (
+                        "Allow anyone to view this {}".format(noun)
+                        if is_private
+                        else "Only allow logged-in users to view this {}".format(noun)
+                    ),
                 }
             ]
 
     return inner
 
 
 async def check_permissions(datasette, request, database):
```

### Comparing `datasette-public-0.2.2/datasette_public/templates/public_table_change_privacy.html` & `datasette-public-0.2.3/datasette_public/templates/public_table_change_privacy.html`

 * *Files identical despite different names*

### Comparing `datasette-public-0.2.2/datasette_public.egg-info/PKG-INFO` & `datasette-public-0.2.3/datasette_public.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: datasette-public
-Version: 0.2.2
+Version: 0.2.3
 Summary: Make specific Datasette tables visible to the public
 Home-page: https://github.com/simonw/datasette-public
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-public/issues
 Project-URL: CI, https://github.com/simonw/datasette-public/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-public/releases
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: datasette>=0.63
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
 
 # datasette-public
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-public.svg)](https://pypi.org/project/datasette-public/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/datasette-public?include_prereleases&label=changelog)](https://github.com/simonw/datasette-public/releases)
 [![Tests](https://github.com/simonw/datasette-public/workflows/Test/badge.svg)](https://github.com/simonw/datasette-public/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/datasette-public/blob/main/LICENSE)
```

### Comparing `datasette-public-0.2.2/setup.py` & `datasette-public-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

