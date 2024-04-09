# Comparing `tmp/mofapy2-0.7.0.tar.gz` & `tmp/mofapy2-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mofapy2-0.7.0.tar", max compression
+gzip compressed data, was "mofapy2-0.7.1.tar", max compression
```

## Comparing `mofapy2-0.7.0.tar` & `mofapy2-0.7.1.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0     7652 2021-01-06 10:30:14.000000 mofapy2-0.7.0/LICENSE
--rw-r--r--   0        0        0      854 2022-10-07 12:20:21.788589 mofapy2-0.7.0/README.md
--rw-r--r--   0        0        0       55 2022-07-30 14:43:07.149748 mofapy2-0.7.0/mofapy2/__init__.py
--rw-r--r--   0        0        0        0 2022-07-30 14:43:07.132821 mofapy2-0.7.0/mofapy2/build_model/__init__.py
--rw-r--r--   0        0        0    13418 2023-02-11 12:12:57.596453 mofapy2-0.7.0/mofapy2/build_model/build_model.py
--rw-r--r--   0        0        0    30916 2023-02-11 12:12:57.596798 mofapy2-0.7.0/mofapy2/build_model/init_model.py
--rw-r--r--   0        0        0    29309 2023-02-11 12:12:57.597320 mofapy2-0.7.0/mofapy2/build_model/save_model.py
--rw-r--r--   0        0        0      645 2023-02-11 12:12:57.597723 mofapy2-0.7.0/mofapy2/build_model/train_model.py
--rw-r--r--   0        0        0     3506 2023-02-11 12:12:57.597997 mofapy2-0.7.0/mofapy2/build_model/utils.py
--rw-r--r--   0        0        0      464 2023-02-11 12:12:57.598282 mofapy2-0.7.0/mofapy2/config.py
--rw-r--r--   0        0        0    29669 2023-02-11 12:12:57.598749 mofapy2-0.7.0/mofapy2/core/BayesNet.py
--rw-r--r--   0        0        0       21 2022-07-30 14:43:07.144810 mofapy2-0.7.0/mofapy2/core/__init__.py
--rw-r--r--   0        0        0      450 2023-02-11 12:12:57.599138 mofapy2-0.7.0/mofapy2/core/distributions/__init__.py
--rw-r--r--   0        0        0     3951 2023-02-11 12:12:57.599410 mofapy2-0.7.0/mofapy2/core/distributions/basic_distributions.py
--rw-r--r--   0        0        0     1385 2023-02-11 12:12:57.599647 mofapy2-0.7.0/mofapy2/core/distributions/bernoulli.py
--rw-r--r--   0        0        0     4867 2023-02-11 12:12:57.600465 mofapy2-0.7.0/mofapy2/core/distributions/bernoulli_gaussian.py
--rw-r--r--   0        0        0     1913 2023-02-11 12:12:57.600738 mofapy2-0.7.0/mofapy2/core/distributions/beta.py
--rw-r--r--   0        0        0     2051 2023-02-11 12:12:57.601210 mofapy2-0.7.0/mofapy2/core/distributions/binomial.py
--rw-r--r--   0        0        0     2218 2023-02-11 12:12:57.601444 mofapy2-0.7.0/mofapy2/core/distributions/gamma.py
--rw-r--r--   0        0        0    38151 2023-02-11 12:12:57.601774 mofapy2-0.7.0/mofapy2/core/distributions/multi_task_GP.py
--rw-r--r--   0        0        0    17516 2023-02-11 12:12:57.602171 mofapy2-0.7.0/mofapy2/core/distributions/multivariate_gaussian.py
--rw-r--r--   0        0        0     1673 2023-02-11 12:12:57.602429 mofapy2-0.7.0/mofapy2/core/distributions/poisson.py
--rw-r--r--   0        0        0     2356 2023-02-11 12:12:57.603058 mofapy2-0.7.0/mofapy2/core/distributions/univariate_gaussian.py
--rw-r--r--   0        0        0     5649 2023-02-11 12:12:57.603519 mofapy2-0.7.0/mofapy2/core/gp_utils.py
--rw-r--r--   0        0        0     1772 2023-02-11 12:12:57.603761 mofapy2-0.7.0/mofapy2/core/gpu_utils.py
--rw-r--r--   0        0        0     6589 2023-02-11 12:12:57.604191 mofapy2-0.7.0/mofapy2/core/nodes/Alpha_nodes.py
--rw-r--r--   0        0        0     4539 2023-02-11 12:12:57.605131 mofapy2-0.7.0/mofapy2/core/nodes/Kc_node.py
--rw-r--r--   0        0        0     3540 2023-02-11 12:12:57.605442 mofapy2-0.7.0/mofapy2/core/nodes/Kg_node.py
--rw-r--r--   0        0        0    53478 2023-02-11 12:12:57.605982 mofapy2-0.7.0/mofapy2/core/nodes/Sigma_node.py
--rwxr-xr-x   0        0        0     5567 2023-02-11 12:12:57.606217 mofapy2-0.7.0/mofapy2/core/nodes/Tau_nodes.py
--rw-r--r--   0        0        0     6758 2023-02-11 12:12:57.606397 mofapy2-0.7.0/mofapy2/core/nodes/Theta_nodes.py
--rw-r--r--   0        0        0     8279 2023-02-11 12:12:57.606582 mofapy2-0.7.0/mofapy2/core/nodes/U_nodes.py
--rwxr-xr-x   0        0        0    11352 2023-02-11 12:12:57.606834 mofapy2-0.7.0/mofapy2/core/nodes/W_nodes.py
--rw-r--r--   0        0        0     3736 2023-02-11 12:12:57.607335 mofapy2-0.7.0/mofapy2/core/nodes/Y_nodes.py
--rwxr-xr-x   0        0        0    16689 2023-02-11 12:12:57.607635 mofapy2-0.7.0/mofapy2/core/nodes/Z_nodes.py
--rw-r--r--   0        0        0     9722 2023-02-11 12:12:57.607945 mofapy2-0.7.0/mofapy2/core/nodes/Z_nodes_GP.py
--rw-r--r--   0        0        0     8402 2023-02-11 12:12:57.608299 mofapy2-0.7.0/mofapy2/core/nodes/Z_nodes_GP_mv.py
--rw-r--r--   0        0        0     7798 2023-02-11 12:12:57.608533 mofapy2-0.7.0/mofapy2/core/nodes/ZgU_node.py
--rw-r--r--   0        0        0      582 2023-02-11 12:12:57.608737 mofapy2-0.7.0/mofapy2/core/nodes/__init__.py
--rw-r--r--   0        0        0     3982 2023-02-11 12:12:57.608940 mofapy2-0.7.0/mofapy2/core/nodes/basic_nodes.py
--rw-r--r--   0        0        0     6992 2023-02-11 12:12:57.609184 mofapy2-0.7.0/mofapy2/core/nodes/multiview_nodes.py
--rw-r--r--   0        0        0    21736 2023-02-11 12:12:57.609454 mofapy2-0.7.0/mofapy2/core/nodes/nongaussian_nodes.py
--rw-r--r--   0        0        0    12578 2023-02-11 12:12:57.609676 mofapy2-0.7.0/mofapy2/core/nodes/variational_nodes.py
--rw-r--r--   0        0        0     3788 2023-02-11 12:12:57.609859 mofapy2-0.7.0/mofapy2/core/utils.py
--rw-r--r--   0        0        0    20317 2023-02-11 18:22:11.368694 mofapy2-0.7.0/mofapy2/notebooks/getting_started_python.ipynb
--rw-r--r--   0        0        0     1394 2022-10-05 16:22:54.436309 mofapy2-0.7.0/mofapy2/notebooks/run_mofa_cpu_vs_gpu.py
--rw-r--r--   0        0        0      325 2022-10-05 16:22:59.880280 mofapy2-0.7.0/mofapy2/notebooks/test_cupy.py
--rw-r--r--   0        0        0        0 2022-07-30 14:43:07.151031 mofapy2-0.7.0/mofapy2/run/__init__.py
--rw-r--r--   0        0        0    78631 2023-02-11 12:12:57.610526 mofapy2-0.7.0/mofapy2/run/entry_point.py
--rw-r--r--   0        0        0   324931 2021-01-06 10:30:14.000000 mofapy2-0.7.0/mofapy2/run/test_data/view_0.txt
--rw-r--r--   0        0        0   324642 2021-01-06 10:30:14.000000 mofapy2-0.7.0/mofapy2/run/test_data/view_1.txt
--rw-r--r--   0        0        0   324951 2021-01-06 10:30:14.000000 mofapy2-0.7.0/mofapy2/run/test_data/view_2.txt
--rw-r--r--   0        0        0   996145 2021-01-06 10:30:14.000000 mofapy2-0.7.0/mofapy2/run/test_data/with_nas/500_0.txt
--rw-r--r--   0        0        0   996423 2021-01-06 10:30:14.000000 mofapy2-0.7.0/mofapy2/run/test_data/with_nas/500_1.txt
--rw-r--r--   0        0        0   995502 2021-01-06 10:30:14.000000 mofapy2-0.7.0/mofapy2/run/test_data/with_nas/500_2.txt
--rw-r--r--   0        0        0        0 2022-07-30 14:43:07.149530 mofapy2-0.7.0/mofapy2/simulate/__init__.py
--rw-r--r--   0        0        0     6948 2023-02-11 12:12:57.610838 mofapy2-0.7.0/mofapy2/simulate/simulate_mofa.py
--rw-r--r--   0        0        0      137 2023-02-11 12:12:57.611398 mofapy2-0.7.0/mofapy2/version.py
--rw-r--r--   0        0        0      636 2023-02-11 12:12:57.612022 mofapy2-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 mofapy2-0.7.0/setup.py
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 mofapy2-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-09 08:24:21.904837 mofapy2-0.7.1/LICENSE
+-rw-r--r--   0        0        0      890 2024-04-09 08:24:21.905154 mofapy2-0.7.1/README.md
+-rw-r--r--   0        0        0       55 2024-04-09 08:24:21.905954 mofapy2-0.7.1/mofapy2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:24:21.906220 mofapy2-0.7.1/mofapy2/build_model/__init__.py
+-rw-r--r--   0        0        0    13372 2024-04-09 08:24:21.906726 mofapy2-0.7.1/mofapy2/build_model/build_model.py
+-rw-r--r--   0        0        0    30904 2024-04-09 08:24:21.907312 mofapy2-0.7.1/mofapy2/build_model/init_model.py
+-rw-r--r--   0        0        0    29296 2024-04-09 08:24:21.907925 mofapy2-0.7.1/mofapy2/build_model/save_model.py
+-rw-r--r--   0        0        0      644 2024-04-09 08:24:21.908246 mofapy2-0.7.1/mofapy2/build_model/train_model.py
+-rw-r--r--   0        0        0     3503 2024-04-09 08:24:21.908676 mofapy2-0.7.1/mofapy2/build_model/utils.py
+-rw-r--r--   0        0        0      464 2024-04-09 08:24:21.910084 mofapy2-0.7.1/mofapy2/config.py
+-rw-r--r--   0        0        0    29662 2024-04-09 08:34:04.999908 mofapy2-0.7.1/mofapy2/core/BayesNet.py
+-rw-r--r--   0        0        0       21 2024-04-09 08:24:21.911205 mofapy2-0.7.1/mofapy2/core/__init__.py
+-rw-r--r--   0        0        0      450 2024-04-09 08:24:21.911671 mofapy2-0.7.1/mofapy2/core/distributions/__init__.py
+-rw-r--r--   0        0        0     3954 2024-04-09 08:34:05.000660 mofapy2-0.7.1/mofapy2/core/distributions/basic_distributions.py
+-rw-r--r--   0        0        0     1385 2024-04-09 08:24:21.912442 mofapy2-0.7.1/mofapy2/core/distributions/bernoulli.py
+-rw-r--r--   0        0        0     4866 2024-04-09 08:24:21.912850 mofapy2-0.7.1/mofapy2/core/distributions/bernoulli_gaussian.py
+-rw-r--r--   0        0        0     1913 2024-04-09 08:24:21.913271 mofapy2-0.7.1/mofapy2/core/distributions/beta.py
+-rw-r--r--   0        0        0     2051 2024-04-09 08:24:21.913596 mofapy2-0.7.1/mofapy2/core/distributions/binomial.py
+-rw-r--r--   0        0        0     2218 2024-04-09 08:24:21.914022 mofapy2-0.7.1/mofapy2/core/distributions/gamma.py
+-rw-r--r--   0        0        0    38151 2024-04-09 08:24:21.914852 mofapy2-0.7.1/mofapy2/core/distributions/multi_task_GP.py
+-rw-r--r--   0        0        0    17516 2024-04-09 08:24:21.915305 mofapy2-0.7.1/mofapy2/core/distributions/multivariate_gaussian.py
+-rw-r--r--   0        0        0     1673 2024-04-09 08:24:21.915572 mofapy2-0.7.1/mofapy2/core/distributions/poisson.py
+-rw-r--r--   0        0        0     2356 2024-04-09 08:24:21.915836 mofapy2-0.7.1/mofapy2/core/distributions/univariate_gaussian.py
+-rw-r--r--   0        0        0     5649 2024-04-09 08:24:21.916309 mofapy2-0.7.1/mofapy2/core/gp_utils.py
+-rw-r--r--   0        0        0     1773 2024-04-09 08:24:21.916592 mofapy2-0.7.1/mofapy2/core/gpu_utils.py
+-rw-r--r--   0        0        0     6589 2024-04-09 08:24:21.917077 mofapy2-0.7.1/mofapy2/core/nodes/Alpha_nodes.py
+-rw-r--r--   0        0        0     4537 2024-04-09 08:24:21.917463 mofapy2-0.7.1/mofapy2/core/nodes/Kc_node.py
+-rw-r--r--   0        0        0     3541 2024-04-09 08:24:21.917816 mofapy2-0.7.1/mofapy2/core/nodes/Kg_node.py
+-rw-r--r--   0        0        0    53473 2024-04-09 08:24:21.919077 mofapy2-0.7.1/mofapy2/core/nodes/Sigma_node.py
+-rwxr-xr-x   0        0        0     5567 2024-04-09 08:24:21.919559 mofapy2-0.7.1/mofapy2/core/nodes/Tau_nodes.py
+-rw-r--r--   0        0        0     6754 2024-04-09 08:24:21.920188 mofapy2-0.7.1/mofapy2/core/nodes/Theta_nodes.py
+-rw-r--r--   0        0        0     8279 2024-04-09 08:24:21.920735 mofapy2-0.7.1/mofapy2/core/nodes/U_nodes.py
+-rwxr-xr-x   0        0        0    11347 2024-04-09 08:24:21.921268 mofapy2-0.7.1/mofapy2/core/nodes/W_nodes.py
+-rw-r--r--   0        0        0     3736 2024-04-09 08:24:21.921551 mofapy2-0.7.1/mofapy2/core/nodes/Y_nodes.py
+-rwxr-xr-x   0        0        0    16687 2024-04-09 08:24:21.921934 mofapy2-0.7.1/mofapy2/core/nodes/Z_nodes.py
+-rw-r--r--   0        0        0     9722 2024-04-09 08:24:21.922269 mofapy2-0.7.1/mofapy2/core/nodes/Z_nodes_GP.py
+-rw-r--r--   0        0        0     8402 2024-04-09 08:24:21.923082 mofapy2-0.7.1/mofapy2/core/nodes/Z_nodes_GP_mv.py
+-rw-r--r--   0        0        0     7797 2024-04-09 08:24:21.923950 mofapy2-0.7.1/mofapy2/core/nodes/ZgU_node.py
+-rw-r--r--   0        0        0      582 2024-04-09 08:24:21.924303 mofapy2-0.7.1/mofapy2/core/nodes/__init__.py
+-rw-r--r--   0        0        0     3982 2024-04-09 08:24:21.924802 mofapy2-0.7.1/mofapy2/core/nodes/basic_nodes.py
+-rw-r--r--   0        0        0     6992 2024-04-09 08:24:21.925730 mofapy2-0.7.1/mofapy2/core/nodes/multiview_nodes.py
+-rw-r--r--   0        0        0    21736 2024-04-09 08:24:21.926549 mofapy2-0.7.1/mofapy2/core/nodes/nongaussian_nodes.py
+-rw-r--r--   0        0        0    12578 2024-04-09 08:24:21.927146 mofapy2-0.7.1/mofapy2/core/nodes/variational_nodes.py
+-rw-r--r--   0        0        0     3788 2024-04-09 08:24:21.928135 mofapy2-0.7.1/mofapy2/core/utils.py
+-rw-r--r--   0        0        0    20317 2024-04-09 08:24:21.928920 mofapy2-0.7.1/mofapy2/notebooks/getting_started_python.ipynb
+-rw-r--r--   0        0        0     1435 2024-04-09 08:24:21.929173 mofapy2-0.7.1/mofapy2/notebooks/run_mofa_cpu_vs_gpu.py
+-rw-r--r--   0        0        0      336 2024-04-09 08:24:21.929954 mofapy2-0.7.1/mofapy2/notebooks/test_cupy.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:24:21.930378 mofapy2-0.7.1/mofapy2/run/__init__.py
+-rw-r--r--   0        0        0    77336 2024-04-09 08:24:21.931530 mofapy2-0.7.1/mofapy2/run/entry_point.py
+-rw-r--r--   0        0        0   324931 2024-04-09 08:24:21.955351 mofapy2-0.7.1/mofapy2/run/test_data/view_0.txt
+-rw-r--r--   0        0        0   324642 2024-04-09 08:24:21.967281 mofapy2-0.7.1/mofapy2/run/test_data/view_1.txt
+-rw-r--r--   0        0        0   324951 2024-04-09 08:24:21.970425 mofapy2-0.7.1/mofapy2/run/test_data/view_2.txt
+-rw-r--r--   0        0        0   996145 2024-04-09 08:24:21.983609 mofapy2-0.7.1/mofapy2/run/test_data/with_nas/500_0.txt
+-rw-r--r--   0        0        0   996423 2024-04-09 08:24:21.996778 mofapy2-0.7.1/mofapy2/run/test_data/with_nas/500_1.txt
+-rw-r--r--   0        0        0   995502 2024-04-09 08:24:22.037072 mofapy2-0.7.1/mofapy2/run/test_data/with_nas/500_2.txt
+-rw-r--r--   0        0        0        0 2024-04-09 08:24:22.038617 mofapy2-0.7.1/mofapy2/simulate/__init__.py
+-rw-r--r--   0        0        0     6896 2024-04-09 08:24:22.040481 mofapy2-0.7.1/mofapy2/simulate/simulate_mofa.py
+-rw-r--r--   0        0        0      137 2024-04-09 08:29:20.363645 mofapy2-0.7.1/mofapy2/version.py
+-rw-r--r--   0        0        0      629 2024-04-09 08:24:22.041805 mofapy2-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 mofapy2-0.7.1/PKG-INFO
```

### Comparing `mofapy2-0.7.0/LICENSE` & `mofapy2-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/README.md` & `mofapy2-0.7.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Multi-Omics Factor Analysis
 
-![PyPi version](https://img.shields.io/pypi/v/mofapy2)
+[![PyPi version](https://img.shields.io/pypi/v/mofapy2)](https://pypi.org/project/mofapy2)
 
 MOFA is a factor analysis model that provides a general framework for the integration of multi-omic data sets in an unsupervised fashion.  
 This repository contains `mofapy2` Python library source code.
 
 - For the downstream analysis in Python please check the mofax package: https://github.com/bioFAM/mofax
 - For the downstream analysis in R please check the MOFA2 package: https://github.com/bioFAM/MOFA2
```

### Comparing `mofapy2-0.7.0/mofapy2/build_model/build_model.py` & `mofapy2-0.7.1/mofapy2/build_model/build_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
         # Initialise hyperparameters for the ThetaZ prior
         initTheta_a = 1.0
         initTheta_b = 1.0
         initTheta_qE = None
         # initTheta_qE = 1.
 
         self.init_model.initThetaZ(
-            self.data_opts["samples_groups"],
             qa=initTheta_a,
             qb=initTheta_b,
             qE=initTheta_qE,
         )
 
     def build_ThetaW(self):
         """Build node ThetaW for the Spike and Slab prior on the weights"""
```

### Comparing `mofapy2-0.7.0/mofapy2/build_model/init_model.py` & `mofapy2-0.7.1/mofapy2/build_model/init_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
         # variance
         qvar = np.ones((self.N, self.K)) * qvar
 
         # mean
         if qmean is not None:
             if isinstance(qmean, str):
-
                 # Random initialisation
                 if qmean == "random":
                     qmean = stats.norm.rvs(loc=0, scale=1, size=(self.N, self.K))
 
                 # Random initialisation with orthogonal factors
                 elif qmean == "orthogonal":
                     pca = sklearn.decomposition.PCA(n_components=self.K, whiten=True)
@@ -195,15 +194,14 @@
 
         # variance
         qvar = np.array([np.eye(self.N) * qvar for k in range(self.K)])
 
         # mean
         if qmean is not None:
             if isinstance(qmean, str):
-
                 # Random initialisation
                 if qmean == "random":
                     qmean = stats.norm.rvs(loc=0, scale=1, size=(self.N, self.K))
 
                 # Random initialisation with orthogonal factors
                 elif qmean == "orthogonal":
                     pca = sklearn.decomposition.PCA(n_components=self.K, whiten=True)
@@ -346,15 +344,14 @@
 
         # variance
         qvar = np.ones((self.N, self.K)) * qvar
 
         # mean
         if qmean is not None:
             if isinstance(qmean, str):
-
                 # Random initialisation
                 if qmean == "random":
                     qmean = stats.norm.rvs(loc=0, scale=1, size=(self.N, self.K))
 
                 # Random initialisation with orthogonal factors
                 elif qmean == "orthogonal":
                     pca = sklearn.decomposition.PCA(n_components=self.K, whiten=True)
@@ -411,15 +408,14 @@
         sample_cov,
         start_opt=20,
         n_grid=10,
         opt_freq=10,
         model_groups=False,
         use_gpytorch=False,
     ):
-
         self.Sigma = Sigma_Node(
             dim=(self.K,),
             sample_cov=sample_cov,
             groups=self.groups,
             start_opt=start_opt,
             n_grid=n_grid,
             opt_freq=opt_freq,
@@ -433,15 +429,14 @@
         start_opt=20,
         n_grid=10,
         idx_inducing=None,
         opt_freq=10,
         model_groups=False,
         use_gpytorch=False,
     ):
-
         self.Sigma = Sigma_Node_sparse(
             dim=(self.K,),
             sample_cov=sample_cov,
             groups=self.groups,
             start_opt=start_opt,
             n_grid=n_grid,
             idx_inducing=idx_inducing,
@@ -460,15 +455,14 @@
         warping_open_begin=True,
         warping_open_end=True,
         warping_groups=None,
         opt_freq=10,
         model_groups=False,
         use_gpytorch=False,
     ):
-
         self.Sigma = Sigma_Node_warping(
             dim=(self.K,),
             sample_cov=sample_cov,
             groups=self.groups,
             start_opt=start_opt,
             n_grid=n_grid,
             warping_freq=warping_freq,
@@ -510,15 +504,14 @@
         # TODO:
         # - add different ways to initialise the expectations of the posterior: random, orthogonal, PCA
 
         ## Initialise prior distribution (P)
 
         ## Initialise variational distribution (Q)
         if isinstance(qmean_T1, str):
-
             if qmean_T1 == "random":
                 qmean_T1 = stats.norm.rvs(loc=0, scale=1, size=(self.N, self.K))
             elif qmean_T1 == "pca":
                 pca = sklearn.decomposition.PCA(n_components=self.K, whiten=True)
                 Ytmp = np.concatenate(Y, axis=1)
 
                 if impute == True:
@@ -575,29 +568,27 @@
         qE: initial value of the expectation of the variational distribution
         qE2: initial value of the second moment of the variational distribution
         """
 
         W_list = [None] * self.M
 
         for m in range(self.M):
-
             ## Initialise prior distribution (P) ##
 
             # mean
             pmean_m = np.ones((self.D[m], self.K)) * pmean
 
             ## Initialise variational distribution (Q) ##
 
             # variance
             qvar_m = np.ones((self.D[m], self.K)) * qvar
 
             # mean
             if qmean is not None:
                 if isinstance(qmean, str):
-
                     # Random initialisation
                     if qmean == "random":
                         qmean_m = stats.norm.rvs(
                             loc=0, scale=1.0, size=(self.D[m], self.K)
                         )
 
                     elif qmean_S1 == "pca":
@@ -661,20 +652,18 @@
         ----------
         (...)
         """
 
         W_list = [None] * self.M
 
         for m in range(self.M):
-
             ## Initialise prior distribution (P)
 
             ## Initialise variational distribution (Q)
             if isinstance(qmean_S1, str):
-
                 if qmean_S1 == "random":
                     qmean_S1_tmp = stats.norm.rvs(
                         loc=0, scale=1.0, size=(self.D[m], self.K)
                     )
                 elif qmean_S1 == "pca":
                     # if np.any(np.isnan(Y[m])):
                     #     print("Initialising weights with PCA solution, but data has missing values. Doing quick feature-wise mean imputation (just for the initialisation)... ")
@@ -796,15 +785,14 @@
         qE: float
             initial expectation of the variational distribution
         """
 
         tau_list = [None] * self.M
 
         for m in range(self.M):
-
             # Poisson noise model for count data
             if self.lik[m] == "poisson":
                 tmp = 0.25 + 0.17 * np.nanmax(self.data[m], axis=0)
                 tmp = np.repeat(tmp[None, :], self.N, axis=0)
                 tau_list[m] = Tau_Seeger(dim=(self.N, self.D[m]), value=tmp)
 
             # Bernoulli noise model for binary data
```

### Comparing `mofapy2-0.7.0/mofapy2/build_model/save_model.py` & `mofapy2-0.7.1/mofapy2/build_model/save_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         groups_names,
         covariates_names,
         samples_metadata,
         features_metadata,
         sort_factors=True,
         compression_level=9,
     ):
-
         # Check that the model is trained
         # NOTE: it might be not trained if saving when training is interrupted
         if not model.trained:
             print("Note: the model to be saved is not trained.")
         self.model = model
 
         # Initialise hdf5 file
@@ -261,15 +260,14 @@
         data_grp = self.hdf5.create_group("data")
         intercept_grp = self.hdf5.create_group("intercepts")
 
         for m in range(len(self.data)):
             data_subgrp = data_grp.create_group(self.views_names[m])
             intercept_subgrp = intercept_grp.create_group(self.views_names[m])
             for g in range(len(self.groups_names)):
-
                 # Subset group
                 samples_idx = np.where(
                     np.array(self.samples_groups) == self.groups_names[g]
                 )[0]
                 tmp = self.data[m][samples_idx, :]
 
                 # Mask missing values
@@ -328,15 +326,14 @@
         # Create HDF5 groups
         data_grp = self.hdf5.create_group("imputed_data")
 
         # Save mean
         for m in range(len(mean)):
             view_subgrp = data_grp.create_group(self.views_names[m])
             for g in range(len(self.groups_names)):
-
                 # Subset group
                 samples_idx = np.where(
                     np.array(self.samples_groups) == self.groups_names[g]
                 )[0]
 
                 # Create HDF5 subgroup
                 group_subgrp = view_subgrp.create_group(self.groups_names[g])
@@ -387,15 +384,14 @@
                     "variance",
                     data=variance[sampleidx, :][:, self.order_factors],
                     compression="gzip",
                     compression_opts=self.compression_level,
                 )
 
     def saveExpectations(self, nodes="all"):
-
         # Get nodes from the model
         nodes_dic = self.model.getNodes()
         if type(nodes) is str:
             nodes = list(nodes_dic.keys()) if nodes == "all" else [nodes]
         elif type(nodes) is list or type(nodes) is tuple:
             assert set(nodes).issubset(
                 [
@@ -431,23 +427,20 @@
             exp = nodes_dic[n].getExpectation()
             # for saving of higher moments:
             # exp = nodes_dic[n].getExpectations()
 
             # Multi-view nodes
             if isinstance(nodes_dic[n], Multiview_Node):
                 for m in range(nodes_dic[n].M):
-
                     # Multi-groups nodes (Tau, Y, and Z)
                     if n in multigroup_nodes:
-
                         # Create subgroup for the view
                         view_subgrp = node_subgrp.create_group(self.views_names[m])
 
                         for g in self.groups_names:
-
                             # Add missing values to Tau and Y nodes
                             exp[m][self.mask[m]] = np.nan
 
                             # create hdf5 data set for the expectation
                             samp_indices = np.where(np.array(self.samples_groups) == g)[
                                 0
                             ]
@@ -467,15 +460,14 @@
                             data=foo[self.order_factors],
                             compression="gzip",
                             compression_opts=self.compression_level,
                         )
 
             # Single-view nodes
             else:
-
                 # Multi-group nodes (Z)
                 if n in multigroup_nodes:
                     for g in self.groups_names:
                         samp_indices = np.where(np.array(self.samples_groups) == g)[0]
                         foo = exp[samp_indices, :].T
                         node_subgrp.create_dataset(
                             g,
@@ -544,21 +536,19 @@
 
             # Collect node parameters
             par = nodes_dic[n].getParameters()
 
             # Multi-view nodes
             if isinstance(nodes_dic[n], Multiview_Node):
                 for m in range(nodes_dic[n].M):
-
                     # Create subgroup for the view
                     view_subgrp = node_subgrp.create_group(self.views_names[m])
 
                     # Multi-groups nodes
                     if n in multigroup_nodes:
-
                         for g in self.groups_names:
                             grp_subgrp = view_subgrp.create_group(g)
 
                             # create hdf5 data set for the parameter
                             samp_indices = np.where(np.array(self.samples_groups) == g)[
                                 0
                             ]
@@ -582,15 +572,14 @@
                                     data=tmp,
                                     compression="gzip",
                                     compression_opts=self.compression_level,
                                 )
 
             # Single-view nodes
             else:
-
                 # Multi-group nodes
                 if n in multigroup_nodes:
                     for g in self.groups_names:
                         grp_subgrp = node_subgrp.create_group(g)
                         samp_indices = np.where(np.array(self.samples_groups) == g)[0]
 
                         for k in par.keys():
@@ -611,15 +600,14 @@
                             compression="gzip",
                             compression_opts=self.compression_level,
                         )
 
         pass
 
     def saveModelOptions(self):
-
         # Subset model options
         options_to_save = [
             "likelihoods",
             "spikeslab_factors",
             "spikeslab_weights",
             "ard_factors",
             "ard_weights",
@@ -713,15 +701,14 @@
 
         # Create HDF5 data sets
         for k, v in opts.items():
             grp.create_dataset(k, data=v)
         grp[k].attrs["names"] = np.asarray(list(opts.keys())).astype("S")
 
     def saveVarianceExplained(self):
-
         # Sort values by alphabetical order of views
         # order = np.argsort(self.views_names)
         # # order = [ i[0] for i in sorted(enumerate(self.views_names), key=lambda x:x[1]) ]
 
         # Store variance explained per factor in each view and group
         grp = self.hdf5.create_group("variance_explained")
```

### Comparing `mofapy2-0.7.0/mofapy2/build_model/train_model.py` & `mofapy2-0.7.1/mofapy2/build_model/train_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import pandas as pd
 import numpy as np
 
 from mofapy2.core.BayesNet import BayesNet
 
 
 def train_model(model):
-
     # Sanity check on the Bayesian Network
     assert isinstance(model, BayesNet), "'model' has to be a BayesNet class"
 
     ####################
     ## Start training ##
     ####################
```

### Comparing `mofapy2-0.7.0/mofapy2/build_model/utils.py` & `mofapy2-0.7.1/mofapy2/build_model/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,15 @@
     # double check axis for pandas
     Y_norm = Y_m.apply(_gaussianise_vec, axis)
 
     return Y_norm
 
 
 def process_data(data, likelihoods, data_opts, samples_groups):
-
     for m in range(len(data)):
-
         # For some wierd reason, when using reticulate from R, missing values are stored as -2147483648
         data[m][data[m] == -2147483648] = np.nan
 
         # Removing features with no variance
         var = data[m].std(axis=0)
         if np.any(var == 0.0):
             print(
@@ -75,15 +73,14 @@
                 "Warning: %d features(s) in view %d are full of missing values, please consider removing them before training the model...\n"
                 % ((tmp == 0.0).sum(), m)
             )
             sys.stdout.flush()
 
         # Centering and scaling is only appropriate for gaussian data
         if likelihoods[m] in ["gaussian"]:
-
             # Center features per group
             if data_opts["center_groups"]:
                 for g in data_opts["groups_names"]:
                     filt = [gp == g for gp in samples_groups]
                     data[m][filt, :] -= np.nanmean(data[m][filt, :], axis=0)
 
             # Scale views to unit variance
```

### Comparing `mofapy2-0.7.0/mofapy2/core/BayesNet.py` & `mofapy2-0.7.1/mofapy2/core/BayesNet.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,14 @@
         return expectations
 
     def getNodes(self):
         """Method to return all nodes"""
         return self.nodes
 
     def calculate_variance_explained(self, total=False):
-
         # Collect relevant expectations
         Z = self.nodes["Z"].getExpectation()
         W = self.nodes["W"].getExpectation()
         Y = self.nodes["Y"].getExpectation()
 
         # Get groups
         groups = self.nodes["Y"].nodes[0].groups
@@ -166,15 +165,15 @@
                     Ypred[mask[gg, :]] = 0.0
                     Res = np.sum((Y[m][gg, :] - Ypred) ** 2.0)
                     r2[g][m] = 1.0 - Res / SS
 
                 # Variance explained per factor
                 else:
                     for k in range(self.dim["K"]):
-                        Ypred = s.outer(Z[gg, k], W[m][:, k])
+                        Ypred = np.outer(Z[gg, k], W[m][:, k])
                         Ypred[mask[gg, :]] = 0.0
                         Res = np.sum((Y[m][gg, :] - Ypred) ** 2.0)
                         r2[g][m, k] = 1.0 - Res / SS
         return r2
 
     def removeInactiveFactors(self, min_r2=None, return_idx=False):
         """Method to remove inactive factors
@@ -232,15 +231,15 @@
         for node in self.nodes["Y"].getNodes():
             node.TauTrick = True
 
         if self.options["verbose"]:
             print("ELBO before training:")
             print(
                 "".join(
-                    ["%s=%.2f  " % (k, v) for k, v in elbo.drop("total").iteritems()]
+                    ["%s=%.2f  " % (k, v) for k, v in elbo.drop("total").items()]
                 )
                 + "\nTotal: %.2f\n" % elbo["total"]
             )
         else:
             if not self.options["quiet"]:
                 print("ELBO before training: %.2f \n" % elbo["total"])
 
@@ -327,15 +326,15 @@
                     # Print ELBO decomposed by node and variance explained
                     if self.options["verbose"]:
                         print(
                             "- ELBO decomposition:  "
                             + "".join(
                                 [
                                     "%s=%.2f  " % (k, v)
-                                    for k, v in elbo.iloc[i].drop("total").iteritems()
+                                    for k, v in elbo.iloc[i].drop("total").items()
                                 ]
                             )
                         )
                         print(
                             "- Time spent in ELBO computation: %.1f%%"
                             % (100 * t_elbo / (t_updates + t_elbo))
                         )
@@ -380,15 +379,15 @@
 
         finally:
             # Finish by collecting the training statistics
             self.train_stats = {
                 "time": iter_time,
                 "number_factors": number_factors,
                 "elbo": elbo["total"].values,
-                "elbo_terms": elbo.drop("total", 1),
+                "elbo_terms": elbo.drop("total", axis=1),
             }
             if "Sigma" in self.nodes.keys():
                 tmp = self.nodes["Sigma"].getParameters()  # save only last iteration
                 self.train_stats["length_scales"] = tmp["l"]
                 self.train_stats["scales"] = tmp["scale"]
                 self.train_stats["Kg"] = tmp["Kg"]
 
@@ -715,15 +714,15 @@
                 # Print ELBO decomposed by node and variance explained
                 if self.options["verbose"]:
                     print(
                         "- ELBO decomposition:  "
                         + "".join(
                             [
                                 "%s=%.2f  " % (k, v)
-                                for k, v in elbo.iloc[i].drop("total").iteritems()
+                                for k, v in elbo.iloc[i].drop("total").items()
                             ]
                         )
                     )
                     print(
                         "- Time spent in ELBO computation: %.1f%%"
                         % (100 * t_elbo / (t_updates + t_elbo))
                     )
```

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/basic_distributions.py` & `mofapy2-0.7.1/mofapy2/core/distributions/basic_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import scipy as s
 import numpy as np
 
 # from mofapy2.config import settings
 # from mofapy2.core.utils import *  # TODO prob not necessary ?
 
+
 # General class for probability distributions
 class Distribution(object):
     """General class for a statistical distribution"""
 
     def __init__(self, dim):
         self.dim = dim
 
@@ -60,16 +61,16 @@
 
     def getExpectations(self):
         """General setter function for expectations"""
         return self.expectations
 
     def CheckDimensionalities(self):
         """General method to do a sanity check on the dimensionalities"""
-        # p_dim = set(map(s.shape, self.params.values()))
-        e_dim = set(map(s.shape, self.expectations.values()))
+        # p_dim = set(map(np.shape, self.params.values()))
+        e_dim = set(map(np.shape, self.expectations.values()))
         # assert len(p_dim) == 1, "Parameters have different dimensionalities"
         assert len(e_dim) == 1, "Expectations have different dimensionalities"
         # assert e_dim == p_dim, "Parameters and Expectations have different dimensionality"
 
     def to_float32(self):
         """Convert numpy arrays from float64 to float32"""
         for i in self.params.keys():
```

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/bernoulli.py` & `mofapy2-0.7.1/mofapy2/core/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/bernoulli_gaussian.py` & `mofapy2-0.7.1/mofapy2/core/distributions/bernoulli_gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         #
 
         # Collect expectations
         self.expectations = {"E": E, "EB": EB, "EN": EN, "E2": E2, "ENN": ENN}
         # self.expectations = {'E':E, 'EB':EB, 'EN':EN, 'E2':E2, 'ENN':ENN, 'EXXT':EXXT }
 
     def removeDimensions(self, axis, idx):
-
         # Method to remove undesired dimensions
         # - axis (int): axis from where to remove the elements
         # - idx (numpy array): indices of the elements to remove
         assert axis <= len(self.dim)
         assert np.all(idx < self.dim[axis])
         self.B.removeDimensions(axis, idx)
         self.N_B0.removeDimensions(axis, idx)
```

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/beta.py` & `mofapy2-0.7.1/mofapy2/core/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/binomial.py` & `mofapy2-0.7.1/mofapy2/core/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/gamma.py` & `mofapy2-0.7.1/mofapy2/core/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/multi_task_GP.py` & `mofapy2-0.7.1/mofapy2/core/distributions/multi_task_GP.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/multivariate_gaussian.py` & `mofapy2-0.7.1/mofapy2/core/distributions/multivariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/poisson.py` & `mofapy2-0.7.1/mofapy2/core/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/distributions/univariate_gaussian.py` & `mofapy2-0.7.1/mofapy2/core/distributions/univariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/gp_utils.py` & `mofapy2-0.7.1/mofapy2/core/gp_utils.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/gpu_utils.py` & `mofapy2-0.7.1/mofapy2/core/gpu_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     pass
 
 # --------------------------------------------------------
 # Defalut is to use numpy, not cupy
 # --------------------------------------------------------
 gpu_mode = False
 
+
 # --------------------------------------------------------
 # operations on single matrices
 # --------------------------------------------------------
 def log(mat):
     if gpu_mode:
         return cp.log(mat)
     else:
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Alpha_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Alpha_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Kc_node.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Kc_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         Function to compute kernel matrix for all lengthscales
         """
 
         for i in range(self.n_grid):
             self.compute_kernel_at_gridpoint(i, spectral_decomp=spectral_decomp)
 
     def compute_kernel_at_gridpoint(self, i, spectral_decomp=True):
-
         # build kernel matrix based on given covariance function
         if not spectral_decomp:
             self.Kmat[i, :, :] = SE(self.covariates, self.l_grid[i], zeta=0)
             # self.Kmat[i, :, :] = Cauchy(self.sample_cov_transformed, self.l_grid[i], zeta=0)
         else:
             Kmat = SE(self.covariates, self.l_grid[i], zeta=0)
             # compute spectral decomposition
@@ -114,11 +113,10 @@
         self.K = self.K - 1
 
     def set_gridix(self, lidx, k):
         self.gridix[k] = lidx
         # no recomputation required as stored on grid
 
     def eval_at_newpoints_k(self, new_cov, k):
-
         Kc_new = SE(new_cov, self.l_grid[self.gridix[k]], zeta=0)
 
         return Kc_new
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Kg_node.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Kg_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import scipy as s
 import numpy as np
 from mofapy2.core import gpu_utils
 from mofapy2.core.gp_utils import covar_to_corr
 from mofapy2.core.nodes.variational_nodes import *
 from mofapy2.core.gp_utils import *
 
+
 # TODO: for large number of groups avoid constructing Kmat if spectral decomp and only save x at the end (getParameters in SigmaNode)
 class Kg_Node(Node):
     """
     Sigma node to model the covariance structure K_g across groups.
     This node constructs the group-group covariance and stores the ELBO-optimal hyperparamters
     KG = xx^T + diag(sigma)
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Sigma_node.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Sigma_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,15 +341,14 @@
         self.updateDim(0, self.dim[0] - len(idx))
         self.K = self.K - 1
         self.Sigma = np.delete(self.Sigma, axis=0, obj=idx)
         self.Sigma_inv = np.delete(self.Sigma_inv, axis=0, obj=idx)
         self.Sigma_inv_logdet = np.delete(self.Sigma_inv_logdet, axis=0, obj=idx)
 
     def calc_neg_elbo_k(self, par, lidx, k, var):
-
         self.zeta[k] = par[0]
         self.Kc.set_gridix(lidx, k)
 
         # if required set group parameters
         if self.model_groups:
             sigma = par[1]
             x = par[2:]
@@ -620,15 +619,14 @@
         print("Optimising sigma node...")
 
         K = var.dim[1]
         assert K == len(self.zeta) and K == self.K, "problem in dropping factor"
 
         # optimise hyperparamters of GP
         for k in range(K):
-
             best_zeta = -1
             best_elbo = -np.Inf
 
             # set initial values for optimization
             if self.model_groups:
                 par_init = np.hstack(
                     [
@@ -747,15 +745,14 @@
         groups,
         start_opt=20,
         opt_freq=10,
         n_grid=10,
         rankx=None,
         model_groups=False,
     ):
-
         super().__init__(
             dim, sample_cov, groups, start_opt, opt_freq, n_grid, rankx, model_groups
         )
 
         # initialize group kernel
         if self.model_groups:
             self.G = len(self.groups)  # number of groups
@@ -808,15 +805,14 @@
         start_opt=20,
         opt_freq=10,
         n_grid=10,
         rankx=None,
         model_groups=False,
         idx_inducing=None,
     ):
-
         super().__init__(
             dim, sample_cov, groups, start_opt, opt_freq, n_grid, rankx, model_groups
         )
 
         # sparse GPs
         self.idx_inducing = idx_inducing
         self.Nu = len(idx_inducing)
@@ -942,15 +938,14 @@
         model_groups=False,
         warping_freq=20,
         warping_ref=0,
         warping_open_begin=True,
         warping_open_end=True,
         warping_groups=None,
     ):
-
         super().__init__(
             dim, sample_cov, groups, start_opt, opt_freq, n_grid, rankx, model_groups
         )
         self.kronecker = False
         self.new_alignment = False
 
         # initialize group kernel
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Tau_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Tau_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Theta_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Theta_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         Qa = self.Ppar["a"] + tmp1
         Qb = self.Ppar["b"] + S.shape[0] - tmp1
 
         # Save updated parameters of the Q distribution
         self.Q.setParameters(a=Qa, b=Qb)
 
     def calculateELBO(self):
-
         # Collect parameters and expectations
         Qpar, Qexp = self.Q.getParameters(), self.Q.getExpectations()
         Pa, Pb, Qa, Qb = self.Ppar["a"], self.Ppar["b"], Qpar["a"], Qpar["b"]
         QE, QlnE, QlnEInv = Qexp["E"], Qexp["lnE"], Qexp["lnEInv"]
 
         # minus cross entropy of Q and P
         lb_p = (Pa - 1.0) * QlnE + (Pb - 1.0) * QlnEInv - special.betaln(Pa, Pb)
@@ -87,15 +86,14 @@
     """
     Theta node on Z per group.
     Dimensions of the node are number of groups * number of factors
     Implementation is similar to the one of AlphaZ_Node_groups
     """
 
     def __init__(self, dim, pa, pb, qa, qb, groups, qE=None):
-
         self.groups = groups
         self.factors_axis = 1
         self.N = len(self.groups)
         self.n_groups = len(np.unique(groups))
 
         self.mini_batch = None
 
@@ -155,15 +153,14 @@
         # Compute parameter updates
         Qa, Qb = self._updateParameters(S, groups, ro)
 
         # Save updated parameters of the Q distribution
         self.Q.setParameters(a=Qa, b=Qb)
 
     def _updateParameters(self, S, groups, ro):
-
         Q = self.Q.getParameters()
         Qa, Qb = Q["a"], Q["b"]
         Qa *= 1 - ro
         Qb *= 1 - ro
 
         # Perform update
         for c in range(self.n_groups):
@@ -182,15 +179,14 @@
             Qb[c, :] += ro * (
                 self.Ppar["b"][c, :] + coeff * (S[mask, :].shape[0] - tmp1)
             )
 
         return Qa, Qb
 
     def calculateELBO(self):
-
         # Collect parameters and expectations
         Qpar, Qexp = self.Q.getParameters(), self.Q.getExpectations()
         Pa, Pb, Qa, Qb = self.Ppar["a"], self.Ppar["b"], Qpar["a"], Qpar["b"]
         QE, QlnE, QlnEInv = Qexp["E"], Qexp["lnE"], Qexp["lnEInv"]
 
         # minus cross entropy of Q and P
         lb_p = (Pa - 1.0) * QlnE + (Pb - 1.0) * QlnEInv - special.betaln(Pa, Pb)
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/U_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/U_nodes.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # Import manually defined functions
 from .variational_nodes import MultivariateGaussian_Unobserved_Variational_Node
 
 # TODO:
 # - integrate into Z node using ix
 
+
 # U_GP_Node_mv
 class U_GP_Node_mv(MultivariateGaussian_Unobserved_Variational_Node):
     """
     U node with a Multivariate Gaussian prior and variational distribution
     """
 
     def __init__(
@@ -60,15 +61,14 @@
         """Method to fetch minibatch"""
         if self.mini_batch is None:
             return self.getExpectations()
         else:
             return self.mini_batch
 
     def updateParameters(self, ix=None, ro=1.0):
-
         # Get expectations from other nodes
         W = self.markov_blanket["W"].getExpectations()
         Y = self.markov_blanket["Y"].get_mini_batch()
         tau = self.markov_blanket["Tau"].get_mini_batch()
         Z = self.markov_blanket["Z"].get_mini_batch()
         mask = [self.markov_blanket["Y"].nodes[m].getMask() for m in range(len(Y))]
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/W_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/W_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         if ro is None:
             ro = 1.0
 
         # compute the update
         self._updateParameters(Y, Z, tau, Mu, Alpha, Qmean, Qvar, coeff, ro)
 
     def _updateParameters(self, Y, Z, tau, Mu, Alpha, Qmean, Qvar, coeff, ro):
-
         for k in range(self.dim[1]):
             foo = coeff * np.dot(Z["E2"][:, k], tau)
 
             bar_tmp1 = gpu_utils.array(Z["E"][:, k])
 
             bar_tmp2 = -gpu_utils.dot(
                 gpu_utils.array(Z["E"][:, np.arange(self.dim[1]) != k]),
@@ -92,15 +91,14 @@
             # does not hold for stochastic because of the ro weighting
             Qmean[:, k] *= 1 - ro
             Qmean[:, k] += (
                 ro * (1 / (Alpha[:, k] + foo)) * (bar + Alpha[:, k] * Mu[:, k])
             )
 
     def calculateELBO(self):
-
         # Collect parameters and expectations of current node
         Qpar, Qexp = self.Q.getParameters(), self.Q.getExpectations()
         Qmean, Qvar = Qpar["mean"], Qpar["var"]
         QE, QE2 = Qexp["E"], Qexp["E2"]
 
         if "MuW" in self.markov_blanket:
             PE, PE2 = (
@@ -171,15 +169,14 @@
         self.factors_axis = 1
         gpu_utils.gpu_mode = options["gpu_mode"]
 
     def removeFactors(self, idx):
         super().removeFactors(idx, axis=1)
 
     def updateParameters(self, ix=None, ro=1.0):
-
         # Collect expectations from other nodes
         Y = self.markov_blanket["Y"].get_mini_batch()
         Z = self.markov_blanket["Z"].get_mini_batch()
         tau = self.markov_blanket["Tau"].get_mini_batch()
         mask = self.markov_blanket["Y"].getMask()
 
         if "AlphaW" in self.markov_blanket:
@@ -231,15 +228,14 @@
         Qtheta,
         SW,
         theta_lnE,
         theta_lnEInv,
         coeff,
         ro,
     ):
-
         # Mask matrices
         tau[mask] = 0.0
 
         # Copy matrices to GPU
         # Y_gpu = gpu_utils.array(Y)
         tau_gpu = gpu_utils.array(tau)
         Z_gpu = gpu_utils.array(Z["E"])
@@ -251,15 +247,14 @@
         foo = gpu_utils.asnumpy(gpu_utils.dot(ZZ_gpu.T, tau_gpu).T)
         term4_tmp1 = gpu_utils.asnumpy(gpu_utils.dot(tauY_gpu, Z_gpu))
 
         del tauY_gpu, ZZ_gpu
 
         # Update each latent variable in turn
         for k in range(self.dim[1]):
-
             # Compute terms
             term1 = (theta_lnE - theta_lnEInv)[:, k]
 
             term2 = 0.5 * np.log(Alpha[:, k])
             term3 = 0.5 * coeff * np.log(foo[:, k] + Alpha[:, k])
 
             # term4_tmp1 = gpu_utils.dot(tauYT, Zk_cp)
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Y_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Y_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Z_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Z_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
             Qvar[:, k] = 1.0 / (Alpha[:, k] + foo[:, k])
             Qmean[:, k] = Qvar[:, k] * (bar + Alpha[:, k] * Mu[:, k])
 
         # Save updated parameters of the Q distribution
         return {"Qmean": Qmean, "Qvar": Qvar}
 
     def calculateELBO(self):
-
         # Collect parameters and expectations of current node
         Qpar, Qexp = self.Q.getParameters(), self.Q.getExpectations()
         Qmean, Qvar = Qpar["mean"], Qpar["var"]
         QE, QE2 = Qexp["E"], Qexp["E2"]
 
         if "MuZ" in self.markov_blanket:
             PE, PE2 = (
@@ -428,15 +427,14 @@
 
             # Update Expectations for the next iteration
             SZ[:, k] = Qtheta[:, k] * Qmean_T1[:, k]
 
         return {"mean_B1": Qmean_T1, "var_B1": Qvar_T1, "theta": Qtheta}
 
     def calculateELBO(self):
-
         # Collect parameters and expectations
         Qpar, Qexp = self.Q.getParameters(), self.Q.getExpectations()
         T, ZZ = Qexp["EB"], Qexp["ENN"]
         Qvar = Qpar["var_B1"]
         theta = self.markov_blanket["ThetaZ"].getExpectations(expand=True)
 
         # Get ARD sparsity or prior variance
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Z_nodes_GP.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Z_nodes_GP.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 
 # Import manually defined functions
 from .variational_nodes import (
     UnivariateGaussian_Unobserved_Variational_Node_with_MultivariateGaussian_Prior,
 )
 
+
 # Z_Node_GP
 class Z_GP_Node(
     UnivariateGaussian_Unobserved_Variational_Node_with_MultivariateGaussian_Prior
 ):
     """
     Z node with a Multivariate Gaussian prior and univariate Gaussian variational
     """
@@ -61,15 +62,14 @@
         """Method to fetch minibatch"""
         if self.mini_batch is None:
             return self.getExpectations()
         else:
             return self.mini_batch
 
     def updateParameters(self, ix=None, ro=1.0):
-
         # Get expectations from other nodes
         W = self.markov_blanket["W"].getExpectations()
         Y = self.markov_blanket["Y"].get_mini_batch()
         tau = self.markov_blanket["Tau"].get_mini_batch()
         mask = [self.markov_blanket["Y"].nodes[m].getMask() for m in range(len(Y))]
 
         if "AlphaZ" in self.markov_blanket:
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/Z_nodes_GP_mv.py` & `mofapy2-0.7.1/mofapy2/core/nodes/Z_nodes_GP_mv.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from mofapy2.core.distributions import *
 import scipy as s
 import numpy as np
 
 # Import manually defined functions
 from .variational_nodes import MultivariateGaussian_Unobserved_Variational_Node
 
+
 # Z_GP_Node_mv
 class Z_GP_Node_mv(MultivariateGaussian_Unobserved_Variational_Node):
     """
     Z node with a Multivariate Gaussian prior and variational distribution
     """
 
     def __init__(self, dim, pmean, pcov, qmean, qcov, qE=None, weight_views=False):
@@ -41,15 +42,14 @@
         """Method to fetch minibatch"""
         if self.mini_batch is None:
             return self.getExpectations()
         else:
             return self.mini_batch
 
     def updateParameters(self, ix=None, ro=1.0):
-
         # Get expectations from other nodes
         W = self.markov_blanket["W"].getExpectations()
         Y = self.markov_blanket["Y"].get_mini_batch()
         tau = self.markov_blanket["Tau"].get_mini_batch()
         mask = [self.markov_blanket["Y"].nodes[m].getMask() for m in range(len(Y))]
 
         if "Sigma" in self.markov_blanket:
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/ZgU_node.py` & `mofapy2-0.7.1/mofapy2/core/nodes/ZgU_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Import manually defined functions
 from .variational_nodes import UnivariateGaussian_Unobserved_Variational_Node
 
 # TODO :
 #  could be integrated in usual Z node (using a check if U is in Markov blanket)
 #  currentyl takes as N(0,1) prior for nonstuctured factors not flexible using pvar pmean
 
+
 # ZgU_node
 class ZgU_node(UnivariateGaussian_Unobserved_Variational_Node):
     """
     This nodes models Z in a model including inducing points U.
     As other updates and the ELBO only require marginal expectations of Z w.r.t q(Z,U) the node is a univariate variational distribution.
     Here we actually model q(z) = int q(z|u) q(u) du as their moment are required by all other nodes, the prior is not of importance and for simplicity set ot he variational distribution.
     """
@@ -55,15 +56,14 @@
         """Method to fetch minibatch"""
         if self.mini_batch is None:
             return self.getExpectations()
         else:
             return self.mini_batch
 
     def updateParameters(self, ix=None, ro=1.0):
-
         # Get expectations from other nodes
         U = self.markov_blanket["U"].getExpectations()
 
         assert (
             "Sigma" in self.markov_blanket
         ), "Sigma Node not found in Markov blanket of ZgU node."
         Sigma = self.markov_blanket["Sigma"].get_mini_batch()
@@ -181,15 +181,14 @@
             p_cov = Sigma["cov"]
         else:
             p_cov = self.P.params["cov"]
 
         # only non-stucutred nodes contribute here, else p(z|u) = q(z|u) --> ELBO is zero
         unstructured = (p_cov[k] == np.eye(p_cov[k].shape[0])).all()
         if unstructured:
-
             tmp1 = -0.5 * (QE2[:, k]).sum()
             tmp2 = 0
 
             lb_p = tmp1 + tmp2
             lb_q = -(np.log(Qvar[:, k])).sum() + self.dim[0] / 2.0
 
             return lb_p - lb_q - self.markov_blanket["U"].calculateELBO_k(k)
```

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/__init__.py` & `mofapy2-0.7.1/mofapy2/core/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/basic_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/multiview_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/multiview_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/nongaussian_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/nongaussian_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/nodes/variational_nodes.py` & `mofapy2-0.7.1/mofapy2/core/nodes/variational_nodes.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/core/utils.py` & `mofapy2-0.7.1/mofapy2/core/utils.py`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/notebooks/getting_started_python.ipynb` & `mofapy2-0.7.1/mofapy2/notebooks/getting_started_python.ipynb`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/notebooks/run_mofa_cpu_vs_gpu.py` & `mofapy2-0.7.1/mofapy2/notebooks/run_mofa_cpu_vs_gpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 
 #####################
 ## Parse arguments ##
 #####################
 
 parser = argparse.ArgumentParser()
-parser.add_argument('--gpu', action='store_true')
+parser.add_argument("--gpu", action="store_true")
 
 args, _ = parser.parse_known_args()
 
 ################################
 ## Load data in matrix format ##
 ################################
 
@@ -26,15 +26,17 @@
 #         datafile = "%s/%s_%s.txt.gz" % (datadir, views[m], sample_groups[g])
 #         data[m][g] = pd.read_csv(datafile, header=None, sep='\t')
 
 ####################################
 ## Load data in data.frame format ##
 ####################################
 
-data = pd.read_csv("ftp://ftp.ebi.ac.uk/pub/databases/mofa/getting_started/data.txt.gz", sep="\t")
+data = pd.read_csv(
+    "ftp://ftp.ebi.ac.uk/pub/databases/mofa/getting_started/data.txt.gz", sep="\t"
+)
 
 ##########
 ## MOFA ##
 ##########
 
 # initialise
 ent = entry_point()
@@ -45,15 +47,24 @@
 # Set data
 ent.set_data_df(data)
 
 # Set model options
 ent.set_model_options(factors=15)
 
 # Set training options
-ent.set_train_options(iter=50, freqELBO=1, dropR2=None, startELBO=1, verbose=False, seed=42, convergence_mode="fast", gpu_mode=args.gpu)
+ent.set_train_options(
+    iter=50,
+    freqELBO=1,
+    dropR2=None,
+    startELBO=1,
+    verbose=False,
+    seed=42,
+    convergence_mode="fast",
+    gpu_mode=args.gpu,
+)
 
 # Build the model
 ent.build()
 
 # Train the model
 ent.run()
```

### Comparing `mofapy2-0.7.0/mofapy2/run/entry_point.py` & `mofapy2-0.7.1/mofapy2/run/entry_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,45 +46,14 @@
                 )
             sys.stdout.flush()
             sys.exit()
 
     return saver
 
 
-def keyboardinterrupt_saver(func):
-    @wraps(func)
-    def saver(self, *args, **kwargs):
-        try:
-            func(self, *args, **kwargs)
-        # Internal methods will raise TypeError when interrupted
-        except (KeyboardInterrupt, TypeError):
-            if self.train_opts["save_interrupted"]:
-                print("Attempting to save the model at the current iteration...")
-                if self.train_opts["outfile"] is not None and self.train_opts != "":
-                    tmp_file = self.train_opts["outfile"]
-                    tmp_file = tmp_file.rstrip(".hdf5") + "_interrupted.hdf5"
-                else:
-                    tmp_file = os.path.join(
-                        "/tmp",
-                        "mofa_{}_interrupted.hdf5".format(strftime("%Y%m%d-%H%M%S")),
-                    )
-                self.save(outfile=tmp_file)
-                print(
-                    "Saved partially trained model in {}. Exiting now.".format(tmp_file)
-                )
-            else:
-                print(
-                    "Exiting now without saving the partially trained model. To save a partially trained model, set save_interrupted in the training options to true."
-                )
-            sys.stdout.flush()
-            sys.exit()
-
-    return saver
-
-
 class entry_point(object):
     def __init__(self):
         self.print_banner()
         self.dimensionalities = {"C": 0}
         self.model = None
 
         # flags
@@ -1062,15 +1031,14 @@
 
         # If to save the partially trained model when the training is interrupted
         self.train_opts["save_interrupted"] = save_interrupted
 
     def set_stochastic_options(
         self, learning_rate=1.0, forgetting_rate=0.0, batch_size=1.0, start_stochastic=1
     ):
-
         # Sanity checks
         if hasattr(self, "smooth_opts"):
             print(
                 "Stochastic inference is not possible when using covariates - train_opts['stochastic'] is set to False - consider using the option 'sparseGP' instead."
             )
             self.train_opts["stochastic"] = False
             return None
@@ -1109,15 +1077,14 @@
         warping_ref=0,
         warping_open_begin=True,
         warping_open_end=True,
         sparseGP=False,
         frac_inducing=None,
         warping_groups=None,
     ):
-
         """
         Method to activate and set options for a functional MOFA model (MEFISTO).
         This requires to specify a covariate using set_covariates.
 
         PARAMETERS:
         - scale_cov: Scale covariates to unit variance (relevant if you have multiple covariates on different scales). Default is False.
         - stat_opt: Iteration where to start the optimization of the hyperparameters for the Gaussian process
@@ -1257,15 +1224,14 @@
 
             print("##")
             print(
                 "## sparseGP set to True: using sparse Gaussian Process to speed up the training procedure"
             )
             print("##")
         else:
-
             self.smooth_opts["sparseGP"] = False
 
         # Define whether to model a group covariance structure
         self.smooth_opts["model_groups"] = model_groups
         if self.dimensionalities["G"] < 2:
             self.smooth_opts["model_groups"] = False
         # self.smooth_opts['use_gpytorch'] = False # experimental, this could be passed as a model_option but to keep options uncluttered set to False
@@ -1430,15 +1396,14 @@
         # Set training options
         self.model.setTrainOptions(self.train_opts)
 
         # Train the model
         train_model(self.model)
 
     def mask_outliers(self):
-
         Z = self.model.nodes["Z"].getExpectation()
         zscore_cutoff = 3 * 1.96  # z-score cutoff
         value_cutoff = 1  # max factor value
 
         for g in range(len(self.data_opts["groups_names"])):
             idx = np.where(
                 np.array(self.data_opts["samples_groups"])
```

### Comparing `mofapy2-0.7.0/mofapy2/run/test_data/view_0.txt` & `mofapy2-0.7.1/mofapy2/run/test_data/view_0.txt`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/run/test_data/view_1.txt` & `mofapy2-0.7.1/mofapy2/run/test_data/view_1.txt`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/run/test_data/view_2.txt` & `mofapy2-0.7.1/mofapy2/run/test_data/view_2.txt`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/run/test_data/with_nas/500_0.txt` & `mofapy2-0.7.1/mofapy2/run/test_data/with_nas/500_0.txt`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/run/test_data/with_nas/500_1.txt` & `mofapy2-0.7.1/mofapy2/run/test_data/with_nas/500_1.txt`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/run/test_data/with_nas/500_2.txt` & `mofapy2-0.7.1/mofapy2/run/test_data/with_nas/500_2.txt`

 * *Files identical despite different names*

### Comparing `mofapy2-0.7.0/mofapy2/simulate/simulate_mofa.py` & `mofapy2-0.7.1/mofapy2/simulate/simulate_mofa.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,15 @@
     for k in range(K):
         sig = Sigma[k]
         Zks.append(np.random.multivariate_normal(np.zeros(N * G), sig, 1))
     Zks = np.vstack(Zks).transpose()
 
     Z = []
     for g in range(G):
-        Z.append(
-            Zks[
-                groupidx == g,
-            ]
-        )
+        Z.append(Zks[groupidx == g,])
 
     # simulate alpha and theta, each factor should be active in at least one view
     theta = 0.5 * np.ones([M, K])
     if alpha is None:
         inactive = 1000
         active = 1
         alpha_tmp = [np.ones(M) * inactive] * K
```

### Comparing `mofapy2-0.7.0/pyproject.toml` & `mofapy2-0.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mofapy2"
-version = "0.7.0"
+version = "0.7.1"
 description = "Multi-omics factor analysis"
 authors = ['Ricard Argelaguet', 'Damien Arnol', 'Danila Bredikhin', 'Britta Velten']
 license = "LGPL-3.0"
 readme = 'README.md'
 repository = "https://github.com/gtca/mofapy2"
 homepage = "https:/biofam.github.io/MOFA2/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-numpy = "^1.21.0"
-pandas = "^1.2.0"
+numpy = "^1"
+pandas = "> 1"
 scipy = "~1"
 scikit-learn = "~1"
 h5py = "~3"
-anndata = { version = "~0.8", optional = true }
+anndata = { version = "> 0.8", optional = true }
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-anndata = "~0.8"
+pytest = "^7.4.2"
+anndata = "~0.9"
```

### Comparing `mofapy2-0.7.0/PKG-INFO` & `mofapy2-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: mofapy2
-Version: 0.7.0
+Version: 0.7.1
 Summary: Multi-omics factor analysis
 Home-page: https:/biofam.github.io/MOFA2/
 License: LGPL-3.0
 Author: Ricard Argelaguet
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anndata (>=0.8,<0.9)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anndata (>0.8)
 Requires-Dist: h5py (>=3,<4)
-Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: pandas (>=1.2.0,<2.0.0)
+Requires-Dist: numpy (>=1,<2)
+Requires-Dist: pandas (>1)
 Requires-Dist: scikit-learn (>=1,<2)
 Requires-Dist: scipy (>=1,<2)
 Project-URL: Repository, https://github.com/gtca/mofapy2
 Description-Content-Type: text/markdown
 
 # Multi-Omics Factor Analysis
 
-![PyPi version](https://img.shields.io/pypi/v/mofapy2)
+[![PyPi version](https://img.shields.io/pypi/v/mofapy2)](https://pypi.org/project/mofapy2)
 
 MOFA is a factor analysis model that provides a general framework for the integration of multi-omic data sets in an unsupervised fashion.  
 This repository contains `mofapy2` Python library source code.
 
 - For the downstream analysis in Python please check the mofax package: https://github.com/bioFAM/mofax
 - For the downstream analysis in R please check the MOFA2 package: https://github.com/bioFAM/MOFA2
```

