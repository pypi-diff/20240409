# Comparing `tmp/kydb-0.7.2.tar.gz` & `tmp/kydb-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kydb-0.7.2.tar", last modified: Mon Apr  8 05:08:19 2024, max compression
+gzip compressed data, was "kydb-0.7.5.tar", last modified: Tue Apr  9 07:40:28 2024, max compression
```

## Comparing `kydb-0.7.2.tar` & `kydb-0.7.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:08:19.321014 kydb-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 05:08:11.000000 kydb-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 05:08:19.321014 kydb-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 05:08:11.000000 kydb-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:08:19.321014 kydb-0.7.2/kydb/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/cache_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/dbobj.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/folder_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:08:19.321014 kydb-0.7.2/kydb/impl/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/http.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/https.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/impl/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/objdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-08 05:08:11.000000 kydb-0.7.2/kydb/union.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:08:19.321014 kydb-0.7.2/kydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 05:08:19.000000 kydb-0.7.2/kydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 05:08:19.000000 kydb-0.7.2/kydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:08:19.000000 kydb-0.7.2/kydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 05:08:19.000000 kydb-0.7.2/kydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 05:08:19.000000 kydb-0.7.2/kydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:08:19.321014 kydb-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-08 05:08:11.000000 kydb-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:40:28.163685 kydb-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 07:40:14.000000 kydb-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 07:40:28.163685 kydb-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 07:40:14.000000 kydb-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:40:28.159685 kydb-0.7.5/kydb/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/cache_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/dbobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/folder_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:40:28.163685 kydb-0.7.5/kydb/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/https.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/impl/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/objdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-09 07:40:14.000000 kydb-0.7.5/kydb/union.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:40:28.163685 kydb-0.7.5/kydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 07:40:28.000000 kydb-0.7.5/kydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 07:40:28.000000 kydb-0.7.5/kydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:40:28.000000 kydb-0.7.5/kydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 07:40:28.000000 kydb-0.7.5/kydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 07:40:28.000000 kydb-0.7.5/kydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:40:28.163685 kydb-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 07:40:14.000000 kydb-0.7.5/setup.py
```

### Comparing `kydb-0.7.2/LICENSE` & `kydb-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/PKG-INFO` & `kydb-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kydb
-Version: 0.7.2
+Version: 0.7.5
 Summary: kydb (Kinyu Database). NoSQL DB interface.
 Home-page: https://github.com/tayglobal/kydb
 Author: Tony Yum
 Author-email: tony.yum@tayglobal.com
 License: MIT
 Keywords: NoSQL,Database,DB
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kydb-0.7.2/README.md` & `kydb-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/api.py` & `kydb-0.7.5/kydb/api.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/base.py` & `kydb-0.7.5/kydb/base.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/cache.py` & `kydb-0.7.5/kydb/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .base import BaseDB
 from .interface import KYDBInterface
 from contextlib import ExitStack
 from .objdb import ObjDBMixin, DBOBJ_CONFIG_PATH
 from .dbobj import DbObj
+import pickle
 
 
 class CacheDB(KYDBInterface, ObjDBMixin):
     """CacheDB
     """
 
     def __init__(self, cache_db: BaseDB, persist_db: BaseDB):
@@ -105,14 +106,21 @@
         def _ensure_db(obj):
             if isinstance(obj, DbObj):
                 obj.db = self
 
             return obj
 
         if self.cache_db.exists(key):
+            raw_data = self.cache_db.get_raw(key)
+
+            data = pickle.loads(raw_data)
+            if self.is_data_dbobj(data):
+                m = data['meta']
+                return self.db_obj_new(m['class_name'], m['key'], data['data'])
+
             return _ensure_db(self.cache_db[key])
 
         item = _ensure_db(self.persist_db[key])
         self.cache_db[key] = item
 
         return item
```

### Comparing `kydb-0.7.2/kydb/dbobj.py` & `kydb-0.7.5/kydb/dbobj.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/folder_meta.py` & `kydb-0.7.5/kydb/folder_meta.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/impl/dynamodb.py` & `kydb-0.7.5/kydb/impl/dynamodb.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/impl/files.py` & `kydb-0.7.5/kydb/impl/files.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/impl/http.py` & `kydb-0.7.5/kydb/impl/http.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/impl/memory.py` & `kydb-0.7.5/kydb/impl/memory.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/impl/redis.py` & `kydb-0.7.5/kydb/impl/redis.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/impl/s3.py` & `kydb-0.7.5/kydb/impl/s3.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/interface.py` & `kydb-0.7.5/kydb/interface.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/objdb.py` & `kydb-0.7.5/kydb/objdb.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb/union.py` & `kydb-0.7.5/kydb/union.py`

 * *Files identical despite different names*

### Comparing `kydb-0.7.2/kydb.egg-info/PKG-INFO` & `kydb-0.7.5/kydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kydb
-Version: 0.7.2
+Version: 0.7.5
 Summary: kydb (Kinyu Database). NoSQL DB interface.
 Home-page: https://github.com/tayglobal/kydb
 Author: Tony Yum
 Author-email: tony.yum@tayglobal.com
 License: MIT
 Keywords: NoSQL,Database,DB
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kydb-0.7.2/setup.py` & `kydb-0.7.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='kydb',
     packages=['kydb', 'kydb.impl'],
-    version='0.7.2',
+    version='0.7.5',
     license='MIT',
     description='kydb (Kinyu Database). NoSQL DB interface.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Tony Yum',
     author_email='tony.yum@tayglobal.com',
     url='https://github.com/tayglobal/kydb',
```

