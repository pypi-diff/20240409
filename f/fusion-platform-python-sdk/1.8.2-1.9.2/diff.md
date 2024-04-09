# Comparing `tmp/fusion-platform-python-sdk-1.8.2.tar.gz` & `tmp/fusion-platform-python-sdk-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-platform-python-sdk-1.8.2.tar", last modified: Wed Oct 18 14:11:31 2023, max compression
+gzip compressed data, was "fusion-platform-python-sdk-1.9.2.tar", last modified: Thu Jan  4 07:44:55 2024, max compression
```

## Comparing `fusion-platform-python-sdk-1.8.2.tar` & `fusion-platform-python-sdk-1.9.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-10-18 14:11:31.049281 fusion-platform-python-sdk-1.8.2/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.8.2/LICENSE.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.8.2/MANIFEST.in
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5126 2023-10-18 14:11:31.048639 fusion-platform-python-sdk-1.8.2/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4456 2023-08-08 06:50:33.000000 fusion-platform-python-sdk-1.8.2/README.md
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-10-18 14:11:31.027581 fusion-platform-python-sdk-1.8.2/fusion_platform/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7151 2023-10-18 14:11:27.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/__main__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/base.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/command.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-10-18 14:11:31.029047 fusion-platform-python-sdk-1.8.2/fusion_platform/common/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/common/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/common/raise_thread.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/common/utilities.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4579 2023-08-08 07:27:21.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/detailed_example.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/documentation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1652653 2023-08-08 06:58:34.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/fusion_platform_sdk.pdf
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4697 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/glasgow.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)  3746742 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/lake_district.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/localisations.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/localise.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-10-18 14:11:31.043078 fusion-platform-python-sdk-1.8.2/fusion_platform/models/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/credit.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/credit.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/data.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/data.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/data_file.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/data_file.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/fields.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/model.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/organisation.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/organisation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    50773 2023-10-02 06:34:58.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-07-06 09:45:04.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10513 2023-07-06 06:16:57.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution_log.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution_log.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/service.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/service.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-10-18 14:11:28.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/user.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/models/user.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1891 2023-08-08 07:27:21.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/quick_example.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/session.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-10-18 14:11:27.000000 fusion-platform-python-sdk-1.8.2/fusion_platform/translations.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-10-18 14:11:31.047543 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5126 2023-10-18 14:11:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1773 2023-10-18 14:11:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-10-18 14:11:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       76 2023-10-18 14:11:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-10-18 14:11:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/requires.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-10-18 14:11:30.000000 fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-10-18 14:11:31.049529 fusion-platform-python-sdk-1.8.2/setup.cfg
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1552 2023-10-18 14:11:27.000000 fusion-platform-python-sdk-1.8.2/setup.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2024-01-04 07:44:55.686307 fusion-platform-python-sdk-1.9.2/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.9.2/LICENSE.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.9.2/MANIFEST.in
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5126 2024-01-04 07:44:55.685833 fusion-platform-python-sdk-1.9.2/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4456 2023-08-08 06:50:33.000000 fusion-platform-python-sdk-1.9.2/README.md
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2024-01-04 07:44:55.657517 fusion-platform-python-sdk-1.9.2/fusion_platform/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7151 2024-01-04 07:44:52.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/__main__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/base.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/command.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2024-01-04 07:44:55.660398 fusion-platform-python-sdk-1.9.2/fusion_platform/common/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/common/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/common/raise_thread.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/common/utilities.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4579 2023-08-08 07:27:21.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/detailed_example.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/documentation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1658388 2024-01-04 07:44:18.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/fusion_platform_sdk.pdf
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4697 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/glasgow.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  3746742 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/lake_district.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/localisations.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/localise.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2024-01-04 07:44:55.680576 fusion-platform-python-sdk-1.9.2/fusion_platform/models/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/credit.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/credit.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/data.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/data.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/data_file.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/data_file.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/fields.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/model.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/organisation.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/organisation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    50773 2023-10-02 06:34:58.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-07-06 09:45:04.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10513 2023-07-06 06:16:57.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution_log.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution_log.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/service.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/service.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2024-01-04 07:44:53.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/user.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/models/user.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1891 2023-08-08 07:27:21.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/quick_example.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/session.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2024-01-04 07:44:52.000000 fusion-platform-python-sdk-1.9.2/fusion_platform/translations.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2024-01-04 07:44:55.684692 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5126 2024-01-04 07:44:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1773 2024-01-04 07:44:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2024-01-04 07:44:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       76 2024-01-04 07:44:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2024-01-04 07:44:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2024-01-04 07:44:55.000000 fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2024-01-04 07:44:55.686524 fusion-platform-python-sdk-1.9.2/setup.cfg
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1552 2024-01-04 07:44:52.000000 fusion-platform-python-sdk-1.9.2/setup.py
```

### Comparing `fusion-platform-python-sdk-1.8.2/LICENSE.txt` & `fusion-platform-python-sdk-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/PKG-INFO` & `fusion-platform-python-sdk-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.8.2
+Version: 1.9.2
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fusion-platform-python-sdk-1.8.2/README.md` & `fusion-platform-python-sdk-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/__init__.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 &copy; [Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 """
 
 # Do not modify the following two lines as they are maintained by the version.sh script.
-__version__ = '1.8.2'
-__version_date__ = '2023-10-18T14:11:27Z'
+__version__ = '1.9.2'
+__version_date__ = '2024-01-04T07:44:52Z'
 
 # Exclude certain sub-modules from documentation.
 # @formatter:off
 __pdoc__ = {
     'base': False,
     'command': False,
     'common': False,
```

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/base.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/base.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/common/raise_thread.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/common/raise_thread.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/common/utilities.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/common/utilities.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/detailed_example.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/detailed_example.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/documentation.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/documentation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.9.2/fusion_platform/fusion_platform_sdk.pdf`

 * *Files 3% similar despite different names*

#### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.9.2/fusion_platform/fusion_platform_sdk.pdf`

 * *Document info*

```diff
@@ -1,5 +1,3 @@
-CreationDate: "D:20230808065834Z00'00'"
-Creator: 'Word'
-ModDate: "D:20230808065834Z00'00'"
-Producer: 'macOS Version 13.4.1 (c) (Build 22F770820d) Quartz PDFContext'
-Title: 'Microsoft Word - fusion_platform_sdk.docx'
+CreationDate: "D:20240104074418Z00'00'"
+ModDate: "D:20240104074418Z00'00'"
+Producer: 'macOS Version 14.2.1 (Build 23C71) Quartz PDFContext'
```

#### pdftotext {} -

```diff
@@ -1,15 +1,15 @@
 Digital Content Analysis Technology Ltd
 
 Fusion Platform®
 
 Python SDK
 
-Version 1.8
-8th August 2023
+Version 1.9
+4th January 2024
 
 Digital Content Analysis Technology Ltd
 
 Table of Contents
 1
 
 Introduction ..................................................................................................... 4
@@ -24,15 +24,15 @@
 
 1.3
 
 Overview ................................................................................................................................................. 4
 
 2
 
-Overview ......................................................................................................... 5
+Overview .......................................................................................................... 5
 
 2.1
 
 User Accounts, Organisations and Credits ............................................................................... 5
 
 2.2
 
@@ -44,65 +44,64 @@
 
 2.4
 
 Usage......................................................................................................................................................... 7
 
 3
 
-Quick Example ................................................................................................. 8
+Quick Example .................................................................................................. 8
 
 4
 
 Authentication ............................................................................................... 10
 
 5
 
-Uploading Files............................................................................................... 13
+Uploading Files ............................................................................................... 13
 
 6
 
-Browsing Services .......................................................................................... 18
+Browsing Services ........................................................................................... 18
 
 7
 
-Creating Processes ......................................................................................... 20
+Creating Processes .......................................................................................... 20
 
 8
 
-Executing and Monitoring Processes .............................................................. 26
+Executing and Monitoring Processes ............................................................... 26
 
 9
 
-Obtaining Execution Inputs and Outputs ........................................................ 30
+Obtaining Execution Inputs and Outputs......................................................... 30
 
-10 Detailed Example ........................................................................................... 32
+10 Detailed Example ............................................................................................ 32
 11 SDK Object Attributes and Methods ............................................................... 36
 11.1
 
 Attributes and Methods ................................................................................................................. 36
 
-12 Glossary of Terms........................................................................................... 38
-13 References ..................................................................................................... 40
+12 Glossary of Terms ........................................................................................... 38
+13 References ...................................................................................................... 40
 
 2
 
 Digital Content Analysis Technology Ltd
 
 Revision History
 
 Draft
 
 7th February 2022
-th
 
 Initial draft for review.
 
 Draft
 
-9 February 2022
+9th February 2022
 
 Updated following internal review.
 
 Draft
 
 22nd February 2022
 
@@ -112,17 +111,15 @@
 
 3rd March 2022
 
 Version candidate.
 
 Draft
 
-th
-
-8 March 2022
+8th March 2022
 
 Revised following internal review to include link to code
 documentation.
 
 Draft
 
 20th April 2022
@@ -149,17 +146,19 @@
 
 Draft
 
 14th June 2022
 
 Revised to include downloading of file previews.
 
+th
+
 Version 1.2
 
-15th June 2022
+15 June 2022
 
 Issued for Fusion Platform® version 1.2.
 
 Draft
 
 27th June 2022
 
@@ -167,17 +166,19 @@
 
 Draft
 
 21st July 2022
 
 Added aggregator to detailed example.
 
+nd
+
 Version 1.3
 
-22nd July 2022
+22 July 2022
 
 Issued for Fusion Platform® version 1.3.
 
 Draft
 
 1st September 2022
 
@@ -192,59 +193,57 @@
 
 Version 1.4
 
 1st September 2022
 
 Issued for Fusion Platform® version 1.4.
 
-th
-
 Draft
 
-24 November 2022
+24th November 2022
 
 Added ability to copy a process.
 
 Version 1.5
 
 29th November 2022
 
 Issued for Fusion Platform® version 1.5.
 
 Version 1.6
 
-8th February 2023
+th
 
-Issued for Fusion Platform® version 1.6.
+8 February 2023
 
-rd
+Issued for Fusion Platform® version 1.6.
 
 Draft
 
-3 May 2023
+3rd May 2023
 
 Added changed_delete_expiry method for process execution.
 
 Draft
 
 23rd May 2023
 
 Added the ability to include dispatchers within a process.
 
+th
+
 Version 1.7
 
-7th June 2023
+7 June 2023
 
 Issued for Fusion Platform® version 1.7.
 
 Draft
 
-th
-
-26 June 2023
+26th June 2023
 
 Extracted and tidied examples.
 
 Draft
 
 7th July 2023
 
@@ -252,21 +251,27 @@
 
 Version 1.8
 
 8th August 2023
 
 Issued for Fusion Platform® version 1.8.
 
+Version 1.9
+
+4th January 2024
+
+Issued for Fusion Platform® version 1.9.
+
 This document has been prepared by Digital Content Analysis Technology Ltd, who can be
 contacted at support@d-cat.co.uk
 Digital Content Analysis Technology Ltd, Registered in Scotland, SC499652.
 This document is copyright and is issued on the strict understanding that it is not to be
 reproduced, copied, or disclosed to a third party, in whole or in part, without the consent of
 Digital Content Analysis Technology Ltd.
-© 2023 Digital Content Analysis Technology Ltd
+© 2024 Digital Content Analysis Technology Ltd
 3
 
 Digital Content Analysis Technology Ltd
 
 1
 
 Introduction
```

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/glasgow.geojson` & `fusion-platform-python-sdk-1.9.2/fusion_platform/glasgow.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/lake_district.geojson` & `fusion-platform-python-sdk-1.9.2/fusion_platform/lake_district.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/localisations.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/localisations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/localise.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/localise.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/credit.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/credit.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/credit.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/credit.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/data.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/data.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/data.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/data.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/data_file.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/data_file.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/data_file.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/data_file.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/fields.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/fields.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/model.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/model.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/organisation.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/organisation.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/organisation.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/organisation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_execution.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_execution.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/process_service_execution_log.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/process_service_execution_log.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/service.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/service.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/service.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/service.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/user.md` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/user.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/models/user.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/models/user.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/quick_example.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/quick_example.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/session.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/session.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform/translations.py` & `fusion-platform-python-sdk-1.9.2/fusion_platform/translations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/PKG-INFO` & `fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.8.2
+Version: 1.9.2
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fusion-platform-python-sdk-1.8.2/fusion_platform_python_sdk.egg-info/SOURCES.txt` & `fusion-platform-python-sdk-1.9.2/fusion_platform_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.8.2/setup.py` & `fusion-platform-python-sdk-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Find the package root directory.
 PACKAGE_DIR = pathlib.Path(__file__).parent
 
 # Set up the package.
 # @formatter:off
 setup(
     name='fusion-platform-python-sdk',
-    version='1.8.2',
+    version='1.9.2',
     description='Python SDK used to interact with the Fusion Platform(r)',
     long_description=(PACKAGE_DIR / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/d-cat-support/fusion-platform-python-sdk',
     author='Digital Content Analysis Technology Ltd',
     author_email='support@d-cat.co.uk',
     license='MIT',
```

