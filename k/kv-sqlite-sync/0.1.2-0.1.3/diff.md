# Comparing `tmp/kv-sqlite-sync-0.1.2.tar.gz` & `tmp/kv-sqlite-sync-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-sqlite-sync-0.1.2.tar", last modified: Fri Apr  5 13:32:13 2024, max compression
+gzip compressed data, was "kv-sqlite-sync-0.1.3.tar", last modified: Tue Apr  9 04:44:47 2024, max compression
```

## Comparing `kv-sqlite-sync-0.1.2.tar` & `kv-sqlite-sync-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.260846 kv-sqlite-sync-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-05 13:32:13.260846 kv-sqlite-sync-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-05 13:15:45.000000 kv-sqlite-sync-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      676 2024-04-05 13:32:11.000000 kv-sqlite-sync-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 13:32:13.260846 kv-sqlite-sync-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.250846 kv-sqlite-sync-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.250846 kv-sqlite-sync-0.1.2/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.250846 kv-sqlite-sync-0.1.2/src/kv/sqlite/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.2/src/kv/sqlite/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.250846 kv-sqlite-sync-0.1.2/src/kv/sqlite/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.2/src/kv/sqlite/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3297 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.2/src/kv/sqlite/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.250846 kv-sqlite-sync-0.1.2/src/kv/sqlite/queries/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.2/src/kv/sqlite/queries/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1546 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.2/src/kv/sqlite/queries/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:13.260846 kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-05 13:32:13.000000 kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-05 13:32:13.000000 kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 13:32:13.000000 kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-05 13:32:13.000000 kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-05 13:32:13.000000 kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-05 13:15:45.000000 kv-sqlite-sync-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      676 2024-04-09 04:44:45.000000 kv-sqlite-sync-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/src/kv/sqlite/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.3/src/kv/sqlite/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/src/kv/sqlite/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.3/src/kv/sqlite/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3305 2024-04-09 04:44:29.000000 kv-sqlite-sync-0.1.3/src/kv/sqlite/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/src/kv/sqlite/queries/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.3/src/kv/sqlite/queries/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1546 2024-04-05 13:12:45.000000 kv-sqlite-sync-0.1.3/src/kv/sqlite/queries/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:47.945027 kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      875 2024-04-09 04:44:47.000000 kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-09 04:44:47.000000 kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 04:44:47.000000 kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-09 04:44:47.000000 kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-09 04:44:47.000000 kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/top_level.txt
```

### Comparing `kv-sqlite-sync-0.1.2/PKG-INFO` & `kv-sqlite-sync-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.2
+Version: 0.1.3
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv-sqlite-sync-0.1.2/src/kv/sqlite/api/api.py` & `kv-sqlite-sync-0.1.3/src/kv/sqlite/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       self.conn.commit()
       return Right(cur)
     except sqlite3.Error as err:
       return Left(DBError(str(err)))
 
   def update(self, key: str, value: T) -> Either[DBError | InexistentItem, None]:
     return self.execute(queries.update(key, self.dump(value), table=self.table)) \
-      & (lambda cur: Left(InexistentItem(key)) if cur.rowcount == 0 else Right())
+      & (lambda cur: Left(InexistentItem(key)) if cur.rowcount == 0 else Right(None))
   
   def insert(self, key: str, value: T, *, replace = False) -> Either[DBError, None]:
     make_query = queries.upsert if replace else queries.insert
     return self.execute(make_query(key, self.dump(value), table=self.table)) | (lambda _: None)
   
   def read(self, key: str) -> Either[DBError | InvalidData | InexistentItem, T]:
     res = self.execute(queries.read(key, table=self.table)) \
@@ -57,15 +57,15 @@
       case Right(bad_data):
         return Left(InvalidData(detail=f'Found invalid row: {bad_data}'))
       case err:
         return err
 
   def delete(self, key: str) -> Either[DBError | InexistentItem, None]:
     return self.execute(queries.delete(key, table=self.table)) \
-      & (lambda cur: Left(InexistentItem(key)) if cur.rowcount == 0 else Right())
+      & (lambda cur: Left(InexistentItem(key)) if cur.rowcount == 0 else Right(None))
   
   def keys(self, batch_size: int | None = None) -> Iterable[Either[DBError, str]]:
     match self.execute(queries.keys(self.table)):
       case Right(cur):
         while (batch := cur.fetchmany(batch_size or 256)) != []:
           for [key] in batch:
             yield Right(key)
```

### Comparing `kv-sqlite-sync-0.1.2/src/kv/sqlite/queries/queries.py` & `kv-sqlite-sync-0.1.3/src/kv/sqlite/queries/queries.py`

 * *Files identical despite different names*

### Comparing `kv-sqlite-sync-0.1.2/src/kv_sqlite_sync.egg-info/PKG-INFO` & `kv-sqlite-sync-0.1.3/src/kv_sqlite_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.2
+Version: 0.1.3
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

