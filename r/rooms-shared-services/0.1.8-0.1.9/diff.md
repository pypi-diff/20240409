# Comparing `tmp/rooms_shared_services-0.1.8.tar.gz` & `tmp/rooms_shared_services-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rooms_shared_services-0.1.8.tar", max compression
+gzip compressed data, was "rooms_shared_services-0.1.9.tar", max compression
```

## Comparing `rooms_shared_services-0.1.8.tar` & `rooms_shared_services-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-01-10 20:24:32.715596 rooms_shared_services-0.1.8/LICENSE
--rw-r--r--   0        0        0      103 2024-01-10 19:47:32.069678 rooms_shared_services-0.1.8/README.md
--rw-r--r--   0        0        0     1636 2024-01-20 10:31:41.466890 rooms_shared_services-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       36 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/__init__.py
--rw-r--r--   0        0        0       19 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/src/__init__.py
--rw-r--r--   0        0        0     1442 2024-01-20 10:31:19.487043 rooms_shared_services-0.1.8/rooms_shared_services/src/fakers/fake.py
--rw-r--r--   0        0        0      584 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/src/main.py
--rw-r--r--   0        0        0       63 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/src/receivers/abstract.py
--rw-r--r--   0        0        0       23 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/src/storage/__init__.py
--rw-r--r--   0        0        0      998 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/src/storage/abstract.py
--rw-r--r--   0        0        0     3430 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.8/rooms_shared_services/src/storage/dynamodb.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 rooms_shared_services-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-10 20:24:32.715596 rooms_shared_services-0.1.9/LICENSE
+-rw-r--r--   0        0        0      103 2024-01-10 19:47:32.069678 rooms_shared_services-0.1.9/README.md
+-rw-r--r--   0        0        0     1636 2024-01-28 21:30:51.918545 rooms_shared_services-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.9/rooms_shared_services/__init__.py
+-rw-r--r--   0        0        0       19 2024-01-20 21:38:48.769936 rooms_shared_services-0.1.9/rooms_shared_services/src/__init__.py
+-rw-r--r--   0        0        0     1557 2024-01-28 21:27:41.767065 rooms_shared_services-0.1.9/rooms_shared_services/src/fakers/fake.py
+-rw-r--r--   0        0        0      584 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.9/rooms_shared_services/src/main.py
+-rw-r--r--   0        0        0       63 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.9/rooms_shared_services/src/receivers/abstract.py
+-rw-r--r--   0        0        0       23 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.9/rooms_shared_services/src/storage/__init__.py
+-rw-r--r--   0        0        0      998 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.9/rooms_shared_services/src/storage/abstract.py
+-rw-r--r--   0        0        0     3430 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.9/rooms_shared_services/src/storage/dynamodb.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 rooms_shared_services-0.1.9/PKG-INFO
```

### Comparing `rooms_shared_services-0.1.8/LICENSE` & `rooms_shared_services-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.8/pyproject.toml` & `rooms_shared_services-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [project.urls]
 Homepage = "https://github.com/kras55/rooms_shared_services"
 Issues = "https://github.com/kras55/rooms_shared_services/issues"
 
 
 [tool.poetry]
 name = "rooms_shared_services"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["kras55 <dkras5577@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.7"
 pydantic = "^2.5.2"
```

### Comparing `rooms_shared_services-0.1.8/rooms_shared_services/src/fakers/fake.py` & `rooms_shared_services-0.1.9/rooms_shared_services/src/fakers/fake.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Literal, TypeVar
+from typing import Any, Literal, TypeVar, get_args
+from random import choice
 
 from faker import Faker
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo
 from uuid import uuid4
 
 fake = Faker()
@@ -28,15 +29,17 @@
     name = field_info.annotation.__name__
     match name:
         case "str":
             return fake.pystr()
         case "int":
             return fake.pyint()
         case "UUID":
-            return uuid4()    
+            return uuid4()
+        case "Literal":
+            return choice(get_args(field_info.annotation))
         case _:
             raise ValueError("Invalid field annotation for generating fake value: {}".format(name))
 
 
 T = TypeVar("T", bound="BaseModel")
```

### Comparing `rooms_shared_services-0.1.8/rooms_shared_services/src/main.py` & `rooms_shared_services-0.1.9/rooms_shared_services/src/main.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.8/rooms_shared_services/src/storage/abstract.py` & `rooms_shared_services-0.1.9/rooms_shared_services/src/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.8/rooms_shared_services/src/storage/dynamodb.py` & `rooms_shared_services-0.1.9/rooms_shared_services/src/storage/dynamodb.py`

 * *Files identical despite different names*

