# Comparing `tmp/airbyte_source_faker-6.0.3.tar.gz` & `tmp/airbyte_source_faker-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_faker-6.0.3.tar", max compression
+gzip compressed data, was "airbyte_source_faker-6.1.0.tar", max compression
```

## Comparing `airbyte_source_faker-6.0.3.tar` & `airbyte_source_faker-6.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4478 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/README.md
--rw-r--r--   0        0        0      784 2024-03-21 18:05:30.762244 airbyte_source_faker-6.0.3/pyproject.toml
--rw-r--r--   0        0        0      122 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/__init__.py
--rw-r--r--   0        0        0      727 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/airbyte_message_with_cached_json.py
--rw-r--r--   0        0        0     4590 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/purchase_generator.py
--rw-r--r--   0        0        0    15346 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/record_data/products.json
--rw-r--r--   0        0        0      266 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/run.py
--rw-r--r--   0        0        0      529 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/schemas/products.json
--rw-r--r--   0        0        0      892 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/schemas/purchases.json
--rw-r--r--   0        0        0     1259 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/schemas/users.json
--rw-r--r--   0        0        0     1395 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/source.py
--rw-r--r--   0        0        0     1849 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/spec.json
--rw-r--r--   0        0        0     6705 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/streams.py
--rw-r--r--   0        0        0     3325 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/user_generator.py
--rw-r--r--   0        0        0      937 2024-03-21 16:27:54.000000 airbyte_source_faker-6.0.3/source_faker/utils.py
--rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 airbyte_source_faker-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4478 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/README.md
+-rw-r--r--   0        0        0      784 2024-04-09 13:40:55.907535 airbyte_source_faker-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/airbyte_message_with_cached_json.py
+-rw-r--r--   0        0        0     4590 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/purchase_generator.py
+-rw-r--r--   0        0        0    15356 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/record_data/products.json
+-rw-r--r--   0        0        0      266 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/run.py
+-rw-r--r--   0        0        0      529 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/schemas/products.json
+-rw-r--r--   0        0        0      892 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/schemas/purchases.json
+-rw-r--r--   0        0        0     1259 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/schemas/users.json
+-rw-r--r--   0        0        0     1395 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/source.py
+-rw-r--r--   0        0        0     1849 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/spec.json
+-rw-r--r--   0        0        0     6705 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/streams.py
+-rw-r--r--   0        0        0     3325 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/user_generator.py
+-rw-r--r--   0        0        0      937 2024-04-08 18:23:38.000000 airbyte_source_faker-6.1.0/source_faker/utils.py
+-rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 airbyte_source_faker-6.1.0/PKG-INFO
```

### Comparing `airbyte_source_faker-6.0.3/README.md` & `airbyte_source_faker-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/pyproject.toml` & `airbyte_source_faker-6.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "6.0.3"
+version = "6.1.0"
 name = "airbyte-source-faker"
 description = "Source implementation for fake but realistic looking data."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_faker-6.0.3/source_faker/airbyte_message_with_cached_json.py` & `airbyte_source_faker-6.1.0/source_faker/airbyte_message_with_cached_json.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/purchase_generator.py` & `airbyte_source_faker-6.1.0/source_faker/purchase_generator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/schemas/products.json` & `airbyte_source_faker-6.1.0/source_faker/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/schemas/purchases.json` & `airbyte_source_faker-6.1.0/source_faker/schemas/purchases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/schemas/users.json` & `airbyte_source_faker-6.1.0/source_faker/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/source.py` & `airbyte_source_faker-6.1.0/source_faker/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/spec.json` & `airbyte_source_faker-6.1.0/source_faker/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/streams.py` & `airbyte_source_faker-6.1.0/source_faker/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/user_generator.py` & `airbyte_source_faker-6.1.0/source_faker/user_generator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/source_faker/utils.py` & `airbyte_source_faker-6.1.0/source_faker/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.0.3/PKG-INFO` & `airbyte_source_faker-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-faker
-Version: 6.0.3
+Version: 6.1.0
 Summary: Source implementation for fake but realistic looking data.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

