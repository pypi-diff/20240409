# Comparing `tmp/rhdzmota_extension_hello_world-0.1.2.tar.gz` & `tmp/rhdzmota_extension_hello_world-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdzmota_extension_hello_world-0.1.2.tar", last modified: Sun Apr  7 23:42:59 2024, max compression
+gzip compressed data, was "rhdzmota_extension_hello_world-0.1.3.tar", last modified: Tue Apr  9 04:56:07 2024, max compression
```

## Comparing `rhdzmota_extension_hello_world-0.1.2.tar` & `rhdzmota_extension_hello_world-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.055406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/enums/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/enums/salutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world_version
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 23:42:43.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota/ext/hello_world_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:42:59.059406 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 23:42:59.000000 rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/enums/salutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world_version
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 04:55:51.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota/ext/hello_world_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:56:07.979475 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 04:56:07.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-09 04:56:07.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:56:07.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:56:07.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 04:56:07.000000 rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/top_level.txt
```

### Comparing `rhdzmota_extension_hello_world-0.1.2/PKG-INFO` & `rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rhdzmota_extension_hello_world
-Version: 0.1.2
+Name: rhdzmota-extension-hello-world
+Version: 0.1.3
 Summary: RHDZMOTA Extension App: hello_world
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_hello_world-0.1.2/README.md` & `rhdzmota_extension_hello_world-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_hello_world-0.1.2/setup.py` & `rhdzmota_extension_hello_world-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/PKG-INFO` & `rhdzmota_extension_hello_world-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rhdzmota-extension-hello-world
-Version: 0.1.2
+Name: rhdzmota_extension_hello_world
+Version: 0.1.3
 Summary: RHDZMOTA Extension App: hello_world
 Home-page: https://github.com/rhdzmota/package.rhdzmota.com
 Author: Rodrigo H. Mota
 Author-email: info@rhdzmota.com
 License: TBD
 Classifier: Typing :: Typed
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rhdzmota_extension_hello_world-0.1.2/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt` & `rhdzmota_extension_hello_world-0.1.3/src/main/rhdzmota_extension_hello_world.egg-info/SOURCES.txt`

 * *Files identical despite different names*

