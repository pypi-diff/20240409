# Comparing `tmp/tscluster-1.0.0.tar.gz` & `tmp/tscluster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscluster-1.0.0.tar", last modified: Mon Mar 25 09:32:11 2024, max compression
+gzip compressed data, was "tscluster-1.0.1.tar", last modified: Mon Apr  8 22:26:36 2024, max compression
```

## Comparing `tscluster-1.0.0.tar` & `tscluster-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.204117 tscluster-1.0.0/
--rw-rw-rw-   0        0        0      411 2024-03-25 09:32:11.203117 tscluster-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      145 2024-03-24 06:02:16.000000 tscluster-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-25 09:32:11.205116 tscluster-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      834 2024-03-25 09:30:55.000000 tscluster-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.064198 tscluster-1.0.0/tscluster/
--rw-rw-rw-   0        0        0        0 2024-03-24 06:02:16.000000 tscluster-1.0.0/tscluster/__init__.py
--rw-rw-rw-   0        0        0     2782 2024-03-25 09:06:17.000000 tscluster-1.0.0/tscluster/base.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.124164 tscluster-1.0.0/tscluster/metrics/
--rw-rw-rw-   0        0        0       55 2024-03-25 06:31:54.000000 tscluster-1.0.0/tscluster/metrics/__init__.py
--rw-rw-rw-   0        0        0     2329 2024-03-25 09:23:22.000000 tscluster-1.0.0/tscluster/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.161143 tscluster-1.0.0/tscluster/opttscluster/
--rw-rw-rw-   0        0        0       61 2024-03-24 06:02:16.000000 tscluster-1.0.0/tscluster/opttscluster/__init__.py
--rw-rw-rw-   0        0        0     9457 2024-03-24 06:02:16.000000 tscluster-1.0.0/tscluster/opttscluster/optcluster.py
--rw-rw-rw-   0        0        0    31854 2024-03-25 04:30:47.000000 tscluster-1.0.0/tscluster/opttscluster/opttscluster.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.181131 tscluster-1.0.0/tscluster/preprocessing/
--rw-rw-rw-   0        0        0       75 2024-03-24 06:02:16.000000 tscluster-1.0.0/tscluster/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     6912 2024-03-25 08:19:19.000000 tscluster-1.0.0/tscluster/preprocessing/base.py
--rw-rw-rw-   0        0        0     6070 2024-03-25 09:07:07.000000 tscluster-1.0.0/tscluster/preprocessing/scaler.py
--rw-rw-rw-   0        0        0     9292 2024-03-25 09:02:44.000000 tscluster-1.0.0/tscluster/preprocessing/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.201120 tscluster-1.0.0/tscluster/tskmeans/
--rw-rw-rw-   0        0        0      110 2024-03-24 06:02:16.000000 tscluster-1.0.0/tscluster/tskmeans/__init__.py
--rw-rw-rw-   0        0        0     1428 2024-03-25 09:14:32.000000 tscluster-1.0.0/tscluster/tskmeans/tsglobalkmeans.py
--rw-rw-rw-   0        0        0     1185 2024-03-25 09:14:20.000000 tscluster-1.0.0/tscluster/tskmeans/tskmeans.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:11.118166 tscluster-1.0.0/tscluster.egg-info/
--rw-rw-rw-   0        0        0      411 2024-03-25 09:32:10.000000 tscluster-1.0.0/tscluster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2024-03-25 09:32:10.000000 tscluster-1.0.0/tscluster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 09:32:10.000000 tscluster-1.0.0/tscluster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-03-25 09:32:10.000000 tscluster-1.0.0/tscluster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-25 09:32:10.000000 tscluster-1.0.0/tscluster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.737304 tscluster-1.0.1/
+-rw-rw-rw-   0        0        0      528 2024-04-08 22:26:36.734306 tscluster-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-01 13:24:00.000000 tscluster-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 22:26:36.739302 tscluster-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      864 2024-04-08 22:26:28.000000 tscluster-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.595385 tscluster-1.0.1/test/
+-rw-rw-rw-   0        0        0     5287 2024-03-26 00:06:35.000000 tscluster-1.0.1/test/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.610377 tscluster-1.0.1/tscluster/
+-rw-rw-rw-   0        0        0        0 2024-03-26 05:37:01.000000 tscluster-1.0.1/tscluster/__init__.py
+-rw-rw-rw-   0        0        0     8005 2024-04-08 21:19:03.000000 tscluster-1.0.1/tscluster/base.py
+-rw-rw-rw-   0        0        0     7733 2024-04-08 20:21:14.000000 tscluster-1.0.1/tscluster/interface.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.670341 tscluster-1.0.1/tscluster/metrics/
+-rw-rw-rw-   0        0        0       55 2024-03-25 06:31:54.000000 tscluster-1.0.1/tscluster/metrics/__init__.py
+-rw-rw-rw-   0        0        0     5905 2024-04-08 10:53:03.000000 tscluster-1.0.1/tscluster/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.687331 tscluster-1.0.1/tscluster/opttscluster/
+-rw-rw-rw-   0        0        0       61 2024-03-24 06:02:16.000000 tscluster-1.0.1/tscluster/opttscluster/__init__.py
+-rw-rw-rw-   0        0        0     9457 2024-03-24 06:02:16.000000 tscluster-1.0.1/tscluster/opttscluster/optcluster.py
+-rw-rw-rw-   0        0        0    35161 2024-04-08 21:06:46.000000 tscluster-1.0.1/tscluster/opttscluster/opttscluster.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.708320 tscluster-1.0.1/tscluster/preprocessing/
+-rw-rw-rw-   0        0        0       75 2024-03-24 06:02:16.000000 tscluster-1.0.1/tscluster/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2289 2024-04-06 08:25:25.000000 tscluster-1.0.1/tscluster/preprocessing/interface.py
+-rw-rw-rw-   0        0        0     5695 2024-04-06 08:32:11.000000 tscluster-1.0.1/tscluster/preprocessing/scaler.py
+-rw-rw-rw-   0        0        0    19702 2024-04-08 10:11:53.000000 tscluster-1.0.1/tscluster/preprocessing/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.718313 tscluster-1.0.1/tscluster/tskmeans/
+-rw-rw-rw-   0        0        0      110 2024-03-24 06:02:16.000000 tscluster-1.0.1/tscluster/tskmeans/__init__.py
+-rw-rw-rw-   0        0        0     7024 2024-04-08 19:48:30.000000 tscluster-1.0.1/tscluster/tskmeans/tsglobalkmeans.py
+-rw-rw-rw-   0        0        0     6658 2024-04-08 19:48:26.000000 tscluster-1.0.1/tscluster/tskmeans/tskmeans.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.731307 tscluster-1.0.1/tscluster/tsplot/
+-rw-rw-rw-   0        0        0       56 2024-04-07 01:33:17.000000 tscluster-1.0.1/tscluster/tsplot/__init__.py
+-rw-rw-rw-   0        0        0    17566 2024-04-08 13:42:30.000000 tscluster-1.0.1/tscluster/tsplot/tsplot.py
+drwxrwxrwx   0        0        0        0 2024-04-08 22:26:36.663345 tscluster-1.0.1/tscluster.egg-info/
+-rw-rw-rw-   0        0        0      528 2024-04-08 22:26:36.000000 tscluster-1.0.1/tscluster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2024-04-08 22:26:36.000000 tscluster-1.0.1/tscluster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 22:26:36.000000 tscluster-1.0.1/tscluster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-04-08 22:26:36.000000 tscluster-1.0.1/tscluster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 22:26:36.000000 tscluster-1.0.1/tscluster.egg-info/top_level.txt
```

### Comparing `tscluster-1.0.0/setup.py` & `tscluster-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
    name='tscluster',
-   version='1.0.0',
+   version='1.0.1',
    description='A useful package for temporal clustering',
    license="MIT",
    long_description=long_description,
    long_description_content_type="text/markdown",
    author='Jolomi Tosanwumi',
    author_email='tjolomi@gmail.com',
    #url="...",
    packages=find_packages(), 
-   #python_requires='>=3.9',
+   #python_requires='>=3.9.18',
    install_requires=[
        'numpy>=1.26', 
        'scipy>=1.10', 
        'gurobipy>=11.0', 
        'tslearn>=0.6.3',   
        'h5py>=3.10',
-       'pandas>=2.2'
+       'pandas>=2.2',
+       'matplotlib>=3.8'
        ], #external packages as dependencies on TEST pypi
    #ToDo: on real pypi: ['numpy==1.26.4', 'scipy==1.12.0', 'gurobipy==11.0.1']. Also considering using >= a lowerbound
 )
```

### Comparing `tscluster-1.0.0/tscluster/opttscluster/optcluster.py` & `tscluster-1.0.1/tscluster/opttscluster/optcluster.py`

 * *Files identical despite different names*

### Comparing `tscluster-1.0.0/tscluster/opttscluster/opttscluster.py` & `tscluster-1.0.1/tscluster/opttscluster/opttscluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,89 +6,106 @@
 import copy
 
 import numpy as np
 import numpy.typing as npt
 from scipy.cluster.vq import kmeans, vq
 import gurobipy as gp
 
+from tscluster.interface import TSClusterInterface
 from tscluster.base import TSCluster
 from tscluster.opttscluster import optcluster
 from tscluster.preprocessing.utils import infer_data
 
-class OptTSCluster(TSCluster):
+class OptTSCluster(TSCluster, TSClusterInterface):
+
+    """
+    Class for optimal time-series clustering. Throughout this doc and code, 'z' refers to cluster centers, while 'c' to label assignment.
+    This creates an OptTSCluster object
+
+    Parameters
+    -----------
+    k: int
+        number of clusters
+    scheme: {'z0c0', 'z0c1', 'z1c0', 'z1c1'}, default='z1c0'
+        The scheme to use for tsclustering. Could be one of:
+            - 'z0c0' means fixed center, fixed assignment
+            - 'z0c1' means fixed center, changing assignment
+            - 'z1c0' means changing center, fixed assignment
+            - 'z1c1' means changing center, changing assignment
+        Scheme needs to be a dynamic label assignment scheme (either 'z1c1' or 'z0c1') when using constrained cluster change (either with `n_allow_assignment_change` or `lagrangian_multiplier`)
+    n_allow_assignment_change: int or None, default=None
+        total number of label changes to allow
+    is_Z_positive: bool, default=True
+        True means assume non-negativity constraint for z. The scale of the final results are not affected since OptTSCluster will return solutions in the original scale of the input data.
+        Setting this to True often leads to speedup. See ... for more details.  
+    is_tight_constraints: bool, default=True
+        Indicate if to use use tight bounds (the bounding box of the data) for z and the objective value
+    lagrangian_multiplier: float, default=0.0
+        The penalty term for constrained label changes. Value should be in range [0, np.inf], the higher the value, the less the number of label changes allowed. When used, `n_allow_assignment_change` is ignored.
+    use_sum_distance: bool, default=False
+        Indicate if to use sum of distance to cluster as the objective. This is the sum of the distances between points in a time series
+        and their centroids. 
+    warm_start: bool, default=True
+        Indicates if to use k-means to initialize the centroids (Z) and their assignments (C).
+    normalise_assignment_penalty: bool, default=True
+        Indicate if to normalize the penalty term when using lagrangian_multiplier
+    strictly_n_allow_assignment_change: bool, default=False
+        If True, indicate if to use n_allow_assignment_change constraint as an active constraint.
+    use_MILP_centroid: bool, default=True
+        If True, cluster_centers_ atrribute will be cluster centers obtained from MILP solution, else the average of the 
+        datapoints per timestep
+    use_full_constraints: bool, default=True
+        If True, use all the samples as constraints. If False, use constraint generation. When using constraint generation, 
+        subsamples are being used as constraints with samples added to the constraints until optimal solution is found.
+    IFrac: float, default=0.2
+        fraction of samples to use as initial constraints when using constraint generation.
+    top_n_percentile: foat, default=0.0
+        percentile of most violated constraints to add to constraints when using constraint generation. 
+        Value should in range [0, 1]. Note that a value of 0 means to use the most violated constraint. 
+    max_iter: int, default=10
+        Maximum number of iterations to use when using constraint violation.
+    random_state: int, default=None
+        Set the random seed used when initializing with k-means or when initializing samples when using constraint generation.
+    add_constraint_per_cluster: bool, default=True
+        If True, top_n_percentile constraints are being from each cluster when using constraint generation. 
+    init_with_prev: bool, default=True
+        If True, use the solution from previous iteration as initial solution for the next iteration when using constraint generation            
+    
+    Attributes
+    ----------
+    cluster_centers_
+    fitted_data_shape_
+    labels_
+    label_dict_
+    n_changes_
+    
+    """
+
     def __init__(
             self, 
             k: int, 
             scheme: str = 'z1c0', 
             n_allow_assignment_change: None|int = None, 
             is_Z_positive: bool = True, 
             is_tight_constraints: bool = True, 
-            lagrangian_multiplier: int = 0, 
+            lagrangian_multiplier: float = 0.0, 
             use_sum_distance: bool = False,
             warm_start: bool = True, 
             normalise_assignment_penalty: bool = True, 
             strictly_n_allow_assignment_change: bool = False, 
             use_MILP_centroid: bool = True,
             use_full_constraints: bool = True, 
             IFrac: float = 0.2, 
             top_n_percentile: float = 0.0, 
             max_iter: int = 10, 
             random_state: None|int = None, 
             add_constraint_per_cluster: bool = True,
             init_with_prev: bool = True
             ) -> None:
 
-        """
-        Class for optimal time-series clustering. Throughout this doc and code, 'z' refers to cluster centers, while 'c' to label assignment.
-        This creates an OptTSCluster object
-
-        k: int
-            number of clusters
-        scheme: {'z0c0', 'z0c1', 'z1c0', 'z1c1'}, default='z1c0'
-            the scheme to use for tsclustering
-        n_allow_assignment_change: int or None, default=None
-            total number of label changes to allow
-        is_Z_positive: bool, default=True
-            True means assume non-negativity constraint for z. The scale of the final results are not affected since OptTSCluster will return solutions in the original scale of the input data.
-            Setting this to True often leads to speedup. See ... for more details.  
-        is_tight_constraints: bool, default=True
-            Indicate if to use use tight bounds (the bounding box of the data) for z and the objective value
-        lagrangian_multiplier: int, default=0
-            The penalty term for constrained label changes. Value should be in range [0, np.inf], the higher the value, the less
-            the number of label changes allowed
-        use_sum_distance: bool, default=False
-            Indicate if to use sum of distance to cluster as the objective. This is the sum of the distances between points in a time series
-            and their centroids. 
-        warm_start: bool, default=True
-            Indicates if to use k-means to initialize the centroids (Z) and their assignments (C).
-        normalise_assignment_penalty: bool, default=True
-            Indicate if to normalize the penalty term when using lagrangian_multiplier
-        strictly_n_allow_assignment_change: bool, default=False
-            If True, indicate if to use n_allow_assignment_change constraint as an active constraint.
-        use_MILP_centroid: bool, default=True
-            If True, cluster_centers_ atrribute will be cluster centers obtained from MILP solution, else the average of the 
-            datapoints per timestep
-        use_full_constraints: bool, default=True
-            If True, use all the samples as constraints. If False, use constraint generation. When using constraint generation, 
-            subsamples are being used as constraints with samples added to the constraints until optimal solution is found.
-        IFrac: float, default=0.2
-            fraction of samples to use as initial constraints when using constraint generation.
-        top_n_percentile: foat, default=0.0
-            percentile of most violated constraints to add to constraints when using constraint generation. 
-            Value should in range [0, 1]. Note that a value of 0 means to use the most violated constraint. 
-        max_iter: int, default=10
-            Maximum number of iterations to use when using constraint violation.
-        random_state: int, default=None
-            Set the random seed used when initializing with k-means or when initializing samples when using constraint generation.
-        add_constraint_per_cluster: bool, default=True
-            If True, top_n_percentile constraints are being from each cluster when using constraint generation. 
-        init_with_prev: bool, default=True
-            If True, use the solution from previous iteration as initial solution for the next iteration when using constraint generation        
-        """
-
         self.k = k
         self.scheme = scheme.lower()
         self.n_allow_assignment_change = n_allow_assignment_change
         self.is_Z_positive = is_Z_positive
         self.is_tight_constraints = is_tight_constraints 
         self.lagrangian_multiplier = lagrangian_multiplier
         self.use_sum_distance = use_sum_distance
@@ -120,36 +137,49 @@
         if re.search("c0", self.scheme, flags=re.IGNORECASE):
             self.n_allow_assignment_change = 0
 
         self.constant_assigment_constraint_violation_scheme = 'allow_v_violations_in_total'
 
         self.x_min = 0
 
-    @infer_data
     def fit(
             self, 
-            X: npt.NDArray[np.float64] | npt.NDArray[np.int64], 
-            y: npt.NDArray[np.float64] | npt.NDArray[np.int64] | None = None, 
+            X: npt.NDArray[np.float64], 
+            label_dict: dict|None = None, 
             verbose: bool = True, 
-            print_to: TextIO = sys.stdout, 
+            print_to: TextIO = sys.stdout,
+            **kwargs
             ) -> "OptTSCluster": 
 
         """
-        Method for solving the MILP model.
-
-        X: np.ndarray of shape (T, N, F)
-            T is the number of timesteps, N is the number of timeseries entities, F is the number of features. The input data to cluster
-        y: ignored, not used. Only present as a convention for fit methods of most models.
-        verbose: bool, default=True
+        Method for fitting the model by solving the MILP model.
+        
+        Parameters
+        -----------
+        X : numpy array
+            Input time series data. Should be a 3 dimensional array in TNF fromat.
+        label_dict : dict, default=None
+            A dictionary of the labels of X. Keys should be 'T', 'N', and 'F' (which are the number of time steps, entities, and features respectively). Value of each key is a list such that the value of key:
+                - 'T' is a list of names/labels of each time step used as index of each dataframe during fit. Default is range(0, T). Where T is the number of time steps in the fitted data
+                - 'N' is a list of names/labels of each entity used as index of the dataframe. Default is range(0, N). Where N is the number of entities/observations in the fitted data 
+                - 'F' is a list of names/labels of each feature used as column of each dataframe. Default is range(0, F). Where F is the number of features in the fitted data 
+            data_loader function from tscluster.preprocessing.utils can help in getting label_dict of a data. 
+        verbose : bool, default=True
             If True, some model training information will be printed out. Set to False to surpress printouts
-        print_to: TextIO, default=sys.stdout
+        print_to : TextIO, default=sys.stdout
             An object with a write method to write model's printout information during training. Default is standard output.
 
-        Return: self, fitted OptTSCluster object. 
+        Returns
+        --------
+        self : 
+            The fitted OptTSCluster object.
         """
+
+        self._label_dict_ = label_dict
+
         epsilon = 1e-4
         verbose_flush = True 
 
         self.verbose = verbose
         self.T_, self.N_, self.F_ = X.shape
         self.X_ = copy.deepcopy(X)
 
@@ -293,22 +323,29 @@
         has_any_new_constraint = True
 
         if self.use_full_constraints:
             self.max_iter = 1
 
         while ((E_hat > E_star+epsilon).sum() > 0 or has_any_new_constraint) and count < self.max_iter+1:
 
-            z_fixed = False
+            self.z_fixed = False
             if re.search("z0", self.scheme, flags=re.IGNORECASE):
-                z_fixed = True
+                self.z_fixed = True
+
+            self.c_fixed = False
+            if re.search("c0", self.scheme, flags=re.IGNORECASE):
+                self.c_fixed = True        
 
+            _get_model_size = kwargs.get('_get_model_size', False)
+                
             solver_time_0 = time()
-            E_star, Z_ans, C_ans = OptTSCluster.solve_ts_MILP(I, self.k, 
+            res = OptTSCluster.solve_ts_MILP(I, self.k, 
                                                                     n_allow_assignment_change=self.n_allow_assignment_change,
-                                                                    z_fixed=z_fixed,
+                                                                    z_fixed=self.z_fixed,
+                                                                    _get_model_size=_get_model_size,
                             constant_assigment_constraint_violation_scheme=self.constant_assigment_constraint_violation_scheme,
                                                                     init_Z=init_Zs,
                                                                     init_C=init_Cs,
                                                 strictly_n_allow_assignment_change=self.strictly_n_allow_assignment_change,
                                                 z_max=z_max,
                                                 z_min=z_min,
                                                 e_max=e_max,
@@ -316,31 +353,36 @@
                                                 is_Z_positive=self.is_Z_positive,
                                                 is_tight_constraints=self.is_tight_constraints,
                                                 lagrangian_multiplier=self.lagrangian_multiplier,
                                                 normalise_assignment_penalty=self.normalise_assignment_penalty,
                                                 use_sum_distance=self.use_sum_distance
                                                                     )
             
+            if _get_model_size:
+                return res 
+            
+            E_star, Z_ans, C_ans = res
+            
             solver_times.append(np.round(time() - solver_time_0, 2))
 
             C_hat = OptTSCluster.assign_cluster(X, Z_ans) # C_hat contains assignment for all datapoints, while
                                                         # C_ans contains only for those used for solving the MILP.
 
             if not self._use_closest_center_for_all: #and self.scheme in ['z1c0']:
                 C_hat[:, I_idx, :] = C_ans
 
             return_E_hat_per_t = False
             # if self.scheme in ['z1c1', 'z1c1_1']:
             #     return_E_hat_per_t = True  
 
             percent_data_used.append(np.round(100*I.size/X.size, 2))
 
-            if self.verbose:
-                print(file=print_to, flush=verbose_flush)
-                print(f"{percent_data_used[-1]}% of data used", file=print_to, flush=verbose_flush)
+            # if self.verbose:
+            #     print(file=print_to, flush=verbose_flush)
+            #     print(f"{percent_data_used[-1]}% of data used", file=print_to, flush=verbose_flush)
 
             if self.use_sum_distance:
                 E_hat, I_add, zi = E_star, [], []
             else:
                 E_hat, I_add, zi = OptTSCluster.add_constraints(X, Z_ans, C_hat, 
                                                                         n_allow_assignment_change=self.n_allow_assignment_change,
                     constant_assigment_constraint_violation_scheme=self.constant_assigment_constraint_violation_scheme,
@@ -371,15 +413,15 @@
                 # if self.scheme == 'z0c1_2':
                 #     Xt = X.reshape(X.shape[0]*X.shape[1], X.shape[2])
                 #     I = Xt[I_idx, :]
                 # else:
             I = X[:, I_idx, :]
 
             if self.verbose:    
-                print(f"Done with {count} of {self.max_iter}. Ehat: {E_hat}, Estar: {E_star}", file=print_to, flush=verbose_flush)
+                print(f"Obj val: {E_star}", file=print_to, flush=verbose_flush)
                 print(file=print_to, flush=verbose_flush)
         
                 count += 1
 
             if self.init_with_prev:
                 init_Zs = Z_ans 
                 init_Cs = C_hat  
@@ -406,43 +448,80 @@
         if self.warm_start:
             self.warm_start_Z_ = Z + self.x_min
             self.warm_start_labels_ = km_labels
 
         if self.verbose:
             print(f"Total time is {np.round(time() - t0, 2)}secs", file=print_to, flush=verbose_flush)  
             print(file=print_to, flush=verbose_flush)
+        
+        self.Zs_ans_avg = None 
+
+        if not self.use_MILP_centroid:
+            labels = self.labels_
 
+            self.Zs_ans_avg = np.zeros((self.T_, self.k, self.F_))
+
+            for t in range(self.T_):
+                for j in range(self.k):
+                    _idx = labels[:, t] == j
+                    self.Zs_ans_avg[t, j, :] = np.mean(self.X_[t, _idx, :], axis=0)
+    
         return self 
         
     @property
     def cluster_centers_(self):
         if self.use_MILP_centroid:
             return self.Zs_ans_[-1]
-        
-        labels_ = self.labels_
-
-        Zs_ans_ = np.zeros((self.T_, self.k, self.F_))
+        else:
+            return self.Zs_ans_avg
 
-        for t in range(self.T_):
-            for j in range(self.k):
-                idx = labels_[:, t] == j
-                Zs_ans_[t, j, :] = np.mean(self.X_[t, idx, :], axis=0)
+    @property
+    def labels_(self):
+        c = np.argmax(self.Cs_hats_[-1], axis=-1).T
 
-        return Zs_ans_
+        if self.c_fixed:
+            return c[:, 0]
+        return c
 
     @property
-    def labels_(self):
-        return np.argmax(self.Cs_hats_[-1], axis=-1).T
+    def fitted_data_shape_(self) -> Tuple[int, int, int]:
+        """
+        returns a tuple of the shape of the fitted data in TNF format. E.g (T, N, F) where T, N, and F are the number of timesteps,
+        observations, and features respectively. 
+        """
+        return self.T_, self.N_, self.F_
+
+    def get_model_size(self,
+            X: npt.NDArray[np.float64]
+            ) -> Tuple:
+        
+        """
+        Method to return the size of the model as a tuple of (v, c). Wehre v is the number of variables, and c is the number of constraints
+
+        Paramters
+        ---------
+        X : numpy array
+            Input time series data. Should be a 3 dimensional array in TNF fromat.        
+
+        Returns
+        -------
+        number of variable
+            The number of variables in the model
+        number of constraints
+            The number of constraints
+        """
+        return self.fit(X, _get_model_size=True, verbose=False)
 
     @staticmethod
     def solve_ts_MILP(
         I: npt.NDArray[np.float64] | npt.NDArray[np.int64], 
         k: int, 
         init_Z: npt.NDArray[np.float64] | npt.NDArray[np.int64] | None = None, 
         init_C: npt.NDArray[np.float64] | npt.NDArray[np.int64] | None = None, 
+        _get_model_size: bool = False,
         **kwargs
         ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64], npt.NDArray[np.float64]]:
 
         # MILP
         m = gp.Model()
 
         z_fixed = False
@@ -600,14 +679,22 @@
         else:
             if use_sum_distance:
                 m.setObjective(gp.quicksum(E[tt, ii] for tt in range(T) for ii in range(N)), gp.GRB.MINIMIZE)
             else:
                 m.setObjective(E, gp.GRB.MINIMIZE)
 
         m.setParam('OutputFlag', 0)
+
+        if _get_model_size:
+            m.update()
+
+            num_vars = m.NumVars
+            num_constraints = m.NumConstrs
+
+            return num_vars, num_constraints
         
         m.optimize() 
         
         if z_fixed:
             Z_ans = np.zeros((k, F))
         else:
             Z_ans = np.zeros((T, k, F))
@@ -739,29 +826,29 @@
         verbose = kwargs['verbose']
 
         if scheme == "allow_v_violations_in_total":
             n_violations = 0
             for i in range(C_hat.shape[1]):
                 y = np.argmax(C_hat[:, i, :], axis=1)
                 if (y[:-1] != y[1:]).sum() > 0:
-                    if verbose:
-                        print(f"i that changed: {i}", file=kwargs['print_to'])
+                    # if verbose:
+                    #     print(f"i that changed: {i}", file=kwargs['print_to'])
                     I_add.append(i)
                     # I_add_all.append(i)
                     n_violations += (y[:-1] != y[1:]).sum()
 
             # if n_violations <= v:
             #     I_add = []
             
         elif scheme == 'allow_v_violations_per_i':
             for i in range(C_hat.shape[1]):
                 y = np.argmax(C_hat[:, i, :], axis=1)
                 if (y[:-1] != y[1:]).sum() > v:
-                    if verbose:
-                        print(f"i that changed: {i}", file=kwargs['print_to'])
+                    # if verbose:
+                    #     print(f"i that changed: {i}", file=kwargs['print_to'])
                     I_add.append(i)
                     # I_add_all.append(i)
 
         return I_add#, I_add_all
 
 if __name__ == "__main__":
     pass
```

### Comparing `tscluster-1.0.0/tscluster.egg-info/SOURCES.txt` & `tscluster-1.0.1/tscluster.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 README.md
 setup.py
+test/test_main.py
 tscluster/__init__.py
 tscluster/base.py
+tscluster/interface.py
 tscluster.egg-info/PKG-INFO
 tscluster.egg-info/SOURCES.txt
 tscluster.egg-info/dependency_links.txt
 tscluster.egg-info/requires.txt
 tscluster.egg-info/top_level.txt
 tscluster/metrics/__init__.py
 tscluster/metrics/metrics.py
 tscluster/opttscluster/__init__.py
 tscluster/opttscluster/optcluster.py
 tscluster/opttscluster/opttscluster.py
 tscluster/preprocessing/__init__.py
-tscluster/preprocessing/base.py
+tscluster/preprocessing/interface.py
 tscluster/preprocessing/scaler.py
 tscluster/preprocessing/utils.py
 tscluster/tskmeans/__init__.py
 tscluster/tskmeans/tsglobalkmeans.py
-tscluster/tskmeans/tskmeans.py
+tscluster/tskmeans/tskmeans.py
+tscluster/tsplot/__init__.py
+tscluster/tsplot/tsplot.py
```

