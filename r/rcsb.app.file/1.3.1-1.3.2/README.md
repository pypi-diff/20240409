# Comparing `tmp/rcsb.app.file-1.3.1.tar.gz` & `tmp/rcsb.app.file-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.app.file-1.3.1.tar", last modified: Wed Mar 13 14:06:43 2024, max compression
+gzip compressed data, was "rcsb.app.file-1.3.2.tar", last modified: Tue Apr  9 19:26:12 2024, max compression
```

## Comparing `rcsb.app.file-1.3.1.tar` & `rcsb.app.file-1.3.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.596547 rcsb.app.file-1.3.1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1792 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       89 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    15831 2024-03-13 14:06:43.596547 rcsb.app.file-1.3.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    14386 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.588547 rcsb.app.file-1.3.1/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.592547 rcsb.app.file-1.3.1/rcsb/app/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.592547 rcsb.app.file-1.3.1/rcsb/app/client/
--rw-r--r--   0 vsts      (1001) docker     (127)    37280 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/client/ClientUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/client/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.592547 rcsb.app.file-1.3.1/rcsb/app/client/front-end/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/client/front-end/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20380 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/client/front-end/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36463 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/client/front-end/gui.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.592547 rcsb.app.file-1.3.1/rcsb/app/config/
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      213 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/config/setConfig.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.596547 rcsb.app.file-1.3.1/rcsb/app/file/
--rw-r--r--   0 vsts      (1001) docker     (127)     7612 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/ConfigProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26658 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/Definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4868 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/DownloadUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14310 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/IoUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/JWTAuthBearer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1673 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/JWTAuthToken.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/KvBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4809 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/KvConnection.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20240 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/KvRedis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5139 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/KvSqlite.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13645 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/PathProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20162 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/RedisLock.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13179 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/Sessions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19159 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/SoftLock.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24742 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/TernaryLock.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14968 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/UploadUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2322 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/downloadRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6500 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/ioRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3300 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6228 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/pathRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3465 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/serverStatus.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1163 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/serverStatusRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)      749 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/tokenRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/rcsb/app/file/uploadRequest.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-13 14:06:43.596547 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    15831 2024-03-13 14:06:43.000000 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-03-13 14:06:43.000000 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-13 14:06:43.000000 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-13 13:47:21.000000 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      395 2024-03-13 14:06:43.000000 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-03-13 14:06:43.000000 rcsb.app.file-1.3.1/rcsb.app.file.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-03-13 14:06:43.596547 rcsb.app.file-1.3.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2150 2024-03-13 13:46:04.000000 rcsb.app.file-1.3.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.661969 rcsb.app.file-1.3.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1833 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       89 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    15936 2024-04-09 19:26:12.661969 rcsb.app.file-1.3.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    14491 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.653969 rcsb.app.file-1.3.2/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.653969 rcsb.app.file-1.3.2/rcsb/app/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.653969 rcsb.app.file-1.3.2/rcsb/app/client/
+-rw-r--r--   0 vsts      (1001) docker     (127)    37280 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/client/ClientUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/client/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.653969 rcsb.app.file-1.3.2/rcsb/app/client/front-end/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/client/front-end/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20380 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/client/front-end/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36463 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/client/front-end/gui.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.653969 rcsb.app.file-1.3.2/rcsb/app/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      213 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/config/setConfig.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.661969 rcsb.app.file-1.3.2/rcsb/app/file/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8853 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/ConfigProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26658 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/Definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4868 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/DownloadUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14310 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/IoUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/JWTAuthBearer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1673 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/JWTAuthToken.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/KvBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4809 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/KvConnection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20240 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/KvRedis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5139 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/KvSqlite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13645 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/PathProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20162 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/RedisLock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13179 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/Sessions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19159 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/SoftLock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24742 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/TernaryLock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15173 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/UploadUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2322 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/downloadRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6500 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/ioRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3300 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6228 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/pathRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3465 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/serverStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1163 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/serverStatusRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      749 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/tokenRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/rcsb/app/file/uploadRequest.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 19:26:12.661969 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15936 2024-04-09 19:26:12.000000 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-04-09 19:26:12.000000 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 19:26:12.000000 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 19:06:24.000000 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      395 2024-04-09 19:26:12.000000 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-09 19:26:12.000000 rcsb.app.file-1.3.2/rcsb.app.file.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-09 19:26:12.661969 rcsb.app.file-1.3.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2150 2024-04-09 19:05:15.000000 rcsb.app.file-1.3.2/setup.py
```

### Comparing `rcsb.app.file-1.3.1/HISTORY.txt` & `rcsb.app.file-1.3.2/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,8 +17,9 @@
  1-Mar-2023  - V0.23 Updates to and reorganization of client utilities
  10-Mar-2023 - V0.24 Rewrote config file path, jwt, shell scripts, and client context
  18-Apr-2023 - V0.25 Streamlined Redis transactions
  5-Jun-2023  - V1.0 Reorganized Python files, streamlined server files and tox tests, removed router prefixes
  1-Aug-2023  - V1.1.0 Expedite Python client, session maintenance module, example cron file
 24-Sep-2023  - V1.1.1 Locking modules with unit test
 26-Feb-2024  - V1.2.1 Async test
-11-Mar-2024  - V1.3.1 Validate settings, change locks to inheritance
+11-Mar-2024  - V1.3.1 Validate settings, change locks to inheritance
+25-Mar-2024  - V1.3.2 Rewrite validation
```

### Comparing `rcsb.app.file-1.3.1/LICENSE` & `rcsb.app.file-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/PKG-INFO` & `rcsb.app.file-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.app.file
-Version: 1.3.1
+Version: 1.3.2
 Summary: RCSB File Access Service Application
 Home-page: https://github.com/rcsb/py-rcsb_app_file
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -364,17 +364,17 @@
 (or service redis stop, but not if Redis was started with /usr/bin/redis-server)
 ```
 
 To view Redis variables
 ```
 
 redis-cli
-KEYS *
-GET keyname
-HGETALL hashkey
+KEYS * (prints two values)
+GET keyname (for keyname, copy/paste the first value)
+HGETALL hashkey (for hashkey, copy/paste the second value)
 exit
 
 ```
 
 To remove all variables
 ```
```

### Comparing `rcsb.app.file-1.3.1/README.md` & `rcsb.app.file-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -320,17 +320,17 @@
 (or service redis stop, but not if Redis was started with /usr/bin/redis-server)
 ```
 
 To view Redis variables
 ```
 
 redis-cli
-KEYS *
-GET keyname
-HGETALL hashkey
+KEYS * (prints two values)
+GET keyname (for keyname, copy/paste the first value)
+HGETALL hashkey (for hashkey, copy/paste the second value)
 exit
 
 ```
 
 To remove all variables
 ```
```

### Comparing `rcsb.app.file-1.3.1/rcsb/app/client/ClientUtility.py` & `rcsb.app.file-1.3.2/rcsb/app/client/ClientUtility.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/client/front-end/client.py` & `rcsb.app.file-1.3.2/rcsb/app/client/front-end/client.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/client/front-end/gui.py` & `rcsb.app.file-1.3.2/rcsb/app/client/front-end/gui.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/ConfigProvider.py` & `rcsb.app.file-1.3.2/rcsb/app/file/ConfigProvider.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         # ---
 
     def get(self, ky: str) -> typing.Optional[str]:
         try:
             if not self.__configD:
                 if self.__configFilePath:
                     self.__readConFigFromConFigYmlFile()
+            if ky == "DEFAULT_FILE_PERMISSIONS":
+                # convert from octal to integer
+                return int(str(self.__configD["data"][ky]), 8)
             return self.__configD["data"][ky]
         except Exception:
             pass
         return None
 
     def getConfig(self) -> typing.Dict:
         try:
@@ -80,126 +83,158 @@
             }
             ok = True
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             ok = False
         return ok
 
-    def set(self, key: str, val: typing.Union[str, int, float, bool]):
-        """
-        facilitate validation tests
-        should only be used by validate
-        """
+    def _set(self, key: str, val: typing.Union[str, int, float, bool]):
         if not self.__configD:
             if self.__configFilePath:
                 self.__readConFigFromConFigYmlFile()
         self.__configD["data"][key] = val
 
     def validate(self) -> bool:
         """
         exit at server start if settings do not validate
         """
+
+        # define our own bools that differ from python
+        def non_empty(value) -> bool:
+            """do not match nulls, whitespace, or empty string"""
+            return value is not None and str(value).strip() != ""
+
+        def falsy(value: int) -> bool:
+            """do not match zero or less than zero"""
+            return value is None or str(value).strip() == "" or int(value) <= 0
+
+        def nullish(value: int) -> bool:
+            """match zero"""
+            return value is None or str(value).strip() == "" or int(value) < 0
+
+        settings = [
+            "SERVER_HOST_AND_PORT",
+            "SURPLUS_PROCESSORS",
+            "REPOSITORY_DIR_PATH",
+            "SESSION_DIR_PATH",
+            "SHARED_LOCK_PATH",
+            "LOCK_TRANSACTIONS",
+            "LOCK_TYPE",
+            "LOCK_TIMEOUT",
+            "KV_MODE",
+            "REDIS_HOST",
+            "KV_SESSION_TABLE_NAME",
+            "KV_MAP_TABLE_NAME",
+            "KV_LOCK_TABLE_NAME",
+            "KV_MAX_SECONDS",
+            "KV_FILE_PATH",
+            "CHUNK_SIZE",
+            "COMPRESSION_TYPE",
+            "HASH_TYPE",
+            "DEFAULT_FILE_PERMISSIONS",
+            "JWT_SUBJECT",
+            "JWT_ALGORITHM",
+            "JWT_SECRET",
+            "JWT_DURATION",
+            "BYPASS_AUTHORIZATION",
+        ]
+        assert_non_falsy = ["KV_MAX_SECONDS", "CHUNK_SIZE", "JWT_DURATION"]
+        assert_non_nullish = ["SURPLUS_PROCESSORS", "LOCK_TIMEOUT"]
+
+        if not all([non_empty(self.get(setting)) for setting in settings]):
+            return False
+        if any([falsy(self.get(setting)) for setting in assert_non_falsy]):
+            return False
+        if any([nullish(self.get(setting)) for setting in assert_non_nullish]):
+            return False
+
         # validate host and port
         host = self.get("SERVER_HOST_AND_PORT")
-        if not host or not validators.url(str(host)):
+        if not validators.url(str(host)):
             return False
         # validate surplus processors
         surplus = self.get("SURPLUS_PROCESSORS")
-        if (
-            surplus is None
-            or surplus == ""
-            or re.match(r"\d+", str(surplus)) is None
-            or int(surplus) < 0
-        ):
+        if not re.fullmatch(r"\d+", str(surplus)):
             return False
         # validate path strings
         paths = [
             self.get("REPOSITORY_DIR_PATH"),
             self.get("SESSION_DIR_PATH"),
             self.get("SHARED_LOCK_PATH"),
             self.get("KV_FILE_PATH"),
         ]
-        if not all(paths) or not all(
-            [re.match(r"\.{0,2}(/?\w+)+/?", str(path)) for path in paths]
+        if not all(
+            [
+                re.fullmatch(r"^\.{0,2}(/?[\w\.\- _\~]+)+/?$", str(path))
+                for path in paths
+            ]
         ):
             return False
         # validate lock transactions
         lock = self.get("LOCK_TRANSACTIONS")
-        if not lock or not isinstance(lock, bool):
+        if not isinstance(lock, bool):
             return False
         # validate lock type
         lock_types = ["soft", "ternary", "redis"]
         lock_type = self.get("LOCK_TYPE")
-        if not lock_type or str(lock_type) not in lock_types:
+        if str(lock_type) not in lock_types:
             return False
         # validate lock timeout
-        lock_timeout = self.get("LOCK_TIMEOUT")
-        if not lock_timeout or not re.match(r"\d+", str(lock_timeout)):
+        timeout = self.get("LOCK_TIMEOUT")
+        if not re.fullmatch(r"\d+", str(timeout)):
             return False
         # validate kv mode
         kv_modes = ["sqlite", "redis"]
         kv_mode = self.get("KV_MODE")
-        if not kv_mode or str(kv_mode) not in kv_modes:
+        if str(kv_mode) not in kv_modes:
             return False
-        # require kv mode redis for lock type redis and vice versa
+        # require kv mode redis for lock type redis but not vice versa
         kv_mode_redis = self.get("KV_MODE") == "redis"
         lock_type_redis = self.get("LOCK_TYPE") == "redis"
-        if any([kv_mode_redis, lock_type_redis]) and not all(
-            [kv_mode_redis, lock_type_redis]
-        ):
+        if lock_type_redis and not kv_mode_redis:
             return False
         # validate redis host
         redis_hosts = ["localhost", "redis"]
         redis_host = self.get("REDIS_HOST")
-        if not redis_host or str(redis_host) not in redis_hosts:
+        if str(redis_host) not in redis_hosts:
             if not validators.url(str(redis_host)):
                 return False
         # validate table names
         table_names = [
             self.get("KV_MAP_TABLE_NAME"),
             self.get("KV_SESSION_TABLE_NAME"),
             self.get("KV_LOCK_TABLE_NAME"),
         ]
-        if not all(table_names) or not all(
-            [re.match(r"\w+", str(name)) for name in table_names]
-        ):
+        if not all([re.fullmatch(r"\w+", str(name)) for name in table_names]):
             return False
         # validate max seconds
         max_seconds = self.get("KV_MAX_SECONDS")
-        if (
-            not max_seconds
-            or not re.match(r"\d+", str(max_seconds))
-            or int(max_seconds) < 0
-        ):
+        if not re.fullmatch(r"\d+", str(max_seconds)):
             return False
         # validate chunk size
         chunk_size = self.get("CHUNK_SIZE")
-        if (
-            not chunk_size
-            or not re.match(r"\d+", str(chunk_size))
-            or int(chunk_size) < 0
-        ):
+        if not re.fullmatch(r"\d+", str(chunk_size)):
             return False
         # validate compression type
         compressions = ["gzip", "zip", "bzip2", "lzma"]
         compression = self.get("COMPRESSION_TYPE")
-        if not compression or str(compression) not in compressions:
+        if str(compression) not in compressions:
             return False
         # validate hash type
         hash_types = ["MD5", "SHA1", "SHA256"]
         hash_type = self.get("HASH_TYPE")
-        if not hash_type or str(hash_type) not in hash_types:
+        if str(hash_type) not in hash_types:
             return False
-        # reading dictionary returns integer value of octal so have no way to verify octal string
+        # validate default file permissions
         permissions = self.__configD["data"]["DEFAULT_FILE_PERMISSIONS"]
-        if not permissions or not re.match(r"\d+", str(permissions)):
+        if not re.fullmatch(r"[0-7]{3}", str(permissions)):
             return False
         # validate jwt strings
         jwts = [self.get("JWT_SUBJECT"), self.get("JWT_SECRET")]
-        if not all(jwts) or not all([re.match(r"\w+", str(jwt)) for jwt in jwts]):
+        if not all([re.fullmatch(r"\w+", str(jwt)) for jwt in jwts]):
             return False
         # validate jwt algorithm
         algorithms = [
             "HS256",
             "HS384",
             "HS512",
             "ES256",
@@ -211,18 +246,19 @@
             "RS512",
             "PS256",
             "PS384",
             "PS512",
             "EdDSA",
         ]
         algorithm = self.get("JWT_ALGORITHM")
-        if not algorithm or str(algorithm) not in algorithms:
+        if str(algorithm) not in algorithms:
             return False
         # validate jwt timeout
         duration = self.get("JWT_DURATION")
-        if not duration or not re.match(r"\d+", str(duration)) or int(duration) < 0:
+        # will not match zero
+        if not re.fullmatch(r"\d+", str(duration)) or int(duration) < 0:
             return False
         # validate bypass authorization
         bypass_authorization = self.get("BYPASS_AUTHORIZATION")
-        if not bypass_authorization or not isinstance(bypass_authorization, bool):
+        if not isinstance(bypass_authorization, bool):
             return False
         return True
```

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/Definitions.py` & `rcsb.app.file-1.3.2/rcsb/app/file/Definitions.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/DownloadUtility.py` & `rcsb.app.file-1.3.2/rcsb/app/file/DownloadUtility.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/IoUtility.py` & `rcsb.app.file-1.3.2/rcsb/app/file/IoUtility.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/JWTAuthBearer.py` & `rcsb.app.file-1.3.2/rcsb/app/file/JWTAuthBearer.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/JWTAuthToken.py` & `rcsb.app.file-1.3.2/rcsb/app/file/JWTAuthToken.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/KvBase.py` & `rcsb.app.file-1.3.2/rcsb/app/file/KvBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/KvConnection.py` & `rcsb.app.file-1.3.2/rcsb/app/file/KvConnection.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/KvRedis.py` & `rcsb.app.file-1.3.2/rcsb/app/file/KvRedis.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/KvSqlite.py` & `rcsb.app.file-1.3.2/rcsb/app/file/KvSqlite.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/PathProvider.py` & `rcsb.app.file-1.3.2/rcsb/app/file/PathProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/RedisLock.py` & `rcsb.app.file-1.3.2/rcsb/app/file/RedisLock.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/Sessions.py` & `rcsb.app.file-1.3.2/rcsb/app/file/Sessions.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/SoftLock.py` & `rcsb.app.file-1.3.2/rcsb/app/file/SoftLock.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/TernaryLock.py` & `rcsb.app.file-1.3.2/rcsb/app/file/TernaryLock.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/UploadUtility.py` & `rcsb.app.file-1.3.2/rcsb/app/file/UploadUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,17 @@
                 try:
                     async with Locking(filePath, "w"):
                         # save final version
                         os.replace(tempPath, filePath)
                         # decompress
                         if decompress and fileExtension:
                             await self.decompressFile(filePath, fileExtension)
+                        # change permissions
+                        default_file_permissions = self.cP.get("DEFAULT_FILE_PERMISSIONS")
+                        os.chmod(filePath, default_file_permissions)
                 except (FileExistsError, OSError) as err:
                     raise HTTPException(status_code=400, detail="error %r" % err)
                 # clear database and temp files
                 await session.close(tempPath, resumable, mapKey)
         except HTTPException as exc:
             await session.close(tempPath, resumable, mapKey)
             raise HTTPException(status_code=exc.status_code, detail=exc.detail)
```

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/downloadRequest.py` & `rcsb.app.file-1.3.2/rcsb/app/file/downloadRequest.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/ioRequest.py` & `rcsb.app.file-1.3.2/rcsb/app/file/ioRequest.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/main.py` & `rcsb.app.file-1.3.2/rcsb/app/file/main.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/pathRequest.py` & `rcsb.app.file-1.3.2/rcsb/app/file/pathRequest.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/serverStatus.py` & `rcsb.app.file-1.3.2/rcsb/app/file/serverStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/serverStatusRequest.py` & `rcsb.app.file-1.3.2/rcsb/app/file/serverStatusRequest.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/tokenRequest.py` & `rcsb.app.file-1.3.2/rcsb/app/file/tokenRequest.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb/app/file/uploadRequest.py` & `rcsb.app.file-1.3.2/rcsb/app/file/uploadRequest.py`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/rcsb.app.file.egg-info/PKG-INFO` & `rcsb.app.file-1.3.2/rcsb.app.file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.app.file
-Version: 1.3.1
+Version: 1.3.2
 Summary: RCSB File Access Service Application
 Home-page: https://github.com/rcsb/py-rcsb_app_file
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -364,17 +364,17 @@
 (or service redis stop, but not if Redis was started with /usr/bin/redis-server)
 ```
 
 To view Redis variables
 ```
 
 redis-cli
-KEYS *
-GET keyname
-HGETALL hashkey
+KEYS * (prints two values)
+GET keyname (for keyname, copy/paste the first value)
+HGETALL hashkey (for hashkey, copy/paste the second value)
 exit
 
 ```
 
 To remove all variables
 ```
```

### Comparing `rcsb.app.file-1.3.1/rcsb.app.file.egg-info/SOURCES.txt` & `rcsb.app.file-1.3.2/rcsb.app.file.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.app.file-1.3.1/setup.py` & `rcsb.app.file-1.3.2/setup.py`

 * *Files identical despite different names*

