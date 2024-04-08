# Comparing `tmp/psicalc-0.5.13.tar.gz` & `tmp/psicalc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psicalc-0.5.13.tar", last modified: Sat Mar  2 19:00:12 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `psicalc-0.5.13.tar` & `psicalc-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2024-03-02 19:00:12.267904 psicalc-0.5.13/
--rw-r--r--   0 thomastownsley   (501) staff       (20)     2490 2024-03-02 19:00:12.267414 psicalc-0.5.13/PKG-INFO
--rw-r--r--   0 thomastownsley   (501) staff       (20)     1928 2024-03-02 18:23:26.000000 psicalc-0.5.13/README.md
-drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2024-03-02 19:00:12.264729 psicalc-0.5.13/psicalc/
--rw-r--r--   0 thomastownsley   (501) staff       (20)       23 2021-02-10 15:47:57.000000 psicalc-0.5.13/psicalc/__init__.py
--rw-r--r--   0 thomastownsley   (501) staff       (20)     9912 2024-03-02 18:39:59.000000 psicalc-0.5.13/psicalc/nmi.py
--rwxr-xr-x   0 thomastownsley   (501) staff       (20)    18112 2024-03-02 18:57:59.000000 psicalc-0.5.13/psicalc/psicalc.py
-drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2024-03-02 19:00:12.266985 psicalc-0.5.13/psicalc.egg-info/
--rw-r--r--   0 thomastownsley   (501) staff       (20)     2490 2024-03-02 19:00:12.000000 psicalc-0.5.13/psicalc.egg-info/PKG-INFO
--rw-r--r--   0 thomastownsley   (501) staff       (20)      226 2024-03-02 19:00:12.000000 psicalc-0.5.13/psicalc.egg-info/SOURCES.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)        1 2024-03-02 19:00:12.000000 psicalc-0.5.13/psicalc.egg-info/dependency_links.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)       20 2024-03-02 19:00:12.000000 psicalc-0.5.13/psicalc.egg-info/requires.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)        8 2024-03-02 19:00:12.000000 psicalc-0.5.13/psicalc.egg-info/top_level.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)       38 2024-03-02 19:00:12.268009 psicalc-0.5.13/setup.cfg
--rw-r--r--   0 thomastownsley   (501) staff       (20)      919 2024-03-02 19:00:06.000000 psicalc-0.5.13/setup.py
+-rw-r--r--   0        0        0    42679 2020-02-02 00:00:00.000000 psicalc-0.6.1/hist-mini.csv
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 psicalc-0.6.1/hist-test.csv
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 psicalc-0.6.1/mm.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 psicalc-0.6.1/requirements.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 psicalc-0.6.1/src/psicalc/__init__.py
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 psicalc-0.6.1/src/psicalc/nmi.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 psicalc-0.6.1/src/psicalc/nmi_util.py
+-rw-r--r--   0        0        0    19790 2020-02-02 00:00:00.000000 psicalc-0.6.1/src/psicalc/psicalc.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 psicalc-0.6.1/tests/epsilon.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 psicalc-0.6.1/utils/batch.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 psicalc-0.6.1/utils/entropy_script.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 psicalc-0.6.1/utils/multiple_msas.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 psicalc-0.6.1/utils/single_run.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 psicalc-0.6.1/.gitignore
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 psicalc-0.6.1/README.md
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 psicalc-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 psicalc-0.6.1/PKG-INFO
```

### Comparing `psicalc-0.5.13/PKG-INFO` & `psicalc-0.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: psicalc
-Version: 0.5.13
+Version: 0.6.1
 Summary: Algorithm for clustering protein multiple sequence alignments using normalized mutual information.
-Home-page: https://github.com/jdeweeselab/psicalc-package
-Author: Thomas Townsley
-Author-email: thomas@mandosoft.dev
+Project-URL: Homepage, https://github.com/jdeweeselab/psicalc-package
+Author-email: Joe Deweese Lab <jdeweeselab@gmail.com>, Thomas Townsley <thomas@mandosoft.dev>, Marc Soda <4rqh5y4p@duck.com>
 Keywords: bioinformatics
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
 
 # PSICalc Algorithm Package
 
-This is a package for clustering Multiple Sequence Alignments (MSAs) utilizing normalized mutual information to examine protein subdomains. A complete data visualization tool for psicalc is available on the releases page. 
+This is a package for clustering Multiple Sequence Alignments (MSAs) utilizing normalized mutual information to examine protein subdomains. A complete data visualization tool for psicalc is available on the releases page.
 
 As an example:
 
 ```
 import psicalc as pc
 
 file = "<your_fasta_file>" # e.g "PF02517_seed.txt"
 
 data = pc.read_txt_file_format(file) # read Fasta file
 
 data = pc.durston_schema(data, 1) # Label column index starting at 1
 
+# If you have multiple sequences or labels, merge them first
+data = pc.merge_sequences([data], ['HIST'])
+
 result = pc.find_clusters(1, data) # will sample every column against msa
 
 # Optionally write dictionary to csv
 pc.write_output_data(1, result)
 ```
 
 The program will run and return a csv or xlsx file with the strongest clusters found in the MSA provided.
 
 Our initial publication can be found here: https://academic.oup.com/bioinformaticsadvances/article/2/1/vbac058/6671262
 
-Following our initial publication, the program was found to associate invariant columns with variable columns in some cases. It was determined that the invariant columns were causing an issue, and due to their low entropy, invariant or nearly invariant positions offered little information in the way of meaningful clustering. Therefore, in the latest version (0.5.1 and beyond), we have added the ability to filter out low entropy columns using a sliding scale from 0-0.25 (0-25%) entropy where entropy is the number of different amino acids found in a column along with the number of occurrences of each amino acid. Invariant columns (i.e., those with only one amino acid) have an entropy of 0. A report of the columns removed due to low entropy is included with the output data file. 
-As a result of these changes, data run using this latest version will not match what was found in our initial paper, but should represent clusters based upon meaningful relationships. In all cases, researchers are advised to inspect the outputs to confirm the associations are meaningful. 
+Following our initial publication, the program was found to associate invariant columns with variable columns in some cases. It was determined that the invariant columns were causing an issue, and due to their low entropy, invariant or nearly invariant positions offered little information in the way of meaningful clustering. Therefore, in the latest version (0.5.1 and beyond), we have added the ability to filter out low entropy columns using a sliding scale from 0-0.25 (0-25%) entropy where entropy is the number of different amino acids found in a column along with the number of occurrences of each amino acid. Invariant columns (i.e., those with only one amino acid) have an entropy of 0. A report of the columns removed due to low entropy is included with the output data file.
+As a result of these changes, data run using this latest version will not match what was found in our initial paper, but should represent clusters based upon meaningful relationships. In all cases, researchers are advised to inspect the outputs to confirm the associations are meaningful.
```

### Comparing `psicalc-0.5.13/README.md` & `psicalc-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # PSICalc Algorithm Package
 
-This is a package for clustering Multiple Sequence Alignments (MSAs) utilizing normalized mutual information to examine protein subdomains. A complete data visualization tool for psicalc is available on the releases page. 
+This is a package for clustering Multiple Sequence Alignments (MSAs) utilizing normalized mutual information to examine protein subdomains. A complete data visualization tool for psicalc is available on the releases page.
 
 As an example:
 
 ```
 import psicalc as pc
 
 file = "<your_fasta_file>" # e.g "PF02517_seed.txt"
 
 data = pc.read_txt_file_format(file) # read Fasta file
 
 data = pc.durston_schema(data, 1) # Label column index starting at 1
 
+# If you have multiple sequences or labels, merge them first
+data = pc.merge_sequences([data], ['HIST'])
+
 result = pc.find_clusters(1, data) # will sample every column against msa
 
 # Optionally write dictionary to csv
 pc.write_output_data(1, result)
 ```
 
 The program will run and return a csv or xlsx file with the strongest clusters found in the MSA provided.
 
 Our initial publication can be found here: https://academic.oup.com/bioinformaticsadvances/article/2/1/vbac058/6671262
 
-Following our initial publication, the program was found to associate invariant columns with variable columns in some cases. It was determined that the invariant columns were causing an issue, and due to their low entropy, invariant or nearly invariant positions offered little information in the way of meaningful clustering. Therefore, in the latest version (0.5.1 and beyond), we have added the ability to filter out low entropy columns using a sliding scale from 0-0.25 (0-25%) entropy where entropy is the number of different amino acids found in a column along with the number of occurrences of each amino acid. Invariant columns (i.e., those with only one amino acid) have an entropy of 0. A report of the columns removed due to low entropy is included with the output data file. 
-As a result of these changes, data run using this latest version will not match what was found in our initial paper, but should represent clusters based upon meaningful relationships. In all cases, researchers are advised to inspect the outputs to confirm the associations are meaningful. 
+Following our initial publication, the program was found to associate invariant columns with variable columns in some cases. It was determined that the invariant columns were causing an issue, and due to their low entropy, invariant or nearly invariant positions offered little information in the way of meaningful clustering. Therefore, in the latest version (0.5.1 and beyond), we have added the ability to filter out low entropy columns using a sliding scale from 0-0.25 (0-25%) entropy where entropy is the number of different amino acids found in a column along with the number of occurrences of each amino acid. Invariant columns (i.e., those with only one amino acid) have an entropy of 0. A report of the columns removed due to low entropy is included with the output data file.
+As a result of these changes, data run using this latest version will not match what was found in our initial paper, but should represent clusters based upon meaningful relationships. In all cases, researchers are advised to inspect the outputs to confirm the associations are meaningful.
```

### Comparing `psicalc-0.5.13/psicalc/nmi.py` & `psicalc-0.6.1/src/psicalc/nmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 #              Joe Deweese, PhD. <joe.deweese@lipscomb.edu>
 #              Kirk Durston, PhD. <kirkdurston@gmail.com>
 #              Timothy Wallace, PhD. <tlwallace@lipscomb.edu>
 #              Salvador Cordova, PhD. <salvador.idcs@gmail.com>
 
 import numpy as np
 import warnings
-from math import log
+import math
 from scipy import sparse as sp
 from sklearn.utils.multiclass import type_of_target
-
 from sklearn.utils.validation import check_array, check_consistent_length
 from sklearn.utils.validation import _deprecate_positional_args
 
+EPSILON = 1e-9
+
 
 def check_clusterings(labels_true, labels_pred):
     """Check that the labels arrays are 1D and of same dimension.
     Parameters
     ----------
     labels_true : array-like of shape (n_samples,)
         The true labels.
@@ -72,17 +73,17 @@
     if eps is not None and sparse:
         raise ValueError("Cannot set 'eps' when sparse=True")
     class_gaps, cluster_gaps, both = False, False, False
     classes, class_idx = np.unique(labels_true, return_inverse=True)
     clusters, cluster_idx = np.unique(labels_pred, return_inverse=True)
     n_classes = classes.shape[0]
     n_clusters = clusters.shape[0]
-    if classes[0] == 0 : class_gaps = True
-    if clusters[0] == 0 : cluster_gaps = True
-    if class_gaps and cluster_gaps : both = True
+    if classes[0] == 0: class_gaps = True
+    if clusters[0] == 0: cluster_gaps = True
+    if class_gaps and cluster_gaps: both = True
     # Using coo_matrix to accelerate simple histogram calculation,
     # i.e. bins are consecutive integers
     # Currently, coo_matrix is faster than histogram2d for simple cases
     contingency = sp.coo_matrix((np.ones(class_idx.shape[0]),
                                  (class_idx, cluster_idx)),
                                 shape=(n_classes, n_clusters),
                                 dtype=dtype)
@@ -148,16 +149,16 @@
     pi = np.ravel(contingency.sum(axis=1))
     pj = np.ravel(contingency.sum(axis=0))
     log_contingency_nm = np.log(nz_val)
     contingency_nm = nz_val / contingency_sum
     # Don't need to calculate the full outer product, just for non-zeroes
     outer = (pi.take(nzx).astype(np.int64, copy=False)
              * pj.take(nzy).astype(np.int64, copy=False))
-    log_outer = -np.log(outer) + log(pi.sum()) + log(pj.sum())
-    mi = (contingency_nm * (log_contingency_nm - log(contingency_sum)) +
+    log_outer = -np.log(outer) + math.log(pi.sum()) + math.log(pj.sum())
+    mi = (contingency_nm * (log_contingency_nm - math.log(contingency_sum)) +
           contingency_nm * log_outer)
     mi = np.where(np.abs(mi) < np.finfo(mi.dtype).eps, 0.0, mi)
 
     return np.clip(mi.sum(), 0.0, None)
 
 
 def entropy(labels):
@@ -177,15 +178,15 @@
     pi = pi[pi > 0]
     if pi.size == 0:
         return 0.0
     pi_sum = np.sum(pi)
 
     # log(a / b) should be calculated as log(a) - log(b) for
     # possible loss of precision
-    return -np.sum((pi / pi_sum) * (np.log(pi) - log(pi_sum)))
+    return -np.sum((pi / pi_sum) * (np.log(pi) - math.log(pi_sum)))
 
 
 def _generalized_average(U, V, average_method):
     """Return a particular mean of two numbers."""
     if average_method == "min":
         return min(U, V)
     elif average_method == "geometric":
@@ -197,15 +198,16 @@
     else:
         raise ValueError("'average_method' must be 'min', 'geometric', "
                          "'arithmetic', or 'max'")
 
 
 @_deprecate_positional_args
 def normalized_mutual_info_score(labels_true, labels_pred, *,
-                                 average_method='geometric'):
+                                 average_method='geometric',
+                                 _use_esp=False):
     """
     This is the core function of the library originally from Pedregosa/sci-kit
     but we've introduced modifications to handle problems associated with MSAs:
 
     1. MSAs contain labels we are not interested in, that is gaps. These are
     handled both in the entropy and the contingency matrix functions. The reason
     we do not simply discard gaps is that some calculations like mutual information
@@ -231,25 +233,28 @@
             return 0.0
         else:
             return 1.0
 
     contingency = contingency_matrix(labels_true, labels_pred, sparse=True)
     contingency = contingency.astype(np.float64, copy=False)
 
-
     # Calculate the MI for the two clusterings
     mi = mutual_info_score(labels_true, labels_pred,
                            contingency=contingency)
 
     # Calculate the expected value for the mutual information
     # Calculate entropy for each labeling
     h_true, h_pred = entropy(labels_true), entropy(labels_pred)
     normalizer = _generalized_average(h_true, h_pred, average_method)
     # Avoid 0.0 / 0.0 when either entropy is zero.
     normalizer = max(normalizer, np.finfo('float64').eps)
     nmi = mi / normalizer
     # Avoid problems associated with low entropy regions
     # not normalizing correctly
-    if nmi > 1.0:
-        nmi = 0.0
+    if _use_esp:  # XXX: Temp for testing
+        if nmi > 1.0 and not math.isclose(nmi, 1.0, rel_tol=EPSILON):
+            nmi = 0.0
+    else:
+        if nmi > 1.0:
+            nmi = 0.0
 
     return nmi
```

### Comparing `psicalc-0.5.13/psicalc/psicalc.py` & `psicalc-0.6.1/src/psicalc/psicalc.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,22 +21,26 @@
 
 Contact: thomas@mandosoft.dev, joe.deweese@lipscomb.edu, kirkdurston@gmail.com
 """
 import sys
 import re
 import time
 import csv
-import warnings
 import pandas as pd
 import numpy as np
-from itertools import combinations, filterfalse
-from .nmi import normalized_mutual_info_score as nmis
-from .nmi import entropy
-
-warnings.filterwarnings("ignore", category=pd.errors.DtypeWarning)
+from itertools import combinations
+from .nmi import normalized_mutual_info_score, entropy, EPSILON
+import psicalc.nmi_util as nmi_util
+
+pd.DataFrame.iteritems = pd.DataFrame.items
+pd.set_option('future.no_silent_downcasting', True)
+
+halt = False
+nmi_util.EPSILON = EPSILON
+nmi_cache = nmi_util.NmiCache(normalized_mutual_info_score)
 
 
 def select_subset(c_list: list, s: int):
     """Selects the width of the sample subset from the MSA"""
     each_nth_col = c_list[::s]
     return each_nth_col
 
@@ -130,15 +134,15 @@
     df.fillna('?', inplace=True)
 
     return df
 
 
 def read_csv_file_format(file) -> pd.DataFrame:
     """Reads CSV MSAs into a dataframe."""
-    df = pd.read_csv(file, encoding='utf-8', engine='c', header=None)
+    df = pd.read_csv(file, encoding='utf-8', header=None, dtype=str)
     df = df.rename(columns={df.columns[0]: 'SEQUENCE_ID'})
     df = df.set_index('SEQUENCE_ID', drop=True)
     df = check_for_duplicates(df)
     df.fillna('?', inplace=True)
 
     if df.index[0] == "Domain: Data":
         df.drop(index=["Domain: Data"], inplace=True)
@@ -151,15 +155,16 @@
     """Calculates the sr_mode and new mode of a cluster and returns both."""
     cc = len(list(combinations(c, 2)))
     if len(c) < 2:
         sr_mode, new_mode = None, None
         return sr_mode, new_mode
     elif len(c) == 2:
         i, j = m_map.get(c[0]), m_map.get(c[1])
-        max_sum = nmis(msa[:, i], msa[:, j], average_method='geometric')
+        max_sum = nmi_cache.get(i, j, msa)
+
         new_mode = c
         """
         if max_sum > 1.0:
             print("\nERROR: Score returned greater than 1.0: ")
             print(c, max_sum)
             exit(1)
         """
@@ -167,25 +172,30 @@
         A = [[column, []] for column in range(len(c))]
         D = len(A)
         shift = 0
         for loc, i in enumerate(c):
             for location, j in enumerate(c):
                 if location != loc and location > shift:
                     l, r = m_map.get(i), m_map.get(j)
-                    A[loc][1].append(nmis(msa[:, l], msa[:, r], average_method='geometric'))
+                    A[loc][1].append(nmi_cache.get(l, r, msa))
             t = loc
             q = loc + 1
             if q != D:
                 while q != D:
                     A[q][1].append(A[loc][1][t])
                     q += 1
                     t += 1
                 shift += 1
 
-        mode_map = np.array([np.sum(v) for (k, v) in A], dtype='d')
+        # XXX: Temp for test
+        if nmi_cache._use_esp:
+            mode_map = np.array([np.sum([item.value for item in v]) for (k, v) in A], dtype='d')
+        else:
+            mode_map = np.array([np.sum(v) for (k, v) in A], dtype='d')
+
         mode_loc = int(np.argmax(mode_map))
         max_sum = np.amax(mode_map)
         new_mode = return_new_mode(mode_loc, c)
 
     sr_mode = max_sum / cc
     if k == "pairwise" or k == "top-pairwise":
         list_store.append([sr_mode, new_mode])
@@ -254,15 +264,15 @@
     return filename
 
 
 def get_unique_elements(df: pd.DataFrame) -> np.ndarray:
     """Returns all unique elements found in a multiple
     sequence alignment."""
     U = np.array([])
-    for name, seq in df.items():
+    for name, seq in df.iteritems():
         U = np.append(U, seq.unique())
 
     return np.unique(U)
 
 
 def rectify_sequences(df: pd.DataFrame) -> pd.DataFrame:
     """Corrects symbols in the multiple sequence alignment."""
@@ -349,90 +359,143 @@
     return
 
 
 def signal_halt() -> bool:
     """Gets the state of the halt global variable. Allows for termination
     of long running process in a safe manner."""
 
-    return halt
+    global halt
+    if halt:
+        halt = False
+        return True
+
+    return False
 
 
 def calculate_time(start):
     """Calculate time taken for program execution."""
     print("\n\n--- took " + str(round((time.time() - start), 3)) + " seconds ---")
 
     return
 
 
-def find_clusters(spread: int, df: pd.DataFrame, k="pairwise", e=0.0) -> dict:
+def merge_sequences(data: [pd.DataFrame], labels: [str]) -> pd.DataFrame:
+    """
+    Combine `data` into one big MSA and fill gaps due to dimension mismatch with
+    '-'. Ignores mismatched indices. Loses row indices
+    """
+
+    # Rename columns with provided names unless there's only one MSA and no name
+    # is provided.
+    if len(labels) > 0:
+        assert len(data) == len(labels), "MSA names != MSA columns"
+        for i in range(len(data)):
+            data[i] = data[i].rename(columns=lambda x: labels[i] + str(x))
+
+    data = [d.reset_index(drop=True) for d in data]
+    data = pd.concat(data, axis=1)
+    data = data.fillna('-')
+    return data
+
+
+def prepare_data(data: pd.DataFrame) -> (np.ndarray, dict):
+    """
+    Prepares MSA data for clustering. Returns the encoded MSA and a mapping of the
+    column indices to labels.
+    """
+
+    print("\nEncoding MSA(s)...")
+    msa = encode_msa(data)
+
+    # Create a mapping of column indices to names
+    col_names = data.columns.tolist()
+    col_indices = list(range(msa.shape[1]))
+    col_map = dict(zip(col_indices, col_names))
+
+    return msa, col_map
+
+
+def filter_entropy(msa: np.ndarray, column_map: dict, e: float) -> (np.ndarray, list, list):
+    """
+    Filters all columns of `msa` with entropy lower than `e`. Returns the filtered msa and lists
+    of included and filtered msa column names.
+    """
+
+    num_columns = msa.shape[1]
+
+    # Create lists of low entropy names and column indices, plus interesting msa column names
+    low_entropy_sites = []
+    low_entropy_columns = []
+    msa_names = []
+    for idx in range(num_columns):
+        if entropy(msa[:, idx]) < e:
+            low_entropy_columns.append(idx)
+            low_entropy_sites.append(column_map[idx])
+        else:
+            msa_names.append(column_map[idx])
+
+    # Create a new matrix without the low entropy regions
+    msa = np.delete(msa, low_entropy_columns, axis=1)
+
+    return msa, msa_names, low_entropy_sites
+
+
+def find_clusters(spread: int, msa: pd.DataFrame, k="pairwise", e=0.0, _use_esp=False) -> dict:
     """
     Discovers cluster sites with high shared normalized mutual information.
     Provide a dataframe and a sample spread-width. Returns a dictionary.
 
     The variable k by default is set to 'pairwise' to look for pairwise clusters
     and aggregate them prior to running Phase 2. Users may also set k to 'pairwise_only'
     if they only want to output pairwise clusters without aggregating them, in which
     case the program will halt once all pairwise clusters are found. This may be useful
     when comparing to methods like DCA.
 
     By default "e" or entropy is set to 0 but may be adjusted to exclude low entropy sites from
     being run in the program.
     """
 
-    print("\nEncoding MSA. This may take a while.")
-
     global halt
     halt = False
     csv_dict = dict()
     start_time = time.time()
     hash_list = list()
 
-    msa_col_list = df.columns.tolist()
-    num_msx = encode_msa(df)
-    num_columns = num_msx.shape[1]
-    encoded_col_list = list(range(num_columns))
-    mapping = dict(zip(msa_col_list, encoded_col_list))
-
-    # Calculate entropy for each column and filter
-    low_entropy_columns = [col_index for col_index in range(num_columns)
-                           if entropy(num_msx[:, col_index]) < e]
-
-    # What will be returned in the data output
-    low_entropy_results = [col_name for col_name in msa_col_list
-                           if mapping[col_name] in low_entropy_columns]
-
-    csv_dict["low_entropy_sites"] = low_entropy_results
-
-    # Create a new msa_index list without values corresponding to low entropy columns
-    msa_index = [col_name for col_name in msa_col_list
-                 if mapping[col_name] not in low_entropy_columns]
-
-    # Create a new matrix without the low entropy regions
-    num_msa = np.delete(num_msx, low_entropy_columns, axis=1)
+    #XXX: Temp for testing
+    global nmi_cache
+    nmi_cache = nmi_util.NmiCache(normalized_mutual_info_score, _use_esp)
+
+    # Map labels to columns
+    msa, column_map = prepare_data(msa.copy(deep=True))
+    csv_dict["column_map"] = column_map
+
+    # Filter low entropy sites
+    num_msa, msa_attrs, low_entropy_sites = filter_entropy(msa, column_map, e)
+    print("\nNumber of low entropy regions excluded: ", len(low_entropy_sites))
+    csv_dict["low_entropy_sites"] = low_entropy_sites
 
-    print("\nNumber of low entropy regions excluded: ", len(low_entropy_results))
-    msa_map = {k: v for v, k in enumerate(msa_index)}
-    subset = select_subset(msa_index, spread)
+    msa_map = {k: v for v, k in enumerate(msa_attrs)}
+    subset = select_subset(msa_attrs, spread)
     subset_list = [[z] for z in subset]
 
     print("\nLooking for strong pairwise clusters...")
     for item, each in enumerate(subset_list):
         max_rii, best_cluster = 0.0, None
-        for location, cluster in enumerate(msa_index):
+        for location, cluster in enumerate(msa_attrs):
             cluster_mode = msa_map.get(cluster)
             subset_mode = msa_map.get(each[0])
 
             if subset_mode != cluster_mode:
-                rii = nmis(num_msa[:, subset_mode], num_msa[:, cluster_mode], average_method='geometric')
+                rii = nmi_cache.get(subset_mode, cluster_mode, num_msa)
                 if rii > max_rii:
                     max_rii, best_cluster = rii, location
         if best_cluster is None:
             continue
         else:
-            subset_list[item].append(msa_index[best_cluster])
+            subset_list[item].append(msa_attrs[best_cluster])
             print("pair located: ", subset_list[item])
 
     pair_list = [x for x in subset_list if len(x) > 1]
 
     for cluster in pair_list:
         return_sr_mode(num_msa, msa_map, cluster, csv_dict, hash_list, k)
 
@@ -455,57 +518,61 @@
         return_sr_mode(num_msa, msa_map, cluster, csv_dict, unranked, k)
 
     C = sorted(unranked, key=lambda x: x[0], reverse=True)
 
     for x, j in C:
         for col in j:
             try:
-                msa_index.remove(col)
+                msa_attrs.remove(col)
             except ValueError:
                 print("\nFAILED: Tried to remove site location ", col, "but it was not found.\n"
-                       "This is likely due to duplicates not being removed during check_intersections().")
+                      "This is likely due to duplicates not being removed during check_intersections().")
                 sys.exit()
 
-    if len(msa_index) == 0:
+    if len(msa_attrs) == 0:
         calculate_time(start_time)
         return csv_dict
 
     print("\nTop ranked clusters:")
     num = 0
     for each in C:
         num += 1
         print(num, ": ", each[1])
 
     # Sets the number of clusters we're actually iterating over
     R = len(C)
-    for remaining in msa_index:
+    for remaining in msa_attrs:
         C.append([0, [remaining]])
     num_clusters = len(C[0:R])
     cluster_halt = 0
 
     # Stage Two: Move through the pairs in the list and finds their best attribute
     try:
         while len(C) >= 1:
 
-            if signal_halt(): break
+            if signal_halt():
+                break
+
             print("\n --> Total Remaining ", len(C))
 
             i = 0
             while i < num_clusters:
 
-                if signal_halt(): break
+                if signal_halt():
+                    break
+
                 location = None
                 cluster_mode = msa_map.get(C[i][1][0])
                 max_rii, best_cluster = 0.0, None
 
                 for loc, entry in enumerate(C):
                     cluster = entry[1]
                     attr_mode = msa_map.get(cluster[0])
                     if cluster_mode != attr_mode:
-                        rii = nmis(num_msa[:, attr_mode], num_msa[:, cluster_mode], average_method='geometric')
+                        rii = nmi_cache.get(attr_mode, cluster_mode, num_msa)
                         if rii > max_rii:
                             max_rii, best_cluster, location = rii, cluster, loc
 
                 if best_cluster is None:
                     i += 1
                     cluster_halt += 1
 
@@ -529,9 +596,10 @@
                 break
 
     except KeyboardInterrupt:
         return_dict_state()
 
     calculate_time(start_time)
     halt = False
+    nmi_cache.clear()
 
     return csv_dict
```

