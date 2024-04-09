# Comparing `tmp/apptrackr-0.2.1.tar.gz` & `tmp/apptrackr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.2.1.tar", max compression
+gzip compressed data, was "apptrackr-0.2.2.tar", max compression
```

## Comparing `apptrackr-0.2.1.tar` & `apptrackr-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.1/README.md
--rw-r--r--   0        0        0     1315 2024-04-08 11:07:28.588800 apptrackr-0.2.1/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.1/apptrackr/model/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-06 11:11:27.442305 apptrackr-0.2.1/apptrackr/model/migrations.py
--rw-r--r--   0        0        0      767 2024-04-06 19:30:04.565191 apptrackr-0.2.1/apptrackr/model/model.py
--rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.1/apptrackr/model/utils.py
--rw-r--r--   0        0        0      560 2024-04-08 05:36:37.348441 apptrackr-0.2.1/apptrackr/modules/config.py
--rw-r--r--   0        0        0    10154 2024-04-08 14:28:47.983920 apptrackr-0.2.1/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      550 2024-04-08 15:00:48.036023 apptrackr-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.2/README.md
+-rw-r--r--   0        0        0     1317 2024-04-08 16:17:56.451298 apptrackr-0.2.2/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.2/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0     1834 2024-04-08 18:13:10.963691 apptrackr-0.2.2/apptrackr/model/migrations.py
+-rw-r--r--   0        0        0     1127 2024-04-08 17:17:42.625400 apptrackr-0.2.2/apptrackr/model/model.py
+-rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.2/apptrackr/model/utils.py
+-rw-r--r--   0        0        0      560 2024-04-08 16:19:41.302996 apptrackr-0.2.2/apptrackr/modules/config.py
+-rw-r--r--   0        0        0    10154 2024-04-08 14:28:47.983920 apptrackr-0.2.2/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      550 2024-04-08 18:13:37.101176 apptrackr-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.2/PKG-INFO
```

### Comparing `apptrackr-0.2.1/apptrackr/main.py` & `apptrackr-0.2.2/apptrackr/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 app = typer.Typer(no_args_is_help=True)
 app.add_typer(storage, name="store", help="Application management")
 app.add_typer(config, name="config", help="Recommendation configs")
 
 
 time_elapsed, company, link = get_last_applied_on()
 typer.secho(
-    f"Last application was {time_elapsed} {f'\nMaybe apply to {company}' if company else ''} {link if link else ''}",
+    f"Last application was {time_elapsed} {'' if not company else f'Maybe apply to {company}'} {link if link else ''}",
     fg=typer.colors.BRIGHT_BLUE,
 )
 
 
 @app.command()
 def make_migrations() -> None:
     """Django Style"""
```

### Comparing `apptrackr-0.2.1/apptrackr/model/utils.py` & `apptrackr-0.2.2/apptrackr/model/utils.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.1/apptrackr/modules/config.py` & `apptrackr-0.2.2/apptrackr/modules/config.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.1/apptrackr/modules/storage.py` & `apptrackr-0.2.2/apptrackr/modules/storage.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.1/pyproject.toml` & `apptrackr-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apptrackr"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Aradhya Tripathi <67282231+Aradhya-Tripathi@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `apptrackr-0.2.1/PKG-INFO` & `apptrackr-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

