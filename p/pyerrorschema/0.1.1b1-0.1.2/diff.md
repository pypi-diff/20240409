# Comparing `tmp/pyerrorschema-0.1.1b1.tar.gz` & `tmp/pyerrorschema-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerrorschema-0.1.1b1.tar", last modified: Mon Mar 25 07:17:38 2024, max compression
+gzip compressed data, was "pyerrorschema-0.1.2.tar", last modified: Tue Apr  9 02:01:09 2024, max compression
```

## Comparing `pyerrorschema-0.1.1b1.tar` & `pyerrorschema-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-03-25 07:17:38.124924 pyerrorschema-0.1.1b1/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     1530 2024-03-22 05:08:42.000000 pyerrorschema-0.1.1b1/LICENSE.txt
--rw-r--r--   0 elliot    (1000) elliot    (1000)     3092 2024-03-25 07:17:38.124924 pyerrorschema-0.1.1b1/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      754 2024-03-25 07:16:11.000000 pyerrorschema-0.1.1b1/README.md
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-03-25 07:17:38.124924 pyerrorschema-0.1.1b1/pyerrorschema/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      206 2024-03-25 06:52:53.000000 pyerrorschema-0.1.1b1/pyerrorschema/__init__.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     1271 2024-03-22 05:42:23.000000 pyerrorschema-0.1.1b1/pyerrorschema/base_error_schema.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     1111 2024-03-22 05:44:59.000000 pyerrorschema-0.1.1b1/pyerrorschema/fastapi_error_schema.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      711 2024-03-22 05:41:43.000000 pyerrorschema-0.1.1b1/pyerrorschema/utils.py
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-03-25 07:17:38.124924 pyerrorschema-0.1.1b1/pyerrorschema.egg-info/
--rw-r--r--   0 elliot    (1000) elliot    (1000)     3092 2024-03-25 07:17:38.000000 pyerrorschema-0.1.1b1/pyerrorschema.egg-info/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      342 2024-03-25 07:17:38.000000 pyerrorschema-0.1.1b1/pyerrorschema.egg-info/SOURCES.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-03-25 07:17:38.000000 pyerrorschema-0.1.1b1/pyerrorschema.egg-info/dependency_links.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       16 2024-03-25 07:17:38.000000 pyerrorschema-0.1.1b1/pyerrorschema.egg-info/requires.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       14 2024-03-25 07:17:38.000000 pyerrorschema-0.1.1b1/pyerrorschema.egg-info/top_level.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      675 2024-03-25 06:44:45.000000 pyerrorschema-0.1.1b1/pyproject.toml
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-03-25 07:17:38.124924 pyerrorschema-0.1.1b1/setup.cfg
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-09 02:01:09.100382 pyerrorschema-0.1.2/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1530 2024-03-22 05:08:42.000000 pyerrorschema-0.1.2/LICENSE.txt
+-rw-r--r--   0 elliot    (1000) elliot    (1000)     3090 2024-04-09 02:01:09.100382 pyerrorschema-0.1.2/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      754 2024-03-25 07:16:11.000000 pyerrorschema-0.1.2/README.md
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-09 02:01:09.100382 pyerrorschema-0.1.2/pyerrorschema/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      205 2024-03-26 03:09:19.000000 pyerrorschema-0.1.2/pyerrorschema/__init__.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1158 2024-03-26 03:44:56.000000 pyerrorschema-0.1.2/pyerrorschema/base_error_schema.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1451 2024-03-26 03:44:56.000000 pyerrorschema-0.1.2/pyerrorschema/fastapi_error_schema.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      711 2024-04-09 01:41:11.000000 pyerrorschema-0.1.2/pyerrorschema/utils.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-09 02:01:09.100382 pyerrorschema-0.1.2/pyerrorschema.egg-info/
+-rw-r--r--   0 elliot    (1000) elliot    (1000)     3090 2024-04-09 02:01:09.000000 pyerrorschema-0.1.2/pyerrorschema.egg-info/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      409 2024-04-09 02:01:09.000000 pyerrorschema-0.1.2/pyerrorschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-09 02:01:09.000000 pyerrorschema-0.1.2/pyerrorschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       16 2024-04-09 02:01:09.000000 pyerrorschema-0.1.2/pyerrorschema.egg-info/requires.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       14 2024-04-09 02:01:09.000000 pyerrorschema-0.1.2/pyerrorschema.egg-info/top_level.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      811 2024-04-09 02:00:29.000000 pyerrorschema-0.1.2/pyproject.toml
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-09 02:01:09.100382 pyerrorschema-0.1.2/setup.cfg
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-09 02:01:09.100382 pyerrorschema-0.1.2/tests/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      330 2024-03-25 09:48:26.000000 pyerrorschema-0.1.2/tests/test_base_error_schema.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2812 2024-03-26 01:59:31.000000 pyerrorschema-0.1.2/tests/test_fastapi_error_schema.py
```

### Comparing `pyerrorschema-0.1.1b1/LICENSE.txt` & `pyerrorschema-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyerrorschema-0.1.1b1/PKG-INFO` & `pyerrorschema-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrorschema
-Version: 0.1.1b1
+Version: 0.1.2
 Summary: Error schema validator
 Author-email: Elliot Su <sodinfeliz@google.com>
 License: Copyright (c) 2024, Elliot Su.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are
```

### Comparing `pyerrorschema-0.1.1b1/README.md` & `pyerrorschema-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyerrorschema-0.1.1b1/pyerrorschema/base_error_schema.py` & `pyerrorschema-0.1.2/pyerrorschema/base_error_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
+
 from .utils import restrict_arguments
 
 
 class ErrorSchema(BaseModel):
+    model_config = ConfigDict(extra="forbid")
+
     type: str = Field(default="")
     msg: str = Field(default="")
     
     def __new__(cls, *args, **kwargs):
         if cls is ErrorSchema:
             raise TypeError("ErrorSchema cannot be instantiated directly!")
         return super().__new__(cls)
 
     def to_dict(self):
         return self.model_dump()
     
-    class Config:
-        """Pydantic model configuration."""
-        extra = "forbid"  # Raise an error when extra fields are present.
-    
     @classmethod
     @restrict_arguments("type")
     def database_error(cls, **kwargs):
         """Factory method to create an instance for a database error."""
         defaults = {
             "type": "database_error",
             "msg": "Database operation failed.",
@@ -31,12 +30,11 @@
     
     @classmethod
     @restrict_arguments("type")
     def file_error(cls, **kwargs):
         """Factory method to create an instance for a file error."""
         defaults = {
             "type": "file_error",
-            "loc": ["request"],
             "msg": "File processing failed.",
         }
         defaults.update(kwargs)
         return cls(**defaults)
```

### Comparing `pyerrorschema-0.1.1b1/pyerrorschema/fastapi_error_schema.py` & `pyerrorschema-0.1.2/pyerrorschema/fastapi_error_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List, Dict
+from typing import Dict, List
+
 from pydantic import Field
 
 from .base_error_schema import ErrorSchema
 from .utils import restrict_arguments
 
 
 class FastAPIErrorSchema(ErrorSchema):
@@ -28,10 +29,21 @@
             "type": "value_error",
             "msg": "Value error.",
         }
         defaults.update(kwargs)
         return cls(**defaults)
     
     @classmethod
+    @restrict_arguments("type")
+    def docker_error(cls, **kwargs):
+        """Factory method to create an instance for a docker error."""
+        defaults = {
+            "type": "docker_error",
+            "msg": "Docker operation failed.",
+        }
+        defaults.update(kwargs)
+        return cls(**defaults)
+    
+    @classmethod
     def customized_error(cls, **kwargs):
         """Factory method to create an instance for a customized error."""
         return cls(**kwargs)
```

### Comparing `pyerrorschema-0.1.1b1/pyerrorschema/utils.py` & `pyerrorschema-0.1.2/pyerrorschema/utils.py`

 * *Files identical despite different names*

### Comparing `pyerrorschema-0.1.1b1/pyerrorschema.egg-info/PKG-INFO` & `pyerrorschema-0.1.2/pyerrorschema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrorschema
-Version: 0.1.1b1
+Version: 0.1.2
 Summary: Error schema validator
 Author-email: Elliot Su <sodinfeliz@google.com>
 License: Copyright (c) 2024, Elliot Su.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are
```

### Comparing `pyerrorschema-0.1.1b1/pyproject.toml` & `pyerrorschema-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyerrorschema"
-version = "0.1.1b1"
+version = "0.1.2"
 license = {file = "LICENSE.txt"}
 description = "Error schema validator"
 authors = [{name = "Elliot Su", email = "sodinfeliz@google.com"}]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     'License :: OSI Approved :: BSD License',
@@ -19,7 +19,17 @@
 ]
 dependencies = [
     "pydantic>=2.6.4"
 ]
 
 [project.urls]
 source = "https://github.com/sodinfeliz/PyErrorSchema"
+
+[tool.pytest.ini_options]
+addopts = "--cov=pyerrorschema"
+testpaths = [
+    "tests"
+]
+minversion = "6.0"
+
+[tool.isort]
+profile = "black"
```

