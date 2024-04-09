# Comparing `tmp/gogotable-0.0.2.tar.gz` & `tmp/gogotable-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogotable-0.0.2.tar", max compression
+gzip compressed data, was "gogotable-0.0.3.tar", max compression
```

## Comparing `gogotable-0.0.2.tar` & `gogotable-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-04-09 17:41:01.686245 gogotable-0.0.2/LICENSE
--rw-r--r--   0        0        0      532 2024-04-09 17:45:41.048846 gogotable-0.0.2/README.md
--rw-r--r--   0        0        0      885 2024-04-09 17:53:03.313440 gogotable-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-09 17:43:34.216229 gogotable-0.0.2/src/gogotable/__init__.py
--rw-r--r--   0        0        0     1447 2024-04-09 17:52:10.851633 gogotable-0.0.2/src/gogotable/gogotable.py
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 gogotable-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-09 17:41:01.686245 gogotable-0.0.3/LICENSE
+-rw-r--r--   0        0        0      627 2024-04-09 19:35:49.594688 gogotable-0.0.3/README.md
+-rw-r--r--   0        0        0      885 2024-04-09 19:36:47.565136 gogotable-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-09 19:09:26.225741 gogotable-0.0.3/src/gogotable/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-09 19:30:07.297188 gogotable-0.0.3/src/gogotable/gogotable.py
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 gogotable-0.0.3/PKG-INFO
```

### Comparing `gogotable-0.0.2/LICENSE` & `gogotable-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gogotable-0.0.2/README.md` & `gogotable-0.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # GoGoTable
 
+[![PyPI version](https://badge.fury.io/py/gogotable.svg)](https://badge.fury.io/py/gogotable)
+
 Converts structured data to a table.
 
 ## Setup Development Environonment
 
 you need the following tools installed on your machine:
 
 - [Poetry](https://python-poetry.org) for Python package management.
```

### Comparing `gogotable-0.0.2/pyproject.toml` & `gogotable-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "gogotable"
-version = "0.0.2"
+version = "0.0.3"
 description = "Convert structured data to a table"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "gogotable", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `gogotable-0.0.2/PKG-INFO` & `gogotable-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogotable
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert structured data to a table
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # GoGoTable
 
+[![PyPI version](https://badge.fury.io/py/gogotable.svg)](https://badge.fury.io/py/gogotable)
+
 Converts structured data to a table.
 
 ## Setup Development Environonment
 
 you need the following tools installed on your machine:
 
 - [Poetry](https://python-poetry.org) for Python package management.
```

