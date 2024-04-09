# Comparing `tmp/countess-0.0.57.tar.gz` & `tmp/countess-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.57.tar", last modified: Thu Apr  4 09:44:33 2024, max compression
+gzip compressed data, was "countess-0.0.58.tar", last modified: Tue Apr  9 05:48:04 2024, max compression
```

## Comparing `countess-0.0.57.tar` & `countess-0.0.58.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.57/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.57/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-04 09:44:33.957883 countess-0.0.57/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-04 09:42:41.000000 countess-0.0.57/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.949883 countess-0.0.57/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-04 09:42:41.000000 countess-0.0.57/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.949883 countess-0.0.57/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.57/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.57/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-03 00:27:43.000000 countess-0.0.57/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.57/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19161 2024-04-03 00:27:43.000000 countess-0.0.57/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-03 05:16:18.000000 countess-0.0.57/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-03 05:16:18.000000 countess-0.0.57/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.953883 countess-0.0.57/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.57/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18458 2024-04-03 05:18:33.000000 countess-0.0.57/countess/gui/config.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.953883 countess-0.0.57/countess/gui/icons/
--rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/add.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/check.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/del.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/hbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/info.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/redbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/sort_dn.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/sort_un.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/sort_up.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/uncheck.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/vbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20088 2024-04-04 09:42:21.000000 countess-0.0.57/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/mini_browser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15188 2024-04-03 00:42:47.000000 countess-0.0.57/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-03 01:42:58.000000 countess-0.0.57/countess/gui/tree.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3565 2024-04-03 05:15:43.000000 countess-0.0.57/countess/gui/widgets.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.57/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/collate.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/column.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/correlation.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-03 23:13:30.000000 countess-0.0.57/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-03 00:27:43.000000 countess-0.0.57/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/hgvs_parser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.57/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3660 2024-04-03 23:55:53.000000 countess-0.0.57/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.57/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.57/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.57/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.57/countess/utils/pandas.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.57/countess/utils/parallel.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18145 2024-04-04 01:40:39.000000 countess-0.0.57/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/countess.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-03 00:27:43.000000 countess-0.0.57/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-04 09:44:33.957883 countess-0.0.57/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.57/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-03 00:27:43.000000 countess-0.0.57/tests/test_cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-03 00:27:43.000000 countess-0.0.57/tests/test_gui.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.57/tests/test_plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.58/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.58/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-09 05:48:04.286211 countess-0.0.58/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-09 05:47:38.000000 countess-0.0.58/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.278211 countess-0.0.58/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-09 05:47:38.000000 countess-0.0.58/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.282211 countess-0.0.58/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.58/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.58/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-05 06:49:16.000000 countess-0.0.58/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.58/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19404 2024-04-09 05:40:26.000000 countess-0.0.58/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-09 05:44:13.000000 countess-0.0.58/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-09 05:44:13.000000 countess-0.0.58/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.282211 countess-0.0.58/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.58/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18505 2024-04-09 05:44:13.000000 countess-0.0.58/countess/gui/config.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.282211 countess-0.0.58/countess/gui/icons/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/add.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/check.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20442 2024-04-09 05:41:27.000000 countess-0.0.58/countess/gui/icons/countess.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/del.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/hbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/info.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/redbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/sort_dn.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/sort_un.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/sort_up.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/icons/uncheck.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/icons/vbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-04-03 00:27:43.000000 countess-0.0.58/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20633 2024-04-09 05:44:13.000000 countess-0.0.58/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/mini_browser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15188 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-05 06:49:16.000000 countess-0.0.58/countess/gui/tree.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3565 2024-04-05 05:13:40.000000 countess-0.0.58/countess/gui/widgets.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.58/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/collate.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/column.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/correlation.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-05 05:13:40.000000 countess-0.0.58/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/hgvs_parser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.58/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3854 2024-04-08 01:06:06.000000 countess-0.0.58/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.58/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3524 2024-04-09 05:44:13.000000 countess-0.0.58/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.58/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.58/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.58/countess/utils/pandas.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.58/countess/utils/parallel.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18172 2024-04-09 05:40:45.000000 countess-0.0.58/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/countess.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1651 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-09 05:48:04.000000 countess-0.0.58/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-05 06:49:16.000000 countess-0.0.58/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-09 05:48:04.286211 countess-0.0.58/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.58/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-09 05:48:04.286211 countess-0.0.58/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-05 05:13:41.000000 countess-0.0.58/tests/test_cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-05 05:13:41.000000 countess-0.0.58/tests/test_gui.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.58/tests/test_plugins.py
```

### Comparing `countess-0.0.57/LICENSE.txt` & `countess-0.0.58/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/PKG-INFO` & `countess-0.0.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.57
+Version: 0.0.58
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.57
+# CountESS 0.0.58
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.57/README.md` & `countess-0.0.58/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.57
+# CountESS 0.0.58
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.57/countess/core/config.py` & `countess-0.0.58/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/core/logger.py` & `countess-0.0.58/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/core/parameters.py` & `countess-0.0.58/countess/core/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,32 +411,25 @@
         self.set_choices([self.PREFIX + c for c in choices])
 
     def get_column_name(self):
         if self.value.startswith(self.PREFIX):
             return self.value[len(self.PREFIX) :]
         return None
 
-    def get_column(self, df):
+    def get_value(self, data: dict):
         if self.value.startswith(self.PREFIX):
-            col = self.value[len(self.PREFIX) :]
-            return _dataframe_get_column(df, col)
+            return data[self.value[len(self.PREFIX) :]]
         else:
-            return None
+            return self.value
 
-
-class ColumnOrIntegerParam(ColumnOrStringParam):
-    def clean_value(self, value):
-        if isinstance(value, str):
-            return int("".join(re.split(r"\D+", value)))
-        else:
-            return int(value)
-
-
-class MultipleChoiceParam(ChoiceParam):
-    pass
+    def set_choices(self, choices: Iterable[str]):
+        self.choices = list(choices)
+        if self._value is not None and self._value.startswith(self.PREFIX) and self._value not in self.choices:
+            self._value = self.DEFAULT_VALUE
+            self._choice = None
 
 
 class ArrayParam(BaseParam):
     """An ArrayParam contains zero or more copies of `param`, which can be a
     SimpleParam or a MultiParam."""
 
     # XXX the only real use for this is as an array of MultiParams so I think
@@ -537,14 +530,17 @@
     def set_column_choices(self, choices):
         self.param.set_column_choices(choices)
         for p in self.params:
             p.set_column_choices(choices)
 
 
 class PerColumnArrayParam(ArrayParam):
+    """An ArrayParam where each value in the array corresponds to a column
+    in the input dataframe, as set by set_column_choices."""
+
     def __init__(self, *a, **k) -> None:
         super().__init__(*a, **k)
         self.read_only = True
 
     def get_parameters(self, key, base_dir="."):
         for n, p in enumerate(self.params):
             yield f"{key}.{n}._label", p.label
@@ -655,8 +651,9 @@
 
     def set_column_choices(self, choices):
         for p in self.params.values():
             p.set_column_choices(choices)
 
 
 class TabularMultiParam(MultiParam):
-    pass
+    """This is just used to drop a hint to the GUI as to how the MultiParam
+    is to be presented ... as a hierarchy or as a table ..."""
```

### Comparing `countess-0.0.57/countess/core/pipeline.py` & `countess-0.0.58/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/core/plugins.py` & `countess-0.0.58/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/gui/config.py` & `countess-0.0.58/countess/gui/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
                     else tk.NORMAL
                 )
         elif isinstance(self.parameter, MultiParam):
             self.update_subwrappers(self.parameter.params.values(), None)
         elif isinstance(self.parameter, ChoiceParam):
             choices = self.parameter.choices or [""]
             self.entry["values"] = choices
+            self.var.set(self.parameter.value)
         elif isinstance(self.parameter, BooleanParam):
             self.set_checkbox_value()
         elif isinstance(self.parameter, TextParam):
             if self.parameter.read_only:
                 self.entry["state"] = "normal"
             self.entry.replace("1.0", tk.END, self.parameter.value)
             if self.parameter.read_only:
```

### Comparing `countess-0.0.57/countess/gui/logger.py` & `countess-0.0.58/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/gui/main.py` & `countess-0.0.58/countess/gui/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from countess.core.pipeline import PipelineGraph
 from countess.core.plugins import get_plugin_classes
 from countess.gui.config import PluginConfigurator
 from countess.gui.logger import LoggerFrame
 from countess.gui.mini_browser import MiniBrowserFrame
 from countess.gui.tabular import TabularDataFrame
 from countess.gui.tree import FlippyCanvas, GraphWrapper
-from countess.gui.widgets import ask_open_filename, ask_saveas_filename, info_button
+from countess.gui.widgets import ask_open_filename, ask_saveas_filename, get_icon, info_button
 from countess.utils.pandas import concat_dataframes
 
 # import faulthandler
 # faulthandler.enable(all_threads=True)
 
 
 plugin_classes = sorted(get_plugin_classes(), key=lambda x: x.name)
@@ -488,14 +488,30 @@
             self.subframe.place(x=x, y=0, w=event.width - x, h=event.height)
         else:
             y = event.height // 4
             self.canvas.place(x=0, y=0, w=event.width, h=y)
             self.subframe.place(x=0, y=y, w=event.width, h=event.height - y)
 
 
+class SplashScreen:
+    def __init__(self, tk_root):
+        bg = "skyblue"
+        self.splash = tk.Toplevel(tk_root, bg=bg)
+        self.splash.attributes("-type", "dialog")
+
+        font = ("TkHeadingFont", 16, "bold")
+        tk.Label(self.splash, text=f"CountESS {VERSION}", font=font, bg=bg).grid(padx=10, pady=10)
+        tk.Label(self.splash, image=get_icon(tk_root, "countess"), bg=bg).grid(padx=10)
+
+        self.splash.after(3500, self.destroy)
+
+    def destroy(self):
+        self.splash.destroy()
+
+
 def make_root():
     try:
         import ttkthemes  # pylint: disable=C0415
 
         root = ttkthemes.ThemedTk()
         themes = set(root.get_themes())
         for t in ["clam", "aqua", "winnative"]:
@@ -519,14 +535,15 @@
         pass
 
     return root
 
 
 def main():
     root = make_root()
+    SplashScreen(root)
     MainWindow(root, sys.argv[1] if len(sys.argv) > 1 else None)
 
     root.mainloop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `countess-0.0.57/countess/gui/mini_browser.py` & `countess-0.0.58/countess/gui/mini_browser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/gui/tabular.py` & `countess-0.0.58/countess/gui/tabular.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/gui/tree.py` & `countess-0.0.58/countess/gui/tree.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/gui/widgets.py` & `countess-0.0.58/countess/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/collate.py` & `countess-0.0.58/countess/plugins/collate.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/column.py` & `countess-0.0.58/countess/plugins/column.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/correlation.py` & `countess-0.0.58/countess/plugins/correlation.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/csv.py` & `countess-0.0.58/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/data_table.py` & `countess-0.0.58/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/expression.py` & `countess-0.0.58/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/fastq.py` & `countess-0.0.58/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/group_by.py` & `countess-0.0.58/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/hgvs_parser.py` & `countess-0.0.58/countess/plugins/hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/join.py` & `countess-0.0.58/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/mutagenize.py` & `countess-0.0.58/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/pivot.py` & `countess-0.0.58/countess/plugins/pivot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 from typing import Dict, List, Optional
 
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_numeric_dtype
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import ChoiceParam, PerColumnArrayParam
 from countess.core.plugins import PandasProcessPlugin
 from countess.utils.pandas import get_all_columns
 
@@ -55,14 +56,18 @@
         if not expand_cols:
             logger.warning("No columns to expand!")
 
         if not pivot_cols:
             logger.error("No columns to pivot on!")
             return []
 
+        for ec in expand_cols:
+            if not is_numeric_dtype(data[ec]):
+                logger.warning(f"Expanding non-numeric column {ec}")
+
         n_pivot = _product(data[pc].nunique() for pc in pivot_cols) * len(expand_cols)
         if n_pivot > 200:
             pivot_cols_str = ", ".join(pivot_cols)
             logger.error(f"Too many pivot combinations on {pivot_cols_str} ({n_pivot})")
             return []
 
         df = pd.pivot_table(
```

### Comparing `countess-0.0.57/countess/plugins/python.py` & `countess-0.0.58/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/regex.py` & `countess-0.0.58/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/sequence.py` & `countess-0.0.58/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/plugins/variant.py` & `countess-0.0.58/countess/plugins/variant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 from typing import Optional
 
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
-from countess.core.parameters import BooleanParam, ColumnChoiceParam, ColumnOrNoneChoiceParam, IntegerParam, StringParam
+from countess.core.parameters import BooleanParam, ColumnChoiceParam, ColumnOrStringParam, IntegerParam, StringParam
 from countess.core.plugins import PandasTransformDictToDictPlugin
 from countess.utils.variant import find_variant_string
 
 
 class VariantPlugin(PandasTransformDictToDictPlugin):
     """Turns a DNA sequence into a HGVS variant code"""
 
     name = "Variant Translator"
     description = "Turns a DNA sequence into a HGVS variant code"
     version = VERSION
     link = "https://countess-project.github.io/CountESS/included-plugins/#variant-caller"
 
     parameters = {
         "column": ColumnChoiceParam("Input Column", "sequence"),
-        "reference": ColumnOrNoneChoiceParam("Reference Column"),
-        "sequence": StringParam("*OR* Reference Sequence"),
+        "reference": ColumnOrStringParam("Reference Sequence"),
         "output": StringParam("Output Column", "variant"),
         "max_mutations": IntegerParam("Max Mutations", 10),
         "protein": StringParam("Protein Column", ""),
         "offset": IntegerParam("Protein Offset", 0),
         "max_protein": IntegerParam("Max Protein Variations", 10),
         "drop": BooleanParam("Drop unidentified variants", False),
         "drop_columns": BooleanParam("Drop Input Column(s)", False),
     }
 
     def process_dict(self, data, logger: Logger) -> dict:
-        assert isinstance(self.parameters["reference"], ColumnOrNoneChoiceParam)
+        assert isinstance(self.parameters["reference"], ColumnOrStringParam)
         sequence = data[self.parameters["column"].value]
         if not sequence:
             return {}
 
-        if self.parameters["reference"].is_none():
-            reference = self.parameters["sequence"].value
-        else:
-            reference = data[self.parameters["reference"].value]
+        reference = self.parameters["reference"].get_value(data)
 
         r = {}
 
         if self.parameters["output"].value:
             try:
                 max_mutations = self.parameters["max_mutations"].value
                 r[self.parameters["output"].value] = find_variant_string("g.", reference, sequence, max_mutations, 0)
@@ -63,25 +59,25 @@
                 pass
             except (TypeError, KeyError, IndexError) as exc:
                 logger.exception(exc)
 
         return r
 
     def process_dataframe(self, dataframe: pd.DataFrame, logger: Logger) -> Optional[pd.DataFrame]:
-        assert isinstance(self.parameters["reference"], ColumnOrNoneChoiceParam)
+        assert isinstance(self.parameters["reference"], ColumnOrStringParam)
         df_out = super().process_dataframe(dataframe, logger)
 
         if df_out is not None:
             if self.parameters["drop"].value:
                 if self.parameters["output"].value:
                     df_out.dropna(subset=self.parameters["output"].value, inplace=True)
                 if self.parameters["protein"].value:
                     df_out.dropna(subset=self.parameters["protein"].value, inplace=True)
             if self.parameters["drop_columns"].value:
                 try:
                     df_out.drop(columns=self.parameters["column"].value, inplace=True)
-                    if self.parameters["reference"].is_not_none():
-                        df_out.drop(columns=self.parameters["reference"].value, inplace=True)
+                    if self.parameters["reference"].get_column_name():
+                        df_out.drop(columns=self.parameters["reference"].get_column_name(), inplace=True)
                 except KeyError:
                     pass
 
         return df_out
```

### Comparing `countess-0.0.57/countess/utils/pandas.py` & `countess-0.0.58/countess/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/utils/parallel.py` & `countess-0.0.58/countess/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/countess/utils/variant.py` & `countess-0.0.58/countess/utils/variant.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
     for opcode in opcodes:
         src_start, src_end = opcode.src_start, opcode.src_end
         src_pro = ref_pro[src_start:src_end]
         dest_pro = var_pro[opcode.dest_start : opcode.dest_end]
 
         if opcode.tag == "delete":
             assert dest_pro == ""
-            if ref_pro[src_end] == '*':
+            if len(ref_pro) > src_end and ref_pro[src_end] == "*":
                 # if the codon just after this deletion is a terminator,
                 # consider this an early termination.
                 yield f"{_ref(src_start)}Ter"
                 return
             if len(src_pro) == 1:
                 yield f"{_ref(src_start)}del"
             else:
```

### Comparing `countess-0.0.57/countess.egg-info/PKG-INFO` & `countess-0.0.58/countess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.57
+Version: 0.0.58
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.57
+# CountESS 0.0.58
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.57/countess.egg-info/SOURCES.txt` & `countess-0.0.58/countess.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 countess/gui/main.py
 countess/gui/mini_browser.py
 countess/gui/tabular.py
 countess/gui/tree.py
 countess/gui/widgets.py
 countess/gui/icons/add.gif
 countess/gui/icons/check.gif
+countess/gui/icons/countess.gif
 countess/gui/icons/del.gif
 countess/gui/icons/hbar.gif
 countess/gui/icons/info.gif
 countess/gui/icons/redbar.gif
 countess/gui/icons/sort_dn.gif
 countess/gui/icons/sort_un.gif
 countess/gui/icons/sort_up.gif
```

### Comparing `countess-0.0.57/countess.egg-info/entry_points.txt` & `countess-0.0.58/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/pyproject.toml` & `countess-0.0.58/pyproject.toml`

 * *Files identical despite different names*

### Comparing `countess-0.0.57/tests/test_plugins.py` & `countess-0.0.58/tests/test_plugins.py`

 * *Files identical despite different names*

