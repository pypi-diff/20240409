# Comparing `tmp/pyliger-0.2.1.tar.gz` & `tmp/pyliger-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyliger-0.2.1.tar", last modified: Thu Feb  1 05:08:47 2024, max compression
+gzip compressed data, was "pyliger-0.2.2.tar", last modified: Tue Apr  9 19:03:12 2024, max compression
```

## Comparing `pyliger-0.2.1.tar` & `pyliger-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35149 2024-02-01 05:08:30.622606 pyliger-0.2.1/LICENSE
--rw-r--r--   0        0        0      578 2024-02-01 05:08:30.622606 pyliger-0.2.1/README.md
--rw-r--r--   0        0        0     1563 2024-02-01 05:08:47.582538 pyliger-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      939 2024-02-01 05:08:30.630606 pyliger-0.2.1/src/pyliger/__init__.py
--rw-r--r--   0        0        0     4620 2024-02-01 05:08:30.630606 pyliger-0.2.1/src/pyliger/_utilities.py
--rw-r--r--   0        0        0     2899 2024-02-01 05:08:30.630606 pyliger-0.2.1/src/pyliger/clustering/_leiden.py
--rw-r--r--   0        0        0     2668 2024-02-01 05:08:30.630606 pyliger-0.2.1/src/pyliger/clustering/_louvain.py
--rw-r--r--   0        0        0     3802 2024-02-01 05:08:30.630606 pyliger-0.2.1/src/pyliger/clustering/_utilities.py
--rw-r--r--   0        0        0     1652 2024-02-01 05:08:30.630606 pyliger-0.2.1/src/pyliger/clustering/todo.py
--rw-r--r--   0        0        0 16300140 2024-02-01 05:08:30.698605 pyliger-0.2.1/src/pyliger/datasets/PBMC_control.h5ad
--rw-r--r--   0        0        0 16633964 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad
--rw-r--r--   0        0        0     7913 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/factorization/_iNMF_ANLS.py
--rw-r--r--   0        0        0     6188 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/factorization/_iNMF_HALS.py
--rw-r--r--   0        0        0    26825 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/factorization/_online_iNMF.py
--rw-r--r--   0        0        0    13328 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/factorization/_utilities.py
--rw-r--r--   0        0        0     1528 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/factorization/todo.py
--rw-r--r--   0        0        0       15 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/logging.py
--rw-r--r--   0        0        0     3757 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/_dataset_cluster.py
--rw-r--r--   0        0        0    11827 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/_gene.py
--rw-r--r--   0        0        0     6683 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/_gene_loadings.py
--rw-r--r--   0        0        0    60226 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/_go.py
--rw-r--r--   0        0        0     2660 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/_spatial.py
--rw-r--r--   0        0        0     1358 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/_utilities.py
--rw-r--r--   0        0        0     1838 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/plotting/todo.py
--rw-r--r--   0        0        0     3380 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/preprocessing/_cal_feature.py
--rw-r--r--   0        0        0     7383 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/preprocessing/_initialization.py
--rw-r--r--   0        0        0     3350 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/preprocessing/_normalization.py
--rw-r--r--   0        0        0     2288 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/preprocessing/_qc.py
--rw-r--r--   0        0        0     4493 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/preprocessing/_scale.py
--rw-r--r--   0        0        0     9777 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/preprocessing/_select_genes.py
--rw-r--r--   0        0        0     8442 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/pyliger.py
--rw-r--r--   0        0        0    16861 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/read_write.py
--rw-r--r--   0        0        0     3609 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/_go.py
--rw-r--r--   0        0        0    14922 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/_marker.py
--rw-r--r--   0        0        0     1837 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/_metrics.py
--rw-r--r--   0        0        0     7867 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/_quantile_norm.py
--rw-r--r--   0        0        0     4599 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/_umap.py
--rw-r--r--   0        0        0    11614 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/_wilcoxon.py
--rw-r--r--   0        0        0     1194 2024-02-01 05:08:30.770605 pyliger-0.2.1/src/pyliger/tools/todo.py
--rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 pyliger-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 19:02:57.844474 pyliger-0.2.2/LICENSE
+-rw-r--r--   0        0        0      578 2024-04-09 19:02:57.844474 pyliger-0.2.2/README.md
+-rw-r--r--   0        0        0     1565 2024-04-09 19:03:12.804442 pyliger-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-04-09 19:02:57.852474 pyliger-0.2.2/src/pyliger/__init__.py
+-rw-r--r--   0        0        0     4620 2024-04-09 19:02:57.852474 pyliger-0.2.2/src/pyliger/_utilities.py
+-rw-r--r--   0        0        0     2899 2024-04-09 19:02:57.852474 pyliger-0.2.2/src/pyliger/clustering/_leiden.py
+-rw-r--r--   0        0        0     2668 2024-04-09 19:02:57.852474 pyliger-0.2.2/src/pyliger/clustering/_louvain.py
+-rw-r--r--   0        0        0     3802 2024-04-09 19:02:57.852474 pyliger-0.2.2/src/pyliger/clustering/_utilities.py
+-rw-r--r--   0        0        0     1652 2024-04-09 19:02:57.852474 pyliger-0.2.2/src/pyliger/clustering/todo.py
+-rw-r--r--   0        0        0 16300140 2024-04-09 19:02:57.920474 pyliger-0.2.2/src/pyliger/datasets/PBMC_control.h5ad
+-rw-r--r--   0        0        0 16633964 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad
+-rw-r--r--   0        0        0     7913 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/factorization/_iNMF_ANLS.py
+-rw-r--r--   0        0        0     6188 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/factorization/_iNMF_HALS.py
+-rw-r--r--   0        0        0    26825 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/factorization/_online_iNMF.py
+-rw-r--r--   0        0        0    13328 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/factorization/_utilities.py
+-rw-r--r--   0        0        0     1528 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/factorization/todo.py
+-rw-r--r--   0        0        0       15 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/logging.py
+-rw-r--r--   0        0        0     3757 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/plotting/_dataset_cluster.py
+-rw-r--r--   0        0        0    11827 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/plotting/_gene.py
+-rw-r--r--   0        0        0     6683 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/plotting/_gene_loadings.py
+-rw-r--r--   0        0        0    60226 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/plotting/_go.py
+-rw-r--r--   0        0        0     2660 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/plotting/_spatial.py
+-rw-r--r--   0        0        0     1358 2024-04-09 19:02:57.992474 pyliger-0.2.2/src/pyliger/plotting/_utilities.py
+-rw-r--r--   0        0        0     1838 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/plotting/todo.py
+-rw-r--r--   0        0        0     3380 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/preprocessing/_cal_feature.py
+-rw-r--r--   0        0        0     7383 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/preprocessing/_initialization.py
+-rw-r--r--   0        0        0     3350 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/preprocessing/_normalization.py
+-rw-r--r--   0        0        0     2288 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/preprocessing/_qc.py
+-rw-r--r--   0        0        0     4493 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/preprocessing/_scale.py
+-rw-r--r--   0        0        0     9777 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/preprocessing/_select_genes.py
+-rw-r--r--   0        0        0     8442 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/pyliger.py
+-rw-r--r--   0        0        0    16861 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/read_write.py
+-rw-r--r--   0        0        0     3609 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/_go.py
+-rw-r--r--   0        0        0    14922 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/_marker.py
+-rw-r--r--   0        0        0     1837 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/_metrics.py
+-rw-r--r--   0        0        0     7867 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/_quantile_norm.py
+-rw-r--r--   0        0        0     4599 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/_umap.py
+-rw-r--r--   0        0        0    11614 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/_wilcoxon.py
+-rw-r--r--   0        0        0     1194 2024-04-09 19:02:57.996474 pyliger-0.2.2/src/pyliger/tools/todo.py
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 pyliger-0.2.2/PKG-INFO
```

### Comparing `pyliger-0.2.1/LICENSE` & `pyliger-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/README.md` & `pyliger-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/pyproject.toml` & `pyliger-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "leidenalg",
     "llvmlite",
     "louvain",
     "matplotlib",
     "mygene",
     "numexpr",
     "numba",
-    "numpy",
+    "numpy<2",
     "pandas",
     "plotnine",
     "python-igraph",
     "scikit-learn",
     "scipy",
     "seaborn",
     "umap-learn",
@@ -59,15 +59,15 @@
 ]
 maintainers = [
     { name = "Andrew Robbins", email = "robbiand@med.umich.edu" },
 ]
 name = "pyliger"
 readme = "README.md"
 requires-python = "<3.13, >=3.9"
-version = "0.2.1"
+version = "0.2.2"
 
 [project.license]
 text = "GPL-3.0-only"
 
 [project.urls]
 homepage = "https://welch-lab.github.io"
 repository = "https://github.com/welch-lab/pyliger"
```

### Comparing `pyliger-0.2.1/src/pyliger/__init__.py` & `pyliger-0.2.2/src/pyliger/__init__.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/_utilities.py` & `pyliger-0.2.2/src/pyliger/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/clustering/_leiden.py` & `pyliger-0.2.2/src/pyliger/clustering/_leiden.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/clustering/_louvain.py` & `pyliger-0.2.2/src/pyliger/clustering/_louvain.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/clustering/_utilities.py` & `pyliger-0.2.2/src/pyliger/clustering/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/clustering/todo.py` & `pyliger-0.2.2/src/pyliger/clustering/todo.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/datasets/PBMC_control.h5ad` & `pyliger-0.2.2/src/pyliger/datasets/PBMC_control.h5ad`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad` & `pyliger-0.2.2/src/pyliger/datasets/PBMC_interferon-stimulated.h5ad`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/factorization/_iNMF_ANLS.py` & `pyliger-0.2.2/src/pyliger/factorization/_iNMF_ANLS.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/factorization/_iNMF_HALS.py` & `pyliger-0.2.2/src/pyliger/factorization/_iNMF_HALS.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/factorization/_online_iNMF.py` & `pyliger-0.2.2/src/pyliger/factorization/_online_iNMF.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/factorization/_utilities.py` & `pyliger-0.2.2/src/pyliger/factorization/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/factorization/todo.py` & `pyliger-0.2.2/src/pyliger/factorization/todo.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/_dataset_cluster.py` & `pyliger-0.2.2/src/pyliger/plotting/_dataset_cluster.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/_gene.py` & `pyliger-0.2.2/src/pyliger/plotting/_gene.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/_gene_loadings.py` & `pyliger-0.2.2/src/pyliger/plotting/_gene_loadings.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/_go.py` & `pyliger-0.2.2/src/pyliger/plotting/_go.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/_spatial.py` & `pyliger-0.2.2/src/pyliger/plotting/_spatial.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/_utilities.py` & `pyliger-0.2.2/src/pyliger/plotting/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/plotting/todo.py` & `pyliger-0.2.2/src/pyliger/plotting/todo.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/preprocessing/_cal_feature.py` & `pyliger-0.2.2/src/pyliger/preprocessing/_cal_feature.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/preprocessing/_initialization.py` & `pyliger-0.2.2/src/pyliger/preprocessing/_initialization.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/preprocessing/_normalization.py` & `pyliger-0.2.2/src/pyliger/preprocessing/_normalization.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/preprocessing/_qc.py` & `pyliger-0.2.2/src/pyliger/preprocessing/_qc.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/preprocessing/_scale.py` & `pyliger-0.2.2/src/pyliger/preprocessing/_scale.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/preprocessing/_select_genes.py` & `pyliger-0.2.2/src/pyliger/preprocessing/_select_genes.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/pyliger.py` & `pyliger-0.2.2/src/pyliger/pyliger.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/read_write.py` & `pyliger-0.2.2/src/pyliger/read_write.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/_go.py` & `pyliger-0.2.2/src/pyliger/tools/_go.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/_marker.py` & `pyliger-0.2.2/src/pyliger/tools/_marker.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/_metrics.py` & `pyliger-0.2.2/src/pyliger/tools/_metrics.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/_quantile_norm.py` & `pyliger-0.2.2/src/pyliger/tools/_quantile_norm.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/_umap.py` & `pyliger-0.2.2/src/pyliger/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/_wilcoxon.py` & `pyliger-0.2.2/src/pyliger/tools/_wilcoxon.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/src/pyliger/tools/todo.py` & `pyliger-0.2.2/src/pyliger/tools/todo.py`

 * *Files identical despite different names*

### Comparing `pyliger-0.2.1/PKG-INFO` & `pyliger-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyliger
-Version: 0.2.1
+Version: 0.2.2
 Summary: The Python version of LIGER package.
 Keywords: LIGER
 Home-page: https://welch-lab.github.io
 Author-Email: Joshua Welch <welchjd@med.umich.edu>, Lu Lu <luluhz@umich.edu>
 Maintainer-Email: Andrew Robbins <robbiand@med.umich.edu>
 License: GPL-3.0-only
 Classifier: Development Status :: 4 - Beta
@@ -27,15 +27,15 @@
 Requires-Dist: leidenalg
 Requires-Dist: llvmlite
 Requires-Dist: louvain
 Requires-Dist: matplotlib
 Requires-Dist: mygene
 Requires-Dist: numexpr
 Requires-Dist: numba
-Requires-Dist: numpy
+Requires-Dist: numpy<2
 Requires-Dist: pandas
 Requires-Dist: plotnine
 Requires-Dist: python-igraph
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: umap-learn
```

