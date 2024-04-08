# Comparing `tmp/neon-phal-plugin-linear_led-0.2.2a2.tar.gz` & `tmp/neon-phal-plugin-linear_led-0.2.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-linear_led-0.2.2a2.tar", last modified: Tue Jun 27 17:08:28 2023, max compression
+gzip compressed data, was "neon-phal-plugin-linear_led-0.2.3a1.tar", last modified: Mon Apr  8 23:16:43 2024, max compression
```

## Comparing `neon-phal-plugin-linear_led-0.2.2a2.tar` & `neon-phal-plugin-linear_led-0.2.3a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:08:28.325366 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/
--rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/neopixel_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/smbus_led.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:43.207287 neon-phal-plugin-linear_led-0.2.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 23:16:37.000000 neon-phal-plugin-linear_led-0.2.3a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-08 23:16:43.207287 neon-phal-plugin-linear_led-0.2.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-08 23:16:37.000000 neon-phal-plugin-linear_led-0.2.3a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:43.207287 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/
+-rw-r--r--   0 runner    (1001) docker     (127)    18591 2024-04-08 23:16:37.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-08 23:16:37.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/neopixel_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-08 23:16:37.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/smbus_led.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:16:43.207287 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-08 23:16:43.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 23:16:43.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:16:43.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 23:16:43.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 23:16:43.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 23:16:43.000000 neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:16:43.207287 neon-phal-plugin-linear_led-0.2.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-08 23:16:37.000000 neon-phal-plugin-linear_led-0.2.3a1/setup.py
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/LICENSE.md` & `neon-phal-plugin-linear_led-0.2.3a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/PKG-INFO` & `neon-phal-plugin-linear_led-0.2.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear_led
-Version: 0.2.2a2
+Version: 0.2.3a1
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/README.md` & `neon-phal-plugin-linear_led-0.2.3a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/__init__.py` & `neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from threading import RLock
 
 from ovos_bus_client import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.templates.phal import PHALPlugin
 from ovos_plugin_manager.hardware.led import Color, AbstractLed
 from ovos_plugin_manager.hardware.led.animations import BreatheLedAnimation, \
-    FillLedAnimation, BlinkLedAnimation, AlternatingLedAnimation,\
+    FillLedAnimation, BlinkLedAnimation, AlternatingLedAnimation, \
     animations, LedAnimation
 from ovos_utils.network_utils import is_connected
 
 
 def transient_animation(func):
     """
     Mark a method as transient and check for persistent states on animation end.
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/neopixel_led.py` & `neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/neopixel_led.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/smbus_led.py` & `neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led/smbus_led.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/PKG-INFO` & `neon-phal-plugin-linear_led-0.2.3a1/neon_phal_plugin_linear_led.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear-led
-Version: 0.2.2a2
+Version: 0.2.3a1
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a2/setup.py` & `neon-phal-plugin-linear_led-0.2.3a1/setup.py`

 * *Files identical despite different names*

