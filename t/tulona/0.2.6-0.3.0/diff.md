# Comparing `tmp/tulona-0.2.6.tar.gz` & `tmp/tulona-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.2.6.tar", last modified: Sun Apr  7 09:59:23 2024, max compression
+gzip compressed data, was "tulona-0.3.0.tar", last modified: Tue Apr  9 09:43:20 2024, max compression
```

## Comparing `tulona-0.2.6.tar` & `tulona-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.542712 tulona-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-07 09:59:18.000000 tulona-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-07 09:59:23.542712 tulona-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-07 09:59:18.000000 tulona-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.534712 tulona-0.2.6/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.534712 tulona-0.2.6/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.538712 tulona-0.2.6/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.538712 tulona-0.2.6/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.538712 tulona-0.2.6/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.538712 tulona-0.2.6/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.538712 tulona-0.2.6/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.542712 tulona-0.2.6/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-07 09:59:18.000000 tulona-0.2.6/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:59:23.542712 tulona-0.2.6/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-07 09:59:23.000000 tulona-0.2.6/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 09:59:23.000000 tulona-0.2.6/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:59:23.000000 tulona-0.2.6/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 09:59:23.000000 tulona-0.2.6/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 09:59:23.000000 tulona-0.2.6/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 09:59:23.000000 tulona-0.2.6/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 09:59:18.000000 tulona-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:59:23.542712 tulona-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.090960 tulona-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-09 09:43:15.000000 tulona-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-09 09:43:20.090960 tulona-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-09 09:43:15.000000 tulona-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.082960 tulona-0.3.0/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.082960 tulona-0.3.0/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.086960 tulona-0.3.0/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.086960 tulona-0.3.0/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.086960 tulona-0.3.0/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.086960 tulona-0.3.0/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.086960 tulona-0.3.0/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.090960 tulona-0.3.0/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-09 09:43:15.000000 tulona-0.3.0/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:43:20.090960 tulona-0.3.0/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-09 09:43:20.000000 tulona-0.3.0/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 09:43:20.000000 tulona-0.3.0/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:43:20.000000 tulona-0.3.0/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 09:43:20.000000 tulona-0.3.0/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 09:43:20.000000 tulona-0.3.0/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 09:43:20.000000 tulona-0.3.0/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 09:43:15.000000 tulona-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:43:20.090960 tulona-0.3.0/setup.cfg
```

### Comparing `tulona-0.2.6/LICENSE` & `tulona-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/PKG-INFO` & `tulona-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.2.6
+Version: 0.3.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -129,56 +129,62 @@
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
 
-* **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
+* **ping**: To test connectivity to the databases for the datasources. Sample command:
 
-  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
+  * To ping one data source pass the name to the `--datasources` parameter:
 
-    ``tulona compare-column --datasources employee_postgres,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
+    ``tulona ping --datasources employee_postgres``
 
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
+  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
 
-    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
+    ``tulona ping --datasources employee_postgres,employee_mysql``
 
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
+* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+
+  * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
+
+    ``tulona profile --datasources employee_postgres,employee_mysql``
+  * Profiling with `--compare` flag. It will produce a comparison view (side by side):
+
+    ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
 * **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
-* **ping**: To test connectivity to the databases for the datasources. Sample command:
+* **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
-  * To ping one data source pass the name to the `--datasources` parameter:
+  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
 
-    ``tulona ping --datasources employee_postgres``
+    ``tulona compare-column --datasources employee_postgres,employee_mysql``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
 
-  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
+    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
 
-    ``tulona ping --datasources employee_postgres,employee_mysql``
+    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
 
-* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
 
-  * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
+* **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
-    ``tulona profile --datasources employee_postgres,employee_mysql``
-  * Profiling with `--compare` flag. It will produce a comparison view (side by side):
+  ``tulona compare --datasources employee_postgres,employee_mysql``
 
-    ``tulona profile --compare --datasources employee_postgres,employee_mysql``
+For debug level log, add `-v` or `--verbose` flag along with any command. For example: ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Development Environment Setup
 -----------------------------
 * For live installation execute `pip install --editable core`.
@@ -193,16 +199,16 @@
 * Execute `pip install <wheel-file.whl>`
 
 
 .. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
 .. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
-.. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
-   :target: https://codecov.io/gh/mrinalsardar/tulona
+.. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/mrinalsardar/tulona/branch/main
    :alt: Coverage status
 .. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
    :target: https://pypi.python.org/pypi/tulona/
 .. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
    :target: https://pypi.org/project/tulona/
 .. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
    :target: http://www.apache.org/licenses/LICENSE-2.0.txt
```

### Comparing `tulona-0.2.6/README.rst` & `tulona-0.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -96,56 +96,62 @@
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
 
-* **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
+* **ping**: To test connectivity to the databases for the datasources. Sample command:
 
-  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
+  * To ping one data source pass the name to the `--datasources` parameter:
 
-    ``tulona compare-column --datasources employee_postgres,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
+    ``tulona ping --datasources employee_postgres``
 
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
+  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
 
-    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
+    ``tulona ping --datasources employee_postgres,employee_mysql``
 
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
+* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+
+  * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
+
+    ``tulona profile --datasources employee_postgres,employee_mysql``
+  * Profiling with `--compare` flag. It will produce a comparison view (side by side):
+
+    ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
 * **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
-* **ping**: To test connectivity to the databases for the datasources. Sample command:
+* **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
-  * To ping one data source pass the name to the `--datasources` parameter:
+  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
 
-    ``tulona ping --datasources employee_postgres``
+    ``tulona compare-column --datasources employee_postgres,employee_mysql``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
 
-  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
+    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
 
-    ``tulona ping --datasources employee_postgres,employee_mysql``
+    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
 
-* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
 
-  * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
+* **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
-    ``tulona profile --datasources employee_postgres,employee_mysql``
-  * Profiling with `--compare` flag. It will produce a comparison view (side by side):
+  ``tulona compare --datasources employee_postgres,employee_mysql``
 
-    ``tulona profile --compare --datasources employee_postgres,employee_mysql``
+For debug level log, add `-v` or `--verbose` flag along with any command. For example: ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Development Environment Setup
 -----------------------------
 * For live installation execute `pip install --editable core`.
@@ -160,16 +166,16 @@
 * Execute `pip install <wheel-file.whl>`
 
 
 .. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
 .. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
-.. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
-   :target: https://codecov.io/gh/mrinalsardar/tulona
+.. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/mrinalsardar/tulona/branch/main
    :alt: Coverage status
 .. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
    :target: https://pypi.python.org/pypi/tulona/
 .. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
    :target: https://pypi.org/project/tulona/
 .. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
    :target: http://www.apache.org/licenses/LICENSE-2.0.txt
```

### Comparing `tulona-0.2.6/core/tulona/adapter/connection.py` & `tulona-0.3.0/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/adapter/mssql.py` & `tulona-0.3.0/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/adapter/mysql.py` & `tulona-0.3.0/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/adapter/postgres.py` & `tulona-0.3.0/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/adapter/snowflake.py` & `tulona-0.3.0/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/cli/base.py` & `tulona-0.3.0/core/tulona/cli/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import click
 
 from tulona.cli import params as p
 from tulona.config.profile import Profile
 from tulona.config.project import Project
 from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingArgumentError
-from tulona.task.compare import CompareColumnTask, CompareDataTask
+from tulona.task.compare import CompareColumnTask, CompareDataTask, CompareTask
 
 # from tulona.task.scan import ScanTask
 from tulona.task.ping import PingTask
 from tulona.task.profile import ProfileTask
+from tulona.util.filesystem import get_outfile_fqn
 
 log = logging.getLogger(__name__)
 logging.basicConfig(
-    level=logging.DEBUG,  # TODO: Set level to INFO once verbosity is fixed
+    level=logging.INFO,
     format="[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s",
 )
 
 # TODO: Make use of command line arguments like exec_engine, outdir etc.
 # to override project config values.
 
 
@@ -33,170 +34,148 @@
 def cli(ctx):
     """Tulona compares data sources to find out differences"""
 
 
 # command: tulona ping
 @cli.command("ping")
 @click.pass_context
-@p.exec_engine
+# @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 def ping(ctx, **kwargs):
     """Test connectivity to datasources"""
 
-    if "datasources" not in kwargs:
+    if not kwargs["datasources"]:
         raise TulonaMissingArgumentError(
             "--datasources argument must be provided with command: ping"
         )
 
     if kwargs["verbose"]:
-        # TODO: Fix me
-        # This setting doesn't enable debug level logging
-        handler = logging.StreamHandler()
-        handler.setLevel(logging.DEBUG)
+        logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
 
     datasource_list = kwargs["datasources"].split(",")
 
-    task = PingTask(ctx.obj["profile"], ctx.obj["project"], datasource_list)
+    task = PingTask(
+        profile=ctx.obj["profile"],
+        project=ctx.obj["project"],
+        datasources=datasource_list,
+    )
     task.execute()
 
 
-# # command: tulona scan
-# @cli.command("scan")
-# @click.pass_context
-# @p.exec_engine
-# @p.outdir
-# @p.verbose
-# @p.datasources
-# def scan(ctx, **kwargs):
-#     """Scans data sources for schemas, tables, columns etc."""
-
-#     if "datasources" not in kwargs:
-#         raise TulonaMissingArgumentError(
-#             "--datasources argument must be provided with command: scan"
-#         )
-
-#     if kwargs["verbose"]:
-#         # TODO: Fix me
-#         # This setting doesn't enable debug level logging
-#         handler = logging.StreamHandler()
-#         handler.setLevel(logging.DEBUG)
-
-#     prof = Profile()
-#     proj = Project()
-
-#     ctx.obj = ctx.obj or {}
-#     ctx.obj["project"] = proj.load_project_config()
-#     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
-#     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
-
-#     datasource_list = kwargs["datasources"].split(",")
-
-#     task = ScanTask(ctx.obj["profile"], ctx.obj["project"], ctx.obj["runtime"], datasource_list)
-#     task.execute()
-
-
 # command: tulona profile
 @cli.command("profile")
 @click.pass_context
-@p.exec_engine
+# @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 @p.compare
 def profile(ctx, **kwargs):
     """Profile data sources to collect metadata [row count, column min/max/mean etc.]"""
 
-    if "datasources" not in kwargs:
+    if not kwargs["datasources"]:
         raise TulonaMissingArgumentError(
             "--datasources argument must be provided with command: profile"
         )
 
     if kwargs["verbose"]:
-        # TODO: Fix me
-        # This setting doesn't enable debug level logging
-        handler = logging.StreamHandler()
-        handler.setLevel(logging.DEBUG)
+        logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
     datasource_list = kwargs["datasources"].split(",")
 
+    # Override config outdir if provided in command line
+    if kwargs["outdir"]:
+        ctx.obj["project"]["outdir"] = kwargs["outdir"]
+    outfile_fqn = get_outfile_fqn(
+        outdir=ctx.obj["project"]["outdir"],
+        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+        infix="data_comparison",
+    )
+
     task = ProfileTask(
-        ctx.obj["profile"],
-        ctx.obj["project"],
-        ctx.obj["runtime"],
-        datasource_list,
+        profile=ctx.obj["profile"],
+        project=ctx.obj["project"],
+        runtime=ctx.obj["runtime"],
+        datasources=datasource_list,
+        outfile_fqn=outfile_fqn,
         compare=kwargs["compare"],
     )
     task.execute()
 
 
 # command: tulona compare-data
 @cli.command("compare-data")
 @click.pass_context
-@p.exec_engine
+# @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 @p.sample_count
 def compare_data(ctx, **kwargs):
     """Compares two data entities"""
 
-    if "datasources" not in kwargs:
+    if not kwargs["datasources"]:
         raise TulonaMissingArgumentError(
             "--datasources argument must be provided with command: compare-data"
         )
 
     if kwargs["verbose"]:
-        # TODO: Fix me
-        # This setting doesn't enable debug level logging
-        logging.basicConfig(
-            level=logging.DEBUG,
-            format="[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s",
-        )
+        logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
     datasource_list = kwargs["datasources"].split(",")
 
+    # Override config outdir if provided in command line
+    if kwargs["outdir"]:
+        ctx.obj["project"]["outdir"] = kwargs["outdir"]
+    outfile_fqn = get_outfile_fqn(
+        outdir=ctx.obj["project"]["outdir"],
+        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+        infix="data_comparison",
+    )
+
     task = CompareDataTask(
         profile=ctx.obj["profile"],
         project=ctx.obj["project"],
         runtime=ctx.obj["runtime"],
         datasources=datasource_list,
+        outfile_fqn=outfile_fqn,
         sample_count=kwargs["sample_count"],
     )
     task.execute()
 
 
 # command: tulona compare-column
 @cli.command("compare-column")
 @click.pass_context
-@p.exec_engine
+# @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 def compare_column(ctx, **kwargs):
     """
     Column name must be specified for task: compare-column
     either by specifying 'compare_column' property in
@@ -207,41 +186,97 @@
     (column name is same for option 3 and 4):-
     1. <datasource1>:<col1>,<datasource2>:<col2>
     2. <datasource1>:<col>,<datasource2>:<col>
     3. <datasource1>:<col>,<datasource2>
     4. <datasource1>,<datasource2>:<col>
     """
 
-    if "datasources" not in kwargs:
+    if not kwargs["datasources"]:
         raise TulonaMissingArgumentError(
             "--datasources argument must be provided with command: compare-column"
         )
 
     if kwargs["verbose"]:
-        # TODO: Fix me
-        # This setting doesn't enable debug level logging
-        logging.basicConfig(
-            level=logging.DEBUG,
-            format="[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s",
-        )
+        logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
     datasource_list = kwargs["datasources"].split(",")
 
+    # Override config outdir if provided in command line
+    if kwargs["outdir"]:
+        ctx.obj["project"]["outdir"] = kwargs["outdir"]
+    outfile_fqn = get_outfile_fqn(
+        outdir=ctx.obj["project"]["outdir"],
+        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+        infix="column_comparison",
+    )
+
     task = CompareColumnTask(
         profile=ctx.obj["profile"],
         project=ctx.obj["project"],
         runtime=ctx.obj["runtime"],
         datasources=datasource_list,
+        outfile_fqn=outfile_fqn,
+    )
+    task.execute()
+
+
+# command: tulona compare
+@cli.command("compare")
+@click.pass_context
+# @p.exec_engine
+@p.outdir
+@p.verbose
+@p.datasources
+@p.sample_count
+def compare(ctx, **kwargs):
+    """
+    Compare everything(profiles, rows and columns) for the given datasoures
+    """
+
+    if not kwargs["datasources"]:
+        raise TulonaMissingArgumentError(
+            "--datasources argument must be provided with command: compare-column"
+        )
+
+    if kwargs["verbose"]:
+        logging.getLogger("tulona").setLevel(logging.DEBUG)
+
+    prof = Profile()
+    proj = Project()
+
+    ctx.obj = ctx.obj or {}
+    ctx.obj["project"] = proj.load_project_config()
+    ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
+    ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
+
+    datasource_list = kwargs["datasources"].split(",")
+
+    # Override config outdir if provided in command line
+    if kwargs["outdir"]:
+        ctx.obj["project"]["outdir"] = kwargs["outdir"]
+    outfile_fqn = get_outfile_fqn(
+        outdir=ctx.obj["project"]["outdir"],
+        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+        infix="comparison",
+    )
+
+    task = CompareTask(
+        profile=ctx.obj["profile"],
+        project=ctx.obj["project"],
+        runtime=ctx.obj["runtime"],
+        datasources=datasource_list,
+        outfile_fqn=outfile_fqn,
+        sample_count=kwargs["sample_count"],
     )
     task.execute()
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `tulona-0.2.6/core/tulona/cli/params.py` & `tulona-0.3.0/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/config/profile.py` & `tulona-0.3.0/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/config/project.py` & `tulona-0.3.0/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/exceptions.py` & `tulona-0.3.0/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/task/base.py` & `tulona-0.3.0/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/task/compare.py` & `tulona-0.3.0/core/tulona/task/compare.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import logging
+import os
 import time
 from dataclasses import _MISSING_TYPE, dataclass, fields
-from datetime import datetime
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Union
 
 import pandas as pd
 
 from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingPrimaryKeyError, TulonaMissingPropertyError
 from tulona.task.base import BaseTask
+from tulona.task.helper import perform_comparison
+from tulona.task.profile import ProfileTask
 from tulona.util.dataframe import apply_column_exclusion
 from tulona.util.excel import highlight_mismatch_cells
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
 from tulona.util.project import extract_table_name_from_config
 from tulona.util.sql import (
     build_filter_query_expression,
     get_column_query,
     get_query_output_as_df,
-    get_sample_row_query,
+    get_table_data_query,
+    get_table_fqn,
 )
 
 log = logging.getLogger(__name__)
 
 DEFAULT_VALUES = {
     "sample_count": 20,
 }
@@ -31,198 +34,214 @@
 
 @dataclass
 class CompareDataTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
     datasources: List[str]
+    outfile_fqn: Union[Path, str]
     sample_count: int = DEFAULT_VALUES["sample_count"]
 
     # Support for default values
     def __post_init__(self):
         for field in fields(self):
             # If there is a default and the value of the field is none we can assign a value
             if (
                 not isinstance(field.default, _MISSING_TYPE)
                 and getattr(self, field.name) is None
             ):
                 setattr(self, field.name, field.default)
 
-    # TODO: needs refactoring to remove duplicate some code
-    def get_table_data(self, datasource, query_expr: str = None):
-        connection_profile = get_connection_profile(
-            self.profile, self.project, datasource
-        )
-        conman = self.get_connection_manager(conn_profile=connection_profile)
-
-        ds_dict = self.project["datasources"][datasource]
-        dbtype = self.profile["profiles"][extract_profile_name(self.project, datasource)][
-            "type"
-        ]
-        table_name = extract_table_name_from_config(config=ds_dict, dbtype=dbtype)
-
-        if query_expr:
-            query = f"select * from {table_name} where {query_expr}"
-        else:
-            query = get_sample_row_query(
-                dbtype=dbtype, table_name=table_name, sample_count=self.sample_count
-            )
-
-        df = get_query_output_as_df(connection_manager=conman, query_text=query)
-        return df
-
-    def get_outfile_fqn(self, ds_list):
-        outdir = create_dir_if_not_exist(self.project["outdir"])
-        out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
-        outfile = f"{'_'.join(ds_list)}_data_comparison_{out_timestamp}.xlsx"
-        outfile_fqn = Path(outdir, outfile)
-        return outfile_fqn
-
     def execute(self):
-        log.info("Starting task: Compare")
+        log.info("------------------------ Starting task: compare-data")
         start_time = time.time()
 
         if len(self.datasources) != 2:
-            raise ValueError("Comparison works between two entities, not more, not less.")
+            raise ValueError("Comparison needs two data sources.")
 
-        datasource1, datasource2 = self.datasources
-        ds_dict1 = self.project["datasources"][datasource1]
-        ds_dict2 = self.project["datasources"][datasource2]
+        # TODO: Add support of composite primary key
+        # TODO: Add support for different names of primary keys in different tables
+        # Check if primary key[s] is[are] specified for row comparison
+        primary_keys = set()
+        ds_names = []
+        ds_name_compressed_list = []
+        ds_configs = []
+        dbtypes = []
+        table_fqns = []
+        connection_managers = []
+        exclude_columns_lol = []
+        for ds_name in self.datasources:
+            log.debug(f"Extracting configs for: {ds_name}")
+            # Extract data source name from datasource:column combination
+            ds_name = ds_name.split(":")[0]
+            ds_names.append(ds_name)
+            ds_name_compressed_list.append(ds_name.replace("_", ""))
+
+            ds_config = self.project["datasources"][ds_name]
+            ds_configs.append(ds_config)
+            dbtype = self.profile["profiles"][
+                extract_profile_name(self.project, ds_name)
+            ]["type"]
+            dbtypes.append(dbtype)
+
+            # MySQL doesn't have logical database
+            if "database" in ds_config and dbtype.lower() != "mysql":
+                database = ds_config["database"]
+            else:
+                database = None
+            schema = ds_config["schema"]
+            table = ds_config["table"]
+
+            table_fqn = get_table_fqn(
+                database,
+                schema,
+                table,
+            )
+            table_fqns.append(table_fqn)
 
-        dbtype1 = self.profile["profiles"][
-            extract_profile_name(self.project, datasource1)
-        ]["type"]
-        dbtype2 = self.profile["profiles"][
-            extract_profile_name(self.project, datasource2)
-        ]["type"]
-        table_name1 = extract_table_name_from_config(config=ds_dict1, dbtype=dbtype1)
-        table_name2 = extract_table_name_from_config(config=ds_dict2, dbtype=dbtype2)
+            log.debug(f"Acquiring connection to the database of: {ds_name}")
+            connection_profile = get_connection_profile(
+                self.profile, self.project, ds_name
+            )
+            connection_managers.append(
+                self.get_connection_manager(conn_profile=connection_profile)
+            )
 
-        # Extract rows from both data sources
-        log.debug(
-            f"Trying to extract {self.sample_count} common records from both data sources"
-        )
-        if "primary_key" in ds_dict1 and "primary_key" in ds_dict2:
-            i = 0
-            while i < 10:
-                log.debug(f"Extraction iteration: {i + 1}")
-
-                df1 = self.get_table_data(datasource=datasource1)
-                if df1.shape[0] == 0:
-                    raise ValueError(f"Table {table_name1} doesn't have any data")
-
-                df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
-
-                if ds_dict1["primary_key"].lower() not in df1.columns.tolist():
-                    raise ValueError(
-                        f"Primary key {ds_dict1['primary_key'].lower()} not present in {table_name1}"
-                    )
-
-                df2 = self.get_table_data(
-                    datasource=datasource2,
-                    query_expr=build_filter_query_expression(
-                        df1, ds_dict1["primary_key"].lower()
-                    ),
-                )
+            exclude_columns = (
+                ds_config["exclude_columns"] if "exclude_columns" in ds_config else []
+            )
+            if isinstance(exclude_columns, str):
+                exclude_columns = [exclude_columns]
+            exclude_columns_lol.append(exclude_columns)
+
+            if "primary_key" in ds_config:
+                if (
+                    isinstance(ds_config["primary_key"], list)
+                    and len(ds_config["primary_key"]) > 1
+                ):
+                    raise ValueError("Composite primary key is not supported yet")
+                primary_keys = primary_keys.union({ds_config["primary_key"]})
 
-                df2 = df2.rename(columns={c: c.lower() for c in df2.columns})
+        if len(primary_keys) == 0:
+            raise TulonaMissingPrimaryKeyError(
+                "Primary key must be provided with at least one of the data source config"
+            )
 
-                if ds_dict2["primary_key"].lower() not in df2.columns.tolist():
-                    raise ValueError(
-                        f"Primary key {ds_dict2['primary_key'].lower()} not present in {table_name2}"
-                    )
-
-                if df2.shape[0] > 0:
-                    df1 = df1[
-                        df1[ds_dict1["primary_key"].lower()].isin(
-                            df2[ds_dict1["primary_key"].lower()].tolist()
-                        )
-                    ]
-                    break
-
-                else:
-                    datasource2, datasource1 = self.datasources
-                    dbtype1 = self.profile["profiles"][
-                        extract_profile_name(self.project, datasource1)
-                    ]["type"]
-                    dbtype2 = self.profile["profiles"][
-                        extract_profile_name(self.project, datasource2)
-                    ]["type"]
-                    table_name1 = extract_table_name_from_config(
-                        config=ds_dict1, dbtype=dbtype1
-                    )
-                    table_name2 = extract_table_name_from_config(
-                        config=ds_dict2, dbtype=dbtype2
-                    )
+        if len(primary_keys) > 1:
+            raise ValueError(
+                "Primary key column name has to be same in all candidate tables for comparison"
+            )
+        primary_key = primary_keys.pop()
 
-                i += 1
+        # Config extraction
+        dbtype1, dbtype2 = dbtypes
+        table_fqn1, table_fqn2 = table_fqns
+        conman1, conman2 = connection_managers
+        exclude_columns1, exclude_columns2 = exclude_columns_lol
+
+        log.info("Extracting row data")
+        # TODO: push column exclusion down to the database/query
+        primary_key = primary_key.lower()
+        query_expr = None
+
+        i = 0
+        while i < 5:
+            log.debug(f"Extraction iteration: {i + 1}/5")
 
+            query1 = get_table_data_query(
+                conman1, dbtype1, table_fqn1, self.sample_count, query_expr
+            )
+            if self.sample_count < 51:
+                log.debug(f"Executing query: {query1}")
+            df1 = get_query_output_as_df(connection_manager=conman1, query_text=query1)
             if df1.shape[0] == 0:
-                raise ValueError(
-                    f"Could not find common data between {table_name1} and {table_name2}"
+                raise ValueError(f"Table {table_fqn1} doesn't have any data")
+
+            df1 = df1.rename(columns={c: c.lower() for c in df1.columns})
+            if primary_key not in df1.columns.tolist():
+                raise ValueError(f"Primary key {primary_key} not present in {table_fqn2}")
+
+            # Exclude columns
+            log.debug(f"Excluding columns from {table_fqn1}")
+            if len(exclude_columns1):
+                df1 = apply_column_exclusion(
+                    df1, primary_key, exclude_columns1, table_fqn1
                 )
-        else:
-            raise TulonaMissingPrimaryKeyError(
-                "Primary key is required for data comparison"
+
+            query2 = get_table_data_query(
+                conman2,
+                dbtype2,
+                table_fqn2,
+                self.sample_count,
+                query_expr=build_filter_query_expression(df1, primary_key),
             )
+            if self.sample_count < 51:
+                log.debug(f"Executing query: {query2}")
+            df2 = get_query_output_as_df(connection_manager=conman2, query_text=query2)
+            df2 = df2.rename(columns={c: c.lower() for c in df2.columns})
+
+            if primary_key not in df2.columns.tolist():
+                raise ValueError(f"Primary key {primary_key} not present in {table_fqn2}")
+
+            # Exclude columns
+            log.debug(f"Excluding columns from {table_fqn2}")
+            if len(exclude_columns2):
+                df2 = apply_column_exclusion(
+                    df2, primary_key, exclude_columns2, table_fqn2
+                )
 
-        # Exclude columns
-        log.debug("Excluding columns")
-        if "exclude_columns" in ds_dict1:
-            df1 = apply_column_exclusion(df1, ds_dict1, table_name1)
-        if "exclude_columns" in ds_dict2:
-            df2 = apply_column_exclusion(df2, ds_dict2, table_name2)
-
-        # Compare
-        common_columns = list(
-            set(df1.columns)
-            .intersection(set(df2.columns))
-            .union({ds_dict1["primary_key"].lower()})
-            .union({ds_dict2["primary_key"].lower()})
-        )
-        df1 = df1[common_columns].rename(
-            columns={c: c + "_" + datasource1.replace("_", "") for c in df1.columns}
-        )
-        df2 = df2[common_columns].rename(
-            columns={c: c + "_" + datasource2.replace("_", "") for c in df2.columns}
-        )
+            if df2.shape[0] > 0:
+                df1 = df1[df1[primary_key].isin(df2[primary_key].tolist())]
+                row_data_list = [df1, df2]
+                break
+            else:
+                query_expr = build_filter_query_expression(
+                    df1, primary_key, positive=False
+                )
 
-        ds1_compressed = datasource1.replace("_", "")
-        ds2_compressed = datasource2.replace("_", "")
+            i += 1
 
-        df_merge = pd.merge(
-            left=df1 if i % 2 == 0 else df2,
-            right=df2 if i % 2 == 0 else df1,
-            left_on=ds_dict1["primary_key"].lower() + "_" + ds1_compressed,
-            right_on=ds_dict2["primary_key"].lower() + "_" + ds2_compressed,
-            validate="one_to_one",
-        )
+        if df2.shape[0] == 0:
+            raise ValueError(
+                f"Could not find common data between {table_fqn1} and {table_fqn2}"
+            )
 
-        df_merge = df_merge[sorted(df_merge.columns.tolist())]
+        log.debug("Preparing row comparison")
+        df_row_comp = perform_comparison(
+            ds_name_compressed_list, row_data_list, primary_key
+        )
+        log.debug(f"Prepared comparision for {df_row_comp.shape[0]} rows")
 
-        outfile_fqn = self.get_outfile_fqn([ds1_compressed, ds2_compressed])
-        log.debug("Writing comparison result into: {outfile_fqn}")
-        df_merge.to_excel(outfile_fqn, sheet_name="Data Comparison", index=False)
+        log.debug(f"Writing comparison result into: {self.outfile_fqn}")
+        _ = create_dir_if_not_exist(self.project["outdir"])
+        with pd.ExcelWriter(
+            self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
+        ) as writer:
+            df_row_comp.to_excel(writer, sheet_name="Row Comparison", index=False)
 
         log.debug("Highlighting mismtach cells")
         highlight_mismatch_cells(
-            excel_file=outfile_fqn, sheet="Data Comparison", num_ds=len(self.datasources)
+            excel_file=self.outfile_fqn,
+            sheet="Row Comparison",
+            num_ds=len(self.datasources),
+            skip_columns=primary_key,
         )
 
         end_time = time.time()
-        log.info("Finished task: Compare")
+        log.info("------------------------ Finished task: compare-data")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
 
 
 @dataclass
 class CompareColumnTask(BaseTask):
     profile: Dict
     project: Dict
     runtime: RunConfig
     datasources: List[str]
+    outfile_fqn: Union[Path, str]
 
     def get_column_data(self, datasource, table, column):
         connection_profile = get_connection_profile(
             self.profile, self.project, datasource
         )
         conman = self.get_connection_manager(conn_profile=connection_profile)
 
@@ -233,25 +252,16 @@
         except Exception as exp:
             log.debug(f"Failed with error: {exp}")
             log.debug(f'Trying quoted column name: "{column}"')
             query = get_column_query(table, column, quoted=True)
             df = get_query_output_as_df(connection_manager=conman, query_text=query)
         return df
 
-    def write_result(self, df, ds1, ds2):
-        outdir = create_dir_if_not_exist(self.project["outdir"])
-        out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
-        outfile = f"{ds1}_{ds2}_column_comparison_{out_timestamp}.xlsx"
-        outfile_fqn = Path(outdir, outfile)
-
-        log.debug(f"Writing output into: {outfile_fqn}")
-        df.to_excel(outfile_fqn, sheet_name="Column Comparison", index=False)
-
     def execute(self):
-        log.info("Starting task: compare-column")
+        log.info("------------------------ Starting task: compare-column")
         start_time = time.time()
 
         if len(self.datasources) != 2:
             raise ValueError("Comparison works between two entities, not more, not less.")
 
         datasource1, datasource2 = self.datasources
         if ":" in datasource1 and ":" in datasource2:
@@ -316,19 +326,83 @@
 
         df_merge = pd.merge(
             left=df1,
             right=df2,
             left_on=column1,
             right_on=column2,
             how="outer",
-            suffixes=["_left_" + ds1_compressed, "_right_" + ds2_compressed],
+            suffixes=("_left_" + ds1_compressed, "_right_" + ds2_compressed),
             validate="one_to_one",
             indicator="presence",
         )
         df_merge = df_merge[df_merge["presence"] != "both"]
+        log.debug(f"Found {df_merge.shape[0]} extra values both side combined")
 
-        log.debug("Writing comparison result")
-        self.write_result(df_merge, ds1_compressed, ds2_compressed)
+        log.debug(f"Writing output into: {self.outfile_fqn}")
+        _ = create_dir_if_not_exist(self.project["outdir"])
+        with pd.ExcelWriter(
+            self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
+        ) as writer:
+            df_merge.to_excel(writer, sheet_name="Column Comparison", index=False)
 
         end_time = time.time()
-        log.info("Finished task: compare-column")
+        log.info("------------------------ Finished task: compare-column")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
+
+
+@dataclass
+class CompareTask(BaseTask):
+    profile: Dict
+    project: Dict
+    runtime: RunConfig
+    datasources: List[str]
+    outfile_fqn: Union[Path, str]
+    sample_count: int = DEFAULT_VALUES["sample_count"]
+
+    # Support for default values
+    def __post_init__(self):
+        for field in fields(self):
+            # If there is a default and the value of the field is none we can assign a value
+            if (
+                not isinstance(field.default, _MISSING_TYPE)
+                and getattr(self, field.name) is None
+            ):
+                setattr(self, field.name, field.default)
+
+    def execute(self):
+        log.info("------------------------ Starting task: compare")
+        start_time = time.time()
+
+        # Metadata comparison
+        ProfileTask(
+            profile=self.profile,
+            project=self.project,
+            runtime=self.runtime,
+            datasources=self.datasources,
+            outfile_fqn=self.outfile_fqn,
+            compare=True,
+        ).execute()
+
+        # Row comparison
+        CompareDataTask(
+            profile=self.profile,
+            project=self.project,
+            runtime=self.runtime,
+            datasources=self.datasources,
+            outfile_fqn=self.outfile_fqn,
+            sample_count=self.sample_count,
+        ).execute()
+
+        # Column comparison
+        CompareColumnTask(
+            profile=self.profile,
+            project=self.project,
+            runtime=self.runtime,
+            datasources=self.datasources,
+            outfile_fqn=self.outfile_fqn,
+        ).execute()
+
+        end_time = time.time()
+        log.info("------------------------ Finished task: compare")
+        log.info(
+            f"Total time taken [profile, compare-data, compare-column]: {(end_time - start_time):.2f} seconds"
+        )
```

### Comparing `tulona-0.2.6/core/tulona/task/ping.py` & `tulona-0.3.0/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/task/scan.py` & `tulona-0.3.0/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/util/database.py` & `tulona-0.3.0/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/util/excel.py` & `tulona-0.3.0/core/tulona/util/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         right=Side(border_style="thin"),
         top=Side(border_style="thin"),
         bottom=Side(border_style="thin"),
     )
 
     if skip_columns:
         skip_columns = skip_columns if isinstance(skip_columns, list) else [skip_columns]
-        skip_idxs = [get_column_index(ws, c) - 1 for c in skip_columns]
+        skip_idxs = [get_column_index(ws, c.lower()) - 1 for c in skip_columns]
         compareable_col_idxs = list(set(range(ws.max_column)) - set(skip_idxs))
     else:
         compareable_col_idxs = list(range(ws.max_column))
 
     for row in ws.iter_rows(
         min_row=2, min_col=0, max_row=ws.max_row, max_col=ws.max_column
     ):
```

### Comparing `tulona-0.2.6/core/tulona/util/filesystem.py` & `tulona-0.3.0/core/tulona/util/filesystem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from datetime import datetime
 from pathlib import Path
-from typing import Union
+from typing import List, Union
 
 
 def path_exists(p: Union[str, Path]) -> bool:
     return Path(p).exists()
 
 
 def recursive_rmdir(directory):
@@ -33,7 +34,14 @@
 def get_output_base_dir(base: str) -> Path:
     return create_or_replace_dir(base)
 
 
 def get_result_dir(dir_dict: dict, base: Union[str, Path], key: str) -> Path:
     p = Path(get_output_base_dir(base), dir_dict[key])
     return create_or_replace_dir(p)
+
+
+def get_outfile_fqn(outdir: str, ds_list: List[str], infix: str):
+    out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+    outfile = f"{'_'.join(ds_list)}_{infix}_{out_timestamp}.xlsx"
+    outfile_fqn = Path(outdir, outfile)
+    return outfile_fqn
```

### Comparing `tulona-0.2.6/core/tulona/util/profiles.py` & `tulona-0.3.0/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.6/core/tulona/util/sql.py` & `tulona-0.3.0/core/tulona/util/sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import Dict
 
 import pandas as pd
 
 from tulona.exceptions import TulonaNotImplementedError
 
 
+def get_table_fqn(database: str, schema: str, table: str) -> str:
+    table_fqn = f"{database + '.' if database else ''}{schema}.{table}"
+    return table_fqn
+
+
 def get_sample_row_query(dbtype: str, table_name: str, sample_count: int):
     dbtype = dbtype.lower()
 
     # TODO: validate sampling mechanism for maximum possible randomness
     if dbtype in ["snowflake", "mssql"]:
         query = f"select * from {table_name} tablesample ({sample_count} rows)"
     elif dbtype == "postgres":
@@ -36,22 +41,24 @@
 
 def get_query_output_as_df(connection_manager, query_text: str):
     with connection_manager.engine.connect() as conn:
         df = pd.read_sql_query(query_text, conn)
     return df
 
 
-def build_filter_query_expression(df: pd.DataFrame, primary_key: str):
+def build_filter_query_expression(
+    df: pd.DataFrame, primary_key: str, positive: bool = True
+):
     primary_keys = df[primary_key].tolist()
 
     if "int" in str(df[primary_key].dtype):
         primary_keys = [str(k) for k in primary_keys]
-        query_expr = f"""{primary_key} in ({", ".join(primary_keys)})"""
+        query_expr = f"""{primary_key}{'' if positive else ' not'} in ({", ".join(primary_keys)})"""
     else:
-        query_expr = f"""{primary_key} in ('{"', '".join(primary_keys)}')"""
+        query_expr = f"""{primary_key}{'' if positive else ' not'} in ('{"', '".join(primary_keys)}')"""
 
     return query_expr
 
 
 def get_metadata_query(database, schema, table):
     if database:
         query = f"""
@@ -65,17 +72,15 @@
         select * from information_schema.columns
         where upper(table_schema) = '{schema.upper()}'
         and upper(table_name) = '{table.upper()}'
         """
     return query
 
 
-def get_metric_query(
-    database, schema, table, columns_dtype: Dict, metrics: list, quoted=False
-):
+def get_metric_query(table_fqn, columns_dtype: Dict, metrics: list, quoted=False):
     numeric_types = [
         "smallint",
         "integer",
         "bigint",
         "decimal",
         "numeric",
         "real",
@@ -150,16 +155,24 @@
                 qp.append(
                     function_map[m.lower()].format(f'"{col}"' if quoted else col, col)
                 )
             else:
                 qp.append(f"'NA' as {col}_{m.lower()}")
         call_funcs.extend(qp)
 
-    table_fqn = f"{database if database else ''}{'.' if database else ''}{schema}.{table}"
-
     query = f"""
     select
         {", ".join(call_funcs)}
     from {table_fqn}
     """
 
     return query
+
+
+def get_table_data_query(conman, dbtype, table_fqn, sample_count, query_expr: str = None):
+    if query_expr:
+        query = f"select * from {table_fqn} where {query_expr}"
+    else:
+        query = get_sample_row_query(
+            dbtype=dbtype, table_name=table_fqn, sample_count=sample_count
+        )
+    return query
```

### Comparing `tulona-0.2.6/core/tulona.egg-info/PKG-INFO` & `tulona-0.3.0/core/tulona.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.2.6
+Version: 0.3.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -129,56 +129,62 @@
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
 
-* **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
+* **ping**: To test connectivity to the databases for the datasources. Sample command:
 
-  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
+  * To ping one data source pass the name to the `--datasources` parameter:
 
-    ``tulona compare-column --datasources employee_postgres,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
+    ``tulona ping --datasources employee_postgres``
 
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
+  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
 
-    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
+    ``tulona ping --datasources employee_postgres,employee_mysql``
 
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
+* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+
+  * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
+
+    ``tulona profile --datasources employee_postgres,employee_mysql``
+  * Profiling with `--compare` flag. It will produce a comparison view (side by side):
+
+    ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
 * **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
-* **ping**: To test connectivity to the databases for the datasources. Sample command:
+* **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
-  * To ping one data source pass the name to the `--datasources` parameter:
+  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
 
-    ``tulona ping --datasources employee_postgres``
+    ``tulona compare-column --datasources employee_postgres,employee_mysql``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
 
-  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
+    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
 
-    ``tulona ping --datasources employee_postgres,employee_mysql``
+    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
+  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
 
-* **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
+    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
 
-  * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
+* **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
-    ``tulona profile --datasources employee_postgres,employee_mysql``
-  * Profiling with `--compare` flag. It will produce a comparison view (side by side):
+  ``tulona compare --datasources employee_postgres,employee_mysql``
 
-    ``tulona profile --compare --datasources employee_postgres,employee_mysql``
+For debug level log, add `-v` or `--verbose` flag along with any command. For example: ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Development Environment Setup
 -----------------------------
 * For live installation execute `pip install --editable core`.
@@ -193,16 +199,16 @@
 * Execute `pip install <wheel-file.whl>`
 
 
 .. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
 .. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
-.. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
-   :target: https://codecov.io/gh/mrinalsardar/tulona
+.. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/mrinalsardar/tulona/branch/main
    :alt: Coverage status
 .. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
    :target: https://pypi.python.org/pypi/tulona/
 .. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
    :target: https://pypi.org/project/tulona/
 .. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
    :target: http://www.apache.org/licenses/LICENSE-2.0.txt
```

### Comparing `tulona-0.2.6/core/tulona.egg-info/SOURCES.txt` & `tulona-0.3.0/core/tulona.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 core/tulona/cli/params.py
 core/tulona/config/__init__.py
 core/tulona/config/profile.py
 core/tulona/config/project.py
 core/tulona/config/runtime.py
 core/tulona/task/base.py
 core/tulona/task/compare.py
+core/tulona/task/helper.py
 core/tulona/task/ping.py
 core/tulona/task/profile.py
 core/tulona/task/scan.py
 core/tulona/util/__init__.py
 core/tulona/util/database.py
 core/tulona/util/dataframe.py
 core/tulona/util/excel.py
```

### Comparing `tulona-0.2.6/pyproject.toml` & `tulona-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.2.6"
+version = "0.3.0"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -96,15 +96,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.2.6"
+current_version = "0.3.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

