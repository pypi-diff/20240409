# Comparing `tmp/apptrackr-0.2.2.tar.gz` & `tmp/apptrackr-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apptrackr-0.2.2.tar", max compression
+gzip compressed data, was "apptrackr-0.2.3.tar", max compression
```

## Comparing `apptrackr-0.2.2.tar` & `apptrackr-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.2/README.md
--rw-r--r--   0        0        0     1317 2024-04-08 16:17:56.451298 apptrackr-0.2.2/apptrackr/main.py
--rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.2/apptrackr/model/__init__.py
--rw-r--r--   0        0        0     1834 2024-04-08 18:13:10.963691 apptrackr-0.2.2/apptrackr/model/migrations.py
--rw-r--r--   0        0        0     1127 2024-04-08 17:17:42.625400 apptrackr-0.2.2/apptrackr/model/model.py
--rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.2/apptrackr/model/utils.py
--rw-r--r--   0        0        0      560 2024-04-08 16:19:41.302996 apptrackr-0.2.2/apptrackr/modules/config.py
--rw-r--r--   0        0        0    10154 2024-04-08 14:28:47.983920 apptrackr-0.2.2/apptrackr/modules/storage.py
--rw-r--r--   0        0        0      550 2024-04-08 18:13:37.101176 apptrackr-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 11:14:34.354815 apptrackr-0.2.3/README.md
+-rw-r--r--   0        0        0     1317 2024-04-08 16:17:56.451298 apptrackr-0.2.3/apptrackr/main.py
+-rw-r--r--   0        0        0       32 2024-04-04 17:56:32.559008 apptrackr-0.2.3/apptrackr/model/__init__.py
+-rw-r--r--   0        0        0     1834 2024-04-08 18:13:10.963691 apptrackr-0.2.3/apptrackr/model/migrations.py
+-rw-r--r--   0        0        0     1127 2024-04-08 17:17:42.625400 apptrackr-0.2.3/apptrackr/model/model.py
+-rw-r--r--   0        0        0     1892 2024-04-08 05:37:54.923684 apptrackr-0.2.3/apptrackr/model/utils.py
+-rw-r--r--   0        0        0      560 2024-04-08 16:19:41.302996 apptrackr-0.2.3/apptrackr/modules/config.py
+-rw-r--r--   0        0        0    10387 2024-04-09 06:19:21.658934 apptrackr-0.2.3/apptrackr/modules/storage.py
+-rw-r--r--   0        0        0      550 2024-04-09 06:23:56.719539 apptrackr-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 apptrackr-0.2.3/PKG-INFO
```

### Comparing `apptrackr-0.2.2/apptrackr/main.py` & `apptrackr-0.2.3/apptrackr/main.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.2/apptrackr/model/migrations.py` & `apptrackr-0.2.3/apptrackr/model/migrations.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.2/apptrackr/model/model.py` & `apptrackr-0.2.3/apptrackr/model/model.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.2/apptrackr/model/utils.py` & `apptrackr-0.2.3/apptrackr/model/utils.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.2/apptrackr/modules/config.py` & `apptrackr-0.2.3/apptrackr/modules/config.py`

 * *Files identical despite different names*

### Comparing `apptrackr-0.2.2/apptrackr/modules/storage.py` & `apptrackr-0.2.3/apptrackr/modules/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,26 +45,30 @@
     apply_link: Annotated[str, typer.Argument(help="Application link")],
     email_id_used: Annotated[
         str, typer.Argument(help="Email Id sent with application")
     ],
     location: Annotated[
         Optional[str], typer.Argument(help="Optional Job location")
     ] = None,
+    expectations: Annotated[
+        Optional[str], typer.Argument(help="Expectations with this application")
+    ] = None,
     date: Annotated[
         Optional[str], typer.Argument(help="Optional Application date")
     ] = None,
 ) -> None:
     """Add new application to the database.
 
     Args:
         name (Annotated[str, typer.Argument, optional): Job application name)].
         status (Annotated[str, typer.Argument, optional): Job status)].
         apply_link (Annotated[str, typer.Argument, optional): Application link)].
         email_id_used (Annotated[str], typer.Argument, optional): Optional Application date)].
         location (Annotated[ Optional[str], typer.Argument, optional): Optional Job location)]=None.
+        expectations (Annotated[ Optional[str], typer.Argument, optional): Optional Job Expectations)]=None.
         date (Annotated[ Optional[str], typer.Argument, optional): Optional Application date)]=None.:
     Raises:
         typer.Exit: For invalid arguments
     """
     if status not in ("active", "rejected", "accepted"):
         typer.secho("Invalid status argument!", fg=typer.colors.BRIGHT_RED)
         raise typer.Exit(-1)
```

### Comparing `apptrackr-0.2.2/pyproject.toml` & `apptrackr-0.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apptrackr"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Aradhya Tripathi <67282231+Aradhya-Tripathi@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `apptrackr-0.2.2/PKG-INFO` & `apptrackr-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apptrackr
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 License: MIT
 Author: Aradhya Tripathi
 Author-email: 67282231+Aradhya-Tripathi@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

