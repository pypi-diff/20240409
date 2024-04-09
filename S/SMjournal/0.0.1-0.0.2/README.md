# Comparing `tmp/SMjournal-0.0.1.tar.gz` & `tmp/SMjournal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjournal-0.0.1.tar", last modified: Tue Dec 26 12:39:35 2023, max compression
+gzip compressed data, was "SMjournal-0.0.2.tar", last modified: Tue Apr  9 15:17:57 2024, max compression
```

## Comparing `SMjournal-0.0.1.tar` & `SMjournal-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-12-26 12:39:35.906000 SMjournal-0.0.1/
--rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjournal-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      702 2023-12-26 12:39:35.841000 SMjournal-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjournal-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-12-26 12:39:35.570000 SMjournal-0.0.1/SMjournal/
--rw-rw-rw-   0        0        0      128 2023-07-10 18:24:49.000000 SMjournal-0.0.1/SMjournal/__init__.py
--rw-rw-rw-   0        0        0     4536 2023-12-26 11:41:18.000000 SMjournal-0.0.1/SMjournal/collinearity.py
--rw-rw-rw-   0        0        0     4814 2023-11-29 19:24:47.000000 SMjournal-0.0.1/SMjournal/data.py
--rw-rw-rw-   0        0        0     1573 2023-08-09 15:09:40.000000 SMjournal-0.0.1/SMjournal/low_level.py
--rw-rw-rw-   0        0        0     4547 2023-10-27 17:01:49.000000 SMjournal-0.0.1/SMjournal/meta_reg.py
--rw-rw-rw-   0        0        0     2974 2023-07-11 22:14:59.000000 SMjournal-0.0.1/SMjournal/potentiality.py
-drwxrwxrwx   0        0        0        0 2023-12-26 12:39:35.817000 SMjournal-0.0.1/SMjournal.egg-info/
--rw-rw-rw-   0        0        0      702 2023-12-26 12:39:34.000000 SMjournal-0.0.1/SMjournal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-12-26 12:39:34.000000 SMjournal-0.0.1/SMjournal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-26 12:39:34.000000 SMjournal-0.0.1/SMjournal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-12-26 12:39:34.000000 SMjournal-0.0.1/SMjournal.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-26 12:39:34.000000 SMjournal-0.0.1/SMjournal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-06-12 14:12:51.000000 SMjournal-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      666 2023-12-26 12:39:35.899000 SMjournal-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 15:17:57.143000 SMjournal-0.0.2/
+-rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjournal-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      702 2024-04-09 15:17:57.115000 SMjournal-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjournal-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:17:56.878000 SMjournal-0.0.2/SMjournal/
+-rw-rw-rw-   0        0        0      128 2023-07-10 18:24:49.000000 SMjournal-0.0.2/SMjournal/__init__.py
+-rw-rw-rw-   0        0        0     4557 2024-04-09 15:14:02.000000 SMjournal-0.0.2/SMjournal/collinearity.py
+-rw-rw-rw-   0        0        0     4814 2023-11-29 19:24:47.000000 SMjournal-0.0.2/SMjournal/data.py
+-rw-rw-rw-   0        0        0     1573 2023-08-09 15:09:40.000000 SMjournal-0.0.2/SMjournal/low_level.py
+-rw-rw-rw-   0        0        0     4547 2023-10-27 17:01:49.000000 SMjournal-0.0.2/SMjournal/meta_reg.py
+-rw-rw-rw-   0        0        0     2974 2023-07-11 22:14:59.000000 SMjournal-0.0.2/SMjournal/potentiality.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:17:57.099000 SMjournal-0.0.2/SMjournal.egg-info/
+-rw-rw-rw-   0        0        0      702 2024-04-09 15:17:56.000000 SMjournal-0.0.2/SMjournal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-09 15:17:56.000000 SMjournal-0.0.2/SMjournal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:17:56.000000 SMjournal-0.0.2/SMjournal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-09 15:17:56.000000 SMjournal-0.0.2/SMjournal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 15:17:56.000000 SMjournal-0.0.2/SMjournal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 14:12:51.000000 SMjournal-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      666 2024-04-09 15:17:57.141000 SMjournal-0.0.2/setup.cfg
```

### Comparing `SMjournal-0.0.1/LICENSE` & `SMjournal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.1/PKG-INFO` & `SMjournal-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.1/SMjournal/collinearity.py` & `SMjournal-0.0.2/SMjournal/collinearity.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
   simil=1-disimil
   similitude=pd.DataFrame(simil)
   similitude.columns =tounderstand
   similitude.index=tounderstand
   return similitude
 
 
-
 def collinearity_test(df1,tounderstand='not',distance="vif",match=False,threshold=0.7):   #full test of collinearity, corr-abs interesting
   df=df1.copy()
   if tounderstand=='not':
     const_cols=[i for i in df.columns if ('.hol' in i.lower()) or ('.mkt' in i.lower())]
     tounderstand=[i for i in df.columns if i not in const_cols+['Geographies','Weeks','non_lin_pred','lin_pred']]
   to_test=tounderstand
 
@@ -135,22 +134,23 @@
   dendrogram(Z, labels=to_test, orientation='top', 
             leaf_rotation=90);
   plt.tight_layout()
   plt.savefig('maybe.svg', format='svg', dpi=1200)
 
   ########third
   try:
-    px.line(((df.groupby('Weeks').mean()-df.groupby('Weeks').mean().mean())/df.groupby('Weeks').mean().std()).reset_index(),x='Weeks',y=tounderstand).show()
+    fig=px.line(((df.groupby('Weeks').mean()-df.groupby('Weeks').mean().mean())/df.groupby('Weeks').mean().std()).reset_index(),x='Weeks',y=tounderstand)
+    fig.show()
   except Exception as e:
     print(e)
 
   # Clusterize the data
   
   labels = fcluster(Z, threshold, criterion='distance')
 
   # Show the cluster
   clus=[]
   for i in range(1,max(labels)+1):
     clus.append(list(np.array(to_test)[np.where(labels==i)[0]]))
-  return clus
+  return clus, fig, plt
```

### Comparing `SMjournal-0.0.1/SMjournal/data.py` & `SMjournal-0.0.2/SMjournal/data.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.1/SMjournal/low_level.py` & `SMjournal-0.0.2/SMjournal/low_level.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.1/SMjournal/meta_reg.py` & `SMjournal-0.0.2/SMjournal/meta_reg.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.1/SMjournal/potentiality.py` & `SMjournal-0.0.2/SMjournal/potentiality.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.1/SMjournal.egg-info/PKG-INFO` & `SMjournal-0.0.2/SMjournal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.1/setup.cfg` & `SMjournal-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 4d6a 6f75 726e 616c 0d0a 7665   = SMjournal..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 310d 0a61  rsion = 0.0.1..a
+00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a61  rsion = 0.0.2..a
 00000030: 7574 686f 7220 3d20 4167 7573 7469 6e20  uthor = Agustin 
 00000040: 4275 7374 6f73 2042 6172 746f 6e0d 0a61  Bustos Barton..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6167  uthor_email = ag
 00000060: 7573 7469 6e62 7573 746f 7362 6172 746f  ustinbustosbarto
 00000070: 6e40 676d 6169 6c2e 636f 6d0d 0a64 6573  n@gmail.com..des
 00000080: 6372 6970 7469 6f6e 203d 2049 6e76 6573  cription = Inves
 00000090: 7469 6761 7469 6f6e 204a 6f75 726e 616c  tigation Journal
```

