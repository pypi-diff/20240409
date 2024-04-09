# Comparing `tmp/STCAT-0.2.tar.gz` & `tmp/STCAT-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STCAT-0.2.tar", last modified: Tue Feb 27 09:09:17 2024, max compression
+gzip compressed data, was "STCAT-0.3.tar", last modified: Tue Apr  9 02:07:54 2024, max compression
```

## Comparing `STCAT-0.2.tar` & `STCAT-0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-02-27 09:09:17.000000 STCAT-0.2/
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)       56 2024-02-27 08:53:16.000000 STCAT-0.2/MANIFEST.in
--rw-r--r--   0 zhangchuyu (10072) zhangchuyu (10076)      631 2024-02-27 09:07:38.000000 STCAT-0.2/PKG-INFO
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     1147 2024-02-27 08:53:16.000000 STCAT-0.2/README.md
-drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-02-27 09:09:17.000000 STCAT-0.2/STCAT/
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)    15073 2024-02-27 08:54:49.000000 STCAT-0.2/STCAT/STCAT.py
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)       68 2024-02-27 08:54:49.000000 STCAT-0.2/STCAT/__init__.py
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     6109 2024-02-27 08:54:49.000000 STCAT-0.2/STCAT/annotate.py
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)    27653 2024-02-27 08:53:16.000000 STCAT-0.2/STCAT/classifier.py
-drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-02-27 09:09:17.000000 STCAT-0.2/STCAT/data/
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)  2115485 2024-02-27 09:03:38.000000 STCAT-0.2/STCAT/data/T_cell.pkl
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)  1051641 2024-02-27 09:03:38.000000 STCAT-0.2/STCAT/data/cd4.pkl
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)   582047 2024-02-27 08:54:49.000000 STCAT-0.2/STCAT/data/cd8.pkl
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)    11065 2024-02-27 08:51:22.000000 STCAT-0.2/STCAT/data/marker_CD4.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     6330 2024-02-27 09:03:38.000000 STCAT-0.2/STCAT/data/marker_CD8.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      233 2024-02-27 08:54:49.000000 STCAT-0.2/STCAT/logger.py
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     7505 2024-02-27 09:03:38.000000 STCAT-0.2/STCAT/models.py
-drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-02-27 09:09:17.000000 STCAT-0.2/STCAT.egg-info/
--rw-r--r--   0 zhangchuyu (10072) zhangchuyu (10076)      631 2024-02-27 08:57:15.000000 STCAT-0.2/STCAT.egg-info/PKG-INFO
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      406 2024-02-27 09:07:38.000000 STCAT-0.2/STCAT.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)        1 2024-02-27 09:07:37.000000 STCAT-0.2/STCAT.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      109 2024-02-27 09:07:37.000000 STCAT-0.2/STCAT.egg-info/requires.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)        6 2024-02-27 08:58:10.000000 STCAT-0.2/STCAT.egg-info/top_level.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      116 2024-02-27 08:51:22.000000 STCAT-0.2/requirements.txt
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)       38 2024-02-27 08:57:16.000000 STCAT-0.2/setup.cfg
--rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      753 2024-02-27 09:07:33.000000 STCAT-0.2/setup.py
+drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-04-09 02:07:54.000000 STCAT-0.3/
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)       56 2024-04-09 01:52:58.000000 STCAT-0.3/MANIFEST.in
+-rw-r--r--   0 zhangchuyu (10072) zhangchuyu (10076)      631 2024-04-09 01:56:41.000000 STCAT-0.3/PKG-INFO
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     1147 2024-04-09 01:54:18.000000 STCAT-0.3/README.md
+drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-04-09 02:07:54.000000 STCAT-0.3/STCAT/
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)    16594 2024-04-09 01:55:04.000000 STCAT-0.3/STCAT/STCAT.py
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)       68 2024-04-09 01:54:18.000000 STCAT-0.3/STCAT/__init__.py
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     6109 2024-04-09 01:52:58.000000 STCAT-0.3/STCAT/annotate.py
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)    27653 2024-04-09 01:51:28.000000 STCAT-0.3/STCAT/classifier.py
+drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-04-09 02:07:54.000000 STCAT-0.3/STCAT/data/
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)  2056303 2024-04-09 02:03:40.000000 STCAT-0.3/STCAT/data/T_cell.pkl
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)  1003868 2024-04-09 02:03:40.000000 STCAT-0.3/STCAT/data/cd4.pkl
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)   582043 2024-04-09 01:54:18.000000 STCAT-0.3/STCAT/data/cd8.pkl
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)    11065 2024-04-09 01:54:18.000000 STCAT-0.3/STCAT/data/marker_CD4.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     6330 2024-04-09 01:54:18.000000 STCAT-0.3/STCAT/data/marker_CD8.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      233 2024-04-09 01:51:28.000000 STCAT-0.3/STCAT/logger.py
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)     7505 2024-04-09 01:54:18.000000 STCAT-0.3/STCAT/models.py
+drwxrwxr-x   0 zhangchuyu (10072) zhangchuyu (10076)        0 2024-04-09 02:07:54.000000 STCAT-0.3/STCAT.egg-info/
+-rw-r--r--   0 zhangchuyu (10072) zhangchuyu (10076)      631 2024-04-09 01:55:19.000000 STCAT-0.3/STCAT.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      406 2024-04-09 01:53:49.000000 STCAT-0.3/STCAT.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)        1 2024-04-09 01:56:39.000000 STCAT-0.3/STCAT.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      109 2024-04-09 01:57:25.000000 STCAT-0.3/STCAT.egg-info/requires.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)        6 2024-04-09 01:53:49.000000 STCAT-0.3/STCAT.egg-info/top_level.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      116 2024-04-09 01:55:04.000000 STCAT-0.3/requirements.txt
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)       38 2024-04-09 01:56:41.000000 STCAT-0.3/setup.cfg
+-rw-rw-r--   0 zhangchuyu (10072) zhangchuyu (10076)      777 2024-04-09 01:54:18.000000 STCAT-0.3/setup.py
```

### Comparing `STCAT-0.2/PKG-INFO` & `STCAT-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: STCAT
-Version: 0.2
+Version: 0.3
 Summary: An automated T cell type annotation tool for scRNA-seq datasets.
 Home-page: https://github.com/GuoBioinfoLab/STCAT
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.19.0
 Requires-Dist: pandas>=1.0.5
 Requires-Dist: scikit-learn>=0.24.1
 Requires-Dist: openpyxl>=3.0.4
 Requires-Dist: click>=7.1.2
-Requires-Dist: scanpy>=1.7.0
+Requires-Dist: scanpy==1.9.3
 Requires-Dist: leidenalg>=0.8.3
```

### Comparing `STCAT-0.2/README.md` & `STCAT-0.3/README.md`

 * *Files identical despite different names*

### Comparing `STCAT-0.2/STCAT/STCAT.py` & `STCAT-0.3/STCAT/STCAT.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     data_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
 
     # Distinguish between T cell/non T cell
     adata.var['CD3'] = adata.var_names.isin(['CD3D','CD3E','CD3G'])
     sc.pp.calculate_qc_metrics(adata, qc_vars=['CD3'], percent_top=None, log1p=False, inplace=True)
     adata_T = adata[adata.obs.total_counts_CD3 > 0]
     adata_None_T = adata[adata.obs.total_counts_CD3 == 0]
-    adata_None_T.obs['marker_results'] = 'None_T'
+    adata_None_T.obs['Prediction'] = 'None T'
 
     logger.info(f'🧮 T cell number : {adata_T.X.shape[0]}')
     logger.info(f'🧮 None T cell number : {adata_None_T.X.shape[0]}')
     
     # pre - processing
     # Calculate the amount of CD4 expression in each cell
     adata_T.var['CD4'] = adata_T.var_names.isin(['CD4'])
@@ -42,14 +42,15 @@
         logger.info(f"💬 The input file seems not a raw count matrix.")
         
         if np.abs(np.expm1(adata_T.X[0]).sum()-10000) > 1:
             logger.info(f"❗ Invalid expression matrix, expect all genes and log1p normalized expression to 10000 counts per cell. The prediction result may not be accurate")
         else:
             logger.info(f"✔ All genes and log1p normalized expression to 10000 counts per cell.")
 
+    adata_T.X = adata_T.X.astype(np.float64)
     np.random.seed(0)
     model = os.path.join(data_path, 'T_cell.pkl')
     predictions_voting = annotate.annotate(adata_T, model = model, majority_voting = True, min_prop =0.3)
     df = predictions_voting.predicted_labels.rename(columns={'predicted_labels': 'predicted_labels_'+ str(0), 'over_clustering': 'over_clustering_' + str(0), 'majority_voting': 'majority_voting_'+ str(0)})
     adata_T.obs = pd.merge(adata_T.obs, df, how='outer', left_index=True, right_index=True)
 
     type_dict = {}
@@ -94,15 +95,15 @@
     adata_T_sub_CD8 = adata_T_sub[adata_T_sub.obs['CD4_OR_CD8'] == 'CD8']
 
 #############################################################################################################################################################################################################
     # process of CD4
     logger.info(f'⚡ Process of CD4')
     def process_CD4(q1):
         global adata_T_sub_CD4
-        if adata_T_sub_CD4.X.shape[0] != 0:
+        if adata_T_sub_CD4.X.shape[0] > 50:
             data_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
             model = os.path.join(data_path, 'cd4.pkl')
             predictions_voting = annotate.annotate(adata_T_sub_CD4, model = model, majority_voting = True, min_prop =0.3)
             df = predictions_voting.predicted_labels.rename(columns={'predicted_labels': 'predicted_labels_'+ 'CD4', 'over_clustering': 'over_clustering_' + 'CD4', 'majority_voting': 'majority_voting_'+ 'CD4'})
             adata_T_sub_CD4.obs = pd.merge(adata_T_sub_CD4.obs, df, how='outer', left_index=True, right_index=True)
 
             # rank_genes_groups
@@ -165,25 +166,33 @@
                         if max_key is not None:
                             type_dict_CD4[key] = max_key           
             for key in type_dict_CD4.keys():
                 if type_dict_CD4[key] in ['CD4 Tn', 'CD4 Tn Quiescence', 'CD4 Tn Adhesion', 'CD4 Tn IFN-Response', 'CD4 Tn Regulating'] and sum(marker in markers[key] for marker in ['CCR7', 'SELL', 'TCF7', 'LEF1']) >2:
                     continue
                 elif type_dict_CD4[key] in ['CD4 Tn', 'CD4 Tn Quiescence', 'CD4 Tn Adhesion', 'CD4 Tn IFN-Response', 'CD4 Tn Regulating'] and any(marker in markers[key] for marker in marker_CD4['CD4 Tcm']):
                     type_dict_CD4[key] = 'CD4 Tcm'
-            adata_T_sub_CD4.obs['marker_results'] = adata_T_sub_CD4.obs['over_clustering_CD4'].map(type_dict_CD4)
+            adata_T_sub_CD4.obs['Prediction'] = adata_T_sub_CD4.obs['over_clustering_CD4'].map(type_dict_CD4)
+        elif 0 < adata_T_sub_CD4.X.shape[0] <= 50:
+            data_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
+            model = os.path.join(data_path, 'cd4.pkl')
+            predictions_voting = annotate.annotate(adata_T_sub_CD4, model = model, majority_voting = True, min_prop =0.3)
+            df = predictions_voting.predicted_labels.rename(columns={'predicted_labels': 'predicted_labels_'+ 'CD4'})
+            df['predicted_labels_CD4'] = df['predicted_labels_CD4'].value_counts().idxmax()
+            adata_T_sub_CD4.obs = pd.merge(adata_T_sub_CD4.obs, df, how='outer', left_index=True, right_index=True)
+            adata_T_sub_CD4.obs['Prediction'] = adata_T_sub_CD4.obs['predicted_labels_CD4']
         else:
             adata_T_sub_CD4 = adata_T_sub_CD4
         q1.put(adata_T_sub_CD4)
         logger.info(f'✅ Process of CD4 done!')
 ##############################################################################################################################################################################################################
     # process of CD8
     logger.info(f'⚡ Process of CD8')
     def process_CD8(q2):
         global adata_T_sub_CD8    
-        if adata_T_sub_CD8.X.shape[0] != 0:
+        if adata_T_sub_CD8.X.shape[0] > 50:
             data_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
             model = os.path.join(data_path, 'cd8.pkl')
             predictions_voting = annotate.annotate(adata_T_sub_CD8, model = model, majority_voting = True, min_prop =0.3)
             df = predictions_voting.predicted_labels.rename(columns={'predicted_labels': 'predicted_labels_'+ 'CD8', 'over_clustering': 'over_clustering_' + 'CD8', 'majority_voting': 'majority_voting_'+ 'CD8'})
             adata_T_sub_CD8.obs = pd.merge(adata_T_sub_CD8.obs, df, how='outer', left_index=True, right_index=True)
 
             # rank_genes_groups
@@ -245,15 +254,23 @@
                         if max_key is not None:
                             type_dict_CD8[key] = max_key
             for key in type_dict_CD8.keys():
                 if type_dict_CD8[key] in ['CD8 Tn'] and sum(marker in markers[key] for marker in ['GZMA', 'GZMB', 'GZMK', 'GZMH','CREM', 'FAM177A1', 'LDHA', 'OAZ1', 'CMC1', 'CLDND1', 'SARAF', 'FTH1', 'TRAT1', 'MLLT3', 'GGA2', 'CYSTM1', 'DUSP2', 'CST7', 'DKK3', 'ITM2C', 'GPR183', 'TRMO', 'ATP6V0C'])>1:
                     type_dict_CD8[key] = 'CD8 Tcm'
                 elif type_dict_CD8[key] in ['CD8 Tcm'] and 'IL7R' not in markers[key]:
                     type_dict_CD8[key] = 'CD8 Tem'
-            adata_T_sub_CD8.obs['marker_results'] = adata_T_sub_CD8.obs['over_clustering_CD8'].map(type_dict_CD8)
+            adata_T_sub_CD8.obs['Prediction'] = adata_T_sub_CD8.obs['over_clustering_CD8'].map(type_dict_CD8)
+        elif 0 < adata_T_sub_CD8.X.shape[0] <= 50:
+            data_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "data")
+            model = os.path.join(data_path, 'cd8.pkl')
+            predictions_voting = annotate.annotate(adata_T_sub_CD8, model = model, majority_voting = True, min_prop =0.3)
+            df = predictions_voting.predicted_labels.rename(columns={'predicted_labels': 'predicted_labels_'+ 'CD8'})
+            df['predicted_labels_CD8'] = df['predicted_labels_CD8'].value_counts().idxmax()
+            adata_T_sub_CD8.obs = pd.merge(adata_T_sub_CD8.obs, df, how='outer', left_index=True, right_index=True)
+            adata_T_sub_CD8.obs['Prediction'] = adata_T_sub_CD8.obs['predicted_labels_CD8']
         else:
             adata_T_sub_CD8 = adata_T_sub_CD8
         q2.put(adata_T_sub_CD8)
         logger.info(f'✅ Process of CD8 done!')
 ################################################################################################################################################################## 
     def start_processes():
         q1 = Queue()
@@ -266,9 +283,9 @@
         adata_T_sub_CD8 = q2.get()
         p1.join()
         p2.join()
         return adata_T_sub_CD4, adata_T_sub_CD8
 
     adata_T_sub_CD4, adata_T_sub_CD8 = start_processes()        
     adata = sc.AnnData.concatenate(adata_None_T, adata_T_UN_D, adata_T_sub_CD4, adata_T_sub_CD8, index_unique = None)
-    logger.info(f'✅ TCAT done!')
+    logger.info(f'✅ STCAT done!')
     return adata
```

### Comparing `STCAT-0.2/STCAT/annotate.py` & `STCAT-0.3/STCAT/annotate.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.2/STCAT/classifier.py` & `STCAT-0.3/STCAT/classifier.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.2/STCAT/data/marker_CD4.txt` & `STCAT-0.3/STCAT/data/marker_CD4.txt`

 * *Files identical despite different names*

### Comparing `STCAT-0.2/STCAT/data/marker_CD8.txt` & `STCAT-0.3/STCAT/data/marker_CD8.txt`

 * *Files identical despite different names*

### Comparing `STCAT-0.2/STCAT/models.py` & `STCAT-0.3/STCAT/models.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.2/STCAT.egg-info/PKG-INFO` & `STCAT-0.3/STCAT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: STCAT
-Version: 0.2
+Version: 0.3
 Summary: An automated T cell type annotation tool for scRNA-seq datasets.
 Home-page: https://github.com/GuoBioinfoLab/STCAT
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.19.0
 Requires-Dist: pandas>=1.0.5
 Requires-Dist: scikit-learn>=0.24.1
 Requires-Dist: openpyxl>=3.0.4
 Requires-Dist: click>=7.1.2
-Requires-Dist: scanpy>=1.7.0
+Requires-Dist: scanpy==1.9.3
 Requires-Dist: leidenalg>=0.8.3
```

### Comparing `STCAT-0.2/setup.py` & `STCAT-0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import setuptools
-
-def get_requirements():
-    with open("requirements.txt", "rt", encoding="utf-8") as fh:
-        return [line.strip() for line in fh.readlines()]
-
-setuptools.setup(
-    name='STCAT',
-    version='0.2',
-    packages=setuptools.find_packages(),
-    install_requires=get_requirements(),
-    include_package_data=True,
-    python_requires='>=3.8',
-    url="https://github.com/GuoBioinfoLab/STCAT",
-    description="An automated T cell type annotation tool for scRNA-seq datasets.",
-    classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "Operating System :: POSIX :: Linux",
-        "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering :: Bio-Informatics",
-        ],
-    license="MIT"
-
-)
+import setuptools
+
+def get_requirements():
+    with open("requirements.txt", "rt", encoding="utf-8") as fh:
+        return [line.strip() for line in fh.readlines()]
+
+setuptools.setup(
+    name='STCAT',
+    version='0.3',
+    packages=setuptools.find_packages(),
+    install_requires=get_requirements(),
+    include_package_data=True,
+    python_requires='>=3.8',
+    url="https://github.com/GuoBioinfoLab/STCAT",
+    description="An automated T cell type annotation tool for scRNA-seq datasets.",
+    classifiers=[
+        "Programming Language :: Python :: 3.8",
+        "Operating System :: POSIX :: Linux",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
+        ],
+    license="MIT"
+
+)
```

