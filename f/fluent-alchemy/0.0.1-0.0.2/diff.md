# Comparing `tmp/fluent_alchemy-0.0.1.tar.gz` & `tmp/fluent_alchemy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluent_alchemy-0.0.1.tar", max compression
+gzip compressed data, was "fluent_alchemy-0.0.2.tar", max compression
```

## Comparing `fluent_alchemy-0.0.1.tar` & `fluent_alchemy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0     1087 2024-03-28 05:47:01.755137 fluent_alchemy-0.0.1/LICENSE
--rw-r--r--   0        0        0     4940 2024-03-28 06:01:00.613111 fluent_alchemy-0.0.1/README.md
--rw-r--r--   0        0        0      211 2024-03-27 08:30:43.439063 fluent_alchemy-0.0.1/fluent_alchemy/__init__.py
--rw-r--r--   0        0        0     2211 2024-03-27 06:50:03.119053 fluent_alchemy-0.0.1/fluent_alchemy/activerecord.py
--rw-r--r--   0        0        0     5061 2024-03-27 05:49:28.350045 fluent_alchemy-0.0.1/fluent_alchemy/builder.py
--rw-r--r--   0        0        0        0 2024-03-18 07:03:20.368595 fluent_alchemy-0.0.1/fluent_alchemy/mixins/__init__.py
--rw-r--r--   0        0        0      400 2024-03-20 10:35:03.478043 fluent_alchemy-0.0.1/fluent_alchemy/mixins/softdelete.py
--rw-r--r--   0        0        0      386 2024-03-18 07:03:20.368894 fluent_alchemy-0.0.1/fluent_alchemy/mixins/timestamp.py
--rw-r--r--   0        0        0      157 2024-03-20 10:35:03.478476 fluent_alchemy-0.0.1/fluent_alchemy/scopes/__init__.py
--rw-r--r--   0        0        0      700 2024-03-20 10:50:46.259853 fluent_alchemy-0.0.1/fluent_alchemy/scopes/softdelete.py
--rw-r--r--   0        0        0      536 2024-03-26 06:18:17.306940 fluent_alchemy-0.0.1/fluent_alchemy/session.py
--rw-r--r--   0        0        0      783 2024-03-28 02:45:14.034790 fluent_alchemy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 fluent_alchemy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-03-28 05:47:01.755137 fluent_alchemy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4940 2024-03-28 06:01:00.613111 fluent_alchemy-0.0.2/README.md
+-rw-r--r--   0        0        0      211 2024-03-27 08:30:43.439063 fluent_alchemy-0.0.2/fluent_alchemy/__init__.py
+-rw-r--r--   0        0        0     2680 2024-04-09 07:23:26.222350 fluent_alchemy-0.0.2/fluent_alchemy/activerecord.py
+-rw-r--r--   0        0        0       47 2024-04-01 09:44:04.020795 fluent_alchemy-0.0.2/fluent_alchemy/builders/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-09 07:23:26.222764 fluent_alchemy-0.0.2/fluent_alchemy/builders/base.py
+-rw-r--r--   0        0        0      806 2024-04-08 06:30:29.754513 fluent_alchemy-0.0.2/fluent_alchemy/builders/delete.py
+-rw-r--r--   0        0        0      770 2024-04-09 07:23:26.223034 fluent_alchemy-0.0.2/fluent_alchemy/builders/insert.py
+-rw-r--r--   0        0        0      173 2024-04-09 07:23:26.223354 fluent_alchemy-0.0.2/fluent_alchemy/builders/query.py
+-rw-r--r--   0        0        0     2493 2024-04-08 06:30:29.754806 fluent_alchemy-0.0.2/fluent_alchemy/builders/select.py
+-rw-r--r--   0        0        0        0 2024-03-18 07:03:20.368595 fluent_alchemy-0.0.2/fluent_alchemy/mixins/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-08 06:30:29.755260 fluent_alchemy-0.0.2/fluent_alchemy/mixins/softdelete.py
+-rw-r--r--   0        0        0      386 2024-03-18 07:03:20.368894 fluent_alchemy-0.0.2/fluent_alchemy/mixins/timestamp.py
+-rw-r--r--   0        0        0      157 2024-03-20 10:35:03.478476 fluent_alchemy-0.0.2/fluent_alchemy/scopes/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-08 06:30:29.755625 fluent_alchemy-0.0.2/fluent_alchemy/scopes/softdelete.py
+-rw-r--r--   0        0        0      536 2024-03-26 06:18:17.306940 fluent_alchemy-0.0.2/fluent_alchemy/session.py
+-rw-r--r--   0        0        0      783 2024-04-09 07:33:45.019092 fluent_alchemy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 fluent_alchemy-0.0.2/PKG-INFO
```

### Comparing `fluent_alchemy-0.0.1/LICENSE` & `fluent_alchemy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fluent_alchemy-0.0.1/README.md` & `fluent_alchemy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fluent_alchemy-0.0.1/fluent_alchemy/activerecord.py` & `fluent_alchemy-0.0.2/fluent_alchemy/activerecord.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Sequence
+from typing import Sequence, Optional
 
 from .session import ScopedSessionHandler
-from .builder import QueryBuilder
+from .builders.query import QueryBuilder
 
 
 class ActiveRecord(ScopedSessionHandler):
     @classmethod
     def select(cls, *entities):
         return cls()._new_query().select(*entities)
 
@@ -51,23 +51,40 @@
     def create(cls, **attributes):
         instance = cls(**attributes)
 
         instance.save()
 
         return instance
 
-    def _new_query(self) -> "QueryBuilder":
+    @classmethod
+    def insert(
+        cls,
+        values: list[dict],
+        returning: Optional[list] = None,
+        execution_options: Optional[dict] = None,
+    ):
+        builder = cls()._new_query()
+
+        if returning:
+            builder.returning(*returning)
+
+        if execution_options:
+            builder.execution_options(**execution_options)
+
+        return builder.insert(values)
+
+    def _new_query(self) -> QueryBuilder:
         scopes = {}
 
         for base in self.__class__.__bases__:
             if hasattr(base, "scope_registry"):
                 scope = base.scope_registry()
                 scopes[scope.__class__] = scope
 
-        return QueryBuilder(self._session, self, scopes)
+        return QueryBuilder(self._session, self).apply_scopes(scopes)
 
     def save(self, refresh: bool = True):
         try:
             self._session.add(self)
             self._session.commit()
 
             if refresh:
@@ -75,12 +92,12 @@
 
         except Exception as e:
             self._session.rollback()
             raise e
 
     def delete(self, force: bool = False):
         try:
-            self._new_query().delete(force)
+            self._new_query().where(self.__class__.id == self.id).delete(force)
 
         except Exception as e:
             self._session.rollback()
             raise e
```

### Comparing `fluent_alchemy-0.0.1/fluent_alchemy/session.py` & `fluent_alchemy-0.0.2/fluent_alchemy/session.py`

 * *Files identical despite different names*

### Comparing `fluent_alchemy-0.0.1/pyproject.toml` & `fluent_alchemy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluent-alchemy"
-version = "0.0.1"
+version = "0.0.2"
 description = "Use SQLAlchemy fluently"
 authors = ["Sam Yao <turisesonia@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["sqlalchemy", "SQLAlchemy", "activerecord", "Active Record"]
 repository = "https://github.com/turisesonia/fluent-alchemy"
 homepage = "https://github.com/turisesonia/fluent-alchemy"
```

### Comparing `fluent_alchemy-0.0.1/PKG-INFO` & `fluent_alchemy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluent-alchemy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Use SQLAlchemy fluently
 Home-page: https://github.com/turisesonia/fluent-alchemy
 License: MIT
 Keywords: sqlalchemy,SQLAlchemy,activerecord,Active Record
 Author: Sam Yao
 Author-email: turisesonia@gmail.com
 Requires-Python: >=3.8,<4.0
```

