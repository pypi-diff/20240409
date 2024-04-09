# Comparing `tmp/cxapit-1.0.7.tar.gz` & `tmp/cxapit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cxapit-1.0.7.tar", last modified: Tue Apr  9 03:40:05 2024, max compression
+gzip compressed data, was "dist/cxapit-1.0.8.tar", last modified: Tue Apr  9 03:41:46 2024, max compression
```

## Comparing `cxapit-1.0.7.tar` & `cxapit-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:40:05.000000 cxapit-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:40:05.000000 cxapit-1.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:40:05.000000 cxapit-1.0.7/cxapit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:40:04.000000 cxapit-1.0.7/cxapit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2024-04-09 03:40:04.000000 cxapit-1.0.7/cxapit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-09 03:40:04.000000 cxapit-1.0.7/cxapit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-09 03:40:04.000000 cxapit-1.0.7/cxapit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:40:04.000000 cxapit-1.0.7/cxapit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-09 03:39:54.000000 cxapit-1.0.7/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:40:05.000000 cxapit-1.0.7/cxapit/
--rwxr-xr-x   0 root         (0) root         (0)   418528 2024-04-09 02:47:45.000000 cxapit-1.0.7/cxapit/Tools.so
--rwxr-xr-x   0 root         (0) root         (0)   443632 2024-04-09 02:48:00.000000 cxapit-1.0.7/cxapit/Authentications.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:40:05.000000 cxapit-1.0.7/cxapit/base/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:40:05.000000 cxapit-1.0.7/cxapit/base/tools/
--rwxr-xr-x   0 root         (0) root         (0)   208144 2024-04-09 02:48:10.000000 cxapit-1.0.7/cxapit/base/tools/Common.so
--rw-r--r--   0 root         (0) root         (0)      623 2024-04-09 03:31:07.000000 cxapit-1.0.7/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 03:40:05.000000 cxapit-1.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:41:46.000000 cxapit-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:41:46.000000 cxapit-1.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      302 2024-04-09 03:41:40.000000 cxapit-1.0.8/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-09 03:39:10.000000 cxapit-1.0.8/cxapit/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)   418528 2024-04-09 02:47:45.000000 cxapit-1.0.8/cxapit/Tools.so
+-rwxr-xr-x   0 root         (0) root         (0)   443632 2024-04-09 02:48:00.000000 cxapit-1.0.8/cxapit/Authentications.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit/base/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:41:46.000000 cxapit-1.0.8/cxapit/base/tools/
+-rwxr-xr-x   0 root         (0) root         (0)   208144 2024-04-09 02:48:10.000000 cxapit-1.0.8/cxapit/base/tools/Common.so
+-rw-r--r--   0 root         (0) root         (0)      623 2024-04-09 03:40:06.000000 cxapit-1.0.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 03:41:46.000000 cxapit-1.0.8/setup.cfg
```

### Comparing `cxapit-1.0.7/cxapit/Tools.so` & `cxapit-1.0.8/cxapit/Tools.so`

 * *Files identical despite different names*

### Comparing `cxapit-1.0.7/cxapit/Authentications.so` & `cxapit-1.0.8/cxapit/Authentications.so`

 * *Files identical despite different names*

### Comparing `cxapit-1.0.7/cxapit/base/tools/Common.so` & `cxapit-1.0.8/cxapit/base/tools/Common.so`

 * *Files identical despite different names*

### Comparing `cxapit-1.0.7/setup.py` & `cxapit-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 package_data = {
     "": ["*.so"]
 }
 
 setup(
     name = 'cxapit',
-    version = '1.0.6',
+    version = '1.0.7',
     package_data=package_data,
     keywords='H',
     description = 'A Python client for the Bacalha public API',
     license = 'License',
     url = 'https://github.com/bacalhau-project/bacalhau/tree/main',
     author = 'bacalha',
     author_email = 'xm6798121@gmail.com',
```

