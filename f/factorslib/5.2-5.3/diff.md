# Comparing `tmp/factorslib-5.2.tar.gz` & `tmp/factorslib-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorslib-5.2.tar", last modified: Thu Dec 14 10:26:26 2023, max compression
+gzip compressed data, was "factorslib-5.3.tar", last modified: Tue Apr  9 06:09:31 2024, max compression
```

## Comparing `factorslib-5.2.tar` & `factorslib-5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-12-14 10:26:26.470496 factorslib-5.2/
--rw-rw-rw-   0        0        0     1038 2023-12-04 06:04:59.000000 factorslib-5.2/LICENCE.txt
--rw-rw-rw-   0        0        0      325 2023-12-14 10:26:26.470496 factorslib-5.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-12-04 06:04:59.000000 factorslib-5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-12-14 10:26:26.468451 factorslib-5.2/factorslib/
--rw-rw-rw-   0        0        0        0 2023-12-04 06:04:59.000000 factorslib-5.2/factorslib/__init__.py
--rw-rw-rw-   0        0        0    73962 2023-12-14 10:26:01.000000 factorslib-5.2/factorslib/factors.py
-drwxrwxrwx   0        0        0        0 2023-12-14 10:26:26.469506 factorslib-5.2/factorslib.egg-info/
--rw-rw-rw-   0        0        0      325 2023-12-14 10:26:26.000000 factorslib-5.2/factorslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-12-14 10:26:26.000000 factorslib-5.2/factorslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-14 10:26:26.000000 factorslib-5.2/factorslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-12-14 10:26:26.000000 factorslib-5.2/factorslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-14 10:26:26.470496 factorslib-5.2/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-12-14 10:26:17.000000 factorslib-5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:09:31.130603 factorslib-5.3/
+-rw-rw-rw-   0        0        0     1038 2023-12-04 06:04:59.000000 factorslib-5.3/LICENCE.txt
+-rw-rw-rw-   0        0        0      325 2024-04-09 06:09:31.130603 factorslib-5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-12-04 06:04:59.000000 factorslib-5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 06:09:31.128609 factorslib-5.3/factorslib/
+-rw-rw-rw-   0        0        0        0 2023-12-04 06:04:59.000000 factorslib-5.3/factorslib/__init__.py
+-rw-rw-rw-   0        0        0    79663 2024-04-09 05:53:57.000000 factorslib-5.3/factorslib/factors.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:09:31.130603 factorslib-5.3/factorslib.egg-info/
+-rw-rw-rw-   0        0        0      325 2024-04-09 06:09:31.000000 factorslib-5.3/factorslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-04-09 06:09:31.000000 factorslib-5.3/factorslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 06:09:31.000000 factorslib-5.3/factorslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 06:09:31.000000 factorslib-5.3/factorslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 06:09:31.130603 factorslib-5.3/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-04-09 05:54:26.000000 factorslib-5.3/setup.py
```

### Comparing `factorslib-5.2/LICENCE.txt` & `factorslib-5.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `factorslib-5.2/factorslib/factors.py` & `factorslib-5.3/factorslib/factors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1223,14 +1223,15 @@
     df1['RSI'] = talib.RSI(close, timeperiod=N1)
     df1['RSIMA'] = talib.SMA(df1['RSI'], timeperiod=N2)
 
     df1['signal'] = 0
     df1.loc[df1['RSI'] >= df1['RSIMA'], 'signal'] = 1
 
     df_final = pd.merge(df1, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['signal'] == 1) & (df_final['bull'] == 1), 'signalF'] = N3
     df_final.loc[(df_final['signal'] == 1) & (df_final['bull'] == 0), 'signalF'] = N4
 
     return df_final
 
@@ -1311,14 +1312,15 @@
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1 = talib_MACD(df=df1, target=close, N1=N1, N2=N2, N3=N3)
     df1['MACDMA'] = talib.SMA(df1['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)], timeperiod=N4)
 
     df_final = pd.merge(df1, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] > 0) & (df_final['bull'] == 1), 'signalF'] = N5
     df_final.loc[(df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] > 0) & (df_final['bull'] == 0), 'signalF'] = N6
     df_final.loc[df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] < df_final['MACDMA'], 'signalF'] = 0
 
     return df_final
@@ -1346,14 +1348,15 @@
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1 = talib_MACD(df=df1, target=close, N1=N1, N2=N2, N3=N3)
     df1['MACDMA1'] = talib.SMA(df1['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)], timeperiod=N4)
     df1['MACDMA2'] = talib.SMA(df1['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)], timeperiod=N5)
 
     df_final = pd.merge(df1, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] > 0) & (df_final['bull'] == 1), 'signalF'] = N6
     df_final.loc[(df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] > 0) & (df_final['bull'] == 0), 'signalF'] = N7
 
     df_final.loc[(df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] < 0) & (df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] > df_final['MACDMA2']) & (df_final['bull'] == 1), 'signalF'] = N8
     df_final.loc[(df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] < 0) & (df_final['MACD_' + str(N1) + '_' + str(N2) + '_' + str(N3)] > df_final['MACDMA2']) & (df_final['bull'] == 0), 'signalF'] = N9
@@ -1419,14 +1422,15 @@
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1 = pdta.kdj(high=high, low=low, close=close, length=N1, signal=N2)
     df1.columns = ['K', 'D', 'J']
     df2 = pd.concat([df, df1], axis=1)
 
     df_final = pd.merge(df2, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['K'] > df_final['D']) & (df_final['bull'] == 1), 'signalF'] = N3
     df_final.loc[(df_final['K'] > df_final['D']) & (df_final['bull'] == 0), 'signalF'] = N4
 
     return df_final
 
@@ -1438,14 +1442,15 @@
     df1 = pdta.kdj(high=high, low=low, close=close, length=N1, signal=N2)
     df1.columns = ['K', 'D', 'J']
     df2 = pd.concat([df, df1], axis=1)
 
     df2['KMA'] = talib.SMA(df2['K'], timeperiod=N3)
 
     df_final = pd.merge(df2, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['K'] > df_final['D']) & (df_final['bull'] == 1), 'signalF'] = N4
     df_final.loc[(df_final['K'] > df_final['D']) & (df_final['bull'] == 0), 'signalF'] = N5
 
     df_final.loc[df2['K'] < df_final['KMA'], 'signalF'] = 0
 
@@ -1472,14 +1477,15 @@
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1 = pdta.stochrsi(close, length=N1, rsi_length=N2, k=N3, d=N4, mamode='sma', talib=False)
     df1.columns = ['STOCHRSIK', 'STOCHRSID']
     df2 = pd.concat([df, df1], axis=1)
 
     df_final = pd.merge(df2, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['STOCHRSIK'] > df_final['STOCHRSID']) & (df_final['bull'] == 1), 'signalF'] = N5
     df_final.loc[(df_final['STOCHRSIK'] > df_final['STOCHRSID']) & (df_final['bull'] == 0), 'signalF'] = N6
 
     return df_final
 
@@ -1495,37 +1501,46 @@
     df2 = i.df
 
     df2['signalF'] = 0
     df2.loc[(df2['Close'] > df2['alligator_jaw'])
             & (df2['Close'] > df2['alligator_teeth'])
             & (df2['Close'] > df2['alligator_lips']), 'signalF'] = 1
 
+    df2 = df2.rename(columns={'Close': closename}).rename(columns={highname: 'High'}).rename(
+        columns={'Low': lowname})
+
     return df2
 
 
 def ALLIGATOR1_timing(df, closename, highname, lowname, N1, N2, N3, N4, N5, N6, N7, N8, MA_df, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1 = df1.rename(columns={closename: 'Close'}).rename(columns={highname: 'High'}).rename(columns={lowname: 'Low'})
     i = Indicators(df1)
-    i.alligator(period_jaws=N1, period_teeth=N2, period_lips=N3, shift_jaws=N4, shift_teeth=N5, shift_lips=N6, column_name_jaws='alligator_jaw', column_name_teeth='alligator_teeth', column_name_lips='alligator_lips')
+    i.alligator(period_jaws=N1, period_teeth=N2, period_lips=N3, shift_jaws=N4, shift_teeth=N5, shift_lips=N6,
+                column_name_jaws='alligator_jaw', column_name_teeth='alligator_teeth',
+                column_name_lips='alligator_lips')
     df2 = i.df
 
     df_final = pd.merge(df2, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['Close'] > df_final['alligator_jaw'])
                  & (df_final['Close'] > df_final['alligator_teeth'])
                  & (df_final['Close'] > df_final['alligator_lips']) & (df_final['bull'] == 1), 'signalF'] = N7
 
     df_final.loc[(df_final['Close'] > df_final['alligator_jaw'])
                  & (df_final['Close'] > df_final['alligator_teeth'])
                  & (df_final['Close'] > df_final['alligator_lips']) & (df_final['bull'] == 0), 'signalF'] = N8
 
+    df_final = df_final.rename(columns={'Close': closename}).rename(columns={highname: 'High'}).rename(
+        columns={'Low': lowname})
+
     return df_final
 
 
 def ALLIGATOR2_timing(df, closename, highname, lowname, N1, N2, N3, N4, N5, N6, N7, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
@@ -1540,14 +1555,17 @@
     df2['signalF'] = 0
     df2.loc[(df2['Close'] > df2['alligator_jaw'])
             & (df2['Close'] > df2['alligator_teeth'])
             & (df2['Close'] > df2['alligator_lips']), 'signalF'] = 1
 
     df2.loc[df2['diff'] < df2['diffMA'], 'signalF'] = 0
 
+    df2 = df2.rename(columns={'Close': closename}).rename(columns={highname: 'High'}).rename(
+        columns={'Low': lowname})
+
     return df2
 
 
 def ALLIGATOR3_timing(df, closename, highname, lowname, N1, N2, N3, N4, N5, N6, N7, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
@@ -1559,14 +1577,17 @@
     df2['diff'] = (abs(df2['alligator_jaw'] - df2['alligator_teeth']) + abs(df2['alligator_jaw'] - df2['alligator_lips']) + abs(df2['alligator_teeth'] - df2['alligator_lips'])) / 3
     df2['diffMA'] = talib.SMA(df2['diff'], timeperiod=N7)
 
     df2['signalF'] = 0
     df2.loc[df2['Close'] > df2['alligator_jaw'], 'signalF'] = 1
     df2.loc[df2['diff'] < df2['diffMA'], 'signalF'] = 0
 
+    df2 = df2.rename(columns={'Close': closename}).rename(columns={highname: 'High'}).rename(
+        columns={'Low': lowname})
+
     return df2
 
 
 def ALLIGATOR4_timing(df, closename, highname, lowname, N1, N2, N3, N4, N5, N6, N7, N8, N9, MA_df, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
@@ -1575,25 +1596,29 @@
     i.alligator(period_jaws=N1, period_teeth=N2, period_lips=N3, shift_jaws=N4, shift_teeth=N5, shift_lips=N6, column_name_jaws='alligator_jaw', column_name_teeth='alligator_teeth', column_name_lips='alligator_lips')
     df2 = i.df
 
     df2['diff'] = (abs(df2['alligator_jaw'] - df2['alligator_teeth']) + abs(df2['alligator_jaw'] - df2['alligator_lips']) + abs(df2['alligator_teeth'] - df2['alligator_lips'])) / 3
     df2['diffMA'] = talib.SMA(df2['diff'], timeperiod=N7)
 
     df_final = pd.merge(df2, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['Close'] > df_final['alligator_jaw'])
                  & (df_final['Close'] > df_final['alligator_teeth'])
                  & (df_final['Close'] > df_final['alligator_lips']) & (df_final['bull'] == 1), 'signalF'] = N8
     df_final.loc[(df_final['Close'] > df_final['alligator_jaw'])
                  & (df_final['Close'] > df_final['alligator_teeth'])
                  & (df_final['Close'] > df_final['alligator_lips']) & (df_final['bull'] == 0), 'signalF'] = N9
 
     df_final.loc[df_final['diff'] < df_final['diffMA'], 'signalF'] = 0
 
+    df_final = df_final.rename(columns={'Close': closename}).rename(columns={highname: 'High'}).rename(
+        columns={'Low': lowname})
+
     return df_final
 
 
 # --------------------------------------------------------20230608新增，择时，BBI
 def BBIC_timing(df, close, N1, N2, N3, N4, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
@@ -1629,14 +1654,15 @@
     df1['MA' + '_' + str(N3)] = ma3.sma_indicator()
     df1['MA' + '_' + str(N4)] = ma4.sma_indicator()
 
     df1['BBI'] = (df1['MA' + '_' + str(N1)] + df1['MA' + '_' + str(N2)] + df1['MA' + '_' + str(N3)] + df1['MA' + '_' + str(N4)]) / 4
     df1['BBIC'] = df1['BBI'] / close
 
     df_final = pd.merge(df1, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(close > df_final['BBI']) & (df_final['bull'] == 1), 'signalF'] = N5
     df_final.loc[(close > df_final['BBI']) & (df_final['bull'] == 0), 'signalF'] = N6
 
     return df_final
 
@@ -1687,14 +1713,15 @@
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df2, df3 = pdta.ichimoku(close=close, high=high, low=low, tenkan=N1, kijun=N2, senkou=N3, talib=False)
     df_final = pd.concat([df1, df2], axis=1)
 
     df_final = pd.merge(df_final, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
     df_final.loc[(df_final['ITS_' + str(N1)] > df_final['IKS_' + str(N2)]) & (close > df_final['IKS_' + str(N2)]) & (df_final['bull'] == 1), 'signalF'] = N4
     df_final.loc[(df_final['ITS_' + str(N1)] > df_final['IKS_' + str(N2)]) & (close > df_final['IKS_' + str(N2)]) & (df_final['bull'] == 0), 'signalF'] = N5
     df_final.loc[df_final['ISB_' + str(N2)] > df_final['ISA_' + str(N1)], 'signalF'] = 0
 
     return df_final
@@ -1722,14 +1749,15 @@
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df2 = pdta.kc(close=close, high=high, low=low, length=N1, scalar=N2, talib=False)
     df2.columns = ['KCL', 'KCM', 'KCU']
     df_final = pd.concat([df1, df2], axis=1)
 
     df_final = pd.merge(df_final, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
 
     df_final.loc[(close > df_final['KCM']) & (close < df_final['KCU']) & (df_final['bull'] == 1), 'signalF'] = N3
     df_final.loc[(close > df_final['KCU']) & (df_final['bull'] == 1), 'signalF'] = N4
     df_final.loc[(close > df_final['KCM']) & (close < df_final['KCU']) & (df_final['bull'] == 0), 'signalF'] = N5
     df_final.loc[(close > df_final['KCU']) & (df_final['bull'] == 0), 'signalF'] = N6
@@ -1742,14 +1770,15 @@
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df2 = pdta.kc(close=close, high=high, low=low, length=N1, scalar=N2, talib=False)
     df2.columns = ['KCL', 'KCM', 'KCU']
     df_final = pd.concat([df1, df2], axis=1)
 
     df_final = pd.merge(df_final, MA_df, on='time', how='left')
+    df_final['bull'].fillna(method='ffill', inplace=True)
 
     df_final['signalF'] = 0
 
     df_final.loc[(close > df_final['KCM']) & (close < df_final['KCU']) & (df_final['bull'] == 1), 'signalF'] = N3
     df_final.loc[(close > df_final['KCU']) & (df_final['bull'] == 1), 'signalF'] = N4
     df_final.loc[(close > df_final['KCM']) & (close < df_final['KCU']) & (df_final['bull'] == 0), 'signalF'] = N5
     df_final.loc[(close > df_final['KCU']) & (df_final['bull'] == 0), 'signalF'] = N6
@@ -1773,14 +1802,15 @@
 def SAR1_timing(df, close, high, low, N1, N2, MA_df, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1['SAR'] = talib.SAR(high=high, low=low)
 
     df1 = pd.merge(df1, MA_df, on='time', how='left')
+    df1['bull'].fillna(method='ffill', inplace=True)
 
     df1['signalF'] = 0
     df1.loc[(close > df1['SAR']) & (df1['bull'] == 1), 'signalF'] = N1
     df1.loc[(close > df1['SAR']) & (df1['bull'] == 0), 'signalF'] = N2
 
     return df1
 
@@ -1824,18 +1854,110 @@
 def CCI1_timing(df, close, high, low, N1, N2, N3, MA_df, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1['CCI'] = talib.CCI(close=close, high=high, low=low, timeperiod=N1)
 
     df1 = pd.merge(df1, MA_df, on='time', how='left')
+    df1['bull'].fillna(method='ffill', inplace=True)
 
     df1['signalF'] = np.nan
     df1.loc[df1['CCI'] <= -100, 'signalF'] = 0
     df1.loc[(df1['CCI'] >= 100) & (df1['bull'] == 1), 'signalF'] = N2
     df1.loc[(df1['CCI'] >= 100) & (df1['bull'] == 0), 'signalF'] = N3
 
     df1.fillna(method='ffill', inplace=True)
     df1.fillna(value=0, inplace=True)
 
     return df1
 
+
+# --------------------------------------------------------20240402新增，动量，STOCHk_N1_N2_N3 and STOCHd_N1_N2_N3
+def talib_STOCH(df, close, high, low, N1, N2, N3, *args, **kwargs):
+    df1 = df.copy()
+    df1['STOCHk_' + str(N1) + '_' + str(N2) + '_' + str(N3)], df1['STOCHd_' + str(N1) + '_' + str(N2) + '_' + str(N3)] = talib.STOCH(close=close, high=high, low=low, fastk_period=N1, slowd_period=N2, slowk_period=N3, slowk_matype=0)
+    return df1
+
+
+def pdta_STOCH(df, close, high, low, N1, N2, N3, *args, **kwargs):
+    df = df.copy()
+    df1 = pdta.stoch(close=close, high=high, low=low, k=N1, d=N2, smooth_k=N3, mamode='sma', talib=False)
+    df2 = pd.concat([df, df1], axis=1)
+    return df2
+
+
+# --------------------------------------------------------20240402新增，择时，STOCH
+def STOCH_timing(df, close, high, low, N1, N2, N3, N4, N5, *args, **kwargs):
+    df1 = df.copy()
+    df1['time'] = pd.to_datetime(df1['time'], utc=True)
+    df1['k'], df1['d'] = talib.STOCH(close=close, high=high, low=low, fastk_period=N1, slowd_period=N2,
+                                     slowk_period=N3, slowk_matype=0)
+
+    df1['signalF'] = 0
+    df1.loc[(df1['k'].shift(1) < df1['d'].shift(1)) & (df1['k'] > df1['d']) & (df1['k'] >= N4) & (
+            df1['k'] <= N5), 'signalF'] = 1
+    df1.loc[(df1['k'] > df1['d']) & (df1['k'] >= N4) & (df1['k'].shift(1) < N4), 'signalF'] = 1
+    df1.loc[(df1['k'].shift(1) > df1['d'].shift(1)) & (df1['k'] < df1['d']) & (df1['k'] >= N4) & (
+            df1['k'] <= N5), 'signalF'] = -1
+    df1.loc[(df1['k'] < df1['d']) & (df1['k'] <= N5) & (df1['k'].shift(1) > N5), 'signalF'] = -1
+
+    return df1
+
+
+# --------------------------------------------------------20240402新增，量比因子，VRATIO_N1_N2
+def talib_VRATIO(df, target, N1, N2, *args, **kwargs):
+    df1 = df.copy()
+    df1['VRATIO_' + str(N1) + '_' + str(N2)] = talib.SMA(target, timeperiod=N1).astype(float) / talib.SMA(target,
+                                                                                                          timeperiod=N2).astype(
+        float)
+    df1['VRATIO_' + str(N1) + '_' + str(N2)].replace([np.inf, -np.inf], 0, inplace=True)
+
+    return df1
+
+
+def pdta_VRATIO(df, target, N1, N2, *args, **kwargs):
+    df1 = df.copy()
+    df1['Vratio_' + str(N1) + '_' + str(N2)] = pdta.sma(target, length=N1, talib=False).astype(float) / pdta.sma(target, length=N2, talib=False).astype(float)
+    return df1
+
+
+# --------------------------------------------------------20240402新增，波动趋势因子，BRATIO_N1_N2
+def talib_BRATIO(df, target, N1, N2, *args, **kwargs):
+    df1 = df.copy()
+    a, b, c = talib.BBANDS(target, timeperiod=N1, nbdevup=2, nbdevdn=2, matype=0)
+    a1, b1, c1 = talib.BBANDS(target, timeperiod=N2, nbdevup=2, nbdevdn=2, matype=0)
+    df1['BRATIO_' + str(N1) + '_' + str(N2)] = (a.astype(float) - b.astype(float)) / (
+                a1.astype(float) - b1.astype(float))
+    df1['BRATIO_' + str(N1) + '_' + str(N2)].replace([np.inf, -np.inf], 0, inplace=True)
+
+    return df1
+
+
+def pdta_BRATIO(df, target, N1, N2, *args, **kwargs):
+    df1 = df.copy()
+
+    a = pdta.bbands(target, length=N1, std=2, talib=False)
+    b = pdta.bbands(target, length=N2, std=2, talib=False)
+
+    df1['BRATIO_' + str(N1) + '_' + str(N2)] = (a['BBU'].astype(float) - a['BBM'].astype(float)) / (b['BBU'].astype(float) - b['BBM'].astype(float))
+
+    return df1
+
+
+# --------------------------------------------------------20240402新增，瞬时波动因子，PRATIO_N
+def talib_PRATIO(df, target, N, *args, **kwargs):
+    df1 = df.copy()
+    chg = (target.apply(np.log) - target.shift(1).apply(np.log)).astype(float)
+    df1['PRATIO_' + str(N)] = chg / talib.SMA(target, timeperiod=N).astype(float)
+    df1['PRATIO_' + str(N)].replace([np.inf, -np.inf], 0, inplace=True)
+
+    return df1
+
+
+def pdta_PRATIO(df, target, N, *args, **kwargs):
+    df1 = df.copy()
+
+    chg = (target.apply(np.log) - target.shift(1).apply(np.log)).astype(float)
+    df1['PRATIO_' + str(N)] = chg / pdta.sma(target, length=N, talib=False).astype(float)
+
+    return df1
+
```

### Comparing `factorslib-5.2/setup.py` & `factorslib-5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="factorslib",
-    version="5.2",
+    version="5.3",
     author="wytxty",
     author_email="yvettewkkaa@gmail.com",
     description="financial factors calculation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wytxty/factorslib",
     packages=setuptools.find_packages(),
```

