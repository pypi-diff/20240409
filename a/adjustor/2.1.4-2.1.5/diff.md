# Comparing `tmp/adjustor-2.1.4.tar.gz` & `tmp/adjustor-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adjustor-2.1.4.tar", last modified: Sun Apr  7 16:34:10 2024, max compression
+gzip compressed data, was "adjustor-2.1.5.tar", last modified: Tue Apr  9 17:32:46 2024, max compression
```

## Comparing `adjustor-2.1.4.tar` & `adjustor-2.1.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.368099 adjustor-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 16:34:04.000000 adjustor-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-07 16:34:04.000000 adjustor-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-07 16:34:10.364099 adjustor-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-07 16:34:04.000000 adjustor-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-07 16:34:04.000000 adjustor-2.1.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:34:10.368099 adjustor-2.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.360099 adjustor-2.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.360099 adjustor-2.1.4/src/adjustor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/acpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/alib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/lenovo.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/asus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/asus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/asus/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/lenovo/
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/lenovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/lenovo/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/smu/
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/smu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/smu/qam.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/smu/smu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/hhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 17:32:40.000000 adjustor-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 17:32:40.000000 adjustor-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-09 17:32:46.464179 adjustor-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 17:32:40.000000 adjustor-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 17:32:40.000000 adjustor-2.1.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:32:46.464179 adjustor-2.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.456179 adjustor-2.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.460179 adjustor-2.1.5/src/adjustor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/src/adjustor/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/core/acpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/core/alib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/core/lenovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/core/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/src/adjustor/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/src/adjustor/drivers/asus/
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/asus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/asus/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/src/adjustor/drivers/lenovo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/lenovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/lenovo/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/src/adjustor/drivers/smu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/smu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/smu/qam.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/drivers/smu/smu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/hhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 17:32:40.000000 adjustor-2.1.5/src/adjustor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:32:46.464179 adjustor-2.1.5/src/adjustor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-09 17:32:46.000000 adjustor-2.1.5/src/adjustor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-09 17:32:46.000000 adjustor-2.1.5/src/adjustor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:32:46.000000 adjustor-2.1.5/src/adjustor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 17:32:46.000000 adjustor-2.1.5/src/adjustor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 17:32:46.000000 adjustor-2.1.5/src/adjustor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:32:46.000000 adjustor-2.1.5/src/adjustor.egg-info/top_level.txt
```

### Comparing `adjustor-2.1.4/LICENSE` & `adjustor-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/PKG-INFO` & `adjustor-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustor
-Version: 2.1.4
+Version: 2.1.5
 Summary: Adjustor, a userspace program for managing the TDP of handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/adjustor
 Project-URL: Bug Tracker, https://github.com/hhd-dev/adjustor/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adjustor-2.1.4/pyproject.toml` & `adjustor-2.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "adjustor"
-version = "2.1.4"
+version = "2.1.5"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Adjustor, a userspace program for managing the TDP of handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `adjustor-2.1.4/readme.md` & `adjustor-2.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/core/acpi.py` & `adjustor-2.1.5/src/adjustor/core/acpi.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/core/alib.py` & `adjustor-2.1.5/src/adjustor/core/alib.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/core/const.py` & `adjustor-2.1.5/src/adjustor/core/const.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/core/lenovo.py` & `adjustor-2.1.5/src/adjustor/core/lenovo.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/core/platform.py` & `adjustor-2.1.5/src/adjustor/core/platform.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/drivers/asus/__init__.py` & `adjustor-2.1.5/src/adjustor/drivers/asus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,28 @@
 # [ 4  8  ]
 
 POINTS = [30, 40, 50, 60, 70, 80, 90, 100]
 MIN_CURVE = [2, 5, 17, 17, 17, 17, 17, 17]
 DEFAULT_CURVE = [5, 10, 20, 35, 55, 75, 75, 75]
 
 
+def set_charge_limit(lim: int):
+    try:
+        # FIXME: Hardcoded path, should match using another characteristic
+        logger.info(f"Setting charge limit to {lim:d} %.")
+        with open(
+            "/sys/class/power_supply/BAT0/charge_control_end_threshold", "w"
+        ) as f:
+            f.write(f"{lim}\n")
+        return True
+    except Exception as e:
+        logger.error(f"Failed to write battery limit with error:\n{e}")
+        return False
+
+
 def set_tdp(pretty: str, fn: str, val: int):
     logger.info(f"Setting tdp value '{pretty}' to {val} by writing to:\n{fn}")
     try:
         with open(fn, "w") as f:
             f.write(f"{val}\n")
         return True
     except Exception as e:
@@ -144,14 +158,38 @@
         # If not old config, exit, as values can not be set
         if not self.old_conf:
             self.old_conf = conf["tdp.asus"]
             return
 
         curr = time.time()
 
+        # Charge limit
+        lim = conf["tdp.asus.charge_limit"].to(str)
+        if (self.startup and lim != "disabled") or (
+            lim != self.old_conf["charge_limit"].to(str)
+        ):
+            match lim:
+                case "p65":
+                    set_charge_limit(65)
+                case "p70":
+                    set_charge_limit(70)
+                case "p80":
+                    set_charge_limit(80)
+                case "p85":
+                    set_charge_limit(85)
+                case "p90":
+                    set_charge_limit(90)
+                case "p95":
+                    set_charge_limit(95)
+                case "disabled":
+                    # Avoid writing charge limit on startup if
+                    # disabled
+                    if not self.startup:
+                        set_charge_limit(100)
+
         #
         # TDP
         #
 
         # Reset fan curve on mode change
         # Has to happen before setting the stdp, ftdp values, in case
         # we are in custom mode
```

### Comparing `adjustor-2.1.4/src/adjustor/drivers/asus/settings.yml` & `adjustor-2.1.5/src/adjustor/drivers/asus/settings.yml`

 * *Files 16% similar despite different names*

```diff
@@ -91,8 +91,36 @@
               Restore a default sane fan curve.
 
           disclaimer:
             title: Fan Curve Limitation
             type: display
             default: >-
               Asus hardware limits the minimum fan curve depending on TDP.
-              The minimums are 25%, 50%, and 75% for low, middle, and high TDPs.
+              The minimums are 25%, 50%, and 75% for low, medium, and high TDPs.
+
+  charge_limit:
+    type: multiple
+    title: Charge Limit (%)
+    tags: [ non-essential ]
+    hint: >-
+      Applies a charge limit to the battery, 75% and up.
+    options:
+      disabled: Disabled
+      p65: 65%
+      p70: 70%
+      p80: 80%
+      p85: 85%
+      p90: 90%
+      p95: 95%
+    default: disabled
+  
+  disclaimer:
+    title: Sleep Bug
+    type: display
+    tags: [ non-essential ]
+    default: >-
+      There is an Asus kernel/BIOS bug that will sometimes limit TDP to 10W
+      after sleep.
+      As the kernel driver is used, this is unfixable from within
+      Handheld Daemon (currently investigated).
+      As an alternative, use SimpleDeckyTDP with RyzenAdj after
+      disabling TDP controls from "Settings".
```

### Comparing `adjustor-2.1.4/src/adjustor/drivers/lenovo/__init__.py` & `adjustor-2.1.5/src/adjustor/drivers/lenovo/__init__.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/drivers/lenovo/settings.yml` & `adjustor-2.1.5/src/adjustor/drivers/lenovo/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/drivers/smu/__init__.py` & `adjustor-2.1.5/src/adjustor/drivers/smu/__init__.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/drivers/smu/smu.yml` & `adjustor-2.1.5/src/adjustor/drivers/smu/smu.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 type: container
 title: Advanced Configurator
 tags: [advanced, expert]
-hint: >-
 children:
   apply:
     type: action
     title: Apply Settings
 
   status:
     title: TDP Status
```

### Comparing `adjustor-2.1.4/src/adjustor/events.py` & `adjustor-2.1.5/src/adjustor/events.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/hhd.py` & `adjustor-2.1.5/src/adjustor/hhd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
 import os
-from threading import Event as TEvent, Thread
+from threading import Event as TEvent
+from threading import Thread
 from typing import Sequence
 
-from hhd.utils import expanduser
 from hhd.plugins import Context, HHDPlugin, HHDSettings, load_relative_yaml
 from hhd.plugins.conf import Config
 from hhd.plugins.plugin import Emitter
+from hhd.utils import expanduser
 
 from adjustor.core.acpi import check_perms, initialize
 from adjustor.core.const import CPU_DATA, DEV_DATA, ROG_ALLY_PP_MAP
 
+from .i18n import _
 from .utils import exists_sentinel, install_sentinel, remove_sentinel
 
 logger = logging.getLogger(__name__)
 
 CONFLICTING_PLUGINS = {
     "SimpleDeckyTDP": "~/homebrew/plugins/SimpleDeckyTDP",
     "PowerControl": "~/homebrew/plugins/PowerControl",
@@ -51,30 +53,29 @@
             conf["hhd.settings.tdp_enable"] = True
 
         old_enabled = conf["hhd.settings.tdp_enable"].to(bool)
         if self.failed:
             conf["hhd.settings.tdp_enable"] = False
         if self.safe_mode:
             logger.warning(f"Due to a sentinel error, auto-start is disabled.")
-            conf["tdp.tdp.tdp_error"] = (
+            conf["tdp.tdp.tdp_error"] = _(
                 "Due to a suspected crash, auto-start was disabled."
             )
             conf["hhd.settings.tdp_enable"] = False
             self.safe_mode = False
 
         self.enabled = conf["hhd.settings.tdp_enable"].to(bool)
 
         if self.init or not old_enabled:
             return
 
         for name, path in CONFLICTING_PLUGINS.items():
             if os.path.exists(expanduser(path, self.context)):
-                err = (
-                    f'Found plugin "{name}" at the following path:\n{path}\n'
-                    + "TDP Controls can not be enabled while other TDP plugins are installed."
+                err = f'Found plugin "{name}" at the following path:\n{path}\n' + _(
+                    "TDP Controls can not be enabled while other TDP plugins are installed."
                 )
                 conf["tdp.tdp.tdp_error"] = err
                 conf["hhd.settings.tdp_enable"] = False
                 logger.error(err)
                 self.failed = True
                 self.enabled = False
                 return
@@ -165,16 +166,16 @@
         self._stop()
 
 
 def autodetect(existing: Sequence[HHDPlugin]) -> Sequence[HHDPlugin]:
     if len(existing):
         return existing
 
-    from .drivers.lenovo import LenovoDriverPlugin
     from .drivers.asus import AsusDriverPlugin
+    from .drivers.lenovo import LenovoDriverPlugin
     from .drivers.smu import SmuDriverPlugin, SmuQamPlugin
 
     drivers = []
     with open("/sys/devices/virtual/dmi/id/product_name") as f:
         prod = f.read().strip()
     with open("/proc/cpuinfo") as f:
         cpuinfo = f.read().strip()
```

### Comparing `adjustor-2.1.4/src/adjustor/settings.yml` & `adjustor-2.1.5/src/adjustor/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor/utils.py` & `adjustor-2.1.5/src/adjustor/utils.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.4/src/adjustor.egg-info/PKG-INFO` & `adjustor-2.1.5/src/adjustor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustor
-Version: 2.1.4
+Version: 2.1.5
 Summary: Adjustor, a userspace program for managing the TDP of handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/adjustor
 Project-URL: Bug Tracker, https://github.com/hhd-dev/adjustor/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adjustor-2.1.4/src/adjustor.egg-info/SOURCES.txt` & `adjustor-2.1.5/src/adjustor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 pyproject.toml
 readme.md
 src/adjustor/__init__.py
 src/adjustor/__main__.py
 src/adjustor/events.py
 src/adjustor/hhd.py
+src/adjustor/i18n.py
 src/adjustor/settings.yml
 src/adjustor/utils.py
 src/adjustor.egg-info/PKG-INFO
 src/adjustor.egg-info/SOURCES.txt
 src/adjustor.egg-info/dependency_links.txt
 src/adjustor.egg-info/entry_points.txt
 src/adjustor.egg-info/requires.txt
```

