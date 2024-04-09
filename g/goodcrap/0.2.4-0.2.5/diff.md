# Comparing `tmp/goodcrap-0.2.4.tar.gz` & `tmp/goodcrap-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodcrap-0.2.4.tar", last modified: Thu Feb  8 01:52:42 2024, max compression
+gzip compressed data, was "goodcrap-0.2.5.tar", last modified: Tue Apr  9 03:47:37 2024, max compression
```

## Comparing `goodcrap-0.2.4.tar` & `goodcrap-0.2.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.181805 goodcrap-0.2.4/
--rw-rw-rw-   0        0        0      388 2024-02-08 01:10:04.000000 goodcrap-0.2.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-05-25 04:23:50.000000 goodcrap-0.2.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0    35803 2023-05-25 04:23:50.000000 goodcrap-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      193 2023-05-25 04:23:50.000000 goodcrap-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0    12838 2024-02-08 01:52:42.176804 goodcrap-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    12273 2023-05-25 04:23:50.000000 goodcrap-0.2.4/README.md
--rw-rw-rw-   0        0        0        5 2024-02-08 01:09:12.000000 goodcrap-0.2.4/VERSION
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.768802 goodcrap-0.2.4/goodcrap/
--rw-rw-rw-   0        0        0       87 2024-02-08 01:09:07.000000 goodcrap-0.2.4/goodcrap/__init__.py
--rw-rw-rw-   0        0        0       72 2024-02-08 01:10:47.000000 goodcrap-0.2.4/goodcrap/__main__.py
--rw-rw-rw-   0        0        0     5953 2023-05-31 21:12:16.000000 goodcrap-0.2.4/goodcrap/cli.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.863819 goodcrap-0.2.4/goodcrap/crappers/
--rw-rw-rw-   0        0        0     1019 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/crappers/__init__.py
--rw-rw-rw-   0        0        0     3935 2024-02-07 22:47:01.000000 goodcrap-0.2.4/goodcrap/crappers/queries.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.883836 goodcrap-0.2.4/goodcrap/data_warehouses/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/data_warehouses/__init__.py
--rw-rw-rw-   0        0        0     2283 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/data_warehouses/dimension_featurizer.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.965802 goodcrap-0.2.4/goodcrap/databases/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/databases/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/databases/database.py
--rw-rw-rw-   0        0        0      532 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/databases/mysql.py
--rw-rw-rw-   0        0        0      194 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/databases/queries.py
--rw-rw-rw-   0        0        0     3915 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/databases/snowflake.py
--rw-rw-rw-   0        0        0      379 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/databases/sqlite.py
--rw-rw-rw-   0        0        0     1508 2024-02-08 01:10:34.000000 goodcrap-0.2.4/goodcrap/fairker.py
--rw-rw-rw-   0        0        0    15620 2024-02-07 22:00:04.000000 goodcrap-0.2.4/goodcrap/goodcrap.py
--rw-rw-rw-   0        0        0     1362 2024-02-07 22:41:13.000000 goodcrap-0.2.4/goodcrap/imitator.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.992800 goodcrap-0.2.4/goodcrap/pipelines/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/pipelines/__init__.py
--rw-rw-rw-   0        0        0     3608 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/pipelines/mage.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.046839 goodcrap-0.2.4/goodcrap/pipelines/templates/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/pipelines/templates/__init__.py
--rw-rw-rw-   0        0        0     1122 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/pipelines/templates/data_exporter_mysql.py
--rw-rw-rw-   0        0        0      683 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/pipelines/templates/data_loader.py
--rw-rw-rw-   0        0        0      832 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/pipelines/templates/metadata.yaml
--rw-rw-rw-   0        0        0     2508 2023-05-31 21:12:16.000000 goodcrap-0.2.4/goodcrap/random_mapper.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.051840 goodcrap-0.2.4/goodcrap/templates/
--rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.057840 goodcrap-0.2.4/goodcrap/templates/__pycache__/
--rw-rw-rw-   0        0        0      159 2023-05-31 22:16:52.000000 goodcrap-0.2.4/goodcrap/templates/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.085803 goodcrap-0.2.4/goodcrap/templates/data_warehouses/
--rw-rw-rw-   0        0        0     4198 2023-05-31 21:12:16.000000 goodcrap-0.2.4/goodcrap/templates/data_warehouses/sales.crap_labels.json
--rw-rw-rw-   0        0        0     3553 2023-05-31 21:12:16.000000 goodcrap-0.2.4/goodcrap/templates/data_warehouses/sales.sql
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.595802 goodcrap-0.2.4/goodcrap/templates/databases/
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.115806 goodcrap-0.2.4/goodcrap/templates/databases/customers_orders/
--rw-rw-rw-   0        0        0      751 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json
--rw-rw-rw-   0        0        0      912 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/databases/customers_orders/customers_orders.sql
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:41.597804 goodcrap-0.2.4/goodcrap/templates/tables/
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.141804 goodcrap-0.2.4/goodcrap/templates/tables/customers/
--rw-rw-rw-   0        0        0      562 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/tables/customers/customers.crap_labels.json
--rw-rw-rw-   0        0        0      457 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/tables/customers/customers.sql
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.167803 goodcrap-0.2.4/goodcrap/templates/tables/orders/
--rw-rw-rw-   0        0        0      244 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/tables/orders/orders.crap_labels.json
--rw-rw-rw-   0        0        0      451 2023-05-25 04:23:50.000000 goodcrap-0.2.4/goodcrap/templates/tables/orders/orders.sql
-drwxrwxrwx   0        0        0        0 2024-02-08 01:52:42.174820 goodcrap-0.2.4/goodcrap.egg-info/
--rw-rw-rw-   0        0        0    12838 2024-02-08 01:52:41.000000 goodcrap-0.2.4/goodcrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2024-02-08 01:52:41.000000 goodcrap-0.2.4/goodcrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 01:52:41.000000 goodcrap-0.2.4/goodcrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-02-08 01:52:41.000000 goodcrap-0.2.4/goodcrap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2024-02-08 01:52:41.000000 goodcrap-0.2.4/goodcrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-08 01:52:41.000000 goodcrap-0.2.4/goodcrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2024-02-08 01:52:42.188803 goodcrap-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1162 2023-05-25 04:23:50.000000 goodcrap-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.549612 goodcrap-0.2.5/
+-rw-rw-rw-   0        0        0      442 2024-04-09 03:46:27.000000 goodcrap-0.2.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-05-25 04:23:50.000000 goodcrap-0.2.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0    35803 2023-05-25 04:23:50.000000 goodcrap-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-05-25 04:23:50.000000 goodcrap-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    12838 2024-04-09 03:47:37.547599 goodcrap-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12273 2023-05-25 04:23:50.000000 goodcrap-0.2.5/README.md
+-rw-rw-rw-   0        0        0        5 2024-04-09 03:46:37.000000 goodcrap-0.2.5/VERSION
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.407602 goodcrap-0.2.5/goodcrap/
+-rw-rw-rw-   0        0        0       87 2024-04-09 03:46:59.000000 goodcrap-0.2.5/goodcrap/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-02-08 01:10:47.000000 goodcrap-0.2.5/goodcrap/__main__.py
+-rw-rw-rw-   0        0        0     5953 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.447603 goodcrap-0.2.5/goodcrap/crappers/
+-rw-rw-rw-   0        0        0     1019 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/crappers/__init__.py
+-rw-rw-rw-   0        0        0     3935 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/crappers/queries.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.452602 goodcrap-0.2.5/goodcrap/data_warehouses/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/data_warehouses/__init__.py
+-rw-rw-rw-   0        0        0     2283 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/data_warehouses/dimension_featurizer.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.469602 goodcrap-0.2.5/goodcrap/databases/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/databases/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/databases/database.py
+-rw-rw-rw-   0        0        0      532 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/databases/mysql.py
+-rw-rw-rw-   0        0        0      194 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/databases/queries.py
+-rw-rw-rw-   0        0        0     3915 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/databases/snowflake.py
+-rw-rw-rw-   0        0        0      379 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/databases/sqlite.py
+-rw-rw-rw-   0        0        0     1981 2024-02-11 13:27:19.000000 goodcrap-0.2.5/goodcrap/fairker.py
+-rw-rw-rw-   0        0        0    15620 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/goodcrap.py
+-rw-rw-rw-   0        0        0     1362 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/imitator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.474620 goodcrap-0.2.5/goodcrap/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     3608 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/pipelines/mage.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.487601 goodcrap-0.2.5/goodcrap/pipelines/templates/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/pipelines/templates/__init__.py
+-rw-rw-rw-   0        0        0     1122 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/pipelines/templates/data_exporter_mysql.py
+-rw-rw-rw-   0        0        0      683 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/pipelines/templates/data_loader.py
+-rw-rw-rw-   0        0        0      832 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/pipelines/templates/metadata.yaml
+-rw-rw-rw-   0        0        0     2508 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/random_mapper.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.489599 goodcrap-0.2.5/goodcrap/templates/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.492599 goodcrap-0.2.5/goodcrap/templates/__pycache__/
+-rw-rw-rw-   0        0        0      159 2023-05-31 22:16:52.000000 goodcrap-0.2.5/goodcrap/templates/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.499600 goodcrap-0.2.5/goodcrap/templates/data_warehouses/
+-rw-rw-rw-   0        0        0     4198 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/templates/data_warehouses/sales.crap_labels.json
+-rw-rw-rw-   0        0        0     3553 2024-02-10 12:35:38.000000 goodcrap-0.2.5/goodcrap/templates/data_warehouses/sales.sql
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.350599 goodcrap-0.2.5/goodcrap/templates/databases/
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.513600 goodcrap-0.2.5/goodcrap/templates/databases/customers_orders/
+-rw-rw-rw-   0        0        0      751 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json
+-rw-rw-rw-   0        0        0      912 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/databases/customers_orders/customers_orders.sql
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.351598 goodcrap-0.2.5/goodcrap/templates/tables/
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.528599 goodcrap-0.2.5/goodcrap/templates/tables/customers/
+-rw-rw-rw-   0        0        0      562 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/tables/customers/customers.crap_labels.json
+-rw-rw-rw-   0        0        0      457 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/tables/customers/customers.sql
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.541598 goodcrap-0.2.5/goodcrap/templates/tables/orders/
+-rw-rw-rw-   0        0        0      244 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/tables/orders/orders.crap_labels.json
+-rw-rw-rw-   0        0        0      451 2023-05-25 04:23:50.000000 goodcrap-0.2.5/goodcrap/templates/tables/orders/orders.sql
+drwxrwxrwx   0        0        0        0 2024-04-09 03:47:37.545601 goodcrap-0.2.5/goodcrap.egg-info/
+-rw-rw-rw-   0        0        0    12838 2024-04-09 03:47:37.000000 goodcrap-0.2.5/goodcrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2024-04-09 03:47:37.000000 goodcrap-0.2.5/goodcrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:47:37.000000 goodcrap-0.2.5/goodcrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-09 03:47:37.000000 goodcrap-0.2.5/goodcrap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2024-04-09 03:47:37.000000 goodcrap-0.2.5/goodcrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 03:47:37.000000 goodcrap-0.2.5/goodcrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      215 2024-04-09 03:47:37.558598 goodcrap-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-05-25 04:23:50.000000 goodcrap-0.2.5/setup.py
```

### Comparing `goodcrap-0.2.4/CONTRIBUTING.rst` & `goodcrap-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/LICENSE` & `goodcrap-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/PKG-INFO` & `goodcrap-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodcrap
-Version: 0.2.4
+Version: 0.2.5
 Summary: goodcrap creates tables, databases and csv files and fill them with random data
 Home-page: https://github.com/goodcrap/goodcrap
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: gpl-3.0
 Keywords: ai,data engineering,fake data,data science
 Description-Content-Type: text/markdown
```

### Comparing `goodcrap-0.2.4/README.md` & `goodcrap-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/cli.py` & `goodcrap-0.2.5/goodcrap/cli.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/crappers/__init__.py` & `goodcrap-0.2.5/goodcrap/crappers/__init__.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/crappers/queries.py` & `goodcrap-0.2.5/goodcrap/crappers/queries.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/data_warehouses/dimension_featurizer.py` & `goodcrap-0.2.5/goodcrap/data_warehouses/dimension_featurizer.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/databases/database.py` & `goodcrap-0.2.5/goodcrap/databases/database.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/databases/mysql.py` & `goodcrap-0.2.5/goodcrap/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/databases/snowflake.py` & `goodcrap-0.2.5/goodcrap/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/fairker.py` & `goodcrap-0.2.5/goodcrap/fairker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 import random
 from faker import Faker as Unfairker
-fake = Unfairker()
 
 
 names_male = [
     "Ahmed",
     "Adam",
     "Alaa",
     "Ali",
     "Adham",
     "Abdulwahab",
     "Abdullah",
     "Abdallah",
     "Adeeb",
     "Adel",
+    "Asim",
+    "Ajay",
+    "Bilal",
     "Basem",
     "Basim",
     "Ibrahim",
+    "Imran",
     "Ismael",
     "Ismail",
     "Idris",
     "Loai",
     "Labib",
+    "Laxmi",
     "Mohamed",
     "Mahmoud",
     "Mehmed",
     "Mounir",
     "Moneer",
     "Mazen",
     "Mazin",
     "Mamdouh",
+    "Mansoor",
+    "Mandeep",
+    "Nadeem",
+    "Rahul",
+    "Ravi",
+    "Rohan",
+    "Sameh",
+    "Sameeh",
+    "Samir",
     "Tamir",
     "Tahir",
     "Taher",
+    "Tanveer",
+    "Tariq",
     "Zayn",
     "Zain",
     "Zakaria",
     "Zaki",
     "Zekri",
-    "Zaker"
+    "Zaker",
 ]
 
 
 names_female = [
     "Aya",
     "Basma",
     "Dina",
@@ -63,27 +78,43 @@
     "Raneem",
     "Rana",
     "Sarah",
     "Seham",
     "Sondos",
     "Sanaa",
     "Zeina",
+    "Nida",
+    "Sarah",
+    "Nabeela",
+    "Romana",
+    "Fiza",
+    "Aliza",
+    "Anaya",
+    "Pooja",
+    "Ananya",
+    "Devi",
+    "Jhangvi",
+    "Sonam",
+    "Riya",
 ]
 
-class Faker:
+
+class Faker(Unfairker):
     def first_name_male(self):
-        if random.random()>0.5:
-            return random.sample(names_male,1)[0]
+        if random.random() > 0.5:
+            return random.sample(names_male, 1)[0]
         else:
-            return fake.first_name_male()
+            return super().__getattr__('first_name_male')()
+        
     def first_name_female(self):
-        if random.random()>0.5:
-            return random.sample(names_female,1)[0]
+        if random.random() > 0.5:
+            return random.sample(names_female, 1)[0]
         else:
-            return fake.first_name_female()
+            return super().__getattr__('first_name_female')()
+        
     def first_name(self):
-        if random.random()>0.5:
+        if random.random() > 0.5:
             return self.first_name_male()
         else:
             return self.first_name_female()
         
-        
+
```

### Comparing `goodcrap-0.2.4/goodcrap/goodcrap.py` & `goodcrap-0.2.5/goodcrap/goodcrap.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/imitator.py` & `goodcrap-0.2.5/goodcrap/imitator.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/pipelines/mage.py` & `goodcrap-0.2.5/goodcrap/pipelines/mage.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/pipelines/templates/data_exporter_mysql.py` & `goodcrap-0.2.5/goodcrap/pipelines/templates/data_exporter_mysql.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/pipelines/templates/data_loader.py` & `goodcrap-0.2.5/goodcrap/pipelines/templates/data_loader.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/pipelines/templates/metadata.yaml` & `goodcrap-0.2.5/goodcrap/pipelines/templates/metadata.yaml`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/random_mapper.py` & `goodcrap-0.2.5/goodcrap/random_mapper.py`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/templates/data_warehouses/sales.crap_labels.json` & `goodcrap-0.2.5/goodcrap/templates/data_warehouses/sales.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/templates/data_warehouses/sales.sql` & `goodcrap-0.2.5/goodcrap/templates/data_warehouses/sales.sql`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json` & `goodcrap-0.2.5/goodcrap/templates/databases/customers_orders/customers_orders.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/templates/databases/customers_orders/customers_orders.sql` & `goodcrap-0.2.5/goodcrap/templates/databases/customers_orders/customers_orders.sql`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap/templates/tables/customers/customers.crap_labels.json` & `goodcrap-0.2.5/goodcrap/templates/tables/customers/customers.crap_labels.json`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/goodcrap.egg-info/PKG-INFO` & `goodcrap-0.2.5/goodcrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodcrap
-Version: 0.2.4
+Version: 0.2.5
 Summary: goodcrap creates tables, databases and csv files and fill them with random data
 Home-page: https://github.com/goodcrap/goodcrap
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: gpl-3.0
 Keywords: ai,data engineering,fake data,data science
 Description-Content-Type: text/markdown
```

### Comparing `goodcrap-0.2.4/goodcrap.egg-info/SOURCES.txt` & `goodcrap-0.2.5/goodcrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goodcrap-0.2.4/setup.py` & `goodcrap-0.2.5/setup.py`

 * *Files identical despite different names*

