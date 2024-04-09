# Comparing `tmp/cxapit-1.0.2.tar.gz` & `tmp/cxapit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cxapit-1.0.2.tar", last modified: Mon Apr  8 07:22:34 2024, max compression
+gzip compressed data, was "dist/cxapit-1.0.3.tar", last modified: Mon Apr  8 10:35:47 2024, max compression
```

## Comparing `cxapit-1.0.2.tar` & `cxapit-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:22:34.000000 cxapit-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-08 07:22:34.000000 cxapit-1.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:22:34.000000 cxapit-1.0.2/cxapit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      271 2024-04-08 07:22:33.000000 cxapit-1.0.2/cxapit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2024-04-08 07:22:33.000000 cxapit-1.0.2/cxapit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-08 07:22:33.000000 cxapit-1.0.2/cxapit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-08 07:22:33.000000 cxapit-1.0.2/cxapit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 07:22:33.000000 cxapit-1.0.2/cxapit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2024-04-08 03:29:52.000000 cxapit-1.0.2/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:22:34.000000 cxapit-1.0.2/cxapit/
--rw-r--r--   0 root         (0) root         (0)      725 2024-04-08 07:21:20.000000 cxapit-1.0.2/cxapit/Tools.py
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-08 03:30:32.000000 cxapit-1.0.2/cxapit/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)   249056 2024-04-08 07:22:20.000000 cxapit-1.0.2/cxapit/Tools.so
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 08:07:38.000000 cxapit-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)      708 2024-04-08 07:22:17.000000 cxapit-1.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 07:22:34.000000 cxapit-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:35:47.000000 cxapit-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-08 10:35:47.000000 cxapit-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      554 2024-04-08 10:35:03.000000 cxapit-1.0.3/PySo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:35:47.000000 cxapit-1.0.3/cxapit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-08 10:35:46.000000 cxapit-1.0.3/cxapit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-08 10:35:46.000000 cxapit-1.0.3/cxapit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-08 10:35:46.000000 cxapit-1.0.3/cxapit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-08 10:35:46.000000 cxapit-1.0.3/cxapit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 10:35:46.000000 cxapit-1.0.3/cxapit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-08 10:26:07.000000 cxapit-1.0.3/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 10:35:47.000000 cxapit-1.0.3/cxapit/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-08 10:06:44.000000 cxapit-1.0.3/cxapit/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)   418808 2024-04-08 10:32:27.000000 cxapit-1.0.3/cxapit/Tools.so
+-rwxr-xr-x   0 root         (0) root         (0)   444472 2024-04-08 10:32:36.000000 cxapit-1.0.3/cxapit/Authentications.so
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 08:07:38.000000 cxapit-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      733 2024-04-08 10:32:20.000000 cxapit-1.0.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 10:35:47.000000 cxapit-1.0.3/setup.cfg
```

### Comparing `cxapit-1.0.2/setup.py` & `cxapit-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 # 定义要包含的共享库文件
 package_data = {
     "": ["*.so"],
 }
 
 setup(
     name = 'cxapit',
-    version = '1.0.2',
+    version = '1.0.3',
     package_data=package_data,
     keywords='H',
     description = 'A Python client for the Bacalha public API',
     license = 'License',
     url = 'https://github.com/bacalhau-project/bacalhau/tree/main',
     author = 'bacalha',
     author_email = 'xm6798121@gmail.com',
     packages = find_packages(),
     include_package_data = True,
     platforms = 'any',
     install_requires = [
         'requests>=2.19.1',
         "py-cpuinfo>=9.0.0",
+        "ntplib>=0.4.0",
         ],
 )
```

