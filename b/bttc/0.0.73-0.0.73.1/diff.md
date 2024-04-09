# Comparing `tmp/bttc-0.0.73.tar.gz` & `tmp/bttc-0.0.73.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.73.tar", last modified: Sun Apr  7 14:59:20 2024, max compression
+gzip compressed data, was "bttc-0.0.73.1.tar", last modified: Tue Apr  9 04:37:46 2024, max compression
```

## Comparing `bttc-0.0.73.tar` & `bttc-0.0.73.1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.718942 bttc-0.0.73/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2075 2024-04-07 14:59:20.718942 bttc-0.0.73/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-07 14:57:22.000000 bttc-0.0.73/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5003 2024-04-07 14:56:58.000000 bttc-0.0.73/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-07 14:56:03.000000 bttc-0.0.73/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-07 14:56:03.000000 bttc-0.0.73/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22466 2024-04-07 14:56:03.000000 bttc-0.0.73/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.710942 bttc-0.0.73/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.718942 bttc-0.0.73/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.718942 bttc-0.0.73/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2868 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2075 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1266 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      164 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-07 14:59:20.718942 bttc-0.0.73/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1682 2024-03-30 03:00:32.000000 bttc-0.0.73/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.354849 bttc-0.0.73.1/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.1/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-09 04:37:46.354849 bttc-0.0.73.1/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.1/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5005 2024-04-09 04:28:05.000000 bttc-0.0.73.1/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.1/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22466 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.346849 bttc-0.0.73.1/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.354849 bttc-0.0.73.1/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.354849 bttc-0.0.73.1/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.1/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.1/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-09 04:37:46.350849 bttc-0.0.73.1/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      164 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-09 04:37:46.000000 bttc-0.0.73.1/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-09 04:37:46.354849 bttc-0.0.73.1/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1682 2024-04-09 04:37:34.000000 bttc-0.0.73.1/setup.py
```

### Comparing `bttc-0.0.73/LICENSE` & `bttc-0.0.73.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/PKG-INFO` & `bttc-0.0.73.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73
+Version: 0.0.73.1
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73/README.md` & `bttc-0.0.73.1/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/__init__.py` & `bttc-0.0.73.1/bttc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.73'
+__version__ = '0.0.73.1'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.73/bttc/ble_data.py` & `bttc-0.0.73.1/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/ble_utils.py` & `bttc-0.0.73.1/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/bt_data.py` & `bttc-0.0.73.1/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/bt_utils.py` & `bttc-0.0.73.1/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/cli/__init__.py` & `bttc-0.0.73.1/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/cli/constants.py` & `bttc-0.0.73.1/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/cli/main.py` & `bttc-0.0.73.1/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/common_data.py` & `bttc-0.0.73.1/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/constants.py` & `bttc-0.0.73.1/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/core.py` & `bttc-0.0.73.1/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/errors.py` & `bttc-0.0.73.1/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/general_utils.py` & `bttc-0.0.73.1/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.73.1/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.73.1/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.73.1/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.73.1/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.73.1/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/avrcp/errors.py` & `bttc-0.0.73.1/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/__init__.py` & `bttc-0.0.73.1/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/constants.py` & `bttc-0.0.73.1/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/errors.py` & `bttc-0.0.73.1/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.73.1/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.73.1/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.73.1/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.73.1/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/strategy.py` & `bttc-0.0.73.1/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/ad_checker.py` & `bttc-0.0.73.1/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/device_factory.py` & `bttc-0.0.73.1/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/iperf/__init__.py` & `bttc-0.0.73.1/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/iperf/errors.py` & `bttc-0.0.73.1/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/key_events_handler.py` & `bttc-0.0.73.1/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/log_parser.py` & `bttc-0.0.73.1/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/logcat.py` & `bttc-0.0.73.1/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/retry.py` & `bttc-0.0.73.1/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils/typing_utils.py` & `bttc-0.0.73.1/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc/utils_loader.py` & `bttc-0.0.73.1/bttc/utils_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility to load functional modules of device."""
 from bttc import core
+from bttc import apk_utils        # noqa: F401
 from bttc import ble_utils        # noqa: F401
 from bttc import general_utils    # noqa: F401
 from bttc import bt_utils         # noqa: F401
 from bttc import wifi_utils       # noqa: F401
 import dataclasses
 import deprecation
 import importlib
```

### Comparing `bttc-0.0.73/bttc/wifi_utils.py` & `bttc-0.0.73.1/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73/bttc.egg-info/PKG-INFO` & `bttc-0.0.73.1/bttc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73
+Version: 0.0.73.1
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.73/bttc.egg-info/SOURCES.txt` & `bttc-0.0.73.1/bttc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 bttc/__init__.py
+bttc/apk_utils.py
 bttc/ble_data.py
 bttc/ble_utils.py
 bttc/bt_data.py
 bttc/bt_utils.py
 bttc/common_data.py
 bttc/constants.py
 bttc/core.py
```

### Comparing `bttc-0.0.73/setup.py` & `bttc-0.0.73.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         'bttc', 'bttc.cli', 'bttc.utils', 'bttc.profiles.hfp', 'bttc.profiles.avrcp',
         'bttc.utils.iperf', 'bttc.mobly_android_device_lib',
         'bttc.mobly_android_device_lib.services'],
     install_requires=[
         'cmd2==2.4.3',
         'deprecation==2.1.0',
         'mobly>=1.12.2',
-        'portpicker==1.5.2',
-        'psutil==5.9.5',
+        'portpicker==1.6.0',
+        'psutil==5.9.8',
         'PyYAML==6.0.1',
         'numpy',
         'six==1.16.0',
         'pure-python-adb==0.3.0.dev0',
         'snippet-uiautomator>=1.1.0',
     ],
     classifiers=[
```

