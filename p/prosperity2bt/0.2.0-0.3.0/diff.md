# Comparing `tmp/prosperity2bt-0.2.0.tar.gz` & `tmp/prosperity2bt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.2.0.tar", last modified: Mon Apr  8 09:08:11 2024, max compression
+gzip compressed data, was "prosperity2bt-0.3.0.tar", last modified: Mon Apr  8 16:35:52 2024, max compression
```

## Comparing `prosperity2bt-0.2.0.tar` & `prosperity2bt-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.932957 prosperity2bt-0.2.0/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.932957 prosperity2bt-0.2.0/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.932957 prosperity2bt-0.2.0/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-08 09:08:05.000000 prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 09:08:11.000000 prosperity2bt-0.2.0/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 09:08:09.000000 prosperity2bt-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:08:11.940956 prosperity2bt-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:52.644639 prosperity2bt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 16:35:52.644639 prosperity2bt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:52.636638 prosperity2bt-0.3.0/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:52.636638 prosperity2bt-0.3.0/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:52.640639 prosperity2bt-0.3.0/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:52.644639 prosperity2bt-0.3.0/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-08 16:35:43.000000 prosperity2bt-0.3.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:35:52.644639 prosperity2bt-0.3.0/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-08 16:35:52.000000 prosperity2bt-0.3.0/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 16:35:52.000000 prosperity2bt-0.3.0/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:35:52.000000 prosperity2bt-0.3.0/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 16:35:52.000000 prosperity2bt-0.3.0/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 16:35:52.000000 prosperity2bt-0.3.0/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 16:35:52.000000 prosperity2bt-0.3.0/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 16:35:49.000000 prosperity2bt-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:35:52.644639 prosperity2bt-0.3.0/setup.cfg
```

### Comparing `prosperity2bt-0.2.0/LICENSE` & `prosperity2bt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/PKG-INFO` & `prosperity2bt-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipython
 Requires-Dist: jsonpickle
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
@@ -84,14 +85,18 @@
 
 # Write algorithm output to custom file
 $ prosperity2bt example/starter.py 1 --out example.log
 
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
+
+# Print trader's output to stdout while running
+# This may be helpful when debugging a broken trader
+$ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
```

### Comparing `prosperity2bt-0.2.0/README.md` & `prosperity2bt-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 
 # Write algorithm output to custom file
 $ prosperity2bt example/starter.py 1 --out example.log
 
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
+
+# Print trader's output to stdout while running
+# This may be helpful when debugging a broken trader
+$ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
```

### Comparing `prosperity2bt-0.2.0/prosperity2bt/core.py` & `prosperity2bt-0.3.0/prosperity2bt/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import defaultdict
-from contextlib import redirect_stdout
+from contextlib import closing, redirect_stdout
 from dataclasses import dataclass
 from io import StringIO
+from IPython.utils.io import Tee
 from prosperity2bt.data import DayData, LIMITS, PriceRow
 from prosperity2bt.datamodel import Observation, Order, OrderDepth, Symbol, Trade, TradingState
 from typing import Any
 
 @dataclass
 class ActivityLogRow:
     columns: list[Any]
@@ -188,15 +189,15 @@
         if row.timestamp != last_timestamp:
             break
 
         total_profit += row.columns[-1]
 
     print(f"Total profit: {total_profit:,.0f}\n")
 
-def run_backtest(trader: Any, data: DayData) -> DayResult:
+def run_backtest(trader: Any, data: DayData, print_output: bool) -> DayResult:
     print(f"Backtesting {trader.__module__} on round {data.round} day {data.day}")
 
     result = DayResult(data.round, data.day, [], [], [])
     trader_data = ""
 
     prices_by_timestamp = defaultdict(dict)
     for row in data.prices:
@@ -243,16 +244,22 @@
             dict(own_trades),
             dict(market_trades),
             position,
             observations,
         )
 
         stdout = StringIO()
-        with redirect_stdout(stdout):
-            orders_by_symbol, conversions, trader_data = trader.run(state)
+        stdout.close = lambda: None
+
+        if print_output:
+            with closing(Tee(stdout)):
+                orders_by_symbol, conversions, trader_data = trader.run(state)
+        else:
+            with redirect_stdout(stdout):
+                orders_by_symbol, conversions, trader_data = trader.run(state)
 
         for product in tradable_products:
             price = prices_by_timestamp[timestamp][product]
 
             profit_loss = profit_loss_by_product[product]
             if own_positions[product] != 0:
                 profit_loss += own_positions[product] * price.mid_price
```

### Comparing `prosperity2bt-0.2.0/prosperity2bt/data.py` & `prosperity2bt-0.3.0/prosperity2bt/data.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/datamodel.py` & `prosperity2bt-0.3.0/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/main.py` & `prosperity2bt-0.3.0/prosperity2bt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,23 +143,24 @@
     parser = ArgumentParser(prog="prosperity2bt", description="Run a backtest.")
     parser.add_argument("algorithm", type=str, help="path to the Python file containing the algoritm to backtest")
     parser.add_argument("days", type=str, nargs="+", help="the days to backtest on (<round>-<day> for a single day, <round> for all days in a round)")
     parser.add_argument("--merge-pnl", action="store_true", help="merge profit and loss across days")
     parser.add_argument("--vis", action="store_true", help="open backtest result in visualizer when done")
     parser.add_argument("--out", type=str, help="path to save output log to (defaults to backtests/<timestamp>.log)")
     parser.add_argument("--data", type=str, help="path to data directory (must look similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources)")
+    parser.add_argument("--print", action="store_true", help="print the trader's output to stdout while it's running")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
     Trader = parse_algorithm(args.algorithm)
     days = parse_days(args.days, args.data)
     output_file = parse_out(args.out)
 
-    results = [run_backtest(Trader(), day) for day in days]
+    results = [run_backtest(Trader(), day, args.print) for day in days]
     merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl), results)
 
     write_output(output_file, merged_results)
 
     if len(days) > 1:
         print_overall_summary(results)
```

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.3.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.3.0/prosperity2bt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.2.0
+Version: 0.3.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipython
 Requires-Dist: jsonpickle
 
 # IMC Prosperity 2 Backtester
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-backtester/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-backtester/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2bt)](https://pypi.org/project/prosperity2bt/)
 
@@ -84,14 +85,18 @@
 
 # Write algorithm output to custom file
 $ prosperity2bt example/starter.py 1 --out example.log
 
 # Backtest on custom data
 # Requires the value passed to `--data` to be a path to a directory that is similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources
 $ prosperity2bt example/starter.py 1 --data prosperity2bt/resources
+
+# Print trader's output to stdout while running
+# This may be helpful when debugging a broken trader
+$ prosperity2bt example/starter.py 1 --print
 ```
 
 ## Order Matching
 
 Orders placed by `Trader.run` at a given timestamp are matched against the order depths of that timestamp's state. Market trades are ignored in the matching process. Orders are executed at your best possible price, e.g. if you place a buy order for €10 but there is non-zero ask volume at €9, your order is (possibly partially) filled at €9. Similarly, if you place a sell order for €10 but there is non-zero bid volume at €11, your order is (possibly partially) filled at €11.
 
 Limits are enforced before orders are matched to order depths. If for a product your position would exceed the limit, assuming all your orders would get filled, all your orders for that product get canceled.
```

### Comparing `prosperity2bt-0.2.0/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.3.0/prosperity2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.2.0/pyproject.toml` & `prosperity2bt-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">= 3.9"
-dependencies = ["jsonpickle"]
+dependencies = ["ipython", "jsonpickle"]
 
 [project.scripts]
 prosperity2bt = "prosperity2bt.main:main"
 
 [project.urls]
 Repository = "https://github.com/jmerle/imc-prosperity-2-backtester"
 Issues = "https://github.com/jmerle/imc-prosperity-2-backtester/issues"
```

