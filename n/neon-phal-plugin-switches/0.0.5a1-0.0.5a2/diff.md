# Comparing `tmp/neon-phal-plugin-switches-0.0.5a1.tar.gz` & `tmp/neon-phal-plugin-switches-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-switches-0.0.5a1.tar", last modified: Fri Jun 16 00:00:19 2023, max compression
+gzip compressed data, was "neon-phal-plugin-switches-0.0.5a2.tar", last modified: Mon Apr  8 23:16:18 2024, max compression
```

## Comparing `neon-phal-plugin-switches-0.0.5a1.tar` & `neon-phal-plugin-switches-0.0.5a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.830643 neon-phal-plugin-switches-0.0.5a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-16 00:00:15.000000 neon-phal-plugin-switches-0.0.5a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 00:00:19.830643 neon-phal-plugin-switches-0.0.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 00:00:15.000000 neon-phal-plugin-switches-0.0.5a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.826643 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches/
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-16 00:00:15.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:00:19.830643 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 00:00:19.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 00:00:19.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:00:19.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 00:00:19.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 00:00:19.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 00:00:19.000000 neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 00:00:19.830643 neon-phal-plugin-switches-0.0.5a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-16 00:00:15.000000 neon-phal-plugin-switches-0.0.5a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:18.494199 neon-phal-plugin-switches-0.0.5a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 23:16:13.000000 neon-phal-plugin-switches-0.0.5a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 23:16:18.494199 neon-phal-plugin-switches-0.0.5a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 23:16:13.000000 neon-phal-plugin-switches-0.0.5a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:18.494199 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-08 23:16:13.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:18.494199 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 23:16:18.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 23:16:18.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:16:18.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 23:16:18.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 23:16:18.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 23:16:18.000000 neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:16:18.494199 neon-phal-plugin-switches-0.0.5a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-08 23:16:13.000000 neon-phal-plugin-switches-0.0.5a2/setup.py
```

### Comparing `neon-phal-plugin-switches-0.0.5a1/LICENSE.md` & `neon-phal-plugin-switches-0.0.5a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-switches-0.0.5a1/PKG-INFO` & `neon-phal-plugin-switches-0.0.5a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-switches
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: Hardware Switch Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-switches
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches/__init__.py` & `neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-switches-0.0.5a1/neon_phal_plugin_switches.egg-info/PKG-INFO` & `neon-phal-plugin-switches-0.0.5a2/neon_phal_plugin_switches.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-switches
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: Hardware Switch Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-switches
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-switches-0.0.5a1/setup.py` & `neon-phal-plugin-switches-0.0.5a2/setup.py`

 * *Files identical despite different names*

