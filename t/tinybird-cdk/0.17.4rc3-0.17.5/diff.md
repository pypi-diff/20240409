# Comparing `tmp/tinybird-cdk-0.17.4rc3.tar.gz` & `tmp/tinybird-cdk-0.17.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.17.4rc3.tar", last modified: Fri Sep  1 11:13:59 2023, max compression
+gzip compressed data, was "tinybird-cdk-0.17.5.tar", last modified: Tue Apr  9 10:52:23 2024, max compression
```

## Comparing `tinybird-cdk-0.17.4rc3.tar` & `tinybird-cdk-0.17.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:59.525584 tinybird-cdk-0.17.4rc3/
--rw-r--r--   0 runner    (1001) docker     (999)      316 2023-09-01 11:13:59.525584 tinybird-cdk-0.17.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    25352 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 11:13:59.525584 tinybird-cdk-0.17.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      801 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:59.517583 tinybird-cdk-0.17.4rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     1970 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:59.521583 tinybird-cdk-0.17.4rc3/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (999)      423 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:59.521583 tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (999)     1450 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2025 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (999)     1474 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (999)     4159 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (999)     4946 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (999)      764 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     7729 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:59.525584 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10438 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (999)      320 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (999)      671 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (999)     1657 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (999)     2152 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (999)      318 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (999)    17899 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (999)     1595 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (999)     2831 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)      840 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (999)      514 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (999)      515 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (999)     3694 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/migration.py
--rw-r--r--   0 runner    (1001) docker     (999)     5546 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (999)    12911 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (999)      237 2023-09-01 11:13:48.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 11:13:59.521583 tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      316 2023-09-01 11:13:59.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      934 2023-09-01 11:13:59.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 11:13:59.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      181 2023-09-01 11:13:59.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       13 2023-09-01 11:13:59.000000 tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25352 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.327281 tinybird-cdk-0.17.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.331281 tinybird-cdk-0.17.5/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.331281 tinybird-cdk-0.17.5/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.17.4rc3/README.md` & `tinybird-cdk-0.17.5/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/setup.py` & `tinybird-cdk-0.17.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tinybird-cdk',
-    version='0.17.4rc3',
+    version='0.17.5',
     description="Tinybird's Connector Development Kit.",
     long_description='This package is under active development and currently meant for internal use only.',
     long_description_content_type='text/markdown',
     author='tinybird.co',
     author_email="support@tinybird.co",
     python_requires='>=3.8, <3.12',
     install_requires=[
```

### Comparing `tinybird-cdk-0.17.4rc3/tests/test_gcp.py` & `tinybird-cdk-0.17.5/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/__init__.py` & `tinybird-cdk-0.17.5/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/abstract_client.py` & `tinybird-cdk-0.17.5/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/gcp.py` & `tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/gcs.py` & `tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/cloud/s3.py` & `tinybird-cdk-0.17.5/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/config.py` & `tinybird-cdk-0.17.5/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connector.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/bigquery.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/kinesis.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/mysql.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/postgresql.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/snowflake.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/connectors/sqlite.py` & `tinybird-cdk-0.17.5/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/errors.py` & `tinybird-cdk-0.17.5/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/export.py` & `tinybird-cdk-0.17.5/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/formats.py` & `tinybird-cdk-0.17.5/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/logger.py` & `tinybird-cdk-0.17.5/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/migration.py` & `tinybird-cdk-0.17.5/tinybird_cdk/migration.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/schema.py` & `tinybird-cdk-0.17.5/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk/tinybird.py` & `tinybird-cdk-0.17.5/tinybird_cdk/tinybird.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.4rc3/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird-cdk-0.17.5/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

