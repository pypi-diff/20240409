# Comparing `tmp/sprocketship-0.4.2.tar.gz` & `tmp/sprocketship-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.4.2.tar", last modified: Mon Apr  8 16:17:57 2024, max compression
+gzip compressed data, was "sprocketship-0.5.0.tar", last modified: Tue Apr  9 00:56:14 2024, max compression
```

## Comparing `sprocketship-0.4.2.tar` & `sprocketship-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.552197 sprocketship-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 16:17:47.000000 sprocketship-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 16:17:47.000000 sprocketship-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-08 16:17:57.552197 sprocketship-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-08 16:17:47.000000 sprocketship-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-08 16:17:47.000000 sprocketship-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:17:57.552197 sprocketship-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.548197 sprocketship-0.4.2/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-08 16:17:47.000000 sprocketship-0.4.2/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.552197 sprocketship-0.4.2/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 16:17:47.000000 sprocketship-0.4.2/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-08 16:17:47.000000 sprocketship-0.4.2/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.552197 sprocketship-0.4.2/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:56:14.483254 sprocketship-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 00:56:05.000000 sprocketship-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 00:56:05.000000 sprocketship-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-09 00:56:14.483254 sprocketship-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-09 00:56:05.000000 sprocketship-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 00:56:05.000000 sprocketship-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:56:14.483254 sprocketship-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:56:14.479254 sprocketship-0.5.0/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-09 00:56:05.000000 sprocketship-0.5.0/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:56:14.479254 sprocketship-0.5.0/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 00:56:05.000000 sprocketship-0.5.0/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-09 00:56:05.000000 sprocketship-0.5.0/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:56:14.479254 sprocketship-0.5.0/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-09 00:56:14.000000 sprocketship-0.5.0/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-09 00:56:14.000000 sprocketship-0.5.0/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:56:14.000000 sprocketship-0.5.0/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 00:56:14.000000 sprocketship-0.5.0/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 00:56:14.000000 sprocketship-0.5.0/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 00:56:14.000000 sprocketship-0.5.0/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.4.2/LICENSE` & `sprocketship-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.2/PKG-INFO` & `sprocketship-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.4.2
+Version: 0.5.0
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.4.2 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.5.0 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
```

### Comparing `sprocketship-0.4.2/README.md` & `sprocketship-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.2/pyproject.toml` & `sprocketship-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.4.2"
+version = "0.5.0"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.4.2/sprocketship/cli.py` & `sprocketship-0.5.0/sprocketship/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 
     err = False
     for proc in procs:
         try:
             rendered_proc = create_javascript_stored_procedure(
                 **proc, **{"project_dir": dir}
             )
+            if 'use_role' in proc.keys():
+                con.cursor().execute(f"USE ROLE {proc['use_role'].upper()}")
+            else:
+                con.cursor().execute(f"USE ROLE {data['snowflake']['role']}")
             con.cursor().execute(rendered_proc)
             msg = click.style(f"{proc['name']} ", fg="green", bold=True)
             msg += click.style(f"launched into schema ", fg="white", bold=True)
             msg += click.style(
                 f"{proc['database']}.{proc['schema']}", fg="blue", bold=True
             )
             click.echo(msg)
@@ -76,15 +80,15 @@
 
     err = False
     for proc in procs:
         try:
             rendered_proc = create_javascript_stored_procedure(
                 **proc, **{"project_dir": dir}
             )
-            with open(os.path.join(dir, target, proc["name"] + ".sql"), "+a") as f:
+            with open(os.path.join(dir, target, proc["name"] + ".sql"), "w") as f:
                 f.write(rendered_proc)
             msg = click.style(f"{proc['name']} ", fg="green", bold=True)
             msg += click.style(f"successfully built", fg="white", bold=True)
             click.echo(msg)
         except Exception as e:
             err = True
             msg = click.style(f"{proc['name']} ", fg="red", bold=True)
```

### Comparing `sprocketship-0.4.2/sprocketship/utils.py` & `sprocketship-0.5.0/sprocketship/utils.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.2/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.5.0/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.4.2
+Version: 0.5.0
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.4.2 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.5.0 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
```

