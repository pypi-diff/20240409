# Comparing `tmp/kivymd2_widgets-0.0.1.tar.gz` & `tmp/kivymd2_widgets-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivymd2_widgets-0.0.1.tar", max compression
+gzip compressed data, was "kivymd2_widgets-0.0.2.tar", max compression
```

## Comparing `kivymd2_widgets-0.0.1.tar` & `kivymd2_widgets-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11324 2024-04-08 22:35:55.505377 kivymd2_widgets-0.0.1/LICENSE
--rw-r--r--   0        0        0     2490 2024-04-08 23:45:53.521141 kivymd2_widgets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 20:23:43.633097 kivymd2_widgets-0.0.1/src/kivymd2_widgets/__init__.py
--rw-r--r--   0        0        0       40 2024-03-07 00:23:29.195481 kivymd2_widgets-0.0.1/src/kivymd2_widgets/pickers/__init__.py
--rw-r--r--   0        0        0       54 2024-03-04 00:22:00.225306 kivymd2_widgets-0.0.1/src/kivymd2_widgets/pickers/themepicker/__init__.py
--rw-r--r--   0        0        0     2377 2024-03-04 00:23:23.248301 kivymd2_widgets-0.0.1/src/kivymd2_widgets/pickers/themepicker/themepicker.kv
--rw-r--r--   0        0        0     1681 2024-03-04 00:23:32.206301 kivymd2_widgets-0.0.1/src/kivymd2_widgets/pickers/themepicker/themepicker.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 kivymd2_widgets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-08 22:35:55.505377 kivymd2_widgets-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2489 2024-04-09 00:16:59.111036 kivymd2_widgets-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 20:23:43.633097 kivymd2_widgets-0.0.2/src/kivymd2_widgets/__init__.py
+-rw-r--r--   0        0        0       40 2024-03-07 00:23:29.195481 kivymd2_widgets-0.0.2/src/kivymd2_widgets/pickers/__init__.py
+-rw-r--r--   0        0        0       54 2024-03-04 00:22:00.225306 kivymd2_widgets-0.0.2/src/kivymd2_widgets/pickers/themepicker/__init__.py
+-rw-r--r--   0        0        0     2377 2024-03-04 00:23:23.248301 kivymd2_widgets-0.0.2/src/kivymd2_widgets/pickers/themepicker/themepicker.kv
+-rw-r--r--   0        0        0     1681 2024-03-04 00:23:32.206301 kivymd2_widgets-0.0.2/src/kivymd2_widgets/pickers/themepicker/themepicker.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 kivymd2_widgets-0.0.2/PKG-INFO
```

### Comparing `kivymd2_widgets-0.0.1/LICENSE` & `kivymd2_widgets-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kivymd2_widgets-0.0.1/pyproject.toml` & `kivymd2_widgets-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "kivymd2_widgets"
-version = "0.0.1"
+version = "0.0.2"
 description = "Collection of widgets for the older kivymd 1.1.1 lib (material design 2)."
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 packages = [
     { include = "kivymd2_widgets", from = "src" },
 ]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/BlackCatDevel0per/kivymd2_widgets"
 Documentation = "https://github.com/BlackCatDevel0per/kivymd2_widgets"
 Repository = "https://github.com/BlackCatDevel0per/kivymd2_widgets"
 
 # TODO: Execute without wait to end (poetry will closed while task is pending)
-[tool.poetry.plugins.commands]
+[tool.poetry-plugin-commands]
 stree = "tree src"
 # TODO: Make some examples (like kivy garden or etc.)
 run-app = "PYTHONPATH=src:. poetry run python examples/pickers.py"
 
 [tool.ruff]
 line-length = 100
 select = [
```

### Comparing `kivymd2_widgets-0.0.1/src/kivymd2_widgets/pickers/themepicker/themepicker.kv` & `kivymd2_widgets-0.0.2/src/kivymd2_widgets/pickers/themepicker/themepicker.kv`

 * *Files identical despite different names*

### Comparing `kivymd2_widgets-0.0.1/src/kivymd2_widgets/pickers/themepicker/themepicker.py` & `kivymd2_widgets-0.0.2/src/kivymd2_widgets/pickers/themepicker/themepicker.py`

 * *Files identical despite different names*

### Comparing `kivymd2_widgets-0.0.1/PKG-INFO` & `kivymd2_widgets-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivymd2_widgets
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collection of widgets for the older kivymd 1.1.1 lib (material design 2).
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

