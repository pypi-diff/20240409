# Comparing `tmp/ml_backtest-0.1.2.tar.gz` & `tmp/ml_backtest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_backtest-0.1.2.tar", last modified: Sun Apr  7 04:05:56 2024, max compression
+gzip compressed data, was "ml_backtest-0.1.3.tar", last modified: Tue Apr  9 14:42:23 2024, max compression
```

## Comparing `ml_backtest-0.1.2.tar` & `ml_backtest-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.345187 ml_backtest-0.1.2/backtesting-with-machine-learning/
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/backtesting-with-machine-learning/machine-learning-class-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/backtesting-with-machine-learning/strategy-creation-class-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.345187 ml_backtest-0.1.2/ml_backtest/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/backtest/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/data/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/interfaces/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/machine_learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/machine_learning/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.349187 ml_backtest-0.1.2/ml_backtest/models/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/models/rfr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/ml_backtest/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/bullishengulfing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/bullishharami.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/dragonflydoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/hammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/invertedhammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/morningstar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/morningstardoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/ml_backtest/strategies/piercingpattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/ml_backtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 04:05:56.000000 ml_backtest-0.1.2/ml_backtest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:56.353186 ml_backtest-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-07 04:04:37.000000 ml_backtest-0.1.2/tests/test_ml_backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.454624 ml_backtest-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-09 14:42:23.454624 ml_backtest-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.446624 ml_backtest-0.1.3/backtesting-with-machine-learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/backtesting-with-machine-learning/machine-learning-class-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/backtesting-with-machine-learning/strategy-creation-class-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.450624 ml_backtest-0.1.3/ml_backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.450624 ml_backtest-0.1.3/ml_backtest/backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/backtest/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.450624 ml_backtest-0.1.3/ml_backtest/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.450624 ml_backtest-0.1.3/ml_backtest/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/interfaces/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.450624 ml_backtest-0.1.3/ml_backtest/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/machine_learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/machine_learning/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.450624 ml_backtest-0.1.3/ml_backtest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/models/rfr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.454624 ml_backtest-0.1.3/ml_backtest/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/bullishengulfing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/bullishharami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/dragonflydoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/hammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/invertedhammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/morningstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/morningstardoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/ml_backtest/strategies/piercingpattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.454624 ml_backtest-0.1.3/ml_backtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-09 14:42:23.000000 ml_backtest-0.1.3/ml_backtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-09 14:42:23.000000 ml_backtest-0.1.3/ml_backtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:42:23.000000 ml_backtest-0.1.3/ml_backtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 14:42:23.000000 ml_backtest-0.1.3/ml_backtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 14:42:23.000000 ml_backtest-0.1.3/ml_backtest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:42:23.454624 ml_backtest-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:42:23.454624 ml_backtest-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 14:41:02.000000 ml_backtest-0.1.3/tests/test_ml_backtest.py
```

### Comparing `ml_backtest-0.1.2/LICENSE` & `ml_backtest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/PKG-INFO` & `ml_backtest-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_backtest-0.1.2/README.md` & `ml_backtest-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/backtesting-with-machine-learning/machine-learning-class-guide.md` & `ml_backtest-0.1.3/backtesting-with-machine-learning/machine-learning-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/backtesting-with-machine-learning/strategy-creation-class-guide.md` & `ml_backtest-0.1.3/backtesting-with-machine-learning/strategy-creation-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/ml_backtest/backtest/backtest.py` & `ml_backtest-0.1.3/ml_backtest/backtest/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,14 @@
                                    'gross profit': np.around(self.__gross_profit, decimals=2),
                                    'gross loss': np.around(self.__gross_loss, decimals=2),
                                    'profit factor': np.around(self.__gross_profit / abs(self.__gross_loss),
                                                               decimals=2)}]
 
         self.__backtest_df = pd.DataFrame(self.__backtest_result)
         self.__backtest_df = self.__backtest_df.T
-        return self.__backtest_df
 
     def get_trades(self) -> pd.DataFrame:
         completed_trades_df = pd.DataFrame(self.__completed_trades)
         return completed_trades_df
 
     def get_results(self) -> pd.DataFrame:
         return self.__backtest_df
```

### Comparing `ml_backtest-0.1.2/ml_backtest/interfaces/interface.py` & `ml_backtest-0.1.3/ml_backtest/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/ml_backtest/machine_learning/wrapper.py` & `ml_backtest-0.1.3/ml_backtest/machine_learning/wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/ml_backtest/models/rfr.py` & `ml_backtest-0.1.3/ml_backtest/models/rfr.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/ml_backtest/strategies/bullishengulfing.py` & `ml_backtest-0.1.3/ml_backtest/strategies/bullishengulfing.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,26 +18,23 @@
             prev_open = open[index - 1]
 
             is_bullish_engulfing = CandleStickPatterns.is_bullish_engulfing(current_open=current_open,
                                                                             current_close=current_close,
                                                                             prev_open=prev_open,
                                                                             prev_close=prev_close)
 
-            # Enter a long position if a bullish engulfing pattern is detected
             if is_bullish_engulfing and not self.in_position and self.trading_hours(current_date):
-                # Make the metadata for the candle stick features for Machine Learning
                 trade_metadata = {
                     'current_open': current_open,
                     'current_close': current_close,
                     'prev_open': prev_open,
                     'prev_close': prev_close
                 }
-                # Assuming you want to enter at the next candle's open, which is current_close
                 entry_price = current_close
-                # Calculate take profit and stop loss as per your strategy
+
                 if self.model is not None:
                     if self.cs_patterns:
                         np_l = CandleStickDataProcessing.calculate_engulfing_features(**trade_metadata)
                         np_l_2d = np_l.reshape(1, -1)
                         prediction = self.predict(current_date, np_l_2d)
                         take_profit = entry_price + prediction
                     else:
```

### Comparing `ml_backtest-0.1.2/ml_backtest/strategies/bullishharami.py` & `ml_backtest-0.1.3/ml_backtest/strategies/piercingpattern.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from ml_backtest.interfaces import Strategy
 from ml_backtest.data import CandleStickPatterns
 from ml_backtest.machine_learning import CandleStickDataProcessing
 from datetime import time
 
 
-class BullishHarami(Strategy):
+class PiercingPattern(Strategy):
     def init(self):
         self.market_open_time = time(9, 30)
         self.market_close_time = time(16, 10)
 
     def on_data(self, index, lows, highs, closes, opens, dates):
-        # Ensure there is at least one previous candle to compare with
         if index > 0:
             current_open = opens[index]
             current_close = closes[index]
             current_date = dates[index]
             prev_open = opens[index - 1]
             prev_close = closes[index - 1]
+            prev_low = lows[index - 1]
 
-            # Check for bullish harami pattern
-            is_bullish_harami = (prev_open > prev_close and
-                                 prev_close <= current_open < current_close <= prev_open and
-                                 current_close - current_open < prev_open - prev_close)
-
-            # Enter a long position if a bullish harami pattern is detected
-            if is_bullish_harami and not self.in_position and self.trading_hours(current_date):
-                # Assuming you want to enter at the next candle's open, which is current_close
+            is_piercing_pattern = CandleStickPatterns.is_piercing_pattern(current_open=current_open,
+                                                                          current_close=current_close,
+                                                                          prev_open=prev_open,
+                                                                          prev_close=prev_close,
+                                                                          prev_low=prev_low)
+
+            if is_piercing_pattern and not self.in_position and self.trading_hours(current_date):
+                trade_metadata = {
+                    'current_open': current_open,
+                    'prev_open': prev_open,
+                    'prev_close': prev_close,
+                    'current_close': current_close
+                }
                 entry_price = current_close
-                # Calculate take profit and stop loss as per your strategy
+
                 if self.model is not None:
-                    prediction = self.predict(current_date)
-                    take_profit = entry_price + prediction
+                    if self.cs_patterns:
+                        np_l = CandleStickDataProcessing.calculate_piercing_pattern_features(**trade_metadata)
+                        np_l_2d = np_l.reshape(1, -1)
+                        prediction = self.predict(current_date, np_l_2d)
+                        take_profit = entry_price + prediction
+                    else:
+                        prediction = self.predict(current_date)
+                        take_profit = entry_price + prediction
                 else:
                     take_profit = entry_price + 50
                 stop_loss = entry_price - 37
                 entry_time = dates[index]
 
-                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss, entry_time=entry_time)
+                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss,
+                         entry_time=entry_time, metadata=trade_metadata)
```

### Comparing `ml_backtest-0.1.2/ml_backtest/strategies/dragonflydoji.py` & `ml_backtest-0.1.3/ml_backtest/strategies/hammer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 from ml_backtest.interfaces import Strategy
 from ml_backtest.data import CandleStickPatterns
 from ml_backtest.machine_learning import CandleStickDataProcessing
 from datetime import time
 
 
-class DragonFlyDoji(Strategy):
+class Hammer(Strategy):
     def init(self):
         self.market_open_time = time(9, 30)
         self.market_close_time = time(16, 10)
 
     def on_data(self, index, lows, highs, closes, opens, dates):
-        if index > 0:  # Ensure there's at least one candle to compare against
+        if index > 0:
             current_open = opens[index]
-            current_close = closes[index]
             current_high = highs[index]
             current_low = lows[index]
+            current_close = closes[index]
             current_date = dates[index]
 
-            # Adjusted calculation to avoid division by zero
-            body_range = abs(current_close - current_open)
-            total_range = current_high - current_low
-            upper_shadow = current_high - max(current_close, current_open)
-            lower_shadow = min(current_close, current_open) - current_low
-
-            # Check for Dragonfly Doji pattern with safeguards against division by zero
-            is_dragonfly_doji = (body_range / (total_range + 0.001) < 0.1 and
-                                 lower_shadow > (3 * body_range) and
-                                 upper_shadow < body_range)
+            is_hammer = CandleStickPatterns.is_hammer(current_open=current_open,
+                                                      current_low=current_low,
+                                                      current_high=current_high,
+                                                      current_close=current_close)
+
+            in_downtrend = current_close < closes[index - 1]
+
+            if is_hammer and in_downtrend and not self.in_position and self.trading_hours(current_date):
+                trade_metadata = {
+                    'current_open': current_open,
+                    'current_close': current_close,
+                    'current_low': current_low,
+                    'current_high': current_high
+                }
+                entry_price = current_close
 
-            if is_dragonfly_doji and not self.in_position and self.trading_hours(current_date):
-                entry_price = current_close  # Assuming entry at the close of the Dragonfly Doji
                 if self.model is not None:
-                    prediction = self.predict(current_date)
-                    take_profit = entry_price + prediction
+                    if self.cs_patterns:
+                        np_l = CandleStickDataProcessing.calculate_hammer_features(**trade_metadata)
+                        np_l_2d = np_l.reshape(1, -1)
+                        prediction = self.predict(current_date, np_l_2d)
+                        take_profit = entry_price + prediction
+                    else:
+                        prediction = self.predict(current_date)
+                        take_profit = entry_price + prediction
                 else:
                     take_profit = entry_price + 50
                 stop_loss = entry_price - 37
                 entry_time = dates[index]
 
-                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss, entry_time=entry_time)
+                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss,
+                         entry_time=entry_time, metadata=trade_metadata)
```

### Comparing `ml_backtest-0.1.2/ml_backtest/strategies/hammer.py` & `ml_backtest-0.1.3/ml_backtest/strategies/invertedhammer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 from ml_backtest.interfaces import Strategy
 from ml_backtest.data import CandleStickPatterns
 from ml_backtest.machine_learning import CandleStickDataProcessing
 from datetime import time
 
 
-class Hammer(Strategy):
+class InvertedHammer(Strategy):
     def init(self):
         self.market_open_time = time(9, 30)
         self.market_close_time = time(16, 10)
 
-    def on_data(self, index, lows, highs, closes, opens, dates):
-        # Ensure there's at least one previous candle to compare with for trend analysis
+    def on_data(self, index, low, high, close, open, dates):
+        # Check if the current candlestick is an inverted hammer
+        # Ensure index is not 0 to have previous data for trend confirmation
         if index > 0:
-            current_open = opens[index]
-            current_high = highs[index]
-            current_low = lows[index]
-            current_close = closes[index]
+            current_close = close[index]
+            current_open = open[index]
+            current_low = low[index]
+            current_high = high[index]
             current_date = dates[index]
 
-            # Check for Hammer pattern
-            is_hammer = (((current_high - current_low) > 3 * (current_open - current_close)) and
-                         ((current_close - current_low) / (0.001 + current_high - current_low) > 0.6) and
-                         ((current_open - current_low) / (0.001 + current_high - current_low) > 0.6))
+            is_inverted_hammer = CandleStickPatterns.is_inverted_hammer(current_open=current_open,
+                                                                        current_low=current_low,
+                                                                        current_high=current_high,
+                                                                        current_close=current_close)
 
             # To ensure it's at the bottom of a downtrend, check if the current close is less than the previous close
-            in_downtrend = current_close < closes[index - 1]
+            in_downtrend = current_close < close[index - 1]
 
-            # Enter a long position if a Hammer pattern is detected at the bottom of a downtrend
-            if is_hammer and in_downtrend and not self.in_position and self.trading_hours(current_date):
-                # Assuming entry at the next candle's open, which is the current close
+            # Enter a long position if an inverted hammer is detected at the bottom of a downtrend
+            if is_inverted_hammer and in_downtrend and not self.in_position and self.trading_hours(current_date):
+                # Make the metadata for the candle stick features for Machine Learning
+                trade_metadata = {
+                    'current_open': current_open,
+                    'current_low': current_low,
+                    'current_high': current_high,
+                    'current_close': current_close
+                }
+                # enter at the next candle's open which is current_close
                 entry_price = current_close
+
                 # Calculate take profit and stop loss as per your strategy
+                # if model is passed into backtest, use model to predict take profit
                 if self.model is not None:
-                    prediction = self.predict(current_date)
-                    take_profit = entry_price + prediction
+                    if self.cs_patterns:
+                        np_l = CandleStickDataProcessing.calculate_inverted_hammer_features(**trade_metadata)
+                        np_l_2d = np_l.reshape(1, -1)
+                        prediction = self.predict(current_date, np_l_2d)
+                        take_profit = entry_price + prediction
+                    else:
+                        prediction = self.predict(current_date)
+                        take_profit = entry_price + prediction
                 else:
                     take_profit = entry_price + 50
                 stop_loss = entry_price - 37
                 entry_time = dates[index]
 
-                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss, entry_time=entry_time)
+                self.buy(price=entry_price, take_profit=take_profit,
+                         stop_loss=stop_loss, entry_time=entry_time, metadata=trade_metadata)
```

### Comparing `ml_backtest-0.1.2/ml_backtest/strategies/piercingpattern.py` & `ml_backtest-0.1.3/ml_backtest/strategies/bullishharami.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 from ml_backtest.interfaces import Strategy
 from ml_backtest.data import CandleStickPatterns
 from ml_backtest.machine_learning import CandleStickDataProcessing
 from datetime import time
 
 
-class PiercingPattern(Strategy):
+class BullishHarami(Strategy):
     def init(self):
         self.market_open_time = time(9, 30)
         self.market_close_time = time(16, 10)
 
     def on_data(self, index, lows, highs, closes, opens, dates):
-        # Ensure there's at least one previous candle to compare with
         if index > 0:
             current_open = opens[index]
             current_close = closes[index]
             current_date = dates[index]
             prev_open = opens[index - 1]
             prev_close = closes[index - 1]
-            prev_low = lows[index - 1]
 
-            # Check for Piercing Pattern
-            is_piercing_pattern = (prev_close < prev_open and
-                                   current_open < prev_low and
-                                   prev_open > current_close > prev_close + ((prev_open - prev_close) / 2))
-
-            # Enter a long position if a Piercing Pattern is detected
-            if is_piercing_pattern and not self.in_position and self.trading_hours(current_date):
-                # Assuming entry at the current close
+            is_bullish_harami = CandleStickPatterns.is_bullish_harami(current_open=current_open,
+                                                                      current_close=current_close,
+                                                                      prev_open=prev_open,
+                                                                      prev_close=prev_close)
+
+            if is_bullish_harami and not self.in_position and self.trading_hours(current_date):
+                trade_metadata = {
+                    'current_open': current_open,
+                    'prev_open': prev_open,
+                    'prev_close': prev_close,
+                    'current_close': current_close
+                }
+
                 entry_price = current_close
-                # Calculate take profit and stop loss as per your strategy
+
                 if self.model is not None:
-                    prediction = self.predict(current_date)
-                    take_profit = entry_price + prediction
+                    if self.cs_patterns:
+                        np_l = CandleStickDataProcessing.calculate_bullish_harami_features(**trade_metadata)
+                        np_l_2d = np_l.reshape(1, -1)
+                        prediction = self.predict(current_date, np_l_2d)
+                        take_profit = entry_price + prediction
+                    else:
+                        prediction = self.predict(current_date)
+                        take_profit = entry_price + prediction
                 else:
                     take_profit = entry_price + 50
                 stop_loss = entry_price - 37
                 entry_time = dates[index]
 
-                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss, entry_time=entry_time)
+                self.buy(price=entry_price, take_profit=take_profit, stop_loss=stop_loss,
+                         entry_time=entry_time, metadata=trade_metadata)
```

### Comparing `ml_backtest-0.1.2/ml_backtest.egg-info/PKG-INFO` & `ml_backtest-0.1.3/ml_backtest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_backtest-0.1.2/ml_backtest.egg-info/SOURCES.txt` & `ml_backtest-0.1.3/ml_backtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/setup.py` & `ml_backtest-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.2/tests/test_ml_backtest.py` & `ml_backtest-0.1.3/tests/test_ml_backtest.py`

 * *Files identical despite different names*

