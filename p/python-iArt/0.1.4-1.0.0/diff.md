# Comparing `tmp/python-iArt-0.1.4.tar.gz` & `tmp/python-iArt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iArt-0.1.4.tar", last modified: Sun Nov 12 06:40:00 2023, max compression
+gzip compressed data, was "python-iArt-1.0.0.tar", last modified: Tue Apr  9 04:14:38 2024, max compression
```

## Comparing `python-iArt-0.1.4.tar` & `python-iArt-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2023-11-12 06:40:00.715236 python-iArt-0.1.4/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     3937 2023-11-12 06:40:00.715012 python-iArt-0.1.4/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     2637 2023-11-12 03:46:44.000000 python-iArt-0.1.4/README.md
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2023-11-12 06:40:00.713283 python-iArt-0.1.4/iArt/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2023-11-11 23:50:55.000000 python-iArt-0.1.4/iArt/__init__.py
--rw-r--r--   0 jiaweizhang   (501) staff       (20)    15328 2023-11-12 06:39:21.000000 python-iArt-0.1.4/iArt/iArt.py
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2023-11-12 06:40:00.714636 python-iArt-0.1.4/python_iArt.egg-info/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     3937 2023-11-12 06:40:00.000000 python-iArt-0.1.4/python_iArt.egg-info/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2023-11-12 06:40:00.000000 python-iArt-0.1.4/python_iArt.egg-info/SOURCES.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2023-11-12 06:40:00.000000 python-iArt-0.1.4/python_iArt.egg-info/dependency_links.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2023-11-12 06:40:00.000000 python-iArt-0.1.4/python_iArt.egg-info/requires.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2023-11-12 06:40:00.000000 python-iArt-0.1.4/python_iArt.egg-info/top_level.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2023-11-12 06:40:00.715331 python-iArt-0.1.4/setup.cfg
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2023-11-12 06:39:44.000000 python-iArt-0.1.4/setup.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-09 04:14:38.621149 python-iArt-1.0.0/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-09 04:14:38.620740 python-iArt-1.0.0/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.0.0/README.md
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-09 04:14:38.617679 python-iArt-1.0.0/iArt/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.0.0/iArt/__init__.py
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)    18113 2024-04-09 03:47:51.000000 python-iArt-1.0.0/iArt/iArt.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-09 04:14:38.619996 python-iArt-1.0.0/python_iArt.egg-info/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/requires.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/top_level.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-09 04:14:38.621318 python-iArt-1.0.0/setup.cfg
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-09 04:14:30.000000 python-iArt-1.0.0/setup.py
```

### Comparing `python-iArt-0.1.4/PKG-INFO` & `python-iArt-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 0.1.4
+Version: 1.0.0
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
         
@@ -12,17 +12,17 @@
         
         Jiawei Zhang*, Siyu Heng*, and Yang Feng (* indicates equal contribution)
         
         ## Maintainers
         
         Jiawei Zhang (Email: jz4721@nyu.edu), Siyu Heng (Email: siyuheng@nyu.edu), and Yang Feng (Email: yang.feng@nyu.edu)
         
-        ## Description
+        ## iArt (Imputation-Assisted Randomization Tests) Description
         
-        iArt (Imputation-Assisted Randomization Tests) is a Python package designed for conducting finite-population-exact randomization tests in design-based causal studies with missing outcomes. It offers a robust solution to handle missing data in causal inference, leveraging the potential outcomes framework and integrating various outcome imputation algorithms.
+        Design-based causal inference, also known as randomization-based or finite-population causal inference, is one of the most widely used causal inference frameworks, largely due to the merit that its statistical validity can be guaranteed by the study design (e.g., randomized experiments) and does not require assuming specific outcome-generating distributions or super-population models. Despite its advantages, design-based causal inference can still suffer from other data-related issues, among which outcome missingness is a prevalent and significant challenge. This work systematically studies the outcome missingness problem in design-based causal inference. First, we propose a general and flexible outcome missingness mechanism that can facilitate finite-population-exact randomization tests for the null effect. Second, under this flexible missingness mechanism, we propose a general framework called ``imputation and re-imputation" for conducting finite-population-exact randomization tests in design-based causal inference with missing outcomes. This framework can incorporate any imputation algorithms (from linear models to advanced machine learning-based imputation algorithms) while ensuring finite-population-exact type-I error rate control. Third, we extend our framework to conduct covariate adjustment in randomization tests and construct finite-population-valid confidence sets with missing outcomes. Our framework is evaluated via extensive simulation studies and applied to a large-scale randomized experiment. Corresponding \textsf{Python} and \textsf{R} packages are also developed.
         
         ## Installation
         
         To install [iArt](https://pypi.org/project/python-iArt/), run the following command:
         
         ```bash
         pip install python-iArt
```

### Comparing `python-iArt-0.1.4/README.md` & `python-iArt-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 Jiawei Zhang*, Siyu Heng*, and Yang Feng (* indicates equal contribution)
 
 ## Maintainers
 
 Jiawei Zhang (Email: jz4721@nyu.edu), Siyu Heng (Email: siyuheng@nyu.edu), and Yang Feng (Email: yang.feng@nyu.edu)
 
-## Description
+## iArt (Imputation-Assisted Randomization Tests) Description
 
-iArt (Imputation-Assisted Randomization Tests) is a Python package designed for conducting finite-population-exact randomization tests in design-based causal studies with missing outcomes. It offers a robust solution to handle missing data in causal inference, leveraging the potential outcomes framework and integrating various outcome imputation algorithms.
+Design-based causal inference, also known as randomization-based or finite-population causal inference, is one of the most widely used causal inference frameworks, largely due to the merit that its statistical validity can be guaranteed by the study design (e.g., randomized experiments) and does not require assuming specific outcome-generating distributions or super-population models. Despite its advantages, design-based causal inference can still suffer from other data-related issues, among which outcome missingness is a prevalent and significant challenge. This work systematically studies the outcome missingness problem in design-based causal inference. First, we propose a general and flexible outcome missingness mechanism that can facilitate finite-population-exact randomization tests for the null effect. Second, under this flexible missingness mechanism, we propose a general framework called ``imputation and re-imputation" for conducting finite-population-exact randomization tests in design-based causal inference with missing outcomes. This framework can incorporate any imputation algorithms (from linear models to advanced machine learning-based imputation algorithms) while ensuring finite-population-exact type-I error rate control. Third, we extend our framework to conduct covariate adjustment in randomization tests and construct finite-population-valid confidence sets with missing outcomes. Our framework is evaluated via extensive simulation studies and applied to a large-scale randomized experiment. Corresponding \textsf{Python} and \textsf{R} packages are also developed.
 
 ## Installation
 
 To install [iArt](https://pypi.org/project/python-iArt/), run the following command:
 
 ```bash
 pip install python-iArt
```

### Comparing `python-iArt-0.1.4/iArt/iArt.py` & `python-iArt-1.0.0/iArt/iArt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+# Description: This file contains the implementation of the Imputation-Assisted Randomization Tests (iArt) 
 import pandas as pd
 import numpy as np
 from statsmodels.stats.multitest import multipletests
 from sklearn.base import clone
 from sklearn.experimental import enable_iterative_imputer
 from sklearn.impute import IterativeImputer
+from sklearn.exceptions import DataConversionWarning
 from sklearn.exceptions import ConvergenceWarning
 from sklearn import linear_model
 import lightgbm as lgb
 import xgboost as xgb
 from sklearn.impute import SimpleImputer
 import time
-from sklearn.exceptions import DataConversionWarning
 import warnings
 
 def holm_bonferroni(p_values, alpha = 0.05):
     """
     Perform the Holm-Bonferroni correction on the p-values
     """
 
@@ -22,41 +23,84 @@
     reject, corrected_p_values, _, _ = multipletests(p_values, alpha=alpha, method='holm')
 
     # Check if any null hypothesis can be rejected
     any_rejected = any(reject)
 
     return any_rejected
 
-def getY(G, Z, X,Y, covariate_adjustment = False):
+def getY(G, Z, X,Y, covariate_adjustment = 0):
     """
     Calculate the imputed Y values using G and df_Z
     if covariate_adjustment is True, return the adjusted Y values based on predicted Y values and X
     else return the predicted Y values
     """
-    if covariate_adjustment:
-        G_adjusted = clone(G)
     df_Z = pd.DataFrame(np.concatenate((Z, X, Y), axis=1))
     # lenY is the number of how many columns are Y
     lenY = Y.shape[1]
     # indexY is the index of the first column of Y
     indexY = Z.shape[1] + X.shape[1]
     # fit the imputation model G
     df_imputed = G.fit_transform(df_Z)
 
     Y_head = df_imputed[:, indexY:indexY+lenY]
     X = df_imputed[:, 1:1+X.shape[1]]
-    if covariate_adjustment:
+    
+    if covariate_adjustment == 0:
+        return Y_head
+    
+    # suppress the warnings
+    warnings.filterwarnings('ignore', category=ConvergenceWarning)
+
+    if covariate_adjustment == 1:
         warnings.filterwarnings(action='ignore', category=DataConversionWarning)
         # use linear regression to adjust the predicted Y values based on X
-        lm = linear_model.LinearRegression()
-        lm.fit(X, Y_head)
-        Y_head_adjusted = lm.predict(X)
-        return Y_head - Y_head_adjusted
-    else:
-        return Y_head
+        Y_head_adjusted = np.zeros_like(Y_head)
+        for i in range(lenY):
+            # Extract the current target predictions
+            Y_current = Y_head[:, i]
+
+            # Fit the model to current target
+            lm = linear_model.BayesianRidge()
+            lm.fit(X, Y_current)
+
+            # Predict and adjust for the current target
+            Y_current_adjusted = lm.predict(X)
+            Y_head_adjusted[:, i] = Y_current - Y_current_adjusted
+
+        return Y_head_adjusted
+    
+    if covariate_adjustment == 2:
+        warnings.filterwarnings(action='ignore', category=DataConversionWarning)
+        # use xgboost to adjust the predicted Y values based on X
+        Y_head_adjusted = np.zeros_like(Y_head)
+        for i in range(lenY):
+            # Extract the current target predictions
+            Y_current = Y_head[:, i]
+
+            xg = xgb.XGBRegressor()
+            xg.fit(X, Y_current)
+            Y_current_adjusted = xg.predict(X)
+            Y_head_adjusted[:, i] = Y_current - Y_current_adjusted
+
+        return Y_head_adjusted
+    
+    if covariate_adjustment == 3:
+        warnings.filterwarnings(action='ignore', category=DataConversionWarning)
+        # use lightgbm to adjust the predicted Y values based on X
+        Y_head_adjusted = np.zeros_like(Y_head)
+        for i in range(lenY):
+            # Extract the current target predictions
+            Y_current = Y_head[:, i]
+
+            lgbm = lgb.LGBMRegressor()
+            lgbm.fit(X, Y_current)
+            Y_current_adjusted = lgbm.predict(X)
+            Y_head_adjusted[:, i] = Y_current - Y_current_adjusted
+        
+        return Y_head_adjusted
 
 def T(z,y):
     """
     Calculate the Wilcoxon rank sum test statistics
     """
 
     #the Wilcoxon rank sum test
@@ -125,58 +169,60 @@
         Z_sim_templates.append(Z_sim_template)
     return Z_sim_templates
 
 def getZsim(Z_sim_templates):
     """ 
     Shuffle each Z_sim template and concatenate them into a single permutated Z_sim array 
     """
-
     Z_sim = []
     for Z_sim_template in Z_sim_templates:
         strata_Z_sim = np.array(Z_sim_template.copy())
         np.random.shuffle(strata_Z_sim)
         Z_sim.append(strata_Z_sim)
     Z_sim = np.concatenate(Z_sim).reshape(-1, 1)
+
     return Z_sim
 
 def preprocess(Z, X, Y, S):
     """ 
     Preprocess the input variables, including reshaping, concatenating, sorting, and extracting
     """
 
     # Reshape Z, X, Y, S, M to (-1, 1) if they're not already in that shape
     Z = np.array(Z)
     X = np.array(X)
     Y = np.array(Y)
     X = X.reshape(-1, X.shape[1])
     Z = Z.reshape(-1, 1)
-    if S == None:
-        S = np.ones(Z.shape)
+
+    if S is None:
+        S = np.ones(Z.shape).reshape(-1, 1)
         M = np.isnan(Y).reshape(-1, Y.shape[1])
         return Z, X, Y, S, M
+    
     S = np.array(S)
     S = S.reshape(-1, 1)
 
     # Concatenate Z, X, Y, S, and M into a single DataFrame
     df = pd.DataFrame(np.concatenate((Z, X, Y, S), axis=1))
-
+    
     # Sort the DataFrame based on S (assuming S is the column before M)
     df = df.sort_values(by=df.columns[-1])
 
     # Extract Z, X, Y, S, and M back into separate arrays
     Z = df.iloc[:, :Z.shape[1]].values.reshape(-1, 1)
     X = df.iloc[:, Z.shape[1]:Z.shape[1] + X.shape[1]].values.reshape(-1, X.shape[1])
     Y = df.iloc[:, Z.shape[1] + X.shape[1]:Z.shape[1] + X.shape[1] + Y.shape[1]].values.reshape(-1, Y.shape[1])
     S = df.iloc[:, Z.shape[1] + X.shape[1] + Y.shape[1]:Z.shape[1] + X.shape[1] + Y.shape[1] + S.shape[1]].values.reshape(-1, 1)
 
     M = np.isnan(Y).reshape(-1, Y.shape[1])
     return Z, X, Y, S, M
 
 
-def check_param(Z, X, Y, S, G, L, verbose, covariate_adjustment,alpha,alternative,random_state):
+def check_param(*,Z, X, Y, S, G, L,mode, verbose, covariate_adjustment,alpha,alternative,random_state):
     """
     Check the validity of the input parameters
     """
 
     # check the dimension of Z, X, Y, S
     if Z.shape[0] != X.shape[0] or Z.shape[0] != Y.shape[0] or Z.shape[0] != S.shape[0]:
         raise ValueError("Z, X, Y, S must have the same number of rows")
@@ -206,51 +252,56 @@
         raise ValueError("alpha must be greater than 0 and less than or equal to 1")
     
     # Check G: Cannot be None
     if G is None:
         raise ValueError("G cannot be None")
     
     # Check covariate_adjustment: must be True or False
-    if covariate_adjustment not in [True, False, 1, 0]:
-        raise ValueError("covariate_adjustment must be True or False")
+    if covariate_adjustment not in [0, 1, 2, 3]:
+        raise ValueError("covariate_adjustment must be one of 0, 1, 2, 3")
 
     # Check alternative: must be one of "greater", "less" or "two-sided" 
     if alternative not in ["greater", "less", "two-sided"]:
         raise ValueError("alternative must be one of greater, less or two-sided")
     
     # Check random_state: must be an integer greater than 0 or None
-    if random_state != None and (not isinstance(random_state, int) or random_state <= 0):
-        raise ValueError("random_state must be an integer greater than 0 or None")
+    if random_state != None and (not isinstance(random_state, int) or random_state < 0):
+        raise ValueError("random_state must be an integer >= 0 or None")
+    
+    # Check mode: must be one of "strata" or "cluster"
+    if mode not in ["strata", "cluster"]:
+        raise ValueError("mode must be one of strata or cluster")
+    
     
 def choosemodel(G):
     """ 
     Choose the imputation model based on the input parameter G.
     If G is a string, choose the imputation model based on the string.
     If G is a function, return the function.
     """
 
     #if G is string
     if isinstance(G, str):
         G = G.lower()
         warnings.filterwarnings('ignore', category=ConvergenceWarning)
         if G == 'xgboost':
             G = IterativeImputer(estimator = xgb.XGBRegressor(), max_iter = 1)
-        if G == 'bayesianridge':
+        if G == 'linear':
             G = IterativeImputer(estimator = linear_model.BayesianRidge(), max_iter = 1,verbose=0)
         if G == 'median':
             G = SimpleImputer(missing_values=np.nan, strategy='median')
         if G == 'mean':
             G = SimpleImputer(missing_values=np.nan, strategy='mean')
         if G == 'lightgbm':
             G = IterativeImputer(estimator = lgb.LGBMRegressor(verbosity = -1), max_iter = 1)
-        if G == 'mice':
+        if G == 'iterative+linear':
             G = IterativeImputer(estimator = linear_model.BayesianRidge())
-        if G == 'mice+lightgbm':
+        if G == 'iterative+lightgbm':
             G = IterativeImputer(estimator = lgb.LGBMRegressor(verbosity = -1))
-        if G == 'mice+xgboost':
+        if G == 'iterative+xgboost':
             G = IterativeImputer(estimator = xgb.XGBRegressor())
     return G
 
 def transformX(X, threshold=0.1, verbose=True):
     """
     Imputes columns in the array X with a missing rate below the given threshold using median imputation.
     Parameters:
@@ -276,26 +327,26 @@
         imputed_columns.append(col)
     
     # Calculate missing rate after imputation
     missing_rate_after = np.isnan(X).mean(axis=0)
     
     # Columns that are not imputed
     not_imputed_columns = [col for col in range(X.shape[1]) if col not in imputed_columns]
-    
+
     if verbose:
         print(f"Missing Rate Before Imputation for X: {missing_rate * 100}")
         
         if len(columns_to_impute)>0:
             print(f"Missing Rate After Imputation for X: {missing_rate_after * 100}")
             print(f"Columns Imputed for X: {imputed_columns}")
         print(f"Columns Not Imputed for X: {not_imputed_columns}")
-
+    
     return X
 
-def test(*,Z, X, Y, G='bayesianridge', S=None,L = 10000,threshholdForX = 0.1,verbose = False, covariate_adjustment = False, random_state=None, alternative = "greater", alpha = 0.05):
+def test(*,Z, X, Y, G='bayesianridge', S=None,L = 10000,threshholdForX = 0.2, mode = 'strata',verbose = False, covariate_adjustment = 0, random_state=None, alternative = "greater", alpha = 0.05):
     """Imputation-Assisted Randomization Tests (iArt) for testing 
     the null hypothesis that the treatment has no effect on the outcome.
 
     Parameters
     ----------
     Z : array_like
         Z is the array of observed treatment indicators
@@ -312,19 +363,25 @@
     G : str or function, default: 'bayesianridge'
         A string for the eight available choice or a function that takes 
         (Z, M, Y_k) as input and returns the imputed complete values 
 
     L : int, default: 10000
         The number of Monte Carlo simulations 
 
+    mode : {'strata','cluster'}, default: 'strata'
+        A string indicating the randomization mode
+
     verbose : bool, default: False
         A boolean indicating whether to print training start and end 
 
-    covarite_adjustment : bool, default: False
-        A boolean indicating whether to do covariate adjustment ()
+    covarite_adjustment : int, default: 0
+        if 0, covariate adjustment is not used
+        if 1, ridge covariate adjustment is used
+        if 2, xgboost covariate adjustment is used
+        if 3, lightgbm covariate adjustment is used
 
     random_state : {None, int, `numpy.random.Generator`,`numpy.random.RandomState`}, default: None
         If `seed` is None (or `np.random`), the `numpy.random.RandomState`
         singleton is used.
         If `seed` is an int, a new ``RandomState`` instance is used,
         seeded with `seed`.
         If `seed` is already a ``Generator`` or ``RandomState`` instance then
@@ -347,16 +404,16 @@
     start_time = time.time()
 
     # preprocess the variable
     Z, X, Y, S, M = preprocess(Z, X, Y, S)
     X = transformX(X,threshholdForX,verbose)
 
     # Check the validity of the input parameters
-    check_param(Z, X, Y, S, G, L, verbose,covariate_adjustment,alpha,alternative,random_state)
-
+    check_param(Z=Z, X=X, Y=Y, S=S, G=G, L=L, mode=mode, verbose=verbose, covariate_adjustment=covariate_adjustment, alpha=alpha, alternative=alternative, random_state=random_state)
+    
     # Set random seed
     np.random.seed(random_state)
 
     # choose the imputation model
     G_model = choosemodel(G)
 
     # impuate the missing values to get the observed test statistics in part 1
@@ -375,20 +432,34 @@
             print("Covariate adjustment is not used")
         print("prediction Wilcoxon rank-sum test statistics:"+str(t_obs))
         #print wheather covariate adjustment is used
         print("=========================================================")
 
     # re-impute the missing values and calculate the observed test statistics in part 2
     t_sim = [ [] for _ in range(L)]
-    Z_sim_templates = getZsimTemplates(Z, S)
+    if mode == 'strata':
+        Z_sim_templates = getZsimTemplates(Z, S)
+    else:
+        p = 0.5
+        cluster_indices = np.unique(S)
+        num_clusters = len(cluster_indices)
+        cluster_sim_template = np.array([0.0] * int(num_clusters * p) + [1.0] * (num_clusters - int(num_clusters * p)))
 
     for l in range(L):
         
         # simulate treatment indicators
-        Z_sim = getZsim(Z_sim_templates)
+        if mode == 'strata':
+            Z_sim = getZsim(Z_sim_templates)
+        else:
+            cluster_sim = cluster_sim_template.copy()
+            np.random.shuffle(cluster_sim)
+            Z_sim = []
+            for s in S.flatten():
+                Z_sim.append(cluster_sim[int(s) - 1])
+            Z_sim = np.array(Z_sim).reshape(-1, 1)
 
         # impute the missing values and get the predicted Y values        
         Y_pred = getY(clone(G_model), Z_sim, X, Y, covariate_adjustment)
         
         # get the test statistics 
         t_sim[l] = getT(Y_pred, Z_sim, Y.shape[1], M)
 
@@ -414,8 +485,8 @@
 
     # perform Holm-Bonferroni correction
     reject = holm_bonferroni(p_values,alpha = alpha)
 
     if verbose:
         print("\nthe time used for the prediction and re-prediction framework:"+str(time.time() - start_time) + " seconds\n")
     
-    return reject, p_values
+    return reject, p_values
```

### Comparing `python-iArt-0.1.4/python_iArt.egg-info/PKG-INFO` & `python-iArt-1.0.0/python_iArt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 0.1.4
+Version: 1.0.0
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
         
@@ -12,17 +12,17 @@
         
         Jiawei Zhang*, Siyu Heng*, and Yang Feng (* indicates equal contribution)
         
         ## Maintainers
         
         Jiawei Zhang (Email: jz4721@nyu.edu), Siyu Heng (Email: siyuheng@nyu.edu), and Yang Feng (Email: yang.feng@nyu.edu)
         
-        ## Description
+        ## iArt (Imputation-Assisted Randomization Tests) Description
         
-        iArt (Imputation-Assisted Randomization Tests) is a Python package designed for conducting finite-population-exact randomization tests in design-based causal studies with missing outcomes. It offers a robust solution to handle missing data in causal inference, leveraging the potential outcomes framework and integrating various outcome imputation algorithms.
+        Design-based causal inference, also known as randomization-based or finite-population causal inference, is one of the most widely used causal inference frameworks, largely due to the merit that its statistical validity can be guaranteed by the study design (e.g., randomized experiments) and does not require assuming specific outcome-generating distributions or super-population models. Despite its advantages, design-based causal inference can still suffer from other data-related issues, among which outcome missingness is a prevalent and significant challenge. This work systematically studies the outcome missingness problem in design-based causal inference. First, we propose a general and flexible outcome missingness mechanism that can facilitate finite-population-exact randomization tests for the null effect. Second, under this flexible missingness mechanism, we propose a general framework called ``imputation and re-imputation" for conducting finite-population-exact randomization tests in design-based causal inference with missing outcomes. This framework can incorporate any imputation algorithms (from linear models to advanced machine learning-based imputation algorithms) while ensuring finite-population-exact type-I error rate control. Third, we extend our framework to conduct covariate adjustment in randomization tests and construct finite-population-valid confidence sets with missing outcomes. Our framework is evaluated via extensive simulation studies and applied to a large-scale randomized experiment. Corresponding \textsf{Python} and \textsf{R} packages are also developed.
         
         ## Installation
         
         To install [iArt](https://pypi.org/project/python-iArt/), run the following command:
         
         ```bash
         pip install python-iArt
```

### Comparing `python-iArt-0.1.4/setup.py` & `python-iArt-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python-iArt",
-    version="0.1.4",
+    version="1.0.0",
     author="Siyu Heng, Jiawei Zhang, and Yang Feng",
     author_email="siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu",
     description="iArt: A Generalized Framework for Imputation-Assisted Randomization Tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py",
     packages=find_packages(),
```

