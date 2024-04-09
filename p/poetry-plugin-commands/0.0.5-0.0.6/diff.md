# Comparing `tmp/poetry_plugin_commands-0.0.5.tar.gz` & `tmp/poetry_plugin_commands-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_commands-0.0.5.tar", max compression
+gzip compressed data, was "poetry_plugin_commands-0.0.6.tar", max compression
```

## Comparing `poetry_plugin_commands-0.0.5.tar` & `poetry_plugin_commands-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.5/LICENSE
--rw-r--r--   0        0        0     1928 2024-04-08 01:11:27.879544 poetry_plugin_commands-0.0.5/README.md
--rw-r--r--   0        0        0     3210 2024-04-08 01:12:36.287540 poetry_plugin_commands-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-08 00:27:30.593692 poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/command.py
--rw-r--r--   0        0        0     1644 2024-04-08 00:44:09.905636 poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/plugins.py
--rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1928 2024-04-08 01:11:27.879544 poetry_plugin_commands-0.0.6/README.md
+-rw-r--r--   0        0        0     3210 2024-04-08 01:21:41.313509 poetry_plugin_commands-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-08 00:27:30.593692 poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/command.py
+-rw-r--r--   0        0        0     1644 2024-04-08 00:44:09.905636 poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/plugins.py
+-rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.6/PKG-INFO
```

### Comparing `poetry_plugin_commands-0.0.5/LICENSE` & `poetry_plugin_commands-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.5/README.md` & `poetry_plugin_commands-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.5/pyproject.toml` & `poetry_plugin_commands-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-commands"
-version = "0.0.5"
+version = "0.0.6"
 description = "Poetry plugin for simple custom user commands execution."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/command.py` & `poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.5/src/poetry_plugin_commands/plugins.py` & `poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.5/PKG-INFO` & `poetry_plugin_commands-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-commands
-Version: 0.0.5
+Version: 0.0.6
 Summary: Poetry plugin for simple custom user commands execution.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

