# Comparing `tmp/deltares_datasuite-0.4.0.tar.gz` & `tmp/deltares_datasuite-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltares_datasuite-0.4.0.tar", max compression
+gzip compressed data, was "deltares_datasuite-0.5.0.tar", max compression
```

## Comparing `deltares_datasuite-0.4.0.tar` & `deltares_datasuite-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-11-07 09:52:00.641547 deltares_datasuite-0.4.0/LICENSE
--rw-r--r--   0        0        0     8050 2023-11-10 13:30:24.947866 deltares_datasuite-0.4.0/README.md
--rw-r--r--   0        0        0      633 2023-11-07 09:52:00.643471 deltares_datasuite-0.4.0/deltares_datasuite/__init__.py
--rw-r--r--   0        0        0       91 2023-11-07 09:52:00.643691 deltares_datasuite-0.4.0/deltares_datasuite/client/__init__.py
--rw-r--r--   0        0        0     3554 2023-11-07 09:52:00.643795 deltares_datasuite-0.4.0/deltares_datasuite/client/dms_client.py
--rw-r--r--   0        0        0       88 2023-11-07 09:52:00.644088 deltares_datasuite-0.4.0/deltares_datasuite/core/__init__.py
--rw-r--r--   0        0        0       42 2023-11-07 09:52:00.644351 deltares_datasuite-0.4.0/deltares_datasuite/core/models/__init__.py
--rw-r--r--   0        0        0     7295 2023-11-10 13:30:24.948230 deltares_datasuite-0.4.0/deltares_datasuite/core/models/item.py
--rw-r--r--   0        0        0     3836 2023-11-10 14:51:42.293781 deltares_datasuite-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9233 1970-01-01 00:00:00.000000 deltares_datasuite-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8050 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/README.md
+-rw-r--r--   0        0        0      633 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/deltares_datasuite/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/deltares_datasuite/client/__init__.py
+-rw-r--r--   0        0        0     3554 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/deltares_datasuite/client/dms_client.py
+-rw-r--r--   0        0        0       88 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/deltares_datasuite/core/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/deltares_datasuite/core/models/__init__.py
+-rw-r--r--   0        0        0     7295 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/deltares_datasuite/core/models/item.py
+-rw-r--r--   0        0        0     3871 2024-04-09 09:39:59.145419 deltares_datasuite-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9279 1970-01-01 00:00:00.000000 deltares_datasuite-0.5.0/PKG-INFO
```

### Comparing `deltares_datasuite-0.4.0/LICENSE` & `deltares_datasuite-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltares_datasuite-0.4.0/README.md` & `deltares_datasuite-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `deltares_datasuite-0.4.0/deltares_datasuite/__init__.py` & `deltares_datasuite-0.5.0/deltares_datasuite/__init__.py`

 * *Files identical despite different names*

### Comparing `deltares_datasuite-0.4.0/deltares_datasuite/client/dms_client.py` & `deltares_datasuite-0.5.0/deltares_datasuite/client/dms_client.py`

 * *Files identical despite different names*

### Comparing `deltares_datasuite-0.4.0/deltares_datasuite/core/models/item.py` & `deltares_datasuite-0.5.0/deltares_datasuite/core/models/item.py`

 * *Files identical despite different names*

### Comparing `deltares_datasuite-0.4.0/pyproject.toml` & `deltares_datasuite-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "deltares_datasuite"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python package to create and update STAC items in the Deltares Data Management Suite"
 readme = "README.md"
 authors = ["Deltares <nathan.clerks@deltares.nl>"]
 maintainers = ["Deltares <nathan.clerks@deltares.nl>"]
 license = "MIT"
 repository = "https://github.com/Deltares-research/data-management-suite"
 homepage = "https://datasuite.deltares.nl"
@@ -32,18 +32,19 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pystac = "^1.8.4"
 geojson = "^3.0.1"
 requests = "^2.31.0"
 types-requests = "^2.31.0.10"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-bandit = "^1.7.5"
-black = { version = "^23.11.0", allow-prereleases = true }
+bandit = "^1.7.7"
+black = { version = ">=23.11,<25.0", allow-prereleases = true }
 darglint = "^1.8.1"
 isort = { extras = ["colors"], version = "^5.12.0" }
 mypy = "^1.6.1"
 pre-commit = "^3.5.0"
 pydocstyle = "^6.3.0"
 pylint = "^3.0.2"
 pytest = "^7.4.3"
@@ -52,15 +53,15 @@
 coverage = "^7.3.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^4.1.1"
 pytest-cov = "^4.1.0"
 psycopg = { extras = ["binary"], version = "^3.1.12" }
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.4.8"
-mkdocstrings = { extras = ["python"], version = "^0.23.0" }
+mkdocstrings = { extras = ["python"], version = ">=0.23,<0.25" }
 mkdocs-macros-plugin = "^1.0.5"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
 color = true
```

### Comparing `deltares_datasuite-0.4.0/PKG-INFO` & `deltares_datasuite-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltares_datasuite
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package to create and update STAC items in the Deltares Data Management Suite
 Home-page: https://datasuite.deltares.nl
 License: MIT
 Author: Deltares
 Author-email: nathan.clerks@deltares.nl
 Maintainer: Deltares
 Maintainer-email: nathan.clerks@deltares.nl
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: geojson (>=3.0.1,<4.0.0)
 Requires-Dist: pystac (>=1.8.4,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-requests (>=2.31.0.10,<3.0.0.0)
 Project-URL: Documentation, https://datasuite.deltares.nl/docs
 Project-URL: Repository, https://github.com/Deltares-research/data-management-suite
 Description-Content-Type: text/markdown
 
 # deltares_datasuite
```

