# Comparing `tmp/hahomematic-2024.4.3.tar.gz` & `tmp/hahomematic-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.3.tar", last modified: Tue Apr  9 08:47:56 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.4.tar", last modified: Tue Apr  9 13:56:59 2024, max compression
```

## Comparing `hahomematic-2024.4.3.tar` & `hahomematic-2024.4.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.117594 hahomematic-2024.4.3/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    58601 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.125594 hahomematic-2024.4.3/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.125594 hahomematic-2024.4.3/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.129594 hahomematic-2024.4.3/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.129594 hahomematic-2024.4.3/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:47:55.000000 hahomematic-2024.4.3/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.129594 hahomematic-2024.4.3/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.614380 hahomematic-2024.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 13:56:59.614380 hahomematic-2024.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.598379 hahomematic-2024.4.4/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.602380 hahomematic-2024.4.4/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.602380 hahomematic-2024.4.4/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    58601 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.602380 hahomematic-2024.4.4/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.602380 hahomematic-2024.4.4/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.606380 hahomematic-2024.4.4/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28648 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.606380 hahomematic-2024.4.4/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.610380 hahomematic-2024.4.4/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.610380 hahomematic-2024.4.4/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.614380 hahomematic-2024.4.4/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 13:56:59.000000 hahomematic-2024.4.4/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-09 13:56:59.000000 hahomematic-2024.4.4/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:56:59.000000 hahomematic-2024.4.4/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:56:59.000000 hahomematic-2024.4.4/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 13:56:59.000000 hahomematic-2024.4.4/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 13:56:59.000000 hahomematic-2024.4.4/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.610380 hahomematic-2024.4.4/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 13:56:59.614380 hahomematic-2024.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:56:59.614380 hahomematic-2024.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-09 13:56:31.000000 hahomematic-2024.4.4/tests/test_text.py
```

### Comparing `hahomematic-2024.4.3/LICENSE` & `hahomematic-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/PKG-INFO` & `hahomematic-2024.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.3/README.md` & `hahomematic-2024.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/__init__.py` & `hahomematic-2024.4.4/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.4/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/caches/persistent.py` & `hahomematic-2024.4.4/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/caches/visibility.py` & `hahomematic-2024.4.4/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/central/__init__.py` & `hahomematic-2024.4.4/hahomematic/central/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/central/decorators.py` & `hahomematic-2024.4.4/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.4/hahomematic/central/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/client/__init__.py` & `hahomematic-2024.4.4/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.4/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.4/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/config.py` & `hahomematic-2024.4.4/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/const.py` & `hahomematic-2024.4.4/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/exceptions.py` & `hahomematic-2024.4.4/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/hmcli.py` & `hahomematic-2024.4.4/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/performance.py` & `hahomematic-2024.4.4/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.4/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,17 @@
         self._data_entities[field] = entity
 
     def unregister_entity_updated_callback(
         self, entity_updated_callback: Callable, custom_id: str
     ) -> None:
         """Unregister update callback."""
         for entity in self._data_entities.values():
-            entity.unregister_internal_update_callback(update_callback=entity_updated_callback)
+            entity.unregister_internal_entity_updated_callback(
+                update_callback=entity_updated_callback
+            )
 
         super().unregister_entity_updated_callback(
             entity_updated_callback=entity_updated_callback, custom_id=custom_id
         )
 
     def _mark_entities(self, entity_def: Mapping[int | tuple[int, ...], tuple[str, ...]]) -> None:
         """Mark entities to be created in HA."""
```

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.4/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.4/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/device.py` & `hahomematic-2024.4.4/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/entity.py` & `hahomematic-2024.4.4/hahomematic/platforms/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,14 @@
     _platform: HmPlatform
 
     def __init__(self, central: hmcu.CentralUnit, unique_id: str) -> None:
         """Init the callback entity."""
         self._central: Final = central
         self._unique_id: Final = unique_id
         self._entity_updated_callbacks: dict[Callable, str] = {}
-        self._entity_refreshed_callbacks: dict[Callable, str] = {}
         self._entity_removed_callbacks: list[Callable] = []
         self._custom_id: str | None = None
 
     @property
     @abstractmethod
     def available(self) -> bool:
         """Return the availability of the device."""
@@ -182,85 +181,53 @@
     ) -> None:
         """Register entity updated callback."""
         if callable(entity_updated_callback):
             self._entity_updated_callbacks[entity_updated_callback] = custom_id
         if custom_id != DEFAULT_CUSTOM_ID:
             if self._custom_id is not None and self._custom_id != custom_id:
                 raise HaHomematicException(
-                    f"REGISTER_ENTITY_UPDATED_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
+                    f"REGISTER_entity_updated_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
 
-    def unregister_internal_update_callback(self, update_callback: Callable) -> None:
+    def unregister_internal_entity_updated_callback(self, update_callback: Callable) -> None:
         """Unregister entity updated callback."""
         self.unregister_entity_updated_callback(
             entity_updated_callback=update_callback, custom_id=DEFAULT_CUSTOM_ID
         )
 
     def unregister_entity_updated_callback(
         self, entity_updated_callback: Callable, custom_id: str
     ) -> None:
         """Unregister entity updated callback."""
         if entity_updated_callback in self._entity_updated_callbacks:
             del self._entity_updated_callbacks[entity_updated_callback]
         if self.custom_id == custom_id:
             self._custom_id = None
 
-    def register_entity_refreshed_callback(
-        self, entity_refreshed_callback: Callable, custom_id: str
-    ) -> None:
-        """Register entity updated callback."""
-        if callable(entity_refreshed_callback):
-            self._entity_refreshed_callbacks[entity_refreshed_callback] = custom_id
-        if custom_id != DEFAULT_CUSTOM_ID:
-            if self._custom_id is not None and self._custom_id != custom_id:
-                raise HaHomematicException(
-                    f"REGISTER_ENTITY_REFRESHED_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
-                )
-            self._custom_id = custom_id
-
-    def unregister_entity_refreshed_callback(
-        self, entity_refreshed_callback: Callable, custom_id: str
-    ) -> None:
-        """Unregister entity updated callback."""
-        if entity_refreshed_callback in self._entity_refreshed_callbacks:
-            del self._entity_refreshed_callbacks[entity_refreshed_callback]
-        if self.custom_id == custom_id:
-            self._custom_id = None
-
     def register_entity_removed_callback(self, entity_removed_callback: Callable) -> None:
         """Register the entity removed callback."""
         if (
             callable(entity_removed_callback)
             and entity_removed_callback not in self._entity_removed_callbacks
         ):
             self._entity_removed_callbacks.append(entity_removed_callback)
 
     def unregister_entity_removed_callback(self, entity_removed_callback: Callable) -> None:
         """Unregister the entity removed callback."""
         if entity_removed_callback in self._entity_removed_callbacks:
             self._entity_removed_callbacks.remove(entity_removed_callback)
 
     def fire_entity_updated_callback(self, *args: Any, **kwargs: Any) -> None:
-        """Do what is needed when the value of the entity has been updated."""
+        """Do what is needed when the value of the entity has been updated/refreshed."""
         for _callback in self._entity_updated_callbacks:
             try:
                 _callback(*args, **kwargs)
             except Exception as ex:
-                _LOGGER.warning("FIRE_ENTITY_UPDATED_EVENT failed: %s", reduce_args(args=ex.args))
-
-    def fire_entity_refreshed_callback(self, *args: Any, **kwargs: Any) -> None:
-        """Do what is needed when the value of the entity has been refreshed."""
-        for _callback in self._entity_refreshed_callbacks:
-            try:
-                _callback(*args, **kwargs)
-            except Exception as ex:
-                _LOGGER.warning(
-                    "FIRE_ENTITY_REFRESHED_EVENT failed: %s", reduce_args(args=ex.args)
-                )
+                _LOGGER.warning("FIRE_entity_updated_EVENT failed: %s", reduce_args(args=ex.args))
 
     def fire_entity_removed_callback(self, *args: Any) -> None:
         """Do what is needed when the entity has been removed."""
         for _callback in self._entity_removed_callbacks:
             try:
                 _callback(*args)
             except Exception as ex:
@@ -696,15 +663,15 @@
                 self._state_uncertain = True
                 self.fire_entity_updated_callback()
             return (old_value, None)
 
         new_value = self._convert_value(value)
         if old_value == new_value:
             self._set_last_refreshed()
-            self.fire_entity_refreshed_callback()
+            self.fire_entity_updated_callback(is_refresh=True)
             return (old_value, new_value)
 
         self._old_value = old_value
         self._value = new_value
         self._state_uncertain = False
         self._set_last_updated()
         self.fire_entity_updated_callback()
```

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/event.py` & `hahomematic-2024.4.4/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.4/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.4/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/support.py` & `hahomematic-2024.4.4/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/platforms/update.py` & `hahomematic-2024.4.4/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.4/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.4/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic/support.py` & `hahomematic-2024.4.4/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.4/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.3/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.4/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/hahomematic_support/client_local.py` & `hahomematic-2024.4.4/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/pyproject.toml` & `hahomematic-2024.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.3"
+version     = "2024.4.4"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.4.3/tests/test_action.py` & `hahomematic-2024.4.4/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_binary_sensor.py` & `hahomematic-2024.4.4/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_button.py` & `hahomematic-2024.4.4/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_central.py` & `hahomematic-2024.4.4/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_central_pydevccu.py` & `hahomematic-2024.4.4/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_climate.py` & `hahomematic-2024.4.4/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_cover.py` & `hahomematic-2024.4.4/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_decorator.py` & `hahomematic-2024.4.4/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_device.py` & `hahomematic-2024.4.4/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_entity.py` & `hahomematic-2024.4.4/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_event.py` & `hahomematic-2024.4.4/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_json_rpc.py` & `hahomematic-2024.4.4/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_light.py` & `hahomematic-2024.4.4/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_lock.py` & `hahomematic-2024.4.4/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_number.py` & `hahomematic-2024.4.4/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_select.py` & `hahomematic-2024.4.4/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_sensor.py` & `hahomematic-2024.4.4/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_siren.py` & `hahomematic-2024.4.4/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_support.py` & `hahomematic-2024.4.4/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_switch.py` & `hahomematic-2024.4.4/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.3/tests/test_text.py` & `hahomematic-2024.4.4/tests/test_text.py`

 * *Files identical despite different names*

