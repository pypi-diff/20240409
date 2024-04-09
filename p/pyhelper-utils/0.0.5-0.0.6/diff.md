# Comparing `tmp/pyhelper_utils-0.0.5.tar.gz` & `tmp/pyhelper_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.5.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.6.tar", max compression
```

## Comparing `pyhelper_utils-0.0.5.tar` & `pyhelper_utils-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-08 07:26:43.178081 pyhelper_utils-0.0.5/LICENSE
--rw-r--r--   0        0        0      680 2024-04-08 07:26:43.178081 pyhelper_utils-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/general.py
--rw-r--r--   0        0        0     1455 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/notifications.py
--rw-r--r--   0        0        0     2324 2024-04-08 07:26:43.179081 pyhelper_utils-0.0.5/pyhelper_utils/shell.py
--rw-r--r--   0        0        0     1532 2024-04-08 07:26:47.255053 pyhelper_utils-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 10:49:55.702341 pyhelper_utils-0.0.6/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-08 10:49:55.702341 pyhelper_utils-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 10:49:55.703341 pyhelper_utils-0.0.6/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-08 10:49:55.703341 pyhelper_utils-0.0.6/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     1455 2024-04-08 10:49:55.703341 pyhelper_utils-0.0.6/pyhelper_utils/notifications.py
+-rw-r--r--   0        0        0     1609 2024-04-08 10:49:55.703341 pyhelper_utils-0.0.6/pyhelper_utils/runners.py
+-rw-r--r--   0        0        0     2324 2024-04-08 10:49:55.703341 pyhelper_utils-0.0.6/pyhelper_utils/shell.py
+-rw-r--r--   0        0        0     1549 2024-04-08 10:49:59.524315 pyhelper_utils-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.6/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.5/LICENSE` & `pyhelper_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.5/README.md` & `pyhelper_utils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.5/pyhelper_utils/general.py` & `pyhelper_utils-0.0.6/pyhelper_utils/general.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.5/pyhelper_utils/notifications.py` & `pyhelper_utils-0.0.6/pyhelper_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.5/pyhelper_utils/shell.py` & `pyhelper_utils-0.0.6/pyhelper_utils/shell.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.5/pyproject.toml` & `pyhelper_utils-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.coverage.run]
 omit = ["tests/*"]
 
 [tool.coverage.report]
-fail_under = 80
+fail_under = 90
 skip_empty = true
 
 [tool.coverage.html]
 directory = ".tests_coverage"
 
 [tool.ruff]
 preview = true
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.5"
+version = "0.0.6"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
@@ -37,23 +37,24 @@
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-simple-logger = "^1.0.19"
 requests = "^2.31.0"
+rich = "^13.7.1"
+ipdb = "^0.13.13"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.14.0"
 
 
 [tool.poetry.group.dev.dependencies]
-ipdb = "^0.13.13"
 ipython = "*"
 
 
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)"
```

### Comparing `pyhelper_utils-0.0.5/PKG-INFO` & `pyhelper_utils-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pyhelper-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Collective utility functions for python projects
 Home-page: https://github.com/RedHatQE/pyhelper-utils
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: python-simple-logger (>=1.0.19,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Project-URL: Documentation, https://github.com/RedHatQE/pyhelper-utils/blob/main/README.md
 Project-URL: Repository, https://github.com/RedHatQE/pyhelper-utils
 Description-Content-Type: text/markdown
 
 # pyhelper-utils
 Repository for various python utilities
 ## Installation
```

