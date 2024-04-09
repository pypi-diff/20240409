# Comparing `tmp/hhd-2.5.3.tar.gz` & `tmp/hhd-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhd-2.5.3.tar", last modified: Sat Apr  6 23:00:59 2024, max compression
+gzip compressed data, was "hhd-2.6.0.tar", last modified: Tue Apr  9 17:55:20 2024, max compression
```

## Comparing `hhd-2.5.3.tar` & `hhd-2.6.0.tar`

### file list

```diff
@@ -1,136 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 23:00:53.000000 hhd-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 23:00:53.000000 hhd-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-06 23:00:59.514540 hhd-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 23:00:53.000000 hhd-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-04-06 23:00:53.000000 hhd-2.5.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 23:00:59.514540 hhd-2.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.490540 hhd-2.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.498540 hhd-2.5.3/src/hhd/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.498540 hhd-2.5.3/src/hhd/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/contrib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/contrib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/contrib/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/contrib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/contrib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.498540 hhd-2.5.3/src/hhd/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/controller/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/lib/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/lib/hide.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/lib/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/lib/uhid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/controller/physical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/physical/evdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/physical/hidraw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/physical/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/physical/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/controller/virtual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/controller/virtual/dualsense/
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/dualsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/dualsense/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/controller/virtual/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/sd/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/controller/virtual/uinput/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/uinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/controller/virtual/uinput/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.494540 hhd-2.5.3/src/hhd/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.502540 hhd-2.5.3/src/hhd/device/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/generic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/generic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/generic/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.490540 hhd-2.5.3/src/hhd/device/gpd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.506540 hhd-2.5.3/src/hhd/device/gpd/win/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/gpd/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/gpd/win/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/gpd/win/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/gpd/win/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.506540 hhd-2.5.3/src/hhd/device/legion_go/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/legion_go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/legion_go/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/legion_go/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/legion_go/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/legion_go/gyro_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/legion_go/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.506540 hhd-2.5.3/src/hhd/device/orange_pi/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/orange_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/orange_pi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/orange_pi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/orange_pi/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.506540 hhd-2.5.3/src/hhd/device/rog_ally/
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/rog_ally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/rog_ally/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/rog_ally/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/rog_ally/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/device/rog_ally/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.510540 hhd-2.5.3/src/hhd/http/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/http/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/http/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.510540 hhd-2.5.3/src/hhd/http/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/http/static/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/http/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.510540 hhd-2.5.3/src/hhd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.510540 hhd-2.5.3/src/hhd/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/display/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/gyro.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/outputs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/src/hhd/plugins/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/overlay/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/overlay/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/overlay/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/overlay/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/src/hhd/plugins/powerbutton/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/powerbutton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/powerbutton/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/powerbutton/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/powerbutton/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/touchpad.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/sections.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 23:00:53.000000 hhd-2.5.3/src/hhd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/src/hhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-06 23:00:59.000000 hhd-2.5.3/src/hhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-06 23:00:59.000000 hhd-2.5.3/src/hhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 23:00:59.000000 hhd-2.5.3/src/hhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-06 23:00:59.000000 hhd-2.5.3/src/hhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 23:00:59.000000 hhd-2.5.3/src/hhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-06 23:00:59.000000 hhd-2.5.3/src/hhd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.494540 hhd-2.5.3/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.494540 hhd-2.5.3/usr/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/usr/lib/modules-load.d/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/modules-load.d/hhd-user.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.494540 hhd-2.5.3/usr/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/usr/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/systemd/system/hhd@.service
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/systemd/system/hhd_local@.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/usr/lib/systemd/user/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/systemd/user/hhd-user.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.494540 hhd-2.5.3/usr/lib/udev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/usr/lib/udev/hwdb.d/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/udev/hwdb.d/83-hhd.hwdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:00:59.514540 hhd-2.5.3/usr/lib/udev/rules.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/udev/rules.d/83-hhd-user.rules
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-06 23:00:53.000000 hhd-2.5.3/usr/lib/udev/rules.d/83-hhd.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.017581 hhd-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 17:55:12.000000 hhd-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 17:55:12.000000 hhd-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-09 17:55:20.017581 hhd-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-09 17:55:12.000000 hhd-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-09 17:55:12.000000 hhd-2.6.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:55:20.017581 hhd-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.993580 hhd-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.001581 hhd-2.6.0/src/hhd/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.001581 hhd-2.6.0/src/hhd/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/contrib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/contrib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/contrib/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/contrib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/contrib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.001581 hhd-2.6.0/src/hhd/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/controller/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/lib/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/lib/hide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/lib/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/lib/uhid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/controller/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/physical/evdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/physical/hidraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/physical/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/physical/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/controller/virtual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/controller/virtual/dualsense/
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/dualsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/dualsense/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/controller/virtual/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/sd/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/controller/virtual/uinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/uinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/controller/virtual/uinput/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.993580 hhd-2.6.0/src/hhd/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/device/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/generic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/generic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/generic/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.993580 hhd-2.6.0/src/hhd/device/gpd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.005581 hhd-2.6.0/src/hhd/device/gpd/win/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/gpd/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/gpd/win/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/gpd/win/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/gpd/win/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/device/legion_go/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/legion_go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/legion_go/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/legion_go/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/legion_go/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/legion_go/gyro_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/legion_go/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/device/orange_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/orange_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/orange_pi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/orange_pi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/orange_pi/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/device/rog_ally/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/rog_ally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/rog_ally/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/rog_ally/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/rog_ally/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/device/rog_ally/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/http/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/http/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/http/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/http/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/http/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/http/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.997581 hhd-2.6.0/src/hhd/i18n/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.009581 hhd-2.6.0/src/hhd/i18n/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-09 17:55:17.000000 hhd-2.6.0/src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16335 2024-04-09 17:55:17.000000 hhd-2.6.0/src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/src/hhd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/src/hhd/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/display/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/gyro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/outputs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/src/hhd/plugins/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/overlay/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/overlay/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/overlay/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/overlay/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/src/hhd/plugins/powerbutton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/powerbutton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/powerbutton/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/powerbutton/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/powerbutton/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/touchpad.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/sections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 17:55:12.000000 hhd-2.6.0/src/hhd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/src/hhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-04-09 17:55:19.000000 hhd-2.6.0/src/hhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-09 17:55:19.000000 hhd-2.6.0/src/hhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:55:19.000000 hhd-2.6.0/src/hhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 17:55:19.000000 hhd-2.6.0/src/hhd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 17:55:19.000000 hhd-2.6.0/src/hhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 17:55:19.000000 hhd-2.6.0/src/hhd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.997581 hhd-2.6.0/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.997581 hhd-2.6.0/usr/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/usr/lib/modules-load.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/modules-load.d/hhd-user.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.997581 hhd-2.6.0/usr/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/usr/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/systemd/system/hhd@.service
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/systemd/system/hhd_local@.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/usr/lib/systemd/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/systemd/user/hhd-user.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:19.997581 hhd-2.6.0/usr/lib/udev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/usr/lib/udev/hwdb.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/udev/hwdb.d/83-hhd.hwdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:55:20.013581 hhd-2.6.0/usr/lib/udev/rules.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/udev/rules.d/83-hhd-user.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 17:55:12.000000 hhd-2.6.0/usr/lib/udev/rules.d/83-hhd.rules
```

### Comparing `hhd-2.5.3/LICENSE` & `hhd-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/PKG-INFO` & `hhd-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.5.3
+Version: 2.6.0
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -499,35 +499,44 @@
 
 You can now either take a picture of your screen or translate the settings into
 text (e.g., x is k, y is l inverted, z is j) and open an issue.
 The override setting also displays the make and model of your device, which
 are required to add the mappings to Handheld Daemon.
 
 ### Localizing Handheld Daemon
-You can find `pot` and `po` files for Handheld Daemon under the  `i18n` directory.
+You can find `pot` and `po` files for Handheld Daemon under the `i18n` directory.
 You can clone/download this repository and open the `./i18n` directory.
-Then, just copy the `template.pot` file into `<your_locale>/LC_MESSAGES/messages.po`
+Then, just copy the `*.pot` files into `<your_locale>/LC_MESSAGES/*.po`
 and begin translating with your favorite text editor, or by using
 tool such as [Lokalize](https://apps.kde.org/lokalize/).
 
+As far as your locale goes, unless you have a good reason to, skip the territory
+code (e.g., `el` instead of `el_GR`).
+
 The files can be updated for a new version with the following commands:
 ```bash
 # Prepare dev environment
 git clone https://github.com/hhd-dev/hhd
 cd hhd
 python -m venv venv
 pip install babel
 pip install -e .
 
-# Generate POT file
-pybabel extract --no-location -F i18n/babel.cfg -o i18n/template.pot src/hhd
-# Update current pot files
-pybabel update -i i18n/template.pot -d i18n -D hhd
-# Generate PO files for your language (essentially a copy with a header change)
-pybabel init -i i18n/template.pot -l el_gr -d i18n -D hhd
+# Regenerate POT files
+pybabel extract --no-location -F i18n/babel.cfg -o i18n/hhd.pot src/hhd
+# Assuming adjustor is in an adjacent directory
+pybabel extract --no-location -F i18n/babel.cfg -o i18n/adjustor.pot ../adjustor/src/adjustor
+
+# Generate PO files for your language if they do not exist
+pybabel init -i i18n/hhd.pot -d i18n -D hhd -l YOUR_LANG
+pybabel init -i i18n/adjustor.pot -d i18n -D adjustor -l YOUR_LANG
+
+# Update current PO files for your language
+pybabel update -i i18n/hhd.pot -d i18n -D hhd -l YOUR_LANG
+pybabel update -i i18n/adjustor.pot -d i18n -D adjustor -l YOUR_LANG
 ```
 
 ### Creating a Local Repo version
 Either follow `Automatic Install` or `Manual Local Install` to install the base rules.
 Then, clone, optionally install the userspace rules, and run.
 ```bash
 # Clone Handheld Daemon
```

### Comparing `hhd-2.5.3/pyproject.toml` & `hhd-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhd"
-version = "2.5.3"
+version = "2.6.0"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Handheld Daemon, a tool for configuring handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -38,14 +38,15 @@
 orange_pi = "hhd.device.orange_pi:autodetect"
 generic = "hhd.device.generic:autodetect"
 powerbuttond = "hhd.plugins.powerbutton:autodetect"
 overlay = "hhd.plugins.overlay:autodetect"
 # display = "hhd.plugins.display:autodetect"
 
 [project.entry-points."hhd.i18n"]
+hhd = "hhd.i18n:locales"
 
 [project.entry-points."babel.extractors"]
 hhd_yaml = "hhd.contrib.i18n:extract_hhd_yaml"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `hhd-2.5.3/readme.md` & `hhd-2.6.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -478,35 +478,44 @@
 
 You can now either take a picture of your screen or translate the settings into
 text (e.g., x is k, y is l inverted, z is j) and open an issue.
 The override setting also displays the make and model of your device, which
 are required to add the mappings to Handheld Daemon.
 
 ### Localizing Handheld Daemon
-You can find `pot` and `po` files for Handheld Daemon under the  `i18n` directory.
+You can find `pot` and `po` files for Handheld Daemon under the `i18n` directory.
 You can clone/download this repository and open the `./i18n` directory.
-Then, just copy the `template.pot` file into `<your_locale>/LC_MESSAGES/messages.po`
+Then, just copy the `*.pot` files into `<your_locale>/LC_MESSAGES/*.po`
 and begin translating with your favorite text editor, or by using
 tool such as [Lokalize](https://apps.kde.org/lokalize/).
 
+As far as your locale goes, unless you have a good reason to, skip the territory
+code (e.g., `el` instead of `el_GR`).
+
 The files can be updated for a new version with the following commands:
 ```bash
 # Prepare dev environment
 git clone https://github.com/hhd-dev/hhd
 cd hhd
 python -m venv venv
 pip install babel
 pip install -e .
 
-# Generate POT file
-pybabel extract --no-location -F i18n/babel.cfg -o i18n/template.pot src/hhd
-# Update current pot files
-pybabel update -i i18n/template.pot -d i18n -D hhd
-# Generate PO files for your language (essentially a copy with a header change)
-pybabel init -i i18n/template.pot -l el_gr -d i18n -D hhd
+# Regenerate POT files
+pybabel extract --no-location -F i18n/babel.cfg -o i18n/hhd.pot src/hhd
+# Assuming adjustor is in an adjacent directory
+pybabel extract --no-location -F i18n/babel.cfg -o i18n/adjustor.pot ../adjustor/src/adjustor
+
+# Generate PO files for your language if they do not exist
+pybabel init -i i18n/hhd.pot -d i18n -D hhd -l YOUR_LANG
+pybabel init -i i18n/adjustor.pot -d i18n -D adjustor -l YOUR_LANG
+
+# Update current PO files for your language
+pybabel update -i i18n/hhd.pot -d i18n -D hhd -l YOUR_LANG
+pybabel update -i i18n/adjustor.pot -d i18n -D adjustor -l YOUR_LANG
 ```
 
 ### Creating a Local Repo version
 Either follow `Automatic Install` or `Manual Local Install` to install the base rules.
 Then, clone, optionally install the userspace rules, and run.
 ```bash
 # Clone Handheld Daemon
```

### Comparing `hhd-2.5.3/src/hhd/__main__.py` & `hhd-2.6.0/src/hhd/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,14 +219,30 @@
             p.validate(tags, config, value) for p in sorted_plugins
         )
 
         if not sorted_plugins:
             logger.error(f"No plugins started, exiting...")
             return
 
+        # Load locales
+        locales = []
+        for register in pkg_resources.iter_entry_points("hhd.i18n"):
+            locales.extend(register.resolve()())
+        locales.sort(key=lambda x: x["priority"], reverse=True)
+
+        if locales:
+            lstr = "Loaded the following locales:\n"
+            for locale in locales:
+                lstr += (
+                    f" - {locale['domain']} ({locale['priority']}): {locale['dir']}\n"
+                )
+            logger.info(lstr[:-1])
+        else:
+            logger.info("No locales found.")
+
         # Open plugins
         lock = RLock()
         cond = Condition(lock)
         emit = EmitHolder(cond, ctx)
         for p in sorted_plugins:
             set_log_plugin(getattr(p, "log") if hasattr(p, "log") else "ukwn")
             p.open(emit, ctx)
@@ -412,15 +428,15 @@
                             with open(token_fn, "r") as f:
                                 token = f.read().strip()
                     else:
                         token = None
 
                     set_log_plugin("rest")
                     https = HHDHTTPServer(localhost, port, token)
-                    https.update(settings, conf, info, profiles, emit)
+                    https.update(settings, conf, info, profiles, emit, locales, ctx)
                     try:
                         https.open()
                     except Exception as e:
                         logger.error(
                             f"Could not start http API on port {port}.\n"
                             + "Is another version of Handheld Daemon open?\n"
                             + "Closing."
@@ -517,15 +533,15 @@
                 p.update(conf)
                 update_log_plugins()
             set_log_plugin("ukwn")
 
             # Notify that events were applied
             # Before saving to reduce delay (yaml files take 100ms :( )
             if https:
-                https.update(settings, conf, info, profiles, emit)
+                https.update(settings, conf, info, profiles, emit, locales, ctx)
 
             #
             # Save loop
             #
 
             has_new = should_initialize.is_set()
             saved = False
```

### Comparing `hhd-2.5.3/src/hhd/contrib/dev.py` & `hhd-2.6.0/src/hhd/contrib/dev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/contrib/gs.py` & `hhd-2.6.0/src/hhd/contrib/gs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/contrib/i18n.py` & `hhd-2.6.0/src/hhd/contrib/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/contrib/main.py` & `hhd-2.6.0/src/hhd/contrib/main.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/__init__.py` & `hhd-2.6.0/src/hhd/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/base.py` & `hhd-2.6.0/src/hhd/controller/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/const.py` & `hhd-2.6.0/src/hhd/controller/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/lib/common.py` & `hhd-2.6.0/src/hhd/controller/lib/common.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/lib/hid.py` & `hhd-2.6.0/src/hhd/controller/lib/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/lib/hide.py` & `hhd-2.6.0/src/hhd/controller/lib/hide.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/lib/ioctl.py` & `hhd-2.6.0/src/hhd/controller/lib/ioctl.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/lib/uhid.py` & `hhd-2.6.0/src/hhd/controller/lib/uhid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/physical/evdev.py` & `hhd-2.6.0/src/hhd/controller/physical/evdev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/physical/hidraw.py` & `hhd-2.6.0/src/hhd/controller/physical/hidraw.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/physical/imu.py` & `hhd-2.6.0/src/hhd/controller/physical/imu.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/physical/rgb.py` & `hhd-2.6.0/src/hhd/controller/physical/rgb.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/virtual/dualsense/__init__.py` & `hhd-2.6.0/src/hhd/controller/virtual/dualsense/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/virtual/dualsense/const.py` & `hhd-2.6.0/src/hhd/controller/virtual/dualsense/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/virtual/sd/__init__.py` & `hhd-2.6.0/src/hhd/controller/virtual/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/virtual/sd/const.py` & `hhd-2.6.0/src/hhd/controller/virtual/sd/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/virtual/uinput/__init__.py` & `hhd-2.6.0/src/hhd/controller/virtual/uinput/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/controller/virtual/uinput/const.py` & `hhd-2.6.0/src/hhd/controller/virtual/uinput/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/generic/__init__.py` & `hhd-2.6.0/src/hhd/device/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/generic/base.py` & `hhd-2.6.0/src/hhd/device/generic/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     context: Context,
     should_exit: TEvent,
     updated: TEvent,
     dconf: dict,
 ):
     first = True
     init = time.perf_counter()
+    repeated_fail = False
     while not should_exit.is_set():
         if conf["controller_mode.mode"].to(str) == "disabled":
             time.sleep(ERROR_DELAY)
             continue
 
         try:
             found_device = bool(enumerate_evs(vid=GAMEPAD_VID))
```

### Comparing `hhd-2.5.3/src/hhd/device/generic/const.py` & `hhd-2.6.0/src/hhd/device/generic/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/generic/controllers.yml` & `hhd-2.6.0/src/hhd/device/generic/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/gpd/win/__init__.py` & `hhd-2.6.0/src/hhd/device/gpd/win/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/gpd/win/base.py` & `hhd-2.6.0/src/hhd/device/gpd/win/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/gpd/win/const.py` & `hhd-2.6.0/src/hhd/device/gpd/win/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/gpd/win/controllers.yml` & `hhd-2.6.0/src/hhd/device/gpd/win/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/legion_go/__init__.py` & `hhd-2.6.0/src/hhd/device/legion_go/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/legion_go/base.py` & `hhd-2.6.0/src/hhd/device/legion_go/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/legion_go/const.py` & `hhd-2.6.0/src/hhd/device/legion_go/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/legion_go/controllers.yml` & `hhd-2.6.0/src/hhd/device/legion_go/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/legion_go/gyro_fix.py` & `hhd-2.6.0/src/hhd/device/legion_go/gyro_fix.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/legion_go/hid.py` & `hhd-2.6.0/src/hhd/device/legion_go/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/orange_pi/__init__.py` & `hhd-2.6.0/src/hhd/device/orange_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/orange_pi/base.py` & `hhd-2.6.0/src/hhd/device/orange_pi/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/orange_pi/const.py` & `hhd-2.6.0/src/hhd/device/orange_pi/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/orange_pi/controllers.yml` & `hhd-2.6.0/src/hhd/device/orange_pi/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/rog_ally/__init__.py` & `hhd-2.6.0/src/hhd/device/rog_ally/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/rog_ally/base.py` & `hhd-2.6.0/src/hhd/device/rog_ally/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/rog_ally/const.py` & `hhd-2.6.0/src/hhd/device/rog_ally/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/rog_ally/controllers.yml` & `hhd-2.6.0/src/hhd/device/rog_ally/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/device/rog_ally/hid.py` & `hhd-2.6.0/src/hhd/device/rog_ally/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/http/api.py` & `hhd-2.6.0/src/hhd/http/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 import json
 import logging
 import os
 from copy import deepcopy
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from socketserver import ThreadingMixIn
 from threading import Condition, Thread
-from typing import Any, Mapping, cast
+from typing import Any, Mapping, Sequence, cast
 from urllib.parse import parse_qs, urlparse
 
 from hhd.plugins import (
     Config,
+    Context,
     Emitter,
+    HHDLocale,
     HHDSettings,
     get_relative_fn,
     load_relative_yaml,
 )
 
+from .i18n import get_user_lang, translate, translate_ver
+
 logger = logging.getLogger(__name__)
 
 
 def sanitize_name(n: str):
     import re
 
     return re.sub(r"[^ a-zA-Z0-9]+", "", n)
@@ -74,14 +78,17 @@
 class RestHandler(BaseHTTPRequestHandler):
     settings: HHDSettings
     cond: Condition
     conf: Config
     info: Config
     profiles: Mapping[str, Config]
     emit: Emitter
+    locales: Sequence[HHDLocale]
+    ctx: Context
+    user_lang: str | None
     token: str | None
 
     def set_response(self, code: int, headers: dict[str, str] = {}):
         # Allow skipping CORS by responding with specific origin
         if og := self.headers.get("Origin", None):
             headers = {**headers, "Access-Control-Allow-Origin": og}
         self.send_response(code)
@@ -230,14 +237,17 @@
                     # Return the profile
                     self.send_json(self.conf.conf)
                 case other:
                     self.send_not_found(f"Command 'profile/{other}' not supported.")
 
     def v1_endpoint(self, content: Any | None):
         segments, params = parse_path(self.path)
+        langs = params.get("lang", params.get("locale", None))
+        lang = langs[0] if langs else None
+
         if not segments:
             return self.send_not_found(f"Empty path.")
 
         if segments[0] != "api":
             return self.send_not_found(
                 f"Only the API endpoint ('/api/v1') is supported for now."
             )
@@ -251,49 +261,49 @@
             return self.send_not_found(f"No command provided")
 
         command = segments[2].lower()
         match command:
             case "profile":
                 self.handle_profile(segments[3:], params, content)
             case "settings":
-                v = self.conf.get("version", "")
+                v = translate_ver(self.conf)
                 self.set_response_ok({"Version": v})
                 with self.cond:
                     s = dict(deepcopy(self.settings))
                     try:
                         s["hhd"]["version"] = {  # type: ignore
                             "type": "version",
                             "tags": ["non-essential", "advanced", "expert", "hide"],
                             "value": v,
                         }
                     except Exception as e:
                         logger.error(f"Error while writing version hash to response.")
+                    s = translate(s, self.conf, self.locales, lang=lang, user_lang=self.user_lang)
                     self.wfile.write(json.dumps(s).encode())
             case "state":
                 self.set_response_ok()
                 with self.cond:
                     if content:
                         if not isinstance(content, Mapping):
                             return self.send_error(
                                 f"State content should be a dictionary."
                             )
                         self.emit({"type": "state", "config": Config(content)})
                         self.cond.wait()
                     elif "poll" in params:
                         # Hang for the next update if the UI requests it.
                         self.cond.wait()
-                    self.wfile.write(
-                        json.dumps(
-                            {**cast(dict, self.conf.conf), "info": self.info.conf}
-                        ).encode()
-                    )
+                    out = {**cast(dict, self.conf.conf), "info": self.info.conf}
+                    out["version"] = translate_ver(self.conf, lang=lang, user_lang=self.user_lang)
+                    out = translate(out, self.conf, self.locales, lang=lang, user_lang=self.user_lang)
+                    self.wfile.write(json.dumps(out).encode())
             case "version":
                 self.send_json({"version": 5})
             case "sections":
-                self.send_json(SECTIONS)
+                self.send_json(translate(SECTIONS, self.conf, self.locales, lang=lang, user_lang=self.user_lang))
             case other:
                 self.send_not_found(f"Command '{other}' not supported.")
 
     def do_GET(self):
         # Danger zone unauthenticated
         # Be very careful
         try:
@@ -381,21 +391,26 @@
     def update(
         self,
         settings: HHDSettings,
         conf: Config,
         info: Config,
         profiles: Mapping[str, Config],
         emit: Emitter,
+        locales: Sequence[HHDLocale],
+        ctx: Context,
     ):
         with self.cond:
             self.handler.settings = settings
             self.handler.conf = conf
             self.handler.info = info
             self.handler.profiles = profiles
             self.handler.emit = emit
+            self.handler.locales = locales
+            self.handler.ctx = ctx
+            self.handler.user_lang = get_user_lang(ctx)
             self.cond.notify_all()
 
     def open(self):
         self.https = ThreadingSimpleServer(
             ("127.0.0.1" if self.localhost else "", self.port), self.handler
         )
         self.t = Thread(target=self.https.serve_forever)
```

### Comparing `hhd-2.5.3/src/hhd/http/index.html` & `hhd-2.6.0/src/hhd/http/index.html`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/http/static/index.js` & `hhd-2.6.0/src/hhd/http/static/index.js`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/logging.py` & `hhd-2.6.0/src/hhd/logging.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/__init__.py` & `hhd-2.6.0/src/hhd/plugins/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from .conf import Config
-from .plugin import HHDAutodetect, HHDPlugin, Context, Emitter, Event
+from .plugin import (
+    HHDAutodetect,
+    HHDPlugin,
+    Context,
+    Emitter,
+    Event,
+    HHDLocale,
+    HHDLocaleRegister,
+)
 from .settings import HHDSettings
 from .utils import get_relative_fn, load_relative_yaml
 from .outputs import get_outputs_config, get_outputs
 from .inputs import get_touchpad_config, get_gyro_config, get_gyro_state, gen_gyro_state
 
 
 __all__ = [
@@ -18,8 +26,10 @@
     "Context",
     "get_outputs_config",
     "get_outputs",
     "get_touchpad_config",
     "get_gyro_config",
     "get_gyro_state",
     "gen_gyro_state",
+    "HHDLocale",
+    "HHDLocaleRegister",
 ]
```

### Comparing `hhd-2.5.3/src/hhd/plugins/conf.py` & `hhd-2.6.0/src/hhd/plugins/conf.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/display/__init__.py` & `hhd-2.6.0/src/hhd/plugins/display/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/gyro.yml` & `hhd-2.6.0/src/hhd/plugins/gyro.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/inputs.py` & `hhd-2.6.0/src/hhd/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/outputs.py` & `hhd-2.6.0/src/hhd/plugins/outputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/outputs.yml` & `hhd-2.6.0/src/hhd/plugins/outputs.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/overlay/__init__.py` & `hhd-2.6.0/src/hhd/plugins/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/overlay/base.py` & `hhd-2.6.0/src/hhd/plugins/overlay/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/overlay/controllers.py` & `hhd-2.6.0/src/hhd/plugins/overlay/controllers.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/overlay/overlay.py` & `hhd-2.6.0/src/hhd/plugins/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/overlay/x11.py` & `hhd-2.6.0/src/hhd/plugins/overlay/x11.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/plugin.py` & `hhd-2.6.0/src/hhd/plugins/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,14 +105,25 @@
 
 
 class HHDAutodetect(Protocol):
     def __call__(self, existing: Sequence[HHDPlugin]) -> Sequence[HHDPlugin]:
         raise NotImplementedError()
 
 
+class HHDLocale(TypedDict):
+    dir: str
+    domain: str
+    priority: int
+
+
+class HHDLocaleRegister(Protocol):
+    def __call__(self) -> Sequence[HHDLocale]:
+        raise NotImplementedError()
+
+
 def get_context(user: str | None) -> Context | None:
     try:
         uid = os.getuid()
         gid = os.getgid()
 
         if not user:
             if not uid:
```

### Comparing `hhd-2.5.3/src/hhd/plugins/powerbutton/__init__.py` & `hhd-2.6.0/src/hhd/plugins/powerbutton/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/powerbutton/base.py` & `hhd-2.6.0/src/hhd/plugins/powerbutton/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/powerbutton/const.py` & `hhd-2.6.0/src/hhd/plugins/powerbutton/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/settings.py` & `hhd-2.6.0/src/hhd/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/touchpad.yml` & `hhd-2.6.0/src/hhd/plugins/touchpad.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/plugins/utils.py` & `hhd-2.6.0/src/hhd/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd/settings.yml` & `hhd-2.6.0/src/hhd/settings.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 settings:
   type: container
   title: Core Settings
   tags: [non-essential]
 
   children:
+    language:
+      type: multiple
+      tags: [i18n, non-essential, language]
+      title: Language [BETA]
+      default: system
+      options:
+        system: System
+        C: English
+        zh: Chinese
+        # pt: Portugese
+
     theme:
       type: multiple
       tags: [theme-selector, advanced]
       title: "Theme"
       hint: >-
         Allows changing the theme in the UI.
         Default is either Diavolo or your distribution's theme.
```

### Comparing `hhd-2.5.3/src/hhd/utils.py` & `hhd-2.6.0/src/hhd/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/src/hhd.egg-info/PKG-INFO` & `hhd-2.6.0/src/hhd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.5.3
+Version: 2.6.0
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -499,35 +499,44 @@
 
 You can now either take a picture of your screen or translate the settings into
 text (e.g., x is k, y is l inverted, z is j) and open an issue.
 The override setting also displays the make and model of your device, which
 are required to add the mappings to Handheld Daemon.
 
 ### Localizing Handheld Daemon
-You can find `pot` and `po` files for Handheld Daemon under the  `i18n` directory.
+You can find `pot` and `po` files for Handheld Daemon under the `i18n` directory.
 You can clone/download this repository and open the `./i18n` directory.
-Then, just copy the `template.pot` file into `<your_locale>/LC_MESSAGES/messages.po`
+Then, just copy the `*.pot` files into `<your_locale>/LC_MESSAGES/*.po`
 and begin translating with your favorite text editor, or by using
 tool such as [Lokalize](https://apps.kde.org/lokalize/).
 
+As far as your locale goes, unless you have a good reason to, skip the territory
+code (e.g., `el` instead of `el_GR`).
+
 The files can be updated for a new version with the following commands:
 ```bash
 # Prepare dev environment
 git clone https://github.com/hhd-dev/hhd
 cd hhd
 python -m venv venv
 pip install babel
 pip install -e .
 
-# Generate POT file
-pybabel extract --no-location -F i18n/babel.cfg -o i18n/template.pot src/hhd
-# Update current pot files
-pybabel update -i i18n/template.pot -d i18n -D hhd
-# Generate PO files for your language (essentially a copy with a header change)
-pybabel init -i i18n/template.pot -l el_gr -d i18n -D hhd
+# Regenerate POT files
+pybabel extract --no-location -F i18n/babel.cfg -o i18n/hhd.pot src/hhd
+# Assuming adjustor is in an adjacent directory
+pybabel extract --no-location -F i18n/babel.cfg -o i18n/adjustor.pot ../adjustor/src/adjustor
+
+# Generate PO files for your language if they do not exist
+pybabel init -i i18n/hhd.pot -d i18n -D hhd -l YOUR_LANG
+pybabel init -i i18n/adjustor.pot -d i18n -D adjustor -l YOUR_LANG
+
+# Update current PO files for your language
+pybabel update -i i18n/hhd.pot -d i18n -D hhd -l YOUR_LANG
+pybabel update -i i18n/adjustor.pot -d i18n -D adjustor -l YOUR_LANG
 ```
 
 ### Creating a Local Repo version
 Either follow `Automatic Install` or `Manual Local Install` to install the base rules.
 Then, clone, optionally install the userspace rules, and run.
 ```bash
 # Clone Handheld Daemon
```

### Comparing `hhd-2.5.3/src/hhd.egg-info/SOURCES.txt` & `hhd-2.6.0/src/hhd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,21 @@
 src/hhd/device/rog_ally/__init__.py
 src/hhd/device/rog_ally/base.py
 src/hhd/device/rog_ally/const.py
 src/hhd/device/rog_ally/controllers.yml
 src/hhd/device/rog_ally/hid.py
 src/hhd/http/__init__.py
 src/hhd/http/api.py
+src/hhd/http/i18n.py
 src/hhd/http/index.html
 src/hhd/http/static/index.js
 src/hhd/http/static/style.css
+src/hhd/i18n/__init__.py
+src/hhd/i18n/zh/LC_MESSAGES/adjustor.mo
+src/hhd/i18n/zh/LC_MESSAGES/hhd.mo
 src/hhd/plugins/__init__.py
 src/hhd/plugins/conf.py
 src/hhd/plugins/gyro.yml
 src/hhd/plugins/inputs.py
 src/hhd/plugins/outputs.py
 src/hhd/plugins/outputs.yml
 src/hhd/plugins/plugin.py
```

### Comparing `hhd-2.5.3/usr/lib/udev/hwdb.d/83-hhd.hwdb` & `hhd-2.6.0/usr/lib/udev/hwdb.d/83-hhd.hwdb`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/usr/lib/udev/rules.d/83-hhd-user.rules` & `hhd-2.6.0/usr/lib/udev/rules.d/83-hhd-user.rules`

 * *Files identical despite different names*

### Comparing `hhd-2.5.3/usr/lib/udev/rules.d/83-hhd.rules` & `hhd-2.6.0/usr/lib/udev/rules.d/83-hhd.rules`

 * *Files identical despite different names*

