# Comparing `tmp/vaccines-1.0.0.tar.gz` & `tmp/vaccines-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaccines-1.0.0.tar", last modified: Tue Apr  9 01:15:16 2024, max compression
+gzip compressed data, was "vaccines-1.0.1.tar", last modified: Tue Apr  9 01:16:20 2024, max compression
```

## Comparing `vaccines-1.0.0.tar` & `vaccines-1.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.637035 vaccines-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-09 01:15:16.637035 vaccines-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/structures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/structures/vaccines/
--rw-r--r--   0 root         (0) root         (0)     2417 2024-04-09 01:04:32.000000 vaccines-1.0.0/modules/structures/vaccines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/structures/vaccines/_coms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/_coms/clique_pro/
--rw-rw-r--   0 root         (0) root         (0)      986 2024-04-09 01:04:34.000000 vaccines-1.0.0/modules/structures/vaccines/_coms/clique_pro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/_coms/clique_pro/group/
--rw-r--r--   0 root         (0) root         (0)     1975 2024-04-09 01:04:35.000000 vaccines-1.0.0/modules/structures/vaccines/_coms/clique_pro/group/trends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/_coms/sanic_pro/
--rw-rw-r--   0 root         (0) root         (0)       10 2024-04-03 22:13:22.000000 vaccines-1.0.0/modules/structures/vaccines/_coms/sanic_pro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/_status/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-16 20:58:19.000000 vaccines-1.0.0/modules/structures/vaccines/_status/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/structures/vaccines/_status/monitors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/_status/monitors/1_mongo_trends_on/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-09 01:04:35.000000 vaccines-1.0.0/modules/structures/vaccines/_status/monitors/1_mongo_trends_on/monitor_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/structures/vaccines/_status/monitors_process/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/_status/monitors_process/1/
--rw-r--r--   0 root         (0) root         (0)       96 2024-02-01 19:10:00.000000 vaccines-1.0.0/modules/structures/vaccines/_status/monitors_process/1/monitor_1.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-04-03 21:59:14.000000 vaccines-1.0.0/modules/structures/vaccines/_status/status.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/climate/
--rw-r--r--   0 root         (0) root         (0)     2643 2024-04-09 01:04:35.000000 vaccines-1.0.0/modules/structures/vaccines/climate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/climate/mongo/
--rw-rw-r--   0 root         (0) root         (0)       84 2024-04-03 22:33:06.000000 vaccines-1.0.0/modules/structures/vaccines/climate/mongo/connection_string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/climate/moves/
--rw-rw-r--   0 root         (0) root         (0)     1354 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/climate/moves/scan_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/config/
--rw-r--r--   0 root         (0) root         (0)     1354 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/config/scan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/mints/
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/mints/clique.py
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/mints/names.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.629035 vaccines-1.0.0/modules/structures/vaccines/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/modules/freight--/
--rw-rw-r--   0 root         (0) root         (0)     1041 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/modules/freight--/save.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/modules/moves/
--rw-rw-r--   0 root         (0) root         (0)     1165 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/mint_to_trends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/modules/moves/save/
--rw-rw-r--   0 root         (0) root         (0)      944 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/save/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/modules/moves/save/modules/
--rw-rw-r--   0 root         (0) root         (0)     1919 2024-04-09 01:04:37.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/save/modules/zip_and_save_to_gridfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/
--rw-rw-r--   0 root         (0) root         (0)     1086 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/extract_to_temp.py
--rw-rw-r--   0 root         (0) root         (0)      374 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/find.py
--rw-rw-r--   0 root         (0) root         (0)     1147 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/forget.py
--rw-rw-r--   0 root         (0) root         (0)      410 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/off.py
--rw-rw-r--   0 root         (0) root         (0)     1929 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/on.py
--rw-rw-r--   0 root         (0) root         (0)      365 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/show.py
--rw-rw-r--   0 root         (0) root         (0)      518 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.633035 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/zips/
--rw-rw-r--   0 root         (0) root         (0)      747 2024-04-09 01:04:39.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/zips/forget.py
--rw-rw-r--   0 root         (0) root         (0)     3227 2024-04-09 01:04:40.000000 vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends_to_mint.py
--rw-rw-r--   0 root         (0) root         (0)      769 2024-04-09 01:04:40.000000 vaccines-1.0.0/modules/structures/vaccines/the.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.637035 vaccines-1.0.0/modules/structures/vaccines/treasuries/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.637035 vaccines-1.0.0/modules/structures/vaccines/treasuries/clique/
--rw-r--r--   0 root         (0) root         (0)      793 2024-04-09 01:04:40.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/clique/__init__.py
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-14 17:52:40.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/close.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-14 17:10:06.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/create.py
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-14 17:10:16.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/destroy.py
--rw-r--r--   0 root         (0) root         (0)     2080 2024-04-09 01:04:40.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/names.py
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-14 17:52:30.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/open.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-11-14 20:01:19.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/path.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-11-14 17:05:43.000000 vaccines-1.0.0/modules/structures/vaccines/treasuries/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:15:16.637035 vaccines-1.0.0/modules/structures/vaccines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-09 01:15:16.000000 vaccines-1.0.0/modules/structures/vaccines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2312 2024-04-09 01:15:16.000000 vaccines-1.0.0/modules/structures/vaccines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 01:15:16.000000 vaccines-1.0.0/modules/structures/vaccines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-09 01:15:16.000000 vaccines-1.0.0/modules/structures/vaccines.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-09 01:15:16.000000 vaccines-1.0.0/modules/structures/vaccines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-09 01:15:16.000000 vaccines-1.0.0/modules/structures/vaccines.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1141 2024-04-09 01:05:37.000000 vaccines-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      712 2024-04-09 01:07:15.000000 vaccines-1.0.0/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 01:15:16.637035 vaccines-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.580313 vaccines-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-09 01:16:20.580313 vaccines-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/structures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/structures/vaccines/
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-09 01:04:32.000000 vaccines-1.0.1/modules/structures/vaccines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/structures/vaccines/_coms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/_coms/clique_pro/
+-rw-rw-r--   0 root         (0) root         (0)      986 2024-04-09 01:04:34.000000 vaccines-1.0.1/modules/structures/vaccines/_coms/clique_pro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/_coms/clique_pro/group/
+-rw-r--r--   0 root         (0) root         (0)     1975 2024-04-09 01:04:35.000000 vaccines-1.0.1/modules/structures/vaccines/_coms/clique_pro/group/trends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/_coms/sanic_pro/
+-rw-rw-r--   0 root         (0) root         (0)       10 2024-04-03 22:13:22.000000 vaccines-1.0.1/modules/structures/vaccines/_coms/sanic_pro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/_status/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-16 20:58:19.000000 vaccines-1.0.1/modules/structures/vaccines/_status/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/structures/vaccines/_status/monitors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/_status/monitors/1_mongo_trends_on/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-09 01:04:35.000000 vaccines-1.0.1/modules/structures/vaccines/_status/monitors/1_mongo_trends_on/monitor_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/structures/vaccines/_status/monitors_process/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/_status/monitors_process/1/
+-rw-r--r--   0 root         (0) root         (0)       96 2024-02-01 19:10:00.000000 vaccines-1.0.1/modules/structures/vaccines/_status/monitors_process/1/monitor_1.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-04-03 21:59:14.000000 vaccines-1.0.1/modules/structures/vaccines/_status/status.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/climate/
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-09 01:04:35.000000 vaccines-1.0.1/modules/structures/vaccines/climate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/climate/mongo/
+-rw-rw-r--   0 root         (0) root         (0)       84 2024-04-03 22:33:06.000000 vaccines-1.0.1/modules/structures/vaccines/climate/mongo/connection_string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/climate/moves/
+-rw-rw-r--   0 root         (0) root         (0)     1354 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/climate/moves/scan_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/config/
+-rw-r--r--   0 root         (0) root         (0)     1354 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/config/scan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/mints/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/mints/clique.py
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/mints/names.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.572313 vaccines-1.0.1/modules/structures/vaccines/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/modules/freight--/
+-rw-rw-r--   0 root         (0) root         (0)     1041 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/modules/freight--/save.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/modules/moves/
+-rw-rw-r--   0 root         (0) root         (0)     1165 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/mint_to_trends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/modules/moves/save/
+-rw-rw-r--   0 root         (0) root         (0)      944 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/save/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/modules/moves/save/modules/
+-rw-rw-r--   0 root         (0) root         (0)     1919 2024-04-09 01:04:37.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/save/modules/zip_and_save_to_gridfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/
+-rw-rw-r--   0 root         (0) root         (0)     1086 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/extract_to_temp.py
+-rw-rw-r--   0 root         (0) root         (0)      374 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/find.py
+-rw-rw-r--   0 root         (0) root         (0)     1147 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/forget.py
+-rw-rw-r--   0 root         (0) root         (0)      410 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/off.py
+-rw-rw-r--   0 root         (0) root         (0)     1929 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/on.py
+-rw-rw-r--   0 root         (0) root         (0)      365 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/show.py
+-rw-rw-r--   0 root         (0) root         (0)      518 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.576313 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/zips/
+-rw-rw-r--   0 root         (0) root         (0)      747 2024-04-09 01:04:39.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/zips/forget.py
+-rw-rw-r--   0 root         (0) root         (0)     3227 2024-04-09 01:04:40.000000 vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends_to_mint.py
+-rw-rw-r--   0 root         (0) root         (0)      769 2024-04-09 01:04:40.000000 vaccines-1.0.1/modules/structures/vaccines/the.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.580313 vaccines-1.0.1/modules/structures/vaccines/treasuries/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.580313 vaccines-1.0.1/modules/structures/vaccines/treasuries/clique/
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-09 01:04:40.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/clique/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       11 2023-11-14 17:52:40.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/close.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-14 17:10:06.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/create.py
+-rw-r--r--   0 root         (0) root         (0)       11 2023-11-14 17:10:16.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/destroy.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-09 01:04:40.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/names.py
+-rw-r--r--   0 root         (0) root         (0)       11 2023-11-14 17:52:30.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/open.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-11-14 20:01:19.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/path.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-11-14 17:05:43.000000 vaccines-1.0.1/modules/structures/vaccines/treasuries/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 01:16:20.580313 vaccines-1.0.1/modules/structures/vaccines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-09 01:16:20.000000 vaccines-1.0.1/modules/structures/vaccines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-09 01:16:20.000000 vaccines-1.0.1/modules/structures/vaccines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 01:16:20.000000 vaccines-1.0.1/modules/structures/vaccines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-09 01:16:20.000000 vaccines-1.0.1/modules/structures/vaccines.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-09 01:16:20.000000 vaccines-1.0.1/modules/structures/vaccines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-09 01:16:20.000000 vaccines-1.0.1/modules/structures/vaccines.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1136 2024-04-09 01:16:10.000000 vaccines-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      712 2024-04-09 01:07:15.000000 vaccines-1.0.1/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 01:16:20.580313 vaccines-1.0.1/setup.cfg
```

### Comparing `vaccines-1.0.0/PKG-INFO` & `vaccines-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vaccines
-Version: 1.0.0
-Summary: How to organize a throne room.
+Version: 1.0.1
+Summary: How to organize remedies.
 Keywords: leads,organization
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: ships
 Requires-Dist: somatic
 Requires-Dist: law_dictionary
 Requires-Dist: deepmerge
```

### Comparing `vaccines-1.0.0/modules/structures/vaccines/__init__.py` & `vaccines-1.0.1/modules/structures/vaccines/__init__.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/_coms/clique_pro/__init__.py` & `vaccines-1.0.1/modules/structures/vaccines/_coms/clique_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/_coms/clique_pro/group/trends.py` & `vaccines-1.0.1/modules/structures/vaccines/_coms/clique_pro/group/trends.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/_status/status.proc.py` & `vaccines-1.0.1/modules/structures/vaccines/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/climate/__init__.py` & `vaccines-1.0.1/modules/structures/vaccines/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/climate/moves/scan_config.py` & `vaccines-1.0.1/modules/structures/vaccines/climate/moves/scan_config.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/config/scan.py` & `vaccines-1.0.1/modules/structures/vaccines/config/scan.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/mints/clique.py` & `vaccines-1.0.1/modules/structures/vaccines/mints/clique.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/mints/names.py` & `vaccines-1.0.1/modules/structures/vaccines/mints/names.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/freight--/save.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/freight--/save.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/mint_to_trends.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/mint_to_trends.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/save/__init__.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/save/__init__.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/save/modules/zip_and_save_to_gridfs.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/save/modules/zip_and_save_to_gridfs.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/extract_to_temp.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/extract_to_temp.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/forget.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/forget.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/on.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/on.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/status.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/status.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends/zips/forget.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends/zips/forget.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/modules/moves/trends_to_mint.py` & `vaccines-1.0.1/modules/structures/vaccines/modules/moves/trends_to_mint.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/the.proc.py` & `vaccines-1.0.1/modules/structures/vaccines/the.proc.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/treasuries/clique/__init__.py` & `vaccines-1.0.1/modules/structures/vaccines/treasuries/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines/treasuries/names.py` & `vaccines-1.0.1/modules/structures/vaccines/treasuries/names.py`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/modules/structures/vaccines.egg-info/PKG-INFO` & `vaccines-1.0.1/modules/structures/vaccines.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vaccines
-Version: 1.0.0
-Summary: How to organize a throne room.
+Version: 1.0.1
+Summary: How to organize remedies.
 Keywords: leads,organization
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: ships
 Requires-Dist: somatic
 Requires-Dist: law_dictionary
 Requires-Dist: deepmerge
```

### Comparing `vaccines-1.0.0/modules/structures/vaccines.egg-info/SOURCES.txt` & `vaccines-1.0.1/modules/structures/vaccines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vaccines-1.0.0/pyproject.toml` & `vaccines-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vaccines"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
 	"volts",
 	"ships",
 	"somatic",
 	"law_dictionary",
 	
 	#
@@ -38,15 +38,15 @@
 	"rich",
 	"tinydb",
 	"click"
 ]
 
 license = { file = "modules/structures/vaccines/license.txt" }
 
-description = "How to organize a throne room."
+description = "How to organize remedies."
 readme = "readme.md"
 keywords = [
 	"leads",
 	"organization"
 ]
 
 [project.scripts]
```

### Comparing `vaccines-1.0.0/readme.md` & `vaccines-1.0.1/readme.md`

 * *Files identical despite different names*

