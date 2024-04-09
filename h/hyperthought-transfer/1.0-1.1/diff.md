# Comparing `tmp/hyperthought-transfer-1.0.tar.gz` & `tmp/hyperthought-transfer-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmpvb9ft0ul\hyperthought-transfer-1.0.tar", last modified: Mon Dec 11 07:05:51 2023, max compression
+gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmp4jmmzayh\hyperthought-transfer-1.1.tar", last modified: Tue Apr  9 11:19:21 2024, max compression
```

## Comparing `hyperthought-transfer-1.0.tar` & `hyperthought-transfer-1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/
--rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/.coveragerc
--rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-1.0/.gitignore
--rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-1.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-1.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-1.0/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/docs/
--rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/changelog.rst
--rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/index.rst
--rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/license.rst
--rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/Makefile
--rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/docs/_static/
--rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/docs/_static/.gitignore
--rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2764 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-1.0/README.rst
--rw-rw-rw-   0        0        0     1335 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-12-06 12:56:22.000000 hyperthought-transfer-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/
--rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/base.py
--rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/_mcafee.py
--rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/
--rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/data.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/
--rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/connect.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/template/
--rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/template/create.py
--rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/template/template.db
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/template/__init__.py
--rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/process/
--rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/process/filebinner.py
--rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/process/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/
--rw-rw-rw-   0        0        0     3273 2023-05-31 09:22:05.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/connect.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/template/
--rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/template/create.py
--rw-rw-rw-   0        0        0   147456 2023-12-11 01:32:47.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/template/template.db
--rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/template/__init__.py
--rw-rw-rw-   0        0        0    74639 2023-12-11 07:05:21.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/processes/
--rw-rw-rw-   0        0        0     6857 2023-05-31 09:04:03.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/processes/rules.py
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/processes/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-12-11 01:04:56.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/utils.py
--rw-rw-rw-   0        0        0    50990 2023-12-11 01:38:07.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/__init__.py
--rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-1.0/src/hyperthought_transfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/
--rw-rw-rw-   0        0        0        1 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2764 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1840 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-11 07:05:51.000000 hyperthought-transfer-1.0/tests/
--rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/tests/conftest.py
--rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/
+-rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/.coveragerc
+-rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-1.1/.gitignore
+-rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-1.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-1.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-1.1/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/docs/
+-rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/license.rst
+-rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/docs/_static/
+-rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2764 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-1.1/README.rst
+-rw-rw-rw-   0        0        0     1335 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2024-01-28 19:41:19.000000 hyperthought-transfer-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/
+-rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/base.py
+-rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/_mcafee.py
+-rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/
+-rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/data.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/
+-rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/connect.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/template/
+-rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/template/create.py
+-rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/template/template.db
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/template/__init__.py
+-rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/process/
+-rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/process/filebinner.py
+-rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/process/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/
+-rw-rw-rw-   0        0        0     3273 2023-05-31 09:22:05.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/connect.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/template/
+-rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/template/create.py
+-rw-rw-rw-   0        0        0   147456 2024-01-28 19:41:19.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/template/template.db
+-rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/template/__init__.py
+-rw-rw-rw-   0        0        0    77845 2024-01-28 19:41:19.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/processes/
+-rw-rw-rw-   0        0        0     6857 2023-05-31 09:04:03.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/processes/rules.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/processes/__init__.py
+-rw-rw-rw-   0        0        0     2010 2024-01-28 19:41:19.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/utils.py
+-rw-rw-rw-   0        0        0    52517 2024-01-28 19:41:19.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-1.1/src/hyperthought_transfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2764 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1840 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 11:19:21.000000 hyperthought-transfer-1.1/tests/
+-rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-1.1/tox.ini
```

### Comparing `hyperthought-transfer-1.0/.coveragerc` & `hyperthought-transfer-1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/.gitignore` & `hyperthought-transfer-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/.readthedocs.yml` & `hyperthought-transfer-1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/CONTRIBUTING.rst` & `hyperthought-transfer-1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/docs/conf.py` & `hyperthought-transfer-1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/docs/index.rst` & `hyperthought-transfer-1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/docs/Makefile` & `hyperthought-transfer-1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/LICENSE.txt` & `hyperthought-transfer-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/PKG-INFO` & `hyperthought-transfer-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 1.0
+Version: 1.1
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-1.0/README.rst` & `hyperthought-transfer-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/setup.cfg` & `hyperthought-transfer-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/setup.py` & `hyperthought-transfer-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from setuptools import setup, find_packages
 
 
 if __name__ == "__main__":
     try:
         setup(
-            version="1.0",
+            version="1.1",
             use_scm_version={
                 "version_scheme": "no-guess-dev",
                 "local-scheme": "no-local-version",
             },
             packages=find_packages(where="src"),
             package_dir={"": "src"},
             include_package_data=True,
```

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/base.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/base.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/_mcafee.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/_mcafee.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/antivirus/__init__.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/antivirus/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/data.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/data.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/connect.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/template/create.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/template/template.db` & `hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/database/__init__.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/filebinner/process/filebinner.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/filebinner/process/filebinner.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/connect.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/template/create.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/template/template.db` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/database/__init__.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/database/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1654,14 +1654,55 @@
             )
         """
         cursor.executemany(sql, rule_data)
 
         if commit:
             self.connection.commit()
 
+    def update_file_status(
+        self,
+        file_ids: Iterable[int],
+        status: FileStatus,
+        commit: bool = True,
+    ) -> None:
+        """
+        Update status for multiple files.
+
+        All files will be given the same status.
+
+        Parameters
+        ----------
+        file_ids : list-like of int
+            Sequence of file ids.
+        status : FileStatus
+            Status to set for all files.
+        commit : bool
+            Determines whether changes will be committed to the database.
+            This may be false if the changes are part of a transaction.
+        """
+        file_ids = list(file_ids)
+
+        for file_id in file_ids:
+            if not isinstance(file_id, int):
+                raise ValueError("All file ids must be ints.")
+
+        file_ids_in = ", ".join(str(file_id) for file_id in file_ids)
+        sql = f"""
+        UPDATE File
+        SET file_status_id = :file_status_id
+        WHERE id IN ({file_ids_in})
+        """
+        cursor = self.connection.cursor()
+        cursor.execute(sql, {"file_status_id": status.value})
+
+        if commit:
+            self.connection.commit()
+
+        cursor.close()
+
     def get_last_id(self, table: str) -> int:
         """Get the last id in a table."""
         valid_tables = {
             "Parser",
             "Metadata",
             "MetadataApplication",
             "File",
@@ -2386,14 +2427,72 @@
             raise FileSpecificMetadataUniquenessException(
                 "Multiple file-specific Metadata records found for file "
                 f"with id {file_id}."
             )
 
         return metadata_id
 
+    def get_metadata_information(
+        self,
+        file_ids: Iterable[int],
+    ) -> Generator[Dict, Optional[None], Optional[None]]:
+        """
+        Get data to be used with the update-metadata endpoint.
+
+        Parameters
+        ----------
+        file_ids : list-like of int
+            Internal file ids for files of interest.
+
+        Yields
+        ------
+        A dict with keys "file_id", "metadata_id", "hyperthought_id", and
+        "metadata".  This information can be used to build data structures
+        mapping file ids to lists of metadata ids, file ids to hyperthought
+        ids, and metadata ids to metadata.  These data structures, in turn,
+        can be used to build a list of dicts having keys "documentId"
+        and "metadata" (combined for each file), which can be used as input
+        to the update-metadata HyperThought endpoint.
+        """
+        # Make defensive copy and ensure multiple iteration.
+        file_ids = list(file_ids)
+
+        # Validate file_ids.
+        for file_id in file_ids:
+            if not isinstance(file_id, int):
+                raise ValueError("file ids must be ints")
+
+        file_ids_str = ", ".join(str(file_id) for file_id in file_ids)
+
+        sql = f"""
+        SELECT
+            MetadataApplication.file_id,
+            MetadataApplication.metadata_id,
+            File.hyperthought_id,
+            Metadata.metadata
+        FROM
+            File
+            INNER JOIN MetadataApplication
+                ON File.id = MetadataApplication.file_id
+            INNER JOIN Metadata
+                ON Metadata.id = MetadataApplication.metadata_id
+        WHERE
+            File.id IN ({file_ids_str})
+        """
+        cursor = self.connection.cursor()
+        cursor.execute(sql)
+
+        for row in cursor.fetchall():
+            yield {
+                key: row[key]
+                for key in row.keys()
+            }
+
+        cursor.close()
+
     def delete_metadata(self, metadata_id: int, commit: bool = True) -> None:
         """Remove a Metadata record."""
         sql = "DELETE FROM Metadata WHERE id = :metadata_id"
         cursor = self.connection.cursor()
         cursor.execute(sql, {"metadata_id": metadata_id})
 
         if commit:
```

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/processes/rules.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/processes/rules.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/utils.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/manifest/__init__.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/manifest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import hyperthought as ht
 from hyperthought.metadata import MetadataItem
 
 from . import database
 from .database import TargetRule
 from .database import FileFilter
+from .database import FileStatus
 from .processes.rules import FileData
 from .processes.rules import RulesEngineProcess
 from .processes.rules import STOP_SIGNAL as RULES_PROCESS_STOP_SIGNAL
 from . import utils
 
 
 MAX_PROCESSES = 60
@@ -704,15 +705,14 @@
         for file_ in self.database.get_files(paths=paths_to_add):
             existing_paths.add(file_["path"])
 
             if file_["is_folder"]:
                 folder_path_to_hyperthought_id[file_["path"]] = (
                     file_["hyperthought_id"])
 
-
         # Add ids for existing folders to the lookup.
         for path in paths_to_add:
             is_folder = os.path.isdir(path)
 
             if path not in existing_paths and is_folder:
                 folder_path_to_hyperthought_id[path] = utils.generate_id()
 
@@ -1358,14 +1358,57 @@
         Returns
         -------
         A list of dicts containing file record data.
         """
         for file_ in self.database.get_files(file_ids=file_ids, paths=paths):
             yield file_
 
+    def get_metadata_information(
+        self,
+        file_ids: Iterable[int],
+    ) -> Generator[Dict, Optional[None], Optional[None]]:
+        """
+        Get data to be used with the update-metadata endpoint.
+
+        Parameters
+        ----------
+        file_ids : list-like of int
+            Internal file ids for files of interest.
+
+        Yields
+        ------
+        A dict with keys "file_id", "metadata_id", "hyperthought_id", and
+        "metadata".  This information can be used to build data structures
+        mapping file ids to lists of metadata ids, file ids to hyperthought
+        ids, and metadata ids to metadata.  These data structures, in turn,
+        can be used to build a list of dicts having keys "documentId"
+        and "metadata" (combined for each file), which can be used as input
+        to the update-metadata HyperThought endpoint.
+        """
+        yield from self.database.get_metadata_information(file_ids=file_ids)
+
+    def update_file_status(
+        self,
+        file_ids: Iterable[int],
+        status: FileStatus,
+    ) -> None:
+        """
+        Update status for multiple files.
+
+        All files will be given the same status.
+
+        Parameters
+        ----------
+        file_ids : list-like of int
+            Sequence of file ids.
+        status : FileStatus
+            Status to set for all files.
+        """
+        self.database.update_file_status(file_ids=file_ids, status=status)
+
 
 def from_json(manifest_data: Dict, manifest_database_file: str) -> Manifest:
     """
     Create and return a manifest with the given (JSON) data.
 
     Convert JSON to SQLite and store in the specified database file.
```

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer/__init__.py` & `hyperthought-transfer-1.1/src/hyperthought_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/PKG-INFO` & `hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 1.0
+Version: 1.1
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-1.0/src/hyperthought_transfer.egg-info/SOURCES.txt` & `hyperthought-transfer-1.1/src/hyperthought_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-1.0/tox.ini` & `hyperthought-transfer-1.1/tox.ini`

 * *Files identical despite different names*

