# Comparing `tmp/neon-phal-plugin-monitoring-0.0.1a2.tar.gz` & `tmp/neon-phal-plugin-monitoring-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-monitoring-0.0.1a2.tar", last modified: Fri Nov 17 03:08:55 2023, max compression
+gzip compressed data, was "neon-phal-plugin-monitoring-0.0.2a1.tar", last modified: Mon Apr  8 23:16:29 2024, max compression
```

## Comparing `neon-phal-plugin-monitoring-0.0.1a2.tar` & `neon-phal-plugin-monitoring-0.0.2a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 03:08:55.725132 neon-phal-plugin-monitoring-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-11-17 03:08:51.000000 neon-phal-plugin-monitoring-0.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-11-17 03:08:55.725132 neon-phal-plugin-monitoring-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-11-17 03:08:51.000000 neon-phal-plugin-monitoring-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 03:08:55.721132 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2023-11-17 03:08:51.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 03:08:55.725132 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-11-17 03:08:55.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-17 03:08:55.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 03:08:55.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-17 03:08:55.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-17 03:08:55.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-17 03:08:55.000000 neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 03:08:55.725132 neon-phal-plugin-monitoring-0.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2023-11-17 03:08:51.000000 neon-phal-plugin-monitoring-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:29.670343 neon-phal-plugin-monitoring-0.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 23:16:26.000000 neon-phal-plugin-monitoring-0.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-08 23:16:29.670343 neon-phal-plugin-monitoring-0.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 23:16:26.000000 neon-phal-plugin-monitoring-0.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:29.670343 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-08 23:16:26.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:29.670343 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-08 23:16:29.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 23:16:29.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:16:29.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 23:16:29.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 23:16:29.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 23:16:29.000000 neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:16:29.670343 neon-phal-plugin-monitoring-0.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-08 23:16:26.000000 neon-phal-plugin-monitoring-0.0.2a1/setup.py
```

### Comparing `neon-phal-plugin-monitoring-0.0.1a2/LICENSE.md` & `neon-phal-plugin-monitoring-0.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-monitoring-0.0.1a2/PKG-INFO` & `neon-phal-plugin-monitoring-0.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-monitoring
-Version: 0.0.1a2
+Version: 0.0.2a1
 Summary: Core Monitoring Service
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-monitoring
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-monitoring-0.0.1a2/README.md` & `neon-phal-plugin-monitoring-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring/__init__.py` & `neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-monitoring-0.0.1a2/neon_phal_plugin_monitoring.egg-info/PKG-INFO` & `neon-phal-plugin-monitoring-0.0.2a1/neon_phal_plugin_monitoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-monitoring
-Version: 0.0.1a2
+Version: 0.0.2a1
 Summary: Core Monitoring Service
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-monitoring
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-monitoring-0.0.1a2/setup.py` & `neon-phal-plugin-monitoring-0.0.2a1/setup.py`

 * *Files identical despite different names*

