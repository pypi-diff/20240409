# Comparing `tmp/cxapit-1.0.5.tar.gz` & `tmp/cxapit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cxapit-1.0.5.tar", last modified: Tue Apr  9 03:07:34 2024, max compression
+gzip compressed data, was "dist/cxapit-1.0.6.tar", last modified: Tue Apr  9 03:31:06 2024, max compression
```

## Comparing `cxapit-1.0.5.tar` & `cxapit-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:34.000000 cxapit-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:07:34.000000 cxapit-1.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:34.000000 cxapit-1.0.5/cxapit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:07:33.000000 cxapit-1.0.5/cxapit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      257 2024-04-09 03:07:33.000000 cxapit-1.0.5/cxapit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-09 03:07:33.000000 cxapit-1.0.5/cxapit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:07:33.000000 cxapit-1.0.5/cxapit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:07:33.000000 cxapit-1.0.5/cxapit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2024-04-09 03:07:27.000000 cxapit-1.0.5/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:34.000000 cxapit-1.0.5/cxapit/
--rwxr-xr-x   0 root         (0) root         (0)   418528 2024-04-09 02:47:45.000000 cxapit-1.0.5/cxapit/Tools.so
--rwxr-xr-x   0 root         (0) root         (0)   443632 2024-04-09 02:48:00.000000 cxapit-1.0.5/cxapit/Authentications.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:34.000000 cxapit-1.0.5/cxapit/base/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:34.000000 cxapit-1.0.5/cxapit/base/tools/
--rwxr-xr-x   0 root         (0) root         (0)   208144 2024-04-09 02:48:10.000000 cxapit-1.0.5/cxapit/base/tools/Common.so
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 08:07:38.000000 cxapit-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)     1520 2024-04-09 03:00:26.000000 cxapit-1.0.5/setup.py
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 03:07:33.000000 cxapit-1.0.5/Version
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 03:07:34.000000 cxapit-1.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:31:06.000000 cxapit-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:31:06.000000 cxapit-1.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:31:06.000000 cxapit-1.0.6/cxapit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-09 03:31:05.000000 cxapit-1.0.6/cxapit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2024-04-09 03:31:05.000000 cxapit-1.0.6/cxapit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-09 03:31:05.000000 cxapit-1.0.6/cxapit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:31:05.000000 cxapit-1.0.6/cxapit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:31:05.000000 cxapit-1.0.6/cxapit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-09 03:30:46.000000 cxapit-1.0.6/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:31:06.000000 cxapit-1.0.6/cxapit/
+-rwxr-xr-x   0 root         (0) root         (0)   418528 2024-04-09 02:47:45.000000 cxapit-1.0.6/cxapit/Tools.so
+-rwxr-xr-x   0 root         (0) root         (0)   443632 2024-04-09 02:48:00.000000 cxapit-1.0.6/cxapit/Authentications.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:31:06.000000 cxapit-1.0.6/cxapit/base/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:31:06.000000 cxapit-1.0.6/cxapit/base/tools/
+-rwxr-xr-x   0 root         (0) root         (0)   208144 2024-04-09 02:48:10.000000 cxapit-1.0.6/cxapit/base/tools/Common.so
+-rw-r--r--   0 root         (0) root         (0)      623 2024-04-09 03:29:34.000000 cxapit-1.0.6/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 03:31:06.000000 cxapit-1.0.6/setup.cfg
```

### Comparing `cxapit-1.0.5/cxapit/Tools.so` & `cxapit-1.0.6/cxapit/Tools.so`

 * *Files identical despite different names*

### Comparing `cxapit-1.0.5/cxapit/Authentications.so` & `cxapit-1.0.6/cxapit/Authentications.so`

 * *Files identical despite different names*

### Comparing `cxapit-1.0.5/cxapit/base/tools/Common.so` & `cxapit-1.0.6/cxapit/base/tools/Common.so`

 * *Files identical despite different names*

