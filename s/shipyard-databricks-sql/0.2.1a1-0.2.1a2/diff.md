# Comparing `tmp/shipyard_databricks_sql-0.2.1a1.tar.gz` & `tmp/shipyard_databricks_sql-0.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_databricks_sql-0.2.1a1.tar", max compression
+gzip compressed data, was "shipyard_databricks_sql-0.2.1a2.tar", max compression
```

## Comparing `shipyard_databricks_sql-0.2.1a1.tar` & `shipyard_databricks_sql-0.2.1a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-12-11 17:36:50.276565 shipyard_databricks_sql-0.2.1a1/README.md
--rw-r--r--   0        0        0      661 2024-04-09 03:35:43.667404 shipyard_databricks_sql-0.2.1a1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-12-11 17:36:50.278442 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:38.928930 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/__init__.py
--rw-r--r--   0        0        0      688 2024-04-09 03:35:33.257067 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/authtest.py
--rw-r--r--   0        0        0     4131 2024-04-01 19:04:10.733520 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/copy_from_s3.py
--rw-r--r--   0        0        0     1604 2024-04-09 02:33:19.119752 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/execute.py
--rw-r--r--   0        0        0     2621 2024-04-09 03:35:33.307369 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/fetch.py
--rw-r--r--   0        0        0     5495 2024-04-09 01:26:28.397565 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/upload.py
--rw-r--r--   0        0        0    27878 2024-04-09 03:35:33.572046 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/databricks.py
--rw-r--r--   0        0        0     2234 2024-04-01 19:04:10.738478 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/utils/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-01 19:04:10.738589 shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/utils/utils.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 shipyard_databricks_sql-0.2.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-11 17:36:50.276565 shipyard_databricks_sql-0.2.1a2/README.md
+-rw-r--r--   0        0        0      661 2024-04-09 14:51:42.943760 shipyard_databricks_sql-0.2.1a2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-12-11 17:36:50.278442 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:38.928930 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-09 03:35:33.257067 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/authtest.py
+-rw-r--r--   0        0        0     4131 2024-04-01 19:04:10.733520 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/copy_from_s3.py
+-rw-r--r--   0        0        0     1604 2024-04-09 02:33:19.119752 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/execute.py
+-rw-r--r--   0        0        0     2621 2024-04-09 03:35:33.307369 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/fetch.py
+-rw-r--r--   0        0        0     4767 2024-04-09 14:51:24.332320 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/upload.py
+-rw-r--r--   0        0        0    27641 2024-04-09 14:51:35.294783 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/databricks.py
+-rw-r--r--   0        0        0     2234 2024-04-01 19:04:10.738478 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/utils/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:04:10.738589 shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/utils/utils.py
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 shipyard_databricks_sql-0.2.1a2/PKG-INFO
```

### Comparing `shipyard_databricks_sql-0.2.1a1/pyproject.toml` & `shipyard_databricks_sql-0.2.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-databricks-sql"
-version = "0.2.1a1"
+version = "0.2.1a2"
 description = "A local client for connecting and working Databricks SQL Warehouses"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shipyard-templates = "^0.8.1"
```

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/authtest.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/copy_from_s3.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/copy_from_s3.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/execute.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/execute.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/fetch.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/cli/upload.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/cli/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,47 +43,14 @@
         "--match-type",
         dest="match_type",
         choices={"exact_match", "glob_match"},
     )
     return parser.parse_args()
 
 
-def list_local_files(directory: Optional[str] = None) -> List[str]:
-    """Returns all the files located within the directory path. If the dirname is not provided, then the current working directory will be used and it will span all subdirectories
-
-    Args:
-        dirname: The optional directory to span
-
-    Returns: List of all the files
-
-    """
-    if directory is None:
-        directory = os.getcwd()
-
-    files = []
-    for root, _, filenames in os.walk(directory):
-        for filename in filenames:
-            file_path = os.path.join(root, filename)
-            files.append(file_path)
-
-    return files
-
-
-def find_all_file_matches(file_names, file_name_re):
-    """
-    Return a list of all matching_file_names that matched the regular expression.
-    """
-    matching_file_names = []
-    for file in file_names:
-        if re.search(file_name_re, file):
-            matching_file_names.append(file)
-
-    return matching_file_names
-
-
 def main():
     args = get_args()
     catalog = args.catalog if args.catalog != "" else None
     schema = args.schema if args.schema != "" else None
     volume = args.volume if args.volume != "" else None
     folder_name = args.folder_name if args.folder_name != "" else None
     data_types = ast.literal_eval(args.data_types) if args.data_types != "" else None
@@ -104,21 +71,24 @@
             http_path=args.http_path,
             access_token=args.access_token,
             catalog=catalog,
             schema=schema,
             volume=volume,
             staging_allowed_local_path=real_path,
         )
+        logger.debug(f"Using {args.match_type} to load files")
         if args.match_type == "glob_match":
             local_files = shipyard.files.find_all_local_file_names(folder_name)
+            logger.debug(f"Files found in {folder_name}: {local_files}")
             file_matches = shipyard.files.find_matching_files(
                 search_term=args.file_name,
                 directory=folder_name,
                 match_type=args.match_type,
             )
+            logger.debug(f"Files matching {args.file_name} pattern: {file_matches}")
 
             if len(file_matches) == 0:
                 logger.error(f"No files found matching {args.file_name} pattern")
                 sys.exit(errs.EXIT_CODE_FILE_NOT_FOUND)
 
             client.upload(
                 file_path=file_matches,
```

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/databricks.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/databricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,14 @@
     RemoveVolumeError,
 )
 
 logger = ShipyardLogger.get_logger()
 
 
 class DatabricksSqlClient(DatabricksDatabase):
-    # EXIT_CODE_VOLUME_CREATION = 101
-    # EXIT_CODE_VOLUME_SQL = 102
-    # EXIT_CODE_VOLUME_UPLOAD_ERROR = 103
-    # EXIT_CODE_COPY_INTO_ERROR = 104
-    # EXIT_CODE_REMOVE_VOLUME_ERROR = 105
-    # EXIT_CODE_SCHEMA_CREATION_ERROR = 106
     SPARK_TYPES = {
         "array": "numpy.ndarray",
         "bigint": "int",
         "binary": "bytearray",
         "boolean": "bool",
         "date": "datetime.date",
         "decimal": "decimal",
```

### Comparing `shipyard_databricks_sql-0.2.1a1/shipyard_databricks_sql/utils/exceptions.py` & `shipyard_databricks_sql-0.2.1a2/shipyard_databricks_sql/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_databricks_sql-0.2.1a1/PKG-INFO` & `shipyard_databricks_sql-0.2.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-databricks-sql
-Version: 0.2.1a1
+Version: 0.2.1a2
 Summary: A local client for connecting and working Databricks SQL Warehouses
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

