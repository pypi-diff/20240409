# Comparing `tmp/pyprland-2.2.3.tar.gz` & `tmp/pyprland-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.3.tar", max compression
+gzip compressed data, was "pyprland-2.2.4.tar", max compression
```

## Comparing `pyprland-2.2.3.tar` & `pyprland-2.2.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.3/LICENSE
--rw-r--r--   0        0        0     4128 2024-04-07 10:28:36.716804 pyprland-2.2.3/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.3/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.3/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.3/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.3/pyprland/adapters/menus.py
--rwxr-xr-x   0        0        0    15682 2024-04-08 16:06:45.965533 pyprland-2.2.3/pyprland/command.py
--rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.3/pyprland/command.py.orig
--rw-r--r--   0        0        0     4190 2024-04-06 13:35:14.309864 pyprland-2.2.3/pyprland/common.py
--rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.2.3/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.3/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.3/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.3/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.3/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2589 2024-04-06 13:35:14.309864 pyprland-2.2.3/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.3/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.3/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.3/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.3/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.3/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.3/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.3/pyprland/plugins/nohup.out
--rw-r--r--   0        0        0     1309 2024-04-06 13:35:25.146759 pyprland-2.2.3/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    35361 2024-04-06 13:37:10.612283 pyprland-2.2.3/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.3/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4149 2024-04-06 13:38:00.979983 pyprland-2.2.3/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-05 20:13:47.397221 pyprland-2.2.3/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.3/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.3/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     3776 2024-04-08 16:06:05.055461 pyprland-2.2.3/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.3/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-08 16:06:45.952200 pyprland-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 pyprland-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.4/LICENSE
+-rw-r--r--   0        0        0     4119 2024-04-08 17:57:27.722353 pyprland-2.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.4/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.4/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.4/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.4/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.4/pyprland/adapters/units.py
+-rwxr-xr-x   0        0        0    16372 2024-04-09 21:30:26.098920 pyprland-2.2.4/pyprland/command.py
+-rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.4/pyprland/command.py.orig
+-rw-r--r--   0        0        0     7410 2024-04-09 21:29:20.927222 pyprland-2.2.4/pyprland/common.py
+-rw-r--r--   0        0        0     6555 2024-04-09 21:02:15.456507 pyprland-2.2.4/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.4/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.4/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.4/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.4/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.4/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.4/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.4/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.4/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.4/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.4/pyprland/plugins/monitors.py.orig
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.4/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.4/pyprland/plugins/nohup.out
+-rw-r--r--   0        0        0     1309 2024-04-06 13:35:25.146759 pyprland-2.2.4/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    35948 2024-04-09 21:16:20.505075 pyprland-2.2.4/pyprland/plugins/scratchpads.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.4/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.4/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.4/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.4/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.4/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     4003 2024-04-09 18:24:41.796795 pyprland-2.2.4/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.4/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-09 21:30:26.088919 pyprland-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4658 1970-01-01 00:00:00.000000 pyprland-2.2.4/PKG-INFO
```

### Comparing `pyprland-2.2.3/LICENSE` & `pyprland-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/README.md` & `pyprland-2.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 ![rect](https://github.com/hyprland-community/pyprland/assets/238622/3fab93b6-6445-4e7b-b757-035095b5c8e8)
 
 [![Hyprland](https://img.shields.io/badge/Made%20for-Hyprland-blue)](https://github.com/hyprwm/Hyprland)
 [![Discord](https://img.shields.io/discord/1055990214411169892?label=discord)](https://discord.gg/zzWqvcKRMy)
 
+[Documentation](https://github.com/hyprland-community/pyprland/wiki) • [Discussions](https://github.com/hyprland-community/pyprland/discussions) • [Changes History](https://github.com/hyprland-community/pyprland/releases) • [Share Your Setup](https://github.com/hyprland-community/pyprland/discussions/46)
+
+
 ## Enhance your Hyprland experience with Pyprland
 
 Welcome to Pyprland, your gateway to extending the capabilities of [Hyprland](https://hyprland.org/). Pyprland offers a plethora of plugins designed for simplicity and efficiency, allowing you to supercharge your productivity and customize your user experience.
 
 - Explore our variety of [plugins](https://github.com/hyprland-community/pyprland/wiki/Plugins) to tailor your Hyprland setup to your liking.
 - New users, check the [getting started](https://github.com/hyprland-community/pyprland/wiki/Getting-started) guide.
 
 
-[Documentation](https://github.com/hyprland-community/pyprland/wiki) • [Discussions](https://github.com/hyprland-community/pyprland/discussions) • [Changes History](https://github.com/hyprland-community/pyprland/releases) • [Share Your Setup](https://github.com/hyprland-community/pyprland/discussions/46)
-
-
 ## About Pyprland
 
 [![Packaging Status](https://repology.org/badge/vertical-allrepos/pyprland.svg)](https://repology.org/project/pyprland/versions)
 
 🎉 Hear what others are saying:
 - ["It just works very very well" - The Linux Cast (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February 2024
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
 
+## Contributing
+
+Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
+
+- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
+- Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
+
+and if you have coding skills you can also
+
+- Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
+- Write new plugins
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
-- **aiofiles** (Python package)
+    - **aiofiles**
 
 ## Latest major changes
 
 > [!note]
 > Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
@@ -57,23 +68,14 @@
 - Introduced [shortcuts_menu](https://github.com/hyprland-community/pyprland/wiki/shortcuts_menu) plugin.
 
 ### 1.8
 
 - Requires Hyprland >= 0.30
 - Added [layout_center](https://github.com/hyprland-community/pyprland/wiki/layout_center) plugin.
 
-## Developers
-
-Contribute to Pyprland in various ways:
-- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
-- Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki) or write new plugins.
-- Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
-
-Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
-
 ## Star History
 
 <a href="https://star-history.com/#fdev31/pyprland&Date">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline&theme=dark" />
     <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
```

#### html2text {}

```diff
@@ -1,49 +1,49 @@
 ![rect](https://github.com/hyprland-community/pyprland/assets/238622/3fab93b6-
 6445-4e7b-b757-035095b5c8e8) [![Hyprland](https://img.shields.io/badge/
 Made%20for-Hyprland-blue)](https://github.com/hyprwm/Hyprland) [![Discord]
 (https://img.shields.io/discord/1055990214411169892?label=discord)](https://
-discord.gg/zzWqvcKRMy) ## Enhance your Hyprland experience with Pyprland
-Welcome to Pyprland, your gateway to extending the capabilities of [Hyprland]
-(https://hyprland.org/). Pyprland offers a plethora of plugins designed for
-simplicity and efficiency, allowing you to supercharge your productivity and
-customize your user experience. - Explore our variety of [plugins](https://
-github.com/hyprland-community/pyprland/wiki/Plugins) to tailor your Hyprland
-setup to your liking. - New users, check the [getting started](https://
-github.com/hyprland-community/pyprland/wiki/Getting-started) guide.
-[Documentation](https://github.com/hyprland-community/pyprland/wiki) â¢
-[Discussions](https://github.com/hyprland-community/pyprland/discussions) â¢
-[Changes History](https://github.com/hyprland-community/pyprland/releases) â¢
-[Share Your Setup](https://github.com/hyprland-community/pyprland/discussions/
-46) ## About Pyprland [![Packaging Status](https://repology.org/badge/vertical-
-allrepos/pyprland.svg)](https://repology.org/project/pyprland/versions) ð
-Hear what others are saying: - ["It just works very very well" - The Linux Cast
-(video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February
-2024 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://
-www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://
-toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/
-js_json_intro.asp)) ## Dependencies - **Hyprland** >= 0.37 - **Python** >= 3.11
-- **aiofiles** (Python package) ## Latest major changes > [!note] > Check the
-[Releases change log](https://github.com/hyprland-community/pyprland/releases)
-for more information ### 2.2 - Added [wallpapers](https://github.com/hyprland-
-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/
-hyprland-community/pyprland/wiki/system_notifier) plugins. ### 2.1 - Requires
-Hyprland >= 0.37 - [Monitors](https://github.com/hyprland-community/pyprland/
-wiki/monitors) plugin improvements. ### 2.0 - New dependency: [aiofiles](https:
-//pypi.org/project/aiofiles/) - Added [hysteresis](https://github.com/hyprland-
+discord.gg/zzWqvcKRMy) [Documentation](https://github.com/hyprland-community/
+pyprland/wiki) â¢ [Discussions](https://github.com/hyprland-community/
+pyprland/discussions) â¢ [Changes History](https://github.com/hyprland-
+community/pyprland/releases) â¢ [Share Your Setup](https://github.com/
+hyprland-community/pyprland/discussions/46) ## Enhance your Hyprland experience
+with Pyprland Welcome to Pyprland, your gateway to extending the capabilities
+of [Hyprland](https://hyprland.org/). Pyprland offers a plethora of plugins
+designed for simplicity and efficiency, allowing you to supercharge your
+productivity and customize your user experience. - Explore our variety of
+[plugins](https://github.com/hyprland-community/pyprland/wiki/Plugins) to
+tailor your Hyprland setup to your liking. - New users, check the [getting
+started](https://github.com/hyprland-community/pyprland/wiki/Getting-started)
+guide. ## About Pyprland [![Packaging Status](https://repology.org/badge/
+vertical-allrepos/pyprland.svg)](https://repology.org/project/pyprland/
+versions) ð Hear what others are saying: - ["It just works very very well" -
+The Linux Cast (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131)
+- February 2024 - [You NEED This in your Hyprland Config - LibrePhoenix
+(video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now
+[TOML](https://toml.io/en/) format is preferred over [JSON](https://
+www.w3schools.com/js/js_json_intro.asp)) ## Contributing Check out the
+[creating a pull request](https://docs.github.com/fr/pull-requests/
+collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
+requests/creating-a-pull-request) document for guidance. - Report bugs or
+propose features [here](https://github.com/hyprland-community/pyprland/issues).
+- Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki) and
+if you have coding skills you can also - Enhance test coverage in our [tests]
+(https://github.com/hyprland-community/pyprland/tree/main/tests). - Write new
+plugins ## Dependencies - **Hyprland** >= 0.37 - **Python** >= 3.11 -
+**aiofiles** ## Latest major changes > [!note] > Check the [Releases change
+log](https://github.com/hyprland-community/pyprland/releases) for more
+information ### 2.2 - Added [wallpapers](https://github.com/hyprland-community/
+pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-
+community/pyprland/wiki/system_notifier) plugins. ### 2.1 - Requires Hyprland
+>= 0.37 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/
+monitors) plugin improvements. ### 2.0 - New dependency: [aiofiles](https://
+pypi.org/project/aiofiles/) - Added [hysteresis](https://github.com/hyprland-
 community/pyprland/wiki/scratchpads#hysteresis-optional) support for
 [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads).
 ### 1.10 - New [fetch_client_menu](https://github.com/hyprland-community/
 pyprland/wiki/fetch_client_menu) and [shortcuts_menu](https://github.com/
 hyprland-community/pyprland/wiki/shortcuts_menu) plugins. ### 1.9 - Introduced
 [shortcuts_menu](https://github.com/hyprland-community/pyprland/wiki/
 shortcuts_menu) plugin. ### 1.8 - Requires Hyprland >= 0.30 - Added
 [layout_center](https://github.com/hyprland-community/pyprland/wiki/
-layout_center) plugin. ## Developers Contribute to Pyprland in various ways: -
-Report bugs or propose features [here](https://github.com/hyprland-community/
-pyprland/issues). - Improve our [wiki](https://github.com/hyprland-community/
-pyprland/wiki) or write new plugins. - Enhance test coverage in our [tests]
-(https://github.com/hyprland-community/pyprland/tree/main/tests). Check out the
-[creating a pull request](https://docs.github.com/fr/pull-requests/
-collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
-requests/creating-a-pull-request) document for guidance. ## Star History_[_S_t_a_r
-_H_i_s_t_o_r_y_ _C_h_a_r_t_]
+layout_center) plugin. ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `pyprland-2.2.3/pyprland/adapters/menus.py` & `pyprland-2.2.4/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/command.py` & `pyprland-2.2.4/pyprland/command.py.orig`

 * *Files 2% similar despite different names*

```diff
@@ -344,15 +344,19 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.3")  # Automatically updated version
+<<<<<<< HEAD
+        print("2.1.4-21")  # Automatically updated version
+=======
+        print("2.1.4-19")  # Automatically updated version
+>>>>>>> ee2fea0 (mitigate code complexity)
         return
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
```

### Comparing `pyprland-2.2.3/pyprland/command.py.orig` & `pyprland-2.2.4/pyprland/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from functools import partial
 from typing import Self
 import tomllib
 import json
 import os
 import sys
 
-from pyprland.common import PyprError, get_logger, init_logger
+from pyprland.common import (
+    PyprError,
+    get_logger,
+    init_logger,
+    merge,
+    run_interactive_program,
+)
 from pyprland.ipc import get_event_stream, notify_error, notify_fatal, notify_info
 from pyprland.ipc import init as ipc_init
 from pyprland.plugins.interface import Plugin
 
 try:
     CONTROL = f'/tmp/hypr/{ os.environ["HYPRLAND_INSTANCE_SIGNATURE"] }/.pyprland.sock'
 except KeyError:
@@ -51,45 +57,56 @@
         self.queues = {}
         self._set_instance(self)
 
     async def initialize(self):
         "Initializes the main structures"
         await self.load_config()  # ensure sockets are connected first
 
-    async def __open_config(self):
+    async def __open_config(self, config_filename=""):
         """Loads config file as self.config"""
-        if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
-            self.log.warning("Consider changing your configuration to TOML format.")
+        if config_filename:
+            fname = os.path.expandvars(os.path.expanduser(config_filename))
+        else:
+            if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
+                self.log.warning("Consider changing your configuration to TOML format.")
+
+            self.config.clear()
+            fname = os.path.expanduser(CONFIG_FILE)
 
-        self.config.clear()
-        fname = os.path.expanduser(CONFIG_FILE)
+        config = {}
         if os.path.exists(fname):
             self.log.info("Loading %s", fname)
             try:
                 with open(fname, "rb") as f:
-                    self.config.update(tomllib.load(f))
+                    config = tomllib.load(f)
             except FileNotFoundError as e:
                 self.log.critical(
                     "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
                 )
                 raise PyprError() from e
         elif os.path.exists(os.path.expanduser(OLD_CONFIG_FILE)):
             self.log.info("Loading %s", OLD_CONFIG_FILE)
             try:
                 with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
-                    self.config.update(json.loads(f.read()))
+                    config = json.loads(f.read())
             except FileNotFoundError as e:
                 self.log.critical(
                     "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
                 )
                 raise PyprError() from e
         else:
-            self.log.critical("No Config file found ! Please create %s", CONFIG_FILE)
+            self.log.critical("Config file not found! Please create %s", fname)
             raise PyprError()
 
+        if not config_filename:
+            for extra_config in list(config["pyprland"].get("include", [])):
+                merge(config, await self.__open_config(extra_config))
+            self.config.update(config)
+        return config
+
     async def _load_single_plugin(self, name, init) -> bool:
         "Load a single plugin, optionally calling `init`"
         if "." in name:
             modname = name
         elif "external:" in name:
             modname = name.replace("external:", "")
         else:
@@ -344,21 +361,23 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-<<<<<<< HEAD
-        print("2.1.4-21")  # Automatically updated version
-=======
-        print("2.1.4-19")  # Automatically updated version
->>>>>>> ee2fea0 (mitigate code complexity)
+        print("2.2.4")  # Automatically updated version
         return
 
+    if sys.argv[1] == "edit":
+        editor = os.environ.get("EDITOR", os.environ.get("VISUAL", "vi"))
+        filename = os.path.expanduser(CONFIG_FILE)
+        run_interactive_program(f'{editor} "{filename}"')
+        sys.argv[1] = "reload"
+
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
 
         print(
```

### Comparing `pyprland-2.2.3/pyprland/ipc.py` & `pyprland-2.2.4/pyprland/ipc.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "notify_info",
     "hyprctl",
     "hyprctlJSON",
 ]
 
 import asyncio
 import json
+import time
 import os
 from typing import Any
 from logging import Logger
 from functools import partial
 
 from .common import PyprError, get_logger
 
@@ -51,44 +52,59 @@
 def retry_on_reset(func):
     "wrapper to retry on reset"
 
     async def wrapper(*args, logger, **kwargs):
         exc = None
         for count in range(3):
             try:
-                return await func(*args, **kwargs)
+                return await func(*args, **kwargs, logger=logger)
             except ConnectionResetError as e:
                 exc = e
                 logger.warning("ipc connection problem, retrying...")
                 await asyncio.sleep(0.5 * count)
         logger.error("ipc connection failed.")
         raise ConnectionResetError() from exc
 
     return wrapper
 
 
+cached_responses: dict[str, list[Any]] = {
+    # <command name>: [expiration_date, payload, retention_time]
+    "monitors": [0, None, 0.1],
+    # "clients": [0, None, 0.02],
+}
+
+
 @retry_on_reset
 async def hyprctlJSON(
     command: str, logger=None
 ) -> list[dict[str, Any]] | dict[str, Any]:
     """Run an IPC command and return the JSON output."""
     logger = logger or log
+    now = time.time()
+    cached = command in cached_responses and cached_responses[command][0] > now
+    if cached:
+        logger.debug(f"{command} (CACHE HIT)")
+        return cached_responses[command][1]  # type: ignore
     logger.debug(command)
     try:
         ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
     except FileNotFoundError as e:
         logger.critical("hyprctl socket not found! is it running ?")
         raise PyprError() from e
     ctl_writer.write(f"-j/{command}".encode())
     await ctl_writer.drain()
     resp = await ctl_reader.read()
     ctl_writer.close()
     await ctl_writer.wait_closed()
     ret = json.loads(resp)
     assert isinstance(ret, (list, dict))
+    if command in cached_responses:  # should fill the cache
+        cached_responses[command][0] = now + cached_responses[command][2]
+        cached_responses[command][1] = ret
     return ret
 
 
 def _format_command(command_list, default_base_command):
     "helper function to format BATCH commands"
     for command in command_list:
         if isinstance(command, str):
```

### Comparing `pyprland-2.2.3/pyprland/plugins/expose.py` & `pyprland-2.2.4/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.4/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/interface.py` & `pyprland-2.2.4/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/layout_center.py` & `pyprland-2.2.4/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/lost_windows.py` & `pyprland-2.2.4/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/magnify.py` & `pyprland-2.2.4/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/monitors.py` & `pyprland-2.2.4/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/monitors.py.orig` & `pyprland-2.2.4/pyprland/plugins/monitors.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.4/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/pyprland.py` & `pyprland-2.2.4/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/scratchpads.py` & `pyprland-2.2.4/pyprland/plugins/scratchpads.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,64 +9,34 @@
 
 from aiofiles import os as aios
 from aiofiles import open as aiopen
 
 from ..ipc import notify_error, get_client_props, get_focused_monitor_props
 from .interface import Plugin
 from ..common import state, CastBoolMixin, apply_variables
+from ..adapters.units import convert_coords, convert_monitor_dimension
 
-DEFAULT_MARGIN = 60  # in pixels
 AFTER_SHOW_INHIBITION = 0.3  # 300ms of ignorance after a show
+DEFAULT_MARGIN = 60  # in pixels
+DEFAULT_HIDE_DELAY = 0.2
 DEFAULT_HYSTERESIS = 0.4  # In seconds
 
 # Helper functions {{{
 
-invert_dimension = {"width": "height", "height": "width"}
-
 
-def get_space_identifier():
+def get_active_space_identifier():
     "Returns a unique object for the workspace + monitor combination"
     return (state.active_workspace, state.active_monitor)
 
 
-def convert_coords(logger, coords, monitor):
-    """
-    Converts a string like "X Y" to coordinates relative to monitor
-    Supported formats for X, Y:
-    - Percentage: "V%". V in [0; 100]
-    - Pixels: "Vpx". V should fit in your screen and not be zero
-
-    Example:
-    "10% 20%", monitor 800x600 => 80, 120
-    """
-
-    assert coords, "coords must be non null"
-
-    def convert(size, dimension):
-        scale = float(monitor["scale"])
-        if monitor["transform"] in (1, 3):
-            dimension = invert_dimension[dimension]
-        if size[-1] == "%":
-            p = int(size[:-1])
-            if p < 0 or p > 100:
-                raise ValueError(f"Percentage must be in range [0; 100], got {p}")
-            return int(monitor[dimension] / scale * p / 100)
-        if size[-2:] == "px":
-            return int(size[:-2])
-        raise ValueError(
-            f"Unsupported format for dimension {dimension} size, got {size}"
-        )
-
-    try:
-        x_str, y_str = coords.split()
-
-        return convert(x_str, "width"), convert(y_str, "height")
-    except Exception as e:
-        logger.error(f"Failed to read coordinates: {e}")
-        raise e
+async def get_all_space_identifiers(monitors):
+    "Returns a list of every space identifiers (workspace + monitor) on active screens"
+    return [
+        (monitor["activeWorkspace"]["name"], monitor["name"]) for monitor in monitors
+    ]
 
 
 # }}}
 
 
 class Animations:  # {{{
     "Animation store"
@@ -78,56 +48,70 @@
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = int(monitor["width"] / scale)
 
         client_width = client["size"][0]
         margin_x = int((mon_width - client_width) / 2) + mon_x
 
-        return f"movewindowpixel exact {margin_x} {mon_y + margin},{client_uid}"
+        corrected_margin = convert_monitor_dimension(margin, monitor["height"], monitor)
+
+        return (
+            f"movewindowpixel exact {margin_x} {mon_y + corrected_margin},{client_uid}"
+        )
 
     @staticmethod
     def frombottom(monitor, client, client_uid, margin):
         "Slide from/to bottom"
         scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = int(monitor["width"] / scale)
         mon_height = int(monitor["height"] / scale)
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_x = int((mon_width - client_width) / 2) + mon_x
-        return f"movewindowpixel exact {margin_x} {mon_y + mon_height - client_height - margin},{client_uid}"
+
+        corrected_margin = convert_monitor_dimension(margin, monitor["height"], monitor)
+
+        return f"movewindowpixel exact {margin_x} {mon_y + mon_height - client_height - corrected_margin},{client_uid}"
 
     @staticmethod
     def fromleft(monitor, client, client_uid, margin):
         "Slide from/to left"
         scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_height = int(monitor["height"] / scale)
 
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
 
-        return f"movewindowpixel exact {margin + mon_x} {margin_y},{client_uid}"
+        corrected_margin = convert_monitor_dimension(margin, monitor["width"], monitor)
+
+        return (
+            f"movewindowpixel exact {corrected_margin + mon_x} {margin_y},{client_uid}"
+        )
 
     @staticmethod
     def fromright(monitor, client, client_uid, margin):
         "Slide from/to right"
         scale = float(monitor["scale"])
         mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = int(monitor["width"] / scale)
         mon_height = int(monitor["height"] / scale)
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
-        return f"movewindowpixel exact {mon_width - client_width - margin + mon_x } {margin_y},{client_uid}"
+
+        corrected_margin = convert_monitor_dimension(margin, monitor["width"], monitor)
+
+        return f"movewindowpixel exact {mon_width - client_width - corrected_margin + mon_x } {margin_y},{client_uid}"
 
 
 # }}}
 
 
 class OverridableConfig:
     "A `dict`-like object allowing per-monitor overrides"
@@ -174,27 +158,14 @@
         self.client_info = {}
         self.should_hide = False
         self.initialized = False
         self.meta = {}
         self.space_identifier = None
         self.monitor = ""
 
-    async def get_auto_offset(self, monitor=None):
-        "Get au automatic offset value computed from client size"
-        width, height = self.client_info["size"]
-        margin = self.conf.get("margin", DEFAULT_MARGIN)
-        if monitor is None:
-            monitor = await get_focused_monitor_props(
-                self.log, name=self.conf.get("force_monitor")
-            )
-        return map(
-            int,
-            [(width + margin) / monitor["scale"], (height + margin) / monitor["scale"]],
-        )
-
     async def initialize(self, ex):
         "Initialize the scratchpad"
         if self.initialized:
             return
         self.initialized = True
         await self.updateClientInfo()
         await ex.hyprctl(
@@ -443,17 +414,15 @@
         self.scratches.setState(scratch, "configured")
         animation_type: str = scratch.conf.get("animation", "fromTop").lower()
         defined_class: str = scratch.conf.get("class", "")
         if defined_class:
             monitor = await self.get_focused_monitor_props(
                 name=scratch.conf.get("force_monitor")
             )
-            width, height = convert_coords(
-                self.log, scratch.conf.get("size", "80% 80%"), monitor
-            )
+            width, height = convert_coords(scratch.conf.get("size", "80% 80%"), monitor)
 
             ipc_commands = [
                 f"windowrule float,^({defined_class})$",
                 f"windowrule workspace special:scratch_{scratch.uid} silent,^({defined_class})$",
             ]
 
             if not self.cast_bool(scratch.conf.get("preserve_aspect")):
@@ -718,17 +687,36 @@
         if not first_scratch:
             self.log.warning("%s doesn't exist, can't toggle.", uids[0])
             await notify_error(
                 f"Scratchpad '{uids[0]}' not found, check your configuration or the toggle parameter"
             )
             return
 
+        if self.cast_bool(first_scratch.conf.get("alt_toggle")):
+            # Needs to be on any monitor (if workspace matches)
+            extra_visibility_check = (
+                first_scratch.space_identifier
+                in await get_all_space_identifiers(await self.hyprctlJSON("monitors"))
+            )
+        else:
+            self.log.debug(
+                "visibility_check: %s == %s",
+                first_scratch.space_identifier,
+                get_active_space_identifier(),
+            )
+            # Needs to be on the active monitor+workspace
+            extra_visibility_check = (
+                first_scratch.space_identifier == get_active_space_identifier()
+            )  # visible on the currently focused monitor
+
         is_visible = first_scratch.visible and (
-            first_scratch.conf.get("force_monitor")
-            or first_scratch.space_identifier == get_space_identifier()
+            first_scratch.conf.get(
+                "force_monitor"
+            )  # always showing on the same monitor
+            or extra_visibility_check
         )
         tasks = []
 
         for uid in uids:
             item = self.scratches.get(uid)
             if not item:
                 self.log.warning("%s is not configured", uid)
@@ -739,47 +727,69 @@
                 if is_visible and await item.isAlive():
                     tasks.append(partial(self.run_hide, uid))
                 else:
                     tasks.append(partial(self.run_show, uid))
         await asyncio.gather(*(asyncio.create_task(t()) for t in tasks))
 
     async def get_offsets(self, scratch, monitor=None):
-        "Return offset from config or compute one"
+        "Return offset from config or use margin as a ref"
         offset = scratch.conf.get("offset")
+        rotated = monitor["transform"] in (1, 3)
+        aspect = (
+            reversed(scratch.client_info["size"])
+            if rotated
+            else scratch.client_info["size"]
+        )
+
+        if monitor is None:
+            monitor = await get_focused_monitor_props(
+                self.log, name=scratch.conf.get("force_monitor")
+            )
+
         if offset:
-            return offset, offset
-        return await scratch.get_auto_offset(monitor)
+            return [convert_monitor_dimension(offset, ref, monitor) for ref in aspect]
+
+        # compute from client size & margin
+        margin = scratch.conf.get("margin", DEFAULT_MARGIN)
+
+        mon_size = (
+            [monitor["height"], monitor["width"]]
+            if rotated
+            else [monitor["width"], monitor["height"]]
+        )
+
+        margins = [convert_monitor_dimension(margin, dim, monitor) for dim in mon_size]
+        return map(int, [(a + m) / monitor["scale"] for a, m in zip(aspect, margins)])
 
     async def _hide_transition(self, scratch, monitor):
         "animate hiding a scratchpad"
 
         animation_type: str = scratch.conf.get("animation", "").lower()
         if not animation_type:
             return False
 
-        await self.updateScratchInfo(scratch)
-
         off_x, off_y = await self.get_offsets(scratch, monitor)
         await self._slide_animation(animation_type, scratch, off_x, off_y)
+        await asyncio.sleep(
+            scratch.conf.get("hide_delay", DEFAULT_HIDE_DELAY)
+        )  # await for animation to finish
         return True
 
     async def _slide_animation(self, animation_type, scratch, off_x, off_y):
         "Slides the window `offset` pixels respecting `animation_type`"
         addr = "address:" + scratch.full_address
         if animation_type == "fromtop":
             await self.hyprctl(f"movewindowpixel 0 {-off_y},{addr}")
         elif animation_type == "frombottom":
             await self.hyprctl(f"movewindowpixel 0 {off_y},{addr}")
         elif animation_type == "fromleft":
             await self.hyprctl(f"movewindowpixel {-off_x} 0,{addr}")
         elif animation_type == "fromright":
             await self.hyprctl(f"movewindowpixel {off_x} 0,{addr}")
 
-        await asyncio.sleep(0.2)  # await for animation to finish
-
     async def run_show(self, uid) -> None:
         """<name> shows scratchpad "name" """
         item = self.scratches.get(uid)
 
         if not item:
             self.log.warning("%s doesn't exist, can't hide.", uid)
             await notify_error(
@@ -805,15 +815,15 @@
             assert scratch
             if scratch.visible:
                 await self.run_hide(e_uid, autohide=True)
         await item.updateClientInfo()
         await item.initialize(self)
 
         item.visible = True
-        item.space_identifier = get_space_identifier()
+        item.space_identifier = get_active_space_identifier()
         monitor = await self.get_focused_monitor_props(
             name=item.conf.get("force_monitor")
         )
 
         assert monitor
         assert item.full_address, "No address !"
 
@@ -841,29 +851,29 @@
             await self._fix_size(item, monitor)
         await item.updateClientInfo()
         position_fixed = False
         if should_set_aspect:
             position_fixed = await self._fix_position(item, monitor)
         if not position_fixed:
             if animation_type:
-                # NOTE: refactor, use single animation method
                 if preserve_aspect and was_alive and not should_set_aspect:
+                    # Relative positioning
                     if "size" not in item.client_info:
                         await self.updateScratchInfo(item)
 
                     ox, oy = await self.get_offsets(item, monitor)
                     await self._slide_animation(animation_type, item, -ox, -oy)
                 else:
-                    margin = item.conf.get("margin", DEFAULT_MARGIN)
+                    # Absolute positioning
                     fn = getattr(Animations, animation_type)
                     command = fn(
                         monitor,
                         item.client_info,
                         "address:" + item.full_address,
-                        margin,
+                        item.conf.get("margin", DEFAULT_MARGIN),
                     )
                     await self.hyprctl(command)
             else:
                 self.log.warning(
                     "No position and no animation provided for %s, don't know where to place it.",
                     item.uid,
                 )
@@ -873,30 +883,30 @@
         item.meta["monitor_info"] = monitor
 
     async def _fix_size(self, item, monitor):
         "apply the `size` config parameter"
 
         size = item.conf.get("size")
         if size:
-            width, height = convert_coords(self.log, size, monitor)
+            width, height = convert_coords(size, monitor)
             max_size = item.conf.get("max_size")
             if max_size:
-                max_width, max_height = convert_coords(self.log, max_size, monitor)
+                max_width, max_height = convert_coords(max_size, monitor)
                 width = min(max_width, width)
                 height = min(max_height, height)
             await self.hyprctl(
                 f"resizewindowpixel exact {width} {height},address:{item.full_address}"
             )
 
     async def _fix_position(self, item, monitor):
         "apply the `position` config parameter"
 
         position = item.conf.get("position")
         if position:
-            x_pos, y_pos = convert_coords(self.log, position, monitor)
+            x_pos, y_pos = convert_coords(position, monitor)
             x_pos_abs, y_pos_abs = x_pos + monitor["x"], y_pos + monitor["y"]
             await self.hyprctl(
                 f"movewindowpixel exact {x_pos_abs} {y_pos_abs},address:{item.full_address}"
             )
             return True
         return False
```

### Comparing `pyprland-2.2.3/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.4/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.4/pyprland/plugins/shortcuts_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
             return f"{prefix} {label} {suffix}".strip()
 
         while True:
             selection = name
             if isinstance(options, str):
                 self.log.info("running %s", options)
-                await self._run_command(options.strip())
+                await self._run_command(options.strip(), state.variables)
                 break
             if isinstance(options, list):
                 self.log.info("interpreting %s", options)
                 await self._handle_chain(options)
                 break
             try:
                 formatted_options = {_format_title(k, v): v for k, v in options.items()}
@@ -90,12 +90,12 @@
                 if autovalidate and len(choices) == 1:
                     variables[var_name] = choices[0]
                 else:
                     selection = await self.menu.run(choices, var_name)
                     variables[var_name] = apply_filter(selection, option.get("filter"))
                     self.log.debug("set %s = %s", var_name, variables[var_name])
 
-    async def _run_command(self, command, variables=None):
+    async def _run_command(self, command, variables):
         "Runs a shell `command`, optionally replacing `variables`"
         final_command = apply_variables(command, variables)
         self.log.info("Executing %s", final_command)
         await asyncio.create_subprocess_shell(final_command)
```

### Comparing `pyprland-2.2.3/pyprland/plugins/system_notifier.py` & `pyprland-2.2.4/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.4/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/toggle_special.py` & `pyprland-2.2.4/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyprland/plugins/wallpapers.py` & `pyprland-2.2.4/pyprland/plugins/wallpapers.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,16 +70,20 @@
         cmd_prefix = self.config.get("command", "swaybg -m fill -i")
         while self.running:
             self.next_background_event.clear()
             filename = self.select_next_image().replace('"', '\\"')
             cmd = f'{cmd_prefix} "{filename}"'
             self.log.info("Running %s", cmd)
             self.proc = await asyncio.create_subprocess_shell(cmd)
+            await asyncio.sleep(1)  # wait for the command to start
+            # check if the command failed
+            if self.proc.returncode:
+                await self.notify_error(f"wallpaper command failed: {cmd}")
 
-            interval = asyncio.sleep(60 * self.config.get("interval", 10))
+            interval = asyncio.sleep(60 * self.config.get("interval", 10) - 1)
             await asyncio.wait(
                 [
                     asyncio.create_task(interval),
                     asyncio.create_task(self.next_background_event.wait()),
                 ],
                 return_when=asyncio.FIRST_COMPLETED,
             )
```

### Comparing `pyprland-2.2.3/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.4/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.3/pyproject.toml` & `pyprland-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.3"
+version = "2.2.4"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.3/PKG-INFO` & `pyprland-2.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.3
+Version: 2.2.4
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,39 +15,50 @@
 Description-Content-Type: text/markdown
 
 ![rect](https://github.com/hyprland-community/pyprland/assets/238622/3fab93b6-6445-4e7b-b757-035095b5c8e8)
 
 [![Hyprland](https://img.shields.io/badge/Made%20for-Hyprland-blue)](https://github.com/hyprwm/Hyprland)
 [![Discord](https://img.shields.io/discord/1055990214411169892?label=discord)](https://discord.gg/zzWqvcKRMy)
 
+[Documentation](https://github.com/hyprland-community/pyprland/wiki) • [Discussions](https://github.com/hyprland-community/pyprland/discussions) • [Changes History](https://github.com/hyprland-community/pyprland/releases) • [Share Your Setup](https://github.com/hyprland-community/pyprland/discussions/46)
+
+
 ## Enhance your Hyprland experience with Pyprland
 
 Welcome to Pyprland, your gateway to extending the capabilities of [Hyprland](https://hyprland.org/). Pyprland offers a plethora of plugins designed for simplicity and efficiency, allowing you to supercharge your productivity and customize your user experience.
 
 - Explore our variety of [plugins](https://github.com/hyprland-community/pyprland/wiki/Plugins) to tailor your Hyprland setup to your liking.
 - New users, check the [getting started](https://github.com/hyprland-community/pyprland/wiki/Getting-started) guide.
 
 
-[Documentation](https://github.com/hyprland-community/pyprland/wiki) • [Discussions](https://github.com/hyprland-community/pyprland/discussions) • [Changes History](https://github.com/hyprland-community/pyprland/releases) • [Share Your Setup](https://github.com/hyprland-community/pyprland/discussions/46)
-
-
 ## About Pyprland
 
 [![Packaging Status](https://repology.org/badge/vertical-allrepos/pyprland.svg)](https://repology.org/project/pyprland/versions)
 
 🎉 Hear what others are saying:
 - ["It just works very very well" - The Linux Cast (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February 2024
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
 
+## Contributing
+
+Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
+
+- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
+- Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
+
+and if you have coding skills you can also
+
+- Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
+- Write new plugins
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
-- **aiofiles** (Python package)
+    - **aiofiles**
 
 ## Latest major changes
 
 > [!note]
 > Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 ### 2.2
@@ -73,23 +84,14 @@
 - Introduced [shortcuts_menu](https://github.com/hyprland-community/pyprland/wiki/shortcuts_menu) plugin.
 
 ### 1.8
 
 - Requires Hyprland >= 0.30
 - Added [layout_center](https://github.com/hyprland-community/pyprland/wiki/layout_center) plugin.
 
-## Developers
-
-Contribute to Pyprland in various ways:
-- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
-- Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki) or write new plugins.
-- Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
-
-Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
-
 ## Star History
 
 <a href="https://star-history.com/#fdev31/pyprland&Date">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline&theme=dark" />
     <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
```

