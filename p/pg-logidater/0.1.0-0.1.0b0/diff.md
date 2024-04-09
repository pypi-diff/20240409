# Comparing `tmp/pg_logidater-0.1.0.tar.gz` & `tmp/pg_logidater-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_logidater-0.1.0.tar", max compression
+gzip compressed data, was "pg_logidater-0.1.0b0.tar", max compression
```

## Comparing `pg_logidater-0.1.0.tar` & `pg_logidater-0.1.0b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.1.0/LICENSE
--rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.1.0/pg_logidater/__init__.py
--rw-r--r--   0        0        0     9157 2024-04-09 06:45:57.036391 pg_logidater-0.1.0/pg_logidater/cli.py
--rw-r--r--   0        0        0     1241 2024-04-09 06:45:57.036788 pg_logidater-0.1.0/pg_logidater/exceptions.py
--rw-r--r--   0        0        0     1519 2024-04-04 09:09:12.988223 pg_logidater-0.1.0/pg_logidater/master.py
--rw-r--r--   0        0        0     1659 2024-04-09 06:46:37.067914 pg_logidater-0.1.0/pg_logidater/replica.py
--rw-r--r--   0        0        0     2285 2024-04-09 06:45:57.037449 pg_logidater-0.1.0/pg_logidater/sqlqueries.py
--rw-r--r--   0        0        0     5011 2024-04-05 18:43:10.841757 pg_logidater-0.1.0/pg_logidater/tartget.py
--rw-r--r--   0        0        0     8883 2024-04-09 06:45:57.037726 pg_logidater-0.1.0/pg_logidater/utils.py
--rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pg_logidater-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.1.0b0/LICENSE
+-rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.1.0b0/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.1.0b0/pg_logidater/__init__.py
+-rw-r--r--   0        0        0     9131 2024-04-05 18:40:28.872527 pg_logidater-0.1.0b0/pg_logidater/cli.py
+-rw-r--r--   0        0        0     1059 2024-03-31 04:40:04.882765 pg_logidater-0.1.0b0/pg_logidater/exceptions.py
+-rw-r--r--   0        0        0     1519 2024-04-04 09:09:12.988223 pg_logidater-0.1.0b0/pg_logidater/master.py
+-rw-r--r--   0        0        0     1454 2024-04-04 09:16:11.717639 pg_logidater-0.1.0b0/pg_logidater/replica.py
+-rw-r--r--   0        0        0     2242 2024-04-04 11:34:45.892987 pg_logidater-0.1.0b0/pg_logidater/sqlqueries.py
+-rw-r--r--   0        0        0     5011 2024-04-05 18:43:10.841757 pg_logidater-0.1.0b0/pg_logidater/tartget.py
+-rw-r--r--   0        0        0     8770 2024-04-05 18:39:36.832184 pg_logidater-0.1.0b0/pg_logidater/utils.py
+-rw-r--r--   0        0        0      853 2024-04-05 19:35:20.054169 pg_logidater-0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 pg_logidater-0.1.0b0/PKG-INFO
```

### Comparing `pg_logidater-0.1.0/LICENSE` & `pg_logidater-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0/README.md` & `pg_logidater-0.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0/pg_logidater/cli.py` & `pg_logidater-0.1.0b0/pg_logidater/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,16 +170,15 @@
         database=args["database"],
         owner=db_owner
     )
     pause_replica(
         psql=replica_sql
     )
     app_name, slot_name = replica_info(
-        host=args["replica_host"],
-        psql=replica_sql
+        host=args["replica_host"]
     )
     replica_stop_position = get_replica_position(
         psql=master_sql,
         app_name=app_name
     )
     sync_roles(
         host=args["replica_host"],
```

### Comparing `pg_logidater-0.1.0/pg_logidater/exceptions.py` & `pg_logidater-0.1.0b0/pg_logidater/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,7 @@
 
 
 class PublicationExists(Exception):
     def __init__(self, message=None):
         if not message:
             message = "Publication exists"
         super().__init__(message)
-
-
-class VersionNotSupported(Exception):
-    def __init__(self, message=None):
-        if not message:
-            message = "Version not supported"
-        super().__init__(message)
```

### Comparing `pg_logidater-0.1.0/pg_logidater/master.py` & `pg_logidater-0.1.0b0/pg_logidater/master.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0/pg_logidater/sqlqueries.py` & `pg_logidater-0.1.0b0/pg_logidater/sqlqueries.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 SQL_SET_SLOT_NAME = "ALTER SUBSCRIPTION {name} SET (slot_name={slot_name})"
 SQL_DISABLE_SUBSCRIPTION = "ALTER SUBSCRIPTION {name} DISABLE"
 SQL_GET_DB_SUBSCRIPTION = "SELECT subname FROM pg_subscription"
 SQL_CREATE_REPL_LOGICAL_SLOT = "SELECT pg_create_logical_replication_slot('{0}', 'pgoutput')"
 SQL_DROP_REPL_SLOT = "SELECT pg_drop_replication_slot('{0}')"
 SQL_CREAATE_PUB = "CREATE publication {0} for all tables"
 SQL_DROP_PUB = "DROP publication {0}"
-SQL_DATA_DIRECTORY = "SHOW data_directory"
 
 SQL_SELECT_ALL_SEQUENCES = """
 SELECT
   sequence_schema,
   sequence_name
 FROM
   information_schema.sequences
```

### Comparing `pg_logidater-0.1.0/pg_logidater/tartget.py` & `pg_logidater-0.1.0b0/pg_logidater/tartget.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0/pg_logidater/utils.py` & `pg_logidater-0.1.0b0/pg_logidater/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,17 +196,14 @@
         if self.query(sql.SQL_CHECK_PUBLICATION.format(name), fetchone=True):
             return True
         return False
 
     def get_sequences(self) -> list[tuple]:
         return self.query(sql.SQL_SELECT_ALL_SEQUENCES, fetchall=True)
 
-    def get_datadirectory(self) -> float:
-        return (self.query(sql.SQL_DATA_DIRECTORY, fetchone=True))[0]
-
 
 def setup_logging(log_level: str, save_log: str, debug_ssh: bool = False,  log_path: str = None) -> None:
     log_level_int = logging.getLevelName(str(log_level).upper())
     handlers = []
     if debug_ssh:
         logging.getLogger("paramiko").setLevel(logging.DEBUG)
     else:
```

### Comparing `pg_logidater-0.1.0/pyproject.toml` & `pg_logidater-0.1.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.1.0/PKG-INFO` & `pg_logidater-0.1.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-logidater
-Version: 0.1.0
+Version: 0.1.0b0
 Summary: Postgresql logical replication setup utility
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Keywords: postgres
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
```

