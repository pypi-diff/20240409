# Comparing `tmp/finhack-0.0.2.dev9.tar.gz` & `tmp/finhack-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finhack-0.0.2.dev9.tar", last modified: Wed Apr  3 02:20:34 2024, max compression
+gzip compressed data, was "finhack-0.0.3.dev1.tar", last modified: Tue Apr  9 06:04:22 2024, max compression
```

## Comparing `finhack-0.0.2.dev9.tar` & `finhack-0.0.3.dev1.tar`

### file list

```diff
@@ -1,331 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/
--rw-r--r--   0 root         (0) root         (0)    73748 2023-12-27 02:20:47.000000 finhack-0.0.2.dev9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-18 10:18:24.000000 finhack-0.0.2.dev9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      159 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3405 2024-04-01 02:06:03.000000 finhack-0.0.2.dev9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-13 11:17:21.000000 finhack-0.0.2.dev9/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/finhack/
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/finhack/collector/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/collector/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:17:00.000000 finhack-0.0.2.dev9/finhack/collector/baseCollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/collector/tushare/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/collector/tushare/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/collector/tushare/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/collector/tushare/__pycache__/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5475 2023-07-18 11:03:58.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockbasic.py
--rwxr-xr-x   0 root         (0) root         (0)    19378 2023-07-18 11:06:31.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockfinance.py
--rwxr-xr-x   0 root         (0) root         (0)    16164 2023-07-18 11:08:47.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockindex.py
--rwxr-xr-x   0 root         (0) root         (0)     2437 2023-07-18 10:59:04.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockmarket.py
--rwxr-xr-x   0 root         (0) root         (0)     7588 2023-07-18 11:15:02.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockother.py
--rwxr-xr-x   0 root         (0) root         (0)     4228 2023-07-18 11:10:21.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockprice.py
--rwxr-xr-x   0 root         (0) root         (0)     4534 2023-07-18 11:14:49.000000 finhack-0.0.2.dev9/finhack/collector/tushare/cb.py
--rwxr-xr-x   0 root         (0) root         (0)     2373 2023-07-18 10:59:25.000000 finhack-0.0.2.dev9/finhack/collector/tushare/econo.py
--rwxr-xr-x   0 root         (0) root         (0)     6335 2023-07-18 11:13:49.000000 finhack-0.0.2.dev9/finhack/collector/tushare/fund.py
--rwxr-xr-x   0 root         (0) root         (0)     1987 2023-07-18 10:59:31.000000 finhack-0.0.2.dev9/finhack/collector/tushare/futures.py
--rwxr-xr-x   0 root         (0) root         (0)      520 2023-07-18 11:12:40.000000 finhack-0.0.2.dev9/finhack/collector/tushare/fx.py
--rwxr-xr-x   0 root         (0) root         (0)    10537 2023-07-18 11:12:33.000000 finhack-0.0.2.dev9/finhack/collector/tushare/helper.py
--rwxr-xr-x   0 root         (0) root         (0)      677 2023-07-18 10:59:39.000000 finhack-0.0.2.dev9/finhack/collector/tushare/hstock.py
--rwxr-xr-x   0 root         (0) root         (0)     1271 2023-07-18 10:59:42.000000 finhack-0.0.2.dev9/finhack/collector/tushare/other.py
--rwxr-xr-x   0 root         (0) root         (0)     7980 2024-01-03 17:45:57.000000 finhack-0.0.2.dev9/finhack/collector/tushare/tushare_collector.py
--rwxr-xr-x   0 root         (0) root         (0)      669 2023-07-18 10:59:45.000000 finhack-0.0.2.dev9/finhack/collector/tushare/ustock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:06:37.000000 finhack-0.0.2.dev9/finhack/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/classes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:05:35.000000 finhack-0.0.2.dev9/finhack/core/classes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/classes/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/classes/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2800 2024-03-20 09:30:47.000000 finhack-0.0.2.dev9/finhack/core/classes/dictobj.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/command/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-30 03:58:55.000000 finhack-0.0.2.dev9/finhack/core/command/finhack
--rw-r--r--   0 root         (0) root         (0)     9001 2024-04-01 11:27:46.000000 finhack-0.0.2.dev9/finhack/core/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/data/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/data/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/loader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:10:41.000000 finhack-0.0.2.dev9/finhack/core/loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/loader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/loader/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-01-31 04:25:19.000000 finhack-0.0.2.dev9/finhack/core/loader/base_loader.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-01-04 11:30:36.000000 finhack-0.0.2.dev9/finhack/core/loader/collector_loader.py
--rw-r--r--   0 root         (0) root         (0)      277 2024-01-04 11:30:49.000000 finhack-0.0.2.dev9/finhack/core/loader/factor_loader.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-01-04 11:32:05.000000 finhack-0.0.2.dev9/finhack/core/loader/helper_loader.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-01-04 11:32:07.000000 finhack-0.0.2.dev9/finhack/core/loader/trader_loader.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:25:21.000000 finhack-0.0.2.dev9/finhack/core/notify.py
--rw-r--r--   0 root         (0) root         (0)      121 2024-01-23 07:25:27.000000 finhack-0.0.2.dev9/finhack/core/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/factor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/factor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/factor/default/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.2.dev9/finhack/factor/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/factor/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/factor/default/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24778 2024-03-19 03:48:09.000000 finhack-0.0.2.dev9/finhack/factor/default/alphaEngine.py
--rw-r--r--   0 root         (0) root         (0)     4955 2024-04-03 01:54:17.000000 finhack-0.0.2.dev9/finhack/factor/default/default_factor.py
--rwxrwxrwx   0 root         (0) root         (0)    18152 2024-03-04 11:36:16.000000 finhack-0.0.2.dev9/finhack/factor/default/factorAnalyzer.py
--rwxrwxrwx   0 root         (0) root         (0)     7888 2024-03-04 10:37:04.000000 finhack-0.0.2.dev9/finhack/factor/default/factorManager.py
--rwxrwxrwx   0 root         (0) root         (0)    13617 2024-04-03 01:56:59.000000 finhack-0.0.2.dev9/finhack/factor/default/factorMining.py
--rwxrwxrwx   0 root         (0) root         (0)     3034 2024-03-04 10:32:09.000000 finhack-0.0.2.dev9/finhack/factor/default/factorPkl.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-07-18 16:57:34.000000 finhack-0.0.2.dev9/finhack/factor/default/factorRepair.py
--rwxrwxrwx   0 root         (0) root         (0)    20166 2024-03-18 10:50:36.000000 finhack-0.0.2.dev9/finhack/factor/default/indicatorCompute.py
--rwxrwxrwx   0 root         (0) root         (0)    18873 2024-03-19 04:08:04.000000 finhack-0.0.2.dev9/finhack/factor/default/preCheck.py
--rwxrwxrwx   0 root         (0) root         (0)     2675 2024-03-19 01:59:28.000000 finhack-0.0.2.dev9/finhack/factor/default/taskRunner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/helper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/helper/struct/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/helper/struct/__init__.py
--rw-r--r--   0 root         (0) root         (0)      192 2023-10-30 10:01:09.000000 finhack-0.0.2.dev9/finhack/helper/struct/struct_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/library/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/library/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/library/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/library/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-04-03 02:00:10.000000 finhack-0.0.2.dev9/finhack/library/ai.py
--rwxrwxrwx   0 root         (0) root         (0)     1437 2024-02-28 08:52:26.000000 finhack-0.0.2.dev9/finhack/library/alert.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-12-28 02:00:35.000000 finhack-0.0.2.dev9/finhack/library/class_loader.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-03-18 12:40:27.000000 finhack-0.0.2.dev9/finhack/library/config.py
--rw-r--r--   0 root         (0) root         (0)     1159 2024-03-27 04:56:20.000000 finhack-0.0.2.dev9/finhack/library/log.py
--rwxrwxrwx   0 root         (0) root         (0)     3254 2023-07-18 11:03:32.000000 finhack-0.0.2.dev9/finhack/library/monitor.py
--rw-r--r--   0 root         (0) root         (0)     2254 2024-02-28 10:19:22.000000 finhack-0.0.2.dev9/finhack/library/mycache.py
--rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-18 03:02:15.000000 finhack-0.0.2.dev9/finhack/library/mydb.py
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-09-18 06:59:38.000000 finhack-0.0.2.dev9/finhack/library/thread.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-12-26 11:12:16.000000 finhack-0.0.2.dev9/finhack/library/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:22:54.000000 finhack-0.0.2.dev9/finhack/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/market/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/astock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 07:33:55.000000 finhack-0.0.2.dev9/finhack/market/astock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/astock/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/market/astock/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1690 2024-01-04 15:33:35.000000 finhack-0.0.2.dev9/finhack/market/astock/astock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/astock/tushare/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 06:44:17.000000 finhack-0.0.2.dev9/finhack/market/astock/tushare/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16872 2024-03-04 10:31:09.000000 finhack-0.0.2.dev9/finhack/market/astock/tushare/astock.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-01 02:44:49.000000 finhack-0.0.2.dev9/finhack/market/astock/tushare/indexHelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/plugin/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/plugin/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-11-02 17:26:48.000000 finhack-0.0.2.dev9/finhack/plugin/default/default_plugin.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-03 02:20:33.000000 finhack-0.0.2.dev9/finhack/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/server/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.2.dev9/finhack/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/server/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.2.dev9/finhack/server/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-04-01 04:43:30.000000 finhack-0.0.2.dev9/finhack/server/default/default_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trader/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trader/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trader/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trader/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2023-12-08 09:41:42.000000 finhack-0.0.2.dev9/finhack/trader/default/calendar.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-03 00:02:23.000000 finhack-0.0.2.dev9/finhack/trader/default/context.py
--rw-r--r--   0 root         (0) root         (0)    17061 2024-03-05 05:58:00.000000 finhack-0.0.2.dev9/finhack/trader/default/data.py
--rw-r--r--   0 root         (0) root         (0)    11661 2024-04-01 11:37:41.000000 finhack-0.0.2.dev9/finhack/trader/default/default_trader.py
--rw-r--r--   0 root         (0) root         (0)     9720 2023-12-23 18:52:29.000000 finhack-0.0.2.dev9/finhack/trader/default/event.py
--rw-r--r--   0 root         (0) root         (0)    18983 2024-04-01 11:41:19.000000 finhack-0.0.2.dev9/finhack/trader/default/function.py
--rw-r--r--   0 root         (0) root         (0)     4930 2024-03-05 06:26:36.000000 finhack-0.0.2.dev9/finhack/trader/default/object.py
--rw-r--r--   0 root         (0) root         (0)     9282 2024-03-20 08:56:55.000000 finhack-0.0.2.dev9/finhack/trader/default/performance.py
--rw-r--r--   0 root         (0) root         (0)     8597 2024-03-26 02:45:51.000000 finhack-0.0.2.dev9/finhack/trader/default/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/auto/__init__.py
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-23 10:56:05.000000 finhack-0.0.2.dev9/finhack/trainer/auto/auto_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/lightgbm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/lightgbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/trainer/lightgbm/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/lightgbm/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13418 2024-03-22 09:36:36.000000 finhack-0.0.2.dev9/finhack/trainer/lightgbm/lightgbm_trainer.py
--rw-r--r--   0 root         (0) root         (0)     4386 2024-03-26 06:58:49.000000 finhack-0.0.2.dev9/finhack/trainer/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 03:52:10.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/.proj
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 02:17:07.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-01 11:40:16.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/choice/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/choice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/index/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/kv/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/kv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/market/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/notice/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:28:17.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/notice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/price/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/price/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 09:02:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-04-03 02:05:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-03 02:05:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/global_var.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 08:25:47.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/ai.conf
--rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/alert.conf
--rw-r--r--   0 root         (0) root         (0)     4433 2024-04-01 11:38:16.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/args.conf
--rw-rw-r--   0 root         (0) root         (0)      156 2024-04-01 06:15:03.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/backtest.conf
--rw-r--r--   0 root         (0) root         (0)      847 2024-03-15 02:02:17.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/constant.conf
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-28 01:09:57.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/core.conf
--rwxrwxrwx   0 root         (0) root         (0)      336 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/db.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13827 2024-03-04 08:10:44.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
--rwxrwxrwx   0 root         (0) root         (0)    22039 2022-12-04 10:31:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3010 2024-04-02 13:15:03.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all
--rw-r--r--   0 root         (0) root         (0)     3443 2023-05-03 18:51:57.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-17 10:39:56.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:23:35.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/global_var.conf
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-09 07:57:06.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/task.conf
--rw-rw-r--   0 root         (0) root         (0)      104 2024-04-01 11:31:20.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/trader.conf
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-24 17:51:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/train.conf
--rwxrwxrwx   0 root         (0) root         (0)      148 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/ts.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/code_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/code_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/date_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/date_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 04:41:32.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 06:44:04.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 10:44:16.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:11:07.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/preds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/preds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 08:48:12.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2227 2024-03-26 09:23:05.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/css/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/images/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/js/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/running/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 04:10:28.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/running/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/
--rw-r--r--   0 root         (0) root         (0)     1195 2022-12-07 19:27:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/QIML365.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8109 2024-01-07 01:31:52.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/extend.py
--rwxrwxrwx   0 root         (0) root         (0)     5827 2024-01-07 01:43:56.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/financial.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-03-20 07:07:21.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/member.py
--rwxrwxrwx   0 root         (0) root         (0)     1948 2024-01-07 01:32:06.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/myfactors.py
--rwxrwxrwx   0 root         (0) root         (0)    21290 2024-01-07 01:32:35.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/ta_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     1954 2024-01-07 01:33:13.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/volumeprice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/
--rw-r--r--   0 root         (0) root         (0)      523 2023-12-28 01:38:27.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      521 2024-01-04 11:32:51.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/testmodule_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:34:57.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:03:25.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/script/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 11:25:50.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/script/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/
--rw-r--r--   0 root         (0) root         (0)     3047 2024-04-01 11:33:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
--rw-r--r--   0 root         (0) root         (0)     3348 2024-01-30 07:19:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-03-12 10:36:21.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10912 2024-03-25 02:37:56.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
--rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 08:45:41.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:17.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 11:19:29.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/calendar.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-12 08:46:32.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/client.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/context.py
--rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/data.py
--rw-r--r--   0 root         (0) root         (0)     2802 2024-03-28 07:35:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py
--rw-r--r--   0 root         (0) root         (0)     6079 2024-04-03 00:53:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/event.py
--rw-r--r--   0 root         (0) root         (0)    11401 2024-04-02 12:03:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/function.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/object.py
--rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-28 01:56:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
--rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
--rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
--rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-02 23:49:54.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
--rw-r--r--   0 root         (0) root         (0)     8747 2024-03-26 02:45:53.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-17 12:29:42.000000 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/constant.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:21:31.000000 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/global_var.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/finhack.egg-info/
--rw-r--r--   0 root         (0) root         (0)      159 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11579 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-03 02:20:20.000000 finhack-0.0.2.dev9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/
+-rw-r--r--   0 root         (0) root         (0)    73748 2023-12-27 02:20:47.000000 finhack-0.0.3.dev1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2024-01-18 10:18:24.000000 finhack-0.0.3.dev1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-04-07 06:51:23.000000 finhack-0.0.3.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/examples/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-13 11:17:21.000000 finhack-0.0.3.dev1/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/collector/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/collector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:17:00.000000 finhack-0.0.3.dev1/finhack/collector/baseCollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/collector/tushare/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/collector/tushare/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/collector/tushare/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/collector/tushare/__pycache__/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5475 2023-07-18 11:03:58.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockbasic.py
+-rwxr-xr-x   0 root         (0) root         (0)    19378 2023-07-18 11:06:31.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockfinance.py
+-rwxr-xr-x   0 root         (0) root         (0)    16164 2023-07-18 11:08:47.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockindex.py
+-rwxr-xr-x   0 root         (0) root         (0)     2437 2023-07-18 10:59:04.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockmarket.py
+-rwxr-xr-x   0 root         (0) root         (0)     7588 2023-07-18 11:15:02.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockother.py
+-rwxr-xr-x   0 root         (0) root         (0)     4228 2023-07-18 11:10:21.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockprice.py
+-rwxr-xr-x   0 root         (0) root         (0)     4534 2023-07-18 11:14:49.000000 finhack-0.0.3.dev1/finhack/collector/tushare/cb.py
+-rwxr-xr-x   0 root         (0) root         (0)     2373 2023-07-18 10:59:25.000000 finhack-0.0.3.dev1/finhack/collector/tushare/econo.py
+-rwxr-xr-x   0 root         (0) root         (0)     6335 2023-07-18 11:13:49.000000 finhack-0.0.3.dev1/finhack/collector/tushare/fund.py
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2023-07-18 10:59:31.000000 finhack-0.0.3.dev1/finhack/collector/tushare/futures.py
+-rwxr-xr-x   0 root         (0) root         (0)      520 2023-07-18 11:12:40.000000 finhack-0.0.3.dev1/finhack/collector/tushare/fx.py
+-rwxr-xr-x   0 root         (0) root         (0)    10537 2023-07-18 11:12:33.000000 finhack-0.0.3.dev1/finhack/collector/tushare/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)      677 2023-07-18 10:59:39.000000 finhack-0.0.3.dev1/finhack/collector/tushare/hstock.py
+-rwxr-xr-x   0 root         (0) root         (0)     1271 2023-07-18 10:59:42.000000 finhack-0.0.3.dev1/finhack/collector/tushare/other.py
+-rwxr-xr-x   0 root         (0) root         (0)     7980 2024-01-03 17:45:57.000000 finhack-0.0.3.dev1/finhack/collector/tushare/tushare_collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      669 2023-07-18 10:59:45.000000 finhack-0.0.3.dev1/finhack/collector/tushare/ustock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:06:37.000000 finhack-0.0.3.dev1/finhack/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/core/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/classes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:05:35.000000 finhack-0.0.3.dev1/finhack/core/classes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/classes/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/classes/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-07 06:44:16.000000 finhack-0.0.3.dev1/finhack/core/classes/dictobj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/command/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-30 03:58:55.000000 finhack-0.0.3.dev1/finhack/core/command/finhack
+-rw-r--r--   0 root         (0) root         (0)     9001 2024-04-01 11:27:46.000000 finhack-0.0.3.dev1/finhack/core/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/data/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/data/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/loader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:10:41.000000 finhack-0.0.3.dev1/finhack/core/loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/loader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/loader/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-01-31 04:25:19.000000 finhack-0.0.3.dev1/finhack/core/loader/base_loader.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-01-04 11:30:36.000000 finhack-0.0.3.dev1/finhack/core/loader/collector_loader.py
+-rw-r--r--   0 root         (0) root         (0)      277 2024-01-04 11:30:49.000000 finhack-0.0.3.dev1/finhack/core/loader/factor_loader.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-01-04 11:32:05.000000 finhack-0.0.3.dev1/finhack/core/loader/helper_loader.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-01-04 11:32:07.000000 finhack-0.0.3.dev1/finhack/core/loader/trader_loader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:25:21.000000 finhack-0.0.3.dev1/finhack/core/notify.py
+-rw-r--r--   0 root         (0) root         (0)      121 2024-01-23 07:25:27.000000 finhack-0.0.3.dev1/finhack/core/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/factor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/factor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/factor/default/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.3.dev1/finhack/factor/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/factor/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/factor/default/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24778 2024-03-19 03:48:09.000000 finhack-0.0.3.dev1/finhack/factor/default/alphaEngine.py
+-rw-r--r--   0 root         (0) root         (0)     4955 2024-04-03 01:54:17.000000 finhack-0.0.3.dev1/finhack/factor/default/default_factor.py
+-rwxrwxrwx   0 root         (0) root         (0)    18152 2024-03-04 11:36:16.000000 finhack-0.0.3.dev1/finhack/factor/default/factorAnalyzer.py
+-rwxrwxrwx   0 root         (0) root         (0)     7888 2024-03-04 10:37:04.000000 finhack-0.0.3.dev1/finhack/factor/default/factorManager.py
+-rwxrwxrwx   0 root         (0) root         (0)    13617 2024-04-03 01:56:59.000000 finhack-0.0.3.dev1/finhack/factor/default/factorMining.py
+-rwxrwxrwx   0 root         (0) root         (0)     3034 2024-03-04 10:32:09.000000 finhack-0.0.3.dev1/finhack/factor/default/factorPkl.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-07-18 16:57:34.000000 finhack-0.0.3.dev1/finhack/factor/default/factorRepair.py
+-rwxrwxrwx   0 root         (0) root         (0)    20166 2024-03-18 10:50:36.000000 finhack-0.0.3.dev1/finhack/factor/default/indicatorCompute.py
+-rwxrwxrwx   0 root         (0) root         (0)    18873 2024-03-19 04:08:04.000000 finhack-0.0.3.dev1/finhack/factor/default/preCheck.py
+-rwxrwxrwx   0 root         (0) root         (0)     2675 2024-03-19 01:59:28.000000 finhack-0.0.3.dev1/finhack/factor/default/taskRunner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/helper/struct/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/helper/struct/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      192 2023-10-30 10:01:09.000000 finhack-0.0.3.dev1/finhack/helper/struct/struct_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/library/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/library/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/library/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/library/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-03 02:00:10.000000 finhack-0.0.3.dev1/finhack/library/ai.py
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2024-02-28 08:52:26.000000 finhack-0.0.3.dev1/finhack/library/alert.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-12-28 02:00:35.000000 finhack-0.0.3.dev1/finhack/library/class_loader.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-03-18 12:40:27.000000 finhack-0.0.3.dev1/finhack/library/config.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-03-27 04:56:20.000000 finhack-0.0.3.dev1/finhack/library/log.py
+-rwxrwxrwx   0 root         (0) root         (0)     3254 2023-07-18 11:03:32.000000 finhack-0.0.3.dev1/finhack/library/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-02-28 10:19:22.000000 finhack-0.0.3.dev1/finhack/library/mycache.py
+-rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-18 03:02:15.000000 finhack-0.0.3.dev1/finhack/library/mydb.py
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-09-18 06:59:38.000000 finhack-0.0.3.dev1/finhack/library/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-12-26 11:12:16.000000 finhack-0.0.3.dev1/finhack/library/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/market/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:22:54.000000 finhack-0.0.3.dev1/finhack/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/market/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/market/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/market/astock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 07:33:55.000000 finhack-0.0.3.dev1/finhack/market/astock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/market/astock/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/market/astock/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1690 2024-01-04 15:33:35.000000 finhack-0.0.3.dev1/finhack/market/astock/astock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/market/astock/tushare/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 06:44:17.000000 finhack-0.0.3.dev1/finhack/market/astock/tushare/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17309 2024-04-08 09:49:34.000000 finhack-0.0.3.dev1/finhack/market/astock/tushare/astock.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-01 02:44:49.000000 finhack-0.0.3.dev1/finhack/market/astock/tushare/indexHelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/plugin/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/plugin/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-11-02 17:26:48.000000 finhack-0.0.3.dev1/finhack/plugin/default/default_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-09 06:04:21.000000 finhack-0.0.3.dev1/finhack/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.3.dev1/finhack/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/server/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.3.dev1/finhack/server/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5545 2024-04-07 17:24:34.000000 finhack-0.0.3.dev1/finhack/server/default/default_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trader/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trader/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trader/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trader/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2023-12-08 09:41:42.000000 finhack-0.0.3.dev1/finhack/trader/default/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-03 00:02:23.000000 finhack-0.0.3.dev1/finhack/trader/default/context.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2024-03-05 05:58:00.000000 finhack-0.0.3.dev1/finhack/trader/default/data.py
+-rw-r--r--   0 root         (0) root         (0)    11700 2024-04-07 08:17:55.000000 finhack-0.0.3.dev1/finhack/trader/default/default_trader.py
+-rw-r--r--   0 root         (0) root         (0)     9720 2023-12-23 18:52:29.000000 finhack-0.0.3.dev1/finhack/trader/default/event.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2024-04-07 06:35:50.000000 finhack-0.0.3.dev1/finhack/trader/default/function.py
+-rw-r--r--   0 root         (0) root         (0)     4930 2024-03-05 06:26:36.000000 finhack-0.0.3.dev1/finhack/trader/default/object.py
+-rw-r--r--   0 root         (0) root         (0)     9397 2024-04-04 16:15:25.000000 finhack-0.0.3.dev1/finhack/trader/default/performance.py
+-rw-r--r--   0 root         (0) root         (0)     8597 2024-03-26 02:45:51.000000 finhack-0.0.3.dev1/finhack/trader/default/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/auto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       32 2024-01-23 10:56:05.000000 finhack-0.0.3.dev1/finhack/trainer/auto/auto_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/lightgbm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/lightgbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/lightgbm/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/lightgbm/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13418 2024-03-22 09:36:36.000000 finhack-0.0.3.dev1/finhack/trainer/lightgbm/lightgbm_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-03-26 06:58:49.000000 finhack-0.0.3.dev1/finhack/trainer/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 03:52:10.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/.proj
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-03 03:37:25.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 03:44:51.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 02:17:07.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2024-04-07 14:16:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/choice/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/choice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/index/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/kv/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/kv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/market/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/notice/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:28:17.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/notice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/price/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/price/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 09:02:59.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      914 2024-04-09 01:00:01.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-09 01:00:01.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/global_var.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 08:25:47.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/ai.conf
+-rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/alert.conf
+-rw-r--r--   0 root         (0) root         (0)     4433 2024-04-04 09:56:10.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/args.conf
+-rw-rw-r--   0 root         (0) root         (0)      283 2024-04-04 09:53:25.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/backtest.conf
+-rw-r--r--   0 root         (0) root         (0)      847 2024-03-15 02:02:17.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/constant.conf
+-rw-r--r--   0 root         (0) root         (0)       18 2023-12-28 01:09:57.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/core.conf
+-rwxrwxrwx   0 root         (0) root         (0)      336 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/db.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13827 2024-03-04 08:10:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
+-rwxrwxrwx   0 root         (0) root         (0)    22039 2022-12-04 10:31:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3010 2024-04-08 10:00:03.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-05-03 18:51:57.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-04-17 10:39:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain
+-rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:23:35.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/global_var.conf
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-09 07:57:06.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/task.conf
+-rw-rw-r--   0 root         (0) root         (0)      106 2024-04-03 03:14:00.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/trader.conf
+-rw-r--r--   0 root         (0) root         (0)       21 2023-12-24 17:51:59.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/train.conf
+-rwxrwxrwx   0 root         (0) root         (0)      148 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/ts.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/code_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/code_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/date_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/date_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 04:41:32.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 06:44:04.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 10:44:16.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:11:07.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/preds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/preds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 08:48:12.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2253 2024-04-07 08:36:40.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/css/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/rqalpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/rqalpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/running/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 04:10:28.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/running/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/
+-rw-r--r--   0 root         (0) root         (0)     1195 2022-12-07 19:27:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/QIML365.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8109 2024-01-07 01:31:52.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/extend.py
+-rwxrwxrwx   0 root         (0) root         (0)     5827 2024-01-07 01:43:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/financial.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-20 07:07:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/member.py
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2024-01-07 01:32:06.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/myfactors.py
+-rwxrwxrwx   0 root         (0) root         (0)    21290 2024-01-07 01:32:35.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/ta_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     1954 2024-01-07 01:33:13.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/volumeprice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-12-28 01:38:27.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      521 2024-01-04 11:32:51.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/testmodule_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:34:57.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:03:25.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/script/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 11:25:50.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/script/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-04-01 11:33:59.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2024-01-30 07:19:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-07 04:58:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2024-03-25 02:37:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
+-rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 08:45:41.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:17.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 11:19:29.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/calendar.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-03-12 08:46:32.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/client.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/context.py
+-rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/data.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-07 06:43:50.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2024-04-08 02:08:50.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/event.py
+-rw-r--r--   0 root         (0) root         (0)    11500 2024-04-08 07:23:29.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/function.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/object.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-04-07 15:23:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
+-rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
+-rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-08 01:58:40.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2024-04-08 07:15:00.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1544 2024-04-07 14:18:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/append_code.py
+-rw-rw-r--   0 root         (0) root         (0)    10542 2024-04-07 14:12:58.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/rqalpha_trader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/context.py
+-rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/data.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-03-28 07:35:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/dictobj.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2024-04-03 00:53:34.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/event.py
+-rw-r--r--   0 root         (0) root         (0)    11401 2024-04-02 12:03:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/function.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/object.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-28 01:56:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmtClient.py
+-rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2.py
+-rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2_grpc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-02 23:49:54.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_trader.py
+-rw-r--r--   0 root         (0) root         (0)     8747 2024-03-26 02:45:53.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-17 12:29:42.000000 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/constant.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:21:31.000000 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/global_var.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12956 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-09 06:04:19.000000 finhack-0.0.3.dev1/setup.py
```

### Comparing `finhack-0.0.2.dev9/LICENSE.txt` & `finhack-0.0.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/README.md` & `finhack-0.0.3.dev1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# FinHack® 炼金术(内测中，文档完善中)
+# FinHack® 炼金术(自测中，5月份开放内测)
 ## 项目介绍
 <div>FinHack®, an easily extensible quantitative finance framework, integrates a complete workflow for quantitative investment research in its current version, including data collection, factor computation, factor mining, factor analysis, machine learning, strategy development, and quantitative backtesting. In later stages, it will expand to include more data sources, trading instruments, analytical tools, and practical plugins, aiming to create an open, customizable, and high-level quantitative finance framework to aid Quants and researchers in related fields with their financial research work.</div>
 <br/>
 FinHack®，一个易于拓展的量化金融框架，它在当前版本中集成了<B>数据采集、因子计算、因子挖掘、因子分析、机器学习、策略编写、量化回测、实盘接入</B>等全流程的量化投研工作，后期它将拓展出更多的数据源、交易品种与分析工具与实用插件，力求打造一个开放的、可定制的、高水平的量化金融框架，助力广大Quant与相关学科工作者的金融研究工作。
 
 ## 项目特点
 - 良好的拓展性，包括但不限于拓展自己的数据源、因子、AI模型、量化策略以及回测规则
@@ -34,7 +34,14 @@
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/74e12eae-93fb-487c-a43f-92c79c8f75d6)
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/19ce463e-9323-4f28-982b-17298c53e1d7)
 
 ## 实盘接入
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/6bafbb9d-0798-4623-bddb-ae5d4f7e2fba)
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/d84e4f1a-d950-49f6-afd9-c3632fe563d0)
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/eacc7656-7161-4a81-8d1a-0a22cf85a76d)
+
+## TODO List
+- 增加更新提醒、公告通知
+- 增加会员注册、数据下载
+- 增加对期货、外汇、美股、比特币的数据、回测、实盘支持
+- 增加多种及其学习算法的支持
+- 策略市场、应用商店
```

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/astockbasic.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/astockbasic.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/astockfinance.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/astockfinance.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/astockindex.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/astockindex.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/astockmarket.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/astockmarket.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/astockother.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/astockother.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/astockprice.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/astockprice.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/cb.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/cb.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/econo.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/econo.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/fund.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/fund.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/futures.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/futures.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/fx.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/fx.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/helper.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/helper.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/hstock.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/hstock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/other.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/other.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/tushare_collector.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/tushare_collector.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/collector/tushare/ustock.py` & `finhack-0.0.3.dev1/finhack/collector/tushare/ustock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/core/classes/dictobj.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/dictobj.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,24 @@
         # 将所有 DictObj 实例转换为普通字典
         state = self._attributes.copy()
         for key, value in state.items():
             if isinstance(value, DictObj):
                 state[key] = value.__getstate__()  # 递归调用以处理嵌套的 DictObj
         return state
 
+
     def __setstate__(self, state):
         # 在反序列化时调用，使用保存的状态重新构建对象
         # 将所有普通字典转换回 DictObj 实例
         for key, value in state.items():
             if isinstance(value, dict):
                 state[key] = DictObj(value)  # 递归调用以处理嵌套的字典
         self._attributes = state
 
+
     def get(self, key, default=None):
         return self._attributes.get(key, default)
         
     def __iter__(self):
         return iter(self._attributes)
         
     def __getitem__(self, key):
```

### Comparing `finhack-0.0.2.dev9/finhack/core/command/finhack` & `finhack-0.0.3.dev1/finhack/core/command/finhack`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/core/core.py` & `finhack-0.0.3.dev1/finhack/core/core.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/core/loader/base_loader.py` & `finhack-0.0.3.dev1/finhack/core/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/alphaEngine.py` & `finhack-0.0.3.dev1/finhack/factor/default/alphaEngine.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/default_factor.py` & `finhack-0.0.3.dev1/finhack/factor/default/default_factor.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/factorAnalyzer.py` & `finhack-0.0.3.dev1/finhack/factor/default/factorAnalyzer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/factorManager.py` & `finhack-0.0.3.dev1/finhack/factor/default/factorManager.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/factorMining.py` & `finhack-0.0.3.dev1/finhack/factor/default/factorMining.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/factorPkl.py` & `finhack-0.0.3.dev1/finhack/factor/default/factorPkl.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/factorRepair.py` & `finhack-0.0.3.dev1/finhack/factor/default/factorRepair.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/indicatorCompute.py` & `finhack-0.0.3.dev1/finhack/factor/default/indicatorCompute.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/preCheck.py` & `finhack-0.0.3.dev1/finhack/factor/default/preCheck.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/factor/default/taskRunner.py` & `finhack-0.0.3.dev1/finhack/factor/default/taskRunner.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/ai.py` & `finhack-0.0.3.dev1/finhack/library/ai.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/alert.py` & `finhack-0.0.3.dev1/finhack/library/alert.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/class_loader.py` & `finhack-0.0.3.dev1/finhack/library/class_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/config.py` & `finhack-0.0.3.dev1/finhack/library/config.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/log.py` & `finhack-0.0.3.dev1/finhack/library/log.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/monitor.py` & `finhack-0.0.3.dev1/finhack/library/monitor.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/mycache.py` & `finhack-0.0.3.dev1/finhack/library/mycache.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/mydb.py` & `finhack-0.0.3.dev1/finhack/library/mydb.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/thread.py` & `finhack-0.0.3.dev1/finhack/library/thread.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/library/utils.py` & `finhack-0.0.3.dev1/finhack/library/utils.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/market/astock/astock.py` & `finhack-0.0.3.dev1/finhack/market/astock/astock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/market/astock/tushare/astock.py` & `finhack-0.0.3.dev1/finhack/market/astock/tushare/astock.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,29 @@
         c1=""
         c2=""
         if not start_date==None:
             c1=" and trade_date>='%s' " % (start_date)
         if not end_date==None:
             c2=" and trade_date<='%s' " % (end_date)
         
-        sql = "select trade_date,close from astock_index_daily where ts_code='%s' %s %s order by trade_date asc" % (ts_code,c1,c2)
+        sql = "select * from astock_index_daily where ts_code='%s' %s %s order by trade_date asc" % (ts_code,c1,c2)
         
         #print(sql)
         
         try:
             df=mydb.selectToDf(sql,'tushare')
+            df["open"]=df["open"].astype(float)
+            df["high"]=df["high"].astype(float)
+            df["low"]=df["low"].astype(float)
+            df["close"]=df["close"].astype(float)
+            df["pre_close"]=df["pre_close"].astype(float)
+            df["change"]=df["change"].astype(float)
+            df["pct_chg"]=df["pct_chg"].astype(float)
+            df["vol"]=df["vol"].astype(float)
+            df['amount']=df['amount'].astype(float)
             return df
         except Exception as e:
             print("MySQL getStockCodeList Error:%s" % str(e))  
             return False   
         return df    
     
     
@@ -104,16 +113,16 @@
 
 
 
         hashstr=','.join(code_list)+'-'+where+'-'+startdate+'-'+enddate+'-'+fq+'-'+db
         md5=hashlib.md5(hashstr.encode(encoding='utf-8')).hexdigest()
         cache_path=PRICE_CACHE_DIR+md5
         if os.path.isfile(cache_path):
-            #print('read cache---'+cache_path)
-            #print(hashstr)
+            print('read cache---'+cache_path)
+            print(hashstr)
             t = time.time()-os.path.getmtime(cache_path)
             if t<60*60*12 and cache: #缓存时间为12小时
                 df=pd.read_pickle(cache_path)
                 return df
 
 
         with ProcessPoolExecutor(max_workers=5) as pool:
```

### Comparing `finhack-0.0.2.dev9/finhack/market/astock/tushare/indexHelper.py` & `finhack-0.0.3.dev1/finhack/market/astock/tushare/indexHelper.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/calendar.py` & `finhack-0.0.3.dev1/finhack/trader/default/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/context.py` & `finhack-0.0.3.dev1/finhack/trader/default/context.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/data.py` & `finhack-0.0.3.dev1/finhack/trader/default/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/default_trader.py` & `finhack-0.0.3.dev1/finhack/trader/default/default_trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         result = mydb.selectToDf(sql, 'finhack')
 
         if not result.empty:
             # 从查询结果中提取数据并还原到 context 变量中
             row = result.iloc[0]
 
             # 还原 trade 相关的字段
+            context.id=id
             context.trade.model_id = row['model']
             context.params= row['params']
             context.trade.strategy = row['strategy']
             context.trade.start_time = row['start_date']
             context.trade.end_time = row['end_date']
             context.trade.benchmark = row['benchmark']
             context.trade.strategy_code = row['strategy_code']
@@ -73,15 +74,15 @@
             
             calendar=Calendar.get_calendar(context.trade.start_time,context.trade.end_time,market='astock')
 
 
             calendar=pd.to_datetime(calendar)
             calendar=calendar[0:len(context.performance.returns)]
 
-
+            
             context.performance.returns = pd.DataFrame(context.performance.returns, index=calendar)
             context.performance.bench_returns = pd.DataFrame(context.performance.bench_returns, index=calendar)
             return context
         else:
             return False
 
 
@@ -189,15 +190,15 @@
         
         #这里后面放到redis里，这样就可以模拟和实盘了
         # print(context)
         # print(context.portfolio)
         
         while context.data.event_list:
             event = context.data.event_list.pop(0)
-            print(event['event_time'],event['event_name'],event['event_type'])
+            #print(event['event_time'],event['event_name'],event['event_type'])
             event_time=datetime.strptime(event['event_time'], '%Y-%m-%d %H:%M:%S')
                 # 如果 event_time 大于当前时间，退出循环
             if event_time > datetime.now():
                 break
             if context.previous_date==None or context.current_dt==None:
                 pass
             elif context.current_dt.date() != event_time.date():
```

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/event.py` & `finhack-0.0.3.dev1/finhack/trader/default/event.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/function.py` & `finhack-0.0.3.dev1/finhack/trader/default/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,17 @@
     context_json = str(args)+str(context['trade'])+str(context['account'])+str(context['portfolio']['cash'])
     hash_value = hashlib.md5(context_json.encode()).hexdigest()
     if args['id']!='':
         context.id=args['id']
     else:
         context.id=hash_value
 
-
+    # print(context_json)
+    # print(hash_value)
+    # exit()
 
 def set_benchmark(code):
     context['trade']['benchmark']=code
     
 def set_option(key,value):
     if key in context['trade']:
         context['trade'][key]=value
```

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/object.py` & `finhack-0.0.3.dev1/finhack/trader/default/object.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/performance.py` & `finhack-0.0.3.dev1/finhack/trader/default/performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,26 @@
         context.performance.returns=context.performance.returns.set_index('trade_date')
         
         benchmark=context.trade.benchmark
         start_date=context.trade.start_time[0:10].replace('-','')
         end_date=context.trade.end_time[0:10].replace('-','')
         
         index=AStock.getIndexPrice(ts_code=benchmark,start_date=start_date,end_date=end_date)
-        index['returns']=index['close']/index['close'].shift(1)
+        #index['returns']=index['close']/index['close'].shift(1)
+        index['returns']=index['pct_chg']/100
         index['values']=index['returns'].cumprod()
         index["trade_date"] = pd.to_datetime(index["trade_date"], format='%Y%m%d')
         index=index.set_index('trade_date')         
         
 
         returns=context.performance.returns['returns']-1
         
         
         
-        benchReturns=index['returns']-1
-        benchReturns.iloc[0] = 0
-        
+        benchReturns=index['returns']
         
         try:
             alpha, beta = ey.alpha_beta(returns = returns, factor_returns = benchReturns, annualization=252) 
         except Exception as e:
             print(str(e))
         indicators = {}
         indicators["alpha"] = alpha
@@ -126,23 +125,23 @@
         i_df=context.performance.bench_returns+1
         
         try:
             p_dates = p_df.index.strftime('%d/%m/%Y').tolist()
         except Exception as e:
             p_dates = p_df
             
-        p_values = (p_df.values.cumprod()).tolist()
+        p_values = (p_df.values.cumprod()-1).tolist()
         
         try:
             i_dates = i_df.index.strftime('%d/%m/%Y').tolist()
         except Exception as e:
             i_dates = i_df.index.strftime('%d/%m/%Y').tolist()
             
  
-        i_values = (i_df.values.cumprod()).tolist()
+        i_values = (i_df.values.cumprod()-1).tolist()
         
         # 绘图
         # 设置图表样式
         plt.plotsize(100, 30)
         plt.canvas_color("default")  # 设置透明背景
         plt.ticks_color("default")  # 设置刻度颜色以匹配终端默认颜色
         plt.axes_color("default") 
@@ -154,35 +153,33 @@
         plt.ylabel("Return")
         plt.grid(True)
         plt.show()   
 
     def save_chart(context):
         p_df=context.performance.returns+1
         i_df=context.performance.bench_returns+1
-        
+        e_df=(p_df-i_df)+1
         try:
             p_dates = p_df.index.strftime('%d/%m/%Y').tolist()
         except Exception as e:
             p_dates = p_df
-            
-        p_values = (p_df.values.cumprod()).tolist()
-        
+        p_values = (p_df.values.cumprod()-1).tolist()
         try:
             i_dates = i_df.index.strftime('%d/%m/%Y').tolist()
         except Exception as e:
             i_dates = i_df.index.strftime('%d/%m/%Y').tolist()
-            
- 
-        i_values = (i_df.values.cumprod()).tolist()
+        i_values = (i_df.values.cumprod()-1).tolist()
+        e_values = (e_df.values.cumprod()-1).tolist()
         
 
         # 绘图
         mplt.figure(figsize=(4, 2))  # 设置图像大小
         mplt.plot(p_dates, p_values, color='red', label=context['trade']['strategy'])
         mplt.plot(i_dates, i_values, color='blue', label=context.trade.benchmark)
+        mplt.plot(i_dates, e_values, color='orange', label="excess")
         # mplt.xlabel("Date")
         # mplt.ylabel("Cumulative Return")
         # 不显示图例
         # plt.legend()  # 这行代码已经被注释掉，不会再显示图例
         # 设置背景为白色
         ax = mplt.gca()  # 获取当前的Axes对象ax
         ax.set_facecolor('white')  # 设置ax的背景颜色为白色
```

### Comparing `finhack-0.0.2.dev9/finhack/trader/default/rules.py` & `finhack-0.0.3.dev1/finhack/trader/default/rules.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trainer/lightgbm/lightgbm_trainer.py` & `finhack-0.0.3.dev1/finhack/trainer/lightgbm/lightgbm_trainer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/trainer/trainer.py` & `finhack-0.0.3.dev1/finhack/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import itertools
 import json
 import psutil
 import time
 import glob
 import gc
 import sys
+import re
+from finhack.core.classes.dictobj import DictObj
 
 class DefaultBacktest():
     def __init__(self):
         pass
 
 
     def del_model_if_idle():
@@ -48,21 +50,49 @@
                     # 将时间差转换为分钟
                     time_diff_minutes = time_diff / 60
                     if time_diff_minutes > 30:
                         #print(f"文件 {pred_data_path} 最后修改时间超过30分钟。")
                         os.remove(pred_data_path)
 
     def run_command_with_semaphore(self, cmd, semaphore):
-        DefaultBacktest.del_model_if_idle()
+        try:
+            DefaultBacktest.del_model_if_idle()
+        except Exception as e:
+            print(f'An error occurred: {e}')
+            
         with semaphore:
             try:
                 os.system(cmd)
             except Exception as e:
                 print(f'An error occurred: {e}')
 
+
+    def rqalpha(self):
+
+        if hasattr(sys, 'frozen'):  # 特别检查，如果是使用 PyInstaller 等工具打包的可执行文件
+            entry_file_path = os.path.realpath(sys.executable)
+        else:
+            entry_file_path = os.path.realpath(sys.argv[0])
+
+        bt_list=mydb.selectToList(f"SELECT id, instance_id, features_list, train, model, strategy, start_date, end_date, init_cash, params, total_value, alpha, beta, annual_return, cagr, annual_volatility, info_ratio, downside_risk, R2, sharpe, sortino, calmar, omega, max_down, SQN, created_at, filter, win, server, trade_num, runtime, starttime, endtime,  roto, simulate, benchmark, strategy_code FROM `finhack`.`backtest`  order by sharpe desc LIMIT 1000",'finhack')   
+        
+        def to_json(s):
+            dict_str = re.sub(r"DictObj\((.*?)\)", r"{\1}", s)
+            dict_str = re.sub(r"(\w+)=('[^']*'|\"[^\"]*\")", r'"\1": \2', dict_str)
+            dict_str = dict_str.replace("'", '"')
+            return dict_str
+        semaphore = multiprocessing.Semaphore(3) 
+        processes = []
+        for bt in bt_list:
+            cmd=f"{entry_file_path} trader run --strategy={bt['strategy']} --log_level=ERROR --id={bt['instance_id']} --model_id={bt['model']} --cash={int(bt['init_cash'])}   --project_path={BASE_DIR}  --params='{to_json(bt['params'])}' --replace=True --vendor=rqalpha"
+            p = multiprocessing.Process(target=self.run_command_with_semaphore, args=(cmd, semaphore))
+            processes.append(p)
+            p.start()
+           
+
     def run(self):
         # 获取入口文件的完整路径
         if hasattr(sys, 'frozen'):  # 特别检查，如果是使用 PyInstaller 等工具打包的可执行文件
             entry_file_path = os.path.realpath(sys.executable)
         else:
             entry_file_path = os.path.realpath(sys.argv[0])
 
@@ -94,15 +124,14 @@
             pt = multiprocessing.Process(target=load_preds_data, args=(model_hash, True, 'lightgbm', cfgTrade['start_time'], cfgTrade['end_time']))
             # 启动进程
             pt.start()
             # 等待进程完成
             pt.join()           
             # preds=load_preds_data(model_id=model_hash, cache=True,trainer='lightgbm',start_time=cfgTrade['start_time'],end_time=cfgTrade['end_time'])
             # del preds
-
             # gc.collect()
             #continue
             processes = []
             for cash in cash_list:
                 for strategy_name in strategy_list:
                     s_params={}
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/constant.conf`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-FRAMEWORK_DIR="/root/anaconda3/envs/finhack/lib/python3.9/site-packages/finhack"
-BASE_DIR="/data/code/finhack/examples/demo-project"
+FRAMEWORK_DIR={FRAMEWORK_DIR}
+BASE_DIR={BASE_DIR}
 DATA_DIR=BASE_DIR+"/data/"
 CACHE_DIR=DATA_DIR+"cache/"
 REPORTS_DIR=DATA_DIR+"reports/"
 CONFIG_DIR=DATA_DIR+"config/"
 MODELS_DIR=DATA_DIR+"models/"
 PREDS_DIR=DATA_DIR+"preds/"
 LOGS_DIR=DATA_DIR+"logs/"
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/args.conf` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/args.conf`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 min_f=16
 max_f=64
 process=1
 
 
 
 [backtest]
-strategy=IndexPlus2
-cash=5000000
-process=12
+strategy=testStrategy
+cash=20000
+process=28
 
 
 [trader]
 id=
 strategy=DemoStrategy
 market=astock
 start_time=2021-01-01 00:00:00
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/constant.conf` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-FRAMEWORK_DIR={FRAMEWORK_DIR}
-BASE_DIR={BASE_DIR}
+FRAMEWORK_DIR="/root/anaconda3/envs/finhack/lib/python3.9/site-packages/finhack"
+BASE_DIR="/data/code/demo_project/"
 DATA_DIR=BASE_DIR+"/data/"
 CACHE_DIR=DATA_DIR+"cache/"
 REPORTS_DIR=DATA_DIR+"reports/"
 CONFIG_DIR=DATA_DIR+"config/"
 MODELS_DIR=DATA_DIR+"models/"
 PREDS_DIR=DATA_DIR+"preds/"
 LOGS_DIR=DATA_DIR+"logs/"
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/index.html` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <title>Finhack回测概览</title>
-    <script src="https://code.jquery.com/jquery-3.5.1.js"></script>
-    <script src="https://cdn.datatables.net/1.10.21/js/jquery.dataTables.min.js"></script>
-    <link rel="stylesheet" href="https://cdn.datatables.net/1.10.21/css/jquery.dataTables.min.css">
+    <script src="/static/js/jquery-3.5.1.js"></script>
+    <script src="/static/js/jquery.dataTables-1.10.21.min.js"></script>
+    <link rel="stylesheet" href="/static/css/jquery.dataTables.min.css">
     <script>
         $(document).ready(function() {
             $('#instanceTable').DataTable({"pageLength": 100});
         });
     </script>
     <style>
         td{
@@ -21,41 +21,42 @@
     <table id="instanceTable" class="display">
         <thead>
             <tr>
                 <th>回测ID</th>
                 <th>模型id</th>
                 <th>策略名称</th>
                 <th>初始资金</th>
-                <th>alpha</th>
-                <th>夏普</th>
-                <th>索提诺</th>
+                <th>夏普1</th>
+                <th>夏普2</th>
+                <!--<th>索提诺</th>-->
                 <th>年化</th>
                 <th>预览</th>
                 <th>最大回撤</th>
                 <th>交易次数</th>
                 <th>胜率</th>
                 <th>详情</th>
                 
             </tr>
         </thead>
         <tbody>
             {% for item in data %}
             <tr>
-                <td width="10%"><a href="/static/trader/bt_{{ item.instance_id }}.html" target="_blank">{{ item.instance_id }}</td>
-                <td>{{item.model}}</td>
+                <td width="10%"><a href="/static/trader/bt_{{ item.instance_id }}.html" target="_blank">{{ item.instance_id[0:16] }}...</td>
+                <td>{{item.model[:16]}}...</td>
                 <td>{{item.strategy}}</td>
                 <td>{{ item.init_cash  }}</td>
-                <td>{{ item.alpha  | round(2)}}</td>
+                <!-- <td>{{ item.alpha  | round(2)}}</td> -->
+                <td>{{ item.sharpe2 | round(2)}}</td>
                 <td>{{ item.sharpe | round(2)}}</td>
-                <td>{{ item.sortino | round(2)}}</td>
+                <!--<td>{{ item.sortino | round(2)}}</td>-->
                 <td>{{  (item.annual_return * 100)  | round(2) }}%</td>
                 <td width="10%"><img src="/static/images/bt_{{ item.instance_id }}.png"  width="150" /></td>
                 <td>{{ (item.max_down * 100)  | round(2) }}%</td>
                 <td>{{ item.trade_num }}</td>
                 <td>{{ (item.win/item.trade_num*100) | round(2)}}%</td>
-                <td width="10%"><a href="/detail?id={{ item.instance_id }}" target="_blank">详情</td>
+                <td><a href="/detail?id={{ item.instance_id }}" target="_blank">详情</td>
             </tr>
             {% endfor %}
         </tbody>
     </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-?回?测IIDD             ?模?型iidd          ?策?略?名?称             ?初?始?资?金           aallpphhaa      ?夏?普          ?索?提?诺          ?年?化                  ?预?览               ?最?大?回?撤           ?交?易?次?数           ?胜?率                  ?详?情
-_{                                               {              {          {           {            {{                  [/static/images/ {{             {
-_{                {             {                {              {          {           {            (item.annual_return bt_{             (item.max_down {              {{ (item.win/
-_i_t_e_m_._i_n_s_t_a_n_c_e___i_d {item.model}} {item.strategy}} item.init_cash item.alpha item.sharpe item.sortino * 100) | round(2)   {                * 100) | round item.trade_num item.trade_num*100) _详_情
-_}_}                                              }}             | round    | round     | round(2)}} }}%                 item.instance_id (2) }}%        }}             | round(2)}}%
-                                                               (2)}}      (2)}}                                        }}.png]
+?回?测IIDD             ?模?型iidd        ?策?略?名?称             ?初?始?资?金           ?夏?普11          ?夏?普22         ?年?化                  ?预?览               ?最?大?回?撤           ?交?易?次?数           ?胜?率                  ?详?情
+_{                                             {              {            {           {{                  [/static/images/ {{             {
+_{                {           {                {              {            {           (item.annual_return bt_{             (item.max_down {              {{ (item.win/
+_i_t_e_m_._i_n_s_t_a_n_c_e___i_d {item.model {item.strategy}} item.init_cash item.sharpe2 item.sharpe * 100) | round(2)   {                * 100) | round item.trade_num item.trade_num*100) _详_情
+_[_0_:_1_6_]_ _}_}_._._.     [:16]}}...                   }}             | round(2)}} | round     }}%                 item.instance_id (2) }}%        }}             | round(2)}}%
+                                                                          (2)}}                           }}.png]
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/QIML365.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/QIML365.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/extend.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/extend.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/financial.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/financial.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/myfactors.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/myfactors.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/ta_lib.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/ta_lib.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/volumeprice.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/volumeprice.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/testmodule_loader.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/testmodule_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,53 +12,52 @@
     # 设定沪深300作为基准
     set_benchmark('000001.SH')
     # True为开启动态复权模式，使用真实价格交易
     set_option('use_real_price', True) 
     # 设定成交量比例
     set_option('order_volume_ratio', 1)
     # # 股票类交易手续费是：买入时佣金万分之三，卖出时佣金万分之三加千分之一印花税, 每笔交易佣金最低扣5块钱
-    set_order_cost(OrderCost(open_tax=0, close_tax=0.001, \
-                             open_commission=0.0003, close_commission=0.0003,\
-                             close_today_commission=0, min_commission=5), type='stock')
+    set_order_cost(OrderCost(open_tax=0, close_tax=0.001, open_commission=0.0003, close_commission=0.0003,close_today_commission=0, min_commission=5), type='stock')
     
     # 为股票设定滑点为百分比滑点                       
     set_slippage(PriceRelatedSlippage(0.00246),type='stock')
     # 持仓数量
-    g.stocknum = 10
+    context.g.stocknum = 10
     # 交易日计时器
-    g.days = 0 
+    context.g.days = 0 
     # 调仓频率
-    g.refresh_rate = 3
+    context.g.refresh_rate = 3
     # 运行函数
     inout_cash(100000)
 
     run_daily(trade, time="09:30")
     # run_daily(trade, time="8:05")
     log.info('get code list')
-    g.stock_list=AStock.getStockCodeList(strict=False)
+    context.g.stock_list=AStock.getStockCodeList(strict=False)
+    
 
 ## 交易函数
 def trade(context):
-    if g.days%g.refresh_rate == 0:
+    if context.g.days%context.g.refresh_rate == 0:
         #print(context.portfolio.cash)
         sell_list = list(context.portfolio.positions.keys()) 
         if len(sell_list) > 0 :
             for stock in sell_list:
                 order_target_value(stock, 0)  
     
-        if len(context.portfolio.positions) < g.stocknum :
-            Num = g.stocknum - len(context.portfolio.positions)
+        if len(context.portfolio.positions) < context.g.stocknum:
+            Num = context.g.stocknum - len(context.portfolio.positions)
             Cash = context.portfolio.cash/Num
         else: 
             Cash = 0
     
         ## 选股
-        stock_list = random.sample(g.stock_list['ts_code'].tolist(), 10)
+        stock_list = random.sample(context.g.stock_list['ts_code'].tolist(), 10)
         ## 买入股票
         for stock in stock_list:
-            if len(context.portfolio.positions.keys()) < g.stocknum:
+            if len(context.portfolio.positions.keys()) < context.g.stocknum:
                 order_value(stock, Cash)
 
         # 天计数加一
-        g.days = 1
+        context.g.days = 1
     else:
-        g.days += 1
+        context.g.days += 1
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/calendar.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/context.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/context.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/data.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py` & `finhack-0.0.3.dev1/finhack/core/classes/dictobj.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 class DictObj:
     def __init__(self, attr=None):
         if attr is None:
             attr = {}
         # 确保所有字典都被封装为 DictObj
         for key, value in attr.items():
             if isinstance(value, dict):
@@ -14,24 +15,22 @@
         # 将所有 DictObj 实例转换为普通字典
         state = self._attributes.copy()
         for key, value in state.items():
             if isinstance(value, DictObj):
                 state[key] = value.__getstate__()  # 递归调用以处理嵌套的 DictObj
         return state
 
-
     def __setstate__(self, state):
         # 在反序列化时调用，使用保存的状态重新构建对象
         # 将所有普通字典转换回 DictObj 实例
         for key, value in state.items():
             if isinstance(value, dict):
                 state[key] = DictObj(value)  # 递归调用以处理嵌套的字典
         self._attributes = state
 
-
     def get(self, key, default=None):
         return self._attributes.get(key, default)
         
     def __iter__(self):
         return iter(self._attributes)
         
     def __getitem__(self, key):
@@ -80,8 +79,12 @@
         
     def push(self, key, value):
         """添加或更新字典中的键值对。"""
         self[key] = value
 
     def pop(self, key, default=None):
         """从字典中移除指定的键并返回其值，如果键不存在，则返回default。"""
-        return self._attributes.pop(key, default)
+        return self._attributes.pop(key, default)
+
+    def to_json(self):
+        """将对象转换为JSON字符串。"""
+        return json.dumps(self.__getstate__(), ensure_ascii=False)
```

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/event.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/event.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/function.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/function.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/object.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/object.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/rules.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/rules.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack/widgets/templates/runtime/constant.py` & `finhack-0.0.3.dev1/finhack/widgets/templates/runtime/constant.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev9/finhack.egg-info/SOURCES.txt` & `finhack-0.0.3.dev1/finhack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 finhack/trainer/lightgbm/__init__.py
 finhack/trainer/lightgbm/lightgbm_trainer.py
 finhack/trainer/lightgbm/__pycache__/__init__.py
 finhack/widgets/__init__.py
 finhack/widgets/templates/__init__.py
 finhack/widgets/templates/empty_project/.proj
 finhack/widgets/templates/empty_project/__init__.py
+finhack/widgets/templates/empty_project/auto/__init__.py
+finhack/widgets/templates/empty_project/auto/default/__init__.py
 finhack/widgets/templates/empty_project/backtest/__init__.py
 finhack/widgets/templates/empty_project/backtest/default/__init__.py
 finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
 finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
 finhack/widgets/templates/empty_project/data/__init__.py
 finhack/widgets/templates/empty_project/data/cache/__init__.py
 finhack/widgets/templates/empty_project/data/cache/runtime.py
@@ -173,14 +175,15 @@
 finhack/widgets/templates/empty_project/data/preds/__init__.py
 finhack/widgets/templates/empty_project/data/reports/__init__.py
 finhack/widgets/templates/empty_project/data/reports/index.html
 finhack/widgets/templates/empty_project/data/reports/static/__init__.py
 finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
 finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
 finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
+finhack/widgets/templates/empty_project/data/reports/static/rqalpha/__init__.py
 finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
 finhack/widgets/templates/empty_project/data/running/__init__.py
 finhack/widgets/templates/empty_project/indicators/QIML365.py
 finhack/widgets/templates/empty_project/indicators/__init__.py
 finhack/widgets/templates/empty_project/indicators/extend.py
 finhack/widgets/templates/empty_project/indicators/financial.py
 finhack/widgets/templates/empty_project/indicators/member.py
@@ -218,10 +221,28 @@
 finhack/widgets/templates/empty_project/trader/qmt/object.py
 finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
 finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
 finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
 finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
 finhack/widgets/templates/empty_project/trader/qmt/rules.py
 finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
+finhack/widgets/templates/empty_project/trader/rqalpha/__init__.py
+finhack/widgets/templates/empty_project/trader/rqalpha/append_code.py
+finhack/widgets/templates/empty_project/trader/rqalpha/rqalpha_trader.py
+finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/__init__.py
+finhack/widgets/templates/empty_project/trader/sim/__init__.py
+finhack/widgets/templates/empty_project/trader/sim/calendar.py
+finhack/widgets/templates/empty_project/trader/sim/context.py
+finhack/widgets/templates/empty_project/trader/sim/data.py
+finhack/widgets/templates/empty_project/trader/sim/dictobj.py
+finhack/widgets/templates/empty_project/trader/sim/event.py
+finhack/widgets/templates/empty_project/trader/sim/function.py
+finhack/widgets/templates/empty_project/trader/sim/object.py
+finhack/widgets/templates/empty_project/trader/sim/qmtClient.py
+finhack/widgets/templates/empty_project/trader/sim/qmt_pb2.py
+finhack/widgets/templates/empty_project/trader/sim/qmt_pb2_grpc.py
+finhack/widgets/templates/empty_project/trader/sim/qmt_trader.py
+finhack/widgets/templates/empty_project/trader/sim/rules.py
+finhack/widgets/templates/empty_project/trader/sim/__pycache__/__init__.py
 finhack/widgets/templates/runtime/__init__.py
 finhack/widgets/templates/runtime/constant.py
 finhack/widgets/templates/runtime/global_var.py
```

### Comparing `finhack-0.0.2.dev9/setup.py` & `finhack-0.0.3.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os 
 
 root_dir = 'finhack'
-version='0.0.2.dev9'
+version='0.0.3.dev1'
 
 for subdir, dirs, files in os.walk(root_dir):
     if not '__init__.py' in files:
         init_file_path = os.path.join(subdir, '__init__.py')
         open(init_file_path, 'a').close()
         print(f'Created __init__.py in {subdir}')
```

