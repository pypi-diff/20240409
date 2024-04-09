# Comparing `tmp/dictlearn-0.2.1.tar.gz` & `tmp/dictlearn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictlearn-0.2.1.tar", last modified: Fri Mar 25 16:05:35 2022, max compression
+gzip compressed data, was "dictlearn-0.2.2.tar", last modified: Tue Apr  9 10:28:10 2024, max compression
```

## Comparing `dictlearn-0.2.1.tar` & `dictlearn-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,60 @@
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      899 2021-12-13 13:05:54.000000 dictlearn-0.2.1/LICENSE
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1402 2022-03-25 16:05:35.787997 dictlearn-0.2.1/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      696 2021-12-13 13:05:54.000000 dictlearn-0.2.1/README.md
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      103 2021-12-13 13:05:54.000000 dictlearn-0.2.1/pyproject.toml
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      832 2022-03-25 16:05:35.787997 dictlearn-0.2.1/setup.cfg
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/dictlearn/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      213 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/__init__.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    27628 2022-03-25 15:48:16.000000 dictlearn-0.2.1/src/dictlearn/_dictionary_learning.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4770 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/_utils.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/dictlearn/datasets/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/datasets/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      920 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/datasets/arface.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      935 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/datasets/caltech101.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      915 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/datasets/mnist.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      915 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/datasets/yaleb.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12100 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/kernel_approximation.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      244 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/kernels.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/dictlearn/methods/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      968 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/__init__.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     5145 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_aksvd.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9482 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_atom.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    11293 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_ksvd.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     2019 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_mod.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    10091 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_nsgk.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1509 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_odl.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     4260 2022-03-25 14:02:57.000000 dictlearn-0.2.1/src/dictlearn/methods/_omp.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5107 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_sgk.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     5949 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/methods/_uaksvd.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/dictlearn/models/
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     6859 2022-03-25 14:02:57.000000 dictlearn-0.2.1/src/dictlearn/models/DDL.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     6211 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/models/DPL.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7986 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/models/KDDL.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8354 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/models/KDPL.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    10262 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/models/KLCDL.py
--rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    11142 2022-03-25 14:02:57.000000 dictlearn-0.2.1/src/dictlearn/models/LCDL.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      135 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/models/__init__.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/dictlearn/utils/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/utils/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25556 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/utils/data_utils.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    21585 2021-12-13 13:05:54.000000 dictlearn-0.2.1/src/dictlearn/utils/generic_utils.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2022-03-25 16:05:35.787997 dictlearn-0.2.1/src/dictlearn.egg-info/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1402 2022-03-25 16:05:35.000000 dictlearn-0.2.1/src/dictlearn.egg-info/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1167 2022-03-25 16:05:35.000000 dictlearn-0.2.1/src/dictlearn.egg-info/SOURCES.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2022-03-25 16:05:35.000000 dictlearn-0.2.1/src/dictlearn.egg-info/dependency_links.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       12 2022-03-25 16:05:35.000000 dictlearn-0.2.1/src/dictlearn.egg-info/requires.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       10 2022-03-25 16:05:35.000000 dictlearn-0.2.1/src/dictlearn.egg-info/top_level.txt
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.737747 dictlearn-0.2.2/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      899 2024-02-25 19:11:12.000000 dictlearn-0.2.2/LICENSE
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3821 2024-04-09 10:28:10.737747 dictlearn-0.2.2/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3110 2024-02-25 19:11:12.000000 dictlearn-0.2.2/README.md
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      103 2024-02-25 19:11:12.000000 dictlearn-0.2.2/pyproject.toml
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      832 2024-04-09 10:28:10.737747 dictlearn-0.2.2/setup.cfg
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.734413 dictlearn-0.2.2/src/
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.734413 dictlearn-0.2.2/src/dictlearn/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      213 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/__init__.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    27728 2024-04-09 10:21:39.000000 dictlearn-0.2.2/src/dictlearn/_dictionary_learning.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4770 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/_utils.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.734413 dictlearn-0.2.2/src/dictlearn/datasets/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/datasets/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      920 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/datasets/arface.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      935 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/datasets/caltech101.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      915 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/datasets/mnist.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      915 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/datasets/yaleb.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12100 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/kernel_approximation.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      244 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/kernels.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.734413 dictlearn-0.2.2/src/dictlearn/methods/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      968 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/__init__.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     5145 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_aksvd.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9482 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_atom.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    11293 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_ksvd.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     2019 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_mod.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    10091 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_nsgk.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1509 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_odl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     4260 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_omp.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5107 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_sgk.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     5949 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/methods/_uaksvd.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.737747 dictlearn-0.2.2/src/dictlearn/models/
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     6859 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/DDL.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     6211 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/DPL.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7986 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/KDDL.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8354 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/KDPL.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    10262 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/KLCDL.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    11142 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/LCDL.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      135 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/models/__init__.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.737747 dictlearn-0.2.2/src/dictlearn/utils/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/utils/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25556 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/utils/data_utils.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    21585 2024-02-25 19:11:12.000000 dictlearn-0.2.2/src/dictlearn/utils/generic_utils.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.737747 dictlearn-0.2.2/src/dictlearn.egg-info/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3821 2024-04-09 10:28:10.000000 dictlearn-0.2.2/src/dictlearn.egg-info/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1389 2024-04-09 10:28:10.000000 dictlearn-0.2.2/src/dictlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2024-04-09 10:28:10.000000 dictlearn-0.2.2/src/dictlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       12 2024-04-09 10:28:10.000000 dictlearn-0.2.2/src/dictlearn.egg-info/requires.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       10 2024-04-09 10:28:10.000000 dictlearn-0.2.2/src/dictlearn.egg-info/top_level.txt
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2024-04-09 10:28:10.737747 dictlearn-0.2.2/tests/
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)      624 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_ddl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     1217 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_dl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     1479 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_dl_all.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)      608 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_dpl.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      685 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_kddl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     1221 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_kdl.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      762 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_kdpl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)    10839 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_kernel_approximation.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      766 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_klcdl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)      711 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_lcdl.py
+-rwxr-xr-x   0 pirofti   (1000) pirofti   (1000)     1217 2024-02-25 19:11:12.000000 dictlearn-0.2.2/tests/test_odl.py
```

### Comparing `dictlearn-0.2.1/LICENSE` & `dictlearn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/setup.cfg` & `dictlearn-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dictlearn
-version = 0.2.1
+version = 0.2.2
 author = Paul Irofti, Denis Ilie-Ablachim, Bogdan Dumitrescu
 author_email = graphomaly@fmi.unibuc.ro
 description = Dictionary Learning Toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = dictionary learning, sparse representations, machine learning, signal processing
 url = https://gitlab.com/unibuc/graphomaly/dictionary-learning
```

### Comparing `dictlearn-0.2.1/src/dictlearn/_dictionary_learning.py` & `dictlearn-0.2.2/src/dictlearn/_dictionary_learning.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         The sparse representations matrix
 
     err : float
       The approximation error
     """
 
     n_features, n_samples = Y.shape
-    n_components = D.shape[0]
+    n_components = D.shape[1]
 
     if algorithm in ("omp"):
         if n_nonzero_coefs is None:
             n_nonzero_coefs = min(max(n_features / 10, 1), n_components)
 
     X, error = _sparse_encode(
         Y,
@@ -409,15 +409,19 @@
     rmse = np.zeros(max_iter)
     error_extra = np.zeros(max_iter)
 
     # Safe initialization of params
     _safe_params_init(params, fit_algorithm.__name__)
 
     # Initialize kernel matrix
-    K = kernel_function(Y, Y, params)
+    # K = kernel_function(Y, Y, params)
+    if "K" in params:
+        K = params["K"]
+    else:
+        K = kernel_function(Y, Y, params)
 
     # Initialize coding coefs
     if transform_algorithm is not None:
         X, _ = sparse_encode(A.T @ K, A.T @ K @ A, transform_algorithm, n_nonzero_coefs)
 
     for iter in range(max_iter):
         # Update dictionary
```

### Comparing `dictlearn-0.2.1/src/dictlearn/_utils.py` & `dictlearn-0.2.2/src/dictlearn/_utils.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/datasets/arface.py` & `dictlearn-0.2.2/src/dictlearn/datasets/arface.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/datasets/caltech101.py` & `dictlearn-0.2.2/src/dictlearn/datasets/caltech101.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/datasets/mnist.py` & `dictlearn-0.2.2/src/dictlearn/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/datasets/yaleb.py` & `dictlearn-0.2.2/src/dictlearn/datasets/yaleb.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/kernel_approximation.py` & `dictlearn-0.2.2/src/dictlearn/kernel_approximation.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/__init__.py` & `dictlearn-0.2.2/src/dictlearn/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_aksvd.py` & `dictlearn-0.2.2/src/dictlearn/methods/_aksvd.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_atom.py` & `dictlearn-0.2.2/src/dictlearn/methods/_atom.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_ksvd.py` & `dictlearn-0.2.2/src/dictlearn/methods/_ksvd.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_mod.py` & `dictlearn-0.2.2/src/dictlearn/methods/_mod.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_nsgk.py` & `dictlearn-0.2.2/src/dictlearn/methods/_nsgk.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_odl.py` & `dictlearn-0.2.2/src/dictlearn/methods/_odl.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_omp.py` & `dictlearn-0.2.2/src/dictlearn/methods/_omp.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_sgk.py` & `dictlearn-0.2.2/src/dictlearn/methods/_sgk.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/methods/_uaksvd.py` & `dictlearn-0.2.2/src/dictlearn/methods/_uaksvd.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/models/DDL.py` & `dictlearn-0.2.2/src/dictlearn/models/DDL.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/models/DPL.py` & `dictlearn-0.2.2/src/dictlearn/models/DPL.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/models/KDDL.py` & `dictlearn-0.2.2/src/dictlearn/models/KDDL.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/models/KDPL.py` & `dictlearn-0.2.2/src/dictlearn/models/KDPL.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/models/KLCDL.py` & `dictlearn-0.2.2/src/dictlearn/models/KLCDL.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/models/LCDL.py` & `dictlearn-0.2.2/src/dictlearn/models/LCDL.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/utils/data_utils.py` & `dictlearn-0.2.2/src/dictlearn/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn/utils/generic_utils.py` & `dictlearn-0.2.2/src/dictlearn/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `dictlearn-0.2.1/src/dictlearn.egg-info/SOURCES.txt` & `dictlearn-0.2.2/src/dictlearn.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -32,8 +32,19 @@
 src/dictlearn/models/KDDL.py
 src/dictlearn/models/KDPL.py
 src/dictlearn/models/KLCDL.py
 src/dictlearn/models/LCDL.py
 src/dictlearn/models/__init__.py
 src/dictlearn/utils/__init__.py
 src/dictlearn/utils/data_utils.py
-src/dictlearn/utils/generic_utils.py
+src/dictlearn/utils/generic_utils.py
+tests/test_ddl.py
+tests/test_dl.py
+tests/test_dl_all.py
+tests/test_dpl.py
+tests/test_kddl.py
+tests/test_kdl.py
+tests/test_kdpl.py
+tests/test_kernel_approximation.py
+tests/test_klcdl.py
+tests/test_lcdl.py
+tests/test_odl.py
```

