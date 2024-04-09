# Comparing `tmp/glhmm-0.2.3.tar.gz` & `tmp/glhmm-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glhmm-0.2.3.tar", last modified: Thu Mar 14 15:01:50 2024, max compression
+gzip compressed data, was "glhmm-0.2.4.tar", last modified: Tue Apr  9 13:52:53 2024, max compression
```

## Comparing `glhmm-0.2.3.tar` & `glhmm-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-14 15:01:50.757474 glhmm-0.2.3/
--rw-r--r--   0 admin      (501) staff       (20)    35149 2023-03-08 15:43:34.000000 glhmm-0.2.3/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)      777 2024-03-14 15:01:50.756499 glhmm-0.2.3/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      955 2024-01-20 15:34:38.000000 glhmm-0.2.3/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-14 15:01:50.748705 glhmm-0.2.3/glhmm/
--rw-r--r--   0 admin      (501) staff       (20)    16487 2024-01-20 15:34:39.000000 glhmm-0.2.3/glhmm/auxiliary.py
--rw-r--r--   0 admin      (501) staff       (20)    82042 2024-03-14 14:54:33.000000 glhmm-0.2.3/glhmm/glhmm.py
--rw-r--r--   0 admin      (501) staff       (20)    55170 2024-02-28 16:36:16.000000 glhmm-0.2.3/glhmm/graphics.py
--rw-r--r--   0 admin      (501) staff       (20)    11236 2024-02-28 16:36:16.000000 glhmm-0.2.3/glhmm/io.py
--rw-r--r--   0 admin      (501) staff       (20)    65084 2023-12-12 10:51:17.000000 glhmm-0.2.3/glhmm/palm_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    87246 2023-12-12 10:51:17.000000 glhmm-0.2.3/glhmm/prediction.py
--rw-r--r--   0 admin      (501) staff       (20)    16779 2023-05-14 21:28:03.000000 glhmm-0.2.3/glhmm/preproc.py
--rw-r--r--   0 admin      (501) staff       (20)   131139 2024-02-28 16:36:16.000000 glhmm-0.2.3/glhmm/statistics.py
--rw-r--r--   0 admin      (501) staff       (20)    10443 2023-03-14 13:09:07.000000 glhmm-0.2.3/glhmm/utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-14 15:01:50.754442 glhmm-0.2.3/glhmm.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      777 2024-03-14 15:01:50.000000 glhmm-0.2.3/glhmm.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      373 2024-03-14 15:01:50.000000 glhmm-0.2.3/glhmm.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-14 15:01:50.000000 glhmm-0.2.3/glhmm.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-18 19:06:24.000000 glhmm-0.2.3/glhmm.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)      141 2024-03-14 15:01:50.000000 glhmm-0.2.3/glhmm.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        6 2024-03-14 15:01:50.000000 glhmm-0.2.3/glhmm.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)      358 2023-03-23 12:02:32.000000 glhmm-0.2.3/pyproject.toml
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-03-14 15:01:50.757649 glhmm-0.2.3/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      581 2024-03-14 15:00:57.000000 glhmm-0.2.3/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 13:52:53.915955 glhmm-0.2.4/
+-rw-r--r--   0 admin      (501) staff       (20)    35149 2023-03-08 15:43:34.000000 glhmm-0.2.4/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)      775 2024-04-09 13:52:53.915430 glhmm-0.2.4/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      942 2024-03-25 09:06:49.000000 glhmm-0.2.4/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 13:52:53.911255 glhmm-0.2.4/glhmm/
+-rw-r--r--   0 admin      (501) staff       (20)    16487 2024-01-20 15:34:39.000000 glhmm-0.2.4/glhmm/auxiliary.py
+-rw-r--r--   0 admin      (501) staff       (20)    85908 2024-04-09 13:48:56.000000 glhmm-0.2.4/glhmm/glhmm.py
+-rw-r--r--   0 admin      (501) staff       (20)    69169 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/graphics.py
+-rw-r--r--   0 admin      (501) staff       (20)    11236 2024-02-28 16:36:16.000000 glhmm-0.2.4/glhmm/io.py
+-rw-r--r--   0 admin      (501) staff       (20)    65221 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/palm_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    87246 2023-12-12 10:51:17.000000 glhmm-0.2.4/glhmm/prediction.py
+-rw-r--r--   0 admin      (501) staff       (20)    16779 2023-05-14 21:28:03.000000 glhmm-0.2.4/glhmm/preproc.py
+-rw-r--r--   0 admin      (501) staff       (20)   136831 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/statistics.py
+-rw-r--r--   0 admin      (501) staff       (20)    11894 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 13:52:53.914237 glhmm-0.2.4/glhmm.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      775 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      373 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-18 19:06:24.000000 glhmm-0.2.4/glhmm.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)      139 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        6 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)      409 2024-03-25 09:06:36.000000 glhmm-0.2.4/pyproject.toml
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-09 13:52:53.916061 glhmm-0.2.4/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      581 2024-04-09 13:52:37.000000 glhmm-0.2.4/setup.py
```

### Comparing `glhmm-0.2.3/LICENSE` & `glhmm-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.3/PKG-INFO` & `glhmm-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhmm
-Version: 0.2.3
+Version: 0.2.4
 Summary: Gaussian Linear Hidden Markov Model
 Home-page: https://github.com/vidaurre/glhmm
 Author: Diego Vidaurre
 Author-email: Diego Vidaurre <dvidaurre@cfin.au.dk>
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
@@ -16,11 +16,11 @@
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: igraph
 Requires-Dist: tqdm
 Requires-Dist: scikit-image
 Requires-Dist: statsmodels
 Provides-Extra: doc
-Requires-Dist: sphinx~=4.2.0; extra == "doc"
+Requires-Dist: sphinx>=5.0; extra == "doc"
 Requires-Dist: myst_parser; extra == "doc"
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
```

### Comparing `glhmm-0.2.3/README.md` & `glhmm-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GLHMM
+![Overview Image](logo2_full.png)
 
 [![Documentation Status](https://readthedocs.org/projects/glhmm/badge/?version=latest)](https://glhmm.readthedocs.io/en/latest/?badge=latest)
 
 The GLHMM toolbox provides facilities to fit a variety of Hidden Markov models (HMM) based on the Gaussian distribution, which we generalise as the Gaussian-Linear HMM. 
 Crucially, the toolbox has a focus on finding associations at various levels between brain data (EEG, MEG, fMRI, ECoG, etc) and non-brain data, such as behavioural or physiological variables.
 
 ## Important links
@@ -23,8 +23,8 @@
 - seaborn
 
 ## Installation
 
 - To install from the repo, use the following command:
 
 ```bash
-pip install --user git+https://github.com/vidaurre/glhmm
+pip install glhmm
```

### Comparing `glhmm-0.2.3/glhmm/auxiliary.py` & `glhmm-0.2.4/glhmm/auxiliary.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.3/glhmm/glhmm.py` & `glhmm-0.2.4/glhmm/glhmm.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,14 +99,16 @@
 
 
         self.beta = None
         self.mean = None
         self.alpha_beta = None
         self.alpha_mean = None
         self.Sigma = None
+        self.P = None
+        self.Pi = None
         self.active_states = np.ones(K,dtype=bool)
         self.trained = False
         
     ## Private methods
 
     def __forward_backward(self,L,indices):
         """
@@ -1240,21 +1242,21 @@
         X : array of shape (n_samples, n_parcels), default=None
             The timeseries of set of variables 1. 
         Gamma : array of shape (n_samples, n_states), default=None
             The state probability timeseries.
 
         Returns:
         --------
-        Gamma : array of shape (n_samples, n_states)
-            The state probability timeseries.
-        Y: array of shape (n_samples,n_parcels)
-            The timeseries of set of variables 2.
-        If X=None:
+        If X is not None:
             X : array of shape (n_samples, n_parcels)
                The timeseries of set of variables 1.
+        Y: array of shape (n_samples,n_parcels)
+            The timeseries of set of variables 2.
+        Gamma : array of shape (n_samples, n_states)
+            The state probability timeseries.
 
         """
 
 
         if not self.trained: 
             raise Exception("The model has not yet been trained") 
 
@@ -1278,16 +1280,18 @@
         
         if Gamma is None:
             Gamma = self.sample_Gamma(size)
 
         rng = np.random.default_rng()
 
         if (self.hyperparameters["model_beta"] != 'no') and (X is None):
-            p = self.beta[0]["Mu"].shape[1]
+            p = self.beta[0]["Mu"].shape[0]
             X = np.random.normal(size=(np.sum(T),p))
+        else: 
+            X = None
 
         # Y, mean
         Y = np.zeros((np.sum(T),q))
         if self.hyperparameters["model_mean"] == 'shared':
             Y += np.expand_dims(self.mean[0]['Mu'],axis=0)
         if self.hyperparameters["model_beta"] == 'shared':
             Y += X @ self.beta[0]["Mu"]
@@ -1296,29 +1300,33 @@
             if self.hyperparameters["model_mean"] == 'state': 
                 Y += np.expand_dims(self.mean[k]["Mu"],axis=0) * np.expand_dims(Gamma[:,k],axis=1)
             if self.hyperparameters["model_beta"] == 'state':
                 Y += (X @ self.beta[k]["Mu"]) * np.expand_dims(Gamma[:,k],axis=1)
 
         # Y, covariance
         if shared_covmat:
-            C = self.Sigma[0]["rate"] / self.Sigma[0]["shape"]
+            C = self.get_covariance_matrix()
             if diagonal_covmat:
                 Y += rng.normal(loc=np.zeros(q),scale=C,size=Y.shape)
             else:
                 Y += rng.multivariate_normal(loc=np.zeros(q),cov=C,size=Y.shape)
         else:
             for k in range(K):
+                C = self.get_covariance_matrix(k)
                 if diagonal_covmat:
                     Y += rng.normal(loc=np.zeros(q),scale=C,size=Y.shape)  \
                         * np.expand_dims(Gamma[:,k],axis=1)
                 else:
                     Y += rng.multivariate_normal(loc=np.zeros(q),cov=C,size=Y.shape) \
                         * np.expand_dims(Gamma[:,k],axis=1)
 
-        return X,Y,Gamma
+        if X is None: 
+            return Y,Gamma
+        else:
+            return X,Y,Gamma
 
 
     def get_active_K(self):
         """Returns the number of active states
 
         Returns:
         --------
@@ -1624,14 +1632,31 @@
             If the model has not been trained.
         
         """
         if not self.trained: 
             raise Exception("The model has not yet been trained") 
 
         return self.Sigma[k]["irate"] * self.Sigma[k]["shape"]
+    
+
+    def set_covariance_matrix(rate,shape,self,k=0):
+        """Sets the covariance matrix to specific values.
+        Useful to create synthetic data for simulations.
+
+        Parameters:
+        -----------
+        rate : ndarray of shape (n_variables_2 x n_variables_2),
+                The rate parameter of the covariance
+        shape : int, the shape parameter of the covariance
+        k : int, optional
+            The index of the state. Default=0.
+        """
+
+        self.Sigma[k]["rate"] = rate
+        self.Sigma[k]["shape"] = shape
 
 
     def get_beta(self,k=0):
         """Returns the regression coefficients (beta) for the specified state.
 
         Parameters:
         -----------
@@ -1653,16 +1678,15 @@
         if not self.trained: 
             raise Exception("The model has not yet been trained") 
 
         if self.hyperparameters["model_beta"] == 'no':
             raise Exception("The model has no beta")
 
         return self.beta[k]["Mu"]
-    
-
+   
 
     def get_betas(self):
         """Returns the regression coefficients (beta) for all states.
 
         Returns:
         --------
         betas: ndarray of shape (n_variables_1 x n_variables_2 x n_states)
@@ -1684,16 +1708,30 @@
         (p,q) = self.beta[0]["Mu"].shape
         K = self.hyperparameters["K"]
         betas = np.zeros((p,q,K))
         for k in range(K): betas[:,:,k] = self.beta[k]["Mu"]
         return betas
 
 
-    def get_mean(self,k=0):
+    def set_beta(self,beta,k=0):
+        """Sets the regression coefficients (beta) to specific values.
+        Useful to create synthetic data for simulations.
+
+        Parameters:
+        -----------
+        beta: ndarray of shape (n_variables_1 x n_variables_2)
+            The regression coefficients of each variable in X on each variable in Y for the specified state k.
+        k : int, optional, default=0
+            The index of the state for which to retrieve the beta value.
+        """
+
+        self.beta[k]["Mu"] = beta
+
 
+    def get_mean(self,k=0):
         """Returns the mean for the specified state.
 
         Parameters:
         -----------
         k : int, optional, default=0
             The index of the state for which to retrieve the mean.
 
@@ -1715,15 +1753,14 @@
         if self.hyperparameters["model_mean"] == 'no':
             raise Exception("The model has no mean")
 
         return self.mean[k]["Mu"]
     
 
     def get_means(self):
-
         """Returns the means for all states.
 
         Returns:
         --------
         means: ndarray of shape (n_variables_2, n_states)
             The mean value of each variable in Y for all states.
 
@@ -1747,14 +1784,91 @@
 
         K = self.hyperparameters["K"]
         means = np.zeros((q,K))
         for k in range(K): means[:,k] = self.mean[k]["Mu"]
         return means    
 
 
+    def set_mean(self,mean,k=0):
+        """Sets the mean to specific values.
+        Useful to create synthetic data for simulations.
+
+        Parameters:
+        -----------
+        mean: ndarray of shape (n_variables_2,)
+            The mean value of each variable in Y for the specified state.
+        k : int, optional, default=0
+            The index of the state for which to retrieve the beta value.
+        """
+
+        self.mean[k]["Mu"] = mean
+
+
+    def get_P(self):
+        """Returns transition probability matrix
+
+        Returns:
+        --------
+        P: ndarray of shape (K,K), where K is the number of states
+
+        Raises:
+        -------
+        Exception
+            If the model has not yet been trained.
+        """
+
+        if not self.trained: 
+            raise Exception("The model has not yet been trained") 
+
+        return self.P
+
+
+    def get_Pi(self):
+        """Returns initial probabilities
+
+        Returns:
+        --------
+        Pi: ndarray of shape (K,), where K is the number of states
+
+        Raises:
+        -------
+        Exception
+            If the model has not yet been trained.
+        """
+
+        if not self.trained: 
+            raise Exception("The model has not yet been trained") 
+
+        return self.Pi    
+
+
+    def set_P(self,P):
+        """Set transition probability matrix.
+        Useful to create synthetic data for simulations.
+
+        Parameters:
+        --------
+        P: ndarray of shape (K,K), where K is the number of states
+        """
+
+        self.P = P
+
+
+    def set_Pi(self,Pi):
+        """Returns initial probabilities.
+        Useful to create synthetic data for simulations.
+
+        Parameters:
+        --------
+        Pi: ndarray of shape (K,), where K is the number of states
+        """
+
+        self.Pi = Pi  
+
+
     def dual_estimate(self,X,Y,indices=None,Gamma=None,Xi=None,for_kernel=False):
         """Dual estimation of HMM parameters.
 
         Parameters:
         -----------
         X : array-like of shape (n_samples, n_variables_1)
             The timeseries of set of variables 1.
@@ -1806,14 +1920,37 @@
         #     hmm_dual[j].update_obsdist(X[tt,:],Y[tt,:],Gamma[tt,:])
         if for_kernel:
             return hmm_dual,Gamma,Xi
         else:
             return hmm_dual
 
 
+    def initialize(self,p,q):
+        """
+        Initialize the parameters of the HMM with initial random values.
+        IMPORTANT: This should not be run before training. 
+        This is only useful for sampling data, and should be combined with subsequent calls to 
+        set_beta, set_mean, set_covariance_matrix, set_P and set_Pi.
+
+        Parameters:
+        -----------
+        p : number of channels in X (not used if only Y is modelled)
+        q : number of channels in Y      
+        """
+
+        T = 1000
+        if self.hyperparameters["model_beta"] != 'no': X = np.random.random((T,p))
+        else: X = None
+        Y = np.random.random((T,q))
+        options = {}
+        options["cyc"] = 1
+        options["initrep"] = 0
+        self.train(X=X,Y=Y,options=options)
+
+
     def train(self,X=None,Y=None,indices=None,files=None,Gamma=None,Xi=None,scale=None,options=None):
         """
         Train the GLHMM on input data X and Y, which most general formulation is
         Y = mu_k + X beta_k + noise
         where noise is Gaussian with mean zero and standard deviation Sigma_k
 
         It supports both standard and stochastic variational learning;
```

### Comparing `glhmm-0.2.3/glhmm/graphics.py` & `glhmm-0.2.4/glhmm/graphics.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     K = P.shape[0]
 
     if not show_diag:
         for k in range(P.shape[0]):
             P[k,k] = 0
             P[k,:] = P[k,:] / np.sum(P[k,:])
 
-    _,ax = plt.subplots()
-    g = sb.heatmap(ax=ax,data=P,\
+    _,axes = plt.subplots()
+    g = sb.heatmap(ax=axes,data=P,\
         cmap='bwr',xticklabels=np.arange(K), yticklabels=np.arange(K),
         square=True,cbar=show_colorbar)
     for k in range(K):
         g.plot([0, K],[k, k], '-k')
         g.plot([k, k],[0, K], '-k')
 
-    ax.axhline(y=0, color='k',linewidth=4)
-    ax.axhline(y=K, color='k',linewidth=4)
-    ax.axvline(x=0, color='k',linewidth=4)
-    ax.axvline(x=K, color='k',linewidth=4)
+    axes.axhline(y=0, color='k',linewidth=4)
+    axes.axhline(y=K, color='k',linewidth=4)
+    axes.axvline(x=0, color='k',linewidth=4)
+    axes.axvline(x=K, color='k',linewidth=4)
 
 
 def show_Gamma(Gamma, line_overlay=None, tlim=None, Hz=1, palette='viridis'):
     """Displays the activity of the hidden states as a function of time.
     
     Parameters:
     -----------
@@ -441,19 +441,19 @@
 
 def interpolate_colormap(cmap_list):     
     """
     Create a new colormap with the modified color_array.
 
     Parameters:
     --------------
-       cmap_list (numpy.ndarray): Original color array for the colormap.
+    cmap_list (numpy.ndarray): Original color array for the colormap.
 
     Returns:
     ----------  
-        modified_cmap (numpy.ndarray): Modified colormap array.
+    modified_cmap (numpy.ndarray): Modified colormap array.
     """
     # Create a new colormap with the modified color_array
     modified_cmap  = np.ones_like(cmap_list)
 
     for channel_idx in range(3):
         # Extract the channel values from the colormap
         channel_values = cmap_list[:, channel_idx]
@@ -494,16 +494,16 @@
 def plot_p_value_matrix(pval, alpha = 0.05, normalize_vals=True, figsize=(9, 5), steps=11, title_text="Heatmap (p-values)", annot=True, cmap_type='default', cmap_reverse=True, xlabel="", ylabel="", xticklabels=None, none_diagonal = False, num_colors = 259):
     from matplotlib import cm, colors
     import seaborn as sb
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     """
     Plot a heatmap of p-values.
 
-    Parameters
-    ----------
+    Parameters:
+    -----------
     pval : numpy.ndarray
         The p-values data to be plotted.
     normalize_vals : bool, optional
         If True, the data range will be normalized from 0 to 1 (Default=False).
     figsize : tuple, optional
         Figure size in inches (width, height) (Default=(12, 7)).
     steps : int, optional
@@ -520,23 +520,23 @@
         Y-axis label. If not provided, default labels based on the method will be used.
     xticklabels : List[str], optional
         If not provided, labels will be numbers equal to shape of pval.shape[1].
         Else you can define your own labels, e.g., xticklabels=['sex', 'age'].
     none_diagonal : bool, optional
         If you want to turn the diagonal into NaN numbers (Default=False).
 
-    Returns
-    -------
+    Returns:
+    --------
     None
         Displays the heatmap plot.
     """
     if pval.ndim==0:
         pval = np.reshape(pval, (1, 1))
         
-    fig, ax = plt.subplots(figsize=figsize)
+    fig, axes = plt.subplots(figsize=figsize)
     if len(pval.shape)==1:
         pval =np.expand_dims(pval,axis=0)
     if cmap_type=='default':
         if normalize_vals:
             color_array = np.logspace(-3, 0, num_colors).reshape(1, -1)
 
         if alpha == None and normalize_vals==False:
@@ -588,42 +588,42 @@
         # Set the diagonal elements to NaN in the copied matrix
         np.fill_diagonal(pval_with_nan_diagonal, np.nan)
         pval = pval_with_nan_diagonal.copy()
 
     if normalize_vals:
         norm = LogNorm(vmin=1e-3, vmax=1)
 
-        heatmap = sb.heatmap(pval, ax=ax, cmap=cmap, annot=annot, fmt=".3f", cbar=False, norm=norm)
+        heatmap = sb.heatmap(pval, ax=axes, cmap=cmap, annot=annot, fmt=".3f", cbar=False, norm=norm)
     else:
-        heatmap = sb.heatmap(pval, ax=ax, cmap=cmap, annot=annot, fmt=".3f", cbar=False)
+        heatmap = sb.heatmap(pval, ax=axes, cmap=cmap, annot=annot, fmt=".3f", cbar=False)
 
     # Add labels and title
-    ax.set_xlabel(xlabel, fontsize=12)
-    ax.set_ylabel(ylabel, fontsize=12)
-    ax.set_title(title_text, fontsize=14)
+    axes.set_xlabel(xlabel, fontsize=12)
+    axes.set_ylabel(ylabel, fontsize=12)
+    axes.set_title(title_text, fontsize=14)
     # Set the x-axis ticks
     if xticklabels is not None:
-        ax.set_xticks(np.arange(len(xticklabels)) + 0.5)
-        ax.set_xticklabels(xticklabels, rotation="horizontal", fontsize=10)
+        axes.set_xticks(np.arange(len(xticklabels)) + 0.5)
+        axes.set_xticklabels(xticklabels, rotation="horizontal", fontsize=10)
     elif pval.shape[1]>1:
-        ax.set_xticks(np.linspace(0, pval.shape[1]-1, steps).astype(int)+0.5)
-        ax.set_xticklabels(np.linspace(1, pval.shape[1], steps).astype(int), rotation="horizontal", fontsize=10)
+        axes.set_xticks(np.linspace(0, pval.shape[1]-1, steps).astype(int)+0.5)
+        axes.set_xticklabels(np.linspace(1, pval.shape[1], steps).astype(int), rotation="horizontal", fontsize=10)
     else:
-        ax.set_xticklabels([])
+        axes.set_xticklabels([])
     # Set the y-axis ticks
     if pval.shape[0]>1:
-        ax.set_yticks(np.linspace(0, pval.shape[0]-1, steps).astype(int)+0.5)
-        ax.set_yticklabels(np.linspace(1, pval.shape[0], steps).astype(int), rotation="horizontal", fontsize=10)
+        axes.set_yticks(np.linspace(0, pval.shape[0]-1, steps).astype(int)+0.5)
+        axes.set_yticklabels(np.linspace(1, pval.shape[0], steps).astype(int), rotation="horizontal", fontsize=10)
     else:
-        ax.set_yticklabels([])
+        axes.set_yticklabels([])
     # Create an axes on the right side of ax. The width of cax will be 5%
     # of ax and the padding between cax and ax will be fixed at 0.05 inch.
     
     if normalize_vals:   
-        divider = make_axes_locatable(ax)
+        divider = make_axes_locatable(axes)
         cax = divider.append_axes("right", size="5%", pad=0.05)
         colorbar = plt.colorbar(heatmap.get_children()[0], cax=cax, ticks=np.logspace(-3, 0, num_colors))
         colorbar.update_ticks()
         
          # Round the tick values to three decimal places
         rounded_ticks = [round(tick, 3) for tick in colorbar.get_ticks()]
         
@@ -643,15 +643,15 @@
         colorbar.ax.tick_params(axis='y')
 
         for idx, tick_line in enumerate(colorbar.ax.yaxis.get_ticklines()):
             if idx not in indices_not_empty:
                 tick_line.set_visible(False)
             
     else:
-        divider = make_axes_locatable(ax)
+        divider = make_axes_locatable(axes)
         cax = divider.append_axes("right", size="5%", pad=0.05)
         # Create a custom colorbar
         colorbar = plt.colorbar(heatmap.get_children()[0], cax=cax)
         # Set the ticks to range from the bottom to the top of the colorbar
         # Get the minimum and maximum values from your data
         min_value = np.nanmin(pval)
         max_value = np.nanmax(pval)
@@ -660,23 +660,22 @@
         colorbar.set_ticks(np.linspace(min_value, max_value, 5).round(2))
         #colorbar.set_ticks([0, 0.25, 0.5, 1])  # Adjust ticks as needed
         
 
     # Show the plot
     plt.show()
     
-def plot_correlation_matrix(corr_vals, performed_tests, normalize_vals=False, figsize=(9, 5), steps=11, title_text="Heatmap (p-values)", annot=True, cmap_type='default', cmap_reverse=True, xlabel="", ylabel="", xticklabels=None, none_diagonal = False, num_colors = 256):
+def plot_correlation_matrix(corr_vals, performed_tests, normalize_vals=False, figsize=(9, 5), steps=11, title_text="Correlation Coefficients Heatmap", annot=True, cmap_type='default', cmap_reverse=True, xlabel="", ylabel="", xticklabels=None, none_diagonal = False, num_colors = 256):
     from matplotlib import cm, colors
-    import seaborn as sb
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     """
     Plot a heatmap of p-values.
 
-    Parameters
-    ----------
+    Parameters:
+    -----------
     corr_vals : numpy.ndarray
         base statistics of corelation coefficients.
     performed_tests : dict
         Holds information about the different test statistics that has been applied
     normalize_vals : bool, optional
         If True, the data range will be normalized from 0 to 1 (Default=False).
     figsize : tuple, optional
@@ -695,26 +694,26 @@
         Y-axis label. If not provided, default labels based on the method will be used.
     xticklabels : List[str], optional
         If not provided, labels will be numbers equal to shape of corr_vals.shape[1].
         Else you can define your own labels, e.g., xticklabels=['sex', 'age'].
     none_diagonal : bool, optional
         If you want to turn the diagonal into NaN numbers (Default=False).
 
-    Returns
-    -------
+    Returns:
+    --------
     None
         Displays the heatmap plot.
     """
     if performed_tests["t_test_cols"]!=[] or performed_tests["f_test_cols"]!=[]:
         raise ValueError("Cannot plot the base statistics for the correlation coefficients because different test statistics have been used.")
     
     if corr_vals.ndim==0:
         corr_vals = np.reshape(corr_vals, (1, 1))
         
-    fig, ax = plt.subplots(figsize=figsize)
+    fig, axes = plt.subplots(figsize=figsize)
     if len(corr_vals.shape)==1:
         corr_vals =np.expand_dims(corr_vals,axis=0)
 
     if cmap_type=='default':
         # seismic_cmap = cm.seismic.reversed()
         coolwarm_cmap = cm.coolwarm.reversed()
         
@@ -728,40 +727,40 @@
         cmap = getattr(cm, cmap_type, None)
         if cmap_reverse:
             cmap =cmap.reversed()
 
     if normalize_vals:
         # Normalize the data range from -1 to 1
         norm = plt.Normalize(vmin=-1, vmax=1)
-        heatmap = sb.heatmap(corr_vals, ax=ax, cmap=cmap, annot=annot, fmt=".3f", cbar=False, norm=norm)
+        heatmap = sb.heatmap(corr_vals, ax=axes, cmap=cmap, annot=annot, fmt=".3f", cbar=False, norm=norm)
     else:
-        heatmap = sb.heatmap(corr_vals, ax=ax, cmap=cmap, annot=annot, fmt=".3f", cbar=False)
+        heatmap = sb.heatmap(corr_vals, ax=axes, cmap=cmap, annot=annot, fmt=".3f", cbar=False)
     # Add labels and title
-    ax.set_xlabel(xlabel, fontsize=12)
-    ax.set_ylabel(ylabel, fontsize=12)
-    ax.set_title(title_text, fontsize=14)
+    axes.set_xlabel(xlabel, fontsize=12)
+    axes.set_ylabel(ylabel, fontsize=12)
+    axes.set_title(title_text, fontsize=14)
     # Set the x-axis ticks
     if xticklabels is not None:
-        ax.set_xticks(np.arange(len(xticklabels)) + 0.5)
-        ax.set_xticklabels(xticklabels, rotation="horizontal", fontsize=10)
+        axes.set_xticks(np.arange(len(xticklabels)) + 0.5)
+        axes.set_xticklabels(xticklabels, rotation="horizontal", fontsize=10)
     elif corr_vals.shape[1]>1:
-        ax.set_xticks(np.linspace(0, corr_vals.shape[1]-1, steps).astype(int)+0.5)
-        ax.set_xticklabels(np.linspace(1, corr_vals.shape[1], steps).astype(int), rotation="horizontal", fontsize=10)
+        axes.set_xticks(np.linspace(0, corr_vals.shape[1]-1, steps).astype(int)+0.5)
+        axes.set_xticklabels(np.linspace(1, corr_vals.shape[1], steps).astype(int), rotation="horizontal", fontsize=10)
     else:
-        ax.set_xticklabels([])
+        axes.set_xticklabels([])
     # Set the y-axis ticks
     if corr_vals.shape[0]>1:
-        ax.set_yticks(np.linspace(0, corr_vals.shape[0]-1, steps).astype(int)+0.5)
-        ax.set_yticklabels(np.linspace(1, corr_vals.shape[0], steps).astype(int), rotation="horizontal", fontsize=10)
+        axes.set_yticks(np.linspace(0, corr_vals.shape[0]-1, steps).astype(int)+0.5)
+        axes.set_yticklabels(np.linspace(1, corr_vals.shape[0], steps).astype(int), rotation="horizontal", fontsize=10)
     else:
-        ax.set_yticklabels([])
+        axes.set_yticklabels([])
     # Create an axes on the right side of ax. The width of cax will be 5%
     # of ax and the padding between cax and ax will be fixed at 0.05 inch.
     
-    divider = make_axes_locatable(ax)
+    divider = make_axes_locatable(axes)
     cax = divider.append_axes("right", size="5%", pad=0.05)
     # Create a custom colorbar
     colorbar = plt.colorbar(heatmap.get_children()[0], cax=cax)
     # Set the ticks to range from the bottom to the top of the colorbar
     # Get the minimum and maximum values from your data
     min_value = np.nanmin(corr_vals)
     max_value = np.nanmax(corr_vals)
@@ -777,27 +776,27 @@
     plt.show()
 
   
 def plot_permutation_distribution(test_statistic, title_text="Permutation Distribution",xlabel="Test Statistic Values",ylabel="Density"):
     """
     Plot the histogram of the permutation with the observed statistic marked.
 
-    Parameters
-    ----------
+    Parameters:
+    -----------
     test_statistic : numpy.ndarray
         An array containing the permutation values.
     title_text : str, optional
         Title text of the plot (Default="Permutation Distribution").
     xlabel : str, optional
         Text of the xlabel (Default="Test Statistic Values").
     ylabel : str, optional
         Text of the ylabel (Default="Density").
 
-    Returns
-    -------
+    Returns:
+    --------
     None
         Displays the histogram plot.
     """
     plt.figure()
     sb.histplot(test_statistic, kde=True)
     plt.axvline(x=test_statistic[0], color='red', linestyle='--', label='Observed Statistic')
     plt.xlabel(xlabel)
@@ -809,16 +808,16 @@
 
 
 
 def plot_scatter_with_labels(p_values, alpha=0.05, title_text="", xlabel=None, ylabel=None, xlim_start=0.9, ylim_start=0):
     """
     Create a scatter plot to visualize p-values with labels indicating significant points.
 
-    Parameters
-    ----------
+    Parameters:
+    -----------
     p_values : numpy.ndarray
         An array of p-values. Can be a 1D array or a 2D array with shape (1, 5).
     alpha : float, optional
         Threshold for significance (Default=0.05).
     title_text : str, optional
         The title text for the plot (Default="").
     xlabel : str, optional
@@ -826,20 +825,20 @@
     ylabel : str, optional
         The label for the y-axis (Default=None).
     xlim_start : float, optional
         Start position of x-axis limits (Default=-5).
     ylim_start : float, optional
         Start position of y-axis limits (Default=-0.1).
 
-    Returns
-    -------
+    Returns:
+    --------
     None
 
-    Note
-    ----
+    Notes:
+    ------
     Points with p-values less than alpha are considered significant and marked with red text.
     """
 
     # If p_values is a 2D array with shape (1, 5), flatten it to 1D
     if len(p_values.shape) == 2 and p_values.shape[0] == 1 and p_values.shape[1] == 5:
         p_values = p_values.flatten()
 
@@ -890,64 +889,121 @@
     # ax.grid(color='lightgray', linestyle='--')
 
     # Show the plot
     plt.tight_layout()
     plt.show()
     
     
-def plot_vpath(vpath, signal =[], xlabel = "Time Steps", figsize=(7, 4), ylabel = "", yticks=None,line_width=2, label_signal="Signal"):
-    # Assuming vpath is your data matrix
-    num_states = vpath.shape[1]
-
-    # Create a Seaborn color palette
-    colors = sb.color_palette("Set3", n_colors=num_states)
-
-    # Plot the stack plot using Seaborn
-    fig, axes = plt.subplots(figsize=figsize)  # Adjust the figure size for better readability
-    axes.stackplot(np.arange(vpath.shape[0]), vpath.T, colors=colors, labels=[f'State {i + 1}' for i in range(num_states)])
-
-    # Set labels and legend to the right of the figure
-    axes.set_xlabel(xlabel, fontsize=14)
-    axes.set_ylabel(ylabel, fontsize=14)
-    axes.legend(title='States', loc='upper left', bbox_to_anchor=(1, 1))  # Adjusted legend position
+import matplotlib.pyplot as plt
+import seaborn as sns
+import numpy as np
+
+def plot_vpath(viterbi_path, signal=None, idx_data=None, figsize=(7, 4), fontsize_labels=13, fontsize_title=16, yticks=None, time_conversion_rate=None, xlabel="Timepoints", ylabel="", title="Viterbi Path", signal_label="Signal", show_legend=True, vertical_linewidth=1.5):
+    """
+    Plot Viterbi path with optional signal overlay.
+
+    Parameters:
+    -----------
+    viterbi_path : array-like
+        The Viterbi path data matrix.
+    signal : array-like, optional
+        Signal data to overlay on the plot. Default is None.
+    idx_data : array-like, optional
+        Array representing time intervals. Default is None.
+    figsize : tuple, optional
+        Figure size. Default is (7, 4).
+    fontsize_labels : int, optional
+        Font size for axis labels. Default is 13.
+    fontsize_title : int, optional
+        Font size for plot title. Default is 16.
+    yticks : bool, optional
+        Whether to show y-axis ticks. Default is None.
+    time_conversion_rate : float, optional
+        Conversion rate from time steps to seconds. Default is None.
+    xlabel : str, optional
+        Label for the x-axis. Default is "Timepoints".
+    ylabel : str, optional
+        Label for the y-axis. Default is "".
+    title : str, optional
+        Title for the plot. Default is "Viterbi Path".
+    signal_label : str, optional
+        Label for the signal plot. Default is "Signal".
+    show_legend : bool, optional
+        Whether to show the legend. Default is True.
+    vertical_linewidth : float, optional
+        Line width for vertical gray lines. Default is 1.5.
+    """
+    num_states = viterbi_path.shape[1]
+    colors = sns.color_palette("Set3", n_colors=num_states)
+    if num_states > len(colors):
+        extra_colors = sns.color_palette("husl", n_colors=num_states - len(colors))
+        colors.extend(extra_colors)
+
+    fig, axes = plt.subplots(figsize=figsize)
+
+    # Plot Viterbi path
+    if time_conversion_rate is not None:
+        time_seconds = np.arange(viterbi_path.shape[0]) / time_conversion_rate
+        axes.stackplot(time_seconds, viterbi_path.T, colors=colors, labels=[f'State {i + 1}' for i in range(num_states)])
+        if xlabel == "Timepoints":
+            xlabel = "Time (seconds)"
+        axes.set_xlabel(xlabel, fontsize=fontsize_labels)
+    else:
+        axes.stackplot(np.arange(viterbi_path.shape[0]), viterbi_path.T, colors=colors, labels=[f'State {i + 1}' for i in range(num_states)])
+        axes.set_xlabel(xlabel, fontsize=fontsize_labels)
+
+    axes.set_ylabel(ylabel, fontsize=fontsize_labels)
+    axes.set_title(title, fontsize=fontsize_title)
+
+    # Plot signal overlay
+    if signal is not None:
+        if time_conversion_rate is not None:
+            time_seconds = np.arange(len(signal)) / time_conversion_rate
+            axes.plot(time_seconds, signal, color='black', label=signal_label)
+            axes.set_xlabel(xlabel, fontsize=fontsize_labels)
+        else:
+            axes.plot(signal, color='black', label=signal_label)
+
+    # Draw vertical gray lines for T_t intervals
+    if idx_data is not None:
+        for idx in idx_data[:-1, 1]:
+            axes.axvline(x=idx, color='gray', linestyle='--', linewidth=vertical_linewidth)
+
+    # Show legend
+    if show_legend:
+        axes.legend(title='States', loc='upper left', bbox_to_anchor=(1, 1))
 
     if yticks:
         scaled_values = [int(val * len(np.unique(signal))) for val in np.unique(signal)]
         # Set y-ticks with formatted integers
         axes.set_yticks(np.unique(signal), scaled_values)
     else:
         # Remove x-axis tick labels
         axes.set_yticks([])
-
+        
     # Remove the frame around the plot
     axes.spines['top'].set_visible(False)
     axes.spines['right'].set_visible(False)
     axes.spines['bottom'].set_visible(False)
     axes.spines['left'].set_visible(False)
 
-    # Add a plot of the signal (replace this with your actual signal data)
-    # com_signal = np.sin(np.linspace(0, 10, vpath.shape[0])) + 2
-    if signal is not None:
-        axes.plot(signal, color='black', label=label_signal, linewidth=line_width)
-    axes.legend(loc='upper left', bbox_to_anchor=(1, 0.8))  # Adjusted legend position
-
+    # Adjust tick label font size
+    axes.tick_params(axis='both', labelsize=fontsize_labels)
 
-    # Increase tick label font size
-    axes.tick_params(axis='both', labelsize=12)
     plt.tight_layout() 
-    # Show the plot
     plt.show()
+
     
 def plot_average_probability(Gamma_reconstruct, title='Average probability for each state', fontsize=16, figsize=(7, 5), vertical_lines=None, line_colors=None, highlight_boxes=False):
 
     """
     Plots the average probability for each state over time.
 
-    Parameters
-    ----------
+    Parameters:
+    -----------
     Gamma_reconstruct : numpy.ndarray
         3D array representing reconstructed gamma values.
         Shape: (num_timepoints, num_trials, num_states)
     title : str, optional
         Title for the plot (Default='Average probability for each state').
     fontsize : int, optional
         Font size for labels and title (Default=16).
@@ -957,16 +1013,16 @@
         List of pairs specifying indices for vertical lines (Default=None).
     line_colors : list of str or bool, optional
         List of colors for each pair of vertical lines. If True, generates random colors
         (unless a list is provided) (Default=None).
     highlight_boxes : bool, optional
         Whether to include highlighted boxes for each pair of vertical lines (Default=False).
     
-    Returns
-    -------
+    Returns:
+    --------
     None
     """
 
     # Initialize an array for average gamma values
     Gamma_avg = np.zeros((Gamma_reconstruct.shape[0], Gamma_reconstruct.shape[-1]))
 
     # Calculate and store average gamma values
@@ -1003,16 +1059,301 @@
         plt.legend(handles=[legend_rect], loc='upper right')
 
     # Place legend for the lines to the right of the figure
     plt.legend(bbox_to_anchor=(1.05, 1), loc='upper left')
 
     # Show the plot
     plt.show()
+
+def plot_FO(FO, figsize=(8, 4), fontsize_labels=13, fontsize_title=16, width=0.8, show_legend=True, num_ticks=10):
+    """
+    Plot fractional occupancies for different states.
+
+    Parameters:
+    -----------
+    FO : array-like
+        Fractional occupancy data matrix.
+    figsize : tuple, optional
+        Figure size. Default is (8, 4).
+    fontsize_labels : int, optional
+        Font size for axes labels. Default is 13.
+    fontsize_title : int, optional
+        Font size for plot title. Default is 16.
+    width : float, optional
+        Width of the bars. Default is 0.5.
+    show_legend : bool, optional
+        Whether to show the legend. Default is True.
+    """
+    fig, axes = plt.subplots(figsize=figsize)
+    bottom = np.zeros(FO.shape[0])
+    sessions = np.arange(1, FO.shape[0] + 1)
+    num_states = FO.shape[1]
+    colors = sns.color_palette("Set3", n_colors=num_states)
+    if num_states > len(colors):
+        extra_colors = sns.color_palette("husl", n_colors=num_states - len(colors))
+        colors.extend(extra_colors)
+        
+    for k in range(num_states):
+        p = axes.bar(sessions, FO[:, k], bottom=bottom, color=colors[k], width=width)
+        bottom += FO[:, k]
+    
+    axes.set_xticks(sessions)
+    axes.set_xlabel('Subject', fontsize=fontsize_labels)
+    axes.set_ylabel('Fractional occupancy', fontsize=fontsize_labels)
+    axes.set_title('State Fractional Occupancies', fontsize=fontsize_title)
+    
+    ticks = np.linspace(1, FO.shape[0], FO.shape[0]).astype(int)
+    # If there are more than 10 states then make a steps of 5
+    if len(ticks)>10:
+        n_ticks = num_ticks
+    else:
+        n_ticks = len(ticks)
+    axes.set_xticks(np.linspace(1, FO.shape[0], n_ticks).astype(int))
+    axes.set_yticks(np.linspace(0, 1, 5))
+    
+    # Remove the frame around the plot
+    axes.spines['top'].set_visible(False)
+    axes.spines['right'].set_visible(False)
+    axes.spines['bottom'].set_visible(False)
+    axes.spines['left'].set_visible(False)
+
+    # Adjust tick label font size
+    axes.tick_params(axis='both', labelsize=fontsize_labels)
+
+    if show_legend:
+        legend = axes.legend(['State {}'.format(i+1) for i in range(FO.shape[1])], fontsize=fontsize_labels, loc='upper left', bbox_to_anchor=(1, 1))
+
+    plt.tight_layout() 
+    plt.show()
+
+
+def plot_switching_rates(SR, figsize=(8, 4), fontsize_labels=13, fontsize_title=16, width=0.18, show_legend=True, num_ticks=10):
+    """
+    Plot switching rates for different states.
+
+    Parameters:
+    -----------
+    SR : 
+        Switching rate data matrix.
+    figsize : tuple, optional
+        Figure size. Default is (6, 4).
+    fontsize_labels : int, optional
+        Font size for axes labels. Default is 13.
+    fontsize_title : int, optional
+        Font size for plot title. Default is 16.
+    width : float, optional
+        Width of the bars. Default is 0.18.
+    show_legend : bool, optional
+        Whether to show the legend. Default is True.
+    """
+    fig, axes = plt.subplots(figsize=figsize, constrained_layout=True)
+    multiplier = 0
+    sessions = np.arange(1, SR.shape[0] + 1)
+    num_states = SR.shape[1]
+    colors = sns.color_palette("Set3", n_colors=num_states)
+    if num_states > len(colors):
+        extra_colors = sns.color_palette("husl", n_colors=num_states - len(colors))
+        colors.extend(extra_colors)
+
+    for k in range(num_states):
+        offset = width * multiplier
+        rects = axes.bar(sessions + offset, SR[:, k], width, color=colors[k])
+        multiplier += 1
+    
+    axes.set_xticks(sessions)
+    axes.set_xlabel('Subject', fontsize=fontsize_labels)
+    axes.set_ylabel('Switching Rate', fontsize=fontsize_labels)
+    axes.set_title('State Switching Rates', fontsize=fontsize_title)
+    
+    ticks = np.linspace(1, SR.shape[0], SR.shape[0]).astype(int)
+    # If there are more than 10 states then make a steps of 5
+    if len(ticks)>10:
+        n_ticks = num_ticks
+    else:
+        n_ticks = len(ticks)
+    axes.set_xticks(np.linspace(1, SR.shape[0], n_ticks).astype(int))
+    
+    # Remove the frame around the plot
+    axes.spines['top'].set_visible(False)
+    axes.spines['right'].set_visible(False)
+    axes.spines['bottom'].set_visible(False)
+    axes.spines['left'].set_visible(False)
+
+    # Adjust tick label font size
+    axes.tick_params(axis='both', labelsize=fontsize_labels)
+
+    if show_legend:
+        axes.legend(['State {}'.format(i+1) for i in range(num_states)], fontsize=fontsize_labels, loc='upper left', bbox_to_anchor=(1, 1))
+
+    plt.show()
+
+def plot_state_lifetimes(LT, figsize=(8, 4), fontsize_labels=13, fontsize_title=16, width=0.18, xlabel='Subject', ylabel='Lifetime', title='State Lifetimes', show_legend=True, num_ticks=10):
+    """
+    Plot state lifetimes for different states.
+
+    Parameters:
+    -----------
+    LT : 
+        State lifetime (dwell time) data matrix.
+    figsize : tuple, optional
+        Figure size. Default is (8, 4).
+    fontsize_labels : int, optional
+        Font size for axeses labels. Default is 13.
+    fontsize_title : int, optional
+        Font size for plot title. Default is 16.
+    width : float, optional
+        Width of the bars. Default is 0.18.
+    xlabel : str, optional
+        Label for the x-axesis. Default is 'Subject'.
+    ylabel : str, optional
+        Label for the y-axesis. Default is 'Lifetime'.
+    title : str, optional
+        Title for the plot. Default is 'State Lifetimes'.
+    show_legend : bool, optional
+        Whether to show the legend. Default is True.
+    """
+    fig, axes = plt.subplots(figsize=figsize, constrained_layout=True)
+    multiplier = 0
+    sessions = np.arange(1, LT.shape[0] + 1)
+    num_states = LT.shape[1]
+    colors = sns.color_palette("Set3", n_colors=num_states)
+    if num_states > len(colors):
+        extra_colors = sns.color_palette("husl", n_colors=num_states - len(colors))
+        colors.extend(extra_colors)
+
+    for k in range(num_states):
+        offset = width * multiplier
+        rects = axes.bar(sessions + offset, LT[:, k], width, color=colors[k])
+        multiplier += 1
+    
+    axes.set_xticks(sessions, sessions)
+    axes.set_xlabel(xlabel, fontsize=fontsize_labels)
+    axes.set_ylabel(ylabel, fontsize=fontsize_labels)
+    axes.set_title(title, fontsize=fontsize_title)
+    
+    ticks = np.linspace(1, LT.shape[0], LT.shape[0]).astype(int)
+    # If there are more than 10 states then make a steps of 5
+    if len(ticks)>10:
+        n_ticks = num_ticks
+    else:
+        n_ticks = len(ticks)
+    axes.set_xticks(np.linspace(1, LT.shape[0], n_ticks).astype(int))
     
+    # Remove the frame around the plot
+    axes.spines['top'].set_visible(False)
+    axes.spines['right'].set_visible(False)
+    axes.spines['bottom'].set_visible(False)
+    axes.spines['left'].set_visible(False)
+
+    # Adjust tick label font size
+    axes.tick_params(axis='both', labelsize=fontsize_labels)
 
+    if show_legend:
+        axes.legend(['State {}'.format(i+1) for i in range(num_states)], fontsize=fontsize_labels, loc='upper left', bbox_to_anchor=(1, 1))
+    plt.show()
+
+def plot_state_prob_and_covariance(init_stateP, TP, state_means, state_FC, cmap='viridis', figsize=(9, 7), num_ticks=5):
+    """
+    Plot HMM parameters.
+
+    Parameters:
+    -----------
+    init_stateP : array-like
+        Initial state probabilities.
+    TP : array-like
+        Transition probabilities.
+    state_means : array-like
+        State means.
+    state_FC : array-like
+        State covariances.
+    cmap : str or Colormap, optional
+        The colormap to be used for plotting. Default is 'viridis'.
+    figsize : tuple, optional
+        Figure size. Default is (9, 7).
+    num_ticks : int, optional
+        Number of ticks for the colorbars
+    """
+    # Define the number of plots and their layout
+    num_plots = 3 + state_FC.shape[2]  # Number of plots including initial stateP, TP, state_means, and state_FC
+    num_cols = min(num_plots, 3)  # Maximum number of columns
+    num_rows = (num_plots - 1) // 3 + 1  # Calculate number of rows
+
+    # Create the figure and subplots
+    fig, axes = plt.subplots(num_rows, 3, figsize=figsize)  # Adjust figsize as needed
+
+    # Plot initial state probabilities
+    im0 = axes[0, 0].imshow(init_stateP.reshape(-1, 1), cmap=cmap)
+    axes[0, 0].set_title("Initial state probabilities")
+    axes[0, 0].set_xticks([])
+    cbar0 = fig.colorbar(im0, ax=axes[0, 0])
+    cbar0.set_ticks(np.linspace(init_stateP.min(), init_stateP.max(), num=num_ticks).round(2))
+    ticks = np.linspace(0, init_stateP.shape[0]-1, init_stateP.shape[0]).astype(int)
+    # If there are more than 10 states then make a steps of 5
+    if len(ticks)>10:
+        num_state = num_ticks
+    else:
+        num_state = len(ticks)
+    axes[0, 0].set_yticks(np.linspace(0, init_stateP.shape[0]-1, num_state).astype(int))
+    axes[0, 0].set_yticklabels(ticks + 1)  # Increment ticks by 1 for labels    
+        
+        
+    # Plot transition probabilities
+    im1 = axes[0, 1].imshow(TP, cmap=cmap)
+    axes[0, 1].set_title("Transition probabilities")
+    cbar1 = fig.colorbar(im1, ax=axes[0, 1])
+    cbar1.set_ticks(np.linspace(TP.min(), TP.max(), num=num_ticks).round(2))
+    ticks = np.linspace(0, TP.shape[0]-1, TP.shape[0]).astype(int)
+    # If there are more than 10 states then make a steps of 5
+    axes[0, 1].set_xticks(np.linspace(0, TP.shape[0]-1, num_state).astype(int))
+    axes[0, 1].set_xticklabels(ticks + 1)  # Increment ticks by 1 for labels
+    axes[0, 1].set_yticks(np.linspace(0, TP.shape[0]-1, num_state).astype(int))
+    axes[0, 1].set_yticklabels(ticks + 1)  # Increment ticks by 1 for labels
+    
+    # Plot state means
+    num_ticks = max(5, min(state_means.shape))
+    im2 = axes[0, 2].imshow(state_means, cmap=cmap, aspect='auto')
+    axes[0, 2].set_title("State means")
+    cbar2 = fig.colorbar(im2, ax=axes[0, 2])
+    cbar2.set_ticks(np.linspace(state_means.min(), state_means.max(), num=num_ticks).round(2))
+    # Set ticks and labels
+    ticks = np.linspace(0, state_means.shape[1]-1, num_ticks).astype(int)
+    axes[0, 2].set_xticks(ticks)
+    axes[0, 2].set_xticklabels(ticks + 1)  # Increment ticks by 1 for labels
+    axes[0, 2].set_yticks(np.linspace(1, state_means.shape[0], num_ticks).astype(int))
+
+    # Plot state covariances
+    min_value = np.min(state_FC)
+    max_value = np.max(state_FC)
+    # Limits the number of ticks
+    if len(ticks)>10:
+        num_state = num_ticks
+    else:
+        num_state = len(ticks)
+        
+    ticks = np.linspace(0, state_FC.shape[0] - 1, num_state).astype(int)
+    # Plot state covariances
+    for k in range((num_cols*num_rows) -3): # have to fill the remaning number of subplots
+        row_idx = (k + 3) // 3  # Shift row index by 3 to start from the second row
+        col_idx = (k + 3) % 3
+        if k < num_plots - 3:
+            im = axes[row_idx, col_idx].imshow(state_FC[:, :, k], cmap=cmap, vmin=min_value, vmax=max_value)
+            axes[row_idx, col_idx].set_title("State covariance\nstate #%s" % (k + 1))
+            # Adjust tick locations
+            axes[row_idx, col_idx].set_xticks(ticks)
+            axes[row_idx, col_idx].set_yticks(ticks)
+            axes[row_idx, col_idx].set_xticklabels(ticks + 1)  # Increment ticks by 1 for labels
+            axes[row_idx, col_idx].set_yticklabels(ticks + 1) # Increment ticks by 1 for
+            cbar = fig.colorbar(im, ax=axes[row_idx, col_idx])
+            cbar.set_ticks(np.linspace(min_value, max_value, num=num_ticks).round(2))
+        else:
+            axes[row_idx, col_idx].axis('off')  # Leave empty plots blank
+
+    plt.subplots_adjust(hspace=0.5, wspace=0.5)
+    plt.show()
+    
 def plot_condition_difference(Gamma_reconstruct, R_trials, title='Average Probability and Difference', fontsize=16, figsize=(9, 2), vertical_lines=None, line_colors=None, highlight_boxes=False):
     """
     Plots the average probability for each state over time for two conditions and their difference.
 
     Parameters:
     -----------
     Gamma_reconstruct : numpy.ndarray
@@ -1087,50 +1428,51 @@
     fig.suptitle(title, fontsize=fontsize)
 
     # Show the plot
     plt.tight_layout(rect=[0, 0, 1, 0.96])
     plt.show()
     
     
-def plot_p_values_over_time(pval, figsize=(8, 4), total_time_seconds=None, xlabel="Time points", 
+def plot_p_values_over_time(pval, figsize=(8, 4), total_time_seconds=None, xlabel="Timepoints", 
                             ylabel="P-values (Log Scale)",title_text="P-values over time", xlim_start=0, 
                             tick_positions=[0, 0.001, 0.01, 0.05, 0.1, 0.3, 1], num_colors=259, 
                             alpha=0.05,plot_style = "line", linewidth=2.5):
     """
     Plot a scatter plot of p-values over time with a log-scale y-axis and a colorbar.
 
     Parameters:
     -----------
     pval : numpy.ndarray
         The p-values data to be plotted.
     total_time_seconds (float, optional): 
         Total time duration in seconds. If provided, time points will be scaled accordingly.
     xlabel (str, optional): 
-        Label for the x-axis. Default is 'Time points'.
+        Label for the x-axis. Default is 'Timepoints'.
     ylabel (str, optional): 
         Label for the y-axis. Default is 'Y-axis (log scale)'.
     title_text (str, optional): 
         Title for the plot. Default is 'P-values over time'.
     tick_positions (list, optional): 
         Specific values to mark on the y-axis. Default is [0, 0.001, 0.01, 0.05, 0.1, 0.3, 1].
     num_colors (int, optional): 
         Resolution for the color bar. Default is 259.
     alpha (float, optional): 
         Alpha value is the threshold we set for the p-values when doing visualization. Default is 0.05.
     plot_style (str, optional): 
-        Style of plot. Default is 'line'.    
+        Style of plot. Default is 'line'.  
+        
     Returns:
     -----------
     None (displays the plot).
     """
     if pval.ndim != 1:
         # Raise an exception and stop function execution
         raise ValueError("To use the function 'plot_p_values_over_time', the variable for p-values must be one-dimensional.")
 
-    # Generate time points based on total_time_seconds
+    # Generate Timepoints based on total_time_seconds
     if total_time_seconds:
         time_points = np.linspace(0, total_time_seconds, len(pval))
     else:
         time_points = np.arange(len(pval))
 
     # Convert to log scale
     color_array = np.logspace(-3, 0, num_colors).reshape(1, -1)
@@ -1171,55 +1513,55 @@
 
         # overwrite the values below alpha
         cmap_list[:num_elements_red,:]=cmap_red
         cmap_list[num_elements_red:,:]=cmap_blue
         cmap = LinearSegmentedColormap.from_list('custom_colormap', cmap_list)
             
     # Create the line plot with varying color based on p-values
-    _, ax = plt.subplots(figsize=figsize)
+    _, axes = plt.subplots(figsize=figsize)
 
     # Normalize the data to [0, 1] for the colormap with logarithmic scale
     norm = LogNorm(vmin=1e-3, vmax=1)
 
     if plot_style == "line":
         if alpha !=None:
             # Plot the line segments with varying colors
             for i in range(len(time_points)-1):
                 if pval[i+1]>alpha:
                     color = cmap(norm(pval[i+1]))
                 else:
                     color = cmap(norm(pval[i]))
-                ax.plot([time_points[i], time_points[i+1]], [pval[i], pval[i+1]], color=color, linewidth=linewidth)
+                axes.plot([time_points[i], time_points[i+1]], [pval[i], pval[i+1]], color=color, linewidth=linewidth)
         else:
             for i in range(len(time_points)-1):
                 if pval[i+1]>0.05:
                     color = cmap(norm(pval[i+1]))
                 else:
                     color = cmap(norm(pval[i]))
-                ax.plot([time_points[i], time_points[i+1]], [pval[i], pval[i+1]], color=color, linewidth=linewidth)
+                axes.plot([time_points[i], time_points[i+1]], [pval[i], pval[i+1]], color=color, linewidth=linewidth)
     elif plot_style=="scatter":
-        ax.scatter(time_points, pval, c=pval, cmap=cmap, norm=LogNorm(vmin=1e-3, vmax=1))
+        axes.scatter(time_points, pval, c=pval, cmap=cmap, norm=LogNorm(vmin=1e-3, vmax=1))
     elif plot_style=="scatter_line":
-        ax.scatter(time_points, pval, c=pval, cmap=cmap, norm=LogNorm(vmin=1e-3, vmax=1))    
+        axes.scatter(time_points, pval, c=pval, cmap=cmap, norm=LogNorm(vmin=1e-3, vmax=1))    
             # Draw lines between points
-        ax.plot(time_points, pval, color='black', linestyle='-', linewidth=1)
+        axes.plot(time_points, pval, color='black', linestyle='-', linewidth=1)
     # Add labels and title
-    ax.set_xlabel(xlabel, fontsize=12)
-    ax.set_ylabel(ylabel, fontsize=12)
-    ax.set_title(title_text, fontsize=14)
+    axes.set_xlabel(xlabel, fontsize=12)
+    axes.set_ylabel(ylabel, fontsize=12)
+    axes.set_title(title_text, fontsize=14)
     
     # Set axis limits to focus on the relevant data range
-    ax.set_xlim(xlim_start, len(pval) + 1)
-    ax.set_ylim([0.0008, 1.5])
+    axes.set_xlim(xlim_start, len(pval) + 1)
+    axes.set_ylim([0.0008, 1.5])
     # Set y-axis to log scale
-    ax.set_yscale('log')
+    axes.set_yscale('log')
     # Mark specific values on the y-axis
     plt.yticks([0.001, 0.01, 0.05, 0.1, 0.3, 1], ['0.001', '0.01', '0.05', '0.1', '0.3', '1'])
     # Add a colorbar to show the correspondence between colors and p-values
-    divider = make_axes_locatable(ax)
+    divider = make_axes_locatable(axes)
     cax = divider.append_axes("right", size="5%", pad=0.05)
     colorbar = plt.colorbar(plt.cm.ScalarMappable(norm=norm, cmap=cmap), cax=cax, ticks=np.logspace(-3, 0, num_colors), format="%1.0e")
     colorbar.update_ticks()
 
     # Round the tick values to three decimal places
     rounded_ticks = [round(tick, 3) for tick in colorbar.get_ticks()]
     tick_labels = [f'{tick:.3f}' if tick in tick_positions else '' for tick in rounded_ticks]
@@ -1234,32 +1576,34 @@
     for idx, tick_line in enumerate(colorbar.ax.yaxis.get_ticklines()):
         if idx not in indices_not_empty:
             tick_line.set_visible(False)
 
     plt.show()
     
     
-def plot_p_values_bar(pval,variables=[],  figsize=(9, 4), num_colors=256, xlabel="",
+def plot_p_values_bar(pval,xticklabels=[],  figsize=(9, 4), num_colors=256, xlabel="",
                         ylabel="P-values (Log Scale)", title_text="Bar Plot",
                         tick_positions=[0, 0.001, 0.01, 0.05, 0.1, 0.3, 1], top_adjustment=0.9, alpha = 0.05, pad_title=20):
     """
     Visualize a bar plot with LogNorm and a colorbar.
 
     Parameters:
-    - variables (list): List of categories or variables.
-    - pval (array-like): Array of p-values.
-    - figsize (tuple, optional): Figure size, default is (9, 4).
-    - num_colors (int, optional): Number of colors in the colormap, default is 256.
-    - xlabel (str, optional): X-axis label, default is "Categories".
-    - ylabel (str, optional): Y-axis label, default is "Values (log scale)".
-    - title_text (str, optional): Plot title, default is "Bar Plot with LogNorm".
-    - tick_positions (list, optional): Positions of ticks on the colorbar, default is [0, 0.001, 0.01, 0.05, 0.1, 0.3, 1].
+    --------------
+    xticklabels (list): List of categories or variables.
+    pval (array-like): Array of p-values.
+    figsize (tuple, optional): Figure size, default is (9, 4).
+    num_colors (int, optional): Number of colors in the colormap, default is 256.
+    xlabel (str, optional): X-axis label, default is "Categories".
+    ylabel (str, optional): Y-axis label, default is "Values (log scale)".
+    title_text (str, optional): Plot title, default is "Bar Plot with LogNorm".
+    tick_positions (list, optional): Positions of ticks on the colorbar, default is [0, 0.001, 0.01, 0.05, 0.1, 0.3, 1].
     top_adjustment (float, optional): Adjustment for extra space between title and plot, default is 0.9.
 
     Returns:
+    ---------
     None
     """
     # Choose a colormap
     coolwarm_cmap = custom_colormap()
 
     # Convert to log scale
     color_array = np.logspace(-3, 0, num_colors).reshape(1, -1)
@@ -1301,47 +1645,47 @@
         cmap_list[num_elements_red:,:]=cmap_blue
 
     
     # Create a LinearSegmentedColormap
     colormap = LinearSegmentedColormap.from_list('custom_colormap', cmap_list)
 
     # Plot the bars with LogNorm
-    fig, ax = plt.subplots(figsize=figsize)
+    fig, axes = plt.subplots(figsize=figsize)
     if isinstance(pval, (float, np.ndarray)) and np.size(pval) == 1:
     # It's a scalar, create a list with a single element
-        variables = [f"Var 1"] if variables==[] else variables
+        xticklabels = [f"Var 1"] if xticklabels==[] else xticklabels
     else:
         # It's an iterable, use len()
-        variables =[f"Var {i+1}" for i in np.arange(len(pval))] if variables==[] else variables
+        xticklabels =[f"Var {i+1}" for i in np.arange(len(pval))] if xticklabels==[] else xticklabels
 
 
-    bars = plt.bar(variables, pval, color=colormap(LogNorm(vmin=1e-3, vmax=1)(pval)))
+    bars = plt.bar(xticklabels, pval, color=colormap(LogNorm(vmin=1e-3, vmax=1)(pval)))
     # Remove the legend
     #plt.legend().set_visible(False)
 
     # Add data labels on top of the bars
     for bar in bars:
         yval = bar.get_height()
         plt.text(bar.get_x() + bar.get_width()/2, yval + 0.5, round(yval, 3), ha='center', va='bottom', color='black', fontweight='bold')
 
 
     # Set y-axis to log scale
-    ax.set_yscale('log')
+    axes.set_yscale('log')
 
     # Customize plot
     plt.yscale('log')
-    ax.set_xlabel(xlabel, fontsize=12)
-    ax.set_ylabel(ylabel, fontsize=12)
-    ax.set_title(title_text, fontsize=14, pad=pad_title)
+    axes.set_xlabel(xlabel, fontsize=12)
+    axes.set_ylabel(ylabel, fontsize=12)
+    axes.set_title(title_text, fontsize=14, pad=pad_title)
 
     # Mark specific values on the y-axis
     plt.yticks([0.001, 0.01, 0.05, 0.1, 0.3, 1], ['0.001', '0.01', '0.05', '0.1', '0.3', '1'])
 
     # Add a colorbar to show the correspondence between colors and p-values
-    divider = make_axes_locatable(ax)
+    divider = make_axes_locatable(axes)
     cax = divider.append_axes("right", size="5%", pad=0.05)
     colorbar = plt.colorbar(plt.cm.ScalarMappable(cmap=colormap, norm=LogNorm(vmin=1e-3, vmax=1)), cax=cax, ticks=np.logspace(-3, 0, num_colors), format="%1.0e")
     colorbar.update_ticks()
 
     # Round the tick values to three decimal places
     rounded_ticks = [round(tick, 3) for tick in colorbar.get_ticks()]
     tick_labels = [f'{tick:.3f}' if tick in tick_positions else '' for tick in rounded_ticks]
@@ -1356,12 +1700,12 @@
     for idx, tick_line in enumerate(colorbar.ax.yaxis.get_ticklines()):
         if idx not in indices_not_empty:
             tick_line.set_visible(False)
 
     # Add extra space between title and plot
     plt.subplots_adjust(top=top_adjustment)
     plt.xticks(rotation=45, ha='right')  # Rotate x-axis labels for better readability
-    ax.spines['right'].set_visible(False)
-    ax.spines['top'].set_visible(False)
+    axes.spines['right'].set_visible(False)
+    axes.spines['top'].set_visible(False)
     plt.tight_layout()
 
-    plt.show()
+    plt.show()
```

### Comparing `glhmm-0.2.3/glhmm/io.py` & `glhmm-0.2.4/glhmm/io.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.3/glhmm/palm_functions.py` & `glhmm-0.2.4/glhmm/palm_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # Sep/2023 (first version)
 
 # We would like to acknowledge Anderson M. Winkler and all contributors to the PALM package for their valuable work in the field of permutation analysis.
 
 import numpy as np
 import pandas as pd
 import copy
+import warnings
+
 ######################### PART 0 - hcp2block #########################################################
 def hcp2block(tmp, blocksfile=None, dz2sib=False, ids=None):
     """
     Convert HCP-style twin data into block structure.
 
     Parameters:
     --------------
@@ -1108,15 +1110,16 @@
     EE (bool, optional): A flag indicating whether to assume exchangeable errors, which allows permutation.
                         Defaults to True.
 
     Returns:
     ----------  
     list: A list containing the generated permutations.
     """
-    
+    # Filter out the specific RuntimeWarning
+    warnings.filterwarnings("ignore", message="overflow encountered in exp")
     # Reindex the input matrix for palm methods with 'fixleaves'
     EB2 = palm_reindex(EB, 'fixleaves')
     
     # Generate a palm tree structure from the reindexed matrix
     Ptree = palm_tree(EB2)
     
     # Generate a set of shufflings (permutations) based on the palm tree structure
```

### Comparing `glhmm-0.2.3/glhmm/prediction.py` & `glhmm-0.2.4/glhmm/prediction.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.3/glhmm/preproc.py` & `glhmm-0.2.4/glhmm/preproc.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.3/glhmm/statistics.py` & `glhmm-0.2.4/glhmm/statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,72 +10,84 @@
 from glhmm.palm_functions import *
 from statsmodels.stats import multitest as smt
 from sklearn.cross_decomposition import CCA
 from skimage.measure import label, regionprops
 from scipy.stats import ttest_ind, f_oneway, pearsonr, f, norm
 
 
-def test_across_subjects(D_data, R_data, method="regression", Nperm=0, confounds = None, dict_family = None, test_statistics_option=False, FWER_correction=False, identify_categories=False, category_lim=10, test_combination=False):
+def test_across_subjects(D_data, R_data, method="regression", Nperm=0, confounds = None, dict_family = None, verbose = True, test_statistics_option=False, FWER_correction=False, identify_categories=False, category_lim=10, test_combination=False):
     """
     This function performs statistical tests between a independent variable (`D_data`) and the dependent-variable (`R_data`) using permutation testing.
     The permutation testing is performed across across different subjects and it is possible to take family structure into account.
     This procedure is particularly valuable for investigating the differences between subjects in one's study. 
     
     Three options are available to customize the statistical analysis to a particular research questions:
         - "regression": Perform permutation testing using regression analysis.
         - "univariate": Conduct permutation testing with correlation analysis.
         - "cca": Apply permutation testing using canonical correlation analysis.
         
     Parameters:
     --------------
-    D_data (numpy.ndarray): Input data array of shape that can be either a 2D array or a 3D array.
-                            For 2D, the data is represented as a (n, p) matrix, where n represents 
-                            the number of subjects, and p represents the number of predictors.
-                            For 3D array, it has a shape (T, n, q), where the first dimension 
-                            represents timepoints, the second dimension represents the number of subjects, 
-                            and the third dimension represents features. 
-                            For 3D, permutation testing is performed per timepoint for each subject.              
-    R_data (numpy.ndarray): The dependent variable can be either a 2D array or a 3D array. 
-                            For 2D array, it has a shape of (n, q), where n represents 
-                            the number of subjects, and q represents the outcome of the dependent variable.
-                            For 3D array, it has a shape (T, n, q), where the first dimension 
-                            represents timepoints, the second dimension represents the number of subjects, 
-                            and the third dimension represents a dependent variable.   
-                            For 3D, permutation testing is performed per timepoint for each subject.                 
-    method (str, optional): The statistical method to be used for the permutation test. Valid options are
-                            "regression", "univariate", or "cca". (default: "regression").      
-                            Note: "cca" stands for Canonical Correlation Analysis                                        
+    D_data (numpy.ndarray): 
+        Input data array of shape that can be either a 2D array or a 3D array.
+        For 2D, the data is represented as a (n, p) matrix, where n represents 
+        the number of subjects, and p represents the number of predictors.
+        For 3D array, it has a shape (T, n, q), where the first dimension 
+        represents timepoints, the second dimension represents the number of subjects, 
+        and the third dimension represents features. 
+        For 3D, permutation testing is performed per timepoint for each subject.              
+    R_data (numpy.ndarray): 
+        The dependent variable can be either a 2D array or a 3D array. 
+        For 2D array, it has a shape of (n, q), where n represents 
+        the number of subjects, and q represents the outcome of the dependent variable.
+        For 3D array, it has a shape (T, n, q), where the first dimension 
+        represents timepoints, the second dimension represents the number of subjects, 
+        and the third dimension represents a dependent variable.   
+        For 3D, permutation testing is performed per timepoint for each subject.                 
+    method (str, optional): 
+        The statistical method to be used for the permutation test. Valid options are
+        "regression", "univariate", or "cca". (default: "regression").      
+        Note: "cca" stands for Canonical Correlation Analysis                                        
     Nperm (int): Number of permutations to perform (default: 1000).                       
     confounds (numpy.ndarray or None, optional): 
-                            The confounding variables to be regressed out from the input data (D_data).
-                            If provided, the regression analysis is performed to remove the confounding effects. 
-                            (default: None)     
+        The confounding variables to be regressed out from the input data (D_data).
+        If provided, the regression analysis is performed to remove the confounding effects. 
+        (default: None)     
     dict_family (dict): 
-                            Dictionary containing family structure information.                          
-                                - file_location (str): The file location of the family structure data in CSV format.
-                                - M (numpy.ndarray, optional): The matrix of attributes, which is not typically required.
-                                                          Defaults to None.
-                                - CMC (bool, optional): A flag indicating whether to use the Conditional Monte Carlo method (CMC).
-                                              Defaults to False.
-                                - EE (bool, optional): A flag indicating whether to assume exchangeable errors, which allows permutation.
-                                              Defaults to True. Other options are not available.            
+        Dictionary containing family structure information.                          
+            - file_location (str): The file location of the family structure data in CSV format.
+            - M (numpy.ndarray, optional): The matrix of attributes, which is not typically required.
+                                        Defaults to None.
+            - CMC (bool, optional): A flag indicating whether to use the Conditional Monte Carlo method (CMC).
+                            Defaults to False.
+            - EE (bool, optional): A flag indicating whether to assume exchangeable errors, which allows permutation.
+                            Defaults to True. Other options are not available.
+    verbose (bool, optional): 
+        If True, display progress messages. If False, suppress progress messages.                                                      
     test_statistics_option (bool, optional): 
-                            If True, the function will return the test statistics for each permutation.
-                            (default: False) 
+        If True, the function will return the test statistics for each permutation.
+        (default: False) 
     FWER_correction (bool, optional): 
-                            Specify whether to perform family-wise error rate (FWER) correction using the MaxT method (default: False)                   
+        Specify whether to perform family-wise error rate (FWER) correction using the MaxT method (default: False) 
+        Note: FWER_correction is not necessary if pval_correction is applied later for multiple comparison p-value correction.                  
     identify_categories : bool or list or numpy.ndarray, optional, default=True
-                            If True, automatically identify categorical columns. If list or ndarray, use the provided list of column indices.    
+        If True, automatically identify categorical columns. If list or ndarray, use the provided list of column indices.    
     category_lim : int or None, optional, default=10
-                            Maximum allowed number of categories for F-test. Acts as a safety measure for columns 
-                            with integer values, like age, which may be mistakenly identified as multiple categories.        
-    test_combination:       Calculates geometric means of p-values using permutation testing (default: False). Valid options are:
-                                - True (bool): Return a single geometric mean per time point.
-                                - "rows" (str): Calculate geometric means for each row.
-                                - "columns" (str): Calculate geometric means for each column.
+        Maximum allowed number of categories for F-test. Acts as a safety measure for columns 
+        with integer values, like age, which may be mistakenly identified as multiple categories.        
+    test_combination:       
+        Calculates geometric means of p-values using permutation testing (default: False).
+        In the context of p-values from permutation testing, calculating geometric means
+        can be useful for summarizing results across multiple tests to get insights into the overall
+        statistical significance across experimental conditions.
+        Valid options are:
+            - True (bool): Return a single geometric mean value.
+            - "across_rows" (str): Calculates geometric means aggregated across rows.
+            - "across_columns" (str): Calculates geometric means aggregated across columns. 
+                                
                                 
                             
                          
     Returns:
     ----------  
     result (dict): A dictionary containing the following keys. Depending on the `test_statistics_option` and `method`, it can return the p-values, 
         correlation coefficients, test statisticss.
@@ -106,27 +118,27 @@
         Nperm+=1
     
     # Check validity of method and data_type
     valid_methods = ["regression", "univariate", "cca"]
     validate_condition(method in valid_methods, "Invalid option specified for 'method'. Must be one of: " + ', '.join(valid_methods))
     
     # Check validity of method
-    valid_test_combination = [False, True, "columns", "rows"]
+    valid_test_combination = [False, True, "across_columns", "across_rows"]
     validate_condition(test_combination in valid_test_combination, "Invalid option specified for 'test_combination'. Must be one of: " + ', '.join(map(str, valid_test_combination)))
     
     if method=="regression" and test_combination in valid_test_combination[-1:]:
             raise ValueError("method is set to 'regression' and 'test_combination' is set to 'rows' "
                          "If you want to perform 'test_combination' while doing 'regression' then please set 'test_combination' to 'True' or 'columns'.")
 
-    if FWER_correction and test_combination in [True, "columns", "rows"]:
+    if FWER_correction and test_combination in [True, "across_columns", "across_rows"]:
        # Raise an exception and stop function execution
         raise ValueError("'FWER_correction' is set to True and 'test_combination' is either True, 'columns', or 'rows'. "
                          "Please set 'FWER_correction' to False if you want to apply 'test_combination' or set 'test_combination' to False if you want to run 'FWER_correction'.")
     # Get the shapes of the data
-    n_T, _, n_p, n_q, D_data, R_data = get_input_shape(D_data, R_data)
+    n_T, _, n_p, n_q, D_data, R_data = get_input_shape(D_data, R_data, verbose)
     # Note for convension we wrote (T, p, q) => (n_T, n_p, n_q)
     
     # Identify categorical columns in R_data
     category_columns = identify_coloumns_for_t_and_f_tests(R_data, method, identify_categories, category_lim) if method=="univariate" or method =="regression" else {'t_test_cols': [], 'f_test_cols': []}
 
     if category_columns["t_test_cols"]!=[] or category_columns["f_test_cols"]!=[]:
         if FWER_correction and (len(category_columns.get('t_test_cols')) != R_data.shape[-1] or len(category_columns.get('f_test_cols')) != R_data.shape[-1]):
@@ -139,15 +151,15 @@
         dict_mfam=process_family_structure(dict_family, Nperm) 
         
     
     # Initialize arrays based on shape of data shape and defined options
     pval, base_statistics, test_statistics_list = initialize_arrays(R_data, n_p, n_q, n_T, method, Nperm, test_statistics_option, test_combination)
     
 
-    for t in tqdm(range(n_T)) if n_T > 1 else range(n_T):
+    for t in tqdm(range(n_T)) if n_T > 1 & verbose ==True else range(n_T):
         # If confounds exist, perform confound regression on the dependent variables
         D_t, R_t = deconfound_values(D_data[t, :],R_data[t, :], confounds)
         
         # Removing rows that contain nan-values
         if method == "regression" or method == "cca":
             # Removing rows that contain nan-values
             D_t, R_t = remove_nan_values(D_t, R_t, t, n_T, method)
@@ -162,15 +174,15 @@
         else:
             # Call function "__palm_quickperms" from glhmm.palm_functions
             permutation_matrix = __palm_quickperms(dict_mfam["EB"], M=dict_mfam["M"], nP=dict_mfam["nP"], 
                                             CMC=dict_mfam["CMC"], EE=dict_mfam["EE"])
             # Need to convert the index so it starts from 0
             permutation_matrix = permutation_matrix-1
             
-        for perm in tqdm(range(Nperm)) if n_T == 1 else range(Nperm):
+        for perm in tqdm(range(Nperm)) if n_T == 1 & verbose==True else range(Nperm):
             # Perform permutation on R_t
             Rin = R_t[permutation_matrix[:, perm]]
             # Calculate the permutation distribution
             test_statistics, bstat = test_statistics_calculations(D_t, Rin, perm, test_statistics, proj, method, category_columns,test_combination)
             base_statistics[t, :] = bstat if perm == 0 and bstat is not None else base_statistics[t, :]
 
         # Calculate p-values
@@ -181,15 +193,15 @@
             test_statistics_list[t,:] = test_statistics
             
     pval =np.squeeze(pval) if np.abs(np.nansum(pval))>0 else np.nan 
     base_statistics =np.squeeze(base_statistics) if base_statistics is not None else [] 
     test_statistics_list =np.squeeze(test_statistics_list) if test_statistics_list is not None else []
     Nperm = 0 if Nperm==1 else Nperm
     
-    if np.sum(np.isnan(pval))>0:
+    if np.sum(np.isnan(pval))>0 & verbose:
         print("Warning: Permutation testing resulted in p-values equal to NaN.")
         print("This may indicate an issue with the input data. Please review your data.")
     
     # Return results
     result = {
         'pval': pval,
         'base_statistics': base_statistics,
@@ -200,15 +212,15 @@
         'max_correction':FWER_correction,
         'performed_tests': category_columns,
         'Nperm': Nperm}
     return result
 
 
 
-def test_across_trials_within_session(D_data, R_data, idx_data, method="regression", Nperm=0, confounds=None, trial_timepoints=None,test_statistics_option=False, FWER_correction=False, identify_categories=False, category_lim=10, test_combination=False):
+def test_across_trials_within_session(D_data, R_data, idx_data, method="regression", Nperm=0, confounds=None, trial_timepoints=None,verbose=True, test_statistics_option=False, FWER_correction=False, identify_categories=False, category_lim=10, test_combination=False):
     """
     This function performs statistical tests between a independent variable (`D_data`) and the dependent-variable (`R_data`) using permutation testing.
     The permutation testing is performed across different trials within a session using permutation testing
     This procedure is particularly valuable for investigating the differences between trials in one or more sessions.  
     An example could be if we want to test if any learning is happening during a session that might speed up times.
     
     Three options are available to customize the statistical analysis to a particular research questions:
@@ -237,29 +249,32 @@
                                 "regression", "univariate", or "cca". (default: "regression").
                                 Note: "cca" stands for Canonical Correlation Analysis    
         Nperm (int): Number of permutations to perform (default: 1000). 
         confounds (numpy.ndarray or None, optional): 
                                 The confounding variables to be regressed out from the input data (D_data).
                                 If provided, the regression analysis is performed to remove the confounding effects. 
                                 (default: None):    
-        trial_timepoints (int): Number of timepoints for each trial (default: None)                                                          
+        trial_timepoints (int): Number of timepoints for each trial (default: None)   
+        verbose (bool, optional): 
+                                If True, display progress messages. If False, suppress progress messages.                                                       
         test_statistics_option (bool, optional): 
                                 If True, the function will return the test statistics for each permutation.
                                 (default: False) 
         FWER_correction (bool, optional): 
-                                Specify whether to perform family-wise error rate (FWER) correction for multiple comparisons using the MaxT method(default: False).                        
+                                Specify whether to perform family-wise error rate (FWER) correction for multiple comparisons using the MaxT method(default: False).
+                                Note: FWER_correction is not necessary if pval_correction is applied later for multiple comparison p-value correction.                        
         identify_categories : bool or list or numpy.ndarray, optional, default=True
                                 If True, automatically identify categorical columns. If list or ndarray, use the provided list of column indices.    
         category_lim : int or None, optional, default=None
                                 Maximum allowed number of categories for F-test. Acts as a safety measure for columns 
                                 with integer values, like age, which may be mistakenly identified as multiple categories.     
         test_combination:       Calculates geometric means of p-values using permutation testing (default: False). Valid options are:
                                 - True (bool): Return a single geometric mean per time point.
-                                - "rows" (str): Calculate geometric means for each row.
-                                - "columns" (str): Calculate geometric means for each column.                                                
+                                - "across_rows" (str): Calculate geometric means for each row.
+                                - "across_columns" (str): Calculate geometric means for each column.                                                
     Returns:
     ----------  
     result (dict): A dictionary containing the following keys. Depending on the `test_statistics_option` and `method`, it can return the p-values, 
         correlation coefficients, test statisticss.
         'pval': P-values for the test with shapes based on the method:
             - method=="Regression": (T, p)
             - method=="univariate": (T, p, q)
@@ -288,28 +303,28 @@
         
           
     # Check validity of method and data_type
     valid_methods = ["regression", "univariate", "cca"]
     validate_condition(method in valid_methods, "Invalid option specified for 'method'. Must be one of: " + ', '.join(valid_methods))
     
     # Check validity of method
-    valid_test_combination = [False, True, "columns", "rows"]
+    valid_test_combination = [False, True, "across_columns", "across_rows"]
     validate_condition(test_combination in valid_test_combination, "Invalid option specified for 'test_combination'. Must be one of: " + ', '.join(map(str, valid_test_combination)))
     
     if method=="regression" and test_combination in valid_test_combination[-1:]:
             raise ValueError("method is set to 'regression' and 'test_combination' is set to 'rows' "
                          "If you want to perform 'test_combination' while doing 'regression' then please set 'test_combination' to 'True' or 'columns'.")
 
-    if FWER_correction and test_combination in [True, "columns", "rows"]:
+    if FWER_correction and test_combination in [True, "across_columns", "across_rows"]:
        # Raise an exception and stop function execution
         raise ValueError("'FWER_correction' is set to True and 'test_combination' is either True, 'columns', or 'rows'. "
                          "Please set 'FWER_correction' to False if you want to apply 'test_combination' or set 'test_combination' to False if you want to run 'FWER_correction'.")
 
     # Get input shape information
-    n_T, _, n_p, n_q, D_data, R_data = get_input_shape(D_data, R_data)
+    n_T, _, n_p, n_q, D_data, R_data = get_input_shape(D_data, R_data, verbose)
 
     # Identify categorical columns in R_data
     category_columns = identify_coloumns_for_t_and_f_tests(R_data, method, identify_categories, category_lim) if method=="univariate" or method =="regression" else {'t_test_cols': [], 'f_test_cols': []}
     
     if category_columns["t_test_cols"]!=[] or category_columns["f_test_cols"]!=[]:
         if FWER_correction and (len(category_columns.get('t_test_cols')) != R_data.shape[-1] or len(category_columns.get('f_test_cols')) != R_data.shape[-1]):
             print("Warning: Cannot perform FWER_correction with different test statisticss.\nConsider to set identify_categories=False")
@@ -320,15 +335,15 @@
         idx_array = get_indices_array(idx_data)
     else:
         idx_array =idx_data.copy()        
 
     # Initialize arrays based on shape of data shape and defined options
     pval, base_statistics, test_statistics_list = initialize_arrays(R_data, n_p, n_q, n_T, method, Nperm, test_statistics_option, test_combination)
 
-    for t in tqdm(range(n_T)) if n_T > 1 else range(n_T):
+    for t in tqdm(range(n_T)) if n_T > 1 & verbose ==True else range(n_T):
         # If confounds exist, perform confound regression on the dependent variables
         D_t, R_t = deconfound_values(D_data[t, :],R_data[t, :], confounds)
         
         # Removing rows that contain nan-values
         if method == "regression" or method == "cca":
             D_t, R_t = remove_nan_values(D_t, R_t, t, n_T, method)
         
@@ -352,15 +367,15 @@
         if test_statistics_option==True:
             test_statistics_list[t,:] = test_statistics
     pval =np.squeeze(pval) if np.abs(np.nansum(pval))>0 else np.nan
     base_statistics =np.squeeze(base_statistics) if base_statistics is not None  else []
     test_statistics_list =np.squeeze(test_statistics_list) if test_statistics_list is not None else []
     Nperm = 0 if Nperm==1 else Nperm
     
-    if np.sum(np.isnan(pval))>0:
+    if np.sum(np.isnan(pval))>0 & verbose:
         print("Warning: Permutation testing resulted in p-values equal to NaN.")
         print("This may indicate an issue with the input data. Please review your data.")
         
     # Return results
     result = {
         'pval': pval,
         'base_statistics': base_statistics,
@@ -370,15 +385,15 @@
         'test_combination': test_combination,
         'max_correction':FWER_correction,
         'performed_tests': category_columns,
         'Nperm': Nperm}
     
     return result
 
-def test_across_sessions_within_subject(D_data, R_data, idx_data, method="regression", Nperm=0, confounds=None,test_statistics_option=False,FWER_correction=False, identify_categories=False, category_lim=10, test_combination=False):
+def test_across_sessions_within_subject(D_data, R_data, idx_data, method="regression", Nperm=0, confounds=None, verbose = True, test_statistics_option=False,FWER_correction=False, identify_categories=False, category_lim=10, test_combination=False):
     """
     This function performs statistical tests between a independent variable (`D_data`) and the dependent-variable (`R_data`) using permutation testing. 
     The permutation testing is performed across sessions within the same subject, while keeping the trial order the same.
     This procedure is particularly valuable for investigating the effects of long-term treatments or monitoring changes in brain responses across sessions over time.
 
     Three options are available to customize the statistical analysis to a particular research questions:
         - 'regression': Perform permutation testing using regression analysis.
@@ -404,29 +419,32 @@
         method (str, optional): The statistical method to be used for the permutation test. Valid options are
                                 "regression", "univariate", or "cca". (default: "regression").
                                 Note: "cca" stands for Canonical Correlation Analysis    
         Nperm (int): Number of permutations to perform (default: 1000).                
         confounds (numpy.ndarray or None, optional): 
                                 The confounding variables to be regressed out from the input data (D_data).
                                 If provided, the regression analysis is performed to remove the confounding effects. 
-                                (default: None):                                                              
+                                (default: None):                           
+        verbose (bool, optional): 
+                                If True, display progress messages and prints. If False, suppress messages.                                                             
         test_statistics_option (bool, optional): 
                                 If True, the function will return the test statistics for each permutation.
                                 (default: False) 
         FWER_correction (bool, optional): 
                                 Specify whether to perform family-wise error rate (FWER) correction for multiple comparisons using the MaxT method(default: False).
+                                Note: FWER_correction is not necessary if pval_correction is applied later for multiple comparison p-value correction.
         identify_categories : bool or list or numpy.ndarray, optional, default=True
                                 If True, automatically identify categorical columns. If list or ndarray, use the provided list of column indices.    
         category_lim : int or None, optional, default=None
                                 Maximum allowed number of categories for F-test. Acts as a safety measure for columns 
                                 with integer values, like age, which may be mistakenly identified as multiple categories.
         test_combination:       Calculates geometric means of p-values using permutation testing (default: False). Valid options are:
                                 - True (bool): Return a single geometric mean per time point.
-                                - "rows" (str): Calculate geometric means for each row.
-                                - "columns" (str): Calculate geometric means for each column.                         
+                                - "across_rows" (str): Calculate geometric means for each row.
+                                - "across_columns" (str): Calculate geometric means for each column.                         
     Returns:
     ----------  
         result (dict): A dictionary containing the following keys. Depending on the `test_statistics_option` and `method`, it can return the p-values, 
             correlation coefficients, test statisticss.
             'pval': P-values for the test with shapes based on the method:
                 - method=="Regression": (T, p)
                 - method=="univariate": (T, p, q)
@@ -455,46 +473,46 @@
         Nperm+=1
      
     # Check validity of method and data_type
     valid_methods = ["regression", "univariate", "cca"]
     validate_condition(method in valid_methods, "Invalid option specified for 'method'. Must be one of: " + ', '.join(valid_methods))
     
     # Check validity of method
-    valid_test_combination = [False, True, "columns", "rows"]
+    valid_test_combination = [False, True, "across_columns", "across_rows"]
     validate_condition(test_combination in valid_test_combination, "Invalid option specified for 'test_combination'. Must be one of: " + ', '.join(map(str, valid_test_combination)))
     
     if method=="regression" and test_combination in valid_test_combination[-1:]:
             raise ValueError("method is set to 'regression' and 'test_combination' is set to 'rows' "
                          "If you want to perform 'test_combination' while doing 'regression' then please set 'test_combination' to 'True' or 'columns'.")
 
-    if FWER_correction and test_combination in [True, "columns", "rows"]:
+    if FWER_correction and test_combination in [True, "across_columns", "across_rows"]:
        # Raise an exception and stop function execution
         raise ValueError("'FWER_correction' is set to True and 'test_combination' is either True, 'columns', or 'rows'. "
                          "Please set 'FWER_correction' to False if you want to apply 'test_combination' or set 'test_combination' to False if you want to run 'FWER_correction'.")
     
     # Get indices for permutation
     if len(idx_data.shape)==2:
         idx_array = get_indices_array(idx_data)
     else:
         idx_array =idx_data.copy()
 
     # Get input shape information
-    n_T, _, n_p, n_q, D_data, R_data = get_input_shape(D_data, R_data)
+    n_T, _, n_p, n_q, D_data, R_data = get_input_shape(D_data, R_data, verbose)
     
     # Identify categorical columns in R_data
     category_columns = identify_coloumns_for_t_and_f_tests(R_data, method, identify_categories, category_lim) if method=="univariate" or method =="regression" else {'t_test_cols': [], 'f_test_cols': []}
     
     if category_columns["t_test_cols"]!=[] or category_columns["f_test_cols"]!=[]:
         if FWER_correction and (len(category_columns.get('t_test_cols')) != R_data.shape[-1] or len(category_columns.get('f_test_cols')) != R_data.shape[-1]):
             print("Warning: Cannot perform FWER_correction with different test statisticss.\nConsider to set identify_categories=False")
             raise ValueError("Cannot perform FWER_correction")
 
 # Initialize arrays based on shape of data shape and defined options
     pval, base_statistics, test_statistics_list = initialize_arrays(R_data, n_p, n_q, n_T, method, Nperm, test_statistics_option, test_combination)
-    for t in tqdm(range(n_T)) if n_T > 1 else range(n_T):
+    for t in tqdm(range(n_T)) if n_T > 1 & verbose==True else range(n_T):
         # If confounds exist, perform confound regression on the dependent variables
         D_t, R_t = deconfound_values(D_data[t, :],R_data[t, :], confounds)
         
         # Removing rows that contain nan-values
         if method == "regression" or method == "cca":
             D_t, R_t = remove_nan_values(D_t, R_t, t, n_T, method)
 
@@ -517,15 +535,15 @@
         if test_statistics_option==True:
             test_statistics_list[t,:] = test_statistics
             
     pval =np.squeeze(pval) if np.abs(np.nansum(pval))>0 else np.nan 
     base_statistics =np.squeeze(base_statistics) if base_statistics is not None  else []
     test_statistics_list =np.squeeze(test_statistics_list) if test_statistics_list is not None  else []
     Nperm = 0 if Nperm==1 else Nperm    
-    if np.sum(np.isnan(pval))>0:
+    if np.sum(np.isnan(pval))>0 & verbose:
         print("Warning: Permutation testing resulted in p-values equal to NaN.")
         print("This may indicate an issue with the input data. Please review your data.")
               
     # Return results
     result = {
         'pval': pval,
         'base_statistics': base_statistics,
@@ -534,44 +552,46 @@
         'method': method,
         'test_combination': test_combination,
         'max_correction':FWER_correction,
         'performed_tests': category_columns,
         'Nperm': Nperm}
     return result
 
-def test_across_visits(input_data, vpath_data, n_states, method="regression", Nperm=0, confounds=None, test_statistics_option=False, pairwise_statistic ="mean",FWER_correction=False, category_lim=None, identify_categories = False):
+def test_across_visits(input_data, vpath_data, n_states, method="regression", Nperm=0, verbose = True, confounds=None, test_statistics_option=False, pairwise_statistic ="mean",FWER_correction=False, category_lim=None, identify_categories = False):
     from itertools import combinations
     """
     Perform permutation testing within a session for continuous data.
     This function performs statistical tests, such as regression, correlation, 
     canonical correlation analysis (cca), one-vs-rest, and state pairs, 
     between a dependent variable (`input_data`) and a hidden state path (`vpath_data`) using permutation testing. 
 
-
     Parameters:
     --------------            
         input_data (numpy.ndarray): Dependent variable with shape (n, q), where n is the number of samples (n_timepoints x n_trials), 
                                     and q represents dependent/target variables.  
         vpath_data (numpy.ndarray): The hidden state path data of the continuous measurements represented as a (n, p) matrix. 
                                     It could be a 2D matrix where each row represents a trials over a period of time and
                                     each column represents a state variable and gives the shape ((n_timepoints X n_trials), n_states). 
                                     If it is a 1D array of of shape ((n_timepoints X n_trials),) where each row value represent a giving state.                                 
         n_states (int):             The number of hidden states in the hidden state path data.
         method (str, optional):     Statistical method for the permutation test. Valid options are 
                                     "regression", "univariate", "cca", "one_vs_rest" or "state_pairs". 
                                     Note: "cca" stands for Canonical Correlation Analysis.   
         Nperm (int):                Number of permutations to perform (default: 0). 
+        verbose (bool, optional): 
+                            If True, display progress messages. If False, suppress progress messages.
         test_statistics_option (bool, optional): 
                                     If True, the function will return the test statistics for each permutation.
                                     (default: False) 
         pairwise_statistic (str, optional)  
                                     The chosen statistic when applying methods "one_vs_rest" or "state_pairs". 
                                     Valid options are "mean" or "median" (default: "mean").
         FWER_correction (bool, optional): 
                                     Specify whether to perform family-wise error rate (FWER) correction for multiple comparisons using the MaxT method(default: False).
+                                    Note: FWER_correction is not necessary if pval_correction is applied later for multiple comparison p-value correction.
                      
     Returns:
     ----------  
         result (dict): A dictionary containing the following keys. Depending on the `test_statistics_option` and `method`, it can return the p-values, 
             correlation coefficients, test statisticss.
             'pval': P-values for the test with shapes based on the method:
                 - method=="Regression": (T, p)
@@ -603,18 +623,18 @@
     validate_condition(pairwise_statistic.lower() in valid_statistic, "Invalid option specified for 'statistic'. Must be one of: " + ', '.join(valid_statistic))
     
     # Convert vpath from matrix to vector
     vpath_array=generate_vpath_1D(vpath_data)
 
     if method == 'regression':
         # Get input shape information
-        n_T, _, n_p, n_q, input_data, vpath_data= get_input_shape(input_data, vpath_array)
+        n_T, _, n_p, n_q, input_data, vpath_data= get_input_shape(input_data, vpath_array, verbose)
     else:
         # Get input shape information
-        n_T, _, n_p, n_q, input_data, vpath_data= get_input_shape(input_data, vpath_data)  
+        n_T, _, n_p, n_q, input_data, vpath_data= get_input_shape(input_data, vpath_data, verbose)  
 
     # Identify categorical columns in R_data
     category_columns = identify_coloumns_for_t_and_f_tests(vpath_data, method, identify_categories, category_lim) if method=="univariate" or method =="regression" else {'t_test_cols': [], 'f_test_cols': []}
     
     # Identify categorical columns
     if category_columns["t_test_cols"]!=[] or category_columns["f_test_cols"]!=[]:
         if FWER_correction and (len(category_columns.get('t_test_cols')) != vpath_data.shape[-1] or len(category_columns.get('f_test_cols')) != R_data.shape[-1]):
@@ -624,38 +644,38 @@
     # Initialize arrays based on shape of data shape and defined options
     pval, base_statistics, test_statistics_list = initialize_arrays(vpath_data, n_p, n_q,
                                                                             n_T, method, Nperm,
                                                                             test_statistics_option)
 
 
     # Print tqdm over n_T if there are more than one timepoint
-    for t in tqdm(range(n_T)) if n_T > 1 else range(n_T):
+    for t in tqdm(range(n_T)) if n_T > 1 & verbose==True else range(n_T):
         # Correct for confounds and center data_t
         data_t, _ = deconfound_values(input_data[t, :],None, confounds)
         
         # Removing rows that contain nan-values
         if method == "regression" or method == "cca":
             data_t, vpath_array = remove_nan_values(data_t, vpath_array, t, n_T, method)
         
         if method != "state_pairs":
             ###################### Permutation testing for other tests beside state pairs #################################
             # Create test_statistics and pval_perms based on method
             test_statistics, proj = initialize_permutation_matrices(method, Nperm, n_p, n_q, 
                                                                             data_t)
             # Perform permutation testing
-            for perm in tqdm(range(Nperm)) if n_T == 1 else range(n_T):
+            for perm in tqdm(range(Nperm)) if n_T == 1 & verbose==True else range(n_T):
                 # Redo vpath_surrogate calculation if the number of states are not the same (out of 1000 permutations it happens maybe 1-2 times with this demo dataset)
                 while True:
                     # Create vpath_surrogate
                     vpath_surrogate = surrogate_state_time(perm, vpath_array, n_states)
                     if len(np.unique(vpath_surrogate)) == n_states:
                         break  # Exit the loop if the condition is satisfied
                 if method =="one_vs_rest":
-                    for state in range(n_states):
-                        test_statistics[perm,state] =calculate_baseline_difference(vpath_surrogate, data_t, state+1, pairwise_statistic.lower())
+                    for state in range(1, n_states+1):
+                        test_statistics[perm,state -1] =calculate_baseline_difference(vpath_surrogate, data_t, state, pairwise_statistic.lower())
                 elif method =="regression":
                     test_statistics, bstat = test_statistics_calculations(data_t,vpath_surrogate , perm,
                                                                             test_statistics, proj, method, category_columns)
                     base_statistics[t, :] = bstat if perm == 0 and bstat is not None else base_statistics[t, :]
                 else:
                     # Apply 1 hot encoding
                     vpath_surrogate_onehot = viterbi_path_to_stc(vpath_surrogate,n_states)
@@ -672,15 +692,16 @@
             data_t, _ = deconfound_values(input_data[t, :],None, confounds)
             
             # Generates all unique combinations of length 2 
             pairwise_comparisons = list(combinations(range(1, n_states + 1), 2))
             test_statistics = np.zeros((Nperm, len(pairwise_comparisons)))
             pval = np.zeros((n_states, n_states))
             # Iterate over pairwise state comparisons
-            for idx, (state_1, state_2) in tqdm(enumerate(pairwise_comparisons), total=len(pairwise_comparisons), desc="Pairwise comparisons"):    
+            
+            for idx, (state_1, state_2) in tqdm(enumerate(pairwise_comparisons), total=len(pairwise_comparisons), desc="Pairwise comparisons") if verbose ==True else enumerate(pairwise_comparisons):    
                 # Generate surrogate state-time data and calculate differences for each permutation
                 for perm in range(Nperm):
                     # Redo vpath_surrogate calculation if the number of states are not the same (out of 1000 permutations it happens maybe 1-2 times with this demo dataset)
                     while True:
                         # Create vpath_surrogate
                         vpath_surrogate = surrogate_state_time(perm, vpath_array, n_states)
                         if len(np.unique(vpath_surrogate)) == n_states:
@@ -700,15 +721,15 @@
             test_statistics_list[t, :] = test_statistics
 
     pval =np.squeeze(pval) if np.abs(np.nansum(pval))>0 else np.nan 
     base_statistics =np.squeeze(base_statistics) if base_statistics is not None else []
     test_statistics_list =np.squeeze(test_statistics_list) if test_statistics_list is not None else []
     Nperm = 0 if Nperm==1 else Nperm
     
-    if np.sum(np.isnan(pval))>0:
+    if np.sum(np.isnan(pval))>0 & verbose:
         print("Warning: Permutation testing resulted in p-values equal to NaN.")
         print("This may indicate an issue with the input data. Please review your data.")
         
     # Return results
     result = {
         'pval': pval,
         'base_statistics': base_statistics,
@@ -791,55 +812,54 @@
         error_message (str): The error message to raise if the condition is not met.
     """
     # Check if a condition is False and raise a ValueError with the given error message
     if not condition:
         raise ValueError(error_message)
 
 
-def get_input_shape(D_data, R_data):
+def get_input_shape(D_data, R_data, verbose):
     """
     Computes the input shape parameters for permutation testing.
 
     Parameters:
     --------------
         D_data (numpy.ndarray): The input data array.
         R_data (numpy.ndarray): The dependent variable.
+        verbose (bool): If True, display progress messages. If False, suppress progress messages.
 
     Returns:
     ----------  
         n_T (int): The number of timepoints.
         n_ST (int): The number of subjects or trials.
         n_p (int): The number of features.
         D_data (numpy.ndarray): The updated input data array.
         R_data (numpy.ndarray): The updated dependent variable.
     """
     # Get the input shape of the data and perform necessary expansions if needed
     if R_data.ndim == 1:
         R_data = np.expand_dims(R_data, axis=1)
     
     if len(D_data.shape) == 1:
-        # This is normally the case when using viterbi path
-        print("performing permutation testing for viterbi path")
         D_data = np.expand_dims(D_data, axis=1)
         D_data = np.expand_dims(D_data, axis=0)
         R_data = np.expand_dims(R_data, axis=0)
         n_T, n_ST, n_p = D_data.shape
         n_q = R_data.shape[-1]
     elif len(D_data.shape) == 2:
         # Performing permutation testing for the whole data
-        
         D_data = np.expand_dims(D_data, axis=0)
         if D_data.ndim !=R_data.ndim:
             R_data = np.expand_dims(R_data, axis=0)
         n_T, n_ST, n_p = D_data.shape
         n_q = R_data.shape[-1]
 
     else:
         # Performing permutation testing per timepoint
-        print("performing permutation testing per timepoint")
+        if verbose:
+            print("performing permutation testing per timepoint")
         n_T, n_ST, n_p = D_data.shape
 
         # Tile the R_data if it doesn't match the number of timepoints in D_data
         if R_data.shape[0] != D_data.shape[0]:
             R_data = np.tile(R_data, (D_data.shape[0],1,1)) 
         n_q = R_data.shape[-1]
     
@@ -933,15 +953,15 @@
         pval (numpy array): p-values for the test (n_T, n_p) if test_statistics_option is False, else None.
         base_statistics (numpy array): Correlation coefficient for the test (n_T, n_p, n_q) if method="univariate", else None.
         test_statistics_list (numpy array): test statistics values (n_T, Nperm, n_p) or (n_T, Nperm, n_p, n_q) if method="univariate" , else None.
     """
     
     # Initialize the arrays based on the selected method and data dimensions
     if  method == "regression":
-        if test_combination in [True, "columns", "rows"]: 
+        if test_combination in [True, "across_columns", "across_rows"]: 
             pval = np.zeros((n_T, 1))
             if test_statistics_option==True:
                 test_statistics_list = np.zeros((n_T, Nperm, 1))
             else:
                 test_statistics_list= None
             base_statistics= np.zeros((n_T, 1, 1))
         else:
@@ -957,20 +977,20 @@
         pval = np.zeros((n_T, 1))
         if test_statistics_option==True:
             test_statistics_list = np.zeros((n_T, Nperm, 1))
         else:
             test_statistics_list= None
         base_statistics= np.zeros((n_T, 1, 1))        
     elif method == "univariate" :  
-        if test_combination in [True, "columns", "rows"]: 
-            pval_shape = (n_T, 1) if test_combination == True else (n_T, n_q) if test_combination == "columns" else (n_T, n_p)
+        if test_combination in [True, "across_columns", "across_rows"]: 
+            pval_shape = (n_T, 1) if test_combination == True else (n_T, n_q) if test_combination == "across_columns" else (n_T, n_p)
             pval = np.zeros(pval_shape)
             base_statistics = pval.copy()
             if test_statistics_option:
-                test_statistics_list_shape = (n_T, Nperm, 1) if test_combination == True else (n_T, Nperm, n_q) if test_combination == "columns" else (n_T, Nperm, n_p)
+                test_statistics_list_shape = (n_T, Nperm, 1) if test_combination == True else (n_T, Nperm, n_q) if test_combination == "across_columns" else (n_T, Nperm, n_p)
                 test_statistics_list = np.zeros(test_statistics_list_shape)
             else:
                 test_statistics_list = None
         else:    
             pval = np.zeros((n_T, n_p, n_q))
             base_statistics = pval.copy()
             if test_statistics_option==True:    
@@ -1056,26 +1076,26 @@
         pval_perms (numpy.ndarray): The p-value permutation array.
         proj (numpy.ndarray or None): The projection matrix (None for correlation methods).
     """
     # Define projection matrix
     proj = None
     # Initialize the permutation matrices based on the selected method
     if method in {"univariate"}:
-        if test_combination in [True, "columns", "rows"]: 
-            test_statistics_shape = (Nperm, 1) if test_combination == True else (Nperm, n_q) if test_combination == "columns" else (Nperm, n_p)
+        if test_combination in [True, "across_columns", "across_rows"]: 
+            test_statistics_shape = (Nperm, 1) if test_combination == True else (Nperm, n_q) if test_combination == "across_columns" else (Nperm, n_p)
             test_statistics = np.zeros(test_statistics_shape)
         else:
             # Initialize test statistics output matrix based on the selected method
             test_statistics = np.zeros((Nperm, n_p, n_q))
         proj = None
     elif method =="cca":
         # Initialize test statistics output matrix based on the selected method
         test_statistics = np.zeros((Nperm, 1))
     else:
-        if test_combination in [True, "columns", "rows"]:
+        if test_combination in [True, "across_columns", "across_rows"]:
             test_statistics = np.zeros((Nperm, 1))
         else:
             # Regression got a N by q matrix 
             test_statistics = np.zeros((Nperm, n_q))
         # Define regularization parameter
         regularization = 0.001
         # Regularized parameter estimation
@@ -1262,45 +1282,46 @@
 
 def permute_subject_trial_idx(idx_array):
     """
     Permutes an array based on unique values while maintaining the structure.
     
     Parameters:
     --------------
-        idx_array (numpy.ndarray): Input array to be permuted.
+    idx_array (numpy.ndarray): Input array to be permuted.
     
     Returns:
     ----------  
-        list: Permuted array based on unique values.
+    list: Permuted array based on unique values.
     """
+    # Get unique values and their counts
     unique_values, value_counts = np.unique(idx_array, return_counts=True)
-    
-    permuted_array = []
-    unique_values_perm = np.random.permutation(unique_values)
-    
-    for value in unique_values_perm:
-        permuted_array.extend([value] * value_counts[np.where(unique_values == value)][0])
-    
+
+    # Permute the unique values
+    permuted_unique_values = np.random.permutation(unique_values)
+
+    # Repeat each unique value according to its original count
+    permuted_array = np.repeat(permuted_unique_values, value_counts)
+
     return permuted_array
 
 
 def permutation_matrix_within_subject_across_sessions(Nperm, D_t, idx_array):
     """
     Generates permutation matrix of within-session across-session data based on given indices.
 
     Parameters:
     --------------
-        Nperm (int): The number of permutations.
-        D_t (numpy.ndarray): The preprocessed data array.
-        idx_array (numpy.ndarray): The indices array.
+    Nperm (int): The number of permutations.
+    D_t (numpy.ndarray): The preprocessed data array.
+    idx_array (numpy.ndarray): The indices array.
 
 
     Returns:
     ----------  
-        permutation_matrix (numpy.ndarray): The within-session continuos indices array.
+    permutation_matrix (numpy.ndarray): The within-session continuos indices array.
     """
     permutation_matrix = np.zeros((D_t.shape[0],Nperm), dtype=int)
     for perm in range(Nperm):
         if perm == 0:
             permutation_matrix[:,perm] = np.arange(D_t.shape[0])
         else:
             idx_array_perm = permute_subject_trial_idx(idx_array)
@@ -1321,15 +1342,15 @@
 
     Returns:
         vpath_array(numpy.ndarray): A 1D array containing the column indices of the non-zero elements.
                                     If the input array is already 1D, it returns a copy of the input array.
 
     """
     if np.ndim(vpath) == 2:
-        vpath_array = np.argmax(vpath, axis=1) + 1
+        vpath_array = np.nonzero(vpath)[1] + 1
     else:
         # Then it is already a vector
         vpath_array = vpath.copy()
 
     return vpath_array
 
 def surrogate_state_time(perm, viterbi_path,n_states):
@@ -1528,15 +1549,15 @@
     ----------  
         test_statistics (numpy.ndarray): Updated test_statistics array.
         pval_perms (numpy.ndarray): Updated pval_perms array.
     """
     if method == 'regression':
         if category_columns["t_test_cols"]==[] and category_columns["f_test_cols"]==[]:
             if np.sum(np.isnan(Rin))>0:
-                if test_combination in [True, "columns"]:
+                if test_combination in [True, "across_columns"]:
                     # Calculate F-statitics with no NaN values.
                     F_statistic =calculate_nan_regression_f_test(Din, Rin, proj, nan_values=True)
                      # Calculate the degrees of freedom for the model and residuals
                     df_model = Din.shape[1]  # Number of predictors including intercept
                     df_resid = Din.shape[0] - df_model
                     p_value = 1 - f.cdf(F_statistic, df_model, df_resid)
                     # Get the base statistics and store p-values as z-scores to the test statistic
@@ -1552,15 +1573,15 @@
                 # Calculate the predicted values
                 predicted_values = Din @ beta
                 # Calculate the residual sum of squares (rss)
                 rss = np.sum((predicted_values - Rin)**2, axis=0)
                 # Calculate the total sum of squares (tss)
                 tss = np.sum((Rin - np.nanmean(Rin, axis=0))**2, axis=0)
                 
-                if test_combination in [True, "columns"]:
+                if test_combination in [True, "across_columns"]:
                     # Calculate the parametric p-values using F-statistics
                     # Calculate the explained sum of squares (ESS)
                     ess = tss - rss
                     # Calculate the degrees of freedom for the model and residuals
                     df_model = Din.shape[1]  # Number of predictors including intercept
                     df_resid = Din.shape[0] - df_model
                     # Calculate the mean squared error (MSE) for the model and residuals
@@ -1575,15 +1596,15 @@
                 else:
                     # Calculate R^2
                     base_statistics = 1 - (rss / tss) #r_squared
                     # Store the R^2 values in the test_statistics array
                     test_statistics[perm] = base_statistics
         else:
             # If we are doing test_combinations, we need to calculate f-statistics on every column
-            if test_combination in [True, "columns"]:
+            if test_combination in [True, "across_columns"]:
                 if np.sum(np.isnan(Rin))>0:
                     # Calculate the explained variance if R got NaN values.
                     F_statistic =calculate_nan_regression_f_test(Din, Rin, proj, nan_values=True)
                 else:
                     # Calculate F-statitics with no NaN values.
                     F_statistic =calculate_nan_regression_f_test(Din, Rin, proj, nan_values=False)
                      # Calculate the degrees of freedom for the model and residuals
@@ -1630,24 +1651,24 @@
     # Calculate for univariate tests              
     elif method == "univariate":
         if category_columns["t_test_cols"]==[] and category_columns["f_test_cols"]==[]:
             # Only calcuating the correlation matrix, since there is no need for t- or f-test
             if np.sum(np.isnan(Din))>0 or np.sum(np.isnan(Rin))>0:
                 # Calculate the correlation matrix while handling NaN values 
                 # column by column without removing entire rows.
-                if test_combination in [True, "columns", "rows"]: 
+                if test_combination in [True, "across_columns", "across_rows"]: 
                     # Return parametric p-values
                     _,base_statistics =calculate_nan_correlation_matrix(Din, Rin, test_combination, reduce_pval_dims=True)
                     test_statistics[perm, :] = base_statistics # Notice that shape of test_statistics are different
                 else:
                     # Return correlation coefficients instead of p-values
                     base_statistics,_ =calculate_nan_correlation_matrix(Din, Rin)
                     test_statistics[perm, :, :] = np.abs(base_statistics)
             else:
-                if test_combination in [True, "columns", "rows"]: 
+                if test_combination in [True, "across_columns", "across_rows"]: 
                     # Return parametric p-values
                     pval_matrix = np.zeros((Din.shape[1],Rin.shape[1]))
                     for i in range(Din.shape[1]):
                         for j in range(Rin.shape[1]):
                             _, pval_matrix[i, j] = pearsonr(Din[:, i], Rin[:, j])
                     base_statistics =calculate_geometric_pval(pval_matrix, test_combination) 
                     test_statistics[perm,:]=abs(base_statistics)         
@@ -1669,76 +1690,76 @@
                         # Get the t-statistic if when NaN values are detected
                         t_test, pval =calculate_nan_t_test(Din, Rin[:, col], nan_values=True)
                     else:
                         # Get the t-statistic if there are no NaN values
                         t_test, pval = calculate_nan_t_test(Din, Rin[:, col], nan_values=False)
                         
                     # Put values inside test_statistics    
-                    if test_combination in [True, "columns", "rows"]:
+                    if test_combination in [True, "across_columns", "across_rows"]:
                         # Save to pval_statistics_com
                         pval_statistics_com[:, col] = pval
                     else:
                         # Save directly to test_statistics
                         test_statistics[perm, :, col] = np.abs(t_test)
                     # save t-test to base_statistics
                     if perm==0:
-                        if test_combination in [True, "columns", "rows"]:
+                        if test_combination in [True, "across_columns", "across_rows"]:
                             # Convert pval to z-score
                             #base_statistics_com[:,col] = norm.ppf(1 - np.array(np.squeeze(pval)))
                             base_statistics_com[:,col] = np.squeeze(pval)
                         else:
                             base_statistics[:,col]= t_test 
                 elif category_columns["f_test_cols"] and col in category_columns["f_test_cols"]:
                     if np.sum(np.isnan(Din))>0 or np.sum(np.isnan(Rin))>0:
                         # Perform f-test while accounting for NaNs
                         f_test, pval =calculate_nan_f_test(Din, Rin[:, col], nan_values=True)
                     else:    
                         # Perform f-statistics
                         f_test, pval =calculate_nan_f_test(Din, Rin[:, col], nan_values=False)
                     # Put values inside test_statistics    
-                    if test_combination in [True, "columns", "rows"]:
+                    if test_combination in [True, "across_columns", "across_rows"]:
                         pval_statistics_com[:, col] = pval
                     else:
                         test_statistics[perm, :, col] = np.abs(f_test)
                     # Insert base statistics
                     if perm==0:
-                        if test_combination in [True, "columns", "rows"]:
+                        if test_combination in [True, "across_columns", "across_rows"]:
                             # Convert pval to z-score
                             #base_statistics_com[:,col] = norm.ppf(1 - np.array(np.squeeze(pval)))
                             base_statistics_com[:,col] = np.squeeze(pval)
                         else:
                             base_statistics[:,col]= f_test                  
                 else:
                     # Perform corrrelation analysis
                     if np.sum(np.isnan(Din))>0 or np.sum(np.isnan(Rin))>0:
                         # Calculate the correlation matrix while handling NaN values 
                         # column by column without removing entire rows.
                         corr_array, pval =calculate_nan_correlation_matrix(Din, Rin[:, col], test_combination)
                     else:
                         # calculate correlation and pval between Din and Rin if there are no NaN values
                         #corr_array, pval= pearsonr(Din, np.expand_dims(Rin[:, col],axis=1))
-                        if test_combination in [True, "columns", "rows"]:
+                        if test_combination in [True, "across_columns", "across_rows"]:
                             
                             pval = np.zeros((Din.shape[-1],1)) 
                             # Have to make a loop between each columns to get the p-values
                             for i in range(Din.shape[1]):
                                 _, pval[i] = pearsonr(Din[:, i], Rin[:, col])
                         else:
                             #Calculate correlation coefficient matrix - Faster calculation
                             corr_coef = np.corrcoef(Din, Rin[:, col], rowvar=False)
                             # get the correlation matrix
                             corr_array = np.squeeze(corr_coef[:Din.shape[1], Din.shape[1]:])
                             # Update test_statistics
-                    if test_combination in [True, "columns", "rows"]:
+                    if test_combination in [True, "across_columns", "across_rows"]:
                         pval_statistics_com[:, col] = np.squeeze(pval)
                     else:
                         test_statistics[perm, :, col] = np.abs(np.squeeze(corr_array))       
                     # Insert base statistics
                     if perm==0:
-                        if test_combination in [True, "columns", "rows"]:
+                        if test_combination in [True, "across_columns", "across_rows"]:
                             # Convert pval to z-score
                             #base_statistics_com[:,col] = norm.ppf(1 - np.array(np.squeeze(pval)))
                             base_statistics_com[:,col] = np.squeeze(pval)
                         else:
                             base_statistics[:,col]= np.squeeze(corr_array)      
             if test_combination!=False:
                 base_statistics = calculate_geometric_pval(base_statistics_com, test_combination) if perm==0 else base_statistics_com
@@ -1764,27 +1785,27 @@
     """
     Calculate test statistics of z-scores converted from p-values based on the specified combination.
 
     Parameters:
     --------------
         p_values (numpy.ndarray):  Matrix of p-values.
         test_combination (str):       Specifies the combination method.
-                                      Valid options: "True", "columns", "rows".
+                                      Valid options: "True", "across_columns", "across_rows".
                                       Default is "True".
 
     Returns:
     ----------  
         result (numpy.ndarray):       Test statistics of z-scores converted from p-values.
     """
     if test_combination == True:
         pval = np.squeeze(np.exp(np.mean(np.log(p_values))))
         z_scores = norm.ppf(1 - np.array(pval))
         test_statistics = z_scores
-    elif test_combination == "columns" or test_combination == "rows":
-        axis = 0 if test_combination == "columns" else 1
+    elif test_combination == "across_columns" or test_combination == "across_rows":
+        axis = 0 if test_combination == "across_columns" else 1
         pval = np.squeeze(np.exp(np.mean(np.log(p_values), axis=axis)))
         z_scores = norm.ppf(1 - np.array(pval))
         test_statistics = z_scores
     else:
         raise ValueError("Invalid value for test_combination parameter")
 
     return test_statistics
@@ -1968,65 +1989,171 @@
             
     # Convert z-map to p-values
     p_values = 1 - norm.cdf(pval_zmap)
     p_values[p_values == 0.5] = 1
     return p_values
 
 
-def get_timestamp_indices(n_timestamps, n_subjects):
+def get_indices_timestamp(n_timestamps, n_subjects):
     """
     Generate indices of the timestamps for each subject in the data.
 
     Parameters:
     --------------
         n_timestamps (int): Number of timestamps.
         n_subjects (int): Number of subjects.
 
     Returns:
     ----------  
         indices (ndarray): NumPy array representing the indices of the timestamps for each subject.
 
     Example:
-    get_timestamp_indices(5, 3)
+    get_indices_timestamp(5, 3)
     array([[ 0,  5],
            [ 5, 10],
            [10, 15]])
     """
     indices = np.column_stack([np.arange(0, n_timestamps * n_subjects, n_timestamps),
                                np.arange(0 + n_timestamps, n_timestamps * n_subjects + n_timestamps, n_timestamps)])
 
     return indices
 
+def get_indices_session(data_label):
+    """
+    Generate session indices in the data based on provided labels.
+    This is done by using 'data_label' to define sessions and generates corresponding indices. 
+    The resulting 'idx_data_sessions' array represents the intervals for each session in the data.
+    
+    Parameters:
+    --------------
+        data_label (ndarray): NumPy array representing the labels for data to be indexed into sessions.
 
-def get_concatenate_sessions(D_sessions, R_sessions, idx_sessions):
+    Returns:
+    ----------  
+        idx_data_sessions (ndarray): The indices of datapoints within each session. It should be a 2D array 
+                            where each row represents the start and end index for a trial. 
+
+    Example:
+    get_indices_session(np.array([1, 1, 2, 2, 2, 3, 3, 3, 3]))
+    array([[0, 2],
+           [2, 5],
+           [5, 9]])
+    """
+    # Get unique labels from the data_label array
+    unique_labels = np.unique(data_label)
+
+    # Initialize an array to store session indices
+    idx_data_sessions  = np.zeros((len(unique_labels), 2)).astype(int)
+
+    # Iterate over unique labels
+    for session in range(len(unique_labels)):
+        # Count occurrences of the current label in the data_label array
+        occurrences = len(data_label[data_label == unique_labels[session]])
+
+        # Update the session indices array
+        if session == 0:
+            idx_data_sessions [session, 1] = occurrences
+        else:
+            idx_data_sessions [session, 0] = idx_data_sessions [session - 1, 1]
+            idx_data_sessions [session, 1] = idx_data_sessions [session - 1, 1] + occurrences
+
+    # Return the generated session indices array
+    return idx_data_sessions 
+
+def get_indices_from_list(data_list, count_timestamps = True):
     """
-    Converts a  3D matrix into a 2D matrix by concatenating timepoints of every trial session into a new design matrix.
+    Generate indices representing the start and end timestamps for each subject or session from a given data list.
 
+    Parameters:
+    --------------
+        data_list (list): List containing data for each subject or session.
+        count_timestamps (bool): If True, counts timestamps for each element in data_list, otherwise assumes each element in data_list is already a count of timestamps.
+
+    Returns:
+    ----------  
+        indices (ndarray): NumPy array with start and end indices for each subject's timestamps.
+
+    """
+    # Initialize an empty NumPy array to store start and end indices for each subject
+    indices = np.zeros((len(data_list), 2), dtype=int)
+    
+    # Iterate through each element in the data list along with its index
+    for i, data in enumerate(data_list):
+        if count_timestamps:
+            # Get the number of timestamps for the current subject or session
+            n_timestamps = len(data)
+        else: 
+            n_timestamps = data 
+        
+        # Update indices based on whether it's the first subject or subsequent ones
+        if i == 0:
+            indices[i, 1] = n_timestamps  # For the first subject, set the end index
+        else:
+            indices[i, 0] = indices[i - 1, 1]  # Set the start index based on the previous subject's end index
+            indices[i, 1] = indices[i - 1, 1] + n_timestamps  # Set the end index
+        
+    # Return the generated indices array
+    return indices
+
+def get_concatenate_subjects(D_sessions):
+    """
+    Converts a  3D matrix into a 2D matrix by concatenating timepoints of every subject into a new design matrix.
 
     Parameters:
     --------------
-        D_sessions (numpy.ndarray): Design matrix for each session.
-        R_sessions (numpy.ndarray): R  matrix time for each trial.
-        idx_sessions (numpy.ndarray): Indices representing the start and end of trials for each session.
+        D_sessions (numpy.ndarray): Design matrix for each subject.
 
     Returns:
     ----------  
         D_con (numpy.ndarray): Concatenated design matrix.
-        R_con (numpy.ndarray): Concatenated R matrix.
-        idx_sessions_con (numpy.ndarray): Updated indices after concatenation.
+
     """
+    D_con = []
+
+    for i in range(D_sessions.shape[1]):
+        # Extend data matrix with selected trials
+        D_con.extend(D_sessions[:, i, :])
+
+    return np.array(D_con)
+
+def get_concatenate_sessions(D_sessions, R_sessions=None, idx_sessions=None):
+    """
+    Converts a  3D matrix into a 2D matrix by concatenating timepoints of every trial session into a new design matrix.
+
+    Parameters:
+    --------------
+    D_sessions (numpy.ndarray): 
+        Design matrix for each session.
+    R_sessions (numpy.ndarray): 
+        R  matrix time for each trial.
+    idx_sessions (numpy.ndarray): 
+        Indices representing the start and end of trials for each session.
+
+    Returns:
+    ----------  
+    D_con (numpy.ndarray): 
+        Concatenated design matrix.
+    R_con (numpy.ndarray): 
+        Concatenated R matrix.
+    idx_sessions_con (numpy.ndarray): 
+        Updated indices after concatenation.
+    """
+    if idx_sessions is None:
+        raise ValueError("idx_sessions cannot be None")
     D_con, R_con, idx_sessions_con = [], [], np.zeros_like(idx_sessions)
 
     for i, (start_idx, end_idx) in enumerate(idx_sessions):
         # Iterate over trials in each session
         for j in range(start_idx, end_idx):
             # Extend data matrix with selected trials
             D_con.extend(D_sessions[:, j, :])
-            # Extend time list for each trial
-            R_con.extend([R_sessions[j]] * D_sessions.shape[0])
+            if R_sessions is not None:
+                # Extend time list for each trial
+                R_con.extend([R_sessions[j]] * D_sessions.shape[0])
+
 
         # Update end index for the concatenated data matrix
         idx_sessions_con[i, 1] = len(D_con)
 
         if i < len(idx_sessions) - 1:
             # Update start index for the next session if not the last iteration
             idx_sessions_con[i + 1, 0] = idx_sessions_con[i, 1]
@@ -2037,23 +2164,29 @@
 
 def reconstruct_concatenated_design(D_con,D_sessions=None, n_timepoints=None, n_trials=None, n_channels = None):
     """
     Reconstructs the concatenated design matrix to the original session variables.
 
     Parameters:
     --------------
-        D_con (numpy.ndarray): Concatenated design matrix.
-        D_sessions (numpy.ndarray, optional): Original design matrix for each session.
-        n_timepoints (int, optional): Number of timepoints per trial.
-        n_trials (int, optional): Number of trials per session.
-        n_channels (int, optional): Number of channels.
+    D_con (numpy.ndarray): 
+        Concatenated design matrix.
+    D_sessions (numpy.ndarray, optional): 
+        Original design matrix for each session.
+    n_timepoints (int, optional): 
+        Number of timepoints per trial.
+    n_trials (int, optional): 
+        Number of trials per session.
+    n_channels (int, optional): 
+        Number of channels.
 
     Returns:
     ----------  
-        D_reconstruct (numpy.ndarray): Reconstructed design matrix for each session.
+    D_reconstruct (numpy.ndarray): 
+        Reconstructed design matrix for each session.
     """
     # Input validation and initialization
     if D_sessions is not None and len([arg for arg in [n_timepoints, n_trials, n_channels] if arg is not None]) == 0:
         if not isinstance(D_sessions, np.ndarray) or D_sessions.ndim != 3:
             raise ValueError("Invalid input: D_sessions must be a 3D numpy array.")
         n_timepoints, n_trials, n_channels = D_sessions.shape
         D_reconstruct = np.zeros_like(D_sessions)
@@ -2276,36 +2409,36 @@
     for i in range(p):
         D_column = D_data[:, i]
         for j in range(q):
             # Do it column by column if R_data got more than 1 column
             R_column = R_data[:, j] if R_data.ndim>1 else R_data
             # If there are no variability between variables then set the value to NaN
             if np.all(D_column == D_column[0]) or np.all(R_column == R_column[0]):
-                if test_combination in [True, "columns", "rows"]:
+                if test_combination in [True, "across_columns", "across_rows"]:
                    pval_matrix[i, j]  = np.nan 
                 else:
                     correlation_matrix[i, j] = np.nan  
             else:
                 # Find non-NaN indices for both D_column and R_column
                 valid_indices = ~np.isnan(D_column) & ~np.isnan(R_column)           
-                if test_combination in [True, "columns", "rows"]:
+                if test_combination in [True, "across_columns", "across_rows"]:
                     #pval_matrix = np.zeros(corr_matrix.shape)
                     _, pval= pearsonr(D_column[valid_indices], R_column[valid_indices])
                     pval_matrix[i, j]  = pval
                 else:
                     # Calculate correlation coefficient matrix
                     corr_coef = np.corrcoef(D_column[valid_indices], R_column[valid_indices], rowvar=False)
                     # get the correlation matrix
                     correlation_matrix[i, j] = corr_coef[0, 1] 
     if reduce_pval_dims:
         if test_combination== True:
             pval_combination=np.squeeze(np.exp(np.nanmean(np.log(pval_matrix))))
-        elif test_combination== "columns":
+        elif test_combination== "across_columns":
             pval_combination=np.squeeze(np.exp(np.nanmean(np.log(pval_matrix), axis=0)))
-        elif test_combination== "rows":
+        elif test_combination== "across_rows":
             pval_combination = np.squeeze(np.exp(np.nanmean(np.log(pval_matrix), axis=1)))
     else:
         # No pval combination has been performed, this is done if we only calculate the p-values columnwise
         pval_combination = pval_matrix.copy()
         
     return correlation_matrix, pval_combination
```

### Comparing `glhmm-0.2.3/glhmm/utils.py` & `glhmm-0.2.4/glhmm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Some public useful functions - Gaussian Linear Hidden Markov Model
 @author: Diego Vidaurre 2023
 """
 
 import numpy as np
 import statistics
 import math
+from scipy.optimize import linear_sum_assignment
 
 def get_FO(Gamma,indices,summation=False):
     """Calculates the fractional occupancy of each state.
     
     Parameters:
     -----------
     Gamma : array-like, shape (n_samples, n_states)
@@ -312,8 +313,55 @@
     for t in range(T):
         for k in range(K):
             if ser[t,k] == 0: continue
             entropy[t] -= math.log(ser[t,k]) * ser[t,k]
     return entropy
 
 
+def get_gamma_similarity(gamma1, gamma2):
+    """Computes a measure of similarity between two sets of state time courses.
+
+    These can have different numbers of states, but they must have the same
+    number of time points.
+
+    Parameters:
+    -----------
+    gamma1 : numpy.ndarray
+        First set of state time courses with shape (T, K).
+    gamma2 : numpy.ndarray
+        Second set of state time courses with shape (T, K2), where K2 may be different from K.
+
+    Returns:
+    --------
+    S : float
+        Similarity, measured as the sum of joint probabilities under the optimal state alignment.
+    assig : numpy.ndarray
+        Optimal state alignment for gamma2 (uses Munkres' algorithm).
+    gamma2 : numpy.ndarray
+        The second set of state time courses reordered to match gamma1.
+    """
+    
+    T, K = gamma1.shape
+    gamma1_0 = gamma1.copy()   
+    g = gamma2
+    K2 = g.shape[1]
+    
+    if K < K2:
+        gamma1 = np.hstack((gamma1_0, np.zeros((T, K2 - K))))
+        K = K2
+    elif K > K2:
+        g = np.hstack((g, np.zeros((T, K - K2))))
+    
+    M = np.zeros((K, K))  # cost
+    
+    for k1 in range(K):
+        for k2 in range(K):
+            M[k1, k2] += (T - np.sum(np.minimum(gamma1[:, k1], g[:, k2]))) / T
+    
+    row_ind, col_ind = linear_sum_assignment(M)
+    S = K - M[row_ind, col_ind].sum()
+    
+    gamma2 = g[:, col_ind]
+    
+    return S, col_ind, gamma2
+
```

### Comparing `glhmm-0.2.3/glhmm.egg-info/PKG-INFO` & `glhmm-0.2.4/glhmm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhmm
-Version: 0.2.3
+Version: 0.2.4
 Summary: Gaussian Linear Hidden Markov Model
 Home-page: https://github.com/vidaurre/glhmm
 Author: Diego Vidaurre
 Author-email: Diego Vidaurre <dvidaurre@cfin.au.dk>
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
@@ -16,11 +16,11 @@
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: igraph
 Requires-Dist: tqdm
 Requires-Dist: scikit-image
 Requires-Dist: statsmodels
 Provides-Extra: doc
-Requires-Dist: sphinx~=4.2.0; extra == "doc"
+Requires-Dist: sphinx>=5.0; extra == "doc"
 Requires-Dist: myst_parser; extra == "doc"
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
```

### Comparing `glhmm-0.2.3/setup.py` & `glhmm-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='glhmm',
-    version='0.2.3',
+    version='0.2.4',
     description='Gaussian Linear Hidden Markov Model',
     url='https://github.com/vidaurre/glhmm',
     author='Diego Vidaurre',
     author_email = "dvidaurre@cfin.au.dk",
     readme = "README.md",
     install_requires=['scipy','numpy','scikit-learn','matplotlib','numba','seaborn', 'pandas','igraph', 'tqdm', 'scikit-image','statsmodels'],
     packages=["glhmm"],
```

