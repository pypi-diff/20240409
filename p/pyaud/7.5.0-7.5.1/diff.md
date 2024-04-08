# Comparing `tmp/pyaud-7.5.0.tar.gz` & `tmp/pyaud-7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaud-7.5.0.tar", max compression
+gzip compressed data, was "pyaud-7.5.1.tar", max compression
```

## Comparing `pyaud-7.5.0.tar` & `pyaud-7.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2024-01-06 00:17:05.482030 pyaud-7.5.0/LICENSE
--rw-r--r--   0        0        0     4308 2024-02-01 03:27:53.852672 pyaud-7.5.0/README.rst
--rw-r--r--   0        0        0      326 2024-01-31 10:25:00.716168 pyaud-7.5.0/pyaud/__init__.py
--rw-r--r--   0        0        0      153 2024-01-31 10:25:00.719960 pyaud-7.5.0/pyaud/__main__.py
--rw-r--r--   0        0        0     2025 2024-01-31 10:25:00.736528 pyaud-7.5.0/pyaud/_builtins.py
--rw-r--r--   0        0        0     1606 2024-01-31 10:25:00.737283 pyaud-7.5.0/pyaud/_cachedir.py
--rw-r--r--   0        0        0     1782 2024-01-31 10:25:00.733025 pyaud-7.5.0/pyaud/_config.py
--rw-r--r--   0        0        0     1060 2024-01-31 10:25:00.731762 pyaud-7.5.0/pyaud/_core.py
--rw-r--r--   0        0        0     1352 2024-01-31 10:25:00.736961 pyaud-7.5.0/pyaud/_files.py
--rw-r--r--   0        0        0      751 2024-01-31 10:25:00.745108 pyaud-7.5.0/pyaud/_main.py
--rw-r--r--   0        0        0      170 2024-01-31 10:25:00.734197 pyaud-7.5.0/pyaud/_objects.py
--rw-r--r--   0        0        0      209 2024-02-01 03:53:38.482082 pyaud-7.5.0/pyaud/_version.py
--rw-r--r--   0        0        0      661 2024-01-31 10:25:00.736192 pyaud-7.5.0/pyaud/exceptions.py
--rw-r--r--   0        0        0      783 2024-01-31 10:25:00.741118 pyaud-7.5.0/pyaud/messages.py
--rw-r--r--   0        0        0    22197 2024-01-31 10:25:00.832288 pyaud-7.5.0/pyaud/plugins.py
--rw-r--r--   0        0        0        0 2023-09-17 09:37:53.784112 pyaud-7.5.0/pyaud/py.typed
--rw-r--r--   0        0        0     2259 2024-02-01 03:53:38.482227 pyaud-7.5.0/pyproject.toml
--rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 pyaud-7.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-03 03:09:11.071127 pyaud-7.5.1/LICENSE
+-rw-r--r--   0        0        0     4308 2024-04-08 23:39:27.961519 pyaud-7.5.1/README.rst
+-rw-r--r--   0        0        0      326 2024-02-03 03:09:11.073258 pyaud-7.5.1/pyaud/__init__.py
+-rw-r--r--   0        0        0      153 2024-02-03 03:09:11.073358 pyaud-7.5.1/pyaud/__main__.py
+-rw-r--r--   0        0        0     2025 2024-02-03 03:09:11.073593 pyaud-7.5.1/pyaud/_builtins.py
+-rw-r--r--   0        0        0     1606 2024-02-03 03:09:11.073699 pyaud-7.5.1/pyaud/_cachedir.py
+-rw-r--r--   0        0        0     1782 2024-02-03 03:09:11.073803 pyaud-7.5.1/pyaud/_config.py
+-rw-r--r--   0        0        0     1060 2024-02-03 03:09:11.074146 pyaud-7.5.1/pyaud/_core.py
+-rw-r--r--   0        0        0     1352 2024-02-03 03:09:11.074276 pyaud-7.5.1/pyaud/_files.py
+-rw-r--r--   0        0        0      751 2024-02-03 03:09:11.074383 pyaud-7.5.1/pyaud/_main.py
+-rw-r--r--   0        0        0      170 2024-02-03 03:09:11.074507 pyaud-7.5.1/pyaud/_objects.py
+-rw-r--r--   0        0        0      209 2024-04-08 23:42:51.369541 pyaud-7.5.1/pyaud/_version.py
+-rw-r--r--   0        0        0      661 2024-02-03 03:09:11.074860 pyaud-7.5.1/pyaud/exceptions.py
+-rw-r--r--   0        0        0      783 2024-02-03 03:09:11.074979 pyaud-7.5.1/pyaud/messages.py
+-rw-r--r--   0        0        0    22197 2024-02-03 03:09:11.075167 pyaud-7.5.1/pyaud/plugins.py
+-rw-r--r--   0        0        0        0 2023-09-17 09:37:53.784112 pyaud-7.5.1/pyaud/py.typed
+-rw-r--r--   0        0        0     2260 2024-04-08 23:42:51.369701 pyaud-7.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 pyaud-7.5.1/PKG-INFO
```

### Comparing `pyaud-7.5.0/LICENSE` & `pyaud-7.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/README.rst` & `pyaud-7.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/_builtins.py` & `pyaud-7.5.1/pyaud/_builtins.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/_cachedir.py` & `pyaud-7.5.1/pyaud/_cachedir.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/_config.py` & `pyaud-7.5.1/pyaud/_config.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/_core.py` & `pyaud-7.5.1/pyaud/_core.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/_files.py` & `pyaud-7.5.1/pyaud/_files.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/_main.py` & `pyaud-7.5.1/pyaud/_main.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/exceptions.py` & `pyaud-7.5.1/pyaud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/messages.py` & `pyaud-7.5.1/pyaud/messages.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyaud/plugins.py` & `pyaud-7.5.1/pyaud/plugins.py`

 * *Files identical despite different names*

### Comparing `pyaud-7.5.0/pyproject.toml` & `pyaud-7.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -70,32 +70,32 @@
 license = "MIT"
 maintainers = [
   "jshwi <stephen@jshwisolutions.com>"
 ]
 name = "pyaud"
 readme = "README.rst"
 repository = "https://github.com/jshwi/pyaud"
-version = "7.5.0"
+version = "7.5.1"
 
 [tool.poetry.dependencies]
-arcon = "^0.3.1"
+arcon = ">=0.3.1"
 gitpython = "^3.1.30"
 lsfiles = ">=0.5"
 object-colors = "^2.0.1"
 pyaud-plugins = ">=0.22.0"
 python = "^3.8"
 rich = "^13.5.2"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 deptry = "^0.12.0"
 ipython = "^8.4.0"
 pre-commit = "^3.1.1"
 pytest-randomly = "^3.12.0"
-pytest-sugar = "^0.9.5"
+pytest-sugar = "^1.0.0"
 restview = "^3.0.0"
 sphinx-immaterial = "^0.11.10"
 sphinx-toolbox = "^3.5.0"
 templatest = "^0.10.1"
 
 [tool.poetry.scripts]
 pyaud = "pyaud.__main__:main"
```

### Comparing `pyaud-7.5.0/PKG-INFO` & `pyaud-7.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaud
-Version: 7.5.0
+Version: 7.5.1
 Summary: Framework for writing Python package audits
 Home-page: https://pypi.org/project/pyaud/
 License: MIT
 Keywords: audit,ci,fix,format,style
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: arcon (>=0.3.1,<0.4.0)
+Requires-Dist: arcon (>=0.3.1)
 Requires-Dist: gitpython (>=3.1.30,<4.0.0)
 Requires-Dist: lsfiles (>=0.5)
 Requires-Dist: object-colors (>=2.0.1,<3.0.0)
 Requires-Dist: pyaud-plugins (>=0.22.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Project-URL: Documentation, https://pyaud.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/jshwi/pyaud
```

