# Comparing `tmp/CodersWheel-0.2.0.tar.gz` & `tmp/CodersWheel-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodersWheel-0.2.0.tar", last modified: Sun Mar 17 09:42:47 2024, max compression
+gzip compressed data, was "CodersWheel-0.2.1.tar", last modified: Tue Apr  9 08:27:15 2024, max compression
```

## Comparing `CodersWheel-0.2.0.tar` & `CodersWheel-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.504011 CodersWheel-0.2.0/CodersWheel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.508011 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.508011 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/MysqlConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/Redisconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/asnyc_mysql_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.508011 CodersWheel-0.2.0/CodersWheel/Core/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/Core/Combine.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/Core/Core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.512011 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/AboutDB.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/AboutDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/AboutSqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/CacheFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/DataFeatureScaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Luhn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/MysqlConnector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5237 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Needleman_Wunsch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/SeriesComparing.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/OtherToolWheel/coroutine_prev_active_decor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.512011 CodersWheel-0.2.0/CodersWheel/QuickTool/
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/MySQLConn_v004_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/MySQLConn_v005_node.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/boost_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/ch2pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17173 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/ch2pandas_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/check_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/detect_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/excel_format_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/generate_str_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/lazy_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/process_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/retry_it.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/task_test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/tasks_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/QuickTool/typeassert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/CodersWheel/ServiceWheel/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ServiceWheel/CoroutineBoostup.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ServiceWheel/Service.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/ServiceWheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/CodersWheel/api/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/api/API.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/api/Wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/CodersWheel/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/CodersWheel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-17 09:42:47.000000 CodersWheel-0.2.0/CodersWheel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-17 09:42:47.000000 CodersWheel-0.2.0/CodersWheel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 09:42:47.000000 CodersWheel-0.2.0/CodersWheel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 09:42:47.000000 CodersWheel-0.2.0/CodersWheel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-17 09:42:47.000000 CodersWheel-0.2.0/CodersWheel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:47.516011 CodersWheel-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:42:33.000000 CodersWheel-0.2.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.438546 CodersWheel-0.2.1/CodersWheel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.438546 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.438546 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/MysqlConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/Redisconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/asnyc_mysql_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.438546 CodersWheel-0.2.1/CodersWheel/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/Core/Combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/Core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.442546 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/AboutDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/AboutDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/AboutSqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/CacheFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/DataFeatureScaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Luhn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/MysqlConnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5237 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Needleman_Wunsch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/SeriesComparing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/OtherToolWheel/coroutine_prev_active_decor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/CodersWheel/QuickTool/
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/MySQLConn_v004_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/MySQLConn_v005_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/boost_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/ch2pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17173 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/ch2pandas_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/check_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/detect_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/excel_format_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/generate_str_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/lazy_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/process_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/retry_it.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/task_test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/tasks_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/QuickTool/typeassert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/CodersWheel/ServiceWheel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ServiceWheel/CoroutineBoostup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ServiceWheel/Service.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/ServiceWheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/CodersWheel/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/api/API.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/api/Wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/CodersWheel/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/CodersWheel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-09 08:27:15.000000 CodersWheel-0.2.1/CodersWheel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-09 08:27:15.000000 CodersWheel-0.2.1/CodersWheel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:27:15.000000 CodersWheel-0.2.1/CodersWheel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:27:15.000000 CodersWheel-0.2.1/CodersWheel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 08:27:15.000000 CodersWheel-0.2.1/CodersWheel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:27:15.450545 CodersWheel-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:15.446545 CodersWheel-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:27:07.000000 CodersWheel-0.2.1/test/__init__.py
```

### Comparing `CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/MysqlConnector.py` & `CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/MysqlConnector.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/Redisconnector.py` & `CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/Redisconnector.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/ConnectorWheel/db_core/asnyc_mysql_connector.py` & `CodersWheel-0.2.1/CodersWheel/ConnectorWheel/db_core/asnyc_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/Core/Combine.py` & `CodersWheel-0.2.1/CodersWheel/Core/Combine.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/AboutDB.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/AboutDB.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/AboutDate.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/AboutDate.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/AboutSqlite.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/AboutSqlite.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/CacheFunctions.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/CacheFunctions.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/DataFeatureScaling.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/DataFeatureScaling.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Luhn.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Luhn.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/MysqlConnector.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/MysqlConnector.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Needleman_Wunsch.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Scheduler.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Scheduler.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/SeriesComparing.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/SeriesComparing.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Tools.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Tools.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/Wrappers.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/Wrappers.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/OtherToolWheel/coroutine_prev_active_decor.py` & `CodersWheel-0.2.1/CodersWheel/OtherToolWheel/coroutine_prev_active_decor.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/MySQLConn_v004_node.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/MySQLConn_v004_node.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/MySQLConn_v005_node.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/MySQLConn_v005_node.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/ch2pandas.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/ch2pandas.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/ch2pandas_node.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/ch2pandas_node.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/check_file_type.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/check_file_type.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/detect_file_path.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/detect_file_path.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/excel_format_parser.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/excel_format_parser.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/file_cache.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/file_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding=utf-8
+from collections import OrderedDict
+
 import datetime
 import hashlib
 import os
 import pickle
-from collections import OrderedDict
 from functools import wraps
 
 __refresh__ = False
 DEFAULT = './'
 format_dict = {'Y': '%Y', 'm': "%Y-%m", 'd': "%Y-%m-%d",
                'H': '%Y-%m-%d %H', 'M': '%Y-%m-%d %H:%M', 'S': '%Y-%m-%d %H:%M:%S'}
 
@@ -56,22 +57,21 @@
     if cls_obj and arg_cls_name is not None and arg_cls_name == cls_name:
         arg_tuple = tuple([cls_name] + list(map(str, arg[1:])))
     else:
         arg_tuple = arg
 
     key = pickle.dumps([func_name, arg_tuple, kwargs, dt_str])  # get the unique key for the same input
     if exploit_func_name:
-        name = f"{func_name}_{hashlib.sha1(key).hexdigest()}_{dt_str}"  # create cache file name
+        name = f"{func_name}_{hashlib.sha1(key).hexdigest()}_{dt_str}.cache"  # create cache file name
     else:
-        name = hashlib.sha1(key).hexdigest()  # create cache file name
+        name = hashlib.sha1(key).hexdigest() + '.cache'  # create cache file name
     file_path = get_cache_path(enable_cache=enable_cache)
     return file_path, name
 
 
-
 def write(fg, res):
     with open(fg, 'wb') as f:
         pickle.dump(res, f)
 
 
 def read(fg):
     with open(fg, 'rb') as f:
@@ -109,14 +109,15 @@
 def file_cache(**deco_arg_dict):
     def _deco(func):
         @wraps(func)
         def __deco(*args, **kwargs):
             return _cache(func, args, kwargs, **deco_arg_dict)
 
         return __deco
+
     return _deco
 
 
 if __name__ == '__main__':
     @file_cache(enable_cache=True)
     def test(a, b=2):
         return a, b
```

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/generate_str_node.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/generate_str_node.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/importer.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/importer.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/lazy_load.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/lazy_load.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/logger.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/logger.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/process_bar.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/process_bar.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/retry_it.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/retry_it.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/singleton.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/singleton.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/task_test_all.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/task_test_all.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/tasks_register.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/tasks_register.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/QuickTool/typeassert.py` & `CodersWheel-0.2.1/CodersWheel/QuickTool/typeassert.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/ServiceWheel/CoroutineBoostup.py` & `CodersWheel-0.2.1/CodersWheel/ServiceWheel/CoroutineBoostup.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel/api/API.py` & `CodersWheel-0.2.1/CodersWheel/api/API.py`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/CodersWheel.egg-info/PKG-INFO` & `CodersWheel-0.2.1/CodersWheel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodersWheel
-Version: 0.2.0
+Version: 0.2.1
 Summary: CodersWheel - CW
 Home-page: https://github.com/sn0wfree
 Author: s & n & 0 & w & f & r & e & e
 Author-email: snowfreedom0815@gmail.com
 License: MIT
 License-File: LICENSE
```

### Comparing `CodersWheel-0.2.0/CodersWheel.egg-info/SOURCES.txt` & `CodersWheel-0.2.1/CodersWheel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/LICENSE` & `CodersWheel-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/PKG-INFO` & `CodersWheel-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodersWheel
-Version: 0.2.0
+Version: 0.2.1
 Summary: CodersWheel - CW
 Home-page: https://github.com/sn0wfree
 Author: s & n & 0 & w & f & r & e & e
 Author-email: snowfreedom0815@gmail.com
 License: MIT
 License-File: LICENSE
```

### Comparing `CodersWheel-0.2.0/README.md` & `CodersWheel-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `CodersWheel-0.2.0/setup.py` & `CodersWheel-0.2.1/setup.py`

 * *Files identical despite different names*

