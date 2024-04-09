# Comparing `tmp/stock-open-api-1.0.5.tar.gz` & `tmp/stock-open-api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-1.0.5.tar", last modified: Sun Apr  7 10:01:39 2024, max compression
+gzip compressed data, was "dist/stock-open-api-1.0.6.tar", last modified: Tue Apr  9 05:57:51 2024, max compression
```

## Comparing `stock-open-api-1.0.5.tar` & `stock-open-api-1.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3181 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/bse/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/bse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/ipo3/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/ipo3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/ipo3/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26956 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/ipo3/neeq_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/jqka/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/jqka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/jqka/company.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/sse/sh_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/api/szse/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/szse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/api/szse/sz_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/convert_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/excel_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/iterator_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/table_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-07 10:01:32.000000 stock-open-api-1.0.5/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:01:39.000000 stock-open-api-1.0.5/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3181 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/bse/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/bse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/ipo3/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/ipo3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/ipo3/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27082 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/ipo3/neeq_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/jqka/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/jqka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/jqka/company.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/sse/sh_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/api/szse/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/szse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/api/szse/sz_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/convert_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/excel_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/table_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 05:57:39.000000 stock-open-api-1.0.6/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:57:51.000000 stock-open-api-1.0.6/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-1.0.5/PKG-INFO` & `stock-open-api-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-1.0.5/README.md` & `stock-open-api-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/setup.py` & `stock-open-api-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/company.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/company.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/company_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/sh_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/sz_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-1.0.6/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/ipo3/config.py` & `stock-open-api-1.0.6/stock_open_api/api/ipo3/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,16 @@
     "股东权益合计": "total_equity",
     "负债和股东权益合计": "total_liabilities_and_shareholder_equity",
     "公告日期": "publish_date"
 }
 
 # 现金流量表
 CASH_FLOWS_STATEMENT_KEY_MAP = {
-    "现金流量表": "2022年报",
-    "报告期": "2022-12-31",
+    "现金流量表": "cash_flows_statement",
+    "报告期": "report_date",
     "销售商品、提供劳务收到的现金": "2.68亿",
     "收到的税费返还": "733.11万",
     "收到其他与经营活动有关的现金": "1,085.65万",
     "经营活动现金流入小计": "2.86亿",
     "购买商品、接受劳务支付的现金": "1.65亿",
     "支付给职工以及为职工支付的现金": "5,186.84万",
     "支付的各项税费": "564.16万",
@@ -202,15 +202,15 @@
     "递延所得税资产减少": "-11.12万",
     "存货的减少": "-442.89万",
     "经营性应收项目的减少": "-695.99万",
     "经营性应付项目的增加": "863.24万",
     "其他": "",
     "现金的期末余额": "5,231.27万",
     "减:现金的期初余额": "5,092.93万",
-    "公告日期": "2022-12-31"
+    "公告日期": "publish_date"
 }
 
 # 财务分析表
 FINANCIAL_ANALYSIS_KEY_MAP = {
     "财务分析": "2022年报",
     "报告期": "2022-12-31",
     "每股收益-基本(元)": "0.56",
```

### Comparing `stock-open-api-1.0.5/stock_open_api/api/ipo3/neeq_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/ipo3/neeq_stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,20 +248,20 @@
             item[key.strip()] = value.strip()
 
         lst.append(item)
 
     return lst
 
 
-def get_income_statement_list(stock_code, date_type='年报', english_key=False):
+def get_income_statement_list(stock_code, date_type='年报', english_key=False, proxies=None, timeout=5):
     """
-    获取利润表
+    犀牛之心-财报摘要-利润表
     eg: https://www.ipo3.com/company-show/stock_code-430510-tab-finance-date_type-001.html#content
     :param stock_code: str 股票代码
-    :param date_type: str 可选值：年报/中报/一季报/三季报
+    :param date_type: str 可选值：['年报', '中报', '一季报', '三季报']
     :param english_key: bool
     :return:
     [
       {
         "利润表": "2022年报",
         "报告期": "2022-12-31",
         "营业总收入": "2.52亿",
@@ -296,15 +296,18 @@
         '中报': 'https://www.ipo3.com/company-show/stock_code-{stock_code}-tab-finance-date_type-002.html#content',
         '一季报': 'https://www.ipo3.com/company-show/stock_code-{stock_code}-tab-finance-date_type-003.html#content',
         '三季报': 'https://www.ipo3.com/company-show/stock_code-{stock_code}-tab-finance-date_type-004.html#content'
     }
 
     # eg: https://www.ipo3.com/company-show/stock_code-430510-tab-finance-date_type-001.html#content
     url = date_type_map[date_type].format(stock_code=stock_code)
-    res = request_util.get(url)
+
+    logger.info("url: %s", url)
+
+    res = request_util.get(url, proxies=proxies, timeout=timeout)
     sel = Selector(text=res.text)
 
     items = parse_finance_table(sel)
 
     if english_key:
         items = [convert_util.convert_key(config.INCOME_STATEMENT_KEY_MAP, item) for item in items]
```

### Comparing `stock-open-api-1.0.5/stock_open_api/api/jqka/company.py` & `stock-open-api-1.0.6/stock_open_api/api/jqka/company.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-1.0.6/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/api/szse/sz_stock.py` & `stock-open-api-1.0.6/stock_open_api/api/szse/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/utils/convert_util.py` & `stock-open-api-1.0.6/stock_open_api/utils/convert_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/utils/excel_util.py` & `stock-open-api-1.0.6/stock_open_api/utils/excel_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/utils/request_util.py` & `stock-open-api-1.0.6/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api/utils/table_util.py` & `stock-open-api-1.0.6/stock_open_api/utils/table_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.5/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-1.0.6/stock_open_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-1.0.5/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-1.0.6/stock_open_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

