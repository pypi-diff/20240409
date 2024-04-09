# Comparing `tmp/fractal_database_matrix-0.0.5.tar.gz` & `tmp/fractal_database_matrix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_database_matrix-0.0.5.tar", max compression
+gzip compressed data, was "fractal_database_matrix-0.0.6.tar", max compression
```

## Comparing `fractal_database_matrix-0.0.5.tar` & `fractal_database_matrix-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/LICENSE
--rw-r--r--   0        0        0       38 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/README.md
--rw-r--r--   0        0        0     2175 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/__init__.py
--rw-r--r--   0        0        0      146 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/admin.py
--rw-r--r--   0        0        0      176 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/apps.py
--rw-r--r--   0        0        0      985 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/broker.py
--rw-r--r--   0        0        0     3320 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/migrations/__init__.py
--rw-r--r--   0        0        0     4327 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/models.py
--rw-r--r--   0        0        0    12321 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/fractal_database_matrix/representations.py
--rw-r--r--   0        0        0      839 2024-03-18 20:40:45.419446 fractal_database_matrix-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 fractal_database_matrix-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/LICENSE
+-rw-r--r--   0        0        0       38 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/README.md
+-rw-r--r--   0        0        0     2175 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/admin.py
+-rw-r--r--   0        0        0      176 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/apps.py
+-rw-r--r--   0        0        0      853 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/broker.py
+-rw-r--r--   0        0        0     3320 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/migrations/__init__.py
+-rw-r--r--   0        0        0     5677 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/models.py
+-rw-r--r--   0        0        0    12429 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/fractal_database_matrix/representations.py
+-rw-r--r--   0        0        0      839 2024-04-09 18:16:34.979972 fractal_database_matrix-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 fractal_database_matrix-0.0.6/PKG-INFO
```

### Comparing `fractal_database_matrix-0.0.5/LICENSE` & `fractal_database_matrix-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_database_matrix-0.0.5/fractal_database_matrix/__init__.py` & `fractal_database_matrix-0.0.6/fractal_database_matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_database_matrix-0.0.5/fractal_database_matrix/broker.py` & `fractal_database_matrix-0.0.6/fractal_database_matrix/broker.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 from taskiq_matrix.matrix_broker import MatrixBroker
 from taskiq_matrix.matrix_result_backend import MatrixResultBackend
 from taskiq_matrix.schedulesource import MatrixRoomScheduleSource
 
 broker = (
     MatrixBroker()
     .with_matrix_config(
-        room_id=os.environ.get("MATRIX_ROOM_ID"),
-        homeserver_url=os.environ.get("MATRIX_HOMESERVER_URL"),
-        access_token=os.environ.get("MATRIX_ACCESS_TOKEN"),
+        os.environ.get("MATRIX_HOMESERVER_URL"),
+        os.environ.get("MATRIX_ACCESS_TOKEN"),
     )
     .with_result_backend(
         MatrixResultBackend(
-            room_id=os.environ.get("MATRIX_ROOM_ID"),
             homeserver_url=os.environ.get("MATRIX_HOMESERVER_URL"),
             access_token=os.environ.get("MATRIX_ACCESS_TOKEN"),
             result_ex_time=60,
         )
     )
     .with_middlewares(SimpleRetryMiddleware(default_retry_count=3))
 )
```

### Comparing `fractal_database_matrix-0.0.5/fractal_database_matrix/migrations/0001_initial.py` & `fractal_database_matrix-0.0.6/fractal_database_matrix/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 5.0.3 on 2024-03-18 20:00
+# Generated by Django 5.0.3 on 2024-03-25 19:52
 
 import django.db.models.deletion
 import uuid
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
```

### Comparing `fractal_database_matrix-0.0.5/fractal_database_matrix/representations.py` & `fractal_database_matrix-0.0.6/fractal_database_matrix/representations.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,16 +230,20 @@
 
         await self.add_subspace(target, room_id, devices_room_id)
 
         target.metadata["room_id"] = room_id
         target.metadata["devices_room_id"] = room_id
 
         if target.database:
-            initial_state[0]["content"]["fixture"] = target.database.to_fixture(json=True)
-        initial_state[1]["content"]["fixture"] = target.to_fixture(json=True)
+            initial_state[0]["content"]["fixture"] = await target.database.ato_fixture(
+                json=True, with_relations=True
+            )
+        initial_state[1]["content"]["fixture"] = await target.ato_fixture(
+            json=True, with_relations=True
+        )
 
         await self.put_state(room_id, target, "f.database", initial_state[0]["content"])
         await self.put_state(room_id, target, "f.database.target", initial_state[1]["content"])
 
         logger.info(
             "Successfully created Matrix Space representation for %s on target %s"
             % (name, target)
```

### Comparing `fractal_database_matrix-0.0.5/pyproject.toml` & `fractal_database_matrix-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-database-matrix"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Justin <jrussel1055@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = "^5.0.0"
```

### Comparing `fractal_database_matrix-0.0.5/PKG-INFO` & `fractal_database_matrix-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-database-matrix
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Justin
 Author-email: jrussel1055@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

