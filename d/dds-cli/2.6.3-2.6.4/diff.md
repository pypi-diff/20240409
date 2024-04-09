# Comparing `tmp/dds_cli-2.6.3.tar.gz` & `tmp/dds_cli-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dds_cli-2.6.3.tar", last modified: Wed Feb 28 12:10:53 2024, max compression
+gzip compressed data, was "dds_cli-2.6.4.tar", last modified: Tue Apr  9 14:34:47 2024, max compression
```

## Comparing `dds_cli-2.6.3.tar` & `dds_cli-2.6.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:10:53.595829 dds_cli-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-28 12:10:22.000000 dds_cli-2.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-02-28 12:10:53.595829 dds_cli-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-02-28 12:10:22.000000 dds_cli-2.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:10:53.591829 dds_cli-2.6.3/dds_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76813 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/custom_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/data_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/data_lister.py
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/data_putter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/data_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/file_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/file_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/file_handler_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/file_handler_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/motd_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/project_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/project_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/project_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/superadmin_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/text_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/unit_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-28 12:10:22.000000 dds_cli-2.6.3/dds_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:10:53.595829 dds_cli-2.6.3/dds_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-02-28 12:10:53.000000 dds_cli-2.6.3/dds_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-28 12:10:53.000000 dds_cli-2.6.3/dds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 12:10:53.000000 dds_cli-2.6.3/dds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-28 12:10:53.000000 dds_cli-2.6.3/dds_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 12:10:40.000000 dds_cli-2.6.3/dds_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-28 12:10:53.000000 dds_cli-2.6.3/dds_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-28 12:10:53.000000 dds_cli-2.6.3/dds_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-28 12:10:22.000000 dds_cli-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 12:10:53.595829 dds_cli-2.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-28 12:10:22.000000 dds_cli-2.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:10:53.591829 dds_cli-2.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_data_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_file_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_file_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_file_handler_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_motd_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19224 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_project_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_superadmin_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-02-28 12:10:22.000000 dds_cli-2.6.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:34:47.057905 dds_cli-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-09 14:34:11.000000 dds_cli-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-09 14:34:47.057905 dds_cli-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-09 14:34:11.000000 dds_cli-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:34:47.053905 dds_cli-2.6.4/dds_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76813 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/custom_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/data_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/data_lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/data_putter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/data_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/file_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/file_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/file_handler_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/file_handler_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/motd_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/project_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/project_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/project_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/superadmin_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/text_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/unit_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 14:34:11.000000 dds_cli-2.6.4/dds_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:34:47.057905 dds_cli-2.6.4/dds_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-09 14:34:46.000000 dds_cli-2.6.4/dds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 14:34:46.000000 dds_cli-2.6.4/dds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:34:46.000000 dds_cli-2.6.4/dds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 14:34:46.000000 dds_cli-2.6.4/dds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:34:33.000000 dds_cli-2.6.4/dds_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 14:34:46.000000 dds_cli-2.6.4/dds_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 14:34:46.000000 dds_cli-2.6.4/dds_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 14:34:11.000000 dds_cli-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:34:47.057905 dds_cli-2.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-09 14:34:11.000000 dds_cli-2.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:34:47.057905 dds_cli-2.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_data_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_file_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_file_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_file_handler_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_motd_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19224 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_project_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_superadmin_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-09 14:34:11.000000 dds_cli-2.6.4/tests/test_utils.py
```

### Comparing `dds_cli-2.6.3/LICENSE` & `dds_cli-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/PKG-INFO` & `dds_cli-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dds_cli
-Version: 2.6.3
+Version: 2.6.4
 Summary: A command line tool to manage data and projects in the SciLifeLab Data Delivery System.
 Home-page: https://github.com/ScilifelabDataCentre/dds_cli
 Author: SciLifeLab Data Centre
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -15,15 +15,15 @@
 License-File: LICENSE
 Requires-Dist: boto3==1.24.73
 Requires-Dist: botocore==1.27.73
 Requires-Dist: click==8.1.3
 Requires-Dist: click-pathlib==2020.3.13.0
 Requires-Dist: cryptography==42.0.4
 Requires-Dist: immutabledict==2.2.1
-Requires-Dist: jwcrypto==1.5.1
+Requires-Dist: jwcrypto==1.5.6
 Requires-Dist: prettytable==3.4.1
 Requires-Dist: prompt-toolkit==3.0.31
 Requires-Dist: PyNaCl==1.5.0
 Requires-Dist: pytz==2022.2.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: questionary==1.10.0
 Requires-Dist: requests==2.31.0
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dds_cli Version: 2.6.3 Summary: A command line tool
+Metadata-Version: 2.1 Name: dds_cli Version: 2.6.4 Summary: A command line tool
 to manage data and projects in the SciLifeLab Data Delivery System. Home-page:
 https://github.com/ScilifelabDataCentre/dds_cli Author: SciLifeLab Data Centre
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 boto3==1.24.73 Requires-Dist: botocore==1.27.73 Requires-Dist: click==8.1.3
 Requires-Dist: click-pathlib==2020.3.13.0 Requires-Dist: cryptography==42.0.4
-Requires-Dist: immutabledict==2.2.1 Requires-Dist: jwcrypto==1.5.1 Requires-
+Requires-Dist: immutabledict==2.2.1 Requires-Dist: jwcrypto==1.5.6 Requires-
 Dist: prettytable==3.4.1 Requires-Dist: prompt-toolkit==3.0.31 Requires-Dist:
 PyNaCl==1.5.0 Requires-Dist: pytz==2022.2.1 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: questionary==1.10.0 Requires-Dist: requests==2.31.0 Requires-
 Dist: rich==12.5.1 Requires-Dist: rich-click==1.5.2 Requires-Dist:
 simplejson==3.17.6 Requires-Dist: tzlocal==4.2 Requires-Dist: zstandard==0.19.0
                     ************ DDaattaa DDeelliivveerryy SSyysstteemm:: CCLLII ************
  AA ccoommmmaanndd lliinnee ttooooll ``ddddss`` ttoo mmaannaaggee pprroojjeeccttss aanndd ddaattaa iinn tthhee SScciiLLiiffeeLLaabb DDaattaa
```

### Comparing `dds_cli-2.6.3/README.md` & `dds_cli-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/__init__.py` & `dds_cli-2.6.4/dds_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/__main__.py` & `dds_cli-2.6.4/dds_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/account_manager.py` & `dds_cli-2.6.4/dds_cli/account_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/auth.py` & `dds_cli-2.6.4/dds_cli/auth.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/base.py` & `dds_cli-2.6.4/dds_cli/base.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/custom_decorators.py` & `dds_cli-2.6.4/dds_cli/custom_decorators.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/data_getter.py` & `dds_cli-2.6.4/dds_cli/data_getter.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/data_lister.py` & `dds_cli-2.6.4/dds_cli/data_lister.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/data_putter.py` & `dds_cli-2.6.4/dds_cli/data_putter.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/data_remover.py` & `dds_cli-2.6.4/dds_cli/data_remover.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/directory.py` & `dds_cli-2.6.4/dds_cli/directory.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/exceptions.py` & `dds_cli-2.6.4/dds_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/file_compressor.py` & `dds_cli-2.6.4/dds_cli/file_compressor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/file_encryptor.py` & `dds_cli-2.6.4/dds_cli/file_encryptor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/file_handler.py` & `dds_cli-2.6.4/dds_cli/file_handler.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/file_handler_local.py` & `dds_cli-2.6.4/dds_cli/file_handler_local.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/file_handler_remote.py` & `dds_cli-2.6.4/dds_cli/file_handler_remote.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/motd_manager.py` & `dds_cli-2.6.4/dds_cli/motd_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/options.py` & `dds_cli-2.6.4/dds_cli/options.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/project_creator.py` & `dds_cli-2.6.4/dds_cli/project_creator.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/project_info.py` & `dds_cli-2.6.4/dds_cli/project_info.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/project_status.py` & `dds_cli-2.6.4/dds_cli/project_status.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/s3_connector.py` & `dds_cli-2.6.4/dds_cli/s3_connector.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/status.py` & `dds_cli-2.6.4/dds_cli/status.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/superadmin_helper.py` & `dds_cli-2.6.4/dds_cli/superadmin_helper.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/text_handler.py` & `dds_cli-2.6.4/dds_cli/text_handler.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/timestamp.py` & `dds_cli-2.6.4/dds_cli/timestamp.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/unit_manager.py` & `dds_cli-2.6.4/dds_cli/unit_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/user.py` & `dds_cli-2.6.4/dds_cli/user.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli/utils.py` & `dds_cli-2.6.4/dds_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/dds_cli.egg-info/PKG-INFO` & `dds_cli-2.6.4/dds_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dds_cli
-Version: 2.6.3
+Version: 2.6.4
 Summary: A command line tool to manage data and projects in the SciLifeLab Data Delivery System.
 Home-page: https://github.com/ScilifelabDataCentre/dds_cli
 Author: SciLifeLab Data Centre
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -15,15 +15,15 @@
 License-File: LICENSE
 Requires-Dist: boto3==1.24.73
 Requires-Dist: botocore==1.27.73
 Requires-Dist: click==8.1.3
 Requires-Dist: click-pathlib==2020.3.13.0
 Requires-Dist: cryptography==42.0.4
 Requires-Dist: immutabledict==2.2.1
-Requires-Dist: jwcrypto==1.5.1
+Requires-Dist: jwcrypto==1.5.6
 Requires-Dist: prettytable==3.4.1
 Requires-Dist: prompt-toolkit==3.0.31
 Requires-Dist: PyNaCl==1.5.0
 Requires-Dist: pytz==2022.2.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: questionary==1.10.0
 Requires-Dist: requests==2.31.0
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dds_cli Version: 2.6.3 Summary: A command line tool
+Metadata-Version: 2.1 Name: dds_cli Version: 2.6.4 Summary: A command line tool
 to manage data and projects in the SciLifeLab Data Delivery System. Home-page:
 https://github.com/ScilifelabDataCentre/dds_cli Author: SciLifeLab Data Centre
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 boto3==1.24.73 Requires-Dist: botocore==1.27.73 Requires-Dist: click==8.1.3
 Requires-Dist: click-pathlib==2020.3.13.0 Requires-Dist: cryptography==42.0.4
-Requires-Dist: immutabledict==2.2.1 Requires-Dist: jwcrypto==1.5.1 Requires-
+Requires-Dist: immutabledict==2.2.1 Requires-Dist: jwcrypto==1.5.6 Requires-
 Dist: prettytable==3.4.1 Requires-Dist: prompt-toolkit==3.0.31 Requires-Dist:
 PyNaCl==1.5.0 Requires-Dist: pytz==2022.2.1 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: questionary==1.10.0 Requires-Dist: requests==2.31.0 Requires-
 Dist: rich==12.5.1 Requires-Dist: rich-click==1.5.2 Requires-Dist:
 simplejson==3.17.6 Requires-Dist: tzlocal==4.2 Requires-Dist: zstandard==0.19.0
                     ************ DDaattaa DDeelliivveerryy SSyysstteemm:: CCLLII ************
  AA ccoommmmaanndd lliinnee ttooooll ``ddddss`` ttoo mmaannaaggee pprroojjeeccttss aanndd ddaattaa iinn tthhee SScciiLLiiffeeLLaabb DDaattaa
```

### Comparing `dds_cli-2.6.3/dds_cli.egg-info/SOURCES.txt` & `dds_cli-2.6.4/dds_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/setup.py` & `dds_cli-2.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_account_manager.py` & `dds_cli-2.6.4/tests/test_account_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_data_remover.py` & `dds_cli-2.6.4/tests/test_data_remover.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_file_compressor.py` & `dds_cli-2.6.4/tests/test_file_compressor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_file_encryptor.py` & `dds_cli-2.6.4/tests/test_file_encryptor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_file_handler_local.py` & `dds_cli-2.6.4/tests/test_file_handler_local.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_motd_manager.py` & `dds_cli-2.6.4/tests/test_motd_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_project_status.py` & `dds_cli-2.6.4/tests/test_project_status.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_superadmin_helper.py` & `dds_cli-2.6.4/tests/test_superadmin_helper.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.6.3/tests/test_utils.py` & `dds_cli-2.6.4/tests/test_utils.py`

 * *Files identical despite different names*

