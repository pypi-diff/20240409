# Comparing `tmp/fastenv-0.4.0.tar.gz` & `tmp/fastenv-0.4.1.tar.gz`

## Comparing `fastenv-0.4.0.tar` & `fastenv-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/__init__.py
--rw-r--r--   0        0        0     8709 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/dotenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/py.typed
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/types.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/cloud/__init__.py
--rw-r--r--   0        0        0    40262 2020-02-02 00:00:00.000000 fastenv-0.4.0/fastenv/cloud/object_storage.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 fastenv-0.4.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastenv-0.4.0/LICENSE
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 fastenv-0.4.0/README.md
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 fastenv-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 fastenv-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/__init__.py
+-rw-r--r--   0        0        0     8709 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/dotenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/py.typed
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/types.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/utilities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/cloud/__init__.py
+-rw-r--r--   0        0        0    40262 2020-02-02 00:00:00.000000 fastenv-0.4.1/fastenv/cloud/object_storage.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 fastenv-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastenv-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 fastenv-0.4.1/README.md
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 fastenv-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 fastenv-0.4.1/PKG-INFO
```

### Comparing `fastenv-0.4.0/fastenv/__init__.py` & `fastenv-0.4.1/fastenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """fastenv
 
 Unified environment variable and settings management for FastAPI and beyond.
 
 https://github.com/br3ndonland/fastenv
 """
+
 try:
     from .cloud.object_storage import ObjectStorageClient, ObjectStorageConfig
 except ImportError:  # pragma: no cover
     pass
 from .dotenv import DotEnv, dotenv_values, dump_dotenv, find_dotenv, load_dotenv
 
 __all__ = (
@@ -15,8 +16,8 @@
     "ObjectStorageClient",
     "ObjectStorageConfig",
     "dotenv_values",
     "dump_dotenv",
     "find_dotenv",
     "load_dotenv",
 )
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `fastenv-0.4.0/fastenv/dotenv.py` & `fastenv-0.4.1/fastenv/dotenv.py`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.0/fastenv/types.py` & `fastenv-0.4.1/fastenv/types.py`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.0/fastenv/cloud/object_storage.py` & `fastenv-0.4.1/fastenv/cloud/object_storage.py`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.0/.gitignore` & `fastenv-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.0/LICENSE` & `fastenv-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.0/README.md` & `fastenv-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.0/pyproject.toml` & `fastenv-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling"]
+requires = ["hatchling<1.22"]
 
 [project]
 authors = [{email = "bws@bws.bio", name = "Brendon Smith"}]
 classifiers = [
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "Natural Language :: English",
@@ -17,28 +17,28 @@
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Topic :: System :: Installation/Setup",
   "Topic :: System :: Systems Administration",
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
 dependencies = [
-  "anyio>=3.3,<4",
+  "anyio>=3.3,<5",
 ]
 description = "Unified environment variable and settings management for FastAPI and beyond."
 dynamic = ["version"]
 keywords = ["asgi", "dotenv", "environment variables", "fastapi", "settings"]
 license = "MIT"
 name = "fastenv"
 readme = "README.md"
 requires-python = ">=3.8.1,<4"
 
 [project.optional-dependencies]
 checks = [
-  "mypy==1.8.0",
-  "ruff>=0.1,<0.2",
+  "mypy==1.9.0",
+  "ruff>=0.3,<0.4",
 ]
 cloud = [
   "httpx>=0.23,<1",
 ]
 docs = [
   "mkdocs-material>=9,<10",
 ]
@@ -120,15 +120,17 @@
 
 [tool.pytest.ini_options]
 addopts = "-q"
 minversion = "6.0"
 testpaths = ["tests"]
 
 [tool.ruff]
-extend-select = ["I"]
 src = ["fastenv", "tests"]
 
 [tool.ruff.format]
 docstring-code-format = true
 
+[tool.ruff.lint]
+extend-select = ["I"]
+
 [tool.ruff.lint.isort]
 known-first-party = ["fastenv", "tests"]
```

### Comparing `fastenv-0.4.0/PKG-INFO` & `fastenv-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastenv
-Version: 0.4.0
+Version: 0.4.1
 Summary: Unified environment variable and settings management for FastAPI and beyond.
 Project-URL: Documentation, https://fastenv.bws.bio
 Project-URL: Homepage, https://github.com/br3ndonland/fastenv
 Project-URL: Repository, https://github.com/br3ndonland/fastenv
 Author-email: Brendon Smith <bws@bws.bio>
 License-Expression: MIT
 License-File: LICENSE
@@ -20,18 +20,18 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.8.1
-Requires-Dist: anyio<4,>=3.3
+Requires-Dist: anyio<5,>=3.3
 Provides-Extra: checks
-Requires-Dist: mypy==1.8.0; extra == 'checks'
-Requires-Dist: ruff<0.2,>=0.1; extra == 'checks'
+Requires-Dist: mypy==1.9.0; extra == 'checks'
+Requires-Dist: ruff<0.4,>=0.3; extra == 'checks'
 Provides-Extra: cloud
 Requires-Dist: httpx<1,>=0.23; extra == 'cloud'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material<10,>=9; extra == 'docs'
 Provides-Extra: httpx
 Requires-Dist: httpx<1,>=0.23; extra == 'httpx'
 Provides-Extra: tests
```

