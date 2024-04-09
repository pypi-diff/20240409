# Comparing `tmp/cloud_orbit_api-1.1.14.tar.gz` & `tmp/cloud_orbit_api-1.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_orbit_api-1.1.14.tar", max compression
+gzip compressed data, was "cloud_orbit_api-1.1.15.tar", max compression
```

## Comparing `cloud_orbit_api-1.1.14.tar` & `cloud_orbit_api-1.1.15.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-04-09 08:48:44.647197 cloud_orbit_api-1.1.14/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:48:44.647197 cloud_orbit_api-1.1.14/cloud_orbit_api/__init__.py
--rw-r--r--   0        0        0     1123 2024-04-09 08:48:44.647197 cloud_orbit_api-1.1.14/cloud_orbit_api/db_factory.py
--rw-r--r--   0        0        0     1474 2024-04-09 08:48:44.647197 cloud_orbit_api-1.1.14/cloud_orbit_api/main.py
--rw-r--r--   0        0        0       90 2024-04-09 08:48:44.647197 cloud_orbit_api-1.1.14/cloud_orbit_api/models.py
--rw-r--r--   0        0        0      494 2024-04-09 08:49:03.731266 cloud_orbit_api-1.1.14/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 cloud_orbit_api-1.1.14/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-09 16:53:04.821055 cloud_orbit_api-1.1.15/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 16:53:04.821055 cloud_orbit_api-1.1.15/cloud_orbit_api/__init__.py
+-rw-r--r--   0        0        0     1123 2024-04-09 16:53:04.821055 cloud_orbit_api-1.1.15/cloud_orbit_api/db_factory.py
+-rw-r--r--   0        0        0     1473 2024-04-09 16:53:04.821055 cloud_orbit_api-1.1.15/cloud_orbit_api/main.py
+-rw-r--r--   0        0        0       90 2024-04-09 16:53:04.821055 cloud_orbit_api-1.1.15/cloud_orbit_api/models.py
+-rw-r--r--   0        0        0      494 2024-04-09 16:53:17.853045 cloud_orbit_api-1.1.15/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 cloud_orbit_api-1.1.15/PKG-INFO
```

### Comparing `cloud_orbit_api-1.1.14/cloud_orbit_api/db_factory.py` & `cloud_orbit_api-1.1.15/cloud_orbit_api/db_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_orbit_api-1.1.14/cloud_orbit_api/main.py` & `cloud_orbit_api-1.1.15/cloud_orbit_api/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from cloud_orbit_api.db_factory import SQLiteSingleton
 # Define the FastAPI app
 app = FastAPI(root_path="backend")
 SQLiteSingleton.get_instance()
 
 @app.get("/")
 async def root():
-    return {"Hello": "World!"}
+    return {"Hello": "Cloud"}
 
 
 # Endpoint to create an item
 @app.post("/items/")
 async def create_item(item: item):
     SQLiteSingleton._instance.cursor.execute(''' INSERT INTO items (name, description) VALUES (?, ?)''', (item.name, item.description))
     SQLiteSingleton._instance.conn.commit()
```

### Comparing `cloud_orbit_api-1.1.14/PKG-INFO` & `cloud_orbit_api-1.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-orbit-api
-Version: 1.1.14
+Version: 1.1.15
 Summary: This a demo project
 Author: sukruth grandhi
 Author-email: sukruthgrandhi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

