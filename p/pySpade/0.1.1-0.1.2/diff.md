# Comparing `tmp/pySpade-0.1.1.tar.gz` & `tmp/pySpade-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pySpade-0.1.1.tar", last modified: Thu Apr  4 18:03:43 2024, max compression
+gzip compressed data, was "dist/pySpade-0.1.2.tar", last modified: Tue Apr  9 16:35:36 2024, max compression
```

## Comparing `pySpade-0.1.1.tar` & `pySpade-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-04 18:03:43.000000 pySpade-0.1.1/
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     1066 2022-09-29 20:16:43.000000 pySpade-0.1.1/LICENSE
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:49:13.000000 pySpade-0.1.1/MANIFEST.in
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-04-04 18:03:43.000000 pySpade-0.1.1/PKG-INFO
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15114 2024-04-04 17:56:05.000000 pySpade-0.1.1/README.md
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-04 18:03:43.000000 pySpade-0.1.1/pySpade/
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-03-21 19:46:56.000000 pySpade-0.1.1/pySpade/DEobs.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     5923 2023-10-30 17:50:45.000000 pySpade-0.1.1/pySpade/DEobsboot.py
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)    12308 2024-03-22 14:30:27.000000 pySpade-0.1.1/pySpade/DErand.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)       36 2024-03-26 21:08:55.000000 pySpade-0.1.1/pySpade/__init__.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     4342 2024-03-21 19:58:28.000000 pySpade-0.1.1/pySpade/__main__.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     2906 2024-01-12 23:46:21.000000 pySpade-0.1.1/pySpade/explevel.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     8198 2024-01-26 01:38:44.000000 pySpade-0.1.1/pySpade/fc.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9465 2024-02-21 19:40:48.000000 pySpade-0.1.1/pySpade/global.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    10315 2024-04-02 16:51:22.000000 pySpade-0.1.1/pySpade/local.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9590 2024-03-26 21:54:47.000000 pySpade-0.1.1/pySpade/manhattan.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    18929 2024-03-25 18:10:56.000000 pySpade-0.1.1/pySpade/parsers.py
--rwxr-----   0 s426305  (426305) Hon_lab   (7001)  2242597 2024-01-26 16:44:04.000000 pySpade-0.1.1/pySpade/plot_annotation.txt
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-01-12 23:45:43.000000 pySpade-0.1.1/pySpade/process.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    14874 2024-03-21 18:32:24.000000 pySpade-0.1.1/pySpade/utils.py
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-04 18:03:43.000000 pySpade-0.1.1/pySpade.egg-info/
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/PKG-INFO
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)      465 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/SOURCES.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        1 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/dependency_links.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       51 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/entry_points.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        8 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/top_level.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       38 2024-04-04 18:03:43.000000 pySpade-0.1.1/setup.cfg
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)      987 2023-06-30 19:38:59.000000 pySpade-0.1.1/setup.py
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-09 16:35:36.000000 pySpade-0.1.2/
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     1066 2022-09-29 20:16:43.000000 pySpade-0.1.2/LICENSE
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:49:13.000000 pySpade-0.1.2/MANIFEST.in
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-04-09 16:35:36.000000 pySpade-0.1.2/PKG-INFO
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15114 2024-04-09 16:27:37.000000 pySpade-0.1.2/README.md
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade/
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-03-21 19:46:56.000000 pySpade-0.1.2/pySpade/DEobs.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     5923 2023-10-30 17:50:45.000000 pySpade-0.1.2/pySpade/DEobsboot.py
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)    12310 2024-04-04 18:35:58.000000 pySpade-0.1.2/pySpade/DErand.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)       36 2024-04-09 16:26:57.000000 pySpade-0.1.2/pySpade/__init__.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     4342 2024-03-21 19:58:28.000000 pySpade-0.1.2/pySpade/__main__.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     2906 2024-01-12 23:46:21.000000 pySpade-0.1.2/pySpade/explevel.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     8198 2024-01-26 01:38:44.000000 pySpade-0.1.2/pySpade/fc.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9465 2024-02-21 19:40:48.000000 pySpade-0.1.2/pySpade/global.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    10315 2024-04-02 16:51:22.000000 pySpade-0.1.2/pySpade/local.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9588 2024-04-09 16:35:35.000000 pySpade-0.1.2/pySpade/manhattan.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    18930 2024-04-09 16:27:59.000000 pySpade-0.1.2/pySpade/parsers.py
+-rwxr-----   0 s426305  (426305) Hon_lab   (7001)  2242597 2024-01-26 16:44:04.000000 pySpade-0.1.2/pySpade/plot_annotation.txt
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-01-12 23:45:43.000000 pySpade-0.1.2/pySpade/process.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    14874 2024-03-21 18:32:24.000000 pySpade-0.1.2/pySpade/utils.py
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade.egg-info/
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade.egg-info/PKG-INFO
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)      465 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade.egg-info/SOURCES.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        1 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade.egg-info/dependency_links.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       51 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade.egg-info/entry_points.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        8 2024-04-09 16:35:36.000000 pySpade-0.1.2/pySpade.egg-info/top_level.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       38 2024-04-09 16:35:36.000000 pySpade-0.1.2/setup.cfg
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)      987 2023-06-30 19:38:59.000000 pySpade-0.1.2/setup.py
```

### Comparing `pySpade-0.1.1/LICENSE` & `pySpade-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/PKG-INFO` & `pySpade-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySpade
-Version: 0.1.1
+Version: 0.1.2
 Summary: Single cell Perturbations - Analysis of Differential gene Expression
 Home-page: https://github.com/Hon-lab/pySpade
 Author: Yihan Wang
 Author-email: Yihan.Wang@UTSouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ## Usage
 ________
 ```
 $pySpade
 usage: pySpade [-h]  ...
 
 pySpade 
-Version: 0.1.1
+Version: 0.1.2
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
     process   process mapping output and reformat for downstream analysis.
```

### Comparing `pySpade-0.1.1/README.md` & `pySpade-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ## Usage
 ________
 ```
 $pySpade
 usage: pySpade [-h]  ...
 
 pySpade 
-Version: 0.1.1
+Version: 0.1.2
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
     process   process mapping output and reformat for downstream analysis.
```

### Comparing `pySpade-0.1.1/pySpade/DEobs.py` & `pySpade-0.1.2/pySpade/DEobs.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/DEobsboot.py` & `pySpade-0.1.2/pySpade/DEobsboot.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/DErand.py` & `pySpade-0.1.2/pySpade/DErand.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,28 +248,28 @@
     
     logger.info('Process up-regulation.')
     for i in idx:
         if (i % 10000 == 0):
             logger.info('Finished ' + str(i) + ' genes.')
 
         up_array = -np.array(up_pval_matrix.tocsr()[:, i].todense()).flatten()    
-        if np.sum(np.isfinite(up_array)) <= 3:
+        if np.sum(np.isfinite(up_array)) <= 10:
             continue
         a, b, c = stats.gamma.fit(up_array[np.isfinite(up_array)])
         A[i] = a 
         B[i] = b
         C[i] = c
 
     logger.info('Process down-regulation.')
     for i in idx:
         if (i % 10000 == 0):
             logger.info('Finished ' + str(i) + ' genes.')
 
         down_array = -np.array(down_pval_matrix.tocsr()[:, i].todense()).flatten()
-        if np.sum(np.isfinite(down_array)) <= 3:
+        if np.sum(np.isfinite(down_array)) <= 10:
             continue
         d, e, f = stats.gamma.fit(down_array[np.isfinite(down_array)])
         D[i] = d
         E[i] = e
         F[i] = f
 
     #save the parameters of gamma distribution
```

### Comparing `pySpade-0.1.1/pySpade/__main__.py` & `pySpade-0.1.2/pySpade/__main__.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/explevel.py` & `pySpade-0.1.2/pySpade/explevel.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/fc.py` & `pySpade-0.1.2/pySpade/fc.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/global.py` & `pySpade-0.1.2/pySpade/global.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/local.py` & `pySpade-0.1.2/pySpade/local.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/manhattan.py` & `pySpade-0.1.2/pySpade/manhattan.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             xtick_pos = np.append(xtick_pos, chrom_midpoint)
 
         print_ChrNames = np.array([])
         for i in chr_order:
             print_ChrNames = np.append(print_ChrNames, i[:1].upper() + i[1:])
 
         ax0.set_xticklabels(print_ChrNames, 
-                            rotation='60',
+                            rotation=60,
                             va='top',
                             ha='center',
                             style='oblique',
                             family='monospace')
 
         for i,e in enumerate(length_list):
             if i == 0:
```

### Comparing `pySpade-0.1.1/pySpade/parsers.py` & `pySpade-0.1.2/pySpade/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
     
     parser.add_argument('-cs', 
                         '--cutoff_significance', 
                         dest='cutoff_significance', 
                         required=False,
                         type=float,
                         default=-5,
-                        help='specify the cutoff of Significance_scpre. Default is -5 (Significance score is smaller than -5)')
+                        help='specify the cutoff of Significance_score. Default is -5 (Significance score is smaller than -5)')
     
     parser.add_argument('-o', 
                         '--output_folder', 
                         dest='output_folder', 
                         required=True,
                         type=str,
-                        help='specify an output folder directory.')
+                        help='specify an output folder directory.')
```

### Comparing `pySpade-0.1.1/pySpade/plot_annotation.txt` & `pySpade-0.1.2/pySpade/plot_annotation.txt`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/process.py` & `pySpade-0.1.2/pySpade/process.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade/utils.py` & `pySpade-0.1.2/pySpade/utils.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.1/pySpade.egg-info/PKG-INFO` & `pySpade-0.1.2/pySpade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySpade
-Version: 0.1.1
+Version: 0.1.2
 Summary: Single cell Perturbations - Analysis of Differential gene Expression
 Home-page: https://github.com/Hon-lab/pySpade
 Author: Yihan Wang
 Author-email: Yihan.Wang@UTSouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ## Usage
 ________
 ```
 $pySpade
 usage: pySpade [-h]  ...
 
 pySpade 
-Version: 0.1.1
+Version: 0.1.2
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
     process   process mapping output and reformat for downstream analysis.
```

### Comparing `pySpade-0.1.1/setup.py` & `pySpade-0.1.2/setup.py`

 * *Files identical despite different names*

