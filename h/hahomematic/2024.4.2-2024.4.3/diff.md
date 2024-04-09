# Comparing `tmp/hahomematic-2024.4.2.tar.gz` & `tmp/hahomematic-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.4.2.tar", last modified: Mon Apr  8 11:38:21 2024, max compression
+gzip compressed data, was "hahomematic-2024.4.3.tar", last modified: Tue Apr  9 08:47:56 2024, max compression
```

## Comparing `hahomematic-2024.4.2.tar` & `hahomematic-2024.4.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    57005 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.966612 hahomematic-2024.4.2/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.970613 hahomematic-2024.4.2/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.970613 hahomematic-2024.4.2/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 11:38:21.000000 hahomematic-2024.4.2/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.974613 hahomematic-2024.4.2/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:21.978613 hahomematic-2024.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    26290 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26187 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    31933 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-08 11:38:00.000000 hahomematic-2024.4.2/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.117594 hahomematic-2024.4.3/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27513 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    58601 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.121594 hahomematic-2024.4.3/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.125594 hahomematic-2024.4.3/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30029 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44592 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.125594 hahomematic-2024.4.3/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.129594 hahomematic-2024.4.3/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.129594 hahomematic-2024.4.3/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:47:55.000000 hahomematic-2024.4.3/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 08:47:56.000000 hahomematic-2024.4.3/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.129594 hahomematic-2024.4.3/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:47:56.133594 hahomematic-2024.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26701 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31975 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-09 08:47:32.000000 hahomematic-2024.4.3/tests/test_text.py
```

### Comparing `hahomematic-2024.4.2/LICENSE` & `hahomematic-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/PKG-INFO` & `hahomematic-2024.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.2/README.md` & `hahomematic-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/__init__.py` & `hahomematic-2024.4.3/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/caches/dynamic.py` & `hahomematic-2024.4.3/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/caches/persistent.py` & `hahomematic-2024.4.3/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/caches/visibility.py` & `hahomematic-2024.4.3/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/central/__init__.py` & `hahomematic-2024.4.3/hahomematic/central/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 This is the python representation of a CCU.
 """
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable, Coroutine, Mapping, Set as AbstractSet
+from collections.abc import Callable, Collection, Coroutine, Mapping, Set as AbstractSet
 from concurrent.futures._base import CancelledError
 from datetime import datetime
 import logging
 import socket
 import threading
+from time import monotonic, sleep
 from typing import Any, Final, TypeVar, cast
 
 from aiohttp import ClientSession
 import orjson
 import voluptuous as vol
 
 from hahomematic import client as hmcl, config
@@ -24,14 +25,15 @@
 from hahomematic.caches.persistent import DeviceDescriptionCache, ParamsetDescriptionCache
 from hahomematic.caches.visibility import ParameterVisibilityCache
 from hahomematic.central import xml_rpc_server as xmlrpc
 from hahomematic.central.decorators import callback_event, callback_system_event
 from hahomematic.client.json_rpc import JsonRpcAioHttpClient
 from hahomematic.client.xml_rpc import XmlRpcProxy
 from hahomematic.const import (
+    BLOCK_LOG_TIMEOUT,
     DATETIME_FORMAT_MILLIS,
     DEFAULT_TLS,
     DEFAULT_VERIFY_TLS,
     ENTITY_EVENTS,
     EVENT_AVAILABLE,
     EVENT_DATA,
     EVENT_INTERFACE_ID,
@@ -61,15 +63,15 @@
 from hahomematic.platforms.device import HmDevice
 from hahomematic.platforms.entity import BaseEntity, CallbackEntity
 from hahomematic.platforms.event import GenericEvent
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.hub import Hub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
-from hahomematic.support import check_config, get_device_address, reduce_args
+from hahomematic.support import cancelling, check_config, get_device_address, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _R = TypeVar("_R")
 _T = TypeVar("_T")
 
 # {instance_name, central}
@@ -326,14 +328,17 @@
                 "There is still another central instance registered"
             )
 
         _LOGGER.debug("STOP: Removing instance")
         if self._name in CENTRAL_INSTANCES:
             del CENTRAL_INSTANCES[self._name]
 
+        # wait until tasks are finished
+        await self.block_till_done()
+
         while self._has_active_threads:
             await asyncio.sleep(1)
         self._started = False
 
     async def restart_clients(self) -> None:
         """Restart clients."""
         await self._stop_clients()
@@ -810,15 +815,17 @@
             await self.device_descriptions.save()
             await self.paramset_descriptions.save()
             await self.device_details.load()
             await self.data_cache.load()
             await self._create_devices()
 
     @callback_event
-    def event(self, interface_id: str, channel_address: str, parameter: str, value: Any) -> None:
+    async def event(
+        self, interface_id: str, channel_address: str, parameter: str, value: Any
+    ) -> None:
         """If a device emits some sort event, we will handle it here."""
         _LOGGER.debug(
             "EVENT: interface_id = %s, channel_address = %s, parameter = %s, value = %s",
             interface_id,
             channel_address,
             parameter,
             str(value),
@@ -902,14 +909,51 @@
         if (
             isinstance(entity, (GenericEntity, GenericEvent))
             and entity.supports_events
             and (entity.channel_address, entity.parameter) in self._entity_event_subscriptions
         ):
             del self._entity_event_subscriptions[(entity.channel_address, entity.parameter)]
 
+    async def block_till_done(self) -> None:
+        """Code from HA. Block until all pending work is done."""
+        # To flush out any call_soon_threadsafe
+        await asyncio.sleep(0)
+        start_time: float | None = None
+        current_task = asyncio.current_task()
+        while tasks := [
+            task for task in self._tasks if task is not current_task and not cancelling(task)
+        ]:
+            await self._await_and_log_pending(tasks)
+
+            if start_time is None:
+                # Avoid calling monotonic() until we know
+                # we may need to start logging blocked tasks.
+                start_time = 0
+            elif start_time == 0:
+                # If we have waited twice then we set the start
+                # time
+                start_time = monotonic()
+            elif monotonic() - start_time > BLOCK_LOG_TIMEOUT:
+                # We have waited at least three loops and new tasks
+                # continue to block. At this point we start
+                # logging all waiting tasks.
+                for task in tasks:
+                    _LOGGER.debug("Waiting for task: %s", task)
+
+    async def _await_and_log_pending(self, pending: Collection[asyncio.Future[Any]]) -> None:
+        """Code from HA. Await and log tasks that take a long time."""
+        wait_time = 0
+        while pending:
+            _, pending = await asyncio.wait(pending, timeout=BLOCK_LOG_TIMEOUT)
+            if not pending:
+                return
+            wait_time += BLOCK_LOG_TIMEOUT
+            for task in pending:
+                _LOGGER.debug("Waited %s seconds for task: %s", wait_time, task)
+
     def create_task(self, target: Coroutine[Any, Any, Any], name: str) -> None:
         """Add task to the executor pool."""
         try:
             self._loop.call_soon_threadsafe(self._async_create_task, target, name)
         except CancelledError:
             _LOGGER.debug(
                 "create_task: task cancelled for %s",
@@ -1163,67 +1207,63 @@
 
     def run(self) -> None:
         """Run the ConnectionChecker thread."""
         _LOGGER.debug(
             "run: Init connection checker to server %s",
             self._central.name,
         )
-
-        self._central.run_coroutine(self._check_connection())
+        while self._active:
+            self._central.run_coroutine(self._check_connection())
+            if self._active:
+                sleep(config.CONNECTION_CHECKER_INTERVAL)
 
     def stop(self) -> None:
         """To stop the ConnectionChecker."""
         self._active = False
 
     async def _check_connection(self) -> None:
         """Periodically check connection to backend."""
-        while self._active:
-            _LOGGER.debug(
-                "check_connection: Checking connection to server %s",
-                self._central.name,
-            )
-            try:
-                if not self._central.has_clients:
-                    _LOGGER.warning(
-                        "CHECK_CONNECTION failed: No clients exist. "
-                        "Trying to create clients for server %s",
-                        self._central.name,
-                    )
-                    await self._central.restart_clients()
-                else:
-                    reconnects: list[Any] = []
-                    for interface_id in self._central.interface_ids:
-                        # check:
-                        #  - client is available
-                        #  - client is connected
-                        #  - interface callback is alive
-                        client = self._central.get_client(interface_id=interface_id)
-                        if (
-                            client.available is False
-                            or not await client.is_connected()
-                            or not client.is_callback_alive()
-                        ):
-                            reconnects.append(client.reconnect())
-                    if reconnects:
-                        await asyncio.gather(*reconnects)
-                        if self._central.available:
-                            await self._central.load_and_refresh_entity_data()
-            except NoConnection as nex:
-                _LOGGER.error(
-                    "CHECK_CONNECTION failed: no connection: %s", reduce_args(args=nex.args)
-                )
-                continue
-            except Exception as err:
-                _LOGGER.error(
-                    "CHECK_CONNECTION failed: %s [%s]",
-                    type(err).__name__,
-                    reduce_args(args=err.args),
+        _LOGGER.debug(
+            "check_connection: Checking connection to server %s",
+            self._central.name,
+        )
+        try:
+            if not self._central.has_clients:
+                _LOGGER.warning(
+                    "CHECK_CONNECTION failed: No clients exist. "
+                    "Trying to create clients for server %s",
+                    self._central.name,
                 )
-            if self._active:
-                await asyncio.sleep(config.CONNECTION_CHECKER_INTERVAL)
+                await self._central.restart_clients()
+            else:
+                reconnects: list[Any] = []
+                for interface_id in self._central.interface_ids:
+                    # check:
+                    #  - client is available
+                    #  - client is connected
+                    #  - interface callback is alive
+                    client = self._central.get_client(interface_id=interface_id)
+                    if (
+                        client.available is False
+                        or not await client.is_connected()
+                        or not client.is_callback_alive()
+                    ):
+                        reconnects.append(client.reconnect())
+                if reconnects:
+                    await asyncio.gather(*reconnects)
+                    if self._central.available:
+                        await self._central.load_and_refresh_entity_data()
+        except NoConnection as nex:
+            _LOGGER.error("CHECK_CONNECTION failed: no connection: %s", reduce_args(args=nex.args))
+        except Exception as err:
+            _LOGGER.error(
+                "CHECK_CONNECTION failed: %s [%s]",
+                type(err).__name__,
+                reduce_args(args=err.args),
+            )
 
 
 class CentralConfig:
     """Config for a Client."""
 
     def __init__(
         self,
```

### Comparing `hahomematic-2024.4.2/hahomematic/central/decorators.py` & `hahomematic-2024.4.3/hahomematic/central/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,21 +66,23 @@
         if asyncio.iscoroutinefunction(func):
             return async_wrapper_callback_system_event
         return wrapper_callback_system_event
 
     return decorator_callback_system_event
 
 
-def callback_event(func: Callable[_P, _R]) -> Callable[_P, _R]:
+def callback_event(
+    func: Callable[_P, _R],
+) -> Callable:
     """Check if callback_event is set and call it AFTER original function."""
 
     @wraps(func)
-    def wrapper_callback_event(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+    async def async_wrapper_callback_event(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         """Wrap callback events."""
-        return_value = func(*args, **kwargs)
+        return_value = cast(_R, await func(*args, **kwargs))  # type: ignore[misc]
         _exec_callback_entity_event(*args, **kwargs)
         return return_value
 
     def _exec_callback_entity_event(*args: Any, **kwargs: Any) -> None:
         """Execute the callback for an entity event."""
         try:
             args = args[1:]
@@ -92,8 +94,8 @@
             _LOGGER.warning(
                 "EXEC_CALLBACK_ENTITY_EVENT failed: Unable to reduce kwargs for callback_event"
             )
             raise HaHomematicException(
                 f"args-exception callback_event [{reduce_args(args=err.args)}]"
             ) from err
 
-    return wrapper_callback_event
+    return async_wrapper_callback_event
```

### Comparing `hahomematic-2024.4.2/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.4.3/hahomematic/central/xml_rpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,22 @@
     def __init__(self, xml_rpc_server: XmlRpcServer) -> None:
         """Init RPCFunctions."""
         self._xml_rpc_server: Final = xml_rpc_server
 
     def event(self, interface_id: str, channel_address: str, parameter: str, value: Any) -> None:
         """If a device emits some sort event, we will handle it here."""
         if central := self._xml_rpc_server.get_central(interface_id):
-            central.event(
-                interface_id=interface_id,
-                channel_address=channel_address,
-                parameter=parameter,
-                value=value,
+            central.create_task(
+                central.event(
+                    interface_id=interface_id,
+                    channel_address=channel_address,
+                    parameter=parameter,
+                    value=value,
+                ),
+                name=f"event-{interface_id}-{channel_address}-{parameter}",
             )
 
     @callback_system_event(system_event=SystemEvent.ERROR)
     def error(self, interface_id: str, error_code: str, msg: str) -> None:
         """When some error occurs the CCU / Homegear will send its error message here."""
         _LOGGER.warning(
             "ERROR failed: interface_id = %s, error_code = %i, message = %s",
@@ -58,24 +61,24 @@
         """Add new devices send from backend."""
         central: hmcu.CentralUnit | None
         if central := self._xml_rpc_server.get_central(interface_id):
             central.create_task(
                 central.add_new_devices(
                     interface_id=interface_id, device_descriptions=tuple(device_descriptions)
                 ),
-                name="newDevices",
+                name=f"newDevices-{interface_id}",
             )
 
     def deleteDevices(self, interface_id: str, addresses: list[str]) -> None:
         """Delete devices send from backend."""
         central: hmcu.CentralUnit | None
         if central := self._xml_rpc_server.get_central(interface_id):
             central.create_task(
                 central.delete_devices(interface_id=interface_id, addresses=tuple(addresses)),
-                name="deleteDevices",
+                name=f"deleteDevices-{interface_id}",
             )
 
     @callback_system_event(system_event=SystemEvent.UPDATE_DEVICE)
     def updateDevice(self, interface_id: str, address: str, hint: int) -> None:
         """
         Update a device.
```

### Comparing `hahomematic-2024.4.2/hahomematic/client/__init__.py` & `hahomematic-2024.4.3/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/client/json_rpc.py` & `hahomematic-2024.4.3/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/client/xml_rpc.py` & `hahomematic-2024.4.3/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/config.py` & `hahomematic-2024.4.3/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/const.py` & `hahomematic-2024.4.3/hahomematic/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 IDENTIFIER_SEPARATOR: Final = "@"
 DATETIME_FORMAT: Final = "%d.%m.%Y %H:%M:%S"
 DATETIME_FORMAT_MILLIS: Final = "%d.%m.%Y %H:%M:%S.%f'"
 INIT_DATETIME: Final = datetime.strptime("01.01.1970 00:00:00", DATETIME_FORMAT)
 IP_ANY_V4: Final = "0.0.0.0"
 PORT_ANY: Final = 0
+BLOCK_LOG_TIMEOUT = 60
 
 PATH_JSON_RPC: Final = "/api/homematic.cgi"
 
 HOMEGEAR_SERIAL = "Homegear_SN0815"
 
 PROGRAM_ADDRESS: Final = "program"
 SYSVAR_ADDRESS: Final = "sysvar"
```

### Comparing `hahomematic-2024.4.2/hahomematic/exceptions.py` & `hahomematic-2024.4.3/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/hmcli.py` & `hahomematic-2024.4.3/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/performance.py` & `hahomematic-2024.4.3/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/__init__.py` & `hahomematic-2024.4.3/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/const.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/light.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/support.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.4.3/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/decorators.py` & `hahomematic-2024.4.3/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/device.py` & `hahomematic-2024.4.3/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/entity.py` & `hahomematic-2024.4.3/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/event.py` & `hahomematic-2024.4.3/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/action.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/button.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/number.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/select.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.4.3/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/button.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/number.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/select.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/hub/text.py` & `hahomematic-2024.4.3/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/support.py` & `hahomematic-2024.4.3/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/platforms/update.py` & `hahomematic-2024.4.3/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.4.3/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.4.3/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.4.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic/support.py` & `hahomematic-2024.4.3/hahomematic/support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Helper functions used within hahomematic."""
 
 from __future__ import annotations
 
+import asyncio
 import base64
 from collections.abc import Collection
 import contextlib
 from dataclasses import dataclass
 from datetime import datetime
 from functools import lru_cache
 import logging
@@ -285,7 +286,12 @@
 
     @property
     def is_valid(self) -> bool:
         """Return if entry is valid."""
         if self.value == NO_CACHE_ENTRY:
             return False
         return changed_within_seconds(last_change=self.last_refresh)
+
+
+def cancelling(task: asyncio.Future[Any]) -> bool:
+    """Return True if task is cancelling."""
+    return bool((cancelling_ := getattr(task, "cancelling", None)) and cancelling_())
```

### Comparing `hahomematic-2024.4.2/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.4.3/hahomematic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.4.2/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.4.3/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/hahomematic_support/client_local.py` & `hahomematic-2024.4.3/hahomematic_support/client_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         channel_address: str,
         paramset_key: str,
         parameter: str,
         value: Any,
         rx_mode: str | None = None,
     ) -> bool:
         """Set single value on paramset VALUES."""
-        self.central.event(self.interface_id, channel_address, parameter, value)
+        await self.central.event(self.interface_id, channel_address, parameter, value)
         return True
 
     async def get_paramset(self, address: str, paramset_key: str) -> Any:
         """
         Return a paramset from CCU.
 
         Address is usually the channel_address,
@@ -248,15 +248,15 @@
         """
         Set paramsets manually.
 
         Address is usually the channel_address,
         but for bidcos devices there is a master paramset at the device.
         """
         for parameter in value:
-            self.central.event(self.interface_id, address, parameter, value[parameter])
+            await self.central.event(self.interface_id, address, parameter, value[parameter])
         return True
 
     async def _load_all_json_files(
         self,
         anchor: str,
         resource: str,
         include_list: list[str] | None = None,
```

### Comparing `hahomematic-2024.4.2/pyproject.toml` & `hahomematic-2024.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.4.2"
+version     = "2024.4.3"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.4.2/tests/test_action.py` & `hahomematic-2024.4.3/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_binary_sensor.py` & `hahomematic-2024.4.3/tests/test_binary_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         HmBinarySensor,
         central.get_generic_entity("VCU5864966:1", "STATE"),
     )
     assert binary_sensor.usage == EntityUsage.ENTITY
     assert binary_sensor.value is False
     assert binary_sensor.is_writeable is False
     assert binary_sensor.visible is True
-    central.event(const.INTERFACE_ID, "VCU5864966:1", "STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU5864966:1", "STATE", 1)
     assert binary_sensor.value is True
-    central.event(const.INTERFACE_ID, "VCU5864966:1", "STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU5864966:1", "STATE", 0)
     assert binary_sensor.value is False
-    central.event(const.INTERFACE_ID, "VCU5864966:1", "STATE", None)
+    await central.event(const.INTERFACE_ID, "VCU5864966:1", "STATE", None)
     assert binary_sensor.value is False
 
     call_count = len(mock_client.method_calls)
     await binary_sensor.send_value(True)
     assert call_count == len(mock_client.method_calls)
```

### Comparing `hahomematic-2024.4.2/tests/test_button.py` & `hahomematic-2024.4.3/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_central.py` & `hahomematic-2024.4.3/tests/test_central.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,15 +671,15 @@
 async def test_ping_pong(factory: helper.Factory) -> None:
     """Test central other methods."""
     central, client = await factory.get_default_central(TEST_DEVICES, do_mock_client=False)
     interface_id = client.interface_id
     await client.check_connection_availability(handle_ping_pong=True)
     assert client.ping_pong_cache.pending_pong_count == 1
     for ts_stored in list(client.ping_pong_cache._pending_pongs):
-        central.event(
+        await central.event(
             interface_id,
             "",
             Parameter.PONG,
             f"{interface_id}#{ts_stored.strftime(DATETIME_FORMAT_MILLIS)}",
         )
     assert client.ping_pong_cache.pending_pong_count == 0
 
@@ -712,15 +712,15 @@
 async def test_unknown_pong_failure(factory: helper.Factory) -> None:
     """Test central other methods."""
     central, client = await factory.get_default_central(TEST_DEVICES, do_mock_client=False)
     interface_id = client.interface_id
     count = 0
     max_count = PING_PONG_MISMATCH_COUNT + 1
     while count < max_count:
-        central.event(
+        await central.event(
             interface_id,
             "",
             Parameter.PONG,
             f"{interface_id}#{datetime.now().strftime(DATETIME_FORMAT_MILLIS)}",
         )
         count += 1
```

### Comparing `hahomematic-2024.4.2/tests/test_central_pydevccu.py` & `hahomematic-2024.4.3/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_climate.py` & `hahomematic-2024.4.3/tests/test_climate.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,38 +48,38 @@
     assert climate.temperature_unit == "°C"
     assert climate.min_temp == 6.0
     assert climate.max_temp == 30.0
     assert climate.supports_preset is False
     assert climate.target_temperature_step == 0.5
 
     assert climate.current_humidity is None
-    central.event(const.INTERFACE_ID, "VCU0000054:1", "HUMIDITY", 75)
+    await central.event(const.INTERFACE_ID, "VCU0000054:1", "HUMIDITY", 75)
     assert climate.current_humidity == 75
 
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
     last_call = call.set_value(
         channel_address="VCU0000054:2",
         paramset_key="VALUES",
         parameter="SETPOINT",
         value=12.0,
     )
     assert mock_client.method_calls[-1] == last_call
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
-    central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
+    await central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
 
     assert climate.hvac_mode == HvacMode.HEAT
     assert climate.hvac_modes == (HvacMode.HEAT,)
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (PresetMode.NONE,)
     assert climate.hvac_action is None
-    central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
+    await central.event(const.INTERFACE_ID, "VCU0000054:1", "TEMPERATURE", 11.0)
 
     # No new method call, because called methods has no implementation
     await climate.set_hvac_mode(HvacMode.HEAT)
     assert mock_client.method_calls[-1] == last_call
     await climate.set_preset_mode(PresetMode.NONE)
     assert mock_client.method_calls[-1] == last_call
     await climate.enable_away_mode_by_duration(hours=100, away_temperature=17.0)
@@ -102,40 +102,40 @@
     assert climate.usage == EntityUsage.CE_PRIMARY
     assert climate.min_temp == 5.0
     assert climate.max_temp == 30.5
     assert climate.supports_preset is True
     assert climate.target_temperature_step == 0.5
     assert climate.preset_mode == PresetMode.NONE
     assert climate.hvac_action is None
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "VALVE_STATE", 10)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "VALVE_STATE", 10)
     assert climate.hvac_action == HvacAction.HEAT
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "VALVE_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "VALVE_STATE", 0)
     assert climate.hvac_action == HvacAction.IDLE
     assert climate.current_humidity is None
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="SET_TEMPERATURE",
         value=12.0,
     )
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "ACTUAL_TEMPERATURE", 11.0)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "ACTUAL_TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
 
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.hvac_modes == (HvacMode.AUTO, HvacMode.HEAT, HvacMode.OFF)
     await climate.set_hvac_mode(HvacMode.HEAT)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4", paramset_key="VALUES", parameter="MANU_MODE", value=12.0
     )
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", ModeHmIP.MANU.value)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", ModeHmIP.MANU.value)
     assert climate.hvac_mode == HvacMode.HEAT
 
     await climate.set_hvac_mode(HvacMode.OFF)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU0000050:4",
         paramset_key="VALUES",
         value={"MANU_MODE": 12.0, "SET_TEMPERATURE": 4.5},
@@ -144,16 +144,16 @@
     assert climate.hvac_mode == HvacMode.OFF
     assert climate.hvac_action == HvacAction.OFF
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4", paramset_key="VALUES", parameter="AUTO_MODE", value=True
     )
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 0)
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "SET_TEMPERATURE", 24.0)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 0)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "SET_TEMPERATURE", 24.0)
     assert climate.hvac_mode == HvacMode.AUTO
 
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.COMFORT,
         PresetMode.ECO,
@@ -162,17 +162,17 @@
     await climate.set_preset_mode(PresetMode.BOOST)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="BOOST_MODE",
         value=True,
     )
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 3)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 3)
     assert climate.preset_mode == PresetMode.BOOST
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 2)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 2)
     assert climate.preset_mode == PresetMode.AWAY
     await climate.set_preset_mode(PresetMode.COMFORT)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="COMFORT_MODE",
         value=True,
@@ -181,15 +181,15 @@
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000050:4",
         paramset_key="VALUES",
         parameter="LOWERING_MODE",
         value=True,
     )
 
-    central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 3)
+    await central.event(const.INTERFACE_ID, "VCU0000050:4", "CONTROL_MODE", 3)
     call_count = len(mock_client.method_calls)
     await climate.set_preset_mode(PresetMode.BOOST)
     assert call_count == len(mock_client.method_calls)
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     call_count = len(mock_client.method_calls)
     await climate.set_hvac_mode(HvacMode.AUTO)
@@ -234,35 +234,35 @@
     )
     assert climate.usage == EntityUsage.CE_PRIMARY
     assert climate.min_temp == 5.0
     assert climate.max_temp == 30.5
     assert climate.supports_preset is True
     assert climate.target_temperature_step == 0.5
     assert climate.hvac_action == HvacAction.IDLE
-    central.event(const.INTERFACE_ID, "VCU1769958:9", "STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU1769958:9", "STATE", 1)
     assert climate.hvac_action == HvacAction.HEAT
-    central.event(const.INTERFACE_ID, "VCU1769958:9", "STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU1769958:9", "STATE", 0)
     assert climate.hvac_action == HvacAction.IDLE
 
     assert climate.current_humidity is None
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "HUMIDITY", 75)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "HUMIDITY", 75)
     assert climate.current_humidity == 75
 
     assert climate.target_temperature is None
     await climate.set_temperature(12.0)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1769958:1",
         paramset_key="VALUES",
         parameter="SET_POINT_TEMPERATURE",
         value=12.0,
     )
     assert climate.target_temperature == 12.0
 
     assert climate.current_temperature is None
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "ACTUAL_TEMPERATURE", 11.0)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "ACTUAL_TEMPERATURE", 11.0)
     assert climate.current_temperature == 11.0
 
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.hvac_modes == (HvacMode.AUTO, HvacMode.HEAT, HvacMode.OFF)
     assert climate.preset_mode == PresetMode.NONE
 
     await climate.set_hvac_mode(HvacMode.OFF)
@@ -276,37 +276,37 @@
 
     await climate.set_hvac_mode(HvacMode.HEAT)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU1769958:1",
         paramset_key="VALUES",
         value={"CONTROL_MODE": 1, "SET_POINT_TEMPERATURE": 5.0},
     )
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.MANU.value)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.MANU.value)
     assert climate.hvac_mode == HvacMode.HEAT
 
     assert climate.preset_mode == PresetMode.NONE
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.NONE,
     )
     await climate.set_preset_mode(PresetMode.BOOST)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1769958:1", paramset_key="VALUES", parameter="BOOST_MODE", value=True
     )
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     assert climate.preset_mode == PresetMode.BOOST
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU1769958:1",
         paramset_key="VALUES",
         value={"BOOST_MODE": False, "CONTROL_MODE": 0},
     )
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     assert climate.hvac_mode == HvacMode.AUTO
     assert climate.preset_modes == (
         PresetMode.BOOST,
         PresetMode.NONE,
         "week_program_1",
         "week_program_2",
         "week_program_3",
@@ -314,18 +314,18 @@
         "week_program_5",
         "week_program_6",
     )
     await climate.set_preset_mode(PresetMode.NONE)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1769958:1", paramset_key="VALUES", parameter="BOOST_MODE", value=False
     )
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AWAY.value)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AWAY.value)
     assert climate.preset_mode == PresetMode.AWAY
 
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_MODE", ModeHmIP.AUTO.value)
     await climate.set_preset_mode(PresetMode.WEEK_PROGRAM_1)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1769958:1", paramset_key="VALUES", parameter="ACTIVE_PROFILE", value=1
     )
     assert climate.preset_mode == PresetMode.WEEK_PROGRAM_1
 
     with freeze_time("2023-03-03 08:00:00"):
@@ -362,20 +362,20 @@
         value={
             "SET_POINT_MODE": 2,
             "PARTY_TIME_START": "2000_01_01 00:00",
             "PARTY_TIME_END": "2000_01_01 00:00",
         },
     )
 
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "BOOST_MODE", 1)
     call_count = len(mock_client.method_calls)
     await climate.set_preset_mode(PresetMode.BOOST)
     assert call_count == len(mock_client.method_calls)
 
-    central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_TEMPERATURE", 12.0)
+    await central.event(const.INTERFACE_ID, "VCU1769958:1", "SET_POINT_TEMPERATURE", 12.0)
     call_count = len(mock_client.method_calls)
     await climate.set_temperature(12.0)
     assert call_count == len(mock_client.method_calls)
 
     await climate.set_hvac_mode(HvacMode.AUTO)
     call_count = len(mock_client.method_calls)
     await climate.set_hvac_mode(HvacMode.AUTO)
```

### Comparing `hahomematic-2024.4.2/tests/test_cover.py` & `hahomematic-2024.4.3/tests/test_cover.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,35 +71,35 @@
         parameter="LEVEL",
         value=_CLOSED_LEVEL,
     )
     assert cover.current_position == 0
 
     assert cover.is_opening is None
     assert cover.is_closing is None
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 1)
     assert cover.is_opening is True
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 2)
     assert cover.is_closing is True
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "ACTIVITY_STATE", 0)
 
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.5)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.5)
     assert cover._channel_level == 0.5
     assert cover.current_position == 50
 
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.0)
     call_count = len(mock_client.method_calls)
     await cover.close()
     assert call_count == len(mock_client.method_calls)
 
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 1.0)
     call_count = len(mock_client.method_calls)
     await cover.open()
     assert call_count == len(mock_client.method_calls)
 
-    central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.4)
+    await central.event(const.INTERFACE_ID, "VCU8537918:3", "LEVEL", 0.4)
     call_count = len(mock_client.method_calls)
     await cover.set_position(position=40)
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
 async def test_ceipblind_dr(factory: helper.Factory) -> None:
@@ -115,42 +115,42 @@
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=81",
     )
-    central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", 0.81)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.is_closed is False
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=100,L=100",
     )
-    central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _OPEN_LEVEL)
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
     )
-    central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _CLOSED_LEVEL)
     assert cover.is_opening is None
     assert cover.is_closing is None
-    central.event(const.INTERFACE_ID, "VCU7807849:1", "ACTIVITY_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "ACTIVITY_STATE", 1)
     assert cover.is_opening is True
-    central.event(const.INTERFACE_ID, "VCU7807849:1", "ACTIVITY_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "ACTIVITY_STATE", 2)
     assert cover.is_closing is True
 
-    central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", 0.5)
+    await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", 0.5)
     assert cover._channel_level == 0.5
     assert cover.current_position == 50
 
 
 @pytest.mark.asyncio()
 async def test_cewindowdrive(factory: helper.Factory) -> None:
     """Test CeWindowDrive."""
@@ -215,82 +215,82 @@
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0xa2,0x00",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.81)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0xc8,0x00",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _OPEN_LEVEL)
     assert cover.current_position == 100
     assert cover.current_tilt_position == 0
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x00",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0xc8",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x5a",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.45)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x00",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x14,0x28",
     )
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.1)
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.2)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", 0.1)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
@@ -302,28 +302,28 @@
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="STOP",
         value=True,
     )
 
     await cover.open_tilt()
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.open_tilt()
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_LEVEL)
     assert call_count == len(mock_client.method_calls)
 
     await cover.close_tilt()
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.close_tilt()
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert call_count == len(mock_client.method_calls)
 
-    central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.4)
+    await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", 0.4)
     call_count = len(mock_client.method_calls)
     await cover.set_position(tilt_position=40)
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
 async def test_ceipblind(factory: helper.Factory) -> None:
@@ -337,111 +337,111 @@
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=81",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.81)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=100,L=100",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 1.0)
     assert cover.current_position == 100
     assert cover.current_tilt_position == 100
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.0)
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=100,L=0",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=45,L=0",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.45)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.0)
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=20,L=10",
     )
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.1)
-    central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.2)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", 0.1)
+    await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL", 0.5)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL", 0.5)
     assert cover._channel_level == 0.5
     assert cover.current_position == 50
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL_2", 0.8)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL_2", 0.8)
     assert cover._channel_tilt_level == 0.8
     assert cover.current_tilt_position == 80
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL", _CLOSED_LEVEL)
     assert cover._channel_level == _CLOSED_LEVEL
     assert cover.current_position == 0
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL_2", _CLOSED_LEVEL)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "LEVEL_2", _CLOSED_LEVEL)
     assert cover._channel_tilt_level == _CLOSED_LEVEL
     assert cover.current_tilt_position == 0
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 1)
     assert cover.is_opening
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 2)
     assert cover.is_closing
 
-    central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 3)
+    await central.event(const.INTERFACE_ID, "VCU1223813:3", "ACTIVITY_STATE", 3)
     assert cover.is_opening is False
     assert cover.is_closing is False
 
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4", paramset_key="VALUES", parameter="STOP", value=True
     )
@@ -456,77 +456,77 @@
 
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.0, "LEVEL": 0.81}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.81)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.81)
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 1.0, "LEVEL": 1.0}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 1.0)
     assert cover.current_position == 100
     assert cover.current_tilt_position == 100
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.0, "LEVEL": 0.0}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 1.0, "LEVEL": 0.0}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 1.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.45, "LEVEL": 0.0}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.45)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.45)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 45
 
     await cover.close_tilt()
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.0, "LEVEL": 0.0}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.0)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 0
 
     await cover.set_position(position=10, tilt_position=20)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3560967:1", paramset_key="VALUES", value={"LEVEL_2": 0.2, "LEVEL": 0.1}
     )
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.1)
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.2)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", 0.1)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", 0.2)
     assert cover.current_position == 10
     assert cover.current_tilt_position == 20
 
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 1)
     assert cover.is_opening
 
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 2)
     assert cover.is_closing
 
-    central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 3)
+    await central.event(const.INTERFACE_ID, "VCU3560967:1", "ACTIVITY_STATE", 3)
     assert cover.is_opening is False
     assert cover.is_closing is False
 
     await cover.stop()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3560967:1", paramset_key="VALUES", parameter="STOP", value=True
     )
@@ -543,44 +543,44 @@
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=1,
     )
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
     )
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
     assert cover.is_closed is True
     await cover.set_position(position=11)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=4,
     )
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 2)
     assert cover.current_position == 10
 
     await cover.set_position(position=5)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
     )
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
@@ -590,40 +590,44 @@
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3574044:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=2,
     )
 
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
 
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "SECTION", GarageDoorActivity.OPENING.value)
+    await central.event(
+        const.INTERFACE_ID, "VCU3574044:1", "SECTION", GarageDoorActivity.OPENING.value
+    )
     assert cover.is_opening is True
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "SECTION", GarageDoorActivity.CLOSING.value)
+    await central.event(
+        const.INTERFACE_ID, "VCU3574044:1", "SECTION", GarageDoorActivity.CLOSING.value
+    )
     assert cover.is_closing is True
 
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "SECTION", None)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "SECTION", None)
     assert cover.is_opening is None
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "SECTION", None)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "SECTION", None)
     assert cover.is_closing is None
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", None)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", None)
     assert cover.is_closed is None
 
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 0)
     call_count = len(mock_client.method_calls)
     await cover.close()
     assert call_count == len(mock_client.method_calls)
 
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 1)
     call_count = len(mock_client.method_calls)
     await cover.open()
     assert call_count == len(mock_client.method_calls)
 
-    central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU3574044:1", "DOOR_STATE", 2)
     call_count = len(mock_client.method_calls)
     await cover.vent()
     assert call_count == len(mock_client.method_calls)
 
 
 @pytest.mark.asyncio()
 async def test_cegaragetm(factory: helper.Factory) -> None:
@@ -636,44 +640,44 @@
     await cover.set_position(position=81)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=1,
     )
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
     )
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
     assert cover.is_closed is True
     await cover.set_position(position=11)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=4,
     )
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 2)
     assert cover.current_position == 10
 
     await cover.set_position(position=5)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=3,
     )
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 0)
     assert cover.current_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
@@ -683,21 +687,21 @@
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6166407:1",
         paramset_key="VALUES",
         parameter="DOOR_COMMAND",
         value=2,
     )
 
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", 1)
     assert cover.current_position == 100
 
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", GarageDoorActivity.OPENING)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", GarageDoorActivity.OPENING)
     assert cover.is_opening is True
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", GarageDoorActivity.CLOSING)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", GarageDoorActivity.CLOSING)
     assert cover.is_closing is True
 
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", None)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", None)
     assert cover.is_opening is None
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", None)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "SECTION", None)
     assert cover.is_closing is None
-    central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", None)
+    await central.event(const.INTERFACE_ID, "VCU6166407:1", "DOOR_STATE", None)
     assert cover.is_closed is None
```

### Comparing `hahomematic-2024.4.2/tests/test_decorator.py` & `hahomematic-2024.4.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_device.py` & `hahomematic-2024.4.3/tests/test_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,36 +46,36 @@
     device = central.get_device(address="VCU6354483")
     assert device.available is True
     for generic_entity in device.generic_entities:
         assert generic_entity.available is True
     for custom_entity in device.custom_entities:
         assert custom_entity.available is True
 
-    central.event(const.INTERFACE_ID, "VCU6354483:0", "UNREACH", 1)
+    await central.event(const.INTERFACE_ID, "VCU6354483:0", "UNREACH", 1)
     assert device.available is False
     for generic_entity in device.generic_entities:
         assert generic_entity.available is False
     for custom_entity in device.custom_entities:
         assert custom_entity.available is False
 
-    central.event(const.INTERFACE_ID, "VCU6354483:0", "UNREACH", 0)
+    await central.event(const.INTERFACE_ID, "VCU6354483:0", "UNREACH", 0)
     assert device.available is True
     for generic_entity in device.generic_entities:
         assert generic_entity.available is True
     for custom_entity in device.custom_entities:
         assert custom_entity.available is True
 
 
 @pytest.mark.asyncio()
 async def test_device_config_pending(factory: helper.Factory) -> None:
     """Test device availability."""
     central, _ = await factory.get_default_central(TEST_DEVICES)
     device = central.get_device(address="VCU2128127")
     assert device._e_config_pending.value is False
     last_save = central.paramset_descriptions.last_save
-    central.event(const.INTERFACE_ID, "VCU2128127:0", "CONFIG_PENDING", True)
+    await central.event(const.INTERFACE_ID, "VCU2128127:0", "CONFIG_PENDING", True)
     assert device._e_config_pending.value is True
     assert last_save == central.paramset_descriptions.last_save
-    central.event(const.INTERFACE_ID, "VCU2128127:0", "CONFIG_PENDING", False)
+    await central.event(const.INTERFACE_ID, "VCU2128127:0", "CONFIG_PENDING", False)
     assert device._e_config_pending.value is False
     await asyncio.sleep(2)
     assert last_save != central.paramset_descriptions.last_save
```

### Comparing `hahomematic-2024.4.2/tests/test_entity.py` & `hahomematic-2024.4.3/tests/test_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,20 @@
     )
     switch.register_entity_removed_callback(entity_removed_callback=device_removed_mock)
     assert switch.value is None
     assert (
         str(switch) == "address_path: switch/CentralTest-BidCos-RF/vcu2128127_4/, "
         "type: HmIP-BSM, name: HmIP-BSM_VCU2128127"
     )
-    central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
     assert factory.entity_event_mock.call_args_list[-1] == call(
         const.INTERFACE_ID, "VCU2128127:4", "STATE", 1
     )
     assert switch.value is True
-    central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 0)
     assert factory.entity_event_mock.call_args_list[-1] == call(
         const.INTERFACE_ID, "VCU2128127:4", "STATE", 0
     )
     assert switch.value is False
     await central.delete_devices(
         interface_id=const.INTERFACE_ID, addresses=[switch.device.device_address]
     )
@@ -91,20 +91,20 @@
     )
     switch.register_entity_removed_callback(entity_removed_callback=device_removed_mock)
     assert switch.value is None
     assert (
         str(switch) == "address_path: switch/CentralTest-BidCos-RF/vcu2128127_4_state/, "
         "type: HmIP-BSM, name: HmIP-BSM_VCU2128127 State ch4"
     )
-    central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 1)
     assert factory.entity_event_mock.call_args_list[-1] == call(
         const.INTERFACE_ID, "VCU2128127:4", "STATE", 1
     )
     assert switch.value is True
-    central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU2128127:4", "STATE", 0)
     assert factory.entity_event_mock.call_args_list[-1] == call(
         const.INTERFACE_ID, "VCU2128127:4", "STATE", 0
     )
     assert switch.value is False
     await central.delete_devices(
         interface_id=const.INTERFACE_ID, addresses=[switch.device.device_address]
     )
```

### Comparing `hahomematic-2024.4.2/tests/test_event.py` & `hahomematic-2024.4.3/tests/test_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @pytest.mark.asyncio()
 async def test_clickevent(factory: helper.Factory) -> None:
     """Test ClickEvent."""
     central, _ = await factory.get_default_central(TEST_DEVICES)
     event: ClickEvent = cast(ClickEvent, central.get_event("VCU2128127:1", "PRESS_SHORT"))
     assert event.usage == EntityUsage.EVENT
     assert event.event_type == EventType.KEYPRESS
-    central.event(const.INTERFACE_ID, "VCU2128127:1", "PRESS_SHORT", True)
+    await central.event(const.INTERFACE_ID, "VCU2128127:1", "PRESS_SHORT", True)
     assert factory.ha_event_mock.call_args_list[-1] == call(
         "homematic.keypress",
         {
             "interface_id": const.INTERFACE_ID,
             "address": "VCU2128127",
             "channel_no": 1,
             "device_type": "HmIP-BSM",
@@ -44,15 +44,15 @@
 @pytest.mark.asyncio()
 async def test_impulseevent(factory: helper.Factory) -> None:
     """Test ImpulseEvent."""
     central, _ = await factory.get_default_central(TEST_DEVICES)
     event: ImpulseEvent = cast(ImpulseEvent, central.get_event("VCU0000263:1", "SEQUENCE_OK"))
     assert event.usage == EntityUsage.EVENT
     assert event.event_type == EventType.IMPULSE
-    central.event(const.INTERFACE_ID, "VCU0000263:1", "SEQUENCE_OK", True)
+    await central.event(const.INTERFACE_ID, "VCU0000263:1", "SEQUENCE_OK", True)
     assert factory.ha_event_mock.call_args_list[-1] == call(
         "homematic.impulse",
         {
             "interface_id": const.INTERFACE_ID,
             "address": "VCU0000263",
             "channel_no": 1,
             "device_type": "HM-Sen-EP",
@@ -68,15 +68,15 @@
     central, _ = await factory.get_default_central(TEST_DEVICES)
     event: DeviceErrorEvent = cast(
         DeviceErrorEvent,
         central.get_event("VCU2128127:0", "ERROR_OVERHEAT"),
     )
     assert event.usage == EntityUsage.EVENT
     assert event.event_type == EventType.DEVICE_ERROR
-    central.event(const.INTERFACE_ID, "VCU2128127:0", "ERROR_OVERHEAT", True)
+    await central.event(const.INTERFACE_ID, "VCU2128127:0", "ERROR_OVERHEAT", True)
     assert factory.ha_event_mock.call_args_list[-1] == call(
         "homematic.device_error",
         {
             "interface_id": const.INTERFACE_ID,
             "address": "VCU2128127",
             "channel_no": 0,
             "device_type": "HmIP-BSM",
```

### Comparing `hahomematic-2024.4.2/tests/test_json_rpc.py` & `hahomematic-2024.4.3/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_light.py` & `hahomematic-2024.4.3/tests/test_light.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         value=0.10980392156862745,
     )
     assert light.brightness == 28
     assert light.brightness_pct == 10
     assert light.is_on
 
     assert light.channel_brightness is None
-    central.event(const.INTERFACE_ID, "VCU1399816:3", "LEVEL", 0.4)
+    await central.event(const.INTERFACE_ID, "VCU1399816:3", "LEVEL", 0.4)
     assert light.channel_brightness == 102
 
     await light.turn_on(on_time=5.0, ramp_time=6.0)
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU1399816:4",
         paramset_key="VALUES",
         value={"LEVEL": 0.10980392156862745, "RAMP_TIME": 6.0, "ON_TIME": 5.0},
@@ -190,17 +190,17 @@
     )
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU3747418:3", paramset_key="VALUES", parameter="PROGRAM", value=1
     )
 
     assert light.effect == "Slow color change"
 
-    central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", 201)
+    await central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", 201)
     assert light.hs_color == (0.0, 0.0)
-    central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", None)
+    await central.event(const.INTERFACE_ID, "VCU3747418:2", "COLOR", None)
     assert light.hs_color == (0.0, 0.0)
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
 
@@ -363,18 +363,18 @@
 
     await light.turn_on(hs_color=(300, 50))
     assert mock_client.method_calls[-1] == call.put_paramset(
         address="VCU3716619:8", paramset_key="VALUES", value={"COLOR": 5, "LEVEL": 1.0}
     )
     assert light.color_name == FixedColor.PURPLE
 
-    central.event(const.INTERFACE_ID, "VCU3716619:7", "LEVEL", 0.5)
+    await central.event(const.INTERFACE_ID, "VCU3716619:7", "LEVEL", 0.5)
     assert light.channel_brightness == 127
 
-    central.event(const.INTERFACE_ID, "VCU3716619:7", "COLOR", 1)
+    await central.event(const.INTERFACE_ID, "VCU3716619:7", "COLOR", 1)
     assert light.channel_hs_color == (240.0, 100.0)
     assert light.channel_color_name == FixedColor.BLUE
 
     await light.turn_off()
     light.set_on_time(18)
     await light.turn_on()
     assert mock_client.method_calls[-1] == call.put_paramset(
@@ -852,17 +852,17 @@
     assert mock_client.method_calls[-2] == call.set_value(
         channel_address="VCU9973336:15", paramset_key="VALUES", parameter="COLOR", value=200
     )
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9973336:13", paramset_key="VALUES", parameter="LEVEL", value=1.0
     )
     assert light.hs_color == (0.0, 0.0)
-    central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", 201)
+    await central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", 201)
     assert light.hs_color == (0.0, 0.0)
-    central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", None)
+    await central.event(const.INTERFACE_ID, "VCU9973336:15", "COLOR", None)
     assert light.hs_color == (0.0, 0.0)
 
     await light.turn_on()
     call_count = len(mock_client.method_calls)
     await light.turn_on()
     assert call_count == len(mock_client.method_calls)
```

### Comparing `hahomematic-2024.4.2/tests/test_lock.py` & `hahomematic-2024.4.3/tests/test_lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,30 +49,30 @@
         channel_address="VCU0000146:1",
         paramset_key="VALUES",
         parameter="OPEN",
         value=True,
     )
 
     assert lock.is_locking is None
-    central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 2)
+    await central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 2)
     assert lock.is_locking is True
-    central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 0)
+    await central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 0)
     assert lock.is_locking is False
 
     assert lock.is_unlocking is False
-    central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 1)
+    await central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 1)
     assert lock.is_unlocking is True
-    central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 0)
+    await central.event(const.INTERFACE_ID, "VCU0000146:1", "DIRECTION", 0)
     assert lock.is_unlocking is False
 
     assert lock.is_jammed is False
-    central.event(const.INTERFACE_ID, "VCU0000146:1", "ERROR", 2)
+    await central.event(const.INTERFACE_ID, "VCU0000146:1", "ERROR", 2)
     assert lock.is_jammed is True
 
-    central.event(const.INTERFACE_ID, "VCU0000146:1", "ERROR", 0)
+    await central.event(const.INTERFACE_ID, "VCU0000146:1", "ERROR", 0)
 
     await lock.open()
     call_count = len(mock_client.method_calls)
     await lock.open()
     assert (call_count + 1) == len(mock_client.method_calls)
 
 
@@ -87,43 +87,43 @@
     await lock.lock()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9724704:1",
         paramset_key="VALUES",
         parameter="LOCK_TARGET_LEVEL",
         value=0,
     )
-    central.event(const.INTERFACE_ID, "VCU9724704:1", "LOCK_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU9724704:1", "LOCK_STATE", 1)
     assert lock.is_locked is True
     await lock.unlock()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9724704:1",
         paramset_key="VALUES",
         parameter="LOCK_TARGET_LEVEL",
         value=1,
     )
-    central.event(const.INTERFACE_ID, "VCU9724704:1", "LOCK_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU9724704:1", "LOCK_STATE", 2)
     assert lock.is_locked is False
     await lock.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU9724704:1",
         paramset_key="VALUES",
         parameter="LOCK_TARGET_LEVEL",
         value=2,
     )
 
     assert lock.is_locking is None
-    central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 2)
     assert lock.is_locking is True
-    central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 0)
     assert lock.is_locking is False
 
     assert lock.is_unlocking is False
-    central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 1)
+    await central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 1)
     assert lock.is_unlocking is True
-    central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU9724704:1", "ACTIVITY_STATE", 0)
     assert lock.is_unlocking is False
 
     assert lock.is_jammed is False
 
     await lock.open()
     call_count = len(mock_client.method_calls)
     await lock.open()
```

### Comparing `hahomematic-2024.4.2/tests/test_number.py` & `hahomematic-2024.4.3/tests/test_number.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000011:3",
         paramset_key="VALUES",
         parameter="LEVEL",
         value=0.3,
     )
     assert efloat.value == 0.3
-    central.event(const.INTERFACE_ID, "VCU0000011:3", "LEVEL", 0.5)
+    await central.event(const.INTERFACE_ID, "VCU0000011:3", "LEVEL", 0.5)
     assert efloat.value == 0.5
     # do not write. value above max
     await efloat.send_value(45.0)
     assert efloat.value == 0.5
 
     call_count = len(mock_client.method_calls)
     await efloat.send_value(45.0)
@@ -112,15 +112,15 @@
         channel_address="VCU4984404:1",
         paramset_key="VALUES",
         parameter="SET_POINT_MODE",
         value=1,
     )
     assert einteger.value == 1
 
-    central.event(const.INTERFACE_ID, "VCU4984404:1", "SET_POINT_MODE", 2)
+    await central.event(const.INTERFACE_ID, "VCU4984404:1", "SET_POINT_MODE", 2)
     assert einteger.value == 2
     await einteger.send_value(6)
     assert mock_client.method_calls[-1] != call.set_value(
         channel_address="VCU4984404:1",
         paramset_key="VALUES",
         parameter="SET_POINT_MODE",
         value=6,
```

### Comparing `hahomematic-2024.4.2/tests/test_select.py` & `hahomematic-2024.4.3/tests/test_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU6354483:1",
         paramset_key="VALUES",
         parameter="WINDOW_STATE",
         value=1,
     )
     assert select.value == "OPEN"
-    central.event(const.INTERFACE_ID, "VCU6354483:1", "WINDOW_STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU6354483:1", "WINDOW_STATE", 0)
     assert select.value == "CLOSED"
 
     await select.send_value(3)
     # do not write. value above max
     assert select.value == "CLOSED"
 
     await select.send_value(1)
```

### Comparing `hahomematic-2024.4.2/tests/test_sensor.py` & `hahomematic-2024.4.3/tests/test_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,36 +26,36 @@
     """Test HmSensor."""
     central, _ = await factory.get_default_central(TEST_DEVICES)
     sensor: HmSensor = cast(HmSensor, central.get_generic_entity("VCU3941846:6", "VOLTAGE"))
     assert sensor.usage == EntityUsage.ENTITY
     assert sensor.unit == "V"
     assert sensor.values is None
     assert sensor.value is None
-    central.event(const.INTERFACE_ID, "VCU3941846:6", "VOLTAGE", 120)
+    await central.event(const.INTERFACE_ID, "VCU3941846:6", "VOLTAGE", 120)
     assert sensor.value == 120.0
-    central.event(const.INTERFACE_ID, "VCU3941846:6", "VOLTAGE", 234.00)
+    await central.event(const.INTERFACE_ID, "VCU3941846:6", "VOLTAGE", 234.00)
     assert sensor.value == 234.00
 
     sensor2: HmSensor = cast(
         HmSensor,
         central.get_generic_entity("VCU3941846:0", "RSSI_DEVICE"),
     )
     assert sensor2.usage == EntityUsage.ENTITY
     assert sensor2.unit == "dBm"
     assert sensor2.values is None
     assert sensor2.value is None
-    central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", 24)
+    await central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", 24)
     assert sensor2.value == -24
-    central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", -40)
+    await central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", -40)
     assert sensor2.value == -40
-    central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", -160)
+    await central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", -160)
     assert sensor2.value == -96
-    central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", 160)
+    await central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", 160)
     assert sensor2.value == -96
-    central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", 400)
+    await central.event(const.INTERFACE_ID, "VCU3941846:0", "RSSI_DEVICE", 400)
     assert sensor2.value is None
 
     sensor3: HmSensor = cast(
         HmSensor,
         central.get_generic_entity("VCU8205532:1", "CONCENTRATION"),
     )
     assert sensor3.usage == EntityUsage.ENTITY
@@ -69,17 +69,17 @@
     """Test HmSensor."""
     central, _ = await factory.get_default_central(TEST_DEVICES)
     sensor: HmSensor = cast(HmSensor, central.get_generic_entity("VCU7981740:1", "STATE"))
     assert sensor.usage == EntityUsage.ENTITY
     assert sensor.unit is None
     assert sensor.values == ("CLOSED", "TILTED", "OPEN")
     assert sensor.value is None
-    central.event(const.INTERFACE_ID, "VCU7981740:1", "STATE", 0)
+    await central.event(const.INTERFACE_ID, "VCU7981740:1", "STATE", 0)
     assert sensor.value == "CLOSED"
-    central.event(const.INTERFACE_ID, "VCU7981740:1", "STATE", 2)
+    await central.event(const.INTERFACE_ID, "VCU7981740:1", "STATE", 2)
     assert sensor.value == "OPEN"
 
 
 @pytest.mark.asyncio()
 async def test_hmsysvarsensor(factory: helper.Factory) -> None:
     """Test HmSysvarSensor."""
     central, _ = await factory.get_default_central({}, add_sysvars=True)
```

### Comparing `hahomematic-2024.4.2/tests/test_siren.py` & `hahomematic-2024.4.3/tests/test_siren.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 async def test_ceipsiren(factory: helper.Factory) -> None:
     """Test CeIpSiren."""
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     siren: CeIpSiren = cast(CeIpSiren, helper.get_prepared_custom_entity(central, "VCU8249617", 3))
     assert siren.usage == EntityUsage.CE_PRIMARY
 
     assert siren.is_on is False
-    central.event(const.INTERFACE_ID, "VCU8249617:3", "ACOUSTIC_ALARM_ACTIVE", 1)
+    await central.event(const.INTERFACE_ID, "VCU8249617:3", "ACOUSTIC_ALARM_ACTIVE", 1)
     assert siren.is_on is True
-    central.event(const.INTERFACE_ID, "VCU8249617:3", "ACOUSTIC_ALARM_ACTIVE", 0)
+    await central.event(const.INTERFACE_ID, "VCU8249617:3", "ACOUSTIC_ALARM_ACTIVE", 0)
     assert siren.is_on is False
-    central.event(const.INTERFACE_ID, "VCU8249617:3", "OPTICAL_ALARM_ACTIVE", 1)
+    await central.event(const.INTERFACE_ID, "VCU8249617:3", "OPTICAL_ALARM_ACTIVE", 1)
     assert siren.is_on is True
-    central.event(const.INTERFACE_ID, "VCU8249617:3", "OPTICAL_ALARM_ACTIVE", 0)
+    await central.event(const.INTERFACE_ID, "VCU8249617:3", "OPTICAL_ALARM_ACTIVE", 0)
     assert siren.is_on is False
 
     await siren.turn_on(
         acoustic_alarm="FREQUENCY_RISING_AND_FALLING",
         optical_alarm="BLINKING_ALTERNATELY_REPEATING",
         duration=30,
     )
@@ -107,21 +107,21 @@
     central, mock_client = await factory.get_default_central(TEST_DEVICES)
     siren: CeIpSirenSmoke = cast(
         CeIpSirenSmoke, helper.get_prepared_custom_entity(central, "VCU2822385", 1)
     )
     assert siren.usage == EntityUsage.CE_PRIMARY
 
     assert siren.is_on is False
-    central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 1)
+    await central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 1)
     assert siren.is_on is True
-    central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 2)
+    await central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 2)
     assert siren.is_on is True
-    central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 3)
+    await central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 3)
     assert siren.is_on is True
-    central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 0)
+    await central.event(const.INTERFACE_ID, "VCU2822385:1", "SMOKE_DETECTOR_ALARM_STATUS", 0)
     assert siren.is_on is False
 
     await siren.turn_on()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU2822385:1",
         paramset_key="VALUES",
         parameter="SMOKE_DETECTOR_COMMAND",
```

### Comparing `hahomematic-2024.4.2/tests/test_support.py` & `hahomematic-2024.4.3/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_switch.py` & `hahomematic-2024.4.3/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.4.2/tests/test_text.py` & `hahomematic-2024.4.3/tests/test_text.py`

 * *Files identical despite different names*

