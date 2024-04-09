# Comparing `tmp/SMjournal-0.0.3.tar.gz` & `tmp/SMjournal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjournal-0.0.3.tar", last modified: Tue Apr  9 18:15:55 2024, max compression
+gzip compressed data, was "SMjournal-0.0.4.tar", last modified: Tue Apr  9 18:55:18 2024, max compression
```

## Comparing `SMjournal-0.0.3.tar` & `SMjournal-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:55.654000 SMjournal-0.0.3/
--rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjournal-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      702 2024-04-09 18:15:55.631000 SMjournal-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjournal-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:55.479000 SMjournal-0.0.3/SMjournal/
--rw-rw-rw-   0        0        0      128 2023-07-10 18:24:49.000000 SMjournal-0.0.3/SMjournal/__init__.py
--rw-rw-rw-   0        0        0     4604 2024-04-09 18:15:19.000000 SMjournal-0.0.3/SMjournal/collinearity.py
--rw-rw-rw-   0        0        0     4814 2023-11-29 19:24:47.000000 SMjournal-0.0.3/SMjournal/data.py
--rw-rw-rw-   0        0        0     1573 2023-08-09 15:09:40.000000 SMjournal-0.0.3/SMjournal/low_level.py
--rw-rw-rw-   0        0        0     4547 2023-10-27 17:01:49.000000 SMjournal-0.0.3/SMjournal/meta_reg.py
--rw-rw-rw-   0        0        0     2974 2023-07-11 22:14:59.000000 SMjournal-0.0.3/SMjournal/potentiality.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:15:55.619000 SMjournal-0.0.3/SMjournal.egg-info/
--rw-rw-rw-   0        0        0      702 2024-04-09 18:15:55.000000 SMjournal-0.0.3/SMjournal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-09 18:15:55.000000 SMjournal-0.0.3/SMjournal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:15:55.000000 SMjournal-0.0.3/SMjournal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-09 18:15:55.000000 SMjournal-0.0.3/SMjournal.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 18:15:55.000000 SMjournal-0.0.3/SMjournal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-06-12 14:12:51.000000 SMjournal-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      666 2024-04-09 18:15:55.652000 SMjournal-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 18:55:18.802000 SMjournal-0.0.4/
+-rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjournal-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      702 2024-04-09 18:55:18.776000 SMjournal-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjournal-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 18:55:18.604000 SMjournal-0.0.4/SMjournal/
+-rw-rw-rw-   0        0        0      128 2023-07-10 18:24:49.000000 SMjournal-0.0.4/SMjournal/__init__.py
+-rw-rw-rw-   0        0        0     4604 2024-04-09 18:15:19.000000 SMjournal-0.0.4/SMjournal/collinearity.py
+-rw-rw-rw-   0        0        0     4814 2023-11-29 19:24:47.000000 SMjournal-0.0.4/SMjournal/data.py
+-rw-rw-rw-   0        0        0     1573 2023-08-09 15:09:40.000000 SMjournal-0.0.4/SMjournal/low_level.py
+-rw-rw-rw-   0        0        0     4547 2023-10-27 17:01:49.000000 SMjournal-0.0.4/SMjournal/meta_reg.py
+-rw-rw-rw-   0        0        0     3016 2024-04-09 18:54:56.000000 SMjournal-0.0.4/SMjournal/potentiality.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:55:18.766000 SMjournal-0.0.4/SMjournal.egg-info/
+-rw-rw-rw-   0        0        0      702 2024-04-09 18:55:18.000000 SMjournal-0.0.4/SMjournal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-09 18:55:18.000000 SMjournal-0.0.4/SMjournal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:55:18.000000 SMjournal-0.0.4/SMjournal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-09 18:55:18.000000 SMjournal-0.0.4/SMjournal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 18:55:18.000000 SMjournal-0.0.4/SMjournal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 14:12:51.000000 SMjournal-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      666 2024-04-09 18:55:18.800000 SMjournal-0.0.4/setup.cfg
```

### Comparing `SMjournal-0.0.3/LICENSE` & `SMjournal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.3/PKG-INFO` & `SMjournal-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.3/SMjournal/collinearity.py` & `SMjournal-0.0.4/SMjournal/collinearity.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.3/SMjournal/data.py` & `SMjournal-0.0.4/SMjournal/data.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.3/SMjournal/low_level.py` & `SMjournal-0.0.4/SMjournal/low_level.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.3/SMjournal/meta_reg.py` & `SMjournal-0.0.4/SMjournal/meta_reg.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.3/SMjournal/potentiality.py` & `SMjournal-0.0.4/SMjournal/potentiality.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tqdm import tqdm
 import pandas as pd
 import plotly.express as px
 from .low_level import getFullCombination
 from IPython.display import display,HTML
 
 
+
 def importance_test(df1,y_col,weight_col=None,control_cols='not',const_cols='not'):
   df=df1.copy()
   if weight_col:
     df=df.loc[df[weight_col]>0]
 
 
   if const_cols=='not':
@@ -51,15 +52,15 @@
   reg = LinearRegression().fit(pre_X, pre_y,weight)
   topred=pd.concat([df[x_cols],
           ],axis=1)
   topred_np=topred.to_numpy()
   df['lin_pred']=reg.predict(topred_np)
   baseError=np.mean((df['lin_pred'].to_numpy()-df[y_col].to_numpy())**2)
   ress=pd.DataFrame(dict(cols=control_cols, imp=np.array(allLosses)-baseError))
-  ress.sort_values('imp').plot('cols', 'imp', 'barh')
+  plot0=ress.sort_values('imp').plot('cols', 'imp', 'barh')
   
 
 
   x_cols=control_cols+const_cols
   pre_y=df[y_col].to_numpy()
   df_x=pd.concat([df[x_cols],
           ],axis=1)
@@ -80,8 +81,9 @@
   fig=px.line(fulltotal,x='Weeks',y=[y_col,'non_lin_pred','lin_pred'])
   fig.show()
   #guardar_fig(fig,"bg overfitteado con vars de covid")
   display(HTML('<h1>First Linear, Second Non-Linear<h1>'))
   np.mean((df['non_lin_pred'].to_numpy()-df[y_col].to_numpy())**2)
   ress=pd.DataFrame(dict(cols=x_cols, imp=rf.feature_importances_))
   # ress.loc[ress["imp"]>0].plot('cols', 'imp', 'barh')
-  ress.sort_values('imp').loc[ress["imp"]>0.001].plot('cols', 'imp', 'barh')
+  plot1=ress.sort_values('imp').loc[ress["imp"]>0.001].plot('cols', 'imp', 'barh')
+  return fig, plot0, plot1
```

### Comparing `SMjournal-0.0.3/SMjournal.egg-info/PKG-INFO` & `SMjournal-0.0.4/SMjournal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.3/setup.cfg` & `SMjournal-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 4d6a 6f75 726e 616c 0d0a 7665   = SMjournal..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 330d 0a61  rsion = 0.0.3..a
+00000020: 7273 696f 6e20 3d20 302e 302e 340d 0a61  rsion = 0.0.4..a
 00000030: 7574 686f 7220 3d20 4167 7573 7469 6e20  uthor = Agustin 
 00000040: 4275 7374 6f73 2042 6172 746f 6e0d 0a61  Bustos Barton..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6167  uthor_email = ag
 00000060: 7573 7469 6e62 7573 746f 7362 6172 746f  ustinbustosbarto
 00000070: 6e40 676d 6169 6c2e 636f 6d0d 0a64 6573  n@gmail.com..des
 00000080: 6372 6970 7469 6f6e 203d 2049 6e76 6573  cription = Inves
 00000090: 7469 6761 7469 6f6e 204a 6f75 726e 616c  tigation Journal
```

