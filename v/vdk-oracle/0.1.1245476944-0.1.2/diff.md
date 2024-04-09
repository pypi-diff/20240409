# Comparing `tmp/vdk-oracle-0.1.1245476944.tar.gz` & `tmp/vdk-oracle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-oracle-0.1.1245476944.tar", last modified: Tue Apr  9 09:18:33 2024, max compression
+gzip compressed data, was "vdk-oracle-0.1.2.tar", last modified: Tue Jan 16 23:54:31 2024, max compression
```

## Comparing `vdk-oracle-0.1.1245476944.tar` & `vdk-oracle-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.108325 vdk-oracle-0.1.1245476944/
--rw-r--r--   0 root         (0) root         (0)     8181 2024-04-09 09:18:33.104325 vdk-oracle-0.1.1245476944/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7172 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 09:18:33.108325 vdk-oracle-0.1.1245476944/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-09 09:18:22.000000 vdk-oracle-0.1.1245476944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.096325 vdk-oracle-0.1.1245476944/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.096325 vdk-oracle-0.1.1245476944/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.096325 vdk-oracle-0.1.1245476944/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.104325 vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/
--rw-rw-rw-   0 root         (0) root         (0)     9726 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/ingest_to_oracle.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/oracle_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/oracle_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/oracle_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.104325 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8181 2024-04-09 09:18:33.000000 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-09 09:18:33.000000 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:18:33.000000 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-09 09:18:33.000000 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-09 09:18:33.000000 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-09 09:18:33.000000 vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:18:33.104325 vdk-oracle-0.1.1245476944/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13599 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/tests/test_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5228 2024-04-09 09:18:12.000000 vdk-oracle-0.1.1245476944/tests/test_secrets_config.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.982146 vdk-oracle-0.1.2/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7363 2024-01-16 23:54:31.979875 vdk-oracle-0.1.2/PKG-INFO
+-rw-r--r--   0 aivanov    (502) staff       (20)     6414 2024-01-16 16:15:12.000000 vdk-oracle-0.1.2/README.md
+-rw-r--r--   0 aivanov    (502) staff       (20)       38 2024-01-16 23:54:31.982451 vdk-oracle-0.1.2/setup.cfg
+-rw-r--r--   0 aivanov    (502) staff       (20)     1646 2024-01-16 23:54:23.000000 vdk-oracle-0.1.2/setup.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.957032 vdk-oracle-0.1.2/src/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.955869 vdk-oracle-0.1.2/src/vdk/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.956330 vdk-oracle-0.1.2/src/vdk/plugin/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.965605 vdk-oracle-0.1.2/src/vdk/plugin/oracle/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7702 2024-01-09 13:57:58.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/ingest_to_oracle.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     4340 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_configuration.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     3168 2024-01-16 17:02:10.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_connection.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     4029 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_plugin.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.976413 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7363 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 aivanov    (502) staff       (20)      468 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)        1 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)       62 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)       27 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/requires.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)        4 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.974616 vdk-oracle-0.1.2/tests/
+-rw-r--r--   0 aivanov    (502) staff       (20)     8319 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/tests/test_plugin.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     5232 2024-01-09 13:57:58.000000 vdk-oracle-0.1.2/tests/test_secrets_config.py
```

### Comparing `vdk-oracle-0.1.1245476944/PKG-INFO` & `vdk-oracle-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: vdk-oracle
-Version: 0.1.1245476944
+Version: 0.1.2
 Summary: Support for VDK Managed Oracle connection
 Home-page: https://github.com/vmware/versatile-data-kit
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
 Project-URL: Source Code, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues/new/choose
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: vdk-core
 Requires-Dist: oracledb
 Requires-Dist: tabulate
 
 # oracle
 
-<a href="https://pypistats.org/packages/vdk-oracle" alt="Monthly Downloads">
-        <img src="https://img.shields.io/pypi/dm/vdk-oracle.svg" alt="monthly download count for vdk-oracle"></a>
-
 Support for VDK Managed Oracle connection
 
 TODO: what the project is about, what is its purpose
 
 
 ## Usage
 
@@ -44,17 +40,15 @@
 | oracle_user              | Username used when connecting to Oracle database                                                                                                                                                                                      | my_user             |
 | oracle_password          | Password used when connecting to Oracle database                                                                                                                                                                                      | super_secret_shhhh  |
 | oracle_use_secrets       | Set to True to use secrets to connect to Oracle                                                                                                                                                                                       | True                |
 | oracle_connection_string | The Oracle connection string                                                                                                                                                                                                          | localhost:1521/free |
 | oracle_host              | The host of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | localhost           |
 | oracle_port              | The port of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | 1521                |
 | oracle_sid               | The SID of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                        | free                |
-| oracle_service_name      | The Service name of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                               | free                |
 | oracle_thick_mode        | Python-oracledb is said to be in Thick mode when Oracle Client libraries are used. True by default. Set to False to disable Oracle Thick mode. More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html | True                |
-| oracle_ingest_batch_size | vdk-oracle splits ingestion payloads into batches. Change this config to control the batch size. Default is set to 100.                                                                                                               | 100                 |
 
 ### Example
 
 #### CLI Queries
 
 ```sh
 export VDK_ORACLE_USER=my_username
```

### Comparing `vdk-oracle-0.1.1245476944/README.md` & `vdk-oracle-0.1.2/src/vdk_oracle.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,28 @@
-# oracle
+Metadata-Version: 2.1
+Name: vdk-oracle
+Version: 0.1.2
+Summary: Support for VDK Managed Oracle connection
+Home-page: https://github.com/vmware/versatile-data-kit
+Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
+Project-URL: Source Code, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
+Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues/new/choose
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Requires-Dist: vdk-core
+Requires-Dist: oracledb
+Requires-Dist: tabulate
 
-<a href="https://pypistats.org/packages/vdk-oracle" alt="Monthly Downloads">
-        <img src="https://img.shields.io/pypi/dm/vdk-oracle.svg" alt="monthly download count for vdk-oracle"></a>
+# oracle
 
 Support for VDK Managed Oracle connection
 
 TODO: what the project is about, what is its purpose
 
 
 ## Usage
@@ -23,17 +40,15 @@
 | oracle_user              | Username used when connecting to Oracle database                                                                                                                                                                                      | my_user             |
 | oracle_password          | Password used when connecting to Oracle database                                                                                                                                                                                      | super_secret_shhhh  |
 | oracle_use_secrets       | Set to True to use secrets to connect to Oracle                                                                                                                                                                                       | True                |
 | oracle_connection_string | The Oracle connection string                                                                                                                                                                                                          | localhost:1521/free |
 | oracle_host              | The host of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | localhost           |
 | oracle_port              | The port of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | 1521                |
 | oracle_sid               | The SID of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                        | free                |
-| oracle_service_name      | The Service name of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                               | free                |
 | oracle_thick_mode        | Python-oracledb is said to be in Thick mode when Oracle Client libraries are used. True by default. Set to False to disable Oracle Thick mode. More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html | True                |
-| oracle_ingest_batch_size | vdk-oracle splits ingestion payloads into batches. Change this config to control the batch size. Default is set to 100.                                                                                                               | 100                 |
 
 ### Example
 
 #### CLI Queries
 
 ```sh
 export VDK_ORACLE_USER=my_username
```

### Comparing `vdk-oracle-0.1.1245476944/setup.py` & `vdk-oracle-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.1245476944"
+__version__ = "0.1.2"
 
 setuptools.setup(
     name="vdk-oracle",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Support for VDK Managed Oracle connection",
     long_description=pathlib.Path("README.md").read_text(),
@@ -27,15 +27,14 @@
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
     ],
     project_urls={
         "Documentation": "https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle",
         "Source Code": "https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle",
         "Bug Tracker": "https://github.com/vmware/versatile-data-kit/issues/new/choose",
     },
 )
```

### Comparing `vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/ingest_to_oracle.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/ingest_to_oracle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,259 +1,193 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import datetime
 import logging
 import math
-import re
 from decimal import Decimal
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Set
 
 from vdk.api.plugin.plugin_input import PEP249Connection
 from vdk.internal.builtin_plugins.connection.impl.router import ManagedConnectionRouter
 from vdk.internal.builtin_plugins.connection.managed_cursor import ManagedCursor
 from vdk.internal.builtin_plugins.ingestion.ingester_base import IIngesterPlugin
 
 log = logging.getLogger(__name__)
 
 
-# Functions for escaping special characters
-def _is_plain_identifier(identifier: str) -> bool:
-    # https://docs.oracle.com/en/error-help/db/ora-00904/
-    # Alphanumeric that doesn't start with a number
-    # Can contain and start with $, # and _
-    regex = "^[A-Za-z\\$#_][0-9A-Za-z\\$#_]*$"
-    return bool(re.fullmatch(regex, identifier))
-
-
-def _normalize_identifier(identifier: str) -> str:
-    return identifier.upper() if _is_plain_identifier(identifier) else identifier
-
-
-def _escape_special_chars(value: str) -> str:
-    return value if _is_plain_identifier(value) else f'"{value}"'
-
-
-class TableCache:
-    def __init__(self, cursor: ManagedCursor):
-        self._tables: Dict[str, Dict[str, str]] = {}
-        self._cursor = cursor
-
-    def cache_columns(self, table: str) -> None:
-        # exit if the table columns have already been cached
-        if table.upper() in self._tables and self._tables[table.upper()]:
-            return
-        try:
-            self._cursor.execute(
-                f"SELECT column_name, data_type, data_scale FROM user_tab_columns WHERE table_name = '{table.upper()}'"
-            )
-            result = self._cursor.fetchall()
-            self._tables[table.upper()] = {
-                col: ("DECIMAL" if data_type == "NUMBER" and data_scale else data_type)
-                for (col, data_type, data_scale) in result
-            }
-        except Exception as e:
-            # TODO: https://github.com/vmware/versatile-data-kit/issues/2932
-            log.exception(
-                "An error occurred while trying to cache columns. Ignoring for now.", e
-            )
-
-    def get_columns(self, table: str) -> Dict[str, str]:
-        return self._tables[table.upper()]
-
-    def update_from_col_defs(self, table: str, col_defs) -> None:
-        self._tables[table.upper()].update(col_defs)
-
-    def get_col_type(self, table: str, col: str) -> str:
-        return self._tables.get(table.upper()).get(
-            col.upper() if _is_plain_identifier(col) else col
-        )
-
-    def table_exists(self, table: str) -> bool:
-        if table.upper() in self._tables:
-            return True
-
-        self._cursor.execute(
-            f"SELECT COUNT(*) FROM user_tables WHERE table_name = :1",
-            [table.upper()],
-        )
-        exists = bool(self._cursor.fetchone()[0])
-
-        if exists:
-            self._tables[table.upper()] = {}
-
-        return exists
-
-
 class IngestToOracle(IIngesterPlugin):
-    def __init__(
-        self, connections: ManagedConnectionRouter, ingest_batch_size: int = 100
-    ):
+    def __init__(self, connections: ManagedConnectionRouter):
         self.conn: PEP249Connection = connections.open_connection("ORACLE").connect()
         self.cursor: ManagedCursor = self.conn.cursor()
-        self.table_cache: TableCache = TableCache(self.cursor)  # New cache for columns
-        self.ingest_batch_size = ingest_batch_size
+        self.table_cache: Set[str] = set()  # Cache to store existing tables
+        self.column_cache: Dict[str, Dict[str, str]] = {}  # New cache for columns
 
     @staticmethod
     def _get_oracle_type(value: Any) -> str:
         type_mappings = {
             int: "NUMBER",
             float: "FLOAT",
             Decimal: "DECIMAL(14, 8)",
             str: "VARCHAR2(255)",
             datetime.datetime: "TIMESTAMP",
             bool: "NUMBER(1)",
             bytes: "BLOB",
         }
         return type_mappings.get(type(value), "VARCHAR2(255)")
 
+    def _table_exists(self, table_name: str) -> bool:
+        if table_name.upper() in self.table_cache:
+            return True
+
+        self.cursor.execute(
+            f"SELECT COUNT(*) FROM user_tables WHERE table_name = :1",
+            [table_name.upper()],
+        )
+        exists = bool(self.cursor.fetchone()[0])
+
+        if exists:
+            self.table_cache.add(table_name.upper())
+
+        return exists
+
     def _create_table(self, table_name: str, row: Dict[str, Any]) -> None:
-        column_defs = [
-            f"{_escape_special_chars(col)} {self._get_oracle_type(row[col])}"
-            for col in row.keys()
-        ]
+        column_defs = [f"{col} {self._get_oracle_type(row[col])}" for col in row.keys()]
         create_table_sql = (
             f"CREATE TABLE {table_name.upper()} ({', '.join(column_defs)})"
         )
         self.cursor.execute(create_table_sql)
 
+    def _cache_columns(self, table_name: str) -> None:
+        try:
+            self.cursor.execute(
+                f"SELECT column_name, data_type, data_scale FROM user_tab_columns WHERE table_name = '{table_name.upper()}'"
+            )
+            result = self.cursor.fetchall()
+            self.column_cache[table_name.upper()] = {
+                col: ("DECIMAL" if data_type == "NUMBER" and data_scale else data_type)
+                for (col, data_type, data_scale) in result
+            }
+        except Exception as e:
+            # TODO: https://github.com/vmware/versatile-data-kit/issues/2932
+            log.error(
+                "An exception occurred while trying to cache columns. Ignoring for now."
+            )
+            log.exception(e)
+
     def _add_columns(self, table_name: str, payload: List[Dict[str, Any]]) -> None:
-        self.table_cache.cache_columns(table_name)
-        existing_columns = self.table_cache.get_columns(table_name)
+        if table_name.upper() not in self.column_cache:
+            self._cache_columns(table_name)
+
+        existing_columns = self.column_cache[table_name.upper()]
 
         # Find unique new columns from all rows in the payload
-        all_columns = {
-            _normalize_identifier(col) for row in payload for col in row.keys()
-        }
+        all_columns = {col.upper() for row in payload for col in row.keys()}
         new_columns = all_columns - existing_columns.keys()
         column_defs = []
         if new_columns:
             for col in new_columns:
                 sample_value = next(
                     (row[col] for row in payload if row.get(col) is not None), None
                 )
                 column_type = (
                     self._get_oracle_type(sample_value)
                     if sample_value is not None
                     else "VARCHAR2(255)"
                 )
                 column_defs.append((col, column_type))
 
-            string_defs = [
-                f"{_escape_special_chars(col_def[0])} {col_def[1]}"
-                for col_def in column_defs
-            ]
+            string_defs = [f"{col_def[0]} {col_def[1]}" for col_def in column_defs]
             alter_sql = (
                 f"ALTER TABLE {table_name.upper()} ADD ({', '.join(string_defs)})"
             )
             self.cursor.execute(alter_sql)
-            self.table_cache.update_from_col_defs(table_name, column_defs)
+            self.column_cache[table_name.upper()].update(column_defs)
 
     # TODO: https://github.com/vmware/versatile-data-kit/issues/2929
     # TODO: https://github.com/vmware/versatile-data-kit/issues/2930
     def _cast_to_correct_type(self, table: str, column: str, value: Any) -> Any:
-        if isinstance(value, float) and math.isnan(value):
-            return None
-
         def cast_string_to_type(db_type: str, payload_value: str) -> Any:
             if db_type == "FLOAT" or db_type == "DECIMAL":
                 return float(payload_value)
             if db_type == "NUMBER":
                 payload_value = payload_value.capitalize()
                 return (
                     bool(payload_value)
                     if payload_value in ["True", "False"]
                     else int(payload_value)
                 )
             if "TIMESTAMP" in db_type:
-                try:
-                    return datetime.datetime.strptime(
-                        payload_value, "%Y-%m-%dT%H:%M:%S"
-                    )
-                except ValueError as v:
-                    if len(v.args) > 0 and v.args[0].startswith(
-                        "unconverted data remains:"
-                    ):
-                        return datetime.datetime.strptime(
-                            payload_value, "%Y-%m-%dT%H:%M:%S.%f"
-                        )
-                    else:
-                        raise
+                return datetime.datetime.strptime(payload_value, "%Y-%m-%dT%H:%M:%S")
             if db_type == "BLOB":
                 return payload_value.encode("utf-8")
             return payload_value
 
+        if (isinstance(value, float) or isinstance(value, int)) and math.isnan(value):
+            return None
         if isinstance(value, Decimal):
             return float(value)
-        elif isinstance(value, str):
-            col_type = self.table_cache.get_col_type(table, column)
+        if isinstance(value, str):
+            col_type = self.column_cache.get(table.upper()).get(column.upper())
             return cast_string_to_type(col_type, value)
-
         return value
 
+    # TODO: Look into potential optimizations
+    # TODO: https://github.com/vmware/versatile-data-kit/issues/2931
     def _insert_data(self, table_name: str, payload: List[Dict[str, Any]]) -> None:
         if not payload:
             return
 
-        def split(lst, n):
-            """Yield successive n-sized chunks from lst."""
-            for i in range(0, len(lst), n):
-                yield lst[i : i + n]
-
-        query, params = self._populate_query_parameters_tuple(table_name, payload)
-        batches = list(split(params, self.ingest_batch_size))
-        for batch in batches:
-            self.cursor.executemany(query, batch)
-
-    def _populate_query_parameters_tuple(
-        self, destination_table: str, payload: List[dict]
-    ) -> (str, list):
-        """
-        Prepare the SQL query and parameters for bulk insertion.
-
-        Returns insert into destination table tuple of query and parameters;
-        E.g. for a table dest_table with columns val1, val2 and payload size 2, this method will return:
-        'INSERT INTO dest_table (val1, val2) VALUES (:0, :1)',
-        [('val1', 'val2'), ('val1', 'val2')]
-        """
-        columns = self.table_cache.get_columns(destination_table)
-        query_columns = [_escape_special_chars(col) for col in columns]
-
-        placeholders = ", ".join(f":{i}" for i in range(len(columns)))
-        query = f"INSERT INTO {destination_table} ({', '.join(query_columns)}) VALUES ({placeholders})"
-
-        parameters = []
-        for obj in payload:
-            row = tuple(
-                self._cast_to_correct_type(
-                    destination_table, column.lower(), obj.get(column.lower())
-                )
-                for column in columns
-            )
-            parameters.append(row)
-
-        return query, parameters
+        # group dicts by key set
+        batches = {}
+        for p in payload:
+            batch = frozenset(p.keys())
+            if batch not in batches:
+                batches[batch] = []
+            batches[batch].append(p)
+
+        # create queries for groups of dicts with the same key set
+        queries = []
+        batch_data = []
+        for column_names, batch in batches.items():
+            columns = list(column_names)
+            insert_sql = f"INSERT INTO {table_name} ({', '.join(columns)}) VALUES ({', '.join([':' + str(i + 1) for i in range(len(columns))])})"
+            queries.append(insert_sql)
+            temp_data = []
+            for row in batch:
+                temp = [
+                    self._cast_to_correct_type(table_name, col, row[col])
+                    for col in columns
+                ]
+                temp_data.append(temp)
+            batch_data.append(temp_data)
+
+        # batch execute queries for dicts with the same key set
+        for i in range(len(queries)):
+            self.cursor.executemany(queries[i], batch_data[i])
 
     def ingest_payload(
         self,
         payload: List[Dict[str, Any]],
         destination_table: Optional[str] = None,
         target: str = None,
         collection_id: Optional[str] = None,
         metadata: Optional[IIngesterPlugin.IngestionMetadata] = None,
     ) -> None:
         if not payload:
             return None
         if not destination_table:
             raise ValueError("Destination table must be specified if not in payload.")
 
-        if not self.table_cache.table_exists(destination_table):
+        if not self._table_exists(destination_table):
             self._create_table(destination_table, payload[0])
-            self.table_cache.cache_columns(destination_table)
+            self._cache_columns(destination_table)
 
         self._add_columns(destination_table, payload)
         self._insert_data(destination_table, payload)
 
+        # TODO: test if we need this commit statement (most probably we don't, the connection already commits after every transaction)
         self.conn.commit()
         return metadata
```

### Comparing `vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/oracle_configuration.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import pathlib
 import tempfile
 from typing import Dict
 from typing import Optional
 
@@ -14,16 +14,14 @@
 ORACLE_USE_SECRETS = "ORACLE_USE_SECRETS"
 ORACLE_THICK_MODE = "ORACLE_THICK_MODE"
 ORACLE_THICK_MODE_LIB_DIR = "ORACLE_THICK_MODE_LIB_DIR"
 ORACLE_CONNECTION_STRING = "ORACLE_CONNECTION_STRING"
 ORACLE_HOST = "ORACLE_HOST"
 ORACLE_PORT = "ORACLE_PORT"
 ORACLE_SID = "ORACLE_SID"
-ORACLE_SERVICE_NAME = "ORACLE_SERVICE_NAME"
-ORACLE_INGEST_BATCH_SIZE = "ORACLE_INGEST_BATCH_SIZE"
 
 
 class OracleConfiguration:
     def __init__(self, configuration: Configuration):
         self.__config = configuration
 
     def get_oracle_user(self) -> str:
@@ -40,29 +38,23 @@
 
     def get_oracle_port(self) -> int:
         return int(self.__config.get_value(ORACLE_PORT))
 
     def get_oracle_sid(self) -> str:
         return self.__config.get_value(ORACLE_SID)
 
-    def get_oracle_service_name(self) -> str:
-        return self.__config.get_value(ORACLE_SERVICE_NAME)
-
     def oracle_use_secrets(self) -> bool:
         return self.__config.get_value(ORACLE_USE_SECRETS)
 
     def oracle_thick_mode(self) -> bool:
         return self.__config.get_value(ORACLE_THICK_MODE)
 
     def oracle_thick_mode_lib_dir(self) -> Optional[str]:
         return self.__config.get_value(ORACLE_THICK_MODE_LIB_DIR)
 
-    def oracle_ingest_batch_size(self) -> Optional[int]:
-        return int(self.__config.get_value(ORACLE_INGEST_BATCH_SIZE))
-
     @staticmethod
     def add_definitions(config_builder: ConfigurationBuilder):
         config_builder.add(
             key=ORACLE_USER,
             default_value=None,
             is_sensitive=True,
             description="The Oracle user for the database connection",
@@ -94,40 +86,29 @@
         config_builder.add(
             key=ORACLE_SID,
             default_value=None,
             is_sensitive=True,
             description="The schema id of the Oracle database. Note: This option is overridden by ORACLE_CONNECTION_STRING",
         )
         config_builder.add(
-            key=ORACLE_SERVICE_NAME,
-            default_value=None,
-            is_sensitive=True,
-            description="The service name of the Oracle database. Note: This option is overridden by ORACLE_CONNECTION_STRING",
-        )
-        config_builder.add(
             key=ORACLE_USE_SECRETS,
             default_value=True,
             description="Set this flag to use secrets to connect to Oracle. This is protype option. "
             "Leave default value unless there are issues.",
         )
         config_builder.add(
             key=ORACLE_THICK_MODE,
-            default_value=True,
+            default_value=False,
             description="Use oracle thick mode. Set to False to disable oracle thick mode."
             "If set to true you may need to manually install client library. "
             "Refer to "
             "https://python-oracledb.readthedocs.io/en/latest/user_guide/initialization.html#enablingthick "
             "More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html",
         )
         config_builder.add(
             key=ORACLE_THICK_MODE_LIB_DIR,
             default_value=None,
-            description="This is the location of the Oracle Client library used when thick mode is enabled. "
+            description="This is the location of the Oracle Client library used when tick mode is enabled. "
             "This option is ignored if ORACLE_THICK_MODE is false."
             "Before setting this follow instruction in "
             "https://python-oracledb.readthedocs.io/en/latest/user_guide/initialization.html#enablingthick ",
         )
-        config_builder.add(
-            key=ORACLE_INGEST_BATCH_SIZE,
-            default_value=100,
-            description="Batch size when ingesting records into Oracle.",
-        )
```

### Comparing `vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/oracle_connection.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 from typing import List
 from typing import Optional
 
 from oracledb import Connection
@@ -18,26 +18,24 @@
     def __init__(
         self,
         user: str,
         password: str,
         connection_string: str = None,
         host=None,
         port=1521,
-        sid: str = None,
-        service_name: str = None,
+        sid=None,
         thick_mode: bool = True,
         thick_mode_lib_dir: Optional[str] = None,
     ):
         super().__init__(log)
         self._oracle_user = user
         self._oracle_password = password
         self._host = host
         self._port = port
         self._sid = sid
-        self._service_name = service_name
         self._oracle_connection_string = connection_string
         self._thick_mode = thick_mode
         self._thick_mode_lib_dir = thick_mode_lib_dir
 
     def _connect(self) -> Connection:
         import oracledb
 
@@ -58,15 +56,14 @@
             log.debug("Connecting to Oracle using host,port,sid")
             params = oracledb.ConnectParams(
                 user=self._oracle_user,
                 password=self._oracle_password,
                 host=self._host,
                 port=self._port,
                 sid=self._sid,
-                service_name=self._service_name,
             )
             conn = oracledb.connect(params=params)
         return conn
 
     def _is_connected(self) -> bool:
         if None is self._is_db_con_open:
             return False
```

### Comparing `vdk-oracle-0.1.1245476944/src/vdk/plugin/oracle/oracle_plugin.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import List
 
 import click
 import oracledb
 from tabulate import tabulate
@@ -31,56 +31,50 @@
     def vdk_configure(self, config_builder: ConfigurationBuilder):
         OracleConfiguration.add_definitions(config_builder)
 
     @hookimpl(trylast=True)
     def initialize_job(self, context: JobContext):
         conf = OracleConfiguration(context.core_context.configuration)
         oracle_user, oracle_pass = conf.get_oracle_user(), conf.get_oracle_password()
+        if conf.oracle_use_secrets():
+            # TODO: this will be removed once support for reading configuration from secrets is added in core
+            job_secrets = context.job_input.get_all_secrets()
+            oracle_user = job_secrets.get(ORACLE_USER.lower(), oracle_user)
+            oracle_pass = job_secrets.get(ORACLE_PASSWORD.lower(), oracle_pass)
         context.connections.add_open_connection_factory_method(
             "ORACLE",
             lambda: OracleConnection(
                 oracle_user,
                 oracle_pass,
                 conf.get_oracle_connection_string(),
                 host=conf.get_oracle_host(),
                 port=conf.get_oracle_port(),
                 sid=conf.get_oracle_sid(),
-                service_name=conf.get_oracle_service_name(),
                 thick_mode=conf.oracle_thick_mode(),
                 thick_mode_lib_dir=conf.oracle_thick_mode_lib_dir(),
             ),
         )
         context.ingester.add_ingester_factory_method(
-            "oracle",
-            lambda: IngestToOracle(
-                context.connections, conf.oracle_ingest_batch_size()
-            ),
+            "oracle", (lambda: IngestToOracle(context.connections))
         )
 
 
 @hookimpl
 def vdk_start(plugin_registry: IPluginRegistry, command_line_args: List):
     plugin_registry.load_plugin_with_hooks_impl(OraclePlugin(), "OraclePlugin")
 
 
 # TODO: https://github.com/vmware/versatile-data-kit/issues/2940
 @click.command(
     name="oracle-query",
-    help="DEPRECATED: use sql-query, instead."
-    "Execute an Oracle query against an Oracle database (should be configured with env variables)",
+    help="Execute an Oracle query against an Oracle database (should be configured with env variables)",
 )
 @click.option("-q", "--query", type=click.STRING, required=True)
 @click.pass_context
 def oracle_query(ctx: click.Context, query):
-    """
-    Deprecated: "Use sql-query instead"
-
-    oracle-query: kept for compatibility
-    """
-    log.warning("oracle-query has been deprecated; please use sql-query instead.")
     conf = ctx.obj.configuration
     conn = oracledb.connect(
         user=conf.get_value(ORACLE_USER),
         password=conf.get_value(ORACLE_PASSWORD),
         dsn=conf.get_value(ORACLE_CONNECTION_STRING),
     )
```

### Comparing `vdk-oracle-0.1.1245476944/src/vdk_oracle.egg-info/PKG-INFO` & `vdk-oracle-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,9 @@
-Metadata-Version: 2.1
-Name: vdk-oracle
-Version: 0.1.1245476944
-Summary: Support for VDK Managed Oracle connection
-Home-page: https://github.com/vmware/versatile-data-kit
-Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
-Project-URL: Source Code, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
-Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues/new/choose
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Requires-Dist: vdk-core
-Requires-Dist: oracledb
-Requires-Dist: tabulate
-
 # oracle
 
-<a href="https://pypistats.org/packages/vdk-oracle" alt="Monthly Downloads">
-        <img src="https://img.shields.io/pypi/dm/vdk-oracle.svg" alt="monthly download count for vdk-oracle"></a>
-
 Support for VDK Managed Oracle connection
 
 TODO: what the project is about, what is its purpose
 
 
 ## Usage
 
@@ -44,17 +20,15 @@
 | oracle_user              | Username used when connecting to Oracle database                                                                                                                                                                                      | my_user             |
 | oracle_password          | Password used when connecting to Oracle database                                                                                                                                                                                      | super_secret_shhhh  |
 | oracle_use_secrets       | Set to True to use secrets to connect to Oracle                                                                                                                                                                                       | True                |
 | oracle_connection_string | The Oracle connection string                                                                                                                                                                                                          | localhost:1521/free |
 | oracle_host              | The host of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | localhost           |
 | oracle_port              | The port of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | 1521                |
 | oracle_sid               | The SID of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                        | free                |
-| oracle_service_name      | The Service name of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                               | free                |
 | oracle_thick_mode        | Python-oracledb is said to be in Thick mode when Oracle Client libraries are used. True by default. Set to False to disable Oracle Thick mode. More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html | True                |
-| oracle_ingest_batch_size | vdk-oracle splits ingestion payloads into batches. Change this config to control the batch size. Default is set to 100.                                                                                                               | 100                 |
 
 ### Example
 
 #### CLI Queries
 
 ```sh
 export VDK_ORACLE_USER=my_username
```

### Comparing `vdk-oracle-0.1.1245476944/tests/test_secrets_config.py` & `vdk-oracle-0.1.2/tests/test_secrets_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import os
 from unittest import mock
 
 import pytest
 from click.testing import Result
```

