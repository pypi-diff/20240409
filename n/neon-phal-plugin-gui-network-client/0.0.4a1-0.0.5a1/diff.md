# Comparing `tmp/neon-phal-plugin-gui-network-client-0.0.4a1.tar.gz` & `tmp/neon-phal-plugin-gui-network-client-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-gui-network-client-0.0.4a1.tar", last modified: Thu Jan 11 20:19:31 2024, max compression
+gzip compressed data, was "neon-phal-plugin-gui-network-client-0.0.5a1.tar", last modified: Mon Apr  8 23:15:12 2024, max compression
```

## Comparing `neon-phal-plugin-gui-network-client-0.0.4a1.tar` & `neon-phal-plugin-gui-network-client-0.0.5a1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.843210 neon-phal-plugin-gui-network-client-0.0.4a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-01-11 20:19:31.839210 neon-phal-plugin-gui-network-client-0.0.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.831210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.831210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.835210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_created.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_stop.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_stopped.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_connecting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_end_setup.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_http_started.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_start_setup.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_user_connected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_wifi_connected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_wifi_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_wifi_scanned.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/launch_setup.intent
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/wifi_intro.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.835210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_created.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_stop.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_stopped.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_connecting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_end_setup.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_http_started.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_start_setup.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_user_connected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_wifi_connected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_wifi_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_wifi_scanned.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/launch_setup.intent
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/wifi_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/wifi_intro_2.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/en-us/wifi_intro_3.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.839210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/BottomActionButton.qml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/GuiClientLoader.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ManageConnectedNetwork.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ManageUnconnectedNetwork.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ModeChoose.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/NetworkingLoader.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/Status.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ViewPod.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.839210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/check-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/info-circle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/ondisplay.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/onmobile.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/times-circle.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.839210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/Connecting.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItem.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemParent.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemSetting.qml
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/SelectNetwork.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.839210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/
--rw-r--r--   0 runner    (1001) docker     (127)    34867 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/connecting.json
--rw-r--r--   0 runner    (1001) docker     (127)   139588 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/fail.json
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/security.json
--rw-r--r--   0 runner    (1001) docker     (127)   145637 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/success.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.839210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/sounds/ui_sounds_clicked.wav
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:19:31.831210 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:19:31.000000 neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 20:19:31.843210 neon-phal-plugin-gui-network-client-0.0.4a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3068 2024-01-11 20:19:28.000000 neon-phal-plugin-gui-network-client-0.0.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.763109 neon-phal-plugin-gui-network-client-0.0.5a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-08 23:15:12.763109 neon-phal-plugin-gui-network-client-0.0.5a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.755109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.751109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.755109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_created.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_stop.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_ap_stopped.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_connecting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_end_setup.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_http_started.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_start_setup.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_user_connected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_wifi_connected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_wifi_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/debug_wifi_scanned.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/launch_setup.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/wifi_intro.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.759109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_created.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_stop.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_ap_stopped.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_connecting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_end_setup.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_http_started.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_start_setup.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_user_connected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_wifi_connected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_wifi_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/debug_wifi_scanned.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/launch_setup.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/wifi_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/wifi_intro_2.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/en-us/wifi_intro_3.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.759109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/BottomActionButton.qml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/GuiClientLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ManageConnectedNetwork.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ManageUnconnectedNetwork.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ModeChoose.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/NetworkingLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/Status.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ViewPod.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.759109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/check-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/info-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/ondisplay.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/onmobile.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/times-circle.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.759109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/Connecting.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItem.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemParent.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemSetting.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/SelectNetwork.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.763109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)    34867 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/connecting.json
+-rw-r--r--   0 runner    (1001) docker     (127)   139588 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/fail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/security.json
+-rw-r--r--   0 runner    (1001) docker     (127)   145637 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/success.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.763109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/sounds/ui_sounds_clicked.wav
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:15:12.755109 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:15:12.000000 neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:15:12.763109 neon-phal-plugin-gui-network-client-0.0.5a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3068 2024-04-08 23:15:03.000000 neon-phal-plugin-gui-network-client-0.0.5a1/setup.py
```

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/LICENSE` & `neon-phal-plugin-gui-network-client-0.0.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/PKG-INFO` & `neon-phal-plugin-gui-network-client-0.0.5a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-gui-network-client
-Version: 0.0.4a1
+Version: 0.0.5a1
 Summary: A PHAL plugin for Neon/OVOS
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-gui-network-client
 Author: Neongecko
 Author-email: defelopers@neon.ai
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/README.md` & `neon-phal-plugin-gui-network-client-0.0.5a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/__init__.py` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/locale/ca-es/launch_setup.intent` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/locale/ca-es/launch_setup.intent`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/BottomActionButton.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/BottomActionButton.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ManageConnectedNetwork.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ManageConnectedNetwork.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ManageUnconnectedNetwork.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ManageUnconnectedNetwork.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ModeChoose.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ModeChoose.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/NetworkingLoader.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/NetworkingLoader.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/Status.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/ViewPod.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/ViewPod.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/check-circle.svg` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/check-circle.svg`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/info-circle.svg` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/info-circle.svg`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/ondisplay.svg` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/ondisplay.svg`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/onmobile.svg` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/onmobile.svg`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/icons/times-circle.svg` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/icons/times-circle.svg`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/Connecting.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/Connecting.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItem.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItem.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemParent.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemParent.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemSetting.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/NetworkItemSetting.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/SelectNetwork.qml` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/SelectNetwork.qml`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/connecting.json` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/connecting.json`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/fail.json` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/fail.json`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/security.json` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/security.json`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/networking/animations/success.json` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/networking/animations/success.json`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client/ui/sounds/ui_sounds_clicked.wav` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client/ui/sounds/ui_sounds_clicked.wav`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/PKG-INFO` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-gui-network-client
-Version: 0.0.4a1
+Version: 0.0.5a1
 Summary: A PHAL plugin for Neon/OVOS
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-gui-network-client
 Author: Neongecko
 Author-email: defelopers@neon.ai
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/neon_phal_plugin_gui_network_client.egg-info/SOURCES.txt` & `neon-phal-plugin-gui-network-client-0.0.5a1/neon_phal_plugin_gui_network_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-gui-network-client-0.0.4a1/setup.py` & `neon-phal-plugin-gui-network-client-0.0.5a1/setup.py`

 * *Files identical despite different names*

