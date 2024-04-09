# Comparing `tmp/weblate_schemas-2023.3.tar.gz` & `tmp/weblate_schemas-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblate_schemas-2023.3.tar", last modified: Thu Jun  8 18:02:14 2023, max compression
+gzip compressed data, was "weblate_schemas-2024.1.tar", last modified: Tue Apr  9 13:40:22 2024, max compression
```

## Comparing `weblate_schemas-2023.3.tar` & `weblate_schemas-2024.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-06-08 18:02:14.158708 weblate_schemas-2023.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      302 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.150708 weblate_schemas-2023.3/weblate_schemas/
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/weblate_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-backup.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)    21715 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-component.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-memory.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)     8600 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-userdata.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/test_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/weblate_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-08 18:02:14.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:40:22.503835 weblate_schemas-2024.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-09 13:40:22.503835 weblate_schemas-2024.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 13:40:22.503835 weblate_schemas-2024.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:40:22.503835 weblate_schemas-2024.1/weblate_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:40:22.503835 weblate_schemas-2024.1/weblate_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/schemas/weblate-backup.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21715 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/schemas/weblate-component.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/schemas/weblate-memory.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/schemas/weblate-userdata.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-04-09 13:40:12.000000 weblate_schemas-2024.1/weblate_schemas/test_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:40:22.503835 weblate_schemas-2024.1/weblate_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-09 13:40:22.000000 weblate_schemas-2024.1/weblate_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 13:40:22.000000 weblate_schemas-2024.1/weblate_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:40:22.000000 weblate_schemas-2024.1/weblate_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:40:22.000000 weblate_schemas-2024.1/weblate_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 13:40:22.000000 weblate_schemas-2024.1/weblate_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 13:40:22.000000 weblate_schemas-2024.1/weblate_schemas.egg-info/top_level.txt
```

### Comparing `weblate_schemas-2023.3/CHANGES.rst` & `weblate_schemas-2024.1/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+2024.1
+------
+
+* Released on 9th April 2024.
+* Dropped support for Python 3.7 and 3.8.
+* Added support for Python 3.12.
+* Clarified address field on user data.
+
 2023.3
 ------
 
 * Released on 8th June 2023.
 * Added theme to user data.
 
 2023.2
```

### Comparing `weblate_schemas-2023.3/LICENSE` & `weblate_schemas-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.3/README.rst` & `weblate_schemas-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.3/pyproject.toml` & `weblate_schemas-2024.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.black]
-target-version = ['py37']
+target-version = ['py39']
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
-format = "github"
 ignore = [
   "D203",  # CONFIG: incompatible with D211
   "D212"  # CONFIG: incompatible with D213
 ]
+output-format = "github"
 select = [
   "E",
   "F",
   "B",
   "T10",
   "A",
   "C4",
@@ -40,11 +40,11 @@
   "TID",
   "RSE",
   "T20",
   "RET",
   "SLF",
   "N"
 ]
-target-version = "py37"
+target-version = "py39"
 
 [tool.ruff.mccabe]
 max-complexity = 16
```

### Comparing `weblate_schemas-2023.3/setup.cfg` & `weblate_schemas-2024.1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weblate_schemas
-version = 2023.3
+version = 2024.1
 description = A collection of JSON schemas used by Weblate
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@cihar.com
 license = MIT
@@ -14,34 +14,29 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Internationalization
 	Topic :: Software Development :: Localization
 	Topic :: Utilities
 download_url = https://github.com/WeblateOrg/weblate_schemas
 keywords = i18n l10n gettext translate weblate
 project_urls = 
 	Issue Tracker=https://github.com/WeblateOrg/weblate_schemas/issues
 	Documentation=https://docs.weblate.org/
 	Source Code=https://github.com/WeblateOrg/weblate_schemas
 	Twitter=https://twitter.com/WeblateOrg
 	Funding=https://weblate.org/donate/
 
 [options]
 packages = find_namespace:
-python_requires = >=3.7
+python_requires = >=3.9
 include_package_data = 1
 zip_safe = 0
 
 [flake8]
 max-complexity = 16
 extend-select = E,W1,W2,W3,W504,W505,W6,B
 enable-extensions = B,C,D,DJ,F,G,I,M,N,R,SF,UPS
```

### Comparing `weblate_schemas-2023.3/weblate_schemas/__init__.py` & `weblate_schemas-2024.1/weblate_schemas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # SPDX-License-Identifier: MIT
 
 """Schemas used by Weblate."""
 
 import json
 from pathlib import Path
-from typing import Dict
 
 from jsonschema import FormatChecker, validate
 
 SCHEMA_BASE = Path(__file__).resolve().parent.joinpath("schemas")
 
 SCHEMA_CACHE = {}
 
@@ -24,11 +23,11 @@
     """Load schema from a disk."""
     if name not in SCHEMA_CACHE:
         with get_path(name).open("r") as handle:
             SCHEMA_CACHE[name] = json.load(handle)
     return SCHEMA_CACHE[name]
 
 
-def validate_schema(data: Dict, name: str):
+def validate_schema(data: dict, name: str):
     """Validate data to match schema."""
     schema = load_schema(name)
     validate(data, schema, format_checker=FormatChecker())
```

### Comparing `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-backup.schema.json` & `weblate_schemas-2024.1/weblate_schemas/schemas/weblate-backup.schema.json`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-component.schema.json` & `weblate_schemas-2024.1/weblate_schemas/schemas/weblate-component.schema.json`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-memory.schema.json` & `weblate_schemas-2024.1/weblate_schemas/schemas/weblate-memory.schema.json`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-userdata.schema.json` & `weblate_schemas-2024.1/weblate_schemas/schemas/weblate-userdata.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999911422902494%*

 * *Differences: {"'properties'": "{'auditlog': {'items': {'properties': {'address': {'anyOf': "*

 * *                 "[OrderedDict([('type', 'null')]), OrderedDict([('type', 'string'), ('default', "*

 * *                 "''), ('examples', ['127.0.0.1']), ('pattern', '^.*$')])], delete: ['type', "*

 * *                 "'default', 'examples', 'pattern']}}}}}"}*

```diff
@@ -18,21 +18,28 @@
                         ],
                         "pattern": "^.*$",
                         "title": "Activity",
                         "type": "string"
                     },
                     "address": {
                         "$id": "#root/auditlog/items/address",
-                        "default": "",
-                        "examples": [
-                            "127.0.0.1"
+                        "anyOf": [
+                            {
+                                "type": "null"
+                            },
+                            {
+                                "default": "",
+                                "examples": [
+                                    "127.0.0.1"
+                                ],
+                                "pattern": "^.*$",
+                                "type": "string"
+                            }
                         ],
-                        "pattern": "^.*$",
-                        "title": "IP address",
-                        "type": "string"
+                        "title": "IP address"
                     },
                     "timestamp": {
                         "$id": "#root/auditlog/items/timestamp",
                         "default": "",
                         "examples": [
                             "2019-11-18T18:58:30.845Z"
                         ],
```

### Comparing `weblate_schemas-2023.3/weblate_schemas/test_valid.py` & `weblate_schemas-2024.1/weblate_schemas/test_valid.py`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.3/weblate_schemas.egg-info/PKG-INFO` & `weblate_schemas-2024.1/weblate_schemas.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 Metadata-Version: 2.1
 Name: weblate-schemas
-Version: 2023.3
+Version: 2024.1
 Summary: A collection of JSON schemas used by Weblate
 Home-page: https://weblate.org/
+Download-URL: https://github.com/WeblateOrg/weblate_schemas
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: MIT
-Download-URL: https://github.com/WeblateOrg/weblate_schemas
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/weblate_schemas/issues
 Project-URL: Documentation, https://docs.weblate.org/
 Project-URL: Source Code, https://github.com/WeblateOrg/weblate_schemas
 Project-URL: Twitter, https://twitter.com/WeblateOrg
 Project-URL: Funding, https://weblate.org/donate/
-Description: .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
-           :alt: Weblate
-           :target: https://weblate.org/
-           :height: 80px
-        
-        **Weblate is libre software web-based continuous localization system,
-        used by over 2500 libre projects and companies in more than 165 countries.**
-        
-        This module contains schemas used in Weblate exports.
-        
-        .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
-            :alt: Website
-            :target: https://weblate.org/
-        
-        .. image:: https://hosted.weblate.org/widgets/weblate/-/svg-badge.svg
-            :alt: Translation status
-            :target: https://hosted.weblate.org/engage/weblate/?utm_source=widget
-        
-        .. image:: https://bestpractices.coreinfrastructure.org/projects/552/badge
-            :alt: CII Best Practices
-            :target: https://bestpractices.coreinfrastructure.org/projects/552
-        
-        .. image:: https://img.shields.io/pypi/v/weblate_schemas.svg
-            :target: https://pypi.org/project/weblate_schemas/
-            :alt: PyPI package
-        
-        .. image:: https://img.shields.io/readthedocs/weblate.svg
-            :alt: Documentation
-            :target: https://docs.weblate.org/en/latest/schemas.html
-        
-        Installation
-        ------------
-        
-        Install using pip:
-        
-        .. code-block:: sh
-        
-            pip3 install weblate_schemas
-        
-        Sources are available at <https://github.com/WeblateOrg/weblate_schemas>.
-        
-        Contributing
-        ------------
-        
-        Contributions are welcome! See `documentation <https://docs.weblate.org/en/latest/contributing/modules.html>`__ for more information.
-        
 Keywords: i18n l10n gettext translate weblate
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
+   :alt: Weblate
+   :target: https://weblate.org/
+   :height: 80px
+
+**Weblate is libre software web-based continuous localization system,
+used by over 2500 libre projects and companies in more than 165 countries.**
+
+This module contains schemas used in Weblate exports.
+
+.. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
+    :alt: Website
+    :target: https://weblate.org/
+
+.. image:: https://hosted.weblate.org/widgets/weblate/-/svg-badge.svg
+    :alt: Translation status
+    :target: https://hosted.weblate.org/engage/weblate/?utm_source=widget
+
+.. image:: https://bestpractices.coreinfrastructure.org/projects/552/badge
+    :alt: CII Best Practices
+    :target: https://bestpractices.coreinfrastructure.org/projects/552
+
+.. image:: https://img.shields.io/pypi/v/weblate_schemas.svg
+    :target: https://pypi.org/project/weblate_schemas/
+    :alt: PyPI package
+
+.. image:: https://img.shields.io/readthedocs/weblate.svg
+    :alt: Documentation
+    :target: https://docs.weblate.org/en/latest/schemas.html
+
+Installation
+------------
+
+Install using pip:
+
+.. code-block:: sh
+
+    pip3 install weblate_schemas
+
+Sources are available at <https://github.com/WeblateOrg/weblate_schemas>.
+
+Contributing
+------------
+
+Contributions are welcome! See `documentation <https://docs.weblate.org/en/latest/contributing/modules.html>`__ for more information.
```

### Comparing `weblate_schemas-2023.3/weblate_schemas.egg-info/SOURCES.txt` & `weblate_schemas-2024.1/weblate_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

