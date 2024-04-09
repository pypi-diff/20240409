# Comparing `tmp/shipyard_databricks_sql-0.2.1a0.tar.gz` & `tmp/shipyard_databricks_sql-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_databricks_sql-0.2.1a0.tar", max compression
+gzip compressed data, was "shipyard_databricks_sql-0.2.1a1.tar", max compression
```

## Comparing `shipyard_databricks_sql-0.2.1a0.tar` & `shipyard_databricks_sql-0.2.1a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-12-11 17:36:50.276565 shipyard_databricks_sql-0.2.1a0/README.md
--rw-r--r--   0        0        0      661 2024-04-08 20:43:04.434758 shipyard_databricks_sql-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-12-11 17:36:50.278442 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:38.928930 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/__init__.py
--rw-r--r--   0        0        0      667 2024-04-08 19:03:13.629501 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/authtest.py
--rw-r--r--   0        0        0     4131 2024-04-01 19:04:10.733520 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/copy_from_s3.py
--rw-r--r--   0        0        0     1629 2024-04-01 19:04:10.735412 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/execute.py
--rw-r--r--   0        0        0     2596 2024-04-01 19:04:10.736714 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/fetch.py
--rw-r--r--   0        0        0     5498 2024-04-08 20:21:46.706453 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/upload.py
--rw-r--r--   0        0        0    27529 2024-04-01 19:04:10.738097 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/databricks.py
--rw-r--r--   0        0        0     2234 2024-04-01 19:04:10.738478 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/utils/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-01 19:04:10.738589 shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/utils/utils.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 shipyard_databricks_sql-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-11 17:36:50.276565 shipyard_databricks_sql-0.2.1a1/README.md
+-rw-r--r--   0        0        0      661 2024-04-09 03:35:43.667404 shipyard_databricks_sql-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-12-11 17:36:50.278442 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:38.928930 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-09 03:35:33.257067 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/authtest.py
+-rw-r--r--   0        0        0     4131 2024-04-01 19:04:10.733520 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/copy_from_s3.py
+-rw-r--r--   0        0        0     1604 2024-04-09 02:33:19.119752 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/execute.py
+-rw-r--r--   0        0        0     2621 2024-04-09 03:35:33.307369 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/fetch.py
+-rw-r--r--   0        0        0     5495 2024-04-09 01:26:28.397565 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/upload.py
+-rw-r--r--   0        0        0    27878 2024-04-09 03:35:33.572046 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/databricks.py
+-rw-r--r--   0        0        0     2234 2024-04-01 19:04:10.738478 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/utils/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:04:10.738589 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/utils/utils.py
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 shipyard_databricks_sql-0.2.1a1/PKG-INFO
```

### Comparing `shipyard_databricks_sql-0.2.1a0/pyproject.toml` & `shipyard_databricks_sql-0.2.1a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-databricks-sql"
-version = "0.2.1a0"
+version = "0.2.1a1"
 description = "A local client for connecting and working Databricks SQL Warehouses"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shipyard-templates = "^0.8.1"
```

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/authtest.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/authtest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 import sys
 from shipyard_databricks_sql import DatabricksSqlClient
-from shipyard_templates import ShipyardLogger 
+from shipyard_templates import ShipyardLogger
 
 logger = ShipyardLogger.get_logger()
 
 
 def main():
     try:
         conn = DatabricksSqlClient(
             access_token=os.getenv("DATABRICKS_SQL_ACCESS_TOKEN"),
             server_host=os.getenv("DATABRICKS_SERVER_HOST"),
             http_path=os.getenv("DATABRICKS_HTTP_PATH"),
         ).connect()
     except Exception as e:
-        logger.authtest(f"Error in connecting to Databricks with provided credentials. Message: {e}")
+        logger.authtest(
+            f"Error in connecting to Databricks with provided credentials. Message: {e}"
+        )
         sys.exit(1)
 
     else:
         conn.close()
         sys.exit(0)
```

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/copy_from_s3.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/copy_from_s3.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/execute.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/execute.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         client = DatabricksSqlClient(
             server_host=args.server_host,
             http_path=args.http_path,
             access_token=args.access_token,
             catalog=catalog,
             schema=schema,
         )
-        client.connect()
         client.execute_query(args.query)
     except ExitCodeException as ec:
         logger.error(f"ExitCodeException: Error in executing query {ec.message}")
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(f"Error in attempting to execute query in Databricks:{str(e)}")
         sys.exit(client.EXIT_CODE_INVALID_QUERY)
```

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/fetch.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import argparse
 import os
 import sys
+import shipyard_bp_utils as shipyard
 
 from shipyard_templates import ExitCodeException, ShipyardLogger
 from shipyard_databricks_sql import DatabricksSqlClient
+from shipyard_databricks_sql.utils import exceptions as errs
+
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
 
@@ -29,31 +32,30 @@
     return parser.parse_args()
 
 
 def main():
     args = get_args()
     catalog = args.catalog if args.catalog != "" else None
     schema = args.schema if args.schema != "" else None
-    folder_name = args.folder_name if args.folder_name != "" else None
+    folder_name = args.folder_name
+    client = None
     try:
         if folder_name:
-            if not os.path.exists(os.path.join(os.getcwd(), folder_name)):
-                os.mkdir(folder_name)
+            shipyard.files.create_folder_if_dne(folder_name)
             full_path = os.path.join(os.getcwd(), folder_name, args.file_name)
         else:
             full_path = os.path.join(os.getcwd(), args.file_name)
 
         client = DatabricksSqlClient(
             server_host=args.server_host,
             http_path=args.http_path,
             access_token=args.access_token,
             catalog=catalog,
             schema=schema,
         )
-        client.connect()
         data = client.fetch(args.query)
         logger.info(f"Successfully fetched {data.shape[0]} rows")
 
         if args.file_type == "csv":
             data.to_csv(full_path, index=False)
         # for parquet files
         else:
@@ -62,16 +64,17 @@
     except ExitCodeException as ec:
         logger.error(
             f"ExitCodeException: Error in attempting to fetch results: {ec.message}"
         )
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(f"Error in attempting to fetch query results:{str(e)}")
-        sys.exit(client.EXIT_CODE_INVALID_QUERY)
+        sys.exit(errs.EXIT_CODE_INVALID_QUERY)
     else:
         logger.info(f"Downloaded results to {full_path}")
     finally:
-        client.close()
+        if client:
+            client.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/cli/upload.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     args = get_args()
     catalog = args.catalog if args.catalog != "" else None
     schema = args.schema if args.schema != "" else None
     volume = args.volume if args.volume != "" else None
     folder_name = args.folder_name if args.folder_name != "" else None
     data_types = ast.literal_eval(args.data_types) if args.data_types != "" else None
     dir_path = None
+    client = None
 
     try:
         if folder_name:
             full_path = os.path.join(os.getcwd(), folder_name, args.file_name)
             dir_path = os.path.join(os.getcwd(), folder_name)
             real_path = os.path.realpath(dir_path)
         else:
@@ -103,15 +104,14 @@
             http_path=args.http_path,
             access_token=args.access_token,
             catalog=catalog,
             schema=schema,
             volume=volume,
             staging_allowed_local_path=real_path,
         )
-        client.connect()
         if args.match_type == "glob_match":
             local_files = shipyard.files.find_all_local_file_names(folder_name)
             file_matches = shipyard.files.find_matching_files(
                 search_term=args.file_name,
                 directory=folder_name,
                 match_type=args.match_type,
             )
@@ -141,21 +141,22 @@
                 datatypes=data_types,
                 insert_method=args.insert_method,
             )
             logger.info(f"Successfully loaded {full_path} into Databricks")
 
     except ExitCodeException as ec:
         logger.error(
-            f"ExitCodeException: Error in attempting to upload {full_path}. Message from Databricks is: {ec.message}"
+            f"Error in attempting to upload {full_path}. Message from Databricks is: {ec.message}"
         )
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(
             f"Error in attempting to upload {full_path}. Mesasge from Databricks is: {str(e)}"
         )
         sys.exit(errs.EXIT_CODE_INVALID_QUERY)
     finally:
-        client.close()
+        if client:
+            client.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/databricks.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,23 +81,32 @@
             user_agent=self.user_agent,
             staging_allowed_local_path=staging_allowed_local_path,
             _connection=None,
             _cursor=None,
         )
 
     def connect(self) -> Connection:
-        return sql.connect(
-            server_hostname=self.server_host,
-            http_path=self.http_path,
-            access_token=self.access_token,
-            catalog=self.catalog,
-            schema=self.schema,
-            _user_agent_entry=self.user_agent,
-            staging_allowed_local_path=self.staging_allowed_local_path,
-        )
+        try:
+            conn = sql.connect(
+                server_hostname=self.server_host,
+                http_path=self.http_path,
+                access_token=self.access_token,
+                catalog=self.catalog,
+                schema=self.schema,
+                _user_agent_entry=self.user_agent,
+                staging_allowed_local_path=self.staging_allowed_local_path,
+            )
+        except Exception as e:
+            raise ExitCodeException(
+                f"Error in connecting to Databricks: {str(e)}",
+                self.EXIT_CODE_INVALID_CREDENTIALS,
+            )
+        else:
+            logger.info("Successfully connected to Databricks")
+            return conn
 
     @property
     def connection(self):
         if not self._connection:
             self._connection = self.connect()
         return self._connection
```

### Comparing `shipyard_databricks_sql-0.2.1a0/shipyard_databricks_sql/utils/exceptions.py` & `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a0/PKG-INFO` & `shipyard_databricks_sql-0.2.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-databricks-sql
-Version: 0.2.1a0
+Version: 0.2.1a1
 Summary: A local client for connecting and working Databricks SQL Warehouses
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

