# Comparing `tmp/scSpectra-0.1.0.tar.gz` & `tmp/scspectra-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scSpectra-0.1.0.tar", last modified: Fri Sep 22 13:08:56 2023, max compression
+gzip compressed data, was "scspectra-0.2.0.tar", max compression
```

## Comparing `scSpectra-0.1.0.tar` & `scspectra-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,16 @@
-drwxr-xr-x   0 krauset  (1714747262)  9696963        0 2023-09-22 13:08:56.255452 scSpectra-0.1.0/
--rw-r--r--   0 krauset  (1714747262)  9696963     1110 2023-09-21 13:05:21.000000 scSpectra-0.1.0/LICENSE.md
--rw-r--r--   0 krauset  (1714747262)  9696963       97 2023-09-21 13:08:30.000000 scSpectra-0.1.0/MANIFEST.in
--rw-r--r--   0 krauset  (1714747262)  9696963    10715 2023-09-22 13:08:56.255221 scSpectra-0.1.0/PKG-INFO
--rw-r--r--   0 krauset  (1714747262)  9696963    10341 2023-09-22 13:07:45.000000 scSpectra-0.1.0/README.md
-drwxr-xr-x   0 krauset  (1714747262)  9696963        0 2023-09-22 13:08:56.244213 scSpectra-0.1.0/Spectra/
--rw-r--r--   0 krauset  (1714747262)  9696963     7446 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/K_est.py
--rw-r--r--   0 krauset  (1714747262)  9696963    64615 2023-09-21 13:22:27.000000 scSpectra-0.1.0/Spectra/Spectra.py
--rw-r--r--   0 krauset  (1714747262)  9696963    52756 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/Spectra_attn.py
--rw-r--r--   0 krauset  (1714747262)  9696963    46264 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/Spectra_gpu.py
--rw-r--r--   0 krauset  (1714747262)  9696963    14232 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/Spectra_util.py
--rw-r--r--   0 krauset  (1714747262)  9696963      270 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/__init__.py
--rw-r--r--   0 krauset  (1714747262)  9696963     4446 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/attend.py
-drwxr-xr-x   0 krauset  (1714747262)  9696963        0 2023-09-22 13:08:56.244763 scSpectra-0.1.0/Spectra/data/
--rw-r--r--   0 krauset  (1714747262)  9696963    76894 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/data/default_gene_sets.json
--rw-r--r--   0 krauset  (1714747262)  9696963  6930953 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/data/sample_data.h5ad
--rw-r--r--   0 krauset  (1714747262)  9696963     1773 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/initialization.py
-drwxr-xr-x   0 krauset  (1714747262)  9696963        0 2023-09-22 13:08:56.254043 scSpectra-0.1.0/Spectra/load/
--rw-r--r--   0 krauset  (1714747262)  9696963        0 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/load/__init__.py
--rw-r--r--   0 krauset  (1714747262)  9696963      292 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/load/default_gene_sets.py
--rw-r--r--   0 krauset  (1714747262)  9696963      286 2023-09-21 13:05:21.000000 scSpectra-0.1.0/Spectra/load/sample_data.py
--rw-r--r--   0 krauset  (1714747262)  9696963        6 2023-09-22 13:08:02.000000 scSpectra-0.1.0/VERSION
-drwxr-xr-x   0 krauset  (1714747262)  9696963        0 2023-09-22 13:08:56.254977 scSpectra-0.1.0/scSpectra.egg-info/
--rw-r--r--   0 krauset  (1714747262)  9696963    10715 2023-09-22 13:08:56.000000 scSpectra-0.1.0/scSpectra.egg-info/PKG-INFO
--rw-r--r--   0 krauset  (1714747262)  9696963      537 2023-09-22 13:08:56.000000 scSpectra-0.1.0/scSpectra.egg-info/SOURCES.txt
--rw-r--r--   0 krauset  (1714747262)  9696963        1 2023-09-22 13:08:56.000000 scSpectra-0.1.0/scSpectra.egg-info/dependency_links.txt
--rw-r--r--   0 krauset  (1714747262)  9696963      113 2023-09-22 13:08:56.000000 scSpectra-0.1.0/scSpectra.egg-info/requires.txt
--rw-r--r--   0 krauset  (1714747262)  9696963        8 2023-09-22 13:08:56.000000 scSpectra-0.1.0/scSpectra.egg-info/top_level.txt
--rw-r--r--   0 krauset  (1714747262)  9696963       38 2023-09-22 13:08:56.255498 scSpectra-0.1.0/setup.cfg
--rw-r--r--   0 krauset  (1714747262)  9696963     1129 2023-09-22 13:06:55.000000 scSpectra-0.1.0/setup.py
+-rw-r--r--   0        0        0     1110 2023-09-11 21:17:22.831485 scspectra-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0      900 2024-04-09 16:04:08.682074 scspectra-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7367 2024-04-09 13:47:41.826214 scspectra-0.2.0/src/Spectra/K_est.py
+-rw-r--r--   0        0        0    68666 2024-04-09 13:47:17.839690 scspectra-0.2.0/src/Spectra/Spectra.py
+-rw-r--r--   0        0        0    56248 2024-04-09 13:47:42.115996 scspectra-0.2.0/src/Spectra/Spectra_attn.py
+-rw-r--r--   0        0        0    48665 2024-04-09 13:48:02.151211 scspectra-0.2.0/src/Spectra/Spectra_gpu.py
+-rw-r--r--   0        0        0    15200 2024-04-09 13:47:41.886037 scspectra-0.2.0/src/Spectra/Spectra_util.py
+-rw-r--r--   0        0        0      302 2024-04-09 16:02:33.951198 scspectra-0.2.0/src/Spectra/__init__.py
+-rw-r--r--   0        0        0     4333 2024-04-09 13:47:41.819590 scspectra-0.2.0/src/Spectra/attend.py
+-rw-r--r--   0        0        0    76894 2023-11-13 18:53:38.608470 scspectra-0.2.0/src/Spectra/data/default_gene_sets.json
+-rw-r--r--   0        0        0  6930953 2023-11-13 18:53:38.625885 scspectra-0.2.0/src/Spectra/data/sample_data.h5ad
+-rw-r--r--   0        0        0     1743 2024-04-09 13:47:41.803302 scspectra-0.2.0/src/Spectra/initialization.py
+-rw-r--r--   0        0        0        0 2023-11-13 19:29:41.214306 scspectra-0.2.0/src/Spectra/load/__init__.py
+-rw-r--r--   0        0        0      294 2024-04-09 13:47:41.799483 scspectra-0.2.0/src/Spectra/load/default_gene_sets.py
+-rw-r--r--   0        0        0      288 2024-04-09 13:47:41.798827 scspectra-0.2.0/src/Spectra/load/sample_data.py
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 scspectra-0.2.0/PKG-INFO
```

### Comparing `scSpectra-0.1.0/LICENSE.md` & `scspectra-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scSpectra-0.1.0/Spectra/K_est.py` & `scspectra-0.2.0/src/Spectra/K_est.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,227 +1,231 @@
 import numpy as np
 from opt_einsum import contract
-import scipy 
+import scipy
 from tqdm import tqdm
 
-class BEMA: 
-    """ 
+
+class BEMA:
+    """
     Performs bulk eigenvalue matching analysis.
     @Russell ZK
-    
-    [1] Algorithm 2 in : https://arxiv.org/abs/2006.00436 
-    
+
+    [1] Algorithm 2 in : https://arxiv.org/abs/2006.00436
+
     Parameters
     __________
     eigenvalues: np.ndarray, ascending order
         the ``(min(n,p),)``-shaped vector of eigenvalues. Must correspond to min(n,p)
-    B: int 
+    B: int
         the number of bootstrapped replicates for estimating the best fit null distribution; default is 10
-    M: int 
-        the number of bootstrapped replicates for determining the K estimation threshold; default is 100 
-    alpha: float 
-        the 
+    M: int
+        the number of bootstrapped replicates for determining the K estimation threshold; default is 100
+    alpha: float
+        the
     beta: float
-    
-    B: int 
-    
+
+    B: int
+
     Output
     __________
-    
-    BEMA.estimate_background(B) ; 
+
+    BEMA.estimate_background(B) ;
         stores gamma parameters self.theta and self.sigma_sq
-        returns None 
-    
-    BEMA.estimate_K(M) ; 
-        stores results of Monte Carlo simulations in a ``(min(n,p), M)``-shaped np.ndarray, sorted from 
-        smallest to largest eigenvalue. Can be used to check model fit 
-        
-        
-        
-    
+        returns None
+
+    BEMA.estimate_K(M) ;
+        stores results of Monte Carlo simulations in a ``(min(n,p), M)``-shaped np.ndarray, sorted from
+        smallest to largest eigenvalue. Can be used to check model fit
+
+
+
+
     Examples
     _________
-    
-    Here we fit a ``(n,p)``-shaped dataset X with BEMA :: 
+
+    Here we fit a ``(n,p)``-shaped dataset X with BEMA ::
         # X a ``(n,p)``-shaped np.ndarray; get covariance matrix
         n = X.shape[0]
         p = X.shape[1]
         cov = X.T.dot(X)/n
-        
+
         # get eigenvalues of covariance matrix
         l,_=np.linalg.eigh(cov)
-        
+
         #initialize BEMA class
         model = BEMA(n, p, l)
         K = model.forward()
-    
-    
-    
+
+
+
     """
-    def __init__(self, n, p, eigenvalues, alpha = 0.2, beta = 0.1, M = 100, B = 10): 
-        #assert(min(n,p) == len(eigenvalues))
 
-        self.eigenvalues = np.array(sorted(eigenvalues))#cast to np.array and sort
+    def __init__(self, n, p, eigenvalues, alpha=0.2, beta=0.1, M=100, B=10):
+        # assert(min(n,p) == len(eigenvalues))
+
+        self.eigenvalues = np.array(sorted(eigenvalues))  # cast to np.array and sort
         self.p = p
-        self.n = n 
-        self.p_tilde = min(n,p)
-        self.gamma_n = p/n 
+        self.n = n
+        self.p_tilde = min(n, p)
+        self.gamma_n = p / n
         self.alpha = alpha
-        self.M = M 
+        self.M = M
         self.beta = beta
-        self.B = B 
-        self.eigenvalues = self.eigenvalues[-1*self.p_tilde:]
+        self.B = B
+        self.eigenvalues = self.eigenvalues[-1 * self.p_tilde :]
+
     def getQT(self, theta, B):
-        """ 
+        """
         getQT function gets the quantiles
         """
-        lambda_b = np.zeros((self.p_tilde,B)) #
-        
-        for b in range(B): 
-            cov = np.random.gamma(theta,1/theta,self.p)
-            Z = np.random.normal(size = (self.n,self.p))
-            Z_s = np.sqrt(cov).reshape(1,-1)*Z
+        lambda_b = np.zeros((self.p_tilde, B))  #
+
+        for b in range(B):
+            cov = np.random.gamma(theta, 1 / theta, self.p)
+            Z = np.random.normal(size=(self.n, self.p))
+            Z_s = np.sqrt(cov).reshape(1, -1) * Z
 
             # if n is larger than p, we compute the regular covariance matrix - otherwise for computational efficiency
             #       compute the n x n matrix with identical non-zero eigenvalues
             if self.n >= self.p:
-                S_b = 1/self.n * contract('ij,ik->jk', Z_s, Z_s)
+                S_b = 1 / self.n * contract("ij,ik->jk", Z_s, Z_s)
             else:
-                S_b = 1/self.n * contract('ji,ki->jk', Z_s, Z_s)
-            l_sim =np.linalg.eigvalsh(S_b)
-            
-            lambda_b[:,b] = l_sim 
-        
-        return lambda_b.mean(axis = 1)
-    
-    def est_sigma(self,theta,qt):
-        eigvals = self.eigenvalues[int(self.alpha*self.p_tilde):int((1-self.alpha)*self.p_tilde)]
-        qt = qt[int(self.alpha*self.p_tilde):int((1-self.alpha)*self.p_tilde)]
+                S_b = 1 / self.n * contract("ji,ki->jk", Z_s, Z_s)
+            l_sim = np.linalg.eigvalsh(S_b)
+
+            lambda_b[:, b] = l_sim
+
+        return lambda_b.mean(axis=1)
+
+    def est_sigma(self, theta, qt):
+        eigvals = self.eigenvalues[
+            int(self.alpha * self.p_tilde) : int((1 - self.alpha) * self.p_tilde)
+        ]
+        qt = qt[int(self.alpha * self.p_tilde) : int((1 - self.alpha) * self.p_tilde)]
         sigma_sq = np.dot(qt, eigvals) / np.dot(qt, qt)
         return sigma_sq
 
     def loss(self, theta, sigma_sq, qt):
-        eigvals = self.eigenvalues[int(self.alpha*self.p_tilde):int((1-self.alpha)*self.p_tilde)]
-        qt = qt[int(self.alpha*self.p_tilde):int((1-self.alpha)*self.p_tilde)]
-        loss_ = ((sigma_sq * qt - eigvals)**2).sum()
-        return loss_ 
+        eigvals = self.eigenvalues[
+            int(self.alpha * self.p_tilde) : int((1 - self.alpha) * self.p_tilde)
+        ]
+        qt = qt[int(self.alpha * self.p_tilde) : int((1 - self.alpha) * self.p_tilde)]
+        loss_ = ((sigma_sq * qt - eigvals) ** 2).sum()
+        return loss_
 
     def estimate_background(self, B):
-        bound = [0.1,6]
-        while bound[1] - bound[0] > 0.001: # todo: make these hyperparameters tunable
+        bound = [0.1, 6]
+        while bound[1] - bound[0] > 0.001:  # todo: make these hyperparameters tunable
             print("Minimization gap... ", bound[1] - bound[0])
             points = np.linspace(bound[0], bound[1], 4)
             losses = []
             for point in points:
                 qt = self.getQT(point, B)
-                sigma_sq = self.est_sigma(point,qt)
-                loss_ = self.loss(point,sigma_sq,qt)
+                sigma_sq = self.est_sigma(point, qt)
+                loss_ = self.loss(point, sigma_sq, qt)
                 losses.append(loss_)
 
             ind = np.argmin(losses)
-            if ind==0:
-                bound=[points[ind],points[ind+1]]
-            elif ind==3:
-                bound=[points[ind-1],points[ind]]
+            if ind == 0:
+                bound = [points[ind], points[ind + 1]]
+            elif ind == 3:
+                bound = [points[ind - 1], points[ind]]
             else:
-                bound=[points[ind-1],points[ind+1]]
+                bound = [points[ind - 1], points[ind + 1]]
 
         self.theta = points[ind]
         qt = self.getQT(self.theta, B)
         self.sigma_sq = self.est_sigma(self.theta, qt)
         return
 
-    
     def estimate_K(self, M):
         """
-        Runs step 2 of the algorithm - estimating K 
+        Runs step 2 of the algorithm - estimating K
         """
-        #store entire results matrix
-        res_matrix = np.zeros((self.p_tilde,M)) 
+        # store entire results matrix
+        res_matrix = np.zeros((self.p_tilde, M))
         for m in tqdm(range(M)):
-            d = np.random.gamma(self.theta,1/self.theta, self.p) 
-            Z = np.random.normal(size = (self.n,self.p))
-            Z_s = np.sqrt(d*self.sigma_sq).reshape(1,-1)*Z
-            
+            d = np.random.gamma(self.theta, 1 / self.theta, self.p)
+            Z = np.random.normal(size=(self.n, self.p))
+            Z_s = np.sqrt(d * self.sigma_sq).reshape(1, -1) * Z
+
             if self.n >= self.p:
-                S_b = 1/self.n * contract('ij,ik->jk', Z_s, Z_s)
+                S_b = 1 / self.n * contract("ij,ik->jk", Z_s, Z_s)
             else:
-                S_b = 1/self.n * contract('ji,ki->jk', Z_s, Z_s)
-            l_sim =np.linalg.eigvalsh(S_b)
-            res_matrix[:,m] = l_sim
-            
-        #update global parameters
+                S_b = 1 / self.n * contract("ji,ki->jk", Z_s, Z_s)
+            l_sim = np.linalg.eigvalsh(S_b)
+            res_matrix[:, m] = l_sim
+
+        # update global parameters
         self.res_matrix = res_matrix
-        self.threshold = np.array(sorted(res_matrix[-1,:]))[int((1-self.beta)*M)] 
+        self.threshold = np.array(sorted(res_matrix[-1, :]))[int((1 - self.beta) * M)]
         return sum(self.eigenvalues > self.threshold)
 
     def forward(self):
         print("Step 1; estimating best fit null distribution... ")
         self.estimate_background(self.B)
         print("Step 2; estimating K...")
         return self.estimate_K(self.M)
-    
+
     def confidence_interval(self, m_0):
-        upper = self.res_matrix[-1,int((1-m_0/2)*self.M)]
-        lower = self.res_matrix[-1,int((m_0/2)*self.M)]
-        return (sum(self.eigenvalues > lower),sum(self.eigenvalues > upper))
+        upper = self.res_matrix[-1, int((1 - m_0 / 2) * self.M)]
+        lower = self.res_matrix[-1, int((m_0 / 2) * self.M)]
+        return (sum(self.eigenvalues > lower), sum(self.eigenvalues > upper))
 
 
-def estimate_L(adata, attribute, highly_variable = False, **kwargs):
-    """ 
+def estimate_L(adata, attribute, highly_variable=False, **kwargs):
+    """
 
     Parameters
     ----------
     adata : sc.AnnData object
 
     attribute : must be column of adata.obs
-    
+
     highly_variable : if True, only uses adata.var.highly_variable to generate eigenvalues
-    
+
     **kwargs: arguments for BEMA class
-    
-    """ 
-    
+
+    """
+
     L_dict = {}
     cell_types = np.unique(adata.obs[attribute])
     init_Ls = np.zeros(len(cell_types) + 1)
     if highly_variable:
         X = adata.X[:, adata.var.highly_variable]
     else:
         X = adata.X
     if type(X) == scipy.sparse.csr.csr_matrix:
         X = np.array(X.todense())
-    
-    data = X - X.mean(axis=0, keepdims = True)
-    sample_cov = contract('ij,ik->jk',data,data)/data.shape[0]
+
+    data = X - X.mean(axis=0, keepdims=True)
+    sample_cov = contract("ij,ik->jk", data, data) / data.shape[0]
     l = np.linalg.eigvalsh(sample_cov)
-    
-    model = BEMA(n = data.shape[0], p = data.shape[1], eigenvalues = l, **kwargs)
+
+    model = BEMA(n=data.shape[0], p=data.shape[1], eigenvalues=l, **kwargs)
     K = model.forward()
 
-    init_Ls[0] = K 
-    
+    init_Ls[0] = K
+
     ct = 1
     for cell_type in cell_types:
         data_ct = data[adata.obs[attribute] == cell_type]
-        sample_cov = contract('ij,ik->jk',data_ct,data_ct)/data_ct.shape[0]
+        sample_cov = contract("ij,ik->jk", data_ct, data_ct) / data_ct.shape[0]
         l = np.linalg.eigvalsh(sample_cov)
-        model = BEMA(n = data_ct.shape[0], p = data_ct.shape[1], eigenvalues = l, **kwargs)
+        model = BEMA(n=data_ct.shape[0], p=data_ct.shape[1], eigenvalues=l, **kwargs)
         K_out = model.forward()
         init_Ls[ct] = K_out
-        ct += 1 
-        
+        ct += 1
+
     """ 
     L_dict["global"] = (sum(init_Ls[1:]) - init_Ls[0])/(len(cell_types) - 1)
     ct = 1
     for cell_type in cell_types:
         L_dict[cell_type] = init_Ls[ct] - L_dict["global"] 
         ct += 1 
-    """ 
+    """
     L_dict["global"] = int(init_Ls[0] + 1)
     ct = 1
     for cell_type in cell_types:
         L_dict[cell_type] = int(init_Ls[ct] + 1)
-        ct +=1
+        ct += 1
     return L_dict
-    
-
```

### Comparing `scSpectra-0.1.0/Spectra/Spectra.py` & `scspectra-0.2.0/src/Spectra/Spectra.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,962 +1,1194 @@
-import numpy as np 
+import numpy as np
 import torch
-from collections import OrderedDict 
+from collections import OrderedDict
 from opt_einsum import contract
 from scipy.special import logit
-from tqdm import tqdm 
+from tqdm import tqdm
 from scipy.special import xlogy
 from scipy.special import softmax
-from Spectra import Spectra_util 
+from Spectra import Spectra_util
 import torch.nn as nn
 import scipy
 import pandas as pd
 from pyvis.network import Network
 import random
 
 from torch.distributions.normal import Normal
 from torch.distributions.log_normal import LogNormal
 from torch.distributions.dirichlet import Dirichlet
 
-### Class for SPECTRA model 
-from Spectra.initialization import * 
+### Class for SPECTRA model
+from Spectra.initialization import *
+
+
+class SPECTRA(nn.Module):
+    """
 
-class SPECTRA(nn.Module): 
-    """ 
-    
     Parameters
         ----------
         X : np.ndarray or torch.Tensor
             the ``(n, p)`` -shaped matrix containing logged expression count data. Used for initialization of self.n and self.p but not stored as an attribute
         labels : np.ndarray or NoneType
             the ``(n, )`` -shaped array containing cell type labels. If use_cell_types == False, then should be set to None
-        
+
         L : dict or OrderedDict [if use_cell_types == False, then int]
             ``number of cell types + 1``-shaped dictionary. Must have "global" as a key, indicating the number of global factors
             {
-                "global": 15, 
-                "CD8": 5 
-                ...    
+                "global": 15,
+                "CD8": 5
+                ...
             }
-            > Format matches output of K_est.py to estimate the number of 
+            > Format matches output of K_est.py to estimate the number of
             > Must match cell type labels provided during training
-            > Recommended practice is to assign at minimum 2 factors per cell type 
+            > Recommended practice is to assign at minimum 2 factors per cell type
             > Note that L contains the number of factors that describe the graph.
         adj_matrix :  dict or OrderedDict
-            ``a dictionary of adjacency matrices, one for every cell type + a "global" 
+            ``a dictionary of adjacency matrices, one for every cell type + a "global"
             {
                 "global": ``(p, p)``-shaped binary np.ndarray
-                "CD8": ... 
+                "CD8": ...
 
-            } 
+            }
         weights : dict or OrderedDict or NoneType [if use_cell_types == False, then ``(p, p)``-shaped array]
             the ``(p, p)``-shaped set of edge weights per . If weight[i,j] is non-zero when adj_matrix[i,j] = 0
-            this weight is ignored. 
-            
+            this weight is ignored.
+
             if weights == None, no weights are used
         lam : float
-            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information  
-        delta : float 
-            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes. 
+            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information
+        delta : float
+            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes.
         kappa : float or NoneType
-            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.  
+            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.
         rho : float or NoneType
-            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data. 
-        use_cell_types: bool 
+            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data.
+        use_cell_types: bool
             use_cell_types is a Boolean variable that determines whether cell type labels are used to fit the model. If False, then parameters are initialized as nn.Parameter rather than as nn.ParameterDict with cell type keys that index nn.Parameter values
         determinant_penalty : float
-            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.  
+            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.
     Attributes
         ----------
         model.delta : delta parameter of the model
 
-        model.lam : lambda parameter of the model 
-       
-        model.determinant_penalty : determinant penalty of the model 
- 
-        model.L : L parameter, either int, dict or OrderedDict() 
+        model.lam : lambda parameter of the model
+
+        model.determinant_penalty : determinant penalty of the model
+
+        model.L : L parameter, either int, dict or OrderedDict()
 
         model.p : number of genes
 
-        model.n : number of cells 
+        model.n : number of cells
 
-        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters. 
+        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters.
 
         model.kappa : if not kappa, nn.ParameterDict() if use_cell_types, else nn.Parameter(). If kappa is a float, it is fixed throughout training
 
         model.rho : if not rho, nn.ParamterDict() if use_cell_types, else nn.Parameter. If rho is a float it is fixed throughout training
 
-        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors 
+        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.weights : contains edge weights. format matches adj_matrix
 
-        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors 
-        
-        model.weights : contains edge weights. format matches adj_matrix 
-        
         model.cell_types : np.ndarray containing array of unique cell types
-       
+
         model.cell_type_counts : dict {key = cell type, values = number of cells}
- 
-        model.theta : nn.ParameterDict() or nn.Parameter() containing the factor weights 
+
+        model.theta : nn.ParameterDict() or nn.Parameter() containing the factor weights
 
         model.alpha : nn.ParameterDict() or nn.Parameter() containing the cell loadings
 
         model.eta : nn.ParameterDict() or nn.Parameter() containing the interaction matrix between factors
 
         model.gene_scaling : nn.ParameterDict() or nn.Parameter() containing the gene scale factors
 
-        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False 
-        
+        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False
+
         model.kgeql_flag : dict or bool. dictionary of boolean values indicating whether K >= L.  When use_cell_types == False, it is a boolean value
 
     Methods
         ----------
 
         model.loss(self, X, labels) : called by fit if use_cell_types = True. Evalutes the loss of the model
 
-        model.loss_no_cell_types(self,X) : called by fit if use_cell_types = False. Evalutes the loss of the model 
-     
+        model.loss_no_cell_types(self,X) : called by fit if use_cell_types = False. Evalutes the loss of the model
+
         model.initialize(self, gene_sets,val) : initialize the model based on given dictionary of gene sets. val is a float that determines the strength of the initialization.
- 
-        model.initialize_no_celltypes(self, gs_list, val) : initialize the model based on given list of gene sets. val is a float that determines the strength of the initialization. 
 
-        
-    To do: 
+        model.initialize_no_celltypes(self, gs_list, val) : initialize the model based on given list of gene sets. val is a float that determines the strength of the initialization.
+
+
+    To do:
         __________
 
-        > Alternative initialization functions 
+        > Alternative initialization functions
 
         > comment SPECTRA-EM code
-        
+
         > test lower bound constraint [see pyspade_global.py implementation]
 
         > Overlap threshold test statistic
 
-    
+
     """
-    def __init__(self, X, labels, adj_matrix, L, weights = None, lam = 0.01, delta = 0.001,kappa = None, rho = 0.001, use_cell_types = True):
-        super(SPECTRA, self).__init__()
 
+    def __init__(
+        self,
+        X,
+        labels,
+        adj_matrix,
+        L,
+        weights=None,
+        lam=0.01,
+        delta=0.001,
+        kappa=None,
+        rho=0.001,
+        use_cell_types=True,
+    ):
+        super(SPECTRA, self).__init__()
 
-        #hyperparameters
-        self.delta = delta 
-        self.lam = lam 
-        self.L = L 
-        #for memory efficiency we don't store X in the object attributes, but require X dimensions to be known at initialization
+        # hyperparameters
+        self.delta = delta
+        self.lam = lam
+        self.L = L
+        # for memory efficiency we don't store X in the object attributes, but require X dimensions to be known at initialization
         self.p = X.shape[1]
         self.n = X.shape[0]
-        self.use_cell_types = use_cell_types 
-        
-        
-        
+        self.use_cell_types = use_cell_types
 
         if not use_cell_types:
-            #check that L is an int
-            assert(isinstance(self.L, int))
+            # check that L is an int
+            assert isinstance(self.L, int)
 
             # trust the user to input a np.ndarray for adj_matrix
-            self.adj_matrix = torch.Tensor(adj_matrix) - torch.Tensor(np.diag(np.diag(adj_matrix)))
+            self.adj_matrix = torch.Tensor(adj_matrix) - torch.Tensor(
+                np.diag(np.diag(adj_matrix))
+            )
             adj_matrix_1m = 1.0 - adj_matrix
-            self.adj_matrix_1m = torch.Tensor(adj_matrix_1m - np.diag(np.diag(adj_matrix_1m)))
+            self.adj_matrix_1m = torch.Tensor(
+                adj_matrix_1m - np.diag(np.diag(adj_matrix_1m))
+            )
             if weights is not None:
-                self.weights = torch.Tensor(weights) - torch.Tensor(np.diag(np.diag(adj_matrix)))
+                self.weights = torch.Tensor(weights) - torch.Tensor(
+                    np.diag(np.diag(adj_matrix))
+                )
             else:
                 self.weights = self.adj_matrix
-            
-            self.theta = nn.Parameter(Normal(0.,1.).sample([self.p, self.L]))
-            self.alpha = nn.Parameter(Normal(0.,1.).sample([self.n, self.L]))
-            self.eta = nn.Parameter(Normal(0.,1.).sample([self.L, self.L]))
-            self.gene_scaling = nn.Parameter(Normal(0.,1.).sample([self.p]))
+
+            self.theta = nn.Parameter(Normal(0.0, 1.0).sample([self.p, self.L]))
+            self.alpha = nn.Parameter(Normal(0.0, 1.0).sample([self.n, self.L]))
+            self.eta = nn.Parameter(Normal(0.0, 1.0).sample([self.L, self.L]))
+            self.gene_scaling = nn.Parameter(Normal(0.0, 1.0).sample([self.p]))
 
             if kappa == None:
-                self.kappa = nn.Parameter(Normal(0.,1.).sample())
+                self.kappa = nn.Parameter(Normal(0.0, 1.0).sample())
             else:
-                self.kappa = torch.tensor(np.log(kappa/(1- kappa))) #
+                self.kappa = torch.tensor(np.log(kappa / (1 - kappa)))  #
             if rho == None:
-                self.rho = nn.Parameter(Normal(0.,1.).sample())
+                self.rho = nn.Parameter(Normal(0.0, 1.0).sample())
             else:
-                self.rho = torch.tensor(np.log(rho/(1-rho)))
-
+                self.rho = torch.tensor(np.log(rho / (1 - rho)))
 
         if use_cell_types:
-            #convert adjacency matrices to pytorch tensors to make optimization easier later
-            self.adj_matrix = {cell_type: torch.Tensor(adj_matrix[cell_type]) - torch.Tensor(np.diag(np.diag(adj_matrix[cell_type]))) if len(adj_matrix[cell_type]) > 0 else [] for cell_type in adj_matrix.keys()}
-            #for convenience store 1 - adjacency matrix elements [except on diagonal, where we store 0]
-            adj_matrix_1m = {cell_type: 1.0 - adj_matrix[cell_type] if len(adj_matrix[cell_type]) > 0 else [] for cell_type in adj_matrix.keys()} #one adj_matrix per cell type 
-            self.adj_matrix_1m = {cell_type: torch.Tensor(adj_matrix_1m[cell_type] - np.diag(np.diag(adj_matrix_1m[cell_type]))) if len(adj_matrix_1m[cell_type]) > 0 else [] for cell_type in adj_matrix_1m.keys()} #one adj_matrix per cell type 
-            
-            #if weights are provided, convert these to tensors, else set weights = to adjacency matrices
+            # convert adjacency matrices to pytorch tensors to make optimization easier later
+            self.adj_matrix = {
+                cell_type: (
+                    torch.Tensor(adj_matrix[cell_type])
+                    - torch.Tensor(np.diag(np.diag(adj_matrix[cell_type])))
+                    if len(adj_matrix[cell_type]) > 0
+                    else []
+                )
+                for cell_type in adj_matrix.keys()
+            }
+            # for convenience store 1 - adjacency matrix elements [except on diagonal, where we store 0]
+            adj_matrix_1m = {
+                cell_type: (
+                    1.0 - adj_matrix[cell_type]
+                    if len(adj_matrix[cell_type]) > 0
+                    else []
+                )
+                for cell_type in adj_matrix.keys()
+            }  # one adj_matrix per cell type
+            self.adj_matrix_1m = {
+                cell_type: (
+                    torch.Tensor(
+                        adj_matrix_1m[cell_type]
+                        - np.diag(np.diag(adj_matrix_1m[cell_type]))
+                    )
+                    if len(adj_matrix_1m[cell_type]) > 0
+                    else []
+                )
+                for cell_type in adj_matrix_1m.keys()
+            }  # one adj_matrix per cell type
+
+            # if weights are provided, convert these to tensors, else set weights = to adjacency matrices
             if weights:
-                self.weights = {cell_type: torch.Tensor(weights[cell_type]) - torch.Tensor(np.diag(np.diag(weights[cell_type]))) if len(weights[cell_type]) > 0 else [] for cell_type in weights.keys()}
+                self.weights = {
+                    cell_type: (
+                        torch.Tensor(weights[cell_type])
+                        - torch.Tensor(np.diag(np.diag(weights[cell_type])))
+                        if len(weights[cell_type]) > 0
+                        else []
+                    )
+                    for cell_type in weights.keys()
+                }
             else:
                 self.weights = self.adj_matrix
 
-            self.cell_types = np.unique(labels) #cell types are the unique labels, again require knowledge of labels at initialization but do not store them
-            
-            #store a dictionary containing the counts of each cell type
+            self.cell_types = np.unique(
+                labels
+            )  # cell types are the unique labels, again require knowledge of labels at initialization but do not store them
+
+            # store a dictionary containing the counts of each cell type
             self.cell_type_counts = {}
             for cell_type in self.cell_types:
                 n_c = sum(labels == cell_type)
-                self.cell_type_counts[cell_type] = n_c 
-            
-            #initialize parameters randomly, we use torch's ParameterDict() for storage for intuitive accessing cell type specific parameters
+                self.cell_type_counts[cell_type] = n_c
+
+            # initialize parameters randomly, we use torch's ParameterDict() for storage for intuitive accessing cell type specific parameters
             self.theta = nn.ParameterDict()
             self.alpha = nn.ParameterDict()
             self.eta = nn.ParameterDict()
             self.gene_scaling = nn.ParameterDict()
 
             if kappa == None:
                 self.kappa = nn.ParameterDict()
             if rho == None:
                 self.rho = nn.ParameterDict()
-            #initialize global params
-            self.theta["global"] = nn.Parameter(Normal(0.,1.).sample([self.p, self.L["global"]]))
-            self.eta["global"] = nn.Parameter(Normal(0.,1.).sample([self.L["global"], self.L["global"]]))
-            self.gene_scaling["global"] = nn.Parameter(Normal(0.,1.).sample([self.p]))
+            # initialize global params
+            self.theta["global"] = nn.Parameter(
+                Normal(0.0, 1.0).sample([self.p, self.L["global"]])
+            )
+            self.eta["global"] = nn.Parameter(
+                Normal(0.0, 1.0).sample([self.L["global"], self.L["global"]])
+            )
+            self.gene_scaling["global"] = nn.Parameter(
+                Normal(0.0, 1.0).sample([self.p])
+            )
             if kappa == None:
-                self.kappa["global"] = nn.Parameter(Normal(0.,1.).sample())
+                self.kappa["global"] = nn.Parameter(Normal(0.0, 1.0).sample())
             if rho == None:
-                self.rho["global"] = nn.Parameter(Normal(0.,1.).sample())
+                self.rho["global"] = nn.Parameter(Normal(0.0, 1.0).sample())
 
-            #initialize all cell type specific params
+            # initialize all cell type specific params
             for cell_type in self.cell_types:
-                self.theta[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.p,self.L[cell_type]]))
-                self.eta[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.L[cell_type], self.L[cell_type]]))
+                self.theta[cell_type] = nn.Parameter(
+                    Normal(0.0, 1.0).sample([self.p, self.L[cell_type]])
+                )
+                self.eta[cell_type] = nn.Parameter(
+                    Normal(0.0, 1.0).sample([self.L[cell_type], self.L[cell_type]])
+                )
                 n_c = sum(labels == cell_type)
-                self.alpha[cell_type] = nn.Parameter(Normal(0.,1.).sample([n_c, self.L["global"] + self.L[cell_type]]))
-                self.gene_scaling[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.p]))
+                self.alpha[cell_type] = nn.Parameter(
+                    Normal(0.0, 1.0).sample([n_c, self.L["global"] + self.L[cell_type]])
+                )
+                self.gene_scaling[cell_type] = nn.Parameter(
+                    Normal(0.0, 1.0).sample([self.p])
+                )
 
                 if kappa == None:
-                    self.kappa[cell_type] = nn.Parameter(Normal(0.,1.).sample())
+                    self.kappa[cell_type] = nn.Parameter(Normal(0.0, 1.0).sample())
 
                 if rho == None:
-                    self.rho[cell_type] = nn.Parameter(Normal(0.,1.).sample())
+                    self.rho[cell_type] = nn.Parameter(Normal(0.0, 1.0).sample())
 
-    
-            #if kappa and rho are provided, hold these fixed during training, else fit as free parameters
+            # if kappa and rho are provided, hold these fixed during training, else fit as free parameters
             # to unify the cases, we put this in the same format
             if kappa != None:
                 self.kappa = {}
-                self.kappa["global"] = torch.tensor(np.log(kappa/(1-kappa)))
+                self.kappa["global"] = torch.tensor(np.log(kappa / (1 - kappa)))
                 for cell_type in self.cell_types:
-                    self.kappa[cell_type] = torch.tensor(np.log(kappa /(1-kappa)))
+                    self.kappa[cell_type] = torch.tensor(np.log(kappa / (1 - kappa)))
                 self.kappa = nn.ParameterDict(self.kappa)
-            
+
             if rho != None:
                 self.rho = {}
-                self.rho["global"] = torch.tensor(np.log(rho/(1-rho)))
+                self.rho["global"] = torch.tensor(np.log(rho / (1 - rho)))
                 for cell_type in self.cell_types:
-                    self.rho[cell_type] = torch.tensor(np.log(rho/(1-rho)))
+                    self.rho[cell_type] = torch.tensor(np.log(rho / (1 - rho)))
                 self.rho = nn.ParameterDict(self.rho)
 
-    
-    def loss(self, X, labels): 
-        assert(self.use_cell_types) #if this is False, fail because model has not been initialized to use cell types
-        
-        #convert inputs to torch.Tensors
+    def loss(self, X, labels):
+        assert (
+            self.use_cell_types
+        )  # if this is False, fail because model has not been initialized to use cell types
+
+        # convert inputs to torch.Tensors
         X = torch.Tensor(X)
-        #labels = torch.Tensor(labels)
+        # labels = torch.Tensor(labels)
 
-        #initialize loss and fetch global parameters
+        # initialize loss and fetch global parameters
         loss = 0.0
-        theta_global = torch.softmax(self.theta["global"], dim = 1)
-        eta_global = (self.eta["global"]).exp()/(1.0 + (self.eta["global"]).exp())
-        eta_global = 0.5*(eta_global + eta_global.T)
-        gene_scaling_global = self.gene_scaling["global"].exp()/(1.0 + self.gene_scaling["global"].exp())
-        kappa_global = self.kappa["global"].exp()/(1 + self.kappa["global"].exp())
-        rho_global = self.rho["global"].exp()/(1 + self.rho["global"].exp())
+        theta_global = torch.softmax(self.theta["global"], dim=1)
+        eta_global = (self.eta["global"]).exp() / (1.0 + (self.eta["global"]).exp())
+        eta_global = 0.5 * (eta_global + eta_global.T)
+        gene_scaling_global = self.gene_scaling["global"].exp() / (
+            1.0 + self.gene_scaling["global"].exp()
+        )
+        kappa_global = self.kappa["global"].exp() / (1 + self.kappa["global"].exp())
+        rho_global = self.rho["global"].exp() / (1 + self.rho["global"].exp())
 
-        #loop through cell types and evaluate loss at every cell type
+        # loop through cell types and evaluate loss at every cell type
         for cell_type in self.cell_types:
-            kappa = self.kappa[cell_type].exp()/(1 + self.kappa[cell_type].exp())
-            rho = self.rho[cell_type].exp()/(1 + self.rho[cell_type].exp())
-            gene_scaling_ct = self.gene_scaling[cell_type].exp()/(1.0 + self.gene_scaling[cell_type].exp())
+            kappa = self.kappa[cell_type].exp() / (1 + self.kappa[cell_type].exp())
+            rho = self.rho[cell_type].exp() / (1 + self.rho[cell_type].exp())
+            gene_scaling_ct = self.gene_scaling[cell_type].exp() / (
+                1.0 + self.gene_scaling[cell_type].exp()
+            )
             X_c = X[labels == cell_type]
-            adj_matrix = self.adj_matrix[cell_type] 
+            adj_matrix = self.adj_matrix[cell_type]
             weights = self.weights[cell_type]
             adj_matrix_1m = self.adj_matrix_1m[cell_type]
-            theta_ct = torch.softmax(self.theta[cell_type], dim = 1)
-            eta_ct = (self.eta[cell_type]).exp()/(1.0 + (self.eta[cell_type]).exp())
-            eta_ct = 0.5*(eta_ct + eta_ct.T)
-            theta_global_ = contract('jk,j->jk',theta_global, gene_scaling_global + self.delta)
-            theta_ct_ = contract('jk,j->jk',theta_ct, gene_scaling_ct + self.delta)
-            theta = torch.cat((theta_global_, theta_ct_),1)
+            theta_ct = torch.softmax(self.theta[cell_type], dim=1)
+            eta_ct = (self.eta[cell_type]).exp() / (1.0 + (self.eta[cell_type]).exp())
+            eta_ct = 0.5 * (eta_ct + eta_ct.T)
+            theta_global_ = contract(
+                "jk,j->jk", theta_global, gene_scaling_global + self.delta
+            )
+            theta_ct_ = contract("jk,j->jk", theta_ct, gene_scaling_ct + self.delta)
+            theta = torch.cat((theta_global_, theta_ct_), 1)
             alpha = torch.exp(self.alpha[cell_type])
-            recon = contract('ik,jk->ij', alpha, theta) 
-            term1 = -1.0*(torch.xlogy(X_c,recon) - recon).sum()
+            recon = contract("ik,jk->ij", alpha, theta)
+            term1 = -1.0 * (torch.xlogy(X_c, recon) - recon).sum()
             if len(adj_matrix) > 0:
-                mat = contract('il,lj,kj->ik',theta_ct,eta_ct,theta_ct) 
-                term2 = -1.0*(torch.xlogy(adj_matrix*weights, (1.0 - rho)*(1.0 -kappa)*mat + (1.0 - rho)*kappa)).sum()
-                term3 = -1.0*(torch.xlogy(adj_matrix_1m,(1.0 -kappa)*(1.0 - rho)*(1.0 - mat) + rho)).sum()
+                mat = contract("il,lj,kj->ik", theta_ct, eta_ct, theta_ct)
+                term2 = (
+                    -1.0
+                    * (
+                        torch.xlogy(
+                            adj_matrix * weights,
+                            (1.0 - rho) * (1.0 - kappa) * mat + (1.0 - rho) * kappa,
+                        )
+                    ).sum()
+                )
+                term3 = (
+                    -1.0
+                    * (
+                        torch.xlogy(
+                            adj_matrix_1m,
+                            (1.0 - kappa) * (1.0 - rho) * (1.0 - mat) + rho,
+                        )
+                    ).sum()
+                )
             else:
                 term2 = 0.0
                 term3 = 0.0
-            #the magnitude of lambda is proportional to the number of cells [todo: simpler to just take the mean instead of sum in term 1]
-            loss = loss + self.lam*term1 +(self.cell_type_counts[cell_type]/float(self.n))*(term2 + term3) 
-            
+            # the magnitude of lambda is proportional to the number of cells [todo: simpler to just take the mean instead of sum in term 1]
+            loss = (
+                loss
+                + self.lam * term1
+                + (self.cell_type_counts[cell_type] / float(self.n)) * (term2 + term3)
+            )
 
-        #compute loss associated with global graph
-        adj_matrix = self.adj_matrix["global"] 
+        # compute loss associated with global graph
+        adj_matrix = self.adj_matrix["global"]
         adj_matrix_1m = self.adj_matrix_1m["global"]
         weights = self.weights["global"]
         if len(adj_matrix) > 0:
-            mat = contract('il,lj,kj->ik',theta_global,eta_global,theta_global) 
-            term2 = -1.0*(torch.xlogy(adj_matrix*weights, (1.0 - rho_global)*(1.0 -kappa_global)*mat + (1.0 - rho_global)*kappa_global)).sum()
-            term3 = -1.0*(torch.xlogy(adj_matrix_1m, (1.0 -kappa_global)*(1.0 - rho_global)*(1.0 - mat) + rho_global)).sum()
-            loss = loss + term2 + term3 
+            mat = contract("il,lj,kj->ik", theta_global, eta_global, theta_global)
+            term2 = (
+                -1.0
+                * (
+                    torch.xlogy(
+                        adj_matrix * weights,
+                        (1.0 - rho_global) * (1.0 - kappa_global) * mat
+                        + (1.0 - rho_global) * kappa_global,
+                    )
+                ).sum()
+            )
+            term3 = (
+                -1.0
+                * (
+                    torch.xlogy(
+                        adj_matrix_1m,
+                        (1.0 - kappa_global) * (1.0 - rho_global) * (1.0 - mat)
+                        + rho_global,
+                    )
+                ).sum()
+            )
+            loss = loss + term2 + term3
         return loss
-    
+
     def loss_no_cell_types(self, X):
-        assert(self.use_cell_types == False) #if this is True, just fail 
+        assert self.use_cell_types == False  # if this is True, just fail
         X = torch.Tensor(X)
 
-        theta = torch.softmax(self.theta, dim = 1)
-        eta = self.eta.exp()/(1.0 + (self.eta).exp())
-        eta = 0.5*(eta + eta.T)
-        gene_scaling = self.gene_scaling.exp()/(1.0 + self.gene_scaling.exp())
-        kappa = self.kappa.exp()/(1 + self.kappa.exp())
-        rho = self.rho.exp()/(1 + self.rho.exp())
+        theta = torch.softmax(self.theta, dim=1)
+        eta = self.eta.exp() / (1.0 + (self.eta).exp())
+        eta = 0.5 * (eta + eta.T)
+        gene_scaling = self.gene_scaling.exp() / (1.0 + self.gene_scaling.exp())
+        kappa = self.kappa.exp() / (1 + self.kappa.exp())
+        rho = self.rho.exp() / (1 + self.rho.exp())
         alpha = torch.exp(self.alpha)
         adj_matrix = self.adj_matrix
         weights = self.weights
         adj_matrix_1m = self.adj_matrix_1m
-        theta_ = contract('jk,j->jk',theta, gene_scaling + self.delta)
-        recon = contract('ik,jk->ij', alpha, theta_) 
-        term1 = -1.0*(torch.xlogy(X,recon) - recon).sum()
-
+        theta_ = contract("jk,j->jk", theta, gene_scaling + self.delta)
+        recon = contract("ik,jk->ij", alpha, theta_)
+        term1 = -1.0 * (torch.xlogy(X, recon) - recon).sum()
 
         if len(adj_matrix) > 0:
-                mat = contract('il,lj,kj->ik',theta,eta,theta) 
-                term2 = -1.0*(torch.xlogy(adj_matrix*weights, (1.0 - rho)*(1.0 -kappa)*mat + (1.0 - rho)*kappa)).sum()
-                term3 = -1.0*(torch.xlogy(adj_matrix_1m,(1.0 -kappa)*(1.0 - rho)*(1.0 - mat) + rho)).sum()
+            mat = contract("il,lj,kj->ik", theta, eta, theta)
+            term2 = (
+                -1.0
+                * (
+                    torch.xlogy(
+                        adj_matrix * weights,
+                        (1.0 - rho) * (1.0 - kappa) * mat + (1.0 - rho) * kappa,
+                    )
+                ).sum()
+            )
+            term3 = (
+                -1.0
+                * (
+                    torch.xlogy(
+                        adj_matrix_1m, (1.0 - kappa) * (1.0 - rho) * (1.0 - mat) + rho
+                    )
+                ).sum()
+            )
         else:
             term2 = 0.0
             term3 = 0.0
 
-        return self.lam*term1 + term2 + term3    
+        return self.lam * term1 + term2 + term3
 
-    def initialize(self,gene_sets,val):    
+    def initialize(self, gene_sets, val):
         """
         form of gene_sets:
-        
+
         cell_type (inc. global) : set of sets of idxs
         """
-        
+
         for ct in self.cell_types:
-            assert(self.L[ct] >= len(gene_sets[ct]))
+            assert self.L[ct] >= len(gene_sets[ct])
             count = 0
             if self.L[ct] > 0:
                 if len(self.adj_matrix[ct]) > 0:
                     for gene_set in gene_sets[ct]:
-                        self.theta[ct].data[:,count][gene_set] = val
+                        self.theta[ct].data[:, count][gene_set] = val
                         count = count + 1
                     for i in range(self.L[ct]):
-                        self.eta[ct].data[i,-1] = -val
-                        self.eta[ct].data[-1,i] = -val
-                    self.theta[ct].data[:,-1][self.adj_matrix[ct].sum(axis = 1) == 0] = val
-                    self.theta[ct].data[:,-1][self.adj_matrix[ct].sum(axis = 1) != 0] = -val
+                        self.eta[ct].data[i, -1] = -val
+                        self.eta[ct].data[-1, i] = -val
+                    self.theta[ct].data[:, -1][self.adj_matrix[ct].sum(axis=1) == 0] = (
+                        val
+                    )
+                    self.theta[ct].data[:, -1][self.adj_matrix[ct].sum(axis=1) != 0] = (
+                        -val
+                    )
 
-        assert(self.L["global"] >= len(gene_sets["global"]))
+        assert self.L["global"] >= len(gene_sets["global"])
         count = 0
         for gene_set in gene_sets["global"]:
-            self.theta["global"].data[:,count][gene_set] = val
+            self.theta["global"].data[:, count][gene_set] = val
             count = count + 1
         for i in range(self.L["global"]):
-            self.eta["global"].data[i,-1] = -val
-            self.eta["global"].data[-1,i] = -val
-        self.theta["global"].data[:,-1][self.adj_matrix["global"].sum(axis = 1) == 0] = val
-        self.theta["global"].data[:,-1][self.adj_matrix["global"].sum(axis = 1) != 0] = -val
-    def initialize_no_celltypes(self,gs_list,val):
-        assert(self.L >= len(gs_list))
+            self.eta["global"].data[i, -1] = -val
+            self.eta["global"].data[-1, i] = -val
+        self.theta["global"].data[:, -1][self.adj_matrix["global"].sum(axis=1) == 0] = (
+            val
+        )
+        self.theta["global"].data[:, -1][self.adj_matrix["global"].sum(axis=1) != 0] = (
+            -val
+        )
+
+    def initialize_no_celltypes(self, gs_list, val):
+        assert self.L >= len(gs_list)
         count = 0
         for gene_set in gs_list:
-            self.theta.data[:,count][gene_set] = val
+            self.theta.data[:, count][gene_set] = val
             count = count + 1
         for i in range(self.L):
-            self.eta.data[i,-1]= -val 
-            self.eta.data[-1,i] = -val 
-        self.theta.data[:,-1][self.adj_matrix.sum(axis = 1) == 0] = val
-        self.theta.data[:,-1][self.adj_matrix.sum(axis = 1) != 0] = -val 
+            self.eta.data[i, -1] = -val
+            self.eta.data[-1, i] = -val
+        self.theta.data[:, -1][self.adj_matrix.sum(axis=1) == 0] = val
+        self.theta.data[:, -1][self.adj_matrix.sum(axis=1) != 0] = -val
+
+
 class spectra_attn(nn.Module):
     """
     Spectra v2: (1) attention based or (2) remove MMSB constraint allowing true multi membership for gene nodes (3) VI uncertainty
     > tradeoff between noisy gene sets and getting lowly expressed genes
     > tradeoff between simplex constraint and adding new genes - simplex allows using background factors
-    > how to add new factors w/ attention based method, if you allow dropping 
+    > how to add new factors w/ attention based method, if you allow dropping
     """
-    def __init__(self, X, K, gene_set_matrix, lambda_ = 1.0, d = 10, lam = 0.01):
+
+    def __init__(self, X, K, gene_set_matrix, lambda_=1.0, d=10, lam=0.01):
         super(spectra_attn, self).__init__()
         self.p = X.shape[1]
         self.n = X.shape[0]
-        self.K = K 
+        self.K = K
         self.d = d
-        self.X = X 
+        self.X = X
         self.gene_set_matrix = gene_set_matrix
         self.L = gene_set_matrix.shape[0]
         self.lambda_ = lambda_
 
-        self.theta = nn.Parameter(Normal(0.,1.).sample([self.n, self.K]))
-        self.gamma = nn.Parameter(Normal(0.,1.).sample([self.p, self.K]))
-        self.query = nn.Parameter(Normal(0.,1.).sample([self.K, self.d]))
-        self.keys = nn.Parameter(Normal(0.,1.).sample([self.L, self.d]))
-    def loss(self): 
-        #compute the Poisson reconstruction loss
+        self.theta = nn.Parameter(Normal(0.0, 1.0).sample([self.n, self.K]))
+        self.gamma = nn.Parameter(Normal(0.0, 1.0).sample([self.p, self.K]))
+        self.query = nn.Parameter(Normal(0.0, 1.0).sample([self.K, self.d]))
+        self.keys = nn.Parameter(Normal(0.0, 1.0).sample([self.L, self.d]))
+
+    def loss(self):
+        # compute the Poisson reconstruction loss
         gamma = self.gamma.exp()
         theta = self.theta.exp()
-        reconstruction  = contract('ij,kj->ik',theta,gamma)
-        loss_1 = (-1*torch.xlogy(self.X, reconstruction) + reconstruction).sum()
-
-        #compute the attention dot products, K x L similarities
-        similarities = contract('ij,kj->ik',self.query, self.keys)/torch.sqrt(self.d)
-        similarities = similarities.softmax(dim = 1)
-
-        #compute assignments, K x p
-        assignments = contract('ij,jk->ik', similarities, self.gene_set_matrix)
-
-        #compute loss per assignments
-        loss_2 = (-1*torch.xlogy(self.assignments, self.gamma.T) + self.gamma.T).sum()
-        return loss_1 + self.lambda_*loss_2
+        reconstruction = contract("ij,kj->ik", theta, gamma)
+        loss_1 = (-1 * torch.xlogy(self.X, reconstruction) + reconstruction).sum()
 
+        # compute the attention dot products, K x L similarities
+        similarities = contract("ij,kj->ik", self.query, self.keys) / torch.sqrt(self.d)
+        similarities = similarities.softmax(dim=1)
+
+        # compute assignments, K x p
+        assignments = contract("ij,jk->ik", similarities, self.gene_set_matrix)
+
+        # compute loss per assignments
+        loss_2 = (-1 * torch.xlogy(self.assignments, self.gamma.T) + self.gamma.T).sum()
+        return loss_1 + self.lambda_ * loss_2
 
 
 class SPECTRA_Model:
-    """ 
-    
+    """
+
     Parameters
         ----------
         X : np.ndarray or torch.Tensor
             the ``(n, p)`` -shaped matrix containing logged expression count data. Used for initialization of self.n and self.p but not stored as an attribute
         labels : np.ndarray or NoneType
             the ``(n, )`` -shaped array containing cell type labels. If use_cell_types == False, then should be set to None
-        
+
         L : dict or OrderedDict [if use_cell_types == False, then int]
             ``number of cell types + 1``-shaped dictionary. Must have "global" as a key, indicating the number of global factors
             {
-                "global": 15, 
-                "CD8": 5 
-                ...    
+                "global": 15,
+                "CD8": 5
+                ...
             }
-            > Format matches output of K_est.py to estimate the number of 
+            > Format matches output of K_est.py to estimate the number of
             > Must match cell type labels provided during training
-            > Recommended practice is to assign at minimum 2 factors per cell type 
+            > Recommended practice is to assign at minimum 2 factors per cell type
             > L contains the number of factors that describe the graph.
         adj_matrix :  dict or OrderedDict
-            ``a dictionary of adjacency matrices, one for every cell type + a "global" 
+            ``a dictionary of adjacency matrices, one for every cell type + a "global"
             {
                 "global": ``(p, p)``-shaped binary np.ndarray
-                "CD8": ... 
+                "CD8": ...
 
-            } 
+            }
         weights : dict or OrderedDict or NoneType [if use_cell_types == False, then ``(p, p)``-shaped array]
             the ``(p, p)``-shaped set of edge weights per . If weight[i,j] is non-zero when adj_matrix[i,j] = 0
-            this weight is ignored. 
-            
+            this weight is ignored.
+
             if weights == None, no weights are used
         lam : float
-            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information  
-        delta : float 
-            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes. 
+            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information
+        delta : float
+            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes.
         kappa : float or NoneType
-            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.  
+            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.
         rho : float or NoneType
-            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data. 
-        use_cell_types: bool 
+            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data.
+        use_cell_types: bool
             use_cell_types is a Boolean variable that determines whether cell type labels are used to fit the model. If False, then parameters are initialized as nn.Parameter rather than as nn.ParameterDict with cell type keys that index nn.Parameter values
         determinant_penalty : float
-            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.  
+            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.
     Attributes
         ----------
         model.delta : delta parameter of the model
 
-        model.lam : lambda parameter of the model 
-       
-        model.determinant_penalty : determinant penalty of the model 
- 
-        model.L : L parameter, either int, dict or OrderedDict() 
+        model.lam : lambda parameter of the model
+
+        model.determinant_penalty : determinant penalty of the model
+
+        model.L : L parameter, either int, dict or OrderedDict()
 
         model.p : number of genes
 
-        model.n : number of cells 
+        model.n : number of cells
 
-        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters. 
+        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters.
 
         model.kappa : if not kappa, nn.ParameterDict() if use_cell_types, else nn.Parameter(). If kappa is a float, it is fixed throughout training
 
         model.rho : if not rho, nn.ParamterDict() if use_cell_types, else nn.Parameter. If rho is a float it is fixed throughout training
 
-        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors 
+        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.weights : contains edge weights. format matches adj_matrix
 
-        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors 
-        
-        model.weights : contains edge weights. format matches adj_matrix 
-        
         model.cell_types : np.ndarray containing array of unique cell types
-       
+
         model.cell_type_counts : dict {key = cell type, values = number of cells}
- 
-        model.factors : nn.ParameterDict() or nn.Parameter() containing the factor weights 
+
+        model.factors : nn.ParameterDict() or nn.Parameter() containing the factor weights
 
         model.cell_scores : nn.ParameterDict() or nn.Parameter() containing the cell loadings
 
         model.eta : nn.ParameterDict() or nn.Parameter() containing the interaction matrix between factors
 
         model.gene_scaling : nn.ParameterDict() or nn.Parameter() containing the gene scale factors
 
-        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False 
-        
-        
+        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False
+
+
 
     Methods
         ----------
 
-        model.train(self, X, labels, lr_schedule,num_epochs, verbose) : 
+        model.train(self, X, labels, lr_schedule,num_epochs, verbose) :
         model.save()
         model.load()
         model.initialize
         model.return_selection()
         model.return_eta_diag()
         model.return_cell_scores()
-        model.return_factors() 
+        model.return_factors()
         model.return_eta()
-        model.return_rho() 
+        model.return_rho()
         model.return_kappa()
         model.return_gene_scalings()
-        model.return_graph(ct = "global") : 
+        model.return_graph(ct = "global") :
         model.matching(markers, gene_names_dict, threshold = 0.4):
 
     """
-    def __init__(self,X, labels,  L, vocab = None, gs_dict = None, use_weights = True, adj_matrix = None, weights = None, lam = 0.01, delta = 0.001,kappa = None, rho = 0.001, use_cell_types = True):
+
+    def __init__(
+        self,
+        X,
+        labels,
+        L,
+        vocab=None,
+        gs_dict=None,
+        use_weights=True,
+        adj_matrix=None,
+        weights=None,
+        lam=0.01,
+        delta=0.001,
+        kappa=None,
+        rho=0.001,
+        use_cell_types=True,
+    ):
         self.L = L
-        self.lam = lam 
-        self.delta = delta 
-        self.kappa = kappa 
-        self.rho = rho 
+        self.lam = lam
+        self.delta = delta
+        self.kappa = kappa
+        self.rho = rho
         self.use_cell_types = use_cell_types
 
         # if gs_dict is provided instead of adj_matrix, convert to adj_matrix, overrides adj_matrix and weights
         if gs_dict is not None:
             gene2id = dict((v, idx) for idx, v in enumerate(vocab))
-            
+
             if use_cell_types:
-                adj_matrix, weights = Spectra_util.process_gene_sets(gs_dict = gs_dict, gene2id = gene2id, weighted = use_weights)
+                adj_matrix, weights = Spectra_util.process_gene_sets(
+                    gs_dict=gs_dict, gene2id=gene2id, weighted=use_weights
+                )
             else:
-                adj_matrix, weights = Spectra_util.process_gene_sets_no_celltypes(gs_dict = gs_dict, gene2id = gene2id, weighted = use_weights)
-
-
-        self.internal_model = SPECTRA(X = X, labels = labels, adj_matrix = adj_matrix, L = L, weights = weights, lam = lam, delta=delta,kappa = kappa, rho = rho, use_cell_types = use_cell_types)
+                adj_matrix, weights = Spectra_util.process_gene_sets_no_celltypes(
+                    gs_dict=gs_dict, gene2id=gene2id, weighted=use_weights
+                )
+
+        self.internal_model = SPECTRA(
+            X=X,
+            labels=labels,
+            adj_matrix=adj_matrix,
+            L=L,
+            weights=weights,
+            lam=lam,
+            delta=delta,
+            kappa=kappa,
+            rho=rho,
+            use_cell_types=use_cell_types,
+        )
 
         self.cell_scores = None
         self.factors = None
         self.B_diag = None
-        self.eta_matrices = None 
-        self.gene_scalings = None 
-        self.rho = None 
-        self.kappa = None 
-
-    def train(self,X, labels = None, lr_schedule = [1.0,.5,.1,.01,.001,.0001],num_epochs = 10000, verbose = False): 
+        self.eta_matrices = None
+        self.gene_scalings = None
+        self.rho = None
+        self.kappa = None
+
+    def train(
+        self,
+        X,
+        labels=None,
+        lr_schedule=[1.0, 0.5, 0.1, 0.01, 0.001, 0.0001],
+        num_epochs=10000,
+        verbose=False,
+    ):
         opt = torch.optim.Adam(self.internal_model.parameters(), lr=lr_schedule[0])
         counter = 0
         last = np.inf
 
         for i in tqdm(range(num_epochs)):
-            #print(counter)
+            # print(counter)
             opt.zero_grad()
             if self.internal_model.use_cell_types:
-                assert(len(labels) == X.shape[0])
+                assert len(labels) == X.shape[0]
                 loss = self.internal_model.loss(X, labels)
             elif self.internal_model.use_cell_types == False:
                 loss = self.internal_model.loss_no_cell_types(X)
 
             loss.backward()
             opt.step()
-        
+
             if loss.item() >= last:
                 counter += 1
-                if int(counter/3) >= len(lr_schedule):
+                if int(counter / 3) >= len(lr_schedule):
                     break
                 if counter % 3 == 0:
-                    opt = torch.optim.Adam(self.internal_model.parameters(), lr=lr_schedule[int(counter/3)])
+                    opt = torch.optim.Adam(
+                        self.internal_model.parameters(),
+                        lr=lr_schedule[int(counter / 3)],
+                    )
                     if verbose:
-                        print("UPDATING LR TO " + str(lr_schedule[int(counter/3)]))
-            last = loss.item() 
+                        print("UPDATING LR TO " + str(lr_schedule[int(counter / 3)]))
+            last = loss.item()
 
-
-        #add all model parameters as attributes 
+        # add all model parameters as attributes
 
         if self.use_cell_types:
             self.__store_parameters(labels)
         else:
             self.__store_parameters_no_celltypes()
+
     def save(self, fp):
-        torch.save(self.internal_model.state_dict(),fp)
-  
-    def load(self,fp,labels = None):
+        torch.save(self.internal_model.state_dict(), fp)
+
+    def load(self, fp, labels=None):
         self.internal_model.load_state_dict(torch.load(fp))
         if self.use_cell_types:
-            assert(labels is not None)
+            assert labels is not None
             self.__store_parameters(labels)
         else:
             self.__store_parameters_no_celltypes()
 
-    def __store_parameters(self,labels):
-
+    def __store_parameters(self, labels):
         """
         Replaces __cell_scores() and __compute factors() and __compute_theta()
         store parameters after fitting the model:
             cell scores
             factors
             eta
             scalings
             gene scalings
-            kappa 
-            rho 
+            kappa
+            rho
         """
 
         model = self.internal_model
 
-        #compute the loading matrix
+        # compute the loading matrix
 
         k = sum(list(model.L.values()))
         out = np.zeros((model.n, k))
-        
+
         global_idx = model.L["global"]
-        
-        tot = global_idx    
-        f  = ["global"]*model.L["global"]
+
+        tot = global_idx
+        f = ["global"] * model.L["global"]
         for cell_type in model.cell_types:
             alpha = torch.exp(model.alpha[cell_type]).detach().numpy()
-            out[labels == cell_type, :global_idx] =  alpha[:,:global_idx]
-            out[labels == cell_type, tot:tot+model.L[cell_type]] = alpha[:,global_idx:]
-            
-            tot += model.L[cell_type]
+            out[labels == cell_type, :global_idx] = alpha[:, :global_idx]
+            out[labels == cell_type, tot : tot + model.L[cell_type]] = alpha[
+                :, global_idx:
+            ]
 
-            f = f + [cell_type]*model.L[cell_type]
+            tot += model.L[cell_type]
 
+            f = f + [cell_type] * model.L[cell_type]
 
         out2 = np.zeros((k, model.p))
-        
-        theta_ct = torch.softmax(model.theta["global"], dim = 1)
+
+        theta_ct = torch.softmax(model.theta["global"], dim=1)
         theta = theta_ct.detach().numpy().T
         tot = 0
-        out2[0:theta.shape[0],:] = theta 
+        out2[0 : theta.shape[0], :] = theta
         tot += theta.shape[0]
-        
+
         for cell_type in model.cell_types:
-            theta_ct = torch.softmax(model.theta[cell_type], dim = 1)
+            theta_ct = torch.softmax(model.theta[cell_type], dim=1)
             theta = theta_ct.detach().numpy().T
-            out2[tot:tot+theta.shape[0],:] = theta 
+            out2[tot : tot + theta.shape[0], :] = theta
             tot += theta.shape[0]
-        
+
         factors = out2
         lst = []
         for i in range(len(f)):
             ct = f[i]
-            scaled = factors[i,:]*(model.gene_scaling[ct].exp().detach()/(1.0 + model.gene_scaling[ct].exp().detach()) + model.delta).numpy()
-
+            scaled = (
+                factors[i, :]
+                * (
+                    model.gene_scaling[ct].exp().detach()
+                    / (1.0 + model.gene_scaling[ct].exp().detach())
+                    + model.delta
+                ).numpy()
+            )
 
             lst.append(scaled)
         scaled = np.array(lst)
-        new_factors = scaled/(scaled.sum(axis = 0,keepdims =True) + 1.0)
-        cell_scores = out*scaled.mean(axis = 1).reshape(1,-1) 
+        new_factors = scaled / (scaled.sum(axis=0, keepdims=True) + 1.0)
+        cell_scores = out * scaled.mean(axis=1).reshape(1, -1)
         self.cell_scores = cell_scores
         self.factors = new_factors
         self.B_diag = self.__B_diag()
         self.eta_matrices = self.__eta_matrices()
-        self.gene_scalings = {ct: model.gene_scaling[ct].exp().detach().numpy()/(1.0 + model.gene_scaling[ct].exp().detach().numpy()) for ct in model.gene_scaling.keys()}
-        self.rho = {ct: model.rho[ct].exp().detach().numpy()/(1.0 + model.rho[ct].exp().detach().numpy()) for ct in model.rho.keys()}
-        self.kappa = {ct: model.kappa[ct].exp().detach().numpy()/(1.0 + model.kappa[ct].exp().detach().numpy()) for ct in model.kappa.keys()}
+        self.gene_scalings = {
+            ct: model.gene_scaling[ct].exp().detach().numpy()
+            / (1.0 + model.gene_scaling[ct].exp().detach().numpy())
+            for ct in model.gene_scaling.keys()
+        }
+        self.rho = {
+            ct: model.rho[ct].exp().detach().numpy()
+            / (1.0 + model.rho[ct].exp().detach().numpy())
+            for ct in model.rho.keys()
+        }
+        self.kappa = {
+            ct: model.kappa[ct].exp().detach().numpy()
+            / (1.0 + model.kappa[ct].exp().detach().numpy())
+            for ct in model.kappa.keys()
+        }
 
     def __B_diag(self):
         model = self.internal_model
         k = sum(list(model.L.values()))
         out = np.zeros(k)
-        
-        Bg = model.eta["global"].exp()/(1.0 + model.eta["global"].exp())
-        Bg = 0.5*(Bg + Bg.T)
+
+        Bg = model.eta["global"].exp() / (1.0 + model.eta["global"].exp())
+        Bg = 0.5 * (Bg + Bg.T)
         B = torch.diag(Bg).detach().numpy()
         tot = 0
-        out[0:B.shape[0]] = B
+        out[0 : B.shape[0]] = B
         tot += B.shape[0]
-        
+
         for cell_type in model.cell_types:
-            Bg = model.eta[cell_type].exp()/(1.0 + model.eta[cell_type].exp())
-            Bg = 0.5*(Bg + Bg.T)
+            Bg = model.eta[cell_type].exp() / (1.0 + model.eta[cell_type].exp())
+            Bg = 0.5 * (Bg + Bg.T)
             B = torch.diag(Bg).detach().numpy()
-            out[tot:tot+B.shape[0]] = B
-            
+            out[tot : tot + B.shape[0]] = B
+
             tot += B.shape[0]
 
         return out
 
     def __eta_matrices(self):
         model = self.internal_model
         eta = OrderedDict()
-        Bg = model.eta["global"].exp()/(1.0 + model.eta["global"].exp())
-        Bg = 0.5*(Bg + Bg.T)
+        Bg = model.eta["global"].exp() / (1.0 + model.eta["global"].exp())
+        Bg = 0.5 * (Bg + Bg.T)
         eta["global"] = Bg.detach().numpy()
 
         for cell_type in model.cell_types:
-            Bg = model.eta[cell_type].exp()/(1.0 + model.eta[cell_type].exp())
-            Bg = 0.5*(Bg + Bg.T)
+            Bg = model.eta[cell_type].exp() / (1.0 + model.eta[cell_type].exp())
+            Bg = 0.5 * (Bg + Bg.T)
             eta[cell_type] = Bg.detach().numpy()
-        return eta 
-
+        return eta
 
     def __store_parameters_no_celltypes(self):
         """
         store parameters after fitting the model:
             cell scores
             factors
             eta
             scalings
             gene scalings
-            kappa 
-            rho 
+            kappa
+            rho
         """
         model = self.internal_model
-        theta_ct = torch.softmax(model.theta, dim = 1)
+        theta_ct = torch.softmax(model.theta, dim=1)
         theta = theta_ct.detach().numpy().T
         alpha = torch.exp(model.alpha).detach().numpy()
         out = alpha
-        factors = theta 
+        factors = theta
 
-        scaled = factors*(model.gene_scaling.exp().detach()/(1.0 + model.gene_scaling.exp().detach()) + model.delta).numpy().reshape(1,-1)
-        new_factors = scaled/(scaled.sum(axis = 0,keepdims =True) + 1.0)
+        scaled = factors * (
+            model.gene_scaling.exp().detach()
+            / (1.0 + model.gene_scaling.exp().detach())
+            + model.delta
+        ).numpy().reshape(1, -1)
+        new_factors = scaled / (scaled.sum(axis=0, keepdims=True) + 1.0)
 
         self.factors = new_factors
-        self.cell_scores = out*scaled.mean(axis = 1).reshape(1,-1)  
-        Bg = model.eta.exp()/(1.0 + model.eta.exp())
-        Bg = 0.5*(Bg + Bg.T)
+        self.cell_scores = out * scaled.mean(axis=1).reshape(1, -1)
+        Bg = model.eta.exp() / (1.0 + model.eta.exp())
+        Bg = 0.5 * (Bg + Bg.T)
         self.B_diag = torch.diag(Bg).detach().numpy()
         self.eta_matrices = Bg.detach().numpy()
-        self.gene_scalings = (model.gene_scaling.exp().detach()/(1.0 + model.gene_scaling.exp().detach())).numpy()
-        self.rho = (model.rho.exp().detach()/(1.0 + model.rho.exp().detach())).numpy()
-        self.kappa = (model.kappa.exp().detach()/(1.0 + model.kappa.exp().detach())).numpy()
-    def initialize(self,annotations, word2id, W, init_scores, val = 25):
+        self.gene_scalings = (
+            model.gene_scaling.exp().detach()
+            / (1.0 + model.gene_scaling.exp().detach())
+        ).numpy()
+        self.rho = (model.rho.exp().detach() / (1.0 + model.rho.exp().detach())).numpy()
+        self.kappa = (
+            model.kappa.exp().detach() / (1.0 + model.kappa.exp().detach())
+        ).numpy()
+
+    def initialize(self, annotations, word2id, W, init_scores, val=25):
         """
         self.use_cell_types must be True
         create form of gene_sets:
-        
+
         cell_type (inc. global) : set of sets of idxs
-        
+
         filter based on L_ct
         """
         if self.use_cell_types:
             if init_scores == None:
-                init_scores = compute_init_scores(annotations, word2id, torch.Tensor(W)) 
+                init_scores = compute_init_scores(annotations, word2id, torch.Tensor(W))
             gs_dict = OrderedDict()
             for ct in annotations.keys():
-                mval = max(self.L[ct] - 1, 0) 
-                sorted_init_scores = sorted(init_scores[ct].items(), key=lambda x:x[1])
-                sorted_init_scores = sorted_init_scores[-1*mval:]
-                names = set([k[0] for k in sorted_init_scores])  
+                mval = max(self.L[ct] - 1, 0)
+                sorted_init_scores = sorted(init_scores[ct].items(), key=lambda x: x[1])
+                sorted_init_scores = sorted_init_scores[-1 * mval :]
+                names = set([k[0] for k in sorted_init_scores])
                 lst_ct = []
                 for key in annotations[ct].keys():
                     if key in names:
                         words = annotations[ct][key]
                         idxs = []
                         for word in words:
                             if word in word2id:
                                 idxs.append(word2id[word])
                         lst_ct.append(idxs)
                 gs_dict[ct] = lst_ct
-            self.internal_model.initialize(gene_sets = gs_dict, val = val)
+            self.internal_model.initialize(gene_sets=gs_dict, val=val)
         else:
             if init_scores == None:
-                init_scores = compute_init_scores_noct(annotations,word2id,torch.Tensor(W))
+                init_scores = compute_init_scores_noct(
+                    annotations, word2id, torch.Tensor(W)
+                )
             lst = []
             mval = max(self.L - 1, 0)
-            sorted_init_scores = sorted(init_scores.items(), key = lambda x:x[1])
-            sorted_init_scores = sorted_init_scores[-1*mval:]
-            names = set([k[0] for k in sorted_init_scores])   
+            sorted_init_scores = sorted(init_scores.items(), key=lambda x: x[1])
+            sorted_init_scores = sorted_init_scores[-1 * mval :]
+            names = set([k[0] for k in sorted_init_scores])
             for key in annotations.keys():
                 if key in names:
                     words = annotations[key]
                     idxs = []
                     for word in words:
                         if word in word2id:
                             idxs.append(word2id[word])
                     lst.append(idxs)
-            self.internal_model.initialize_no_celltypes(gs_list = lst, val = val)
-        
+            self.internal_model.initialize_no_celltypes(gs_list=lst, val=val)
+
     def return_eta_diag(self):
         return self.B_diag
+
     def return_cell_scores(self):
         return self.cell_scores
+
     def return_factors(self):
-        return self.factors 
+        return self.factors
+
     def return_eta(self):
         return self.eta_matrices
+
     def return_rho(self):
-        return self.rho 
+        return self.rho
+
     def return_kappa(self):
         return self.kappa
-    def return_gene_scalings(self): 
+
+    def return_gene_scalings(self):
         return self.gene_scalings
-    def return_graph(self, ct = "global"):
+
+    def return_graph(self, ct="global"):
         model = self.internal_model
         if self.use_cell_types:
-            eta = (model.eta[ct]).exp()/(1.0 + (model.eta[ct]).exp())
-            eta = 0.5*(eta + eta.T)
-            theta = torch.softmax(model.theta[ct], dim = 1)
-            mat = contract('il,lj,kj->ik',theta,eta,theta).detach().numpy()
-        else: 
-            eta = model.eta.exp()/(1.0 + model.eta.exp())
-            eta = 0.5*(eta + eta.T)
-            theta = torch.softmax(model.theta, dim = 1)
-            mat = contract('il,lj,kj->ik',theta,eta,theta).detach().numpy()
+            eta = (model.eta[ct]).exp() / (1.0 + (model.eta[ct]).exp())
+            eta = 0.5 * (eta + eta.T)
+            theta = torch.softmax(model.theta[ct], dim=1)
+            mat = contract("il,lj,kj->ik", theta, eta, theta).detach().numpy()
+        else:
+            eta = model.eta.exp() / (1.0 + model.eta.exp())
+            eta = 0.5 * (eta + eta.T)
+            theta = torch.softmax(model.theta, dim=1)
+            mat = contract("il,lj,kj->ik", theta, eta, theta).detach().numpy()
         return mat
-        
-    def matching(self, markers, gene_names_dict, threshold = 0.4):
+
+    def matching(self, markers, gene_names_dict, threshold=0.4):
         """
         best match based on overlap coefficient
         """
         markers = pd.DataFrame(markers)
         if self.use_cell_types:
             matches = []
             jaccards = []
             for i in range(markers.shape[0]):
-                max_jacc = 0.0 
+                max_jacc = 0.0
                 best = ""
                 for key in gene_names_dict.keys():
                     for gs in gene_names_dict[key].keys():
                         t = gene_names_dict[key][gs]
 
-                        jacc = Spectra_util.overlap_coefficient(list(markers.iloc[i,:]),t)
+                        jacc = Spectra_util.overlap_coefficient(
+                            list(markers.iloc[i, :]), t
+                        )
                         if jacc > max_jacc:
                             max_jacc = jacc
-                            best = gs 
+                            best = gs
                 matches.append(best)
                 jaccards.append(max_jacc)
-            
+
         else:
             matches = []
             jaccards = []
             for i in range(markers.shape[0]):
-                max_jacc = 0.0 
+                max_jacc = 0.0
                 best = ""
                 for key in gene_names_dict.keys():
                     t = gene_names_dict[key]
 
-                    jacc = Spectra_util.overlap_coefficient(list(markers.iloc[i,:]),t)
+                    jacc = Spectra_util.overlap_coefficient(list(markers.iloc[i, :]), t)
                     if jacc > max_jacc:
                         max_jacc = jacc
-                        best = key 
+                        best = key
                 matches.append(best)
                 jaccards.append(max_jacc)
         output = []
         for j in range(markers.shape[0]):
             if jaccards[j] > threshold:
                 output.append(matches[j])
             else:
                 output.append("0")
         return np.array(output)
 
+
 class SPECTRA_EM:
     """
     non-integrative SPECTRA -- EM Routine
 
-    Usage: 
+    Usage:
 
     model = EMSPADE(X = X, A=A, K = K, lam = 0.5, T= 15, kappa = 0)
-    model.fit(n_epochs = 200) 
+    model.fit(n_epochs = 200)
 
 
     Notes
     _________________
 
     > EM is recommended for problems where K is smaller [as the memory scales with K**2, as opposed to K for GD]
-        e.g. when we are only interested in 1 cell type 
+        e.g. when we are only interested in 1 cell type
 
-    > EM does not currently support estimation of rho and kappa (this was added after the paper) 
+    > EM does not currently support estimation of rho and kappa (this was added after the paper)
 
-    > We notice more stable estimates from EM in general 
+    > We notice more stable estimates from EM in general
 
     """
-    def __init__(self, X, A, weights = None, K = 10, delta = 0.001, kappa = None,rho = 0.001,lam = 0.01, T = 3):
+
+    def __init__(
+        self,
+        X,
+        A,
+        weights=None,
+        K=10,
+        delta=0.001,
+        kappa=None,
+        rho=0.001,
+        lam=0.01,
+        T=3,
+    ):
         self.EPS = 0.0
-        #fixed constants
+        # fixed constants
         self.K = K
         self.delta = delta
         self.kappa = kappa
         self.lam = lam
         self.rho = rho
         self.T = T
         self.n = X.shape[0]
         self.p = X.shape[1]
-        
-        #data
+
+        # data
         self.X = X
         self.A = A - np.diag(np.diag(A))
         A1m = 1 - A
         self.A1m = A1m - np.diag(np.diag(A1m))
         if weights is not None:
             self.weights = weights
         else:
             self.weights = self.A
-        
-        #random initializations 
-        self.theta = np.random.normal(size = (self.p,self.K))
-        self.theta = softmax(self.theta, axis = 1)
-        self.alpha = np.exp(np.random.normal(size = (self.n,self.K)))
-        self.g = np.random.normal(size= self.p)
-        self.g = np.exp(self.g)/(1.0 + np.exp(self.g))
-        self.B = np.random.normal(size = (self.K,self.K))
-        self.B = np.exp(self.B)/(1.0 + np.exp(self.B)) 
-        self.B = 0.5*(self.B + (self.B).T) #make symmetric
-        
-        #initialize pseudo-data
-        self.phi = np.exp(np.random.normal(size = (self.n, self.p, self.K)))
-        self.phi_tilde = np.exp(np.random.normal(size = (self.p, self.p, self.K, self.K)))
+
+        # random initializations
+        self.theta = np.random.normal(size=(self.p, self.K))
+        self.theta = softmax(self.theta, axis=1)
+        self.alpha = np.exp(np.random.normal(size=(self.n, self.K)))
+        self.g = np.random.normal(size=self.p)
+        self.g = np.exp(self.g) / (1.0 + np.exp(self.g))
+        self.B = np.random.normal(size=(self.K, self.K))
+        self.B = np.exp(self.B) / (1.0 + np.exp(self.B))
+        self.B = 0.5 * (self.B + (self.B).T)  # make symmetric
+
+        # initialize pseudo-data
+        self.phi = np.exp(np.random.normal(size=(self.n, self.p, self.K)))
+        self.phi_tilde = np.exp(np.random.normal(size=(self.p, self.p, self.K, self.K)))
         for j in range(self.p):
-            self.phi_tilde[j,j,:,:] = np.zeros((self.K,self.K))
+            self.phi_tilde[j, j, :, :] = np.zeros((self.K, self.K))
+
     def M_step(self):
-        #print(self.NLL())
-        #print("Running Newton iters...")
         for t in range(self.T):
             self.update_theta_newton()
-        #print(self.NLL())
-        #print("#"*20)
-        #print("Update B")
         self.update_B()
-        #print("Update alpha")
         self.update_alpha()
-        #print("Update g")
         self.update_g()
-        
+
         return
+
     def E_step(self):
         """
         need to do all computations on the ln scale
-        
+
         get up to proportionality then normalize - custom softmax for phi_tilde
-        
+
         keep self.phi_tilde[i,i,:,:] = 0s  <-- ** really important **
         """
-        
-        #phi update
-        alpha_theta = contract('ik,jk->ijk',self.alpha,self.theta)
-        multinomial_parameter = alpha_theta/(alpha_theta.sum(axis = 2, keepdims = True)+self.EPS)
+
+        # phi update
+        alpha_theta = contract("ik,jk->ijk", self.alpha, self.theta)
+        multinomial_parameter = alpha_theta / (
+            alpha_theta.sum(axis=2, keepdims=True) + self.EPS
+        )
         multinomial_parameter[~np.isfinite(multinomial_parameter)] = 0
-        self.phi = contract('ij,ijk->ijk',self.X,multinomial_parameter)
-        
-        #phi_tilde update
-        theta_prods = contract('ik,jl->ijkl',self.theta,self.theta)
-        log_term2 = contract('ij,ij,kl->ijkl',self.A, self.weights, np.log((1-self.kappa)*self.B + self.kappa))
-        log_term2[~np.isfinite(log_term2)] = 0 # A should be 0 anyways, so 
-        log_term3 = contract('ij,kl->ijkl', self.A1m, np.log((1-self.kappa)*(1 - self.rho)*(1.0 - self.B) + self.rho))
+        self.phi = contract("ij,ijk->ijk", self.X, multinomial_parameter)
+
+        # phi_tilde update
+        theta_prods = contract("ik,jl->ijkl", self.theta, self.theta)
+        log_term2 = contract(
+            "ij,ij,kl->ijkl",
+            self.A,
+            self.weights,
+            np.log((1 - self.kappa) * self.B + self.kappa),
+        )
+        log_term2[~np.isfinite(log_term2)] = 0  # A should be 0 anyways, so
+        log_term3 = contract(
+            "ij,kl->ijkl",
+            self.A1m,
+            np.log((1 - self.kappa) * (1 - self.rho) * (1.0 - self.B) + self.rho),
+        )
         log_term3[~np.isfinite(log_term3)] = 0
         log_term4 = log_term2 + log_term3
-        theta_prods = theta_prods*np.exp(log_term4)
-        self.phi_tilde = theta_prods/(theta_prods.sum(axis = (2,3), keepdims = True)+self.EPS)
+        theta_prods = theta_prods * np.exp(log_term4)
+        self.phi_tilde = theta_prods / (
+            theta_prods.sum(axis=(2, 3), keepdims=True) + self.EPS
+        )
         self.phi_tilde[~np.isfinite(self.phi_tilde)] = 0
         for j in range(self.p):
-            self.phi_tilde[j,j,:,:] = np.zeros((self.K,self.K))
-        
+            self.phi_tilde[j, j, :, :] = np.zeros((self.K, self.K))
+
         return
-           
+
     def update_theta_newton(self):
         """
         Runs one step of a simplex constrained newton raphson algorithm to update theta
         """
         """
         evidence = self.phi.sum(axis = 0) + self.lam*(self.phi_tilde.sum(axis = (1,3)) + self.phi_tilde.sum(axis = (0,2))) # P x K
         grad_ = evidence/(self.theta + self.EPS) + (self.g + self.delta).reshape(-1,1)*(self.alpha.sum(axis = 0).reshape(1,-1))  #analytic gradient
@@ -968,112 +1200,144 @@
         #h_inv[~np.isfinite(h_inv)] = 0
         lagrange_multiplier = -1.0*gh_inv/(h_inv + self.EPS)#enforces simplex constraint
         #lagrange_multiplier[~np.isfinite(lagrange_multiplier)] = 0
         theta = self.theta - inverse_hessian*(lagrange_multiplier.reshape(-1,1) + grad_)
         self.theta = theta
         self.theta = self.theta/self.theta.sum(axis = 1, keepdims = True) #ensure sum to 1 constraint. - without numerical error does nothing
         """
-        
-        evidence = self.phi.sum(axis = 0) + self.lam*(self.phi_tilde.sum(axis = (1,3)) + self.phi_tilde.sum(axis = (0,2))) # P x K
-        inverse_hessian = -1.0*(self.theta**2)/(evidence + self.EPS)#analytic second derivative
-        inverse_hessian[~np.isfinite(inverse_hessian)] = 0 # control instability
-        gh = -1.0*(self.theta - (self.theta**2)/evidence*(self.g + self.delta).reshape(-1,1)*(self.alpha.sum(axis = 0).reshape(1,-1)))
-        gh[~np.isfinite(gh)] = 0 #control instability
-        gh_inv = gh.sum(axis = 1)
-        h_inv = inverse_hessian.sum(axis = 1)
-        lagrange_multiplier = -1.0*gh_inv/(h_inv + self.EPS)#enforces simplex constraint
-        theta = self.theta - inverse_hessian*lagrange_multiplier.reshape(-1,1) - gh
+
+        evidence = self.phi.sum(axis=0) + self.lam * (
+            self.phi_tilde.sum(axis=(1, 3)) + self.phi_tilde.sum(axis=(0, 2))
+        )  # P x K
+        inverse_hessian = (
+            -1.0 * (self.theta**2) / (evidence + self.EPS)
+        )  # analytic second derivative
+        inverse_hessian[~np.isfinite(inverse_hessian)] = 0  # control instability
+        gh = -1.0 * (
+            self.theta
+            - (self.theta**2)
+            / evidence
+            * (self.g + self.delta).reshape(-1, 1)
+            * (self.alpha.sum(axis=0).reshape(1, -1))
+        )
+        gh[~np.isfinite(gh)] = 0  # control instability
+        gh_inv = gh.sum(axis=1)
+        h_inv = inverse_hessian.sum(axis=1)
+        lagrange_multiplier = (
+            -1.0 * gh_inv / (h_inv + self.EPS)
+        )  # enforces simplex constraint
+        theta = self.theta - inverse_hessian * lagrange_multiplier.reshape(-1, 1) - gh
         self.theta = theta
-        self.theta[self.theta <0] = 0.0
-        self.theta = self.theta/self.theta.sum(axis = 1, keepdims = True) #ensure sum to 1 constraint. - without numerical error does nothing
+        self.theta[self.theta < 0] = 0.0
+        self.theta = self.theta / self.theta.sum(
+            axis=1, keepdims=True
+        )  # ensure sum to 1 constraint. - without numerical error does nothing
         return
-    
+
     def update_B(self):
         """
         last step must truncate for constraints
         """
-        evidence_num = contract('ijkl,ij,ij->kl',self.phi_tilde,self.weights,self.A)
-        evidence_denom = contract('ijkl,ij->kl',self.phi_tilde, self.A1m)
-        #evidence = evidence_num/(evidence_denom + self.EPS)
-        #evidence[~np.isfinite(evidence)] = 0
-        self.B = ((self.rho/(1.0-self.rho) + 1.0 - self.kappa)*evidence_num - self.kappa*evidence_denom)/((1.0-self.kappa)*(evidence_num+ evidence_denom) + self.EPS)
+        evidence_num = contract("ijkl,ij,ij->kl", self.phi_tilde, self.weights, self.A)
+        evidence_denom = contract("ijkl,ij->kl", self.phi_tilde, self.A1m)
+        # evidence = evidence_num/(evidence_denom + self.EPS)
+        # evidence[~np.isfinite(evidence)] = 0
+        self.B = (
+            (self.rho / (1.0 - self.rho) + 1.0 - self.kappa) * evidence_num
+            - self.kappa * evidence_denom
+        ) / ((1.0 - self.kappa) * (evidence_num + evidence_denom) + self.EPS)
         self.B[~np.isfinite(self.B)] = 0
         self.B[self.B > 1] = 1.0
         self.B[self.B < 0] = 0.0
         return
-    
+
     def update_g(self):
         """
         last step must truncate for constraints
         """
-        
-        num_ = self.phi.sum(axis = (0,2)) # P  
-        denom_ = contract('ik,jk->j',self.alpha, self.theta) #P 
-        self.g = num_/(denom_ + self.EPS) - self.delta
-        #self.g[~np.isfinite(self.g)] = 0
-        #enforce constraints - strictly convex--> suffices to truncate 
+
+        num_ = self.phi.sum(axis=(0, 2))  # P
+        denom_ = contract("ik,jk->j", self.alpha, self.theta)  # P
+        self.g = num_ / (denom_ + self.EPS) - self.delta
+        # self.g[~np.isfinite(self.g)] = 0
+        # enforce constraints - strictly convex--> suffices to truncate
         self.g[self.g > 1] = 1.0
         self.g[self.g < 0] = 0.0
         return
-    
+
     def update_alpha(self):
-        num_ = self.phi.sum(axis = 1) # N x K 
-        denom_ = contract('jk,j->k' , self.theta, self.g + self.delta).reshape(1,-1) # 1 x K 
-        self.alpha = num_/(denom_ +self.EPS)# N x K
-        #self.alpha[~np.isfinite(self.alpha)] = 0
+        num_ = self.phi.sum(axis=1)  # N x K
+        denom_ = contract("jk,j->k", self.theta, self.g + self.delta).reshape(
+            1, -1
+        )  # 1 x K
+        self.alpha = num_ / (denom_ + self.EPS)  # N x K
+        # self.alpha[~np.isfinite(self.alpha)] = 0
         return
-    
+
     def NLL(self):
-        recon = contract('ik,jk,j->ij', self.alpha, self.theta,self.g + self.delta) 
-        term1 = -1.0*(xlogy(self.X, recon) - recon).sum()
-        mat = contract('il,lj,kj->ik',self.theta,self.B,self.theta) 
-        term2 = -1.0*(np.log((1.0 -self.kappa)*mat + self.kappa)*self.A*self.weights).sum()
-        term3 = -1.0*(np.log((1.0 -self.kappa)*(1.0 - self.rho)*(1.0 - mat) + self.rho)*self.A1m).sum()
-        return term1 + self.lam*(term2 + term3)
-    
-    def fit(self, n_epochs = 10000, thres = 1, suppress = True):
+        recon = contract("ik,jk,j->ij", self.alpha, self.theta, self.g + self.delta)
+        term1 = -1.0 * (xlogy(self.X, recon) - recon).sum()
+        mat = contract("il,lj,kj->ik", self.theta, self.B, self.theta)
+        term2 = (
+            -1.0
+            * (
+                np.log((1.0 - self.kappa) * mat + self.kappa) * self.A * self.weights
+            ).sum()
+        )
+        term3 = (
+            -1.0
+            * (
+                np.log((1.0 - self.kappa) * (1.0 - self.rho) * (1.0 - mat) + self.rho)
+                * self.A1m
+            ).sum()
+        )
+        return term1 + self.lam * (term2 + term3)
+
+    def fit(self, n_epochs=10000, thres=1, suppress=True):
         """
         must run E step first
         """
         prev_nll = np.inf
         for t in range(n_epochs):
-            #print("E_step")
+            # print("E_step")
             self.E_step()
-            #print("M_step")
+            # print("M_step")
             self.M_step()
-            #print(model.B.max())
-            
+            # print(model.B.max())
+
             if t % 1 == 0:
                 nll = self.NLL()
                 if not suppress:
                     print("NLL: ", round(nll, 3))
                 if prev_nll - nll < thres:
                     return
                 else:
                     prev_nll = nll
         return
 
-    def initialize(self,gene_sets, val = 10):
-        ct = 0 
+    def initialize(self, gene_sets, val=10):
+        ct = 0
         for gene_set in gene_sets:
             self.theta[np.array(gene_set), ct] = val
-            self.B[ct,ct] = 1.0
+            self.B[ct, ct] = 1.0
             ct = ct + 1
 
-        self.theta = self.theta/(self.theta.sum(axis = 1, keepdims = True))
+        self.theta = self.theta / (self.theta.sum(axis=1, keepdims=True))
 
     def markers(self, offset, id2gene, n_top):
-        #compute marker weights
-        marker_weights = self.theta*(self.g + self.delta).reshape(-1,1) + offset
-        marker_weights = marker_weights/marker_weights.sum(axis = 1, keepdims = True) 
+        # compute marker weights
+        marker_weights = self.theta * (self.g + self.delta).reshape(-1, 1) + offset
+        marker_weights = marker_weights / marker_weights.sum(axis=1, keepdims=True)
 
-        #print genes per factors
+        # print genes per factors
         df = pd.DataFrame()
         for j in range(self.K):
-            df["factor" + str(j)] = [id2gene[i] for i in np.argsort(marker_weights[:,j])[::-1][:n_top]]
+            df["factor" + str(j)] = [
+                id2gene[i] for i in np.argsort(marker_weights[:, j])[::-1][:n_top]
+            ]
         return df
 
 
 """ 
 Public Functions 
 
 
@@ -1084,102 +1348,127 @@
     graph_network():  
 
     markers
 
 
 """
 
+
 def get_factor_celltypes(adata, obs_key, cellscore):
-    '''
+    """
     Assigns Spectra factors to cell types by analyzing the factor cell scores.
     Cell type specific factors will have zero cell scores except in their respective cell type
-    
+
     adata: AnnData , object containing the Spectra output
     obs_key: str , column name in adata.obs containing the cell type annotations
     cellscore_obsm_key: str , key for adata.obsm containing the Spectra cell scores
-    
+
     returns: dict , dictionary of {factor index : 'cell type'}
-    '''
-    
-    #get cellscores
+    """
+
+    # get cellscores
     cell_scores_df = pd.DataFrame(cellscore)
-    cell_scores_df['celltype'] = list(adata.obs[obs_key])
-    
-    #find global and cell type specific fators
-    global_factors_series = (cell_scores_df.groupby('celltype').mean() !=0).all()
-    global_factors = [factor for factor in global_factors_series.index if global_factors_series[factor]]
+    cell_scores_df["celltype"] = list(adata.obs[obs_key])
+
+    # find global and cell type specific fators
+    global_factors_series = (cell_scores_df.groupby("celltype").mean() != 0).all()
+    global_factors = [
+        factor
+        for factor in global_factors_series.index
+        if global_factors_series[factor]
+    ]
 
     specific_factors = {}
-    if len(global_factors) != (len(cell_scores_df.columns)-1):
-        specific_cell_scores = (cell_scores_df.groupby('celltype').mean()).T[~global_factors_series].T
-    
-    
-        for i in set(cell_scores_df['celltype']):
-            specific_factors[i]=[factor for factor in specific_cell_scores.loc[i].index if specific_cell_scores.loc[i,factor]]
-    
-        #inverse dict factor:celltype
+    if len(global_factors) != (len(cell_scores_df.columns) - 1):
+        specific_cell_scores = (
+            (cell_scores_df.groupby("celltype").mean()).T[~global_factors_series].T
+        )
+
+        for i in set(cell_scores_df["celltype"]):
+            specific_factors[i] = [
+                factor
+                for factor in specific_cell_scores.loc[i].index
+                if specific_cell_scores.loc[i, factor]
+            ]
+
+        # inverse dict factor:celltype
         factors_inv = {}
-        for i,v in specific_factors.items():
+        for i, v in specific_factors.items():
             for factor in v:
-                factors_inv[factor]=i
-    
-        #add global
+                factors_inv[factor] = i
+
+        # add global
 
         for factor in global_factors:
-            factors_inv[factor]= 'global'
-                
-        
-    
+            factors_inv[factor] = "global"
+
     else:
         factors_inv = {}
         for factor in global_factors:
-            factors_inv[factor]= 'global'
-    
+            factors_inv[factor] = "global"
+
     return factors_inv
 
 
+def est_spectra(
+    adata,
+    gene_set_dictionary,
+    L=None,
+    use_highly_variable=True,
+    cell_type_key="cell_type_annotations",
+    use_weights=True,
+    lam=0.01,
+    delta=0.001,
+    kappa=None,
+    rho=0.001,
+    use_cell_types=True,
+    n_top_vals=50,
+    filter_sets=True,
+    label_factors=True,
+    clean_gs=True,
+    min_gs_num=3,
+    overlap_threshold=0.2,
+    **kwargs,
+):
+    """
 
-def est_spectra(adata, gene_set_dictionary, L = None,use_highly_variable = True, cell_type_key = None, use_weights = True, lam = 0.01, delta=0.001,kappa = None, rho = 0.001, use_cell_types = True, n_top_vals = 50, 
-filter_sets = True, label_factors=True, clean_gs = True, min_gs_num = 3, overlap_threshold= 0.2, **kwargs):
-    """ 
-    
     Parameters
         ----------
-        adata : AnnData object 
+        adata : AnnData object
             containing cell_type_key with log count data stored in .X
-        gene_set_dictionary : dict or OrderedDict() 
-            maps cell types to gene set names to gene sets ; if use_cell_types == False then maps gene set names to gene sets ; 
+        gene_set_dictionary : dict or OrderedDict()
+            maps cell types to gene set names to gene sets ; if use_cell_types == False then maps gene set names to gene sets ;
             must contain "global" key in addition to every unique cell type under .obs.<cell_type_key>
         L : dict, OrderedDict(), int , NoneType
             number of factors per cell type ; if use_cell_types == False then int. Else dictionary. If None then match factors
-            to number of gene sets (recommended) 
-        use_highly_variable : bool 
+            to number of gene sets (recommended)
+        use_highly_variable : bool
             if True, then uses highly_variable_genes
         cell_type_key : str
             cell type key, must be under adata.obs.<cell_type_key> . If use_cell_types == False, this is ignored
         use_weights : bool
             if True, edge weights are estimated based on graph structure and used throughout training
-        lam : float 
+        lam : float
             lambda parameter of the model. weighs relative contribution of graph and expression loss functions
         delta : float
             delta parameter of the model. lower bounds possible gene scaling factors so that maximum ratio of gene scalings
-            cannot be too large 
+            cannot be too large
         kappa : float or None
             if None, estimate background rate of 1s in the graph from data
-        rho : float or None 
+        rho : float or None
             if None, estimate background rate of 0s in the graph from data
         use_cell_types : bool
             if True then cell type label is used to fit cell type specific factors. If false then cell types are ignored
         n_top_vals : int
             number of top markers to return in markers dataframe
-        determinant_penalty : float 
+        determinant_penalty : float
             determinant penalty of the attention mechanism. If set higher than 0 then sparse solutions of the attention weights
-            and diverse attention weights are encouraged. However, tuning is crucial as setting too high reduces the selection 
+            and diverse attention weights are encouraged. However, tuning is crucial as setting too high reduces the selection
             accuracy because convergence to a hard selection occurs early during training [todo: annealing strategy]
-        filter_sets : bool 
+        filter_sets : bool
             whether to filter the gene sets based on coherence
         label_factors : bool
             whether to label the factors by their cell type specificity and their overlap coefficient with the input marker genes
         clean_gs : bool
             if True cleans up the gene set dictionary to:
                 1. checks that annotations dictionary cell type keys and adata cell types are identical.
                 2. to contain only genes contained in the adata
@@ -1188,283 +1477,355 @@
             only use if clean_gs True, minimum number of genes per gene set expressed in adata, other gene sets will be filtered out
         overlap_threshold: float
             minimum overlap coefficient to assign an input gene set label to a factor
 
         **kwargs : (num_epochs = 10000, lr_schedule = [...], verbose = False)
             arguments to .train(), maximum number of training epochs, learning rate schedule and whether to print changes in
             learning rate
-            
+
      Returns: SPECTRA_Model object [after training]
-     
-     In place: adds 1. factors, 2. cell scores, 3. vocabulary, 4. markers, 5. overlap coefficient of markers vs input gene sets as attributes in .obsm, .var, .uns   
 
-    
+     In place: adds 1. factors, 2. cell scores, 3. vocabulary, 4. markers, 5. overlap coefficient of markers vs input gene sets as attributes in .obsm, .var, .uns
+
+
     """
-    
-    #filter gene set dictionary
+
+    # filter gene set dictionary
     if clean_gs:
-        gene_set_dictionary = Spectra_util.check_gene_set_dictionary(adata, gene_set_dictionary, obs_key=cell_type_key,global_key='global', return_dict = True, min_len=min_gs_num,use_cell_types=use_cell_types)
+        gene_set_dictionary = Spectra_util.check_gene_set_dictionary(
+            adata,
+            gene_set_dictionary,
+            obs_key=cell_type_key,
+            global_key="global",
+            return_dict=True,
+            min_len=min_gs_num,
+            use_cell_types=use_cell_types,
+        )
     if L == None:
         init_flag = True
         if use_cell_types:
             L = {}
-            for key in gene_set_dictionary.keys(): 
+            for key in gene_set_dictionary.keys():
                 length = len(list(gene_set_dictionary[key].values()))
-                L[key] = length + 1 
+                L[key] = length + 1
         else:
             length = len(list(gene_set_dictionary.values()))
             L = length + 1
-    #create vocab list from gene_set_dictionary
+    # create vocab list from gene_set_dictionary
     lst = []
     if use_cell_types:
         for key in gene_set_dictionary:
             for key2 in gene_set_dictionary[key]:
-                gene_list = gene_set_dictionary[key][key2] 
+                gene_list = gene_set_dictionary[key][key2]
                 lst += gene_list
     else:
         for key in gene_set_dictionary:
             gene_list = gene_set_dictionary[key]
             lst += gene_list
 
-    #lst contains all of the genes that are in the gene sets --> convert to boolean array 
-    bools = [] 
+    # lst contains all of the genes that are in the gene sets --> convert to boolean array
+    bools = []
     for gene in adata.var_names:
         if gene in lst:
             bools.append(True)
-        else: 
+        else:
             bools.append(False)
     bools = np.array(bools)
 
     if use_highly_variable:
-        idx_to_use = bools | adata.var.highly_variable #take union of highly variable and gene set genes (todo: add option to change this at some point)
-        X = adata.X[:,idx_to_use] 
+        idx_to_use = (
+            bools | adata.var.highly_variable
+        )  # take union of highly variable and gene set genes (todo: add option to change this at some point)
+        X = adata.X[:, idx_to_use]
         vocab = adata.var_names[idx_to_use]
         adata.var["spectra_vocab"] = idx_to_use
-    else: 
+    else:
         X = adata.X
-        vocab = adata.var_names 
-    
+        vocab = adata.var_names
+
     if use_cell_types:
         labels = adata.obs[cell_type_key].values
         for label in np.unique(labels):
             if label not in gene_set_dictionary:
                 gene_set_dictionary[label] = {}
             if label not in L:
-                L[label] = 1 
+                L[label] = 1
     else:
-        labels = None 
+        labels = None
     if type(X) == scipy.sparse.csr.csr_matrix:
         X = np.array(X.todense())
     word2id = dict((v, idx) for idx, v in enumerate(vocab))
     id2word = dict((idx, v) for idx, v in enumerate(vocab))
-    
+
     if filter_sets:
         if use_cell_types:
             new_gs_dict = {}
-            init_scores = compute_init_scores(gene_set_dictionary,word2id, torch.Tensor(X))
+            init_scores = compute_init_scores(
+                gene_set_dictionary, word2id, torch.Tensor(X)
+            )
             for ct in gene_set_dictionary.keys():
                 new_gs_dict[ct] = {}
-                mval = max(L[ct] - 1, 0) 
-                sorted_init_scores = sorted(init_scores[ct].items(), key=lambda x:x[1])
-                sorted_init_scores = sorted_init_scores[-1*mval:]
-                names = set([k[0] for k in sorted_init_scores]) 
+                mval = max(L[ct] - 1, 0)
+                sorted_init_scores = sorted(init_scores[ct].items(), key=lambda x: x[1])
+                sorted_init_scores = sorted_init_scores[-1 * mval :]
+                names = set([k[0] for k in sorted_init_scores])
                 for key in gene_set_dictionary[ct].keys():
                     if key in names:
                         new_gs_dict[ct][key] = gene_set_dictionary[ct][key]
         else:
-            init_scores = compute_init_scores_noct(gene_set_dictionary, word2id, torch.Tensor(X))
+            init_scores = compute_init_scores_noct(
+                gene_set_dictionary, word2id, torch.Tensor(X)
+            )
             new_gs_dict = {}
-            mval = max(L - 1, 0) 
-            sorted_init_scores = sorted(init_scores.items(), key=lambda x:x[1])
-            sorted_init_scores = sorted_init_scores[-1*mval:]
+            mval = max(L - 1, 0)
+            sorted_init_scores = sorted(init_scores.items(), key=lambda x: x[1])
+            sorted_init_scores = sorted_init_scores[-1 * mval :]
             names = set([k[0] for k in sorted_init_scores])
             for key in gene_set_dictionary.keys():
                 if key in names:
                     new_gs_dict[key] = gene_set_dictionary[key]
         gene_set_dictionary = new_gs_dict
     else:
         init_scores = None
-   
-    spectra = SPECTRA_Model(X = X, labels = labels,  L = L, vocab = vocab, gs_dict = gene_set_dictionary, use_weights = use_weights, lam = lam, delta=delta,kappa = kappa, rho = rho, use_cell_types = use_cell_types)
-    
+
+    spectra = SPECTRA_Model(
+        X=X,
+        labels=labels,
+        L=L,
+        vocab=vocab,
+        gs_dict=gene_set_dictionary,
+        use_weights=use_weights,
+        lam=lam,
+        delta=delta,
+        kappa=kappa,
+        rho=rho,
+        use_cell_types=use_cell_types,
+    )
+
     spectra.initialize(gene_set_dictionary, word2id, X, init_scores)
 
-    spectra.train(X = X, labels = labels,**kwargs)
+    spectra.train(X=X, labels=labels, **kwargs)
 
     adata.uns["SPECTRA_factors"] = spectra.factors
-    adata.uns["SPECTRA_markers"] = return_markers(factor_matrix = spectra.factors, id2word = id2word, n_top_vals = n_top_vals)
+    adata.uns["SPECTRA_markers"] = return_markers(
+        factor_matrix=spectra.factors, id2word=id2word, n_top_vals=n_top_vals
+    )
     adata.uns["SPECTRA_L"] = L
 
-    #label factors
+    # label factors
 
-    #transform input nested dictionary into a flat dictionary
+    # transform input nested dictionary into a flat dictionary
     gene_set_dictionary_flat = {}
 
-    for k,v in gene_set_dictionary.items():
-        if isinstance(v,dict):
-            for k2,v2 in v.items():
+    for k, v in gene_set_dictionary.items():
+        if isinstance(v, dict):
+            for k2, v2 in v.items():
                 gene_set_dictionary_flat[k2] = v2
             is_global = False
         else:
             gene_set_dictionary_flat[k] = v
             is_global = True
 
-    #labeling function
+    # labeling function
     if label_factors:
-        #get cell type specificity of every factor
+        # get cell type specificity of every factor
         if is_global == False:
-            celltype_dict = get_factor_celltypes(adata, cell_type_key, cellscore=spectra.cell_scores)
-            max_celltype = [celltype_dict[x] for x in range(spectra.cell_scores.shape[1])]
+            celltype_dict = get_factor_celltypes(
+                adata, cell_type_key, cellscore=spectra.cell_scores
+            )
+            max_celltype = [
+                celltype_dict[x] for x in range(spectra.cell_scores.shape[1])
+            ]
         else:
-            max_celltype = ['global']*(spectra.cell_scores.shape[1])
-        #get gene set with maximum overlap coefficient with top marker genes
-        overlap_df  = Spectra_util.label_marker_genes(adata.uns["SPECTRA_markers"] , gene_set_dictionary_flat, threshold = overlap_threshold)
+            max_celltype = ["global"] * (spectra.cell_scores.shape[1])
+        # get gene set with maximum overlap coefficient with top marker genes
+        overlap_df = Spectra_util.label_marker_genes(
+            adata.uns["SPECTRA_markers"],
+            gene_set_dictionary_flat,
+            threshold=overlap_threshold,
+        )
 
-        #create new column labels
+        # create new column labels
         column_labels = []
         for i in range(len(spectra.cell_scores.T)):
-            column_labels.append(str(i) + '-X-' + str(max_celltype[i]) + '-X-' + str(list(overlap_df.index)[i]))
+            column_labels.append(
+                str(i)
+                + "-X-"
+                + str(max_celltype[i])
+                + "-X-"
+                + str(list(overlap_df.index)[i])
+            )
 
         overlap_df.index = column_labels
         adata.uns["SPECTRA_overlap"] = overlap_df
-    
+
     adata.obsm["SPECTRA_cell_scores"] = spectra.cell_scores
 
-    
     return spectra
 
-def return_markers(factor_matrix, id2word,n_top_vals = 100):
-    idx_matrix = np.argsort(factor_matrix,axis = 1)[:,::-1][:,:n_top_vals]
+
+def return_markers(factor_matrix, id2word, n_top_vals=100):
+    idx_matrix = np.argsort(factor_matrix, axis=1)[:, ::-1][:, :n_top_vals]
     df = pd.DataFrame(np.zeros(idx_matrix.shape))
     for i in range(idx_matrix.shape[0]):
         for j in range(idx_matrix.shape[1]):
-            df.iloc[i,j] = id2word[idx_matrix[i,j]]
+            df.iloc[i, j] = id2word[idx_matrix[i, j]]
     return df.values
 
+
 def load_from_pickle(fp, adata, gs_dict, cell_type_key):
-    model = SPECTRA_Model(X = adata[:,adata.var["spectra_vocab"]].X, labels = np.array(adata.obs[cell_type_key]),  L = adata.uns["SPECTRA_L"], 
-                          vocab = adata.var_names[adata.var["spectra_vocab"]], gs_dict = gs_dict)
-    model.load(fp, labels = np.array(adata.obs[cell_type_key]))
-    return(model)
+    model = SPECTRA_Model(
+        X=adata[:, adata.var["spectra_vocab"]].X,
+        labels=np.array(adata.obs[cell_type_key]),
+        L=adata.uns["SPECTRA_L"],
+        vocab=adata.var_names[adata.var["spectra_vocab"]],
+        gs_dict=gs_dict,
+    )
+    model.load(fp, labels=np.array(adata.obs[cell_type_key]))
+    return model
+
+
+def graph_network(adata, mat, gene_set, thres=0.20, N=50):
 
-def graph_network(adata, mat, gene_set,thres = 0.20, N = 50):
-    
     vocab = adata.var_names[adata.var["spectra_vocab"]]
     word2id = dict((v, idx) for idx, v in enumerate(vocab))
     id2word = dict((idx, v) for idx, v in enumerate(vocab))
-    
-    net = Network(height='750px', width='100%', bgcolor='#FFFFFF', font_color='black', notebook = True)
+
+    net = Network(
+        height="750px",
+        width="100%",
+        bgcolor="#FFFFFF",
+        font_color="black",
+        notebook=True,
+    )
     net.barnes_hut()
-    
+
     idxs = []
     for term in gene_set:
         idxs.append(word2id[term])
-    ests = list(set(list(mat[idxs,:].sum(axis = 0).argsort()[::-1][:N]) + idxs))
+    ests = list(set(list(mat[idxs, :].sum(axis=0).argsort()[::-1][:N]) + idxs))
     ests_names = []
-    count = 0 
+    count = 0
     for est in ests:
         ests_names.append(id2word[est])
         if est not in idxs:
-            net.add_node(count, label = id2word[est], color = '#00ff1e')
+            net.add_node(count, label=id2word[est], color="#00ff1e")
         else:
-            net.add_node(count, label = id2word[est], color = '#162347')
+            net.add_node(count, label=id2word[est], color="#162347")
         count += 1
-        
-    inferred_mat = mat[ests,:][:,ests]
+
+    inferred_mat = mat[ests, :][:, ests]
     for i in range(len(inferred_mat)):
-        for j in range(i+1, len(inferred_mat)):
-            if inferred_mat[i,j] > thres:
+        for j in range(i + 1, len(inferred_mat)):
+            if inferred_mat[i, j] > thres:
                 net.add_edge(i, j)
     neighbor_map = net.get_adj_list()
     for node in net.nodes:
-        node['value'] = len(neighbor_map[node['id']])
+        node["value"] = len(neighbor_map[node["id"]])
 
     return net
 
-def graph_network_multiple(adata, mat, gene_sets,thres = 0.20, N = 50):
+
+def graph_network_multiple(adata, mat, gene_sets, thres=0.20, N=50):
     gene_set = []
     for gs in gene_sets:
         gene_set += gs
-        
+
     vocab = adata.var_names[adata.var["spectra_vocab"]]
     word2id = dict((v, idx) for idx, v in enumerate(vocab))
     id2word = dict((idx, v) for idx, v in enumerate(vocab))
-    
-    net = Network(height='750px', width='100%', bgcolor='#FFFFFF', font_color='black', notebook = True)
+
+    net = Network(
+        height="750px",
+        width="100%",
+        bgcolor="#FFFFFF",
+        font_color="black",
+        notebook=True,
+    )
     net.barnes_hut()
     idxs = []
     for term in gene_set:
         idxs.append(word2id[term])
-    ests = list(set(list(mat[idxs,:].sum(axis = 0).argsort()[::-1][:N]) + idxs))
+    ests = list(set(list(mat[idxs, :].sum(axis=0).argsort()[::-1][:N]) + idxs))
     ests_names = []
-    count = 0 
-    
+    count = 0
+
     color_map = []
     for gene_set in gene_sets:
-        random_color = ["#"+''.join([random.choice('ABCDEF0123456789') for i in range(6)])]
+        random_color = [
+            "#" + "".join([random.choice("ABCDEF0123456789") for i in range(6)])
+        ]
         color_map.append(random_color[0])
-        
+
     for est in ests:
         ests_names.append(id2word[est])
         if est not in idxs:
-            net.add_node(count, label = id2word[est], color = '#00ff1e')
+            net.add_node(count, label=id2word[est], color="#00ff1e")
         else:
             for i in range(len(gene_sets)):
                 if id2word[est] in gene_sets[i]:
                     color = color_map[i]
                     break
-            net.add_node(count, label = id2word[est], color = color)
+            net.add_node(count, label=id2word[est], color=color)
         count += 1
-        
-    inferred_mat = mat[ests,:][:,ests]
+
+    inferred_mat = mat[ests, :][:, ests]
     for i in range(len(inferred_mat)):
-        for j in range(i+1, len(inferred_mat)):
-            if inferred_mat[i,j] > thres:
+        for j in range(i + 1, len(inferred_mat)):
+            if inferred_mat[i, j] > thres:
                 net.add_edge(i, j)
     neighbor_map = net.get_adj_list()
     for node in net.nodes:
-        node['value'] = len(neighbor_map[node['id']])
+        node["value"] = len(neighbor_map[node["id"]])
 
     return net
 
+
 def gene_set_graph(gene_sets):
     """
     input
     [
     ["a","b", ... ],
     ["b", "d"],
-    
-    ... 
+
+    ...
     ]
     """
-    
-    net = Network(height='750px', width='100%', bgcolor='#FFFFFF', font_color='black', notebook = True)
+
+    net = Network(
+        height="750px",
+        width="100%",
+        bgcolor="#FFFFFF",
+        font_color="black",
+        notebook=True,
+    )
     net.barnes_hut()
     count = 0
-    #create nodes
+    # create nodes
     genes = []
     for gene_set in gene_sets:
         genes += gene_set
-    
+
     color_map = []
     for gene_set in gene_sets:
-        random_color = ["#"+''.join([random.choice('ABCDEF0123456789') for i in range(6)])]
+        random_color = [
+            "#" + "".join([random.choice("ABCDEF0123456789") for i in range(6)])
+        ]
         color_map.append(random_color[0])
-        
-    for gene in genes:          
+
+    for gene in genes:
         for i in range(len(gene_sets)):
             if gene in gene_sets[i]:
                 color = color_map[i]
                 break
-        net.add_node(gene, label = gene, color = color)
+        net.add_node(gene, label=gene, color=color)
 
     for gene_set in gene_sets:
         for i in range(len(gene_set)):
-            for j in range(i+1, len(gene_set)):
+            for j in range(i + 1, len(gene_set)):
                 net.add_edge(gene_set[i], gene_set[j])
 
-        
     neighbor_map = net.get_adj_list()
     for node in net.nodes:
-        node['value'] = len(neighbor_map[node['id']])
+        node["value"] = len(neighbor_map[node["id"]])
 
     return net
```

### Comparing `scSpectra-0.1.0/Spectra/Spectra_attn.py` & `scspectra-0.2.0/src/Spectra/Spectra_gpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1158 +1,1270 @@
-import numpy as np 
+import numpy as np
 import torch
-from collections import OrderedDict 
+from collections import OrderedDict
 from opt_einsum import contract
 from scipy.special import logit
-from tqdm import tqdm 
+from tqdm import tqdm
 from scipy.special import xlogy
 from scipy.special import softmax
-from Spectra import Spectra_util 
+from Spectra import Spectra_util
 import torch.nn as nn
 import scipy
 import pandas as pd
 from pyvis.network import Network
 import random
 
 from torch.distributions.normal import Normal
 from torch.distributions.log_normal import LogNormal
 from torch.distributions.dirichlet import Dirichlet
 
+### Class for SPECTRA model
+from Spectra.initialization import *
 
-class SPECTRA_select(nn.Module): 
-    """ 
+print(
+    "Spectra GPU support is still under development. Raise any issues on github \n \n Changes from v1: \n (1) GPU support [see tutorial] \n (2) minibatching for local parameters and data \n Note that minibatching may affect optimization results \n Code will eventually be merged into spectra.py"
+)
+
+"""
+Changes from v1:
+
+(1) conversion of cell type loop to zero padded matrix multiplication
+(2) support for minibatching local parameters and data
+(3) GPU support 
+
+def batchify(to_batch, batch_size)
+    batches iterables -- helper function for minibatching 
+
+class SPECTRA(nn.Module)
+    new public attributes: 
+    ________________________
+    self.adj_matrix `(cell types + 1 , p, p )`- shaped torch.Tensor 
+    self.adj_matrix1m `(cell types + 1 , p, p )`- shaped torch.Tensor 
+    self.weights `(cell types + 1 , p, p )`- shaped torch.Tensor 
+    self.L_tot - int, total number of factors 
+    self.ct_order -  list, order of the cell types 
+    self.L_list - list of numbers of factors per cell type 
+    self.n_cell_typesp1 - number of cell types + 1 (global)
+    self.start_pos - dictionary {ct : start_pos in array}
+
+    Learnable parameters: 
+
+    self.theta - `(self.p, self.L_tot)`- shaped torch.Tensor 
+    self.eta - `(self.L_tot, self.L_tot)`- shaped torch.Tensor 
+    self.alpha - `(self.n, self.L_tot)`- shaped torch.Tensor [LOCAL: must be minibatched]
+    self.gene_scalings - `(self.n_cell_typesp1, self.p)`- shaped torch.Tensor
+
+    Masks: 
+
+    self.alpha_mask = `(self.n,self.L_tot)` - shaped torch.Tensor - binary mask that indicates relevant factors per cell [LOCAL: must be minibatched]
+    self.B_mask = `(self.n_cell_typesp1, self.L_tot, self.L_tot)` - shaped torch.Tensor - binary mask that retains submatrix corresponding to cell type 
+    self.factor_to_celltype = `(self.L_tot, self.n_cell_typesp1)`- shaped torch.Tensor - binary mask that contains which cell types correspond to which factors 
+
+
+    new private method: 
+    ________________________
+    __store_parameters(self, ...) : after model fitting, converts parameters to mimic format of old spectra so that wrappers are backwards compatible  -- entirely different implementation
     
+
+    
+
+
+
+To do list; 
+
+Implementation: 
+> re-read vectorization of cell type for loop -- add line by line comments - DONE 
+> store_parameters() ; should just get output of convert_params and run as normal  
+> initialization() ; this is kind of a nightmare - DONE
+> learning rate and penalty must be changed to account for batching - DONE 
+
+
+Testing: 
+> check outputs match when minibatch size is whole dataset
+> Behavior same when # gene sets 0 for a cell type 
+> Check that masks are correct for toy data
+
+Extensions: 
+> batch both cells and genes together (implement later) 
+        -- I'm wondering how severely the training dynamics are changed when gradients for local parameters are substantially noisier than global ones
+        -- to address this we could batch on both cells & genes 
+> support for use_cell_types == False
+"""
+
+
+# debugging
+import pdb
+
+
+def batchify(to_batch, batch_size):
+    """
+    batches all iterables in to_batch in same random permutation
+    """
+    M = to_batch[0].shape[0]
+    rand = torch.randperm(M)
+    for thing in to_batch:
+        thing = thing[rand]
+
+    i = 0
+    out = [[] for thing in to_batch]
+
+    while i + batch_size < M:
+        for j, thing in enumerate(to_batch):
+            out[j].append(thing[i : i + batch_size])
+        i += batch_size
+    for j, thing in enumerate(to_batch):
+        out[j].append(thing[i:])
+    return out
+
+
+class SPECTRA(nn.Module):
+    """
+
     Parameters
         ----------
         X : np.ndarray or torch.Tensor
             the ``(n, p)`` -shaped matrix containing logged expression count data. Used for initialization of self.n and self.p but not stored as an attribute
         labels : np.ndarray or NoneType
             the ``(n, )`` -shaped array containing cell type labels. If use_cell_types == False, then should be set to None
-        K : dict or OrderedDict [if use_cell_types == False then int]
-            ``number of cell types + 1`` -shaped dictionary. Must have "global" as a key, indicating the number of global factors 
-            { 
-                "global": 15,
-                 "CD8": 5, 
-            } 
-            > Note that K contains the number of factors that describe the expression data while L contains the number of factors that describe the graph. When K < L an additional parameter that projects the L graph factors down is initialized. When L < K the behavior is to set L to max(L,K)
+
         L : dict or OrderedDict [if use_cell_types == False, then int]
             ``number of cell types + 1``-shaped dictionary. Must have "global" as a key, indicating the number of global factors
             {
-                "global": 15, 
-                "CD8": 5 
-                ...    
+                "global": 15,
+                "CD8": 5
+                ...
             }
-            > Format matches output of K_est.py to estimate the number of 
+            > Format matches output of K_est.py to estimate the number of
             > Must match cell type labels provided during training
-            > Recommended practice is to assign at minimum 2 factors per cell type 
-            > Note that K contains the number of factors that describe the expression data while L contains the number of factors that describe the graph. When K < L an additional parameter that projects the L graph factors down is initialized. When L < K the behavior is to set L to max(L,K) 
+            > Recommended practice is to assign at minimum 2 factors per cell type
+            > Note that L contains the number of factors that describe the graph.
         adj_matrix :  dict or OrderedDict
-            ``a dictionary of adjacency matrices, one for every cell type + a "global" 
+            ``a dictionary of adjacency matrices, one for every cell type + a "global"
             {
                 "global": ``(p, p)``-shaped binary np.ndarray
-                "CD8": ... 
+                "CD8": ...
 
-            } 
+            }
         weights : dict or OrderedDict or NoneType [if use_cell_types == False, then ``(p, p)``-shaped array]
             the ``(p, p)``-shaped set of edge weights per . If weight[i,j] is non-zero when adj_matrix[i,j] = 0
-            this weight is ignored. 
-            
+            this weight is ignored.
+
             if weights == None, no weights are used
         lam : float
-            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information  
-        delta : float 
-            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes. 
+            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information
+        delta : float
+            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes.
         kappa : float or NoneType
-            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.  
+            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.
         rho : float or NoneType
-            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data. 
-        use_cell_types: bool 
+            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data.
+        use_cell_types: bool
             use_cell_types is a Boolean variable that determines whether cell type labels are used to fit the model. If False, then parameters are initialized as nn.Parameter rather than as nn.ParameterDict with cell type keys that index nn.Parameter values
-        determinant_penalty : float
-            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.  
+
     Attributes
         ----------
         model.delta : delta parameter of the model
 
-        model.lam : lambda parameter of the model 
-       
-        model.determinant_penalty : determinant penalty of the model 
-
-        model.K : K parameter, either int, dict, or OrderedDict() 
- 
-        model.L : L parameter, either int, dict or OrderedDict() 
+        model.lam : lambda parameter of the model
+
+
+        model.L : L parameter, either int, dict or OrderedDict()
 
         model.p : number of genes
 
-        model.n : number of cells 
+        model.n : number of cells
 
-        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters. 
+        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters.
 
         model.kappa : if not kappa, nn.ParameterDict() if use_cell_types, else nn.Parameter(). If kappa is a float, it is fixed throughout training
 
         model.rho : if not rho, nn.ParamterDict() if use_cell_types, else nn.Parameter. If rho is a float it is fixed throughout training
 
-        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors 
+        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.weights : contains edge weights. format matches adj_matrix
 
-        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors 
-        
-        model.weights : contains edge weights. format matches adj_matrix 
-        
         model.cell_types : np.ndarray containing array of unique cell types
-       
+
         model.cell_type_counts : dict {key = cell type, values = number of cells}
- 
-        model.theta : nn.ParameterDict() or nn.Parameter() containing the factor weights 
+
+        model.theta : nn.ParameterDict() or nn.Parameter() containing the factor weights
 
         model.alpha : nn.ParameterDict() or nn.Parameter() containing the cell loadings
 
         model.eta : nn.ParameterDict() or nn.Parameter() containing the interaction matrix between factors
 
         model.gene_scaling : nn.ParameterDict() or nn.Parameter() containing the gene scale factors
 
-        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False 
-        
+        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False
+
         model.kgeql_flag : dict or bool. dictionary of boolean values indicating whether K >= L.  When use_cell_types == False, it is a boolean value
 
     Methods
         ----------
 
         model.loss(self, X, labels) : called by fit if use_cell_types = True. Evalutes the loss of the model
 
-        model.loss_no_cell_types(self,X) : called by fit if use_cell_types = False. Evalutes the loss of the model 
-     
-        model.initialize(self, gene_sets,val) : initialize the model based on given dictionary of gene sets. val is a float that determines the strength of the initialization.
- 
-        model.initialize_no_celltypes(self, gs_list, val) : initialize the model based on given list of gene sets. val is a float that determines the strength of the initialization. 
+        model.loss_no_cell_types(self,X) : called by fit if use_cell_types = False. Evalutes the loss of the model
 
-        
-    To do: 
-        __________
+        model.initialize(self, gene_sets,val) : initialize the model based on given dictionary of gene sets. val is a float that determines the strength of the initialization.
 
-        > Alternative initialization functions 
+        model.initialize_no_celltypes(self, gs_list, val) : initialize the model based on given list of gene sets. val is a float that determines the strength of the initialization.
 
-        > comment SPECTRA-EM code
-        
-        > test lower bound constraint [see pyspade_global.py implementation]
 
-        > Overlap threshold test statistic
 
-    
     """
-    def __init__(self, X, labels, adj_matrix, K, L, weights = None, lam = 10e-4, delta=0.1,kappa = 0.00001, rho = 0.00001, use_cell_types = True, determinant_penalty = 0.0):
-        super(SPECTRA_select, self).__init__()
-
 
-        #hyperparameters
-        self.delta = delta 
-        self.lam = lam 
-        self.determinant_penalty = determinant_penalty
-        #L and K are potentially different now - we have a projection parameter whereever L > K
-        self.L = L 
-        self.K = K
-        #for memory efficiency we don't store X in the object attributes, but require X dimensions to be known at initialization
+    def __init__(
+        self,
+        X,
+        labels,
+        adj_matrix,
+        L,
+        weights=None,
+        lam=10e-4,
+        delta=0.1,
+        kappa=0.00001,
+        rho=0.00001,
+        use_cell_types=True,
+    ):
+        super(SPECTRA, self).__init__()
+
+        device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        # hyperparameters
+        self.delta = delta
+        self.lam = lam
+        self.L = L
+        # for memory efficiency we don't store X in the object attributes, but require X dimensions to be known at initialization
         self.p = X.shape[1]
         self.n = X.shape[0]
-        self.use_cell_types = use_cell_types 
-        
-        
-        
-
-        if not use_cell_types:
-            #check that L is an int
-            assert(isinstance(self.L, int))
-
-            # trust the user to input a np.ndarray for adj_matrix
-            self.adj_matrix = torch.Tensor(adj_matrix) - torch.Tensor(np.diag(np.diag(adj_matrix)))
-            adj_matrix_1m = 1.0 - adj_matrix
-            self.adj_matrix_1m = torch.Tensor(adj_matrix_1m - np.diag(np.diag(adj_matrix_1m)))
-            if weights is not None:
-                self.weights = torch.Tensor(weights) - torch.Tensor(np.diag(np.diag(adj_matrix)))
-            else:
-                self.weights = self.adj_matrix
-            
-            
-            if self.K >= self.L:  
-                self.theta = nn.Parameter(Normal(0.,1.).sample([self.p, self.K]))
-                self.eta = nn.Parameter(Normal(0.,1.).sample([self.K, self.K]))
-                self.kgeql_flag = True
-            else:
-                self.theta = nn.Parameter(Normal(0.,1.).sample([self.p, self.L]))
-                self.selection = nn.Parameter(Normal(0.,1.).sample([self.K, self.L]))
-                self.eta = nn.Parameter(Normal(0.,1.).sample([self.L, self.L]))
-                self.kgeql_flag = False
-                
-            self.alpha = nn.Parameter(Normal(0.,1.).sample([self.n, self.K]))
-            
-            self.gene_scaling = nn.Parameter(Normal(0.,1.).sample([self.p]))
-
-            if kappa == None:
-                self.kappa = nn.Parameter(Normal(0.,1.).sample())
-            else:
-                self.kappa = torch.tensor(np.log(kappa/(1- kappa))) #
-            if rho == None:
-                self.rho = nn.Parameter(Normal(0.,1.).sample())
-            else:
-                self.rho = torch.tensor(np.log(rho/(1-rho)))
-
+        self.use_cell_types = use_cell_types
 
-        if use_cell_types:
-            #convert adjacency matrices to pytorch tensors to make optimization easier later
-            self.adj_matrix = {cell_type: torch.Tensor(adj_matrix[cell_type]) - torch.Tensor(np.diag(np.diag(adj_matrix[cell_type]))) if len(adj_matrix[cell_type]) > 0 else [] for cell_type in adj_matrix.keys()}
-            #for convenience store 1 - adjacency matrix elements [except on diagonal, where we store 0]
-            adj_matrix_1m = {cell_type: 1.0 - adj_matrix[cell_type] if len(adj_matrix[cell_type]) > 0 else [] for cell_type in adj_matrix.keys()} #one adj_matrix per cell type 
-            self.adj_matrix_1m = {cell_type: torch.Tensor(adj_matrix_1m[cell_type] - np.diag(np.diag(adj_matrix_1m[cell_type]))) if len(adj_matrix_1m[cell_type]) > 0 else [] for cell_type in adj_matrix_1m.keys()} #one adj_matrix per cell type 
-            
-            #if weights are provided, convert these to tensors, else set weights = to adjacency matrices
-            if weights:
-                self.weights = {cell_type: torch.Tensor(weights[cell_type]) - torch.Tensor(np.diag(np.diag(weights[cell_type]))) if len(weights[cell_type]) > 0 else [] for cell_type in weights.keys()}
-            else:
-                self.weights = self.adj_matrix
+        print("Building parameter set...")
+        # we only have to do this once so for loop is ok
 
-            self.cell_types = np.unique(labels) #cell types are the unique labels, again require knowledge of labels at initialization but do not store them
-            
-            #store a dictionary containing the counts of each cell type
-            self.cell_type_counts = {}
-            for cell_type in self.cell_types:
-                n_c = sum(labels == cell_type)
-                self.cell_type_counts[cell_type] = n_c 
-            
-            #initialize parameters randomly, we use torch's ParameterDict() for storage for intuitive accessing cell type specific parameters
-            self.theta = nn.ParameterDict()
-            self.alpha = nn.ParameterDict()
-            self.eta = nn.ParameterDict()
-            self.gene_scaling = nn.ParameterDict()
-            self.selection = nn.ParameterDict()
-            self.kgeql_flag = {}
-            
-            
-            if kappa == None:
-                self.kappa = nn.ParameterDict()
-            if rho == None:
-                self.rho = nn.ParameterDict()
-            #initialize global params
-            
-            if self.K["global"] >= self.L["global"]:
-                self.kgeql_flag["global"] = True
-                self.theta["global"] = nn.Parameter(Normal(0.,1.).sample([self.p, self.K["global"]]))
-                self.eta["global"] = nn.Parameter(Normal(0.,1.).sample([self.K["global"], self.K["global"]]))
+        # here we are creating lists in place of the original input formats -- to be converted into 3-way tensors instead of dictionaries with a cell type axis
+        lst_adj_matrix = []
+        lst_adj_matrix1m = []
+        lst_weights = []
+        ct_order = []
+        L_tot = 0
+        L_list = []
+        self.start_pos = OrderedDict()
+
+        for cell_type in adj_matrix.keys():
+            ct_order.append(cell_type)
+            L_tot += L[cell_type]
+            L_list.append(L[cell_type])
+            if len(adj_matrix[cell_type]) > 0:
+                temp = torch.Tensor(adj_matrix[cell_type]) - torch.Tensor(
+                    np.diag(np.diag(adj_matrix[cell_type]))
+                )
+                lst_adj_matrix.append(temp)
+                lst_adj_matrix1m.append(1.0 - temp - torch.diag(torch.diag(1.0 - temp)))
             else:
-                self.kgeql_flag["global"] = False
-                self.theta["global"] = nn.Parameter(Normal(0.,1.).sample([self.p, self.L["global"]]))
-                self.selection["global"] = nn.Parameter(Normal(0.,1.).sample([self.K["global"], self.L["global"]]))
-                self.eta["global"] = nn.Parameter(Normal(0.,1.).sample([self.L["global"], self.L["global"]]))
-           
-            self.gene_scaling["global"] = nn.Parameter(Normal(0.,1.).sample([self.p]))
-            
-            if kappa == None:
-                self.kappa["global"] = nn.Parameter(Normal(0.,1.).sample())
-            if rho == None:
-                self.rho["global"] = nn.Parameter(Normal(0.,1.).sample())
-
-            #initialize all cell type specific params
-            for cell_type in self.cell_types:
-                
-                if self.K[cell_type] >= self.L[cell_type]:
-                    self.kgeql_flag[cell_type] = True
-                    self.theta[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.p, self.K[cell_type]]))
-                    self.eta[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.K[cell_type], self.K[cell_type]]))
+                lst_adj_matrix.append(torch.zeros((self.p, self.p)))
+                lst_adj_matrix1m.append(torch.zeros((self.p, self.p)))
+        self.adj_matrix = torch.stack(lst_adj_matrix).to(
+            device
+        )  # (cell_types + 1, p, p )
+        self.adj_matrix_1m = torch.stack(lst_adj_matrix1m).to(
+            device
+        )  # (cell_types + 1, p, p)
+
+        if weights:
+            for cell_type in ct_order:
+                if len(weights[cell_type]) > 0:
+                    lst_weights.append(
+                        torch.Tensor(weights[cell_type])
+                        - torch.Tensor(np.diag(np.diag(weights[cell_type])))
+                    )
                 else:
-                    self.kgeql_flag[cell_type] = False
-                    self.theta[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.p, self.L[cell_type]]))
-                    self.selection[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.K[cell_type], self.L[cell_type]]))
-                    self.eta[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.L[cell_type], self.L[cell_type]]))
-
-                n_c = sum(labels == cell_type)
-                self.alpha[cell_type] = nn.Parameter(Normal(0.,1.).sample([n_c, self.K["global"] + self.K[cell_type]]))
-                self.gene_scaling[cell_type] = nn.Parameter(Normal(0.,1.).sample([self.p]))
-                
-                if kappa == None:
-                    self.kappa[cell_type] = nn.Parameter(Normal(0.,1.).sample())
-
-                if rho == None:
-                    self.rho[cell_type] = nn.Parameter(Normal(0.,1.).sample())
-
-    
-            #if kappa and rho are provided, hold these fixed during training, else fit as free parameters
-            # to unify the cases, we put this in the same format
-            if kappa != None:
-                self.kappa = {}
-                self.kappa["global"] = torch.tensor(np.log(kappa/(1-kappa)))
-                for cell_type in self.cell_types:
-                    self.kappa[cell_type] = torch.tensor(np.log(kappa /(1-kappa)))
-            
-            if rho != None:
-                self.rho = {}
-                self.rho["global"] = torch.tensor(np.log(rho/(1-rho)))
-                for cell_type in self.cell_types:
-                    self.rho[cell_type] = torch.tensor(np.log(rho/(1-rho)))
-
-    
-    def loss(self, X, labels): 
-        assert(self.use_cell_types) #if this is False, fail because model has not been initialized to use cell types
-        
-        #convert inputs to torch.Tensors
-        X = torch.Tensor(X)
-        #labels = torch.Tensor(labels)
-
-        #initialize loss and fetch global parameters
-        loss = 0.0
-        theta_global = torch.softmax(self.theta["global"], dim = 1)
-        eta_global = (self.eta["global"]).exp()/(1.0 + (self.eta["global"]).exp())
-        eta_global = 0.5*(eta_global + eta_global.T)
-        gene_scaling_global = self.gene_scaling["global"].exp()/(1.0 + self.gene_scaling["global"].exp())
-        kappa_global = self.kappa["global"].exp()/(1 + self.kappa["global"].exp())
-        rho_global = self.rho["global"].exp()/(1 + self.rho["global"].exp())
-        
-        
-        if self.kgeql_flag["global"]:
-            theta_global_new = theta_global
+                    lst_weights.append(torch.zeros((self.p, self.p)))
         else:
-            selection_global = self.selection["global"].softmax(dim = 1)
-            theta_global_new = contract('ij,kj->ki',selection_global,theta_global)
-            loss = loss - self.determinant_penalty*torch.logdet(contract('ij,kj->ik',selection_global, selection_global))
-            
-        #loop through cell types and evaluate loss at every cell type
-        for cell_type in self.cell_types:
-            kappa = self.kappa[cell_type].exp()/(1 + self.kappa[cell_type].exp())
-            rho = self.rho[cell_type].exp()/(1 + self.rho[cell_type].exp())
-            gene_scaling_ct = self.gene_scaling[cell_type].exp()/(1.0 + self.gene_scaling[cell_type].exp())
-            X_c = X[labels == cell_type]
-            adj_matrix = self.adj_matrix[cell_type] 
-            weights = self.weights[cell_type]
-            adj_matrix_1m = self.adj_matrix_1m[cell_type]
-            theta_ct = torch.softmax(self.theta[cell_type], dim = 1)
-            eta_ct = (self.eta[cell_type]).exp()/(1.0 + (self.eta[cell_type]).exp())
-            eta_ct = 0.5*(eta_ct + eta_ct.T)
-            theta_global_ = contract('jk,j->jk',theta_global_new, gene_scaling_global + self.delta)
-            alpha = torch.exp(self.alpha[cell_type])
-            #recon = contract('ik,jk->ij', alpha, theta) 
-            #term1 = -1.0*(torch.xlogy(X_c,recon) - recon).sum()
-            
-            if self.kgeql_flag[cell_type]: 
-                theta_ct_ = contract('jk,j->jk',theta_ct, gene_scaling_ct + self.delta)
-                theta = torch.cat((theta_global_, theta_ct_),1)
-                recon = contract('ik,jk->ij', alpha, theta) 
-                term1 = -1.0*(torch.xlogy(X_c,recon) - recon).sum()
+            self.weights = self.adj_matrix
+        self.weights = torch.stack(lst_weights).to(device)
+        self.ct_order = ct_order
+        self.L_tot = L_tot
+        self.L_list = L_list
+        self.n_cell_typesp1 = len(ct_order)
+
+        # just need to construct these masks once
+        self.alpha_mask = torch.zeros((self.n, self.L_tot)).to(device)
+        self.B_mask = torch.zeros((self.n_cell_typesp1, self.L_tot, self.L_tot)).to(
+            device
+        )  # need to double check that this works
+        self.factor_to_celltype = torch.zeros((self.L_tot, self.n_cell_typesp1)).to(
+            device
+        )
+
+        self.theta = nn.Parameter(Normal(0.0, 1.0).sample([self.p, self.L_tot]))
+        self.eta = nn.Parameter(Normal(0.0, 1.0).sample([self.L_tot, self.L_tot]))
+        self.alpha = nn.Parameter(Normal(0.0, 1.0).sample([self.n, self.L_tot]))
+        self.gene_scalings = nn.Parameter(
+            Normal(0.0, 1.0).sample([self.n_cell_typesp1, self.p])
+        )
+
+        # need to add kappa and rho initilizations and figure out the masking for B and loadings and how to multiply the gene scalings by the factors -- create a one hot vector for cell type --> factor assignments to get
+        if kappa == None:
+            self.kappa = nn.Parameter(Normal(0.0, 1.0).sample([self.n_cell_typesp1]))
+        if rho == None:
+            self.rho = nn.Parameter(Normal(0.0, 1.0).sample([self.n_cell_typesp1]))
+        if kappa != None:
+            self.kappa = (
+                torch.ones((self.n_cell_typesp1))
+                * torch.tensor(np.log(kappa / (1 - kappa)))
+            ).to(device)
+        if rho != None:
+            self.rho = (
+                torch.ones((self.n_cell_typesp1))
+                * torch.tensor(np.log(rho / (1 - rho)))
+            ).to(device)
+
+        # make sure
+        if ct_order[0] != "global":
+            raise Exception("First key in ordered dict must be global")
+
+        counter = 0
+        counter_B = 0
+        for ct in ct_order:
+            self.start_pos[ct] = counter
+            if ct == "global":
+                self.alpha_mask[:, counter : counter + L[ct]] = 1.0
             else:
-                selection_ct = self.selection[cell_type].softmax(dim = 1)
-                theta_ct_new = contract('ij,kj->ki',selection_ct,theta_ct)
-                theta_ct_ = contract('jk,j->jk',theta_ct_new, gene_scaling_ct + self.delta)
-                theta = torch.cat((theta_global_, theta_ct_),1)
-                recon = contract('ik,jk->ij', alpha, theta) 
-                term1 = -1.0*(torch.xlogy(X_c,recon) - recon).sum() - self.determinant_penalty*torch.logdet(contract('ij,kj->ik',selection_ct, selection_ct))
-
-            
-            if len(adj_matrix) > 0:
-                mat = contract('il,lj,kj->ik',theta_ct,eta_ct,theta_ct) 
-                term2 = -1.0*(torch.xlogy(adj_matrix*weights, (1.0 - rho)*(1.0 -kappa)*mat + (1.0 - rho)*kappa)).sum()
-                term3 = -1.0*(torch.xlogy(adj_matrix_1m,(1.0 -kappa)*(1.0 - rho)*(1.0 - mat) + rho)).sum()
+                cells_mask = labels == ct
+                self.alpha_mask[cells_mask, counter : counter + L[ct]] = 1.0
+
+            self.B_mask[
+                counter_B, counter : counter + L[ct], counter : counter + L[ct]
+            ] = 1.0
+            self.factor_to_celltype[counter : counter + L[ct], counter_B] = 1.0
+            counter = counter + L[ct]
+            counter_B = counter_B + 1
+
+        # check that these masks are correct
+        self.cell_type_counts = []
+        for cell_type in ct_order:
+            if cell_type == "global":
+                self.cell_type_counts.append(self.n)
             else:
-                term2 = 0.0
-                term3 = 0.0
-            #the magnitude of lambda is proportional to the number of cells [todo: simpler to just take the mean instead of sum in term 1]
-            loss = loss + self.lam*term1 +(self.cell_type_counts[cell_type]/float(self.n))*(term2 + term3) 
-            
-        
-        #compute loss associated with global graph
-        adj_matrix = self.adj_matrix["global"] 
-        adj_matrix_1m = self.adj_matrix_1m["global"]
-        weights = self.weights["global"]
-        if len(adj_matrix) > 0:
-            mat = contract('il,lj,kj->ik',theta_global,eta_global,theta_global) 
-            term2 = -1.0*(torch.xlogy(adj_matrix*weights, (1.0 - rho_global)*(1.0 -kappa_global)*mat + (1.0 - rho_global)*kappa_global)).sum()
-            term3 = -1.0*(torch.xlogy(adj_matrix_1m, (1.0 -kappa_global)*(1.0 - rho_global)*(1.0 - mat) + rho_global)).sum()
-            loss = loss + term2 + term3 
+                n_c = sum(labels == cell_type)
+                # mimic behavior of old version: Tues Feb 21, 2023 <-- if there are no annotations we'll just set the whole loss to 0 by setting cell type counts to 0
+                if len(adj_matrix[cell_type]) > 0:
+                    self.cell_type_counts.append(n_c)
+                else:
+                    self.cell_type_counts.append(0)
+        self.cell_type_counts = np.array(self.cell_type_counts)
+        self.ct_vec = torch.Tensor(self.cell_type_counts / float(self.n)).to(device)
+
+    def loss(self, X, alpha_mask, alpha, batch_size):
+        device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        assert (
+            self.use_cell_types
+        )  # if this is False, fail because model has not been initialized to use cell types
+
+        # convert inputs to torch.Tensors
+        # X = torch.Tensor(X).to(device)
+        # alpha_mask = alpha_mask.to(device)
+        # creat the weird softmax theta
+        theta = torch.cat(
+            [
+                temp.softmax(dim=1)
+                for temp in torch.split(
+                    self.theta, split_size_or_sections=self.L_list, dim=1
+                )
+            ],
+            dim=1,
+        )
+        # initialize loss and fetch global parameters
+        eta = self.eta.exp() / (1.0 + (self.eta).exp())
+        eta = 0.5 * (eta + eta.T)
+        gene_scaling = self.gene_scalings.exp() / (
+            1.0 + self.gene_scalings.exp()
+        )  # ctp1 x p
+        kappa = self.kappa.exp() / (1 + self.kappa.exp())  # ctp1
+        rho = self.rho.exp() / (1 + self.rho.exp())  # ctp1
+        alpha = torch.exp(alpha)  # batch x L_tot
+        # handle theta x gene_scalings
+
+        gene_scaling_ = contract(
+            "ij,ki->jk", gene_scaling, self.factor_to_celltype
+        )  # p x L_tot
+        theta_ = theta * (gene_scaling_ + self.delta)  # p x L_tot
+        alpha_ = alpha * alpha_mask  # batch x L_tot
+        recon = contract("ik,jk->ij", alpha_, theta_)
+        term1 = -1.0 * (torch.xlogy(X, recon) - recon).sum()
+
+        eta_ = eta[None, :, :] * self.B_mask  # ctp1 x L_tot x L_tot
+
+        mat = contract("il,clj,kj->cik", theta_, eta_, theta_)  # ctp1 x p x p
+        term2 = (
+            -1.0
+            * (
+                (
+                    torch.xlogy(
+                        self.adj_matrix * self.weights,
+                        (1.0 - rho.reshape(-1, 1, 1))
+                        * (1.0 - kappa.reshape(-1, 1, 1))
+                        * mat
+                        + (1.0 - rho.reshape(-1, 1, 1)) * kappa.reshape(-1, 1, 1),
+                    )
+                )
+                * self.ct_vec.reshape(-1, 1, 1)
+            ).sum()
+        )
+        term3 = (
+            -1.0
+            * (
+                (
+                    torch.xlogy(
+                        self.adj_matrix_1m,
+                        (1.0 - kappa.reshape(-1, 1, 1))
+                        * (1.0 - rho.reshape(-1, 1, 1))
+                        * (1.0 - mat)
+                        + rho.reshape(-1, 1, 1),
+                    )
+                )
+                * self.ct_vec.reshape(-1, 1, 1)
+            ).sum()
+        )
+        loss = (
+            (self.n / batch_size) * self.lam * term1 + term2 + term3
+        )  # upweight local param terms to be correct on expectation
         return loss
-    
-    def loss_no_cell_types(self, X):
-        assert(self.use_cell_types == False) #if this is True, just fail 
-        X = torch.Tensor(X)
-
-        theta = torch.softmax(self.theta, dim = 1)
-        eta = self.eta.exp()/(1.0 + (self.eta).exp())
-        eta = 0.5*(eta + eta.T)
-        gene_scaling = self.gene_scaling.exp()/(1.0 + self.gene_scaling.exp())
-        kappa = self.kappa.exp()/(1 + self.kappa.exp())
-        rho = self.rho.exp()/(1 + self.rho.exp())
-        alpha = torch.exp(self.alpha)
-        adj_matrix = self.adj_matrix
-        weights = self.weights
-        adj_matrix_1m = self.adj_matrix_1m
-        
-        if self.kgeql_flag: 
-            theta_ = contract('jk,j->jk',theta, gene_scaling + self.delta)
-            recon = contract('ik,jk->ij', alpha, theta_) 
-            term1 = -1.0*(torch.xlogy(X,recon) - recon).sum()
-        else:
-            selection = self.selection.softmax(dim = 1)
-            theta_new = contract('ij,kj->ki',selection,theta)
-            theta_ = contract('jk,j->jk',theta_new, gene_scaling + self.delta)
-            recon = contract('ik,jk->ij', alpha, theta_) 
-            term1 = -1.0*(torch.xlogy(X,recon) - recon).sum() - self.determinant_penalty*torch.logdet(contract('ij,kj->ik',selection, selection))
-
 
-        if len(adj_matrix) > 0:
-                mat = contract('il,lj,kj->ik',theta,eta,theta) 
-                term2 = -1.0*(torch.xlogy(adj_matrix*weights, (1.0 - rho)*(1.0 -kappa)*mat + (1.0 - rho)*kappa)).sum()
-                term3 = -1.0*(torch.xlogy(adj_matrix_1m,(1.0 -kappa)*(1.0 - rho)*(1.0 - mat) + rho)).sum()
-        else:
-            term2 = 0.0
-            term3 = 0.0
-
-        return self.lam*term1 + term2 + term3    
-
-    def initialize(self,gene_sets,val):    
+    def initialize(self, gene_sets, val):
         """
         form of gene_sets:
-        
+
         cell_type (inc. global) : set of sets of idxs
         """
-        
-        for ct in self.cell_types:
-            assert(self.L[ct] >= len(gene_sets[ct]))
-            count = 0
+
+        for i, ct in enumerate(self.ct_order):
+            assert self.L[ct] >= len(gene_sets[ct])
+            count = self.start_pos[ct]
             if self.L[ct] > 0:
-                if len(self.adj_matrix[ct]) > 0:
+                if self.cell_type_counts[i] > 0:
                     for gene_set in gene_sets[ct]:
-                        self.theta[ct].data[:,count][gene_set] = val
+                        self.theta.data[:, count][gene_set] = val
                         count = count + 1
-                    for i in range(self.L[ct]):
-                        self.eta[ct].data[i,-1] = -val
-                        self.eta[ct].data[-1,i] = -val
-                    self.theta[ct].data[:,-1][self.adj_matrix[ct].sum(axis = 1) == 0] = val
-                    self.theta[ct].data[:,-1][self.adj_matrix[ct].sum(axis = 1) != 0] = -val
-
-        assert(self.L["global"] >= len(gene_sets["global"]))
-        count = 0
-        for gene_set in gene_sets["global"]:
-            self.theta["global"].data[:,count][gene_set] = val
-            count = count + 1
-        for i in range(self.L["global"]):
-            self.eta["global"].data[i,-1] = -val
-            self.eta["global"].data[-1,i] = -val
-        self.theta["global"].data[:,-1][self.adj_matrix["global"].sum(axis = 1) == 0] = val
-        self.theta["global"].data[:,-1][self.adj_matrix["global"].sum(axis = 1) != 0] = -val
-    def initialize_no_celltypes(self,gs_list,val):
-        assert(self.L >= len(gs_list))
-        count = 0
-        for gene_set in gs_list:
-            self.theta.data[:,count][gene_set] = val
-            count = count + 1
-        for i in range(self.L):
-            self.eta.data[i,-1]= -val 
-            self.eta.data[-1,i] = -val 
-        self.theta.data[:,-1][self.adj_matrix.sum(axis = 1) == 0] = val
-        self.theta.data[:,-1][self.adj_matrix.sum(axis = 1) != 0] = -val 
+                    for j in range(self.L[ct]):
+                        self.eta.data[
+                            self.start_pos[ct] + j, self.start_pos[ct] + self.L[ct] - 1
+                        ] = -val
+                        self.eta.data[
+                            self.start_pos[ct] + self.L[ct] - 1, self.start_pos[ct] + j
+                        ] = -val
+                    self.theta.data[:, self.start_pos[ct] + self.L[ct] - 1][
+                        self.adj_matrix[i].sum(axis=1) == 0
+                    ] = val
+                    self.theta.data[:, self.start_pos[ct] + self.L[ct] - 1][
+                        self.adj_matrix[i].sum(axis=1) != 0
+                    ] = -val
 
 
 class SPECTRA_Model:
-    """ 
-    
+    """
+
     Parameters
         ----------
         X : np.ndarray or torch.Tensor
             the ``(n, p)`` -shaped matrix containing logged expression count data. Used for initialization of self.n and self.p but not stored as an attribute
         labels : np.ndarray or NoneType
             the ``(n, )`` -shaped array containing cell type labels. If use_cell_types == False, then should be set to None
-        K : dict or OrderedDict [if use_cell_types == False then int]
-            ``number of cell types + 1`` -shaped dictionary. Must have "global" as a key, indicating the number of global factors 
-            { 
-                "global": 15,
-                 "CD8": 5, 
-            } 
-            > Note that K contains the number of factors that describe the expression data while L contains the number of factors that describe the graph. When K < L an additional parameter that projects the L graph factors down is initialized. When L < K the behavior is to set L to max(L,K)
+
         L : dict or OrderedDict [if use_cell_types == False, then int]
             ``number of cell types + 1``-shaped dictionary. Must have "global" as a key, indicating the number of global factors
             {
-                "global": 15, 
-                "CD8": 5 
-                ...    
+                "global": 15,
+                "CD8": 5
+                ...
             }
-            > Format matches output of K_est.py to estimate the number of 
+            > Format matches output of K_est.py to estimate the number of
             > Must match cell type labels provided during training
-            > Recommended practice is to assign at minimum 2 factors per cell type 
-            > Note that K contains the number of factors that describe the expression data while L contains the number of factors that describe the graph. When K < L an additional parameter that projects the L graph factors down is initialized. When L < K the behavior is to set L to max(L,K) 
+            > Recommended practice is to assign at minimum 2 factors per cell type
+            > L contains the number of factors that describe the graph.
         adj_matrix :  dict or OrderedDict
-            ``a dictionary of adjacency matrices, one for every cell type + a "global" 
+            ``a dictionary of adjacency matrices, one for every cell type + a "global"
             {
                 "global": ``(p, p)``-shaped binary np.ndarray
-                "CD8": ... 
+                "CD8": ...
 
-            } 
+            }
         weights : dict or OrderedDict or NoneType [if use_cell_types == False, then ``(p, p)``-shaped array]
             the ``(p, p)``-shaped set of edge weights per . If weight[i,j] is non-zero when adj_matrix[i,j] = 0
-            this weight is ignored. 
-            
+            this weight is ignored.
+
             if weights == None, no weights are used
         lam : float
-            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information  
-        delta : float 
-            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes. 
+            lambda parameter of the model, which controls the relative influence of the graph vs expression loss functions. This term multiplies the expression loss, so smaller values of lambda upweight the prior information
+        delta : float
+            delta parameter of the model, which controls a lower bound for gene scaling factors. If delta is small then the maximum ratio between gene scaling factors is larger and lowly expressed genes can be put on the same scale as highly expressed genes.
         kappa : float or NoneType
-            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.  
+            kappa controls the background rate of edges in the graph. if kappa is a float, kappa is fixed to the given float value. If kappa == None, then kappa is a parameter that is estimated from the data.
         rho : float or NoneType
-            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data. 
-        use_cell_types: bool 
+            rho controls the bakcground rate of non-edges in the graph. if rho is a float, rho is fixed to the given float value. If rho == None, then rho is a parameter that is estimated from the data.
+        use_cell_types: bool
             use_cell_types is a Boolean variable that determines whether cell type labels are used to fit the model. If False, then parameters are initialized as nn.Parameter rather than as nn.ParameterDict with cell type keys that index nn.Parameter values
         determinant_penalty : float
-            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.  
+            determinant penalty affects the selection parameters that are fit when L[cell_type] > K[cell_type]. A determinantally regularized selection parameter is fit with determinant penalty that encourages sparsity and diversity.
     Attributes
         ----------
         model.delta : delta parameter of the model
 
-        model.lam : lambda parameter of the model 
-       
-        model.determinant_penalty : determinant penalty of the model 
-
-        model.K : K parameter, either int, dict, or OrderedDict() 
- 
-        model.L : L parameter, either int, dict or OrderedDict() 
+        model.lam : lambda parameter of the model
+
+        model.determinant_penalty : determinant penalty of the model
+
+        model.L : L parameter, either int, dict or OrderedDict()
 
         model.p : number of genes
 
-        model.n : number of cells 
+        model.n : number of cells
 
-        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters. 
+        model.use_cell_types : if True then cell types are considered, else cell types ignored. Affects the dimensions of the initialized parameters.
 
         model.kappa : if not kappa, nn.ParameterDict() if use_cell_types, else nn.Parameter(). If kappa is a float, it is fixed throughout training
 
         model.rho : if not rho, nn.ParamterDict() if use_cell_types, else nn.Parameter. If rho is a float it is fixed throughout training
 
-        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors 
+        model.adj_matrix : adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors
+
+        model.weights : contains edge weights. format matches adj_matrix
 
-        model.adj_matrix_1m : 1 - adjacency matrix with diagonal removed. dict containing torch.Tensors 
-        
-        model.weights : contains edge weights. format matches adj_matrix 
-        
         model.cell_types : np.ndarray containing array of unique cell types
-       
+
         model.cell_type_counts : dict {key = cell type, values = number of cells}
- 
-        model.factors : nn.ParameterDict() or nn.Parameter() containing the factor weights 
+
+        model.factors : nn.ParameterDict() or nn.Parameter() containing the factor weights
 
         model.cell_scores : nn.ParameterDict() or nn.Parameter() containing the cell loadings
 
         model.eta : nn.ParameterDict() or nn.Parameter() containing the interaction matrix between factors
 
         model.gene_scaling : nn.ParameterDict() or nn.Parameter() containing the gene scale factors
 
-        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False 
-        
-        
+        model.selection :  nn.ParameterDict() or nn.Parameter() containing the attention weights. Only initialized when L[cell_type] > K[cell_type] for some cell type or when L > K and use_cell_types == False
+
+
 
     Methods
         ----------
 
-        model.train(self, X, labels, lr_schedule,num_epochs, verbose) : 
+        model.train(self, X, labels, lr_schedule,num_epochs, verbose) :
         model.save()
         model.load()
         model.initialize
         model.return_selection()
         model.return_eta_diag()
         model.return_cell_scores()
-        model.return_factors() 
+        model.return_factors()
         model.return_eta()
-        model.return_rho() 
+        model.return_rho()
         model.return_kappa()
         model.return_gene_scalings()
-        model.return_graph(ct = "global") : 
+        model.return_graph(ct = "global") :
         model.matching(markers, gene_names_dict, threshold = 0.4):
 
     """
-    def __init__(self,X, labels,  K, L = None, vocab = None, gs_dict = None, use_weights = False, adj_matrix = None, weights = None, lam = 0.1, delta=0.1,kappa = None, rho = None, use_cell_types = True,determinant_penalty = 0.0):
-        self.K = K
+
+    def __init__(
+        self,
+        X,
+        labels,
+        L,
+        vocab=None,
+        gs_dict=None,
+        use_weights=False,
+        adj_matrix=None,
+        weights=None,
+        lam=0.1,
+        delta=0.1,
+        kappa=None,
+        rho=None,
+        use_cell_types=True,
+    ):
         self.L = L
-        self.lam = lam 
-        self.delta = delta 
-        self.kappa = kappa 
-        self.rho = rho 
+        self.lam = lam
+        self.delta = delta
+        self.kappa = kappa
+        self.rho = rho
         self.use_cell_types = use_cell_types
-        self.determinant_penalty = determinant_penalty
-        
-        
-         
+
         # if gs_dict is provided instead of adj_matrix, convert to adj_matrix, overrides adj_matrix and weights
         if gs_dict is not None:
             gene2id = dict((v, idx) for idx, v in enumerate(vocab))
-            
+
             if use_cell_types:
-                adj_matrix, weights = Spectra_util.process_gene_sets(gs_dict = gs_dict, gene2id = gene2id, weighted = use_weights)
-                #determine L
-                L = OrderedDict()
-                for key in gs_dict.keys():
-                    L[key] = len(gs_dict[key]) + 1
+                adj_matrix, weights = Spectra_util.process_gene_sets(
+                    gs_dict=gs_dict, gene2id=gene2id, weighted=use_weights
+                )
             else:
-                adj_matrix, weights = Spectra_util.process_gene_sets_no_celltypes(gs_dict = gs_dict, gene2id = gene2id, weighted = use_weights)
-                L = len(gs_dict) + 1
-            
-            
-                
-
-
-        self.internal_model = SPECTRA_select(X = X, labels = labels, adj_matrix = adj_matrix, L = L, K = K,weights = weights, lam = lam, delta=delta,kappa = kappa, rho = rho, use_cell_types = use_cell_types, determinant_penalty = determinant_penalty)
+                adj_matrix, weights = Spectra_util.process_gene_sets_no_celltypes(
+                    gs_dict=gs_dict, gene2id=gene2id, weighted=use_weights
+                )
+
+        self.internal_model = SPECTRA(
+            X=X,
+            labels=labels,
+            adj_matrix=adj_matrix,
+            L=L,
+            weights=weights,
+            lam=lam,
+            delta=delta,
+            kappa=kappa,
+            rho=rho,
+            use_cell_types=use_cell_types,
+        )
 
         self.cell_scores = None
         self.factors = None
         self.B_diag = None
-        self.eta_matrices = None 
-        self.gene_scalings = None 
-        self.rho = None 
-        self.kappa = None 
-
-    def train(self,X, labels = None, lr_schedule = [1.0,.5,.1,.01,.001,.0001],num_epochs = 10000, verbose = False): 
+        self.eta_matrices = None
+        self.gene_scalings = None
+        self.rho = None
+        self.kappa = None
+
+    def train(
+        self,
+        X,
+        labels=None,
+        lr_schedule=[0.5, 0.1, 0.01, 0.001, 0.0001],
+        num_epochs=100,
+        batch_size=1000,
+        skip=15,
+        verbose=False,
+    ):
         opt = torch.optim.Adam(self.internal_model.parameters(), lr=lr_schedule[0])
         counter = 0
         last = np.inf
-
+        device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        if self.internal_model.use_cell_types == False:
+            raise NotImplementedError("use_cell_types == False is not yet supported")
         for i in tqdm(range(num_epochs)):
-            #print(counter)
-            opt.zero_grad()
-            if self.internal_model.use_cell_types:
-                assert(len(labels) == X.shape[0])
-                loss = self.internal_model.loss(X, labels)
-            elif self.internal_model.use_cell_types == False:
-                loss = self.internal_model.loss_no_cell_types(X)
-
-            loss.backward()
-            opt.step()
-        
-            if loss.item() >= last:
-                counter += 1
-                if int(counter/3) >= len(lr_schedule):
-                    break
-                if counter % 3 == 0:
-                    opt = torch.optim.Adam(self.internal_model.parameters(), lr=lr_schedule[int(counter/3)])
-                    if verbose:
-                        print("UPDATING LR TO " + str(lr_schedule[int(counter/3)]))
-            last = loss.item() 
-
+            # At the beginning of epoch, get local parameters and batch them in random order
+            to_batch = [
+                torch.Tensor(X),
+                self.internal_model.alpha_mask,
+                self.internal_model.alpha,
+            ]
+            batches = batchify(to_batch, batch_size)
+            X_b, alpha_mask_b, alpha_b = batches[0], batches[1], batches[2]
+
+            tot = 0
+            for j in range(len(X_b)):
+                opt.zero_grad()
+                loss = self.internal_model.loss(
+                    X_b[j].to(device),
+                    alpha_mask_b[j].to(device),
+                    alpha_b[j],
+                    batch_size,
+                )
+                loss.backward()
+                opt.step()
+                tot += loss.item()
+
+                if loss.item() >= last:
+                    counter += 1
+                    if int(counter / skip) >= len(lr_schedule):
+                        break
+                    if counter % skip == 0:
+                        opt = torch.optim.Adam(
+                            self.internal_model.parameters(),
+                            lr=lr_schedule[int(counter / skip)],
+                        )
+                        if verbose:
+                            print(
+                                "UPDATING LR TO "
+                                + str(lr_schedule[int(counter / skip)])
+                            )
+                last = loss.item()
 
-        #add all model parameters as attributes 
+        # add all model parameters as attributes
 
         if self.use_cell_types:
             self.__store_parameters(labels)
         else:
             self.__store_parameters_no_celltypes()
+
     def save(self, fp):
-        torch.save(self.internal_model.state_dict(),fp)
-  
-    def load(self,fp,labels = None):
+        torch.save(self.internal_model.state_dict(), fp)
+
+    def load(self, fp, labels=None):
         self.internal_model.load_state_dict(torch.load(fp))
         if self.use_cell_types:
-            assert(labels is not None)
+            assert labels is not None
             self.__store_parameters(labels)
         else:
             self.__store_parameters_no_celltypes()
 
-    def __store_parameters(self,labels):
-
+    def __store_parameters(self, labels):
         """
         Replaces __cell_scores() and __compute factors() and __compute_theta()
         store parameters after fitting the model:
             cell scores
             factors
             eta
             scalings
             gene scalings
-            kappa 
-            rho 
+            kappa
+            rho
         """
 
         model = self.internal_model
 
-        #compute the loading matrix
+        # compute the loading matrix
+
+        k = model.L_tot
+        out = (torch.exp(model.alpha) * model.alpha_mask).detach().cpu().numpy()
+        theta = torch.cat(
+            [
+                temp.softmax(dim=1)
+                for temp in torch.split(
+                    model.theta, split_size_or_sections=model.L_list, dim=1
+                )
+            ],
+            dim=1,
+        )
+
+        gene_scaling = model.gene_scalings.exp() / (1.0 + model.gene_scalings.exp())
+        gene_scaling_ = contract(
+            "ij,ki->jk", gene_scaling, model.factor_to_celltype
+        )  # p x L_tot
+        scaled = (theta * (gene_scaling_ + model.delta)).T.detach().cpu().numpy()
 
-        k = sum(list(model.K.values()))
-        out = np.zeros((model.n, k))
-        
-        global_idx = model.K["global"]
-        
-        tot = global_idx    
-        f  = ["global"]*model.K["global"]
-        for cell_type in model.cell_types:
-            alpha = torch.exp(model.alpha[cell_type]).detach().numpy()
-            out[labels == cell_type, :global_idx] =  alpha[:,:global_idx]
-            out[labels == cell_type, tot:tot+model.K[cell_type]] = alpha[:,global_idx:]
-            
-            tot += model.K[cell_type]
-
-            f = f + [cell_type]*model.K[cell_type]
-
-
-        out2 = np.zeros((k, model.p))
-        
-        theta_ct = torch.softmax(model.theta["global"], dim = 1)
-        if model.kgeql_flag["global"] == False:
-            selection_ct = model.selection["global"].softmax(dim = 1)
-            theta_ct = contract('ij,kj->ki',selection_ct,theta_ct)
-            
-        theta = theta_ct.detach().numpy().T
-        tot = 0
-        out2[0:theta.shape[0],:] = theta 
-        tot += theta.shape[0]
-        
-        for cell_type in model.cell_types:
-            theta_ct = torch.softmax(model.theta[cell_type], dim = 1)
-            if model.kgeql_flag[cell_type] == False:
-                selection_ct = model.selection[cell_type].softmax(dim = 1)
-                theta_ct = contract('ij,kj->ki',selection_ct,theta_ct)
-            theta = theta_ct.detach().numpy().T
-            out2[tot:tot+theta.shape[0],:] = theta 
-            tot += theta.shape[0]
-        
-        factors = out2
-        lst = []
-        for i in range(len(f)):
-            ct = f[i]
-            scaled = factors[i,:]*(model.gene_scaling[ct].exp().detach()/(1.0 + model.gene_scaling[ct].exp().detach()) + model.delta).numpy()
-
-
-            lst.append(scaled)
-        scaled = np.array(lst)
-        new_factors = scaled/(scaled.sum(axis = 0,keepdims =True) + 1.0)
-        cell_scores = out*scaled.mean(axis = 1).reshape(1,-1) 
+        new_factors = scaled / (scaled.sum(axis=0, keepdims=True) + 1.0)
+        cell_scores = out * scaled.mean(axis=1).reshape(1, -1)
+
+        # new store params stuff
         self.cell_scores = cell_scores
         self.factors = new_factors
         self.B_diag = self.__B_diag()
         self.eta_matrices = self.__eta_matrices()
-        self.gene_scalings = {ct: model.gene_scaling[ct].exp().detach().numpy()/(1.0 + model.gene_scaling[ct].exp().detach().numpy()) for ct in model.gene_scaling.keys()}
-        self.rho = {ct: model.rho[ct].exp().detach().numpy()/(1.0 + model.rho[ct].exp().detach().numpy()) for ct in model.rho.keys()}
-        self.kappa = {ct: model.kappa[ct].exp().detach().numpy()/(1.0 + model.kappa[ct].exp().detach().numpy()) for ct in model.kappa.keys()}
-        self.selection = {ct: model.selection[ct].softmax(dim = 1).detach().numpy() for ct in model.selection.keys()}
+        self.gene_scalings = {
+            ct: gene_scaling[i].detach().cpu().numpy()
+            for i, ct in enumerate(model.ct_order)
+        }
+        self.rho = {
+            ct: model.rho[i].exp().detach().cpu().numpy()
+            / (1.0 + model.rho[i].exp().detach().cpu().numpy())
+            for i, ct in enumerate(model.ct_order)
+        }
+        self.kappa = {
+            ct: model.kappa[i].exp().detach().cpu().numpy()
+            / (1.0 + model.kappa[i].exp().detach().cpu().numpy())
+            for i, ct in enumerate(model.ct_order)
+        }
 
     def __B_diag(self):
         model = self.internal_model
-        k = 0 
-        
-        for key in model.K.keys():
-            k += max(model.K[key], model.L[key]) 
-        out = np.zeros(k)
-        
-        Bg = model.eta["global"].exp()/(1.0 + model.eta["global"].exp())
-        Bg = 0.5*(Bg + Bg.T)
-        B = torch.diag(Bg).detach().numpy()
-        tot = 0
-        out[0:B.shape[0]] = B
-        tot += B.shape[0]
-        
-        for cell_type in model.cell_types:
-            Bg = model.eta[cell_type].exp()/(1.0 + model.eta[cell_type].exp())
-            Bg = 0.5*(Bg + Bg.T)
-            B = torch.diag(Bg).detach().numpy()
-            out[tot:tot+B.shape[0]] = B
-            
-            tot += B.shape[0]
 
-        return out
+        Bg = model.eta.exp() / (1.0 + model.eta.exp())
+        Bg = 0.5 * (Bg + Bg.T)
+        B = torch.diag(Bg).detach().cpu().numpy()
+        return B
 
     def __eta_matrices(self):
         model = self.internal_model
         eta = OrderedDict()
-        Bg = model.eta["global"].exp()/(1.0 + model.eta["global"].exp())
-        Bg = 0.5*(Bg + Bg.T)
-        eta["global"] = Bg.detach().numpy()
-
-        for cell_type in model.cell_types:
-            Bg = model.eta[cell_type].exp()/(1.0 + model.eta[cell_type].exp())
-            Bg = 0.5*(Bg + Bg.T)
-            eta[cell_type] = Bg.detach().numpy()
-        return eta 
-
+        Bg = model.eta.exp() / (1.0 + model.eta.exp())
+        Bg = 0.5 * (Bg + Bg.T)
 
-    def __store_parameters_no_celltypes(self):
-        """
-        store parameters after fitting the model:
-            cell scores
-            factors
-            eta
-            scalings
-            gene scalings
-            kappa 
-            rho 
-        """
-        model = self.internal_model
-        
-        
-        alpha = torch.exp(model.alpha).detach().numpy()
-        out = alpha
-        if model.kgeql_flag:
-            theta_ct = torch.softmax(model.theta, dim = 1)
-        else: 
-            seletion_ct = model.selection.softmax(dim = 1)
-            theta_ct = torch.softmax(model.theta, dim = 1)
-            theta_ct = contract('ij,kj->ki',selection_ct,theta_ct)
-        theta = theta_ct.detach().numpy().T
-        factors = theta 
-        scaled = factors*(model.gene_scaling.exp().detach()/(1.0 + model.gene_scaling.exp().detach()) + model.delta).numpy().reshape(1,-1)
-        new_factors = scaled/(scaled.sum(axis = 0,keepdims =True) + 1.0)
+        for ct in model.ct_order:
+            eta[ct] = (
+                Bg[
+                    model.start_pos[ct] : model.start_pos[ct] + model.L[ct],
+                    model.start_pos[ct] : model.start_pos[ct] + model.L[ct],
+                ]
+                .detach()
+                .cpu()
+                .numpy()
+            )
+        return eta
 
-        self.factors = new_factors
-        self.cell_scores = out*scaled.mean(axis = 1).reshape(1,-1)  
-        Bg = model.eta.exp()/(1.0 + model.eta.exp())
-        Bg = 0.5*(Bg + Bg.T)
-        self.B_diag = torch.diag(Bg).detach().numpy()
-        self.eta_matrices = Bg.detach().numpy()
-        self.gene_scalings = (model.gene_scaling.exp().detach()/(1.0 + model.gene_scaling.exp().detach())).numpy()
-        self.rho = (model.rho.exp().detach()/(1.0 + model.rho.exp().detach())).numpy()
-        self.kappa = (model.kappa.exp().detach()/(1.0 + model.kappa.exp().detach())).numpy()
-        self.selection = model.selection.softmax(dim = 1).detach().numpy()
-    def initialize(self,annotations, word2id, val = 25):
+    def initialize(self, annotations, word2id, W, init_scores, val=25):
         """
         self.use_cell_types must be True
         create form of gene_sets:
-        
+
         cell_type (inc. global) : set of sets of idxs
+
+        filter based on L_ct
         """
         if self.use_cell_types:
+            if init_scores == None:
+                init_scores = compute_init_scores(annotations, word2id, torch.Tensor(W))
             gs_dict = OrderedDict()
             for ct in annotations.keys():
+                mval = max(self.L[ct] - 1, 0)
+                sorted_init_scores = sorted(init_scores[ct].items(), key=lambda x: x[1])
+                sorted_init_scores = sorted_init_scores[-1 * mval :]
+                names = set([k[0] for k in sorted_init_scores])
                 lst_ct = []
                 for key in annotations[ct].keys():
-                    words = annotations[ct][key]
-                    idxs = []
-                    for word in words:
-                        if word in word2id:
-                            idxs.append(word2id[word])
-                    lst_ct.append(idxs)
+                    if key in names:
+                        words = annotations[ct][key]
+                        idxs = []
+                        for word in words:
+                            if word in word2id:
+                                idxs.append(word2id[word])
+                        lst_ct.append(idxs)
                 gs_dict[ct] = lst_ct
-            self.internal_model.initialize(gene_sets = gs_dict, val = val)
+            self.internal_model.initialize(gene_sets=gs_dict, val=val)
         else:
+            if init_scores == None:
+                init_scores = compute_init_scores_noct(
+                    annotations, word2id, torch.Tensor(W)
+                )
             lst = []
+            mval = max(self.L - 1, 0)
+            sorted_init_scores = sorted(init_scores.items(), key=lambda x: x[1])
+            sorted_init_scores = sorted_init_scores[-1 * mval :]
+            names = set([k[0] for k in sorted_init_scores])
             for key in annotations.keys():
-                words = annotations[key]
-                idxs = []
-                for word in words:
-                    if word in word2id:
-                        idxs.append(word2id[word])
-                lst.append(idxs)
-            self.internal_model.initialize_no_celltypes(gs_list = lst, val = val)
-    def return_selection(self):
-        return self.selection
+                if key in names:
+                    words = annotations[key]
+                    idxs = []
+                    for word in words:
+                        if word in word2id:
+                            idxs.append(word2id[word])
+                    lst.append(idxs)
+            self.internal_model.initialize_no_celltypes(gs_list=lst, val=val)
+
     def return_eta_diag(self):
         return self.B_diag
+
     def return_cell_scores(self):
         return self.cell_scores
+
     def return_factors(self):
-        return self.factors 
+        return self.factors
+
     def return_eta(self):
         return self.eta_matrices
+
     def return_rho(self):
-        return self.rho 
+        return self.rho
+
     def return_kappa(self):
         return self.kappa
-    def return_gene_scalings(self): 
+
+    def return_gene_scalings(self):
         return self.gene_scalings
-    def return_graph(self, ct = "global"):
+
+    def return_graph(self, ct="global"):
         model = self.internal_model
         if self.use_cell_types:
-            eta = (model.eta[ct]).exp()/(1.0 + (model.eta[ct]).exp())
-            eta = 0.5*(eta + eta.T)
-            theta = torch.softmax(model.theta[ct], dim = 1)
-            mat = contract('il,lj,kj->ik',theta,eta,theta).detach().numpy()
-        else: 
-            eta = model.eta.exp()/(1.0 + model.eta.exp())
-            eta = 0.5*(eta + eta.T)
-            theta = torch.softmax(model.theta, dim = 1)
-            mat = contract('il,lj,kj->ik',theta,eta,theta).detach().numpy()
+            eta = (model.eta[ct]).exp() / (1.0 + (model.eta[ct]).exp())
+            eta = 0.5 * (eta + eta.T)
+            theta = torch.softmax(model.theta[ct], dim=1)
+            mat = contract("il,lj,kj->ik", theta, eta, theta).detach().numpy()
+        else:
+            eta = model.eta.exp() / (1.0 + model.eta.exp())
+            eta = 0.5 * (eta + eta.T)
+            theta = torch.softmax(model.theta, dim=1)
+            mat = contract("il,lj,kj->ik", theta, eta, theta).detach().numpy()
         return mat
-        
-    def matching(self, markers, gene_names_dict, threshold = 0.4):
+
+    def matching(self, markers, gene_names_dict, threshold=0.4):
         """
         best match based on overlap coefficient
         """
         markers = pd.DataFrame(markers)
         if self.use_cell_types:
             matches = []
             jaccards = []
             for i in range(markers.shape[0]):
-                max_jacc = 0.0 
+                max_jacc = 0.0
                 best = ""
                 for key in gene_names_dict.keys():
                     for gs in gene_names_dict[key].keys():
                         t = gene_names_dict[key][gs]
 
-                        jacc = Spectra_util.overlap_coefficient(list(markers.iloc[i,:]),t)
+                        jacc = Spectra_util.overlap_coefficient(
+                            list(markers.iloc[i, :]), t
+                        )
                         if jacc > max_jacc:
                             max_jacc = jacc
-                            best = gs 
+                            best = gs
                 matches.append(best)
                 jaccards.append(max_jacc)
-            
+
         else:
             matches = []
             jaccards = []
             for i in range(markers.shape[0]):
-                max_jacc = 0.0 
+                max_jacc = 0.0
                 best = ""
                 for key in gene_names_dict.keys():
                     t = gene_names_dict[key]
 
-                    jacc = Spectra_util.overlap_coefficient(list(markers.iloc[i,:]),t)
+                    jacc = Spectra_util.overlap_coefficient(list(markers.iloc[i, :]), t)
                     if jacc > max_jacc:
                         max_jacc = jacc
-                        best = key 
+                        best = key
                 matches.append(best)
                 jaccards.append(max_jacc)
         output = []
         for j in range(markers.shape[0]):
             if jaccards[j] > threshold:
                 output.append(matches[j])
             else:
                 output.append("0")
         return np.array(output)
 
 
+def est_spectra(
+    adata,
+    gene_set_dictionary,
+    L=None,
+    use_highly_variable=True,
+    cell_type_key=None,
+    use_weights=True,
+    lam=0.008,
+    delta=0.001,
+    kappa=None,
+    rho=0.05,
+    use_cell_types=True,
+    n_top_vals=50,
+    filter_sets=True,
+    **kwargs,
+):
+    """
 
-""" 
-Public Functions 
-
-
-    est_spectra():
-
-    matching(): 
-
-    graph_network():  
-
-    markers
-
-
-"""
-
-def est_spectra(adata, gene_set_dictionary, K = None, use_highly_variable = True, cell_type_key = None, use_weights = False, lam = 0.1, delta=0.1,kappa = None, rho = None, use_cell_types = True, n_top_vals = 50, determinant_penalty = 0.0, **kwargs):
-    """ 
-    
     Parameters
         ----------
-        adata : AnnData object 
+        adata : AnnData object
             containing cell_type_key with log count data stored in .X
-        gene_set_dictionary : dict or OrderedDict() 
-            maps cell types to gene set names to gene sets ; if use_cell_types == False then maps gene set names to gene sets ; 
+        gene_set_dictionary : dict or OrderedDict()
+            maps cell types to gene set names to gene sets ; if use_cell_types == False then maps gene set names to gene sets ;
             must contain "global" key in addition to every unique cell type under .obs.<cell_type_key>
-        K : dict, OrderedDict(), int , NoneType
+        L : dict, OrderedDict(), int , NoneType
             number of factors per cell type ; if use_cell_types == False then int. Else dictionary. If None then match factors
-            to number of gene sets (recommended) 
-        use_highly_variable : bool 
+            to number of gene sets (recommended)
+        use_highly_variable : bool
             if True, then uses highly_variable_genes
         cell_type_key : str
             cell type key, must be under adata.obs.<cell_type_key> . If use_cell_types == False, this is ignored
         use_weights : bool
             if True, edge weights are estimated based on graph structure and used throughout training
-        lam : float 
+        lam : float
             lambda parameter of the model. weighs relative contribution of graph and expression loss functions
         delta : float
             delta parameter of the model. lower bounds possible gene scaling factors so that maximum ratio of gene scalings
-            cannot be too large 
+            cannot be too large
         kappa : float or None
             if None, estimate background rate of 1s in the graph from data
-        rho : float or None 
+        rho : float or None
             if None, estimate background rate of 0s in the graph from data
         use_cell_types : bool
             if True then cell type label is used to fit cell type specific factors. If false then cell types are ignored
         n_top_vals : int
             number of top markers to return in markers dataframe
-        determinant_penalty : float 
+        determinant_penalty : float
             determinant penalty of the attention mechanism. If set higher than 0 then sparse solutions of the attention weights
-            and diverse attention weights are encouraged. However, tuning is crucial as setting too high reduces the selection 
+            and diverse attention weights are encouraged. However, tuning is crucial as setting too high reduces the selection
             accuracy because convergence to a hard selection occurs early during training [todo: annealing strategy]
+        filter_sets : bool
+            whether to filter the gene sets based on coherence
         **kwargs : (num_epochs = 10000, lr_schedule = [...], verbose = False)
             arguments to .train(), maximum number of training epochs, learning rate schedule and whether to print changes in
             learning rate
-            
+
      Returns: SPECTRA_Model object [after training]
-     
-     In place: adds 1. factors, 2. cell scores, 3. vocabulary, and 4. markers as attributes in .obsm, .var, .uns   
 
-    
+     In place: adds 1. factors, 2. cell scores, 3. vocabulary, and 4. markers as attributes in .obsm, .var, .uns
+
+
     """
 
-    if K == None:
+    if use_cell_types == False:
+        raise NotImplementedError("use_cell_types == False is not supported yet")
+
+    print("CUDA Available: ", torch.cuda.is_available())
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+
+    if L == None:
+        init_flag = True
         if use_cell_types:
-            K = {}
-            for key in gene_set_dictionary.keys(): 
+            L = {}
+            for key in gene_set_dictionary.keys():
                 length = len(list(gene_set_dictionary[key].values()))
-                K[key] = length + 1 
+                L[key] = length + 1
         else:
             length = len(list(gene_set_dictionary.values()))
-            K = length + 1
-    #create vocab list from gene_set_dictionary
+            L = length + 1
+    # create vocab list from gene_set_dictionary
     lst = []
     if use_cell_types:
         for key in gene_set_dictionary:
             for key2 in gene_set_dictionary[key]:
-                gene_list = gene_set_dictionary[key][key2] 
+                gene_list = gene_set_dictionary[key][key2]
                 lst += gene_list
     else:
         for key in gene_set_dictionary:
             gene_list = gene_set_dictionary[key]
             lst += gene_list
 
-    #lst contains all of the genes that are in the gene sets --> convert to boolean array 
-    bools = [] 
+    # lst contains all of the genes that are in the gene sets --> convert to boolean array
+    bools = []
     for gene in adata.var_names:
         if gene in lst:
             bools.append(True)
-        else: 
+        else:
             bools.append(False)
     bools = np.array(bools)
 
     if use_highly_variable:
-        idx_to_use = bools | adata.var.highly_variable #take intersection of highly variable and gene set genes (todo: add option to change this at some point)
-        X = adata.X[:,idx_to_use] 
+        idx_to_use = (
+            bools | adata.var.highly_variable
+        )  # take intersection of highly variable and gene set genes (todo: add option to change this at some point)
+        X = adata.X[:, idx_to_use]
         vocab = adata.var_names[idx_to_use]
         adata.var["spectra_vocab"] = idx_to_use
-    else: 
+    else:
         X = adata.X
-        vocab = adata.var_names 
-    
-    if cell_type_key is not None:
+        vocab = adata.var_names
+
+    if use_cell_types:
         labels = adata.obs[cell_type_key].values
+        for label in np.unique(labels):
+            if label not in gene_set_dictionary:
+                gene_set_dictionary[label] = {}
+            if label not in L:
+                L[label] = 1
     else:
-        labels = None 
+        labels = None
     if type(X) == scipy.sparse.csr.csr_matrix:
         X = np.array(X.todense())
     word2id = dict((v, idx) for idx, v in enumerate(vocab))
     id2word = dict((idx, v) for idx, v in enumerate(vocab))
 
-    spectra = SPECTRA_Model(X = X, labels = labels,  K =K, L = None, vocab = vocab, gs_dict = gene_set_dictionary, use_weights = use_weights, lam = lam, delta=delta,kappa = kappa, rho = rho, use_cell_types = use_cell_types,determinant_penalty = determinant_penalty)
-    spectra.initialize(gene_set_dictionary, word2id)
-    spectra.train(X = X, labels = labels,**kwargs)
+    if filter_sets:
+        if use_cell_types:
+            new_gs_dict = {}
+            init_scores = compute_init_scores(
+                gene_set_dictionary, word2id, torch.Tensor(X)
+            )
+            for ct in gene_set_dictionary.keys():
+                new_gs_dict[ct] = {}
+                mval = max(L[ct] - 1, 0)
+                sorted_init_scores = sorted(init_scores[ct].items(), key=lambda x: x[1])
+                sorted_init_scores = sorted_init_scores[-1 * mval :]
+                names = set([k[0] for k in sorted_init_scores])
+                for key in gene_set_dictionary[ct].keys():
+                    if key in names:
+                        new_gs_dict[ct][key] = gene_set_dictionary[ct][key]
+        else:
+            init_scores = compute_init_scores_noct(
+                gene_set_dictionary, word2id, torch.Tensor(X)
+            )
+            new_gs_dict = {}
+            mval = max(L - 1, 0)
+            sorted_init_scores = sorted(init_scores.items(), key=lambda x: x[1])
+            sorted_init_scores = sorted_init_scores[-1 * mval :]
+            names = set([k[0] for k in sorted_init_scores])
+            for key in gene_set_dictionary.keys():
+                if key in names:
+                    new_gs_dict[key] = gene_set_dictionary[key]
+        gene_set_dictionary = new_gs_dict
+    else:
+        init_scores = None
+    print("Initializing model...")
+    spectra = SPECTRA_Model(
+        X=X,
+        labels=labels,
+        L=L,
+        vocab=vocab,
+        gs_dict=gene_set_dictionary,
+        use_weights=use_weights,
+        lam=lam,
+        delta=delta,
+        kappa=kappa,
+        rho=rho,
+        use_cell_types=use_cell_types,
+    )
+    spectra.internal_model.to(device)
+    print("CUDA memory: ", 1e-9 * torch.cuda.memory_allocated(device=device))
+    spectra.initialize(gene_set_dictionary, word2id, X, init_scores)
+    print("Beginning training...")
+    spectra.train(X=X, labels=labels, **kwargs)
 
     adata.uns["SPECTRA_factors"] = spectra.factors
     adata.obsm["SPECTRA_cell_scores"] = spectra.cell_scores
-    adata.uns["SPECTRA_markers"] = return_markers(factor_matrix = spectra.factors, id2word = id2word, n_top_vals = n_top_vals)
-
+    adata.uns["SPECTRA_markers"] = return_markers(
+        factor_matrix=spectra.factors, id2word=id2word, n_top_vals=n_top_vals
+    )
+    adata.uns["SPECTRA_L"] = L
     return spectra
 
-def return_markers(factor_matrix, id2word,n_top_vals = 100):
-    idx_matrix = np.argsort(factor_matrix,axis = 1)[:,::-1][:,:n_top_vals]
+
+def return_markers(factor_matrix, id2word, n_top_vals=100):
+    idx_matrix = np.argsort(factor_matrix, axis=1)[:, ::-1][:, :n_top_vals]
     df = pd.DataFrame(np.zeros(idx_matrix.shape))
     for i in range(idx_matrix.shape[0]):
         for j in range(idx_matrix.shape[1]):
-            df.iloc[i,j] = id2word[idx_matrix[i,j]]
+            df.iloc[i, j] = id2word[idx_matrix[i, j]]
     return df.values
 
 
+def load_from_pickle(fp, adata, gs_dict, cell_type_key):
+    model = SPECTRA_Model(
+        X=adata[:, adata.var["spectra_vocab"]].X,
+        labels=np.array(adata.obs[cell_type_key]),
+        L=adata.uns["SPECTRA_L"],
+        vocab=adata.var_names[adata.var["spectra_vocab"]],
+        gs_dict=gs_dict,
+    )
+    model.load(fp, labels=np.array(adata.obs[cell_type_key]))
+    return model
 
 
-def graph_network(adata, mat, gene_set,thres = 0.20, N = 50):
-    
+def graph_network(adata, mat, gene_set, thres=0.20, N=50):
+
     vocab = adata.var_names[adata.var["spectra_vocab"]]
     word2id = dict((v, idx) for idx, v in enumerate(vocab))
     id2word = dict((idx, v) for idx, v in enumerate(vocab))
-    
-    net = Network(height='750px', width='100%', bgcolor='#FFFFFF', font_color='black', notebook = True)
+
+    net = Network(
+        height="750px",
+        width="100%",
+        bgcolor="#FFFFFF",
+        font_color="black",
+        notebook=True,
+    )
     net.barnes_hut()
-    
+
     idxs = []
     for term in gene_set:
         idxs.append(word2id[term])
-    ests = list(set(list(mat[idxs,:].sum(axis = 0).argsort()[::-1][:N]) + idxs))
+    ests = list(set(list(mat[idxs, :].sum(axis=0).argsort()[::-1][:N]) + idxs))
     ests_names = []
-    count = 0 
+    count = 0
     for est in ests:
         ests_names.append(id2word[est])
         if est not in idxs:
-            net.add_node(count, label = id2word[est], color = '#00ff1e')
+            net.add_node(count, label=id2word[est], color="#00ff1e")
         else:
-            net.add_node(count, label = id2word[est], color = '#162347')
+            net.add_node(count, label=id2word[est], color="#162347")
         count += 1
-        
-    inferred_mat = mat[ests,:][:,ests]
+
+    inferred_mat = mat[ests, :][:, ests]
     for i in range(len(inferred_mat)):
-        for j in range(i+1, len(inferred_mat)):
-            if inferred_mat[i,j] > thres:
+        for j in range(i + 1, len(inferred_mat)):
+            if inferred_mat[i, j] > thres:
                 net.add_edge(i, j)
     neighbor_map = net.get_adj_list()
     for node in net.nodes:
-        node['value'] = len(neighbor_map[node['id']])
+        node["value"] = len(neighbor_map[node["id"]])
 
     return net
 
-def graph_network_multiple(adata, mat, gene_sets,thres = 0.20, N = 50):
+
+def graph_network_multiple(adata, mat, gene_sets, thres=0.20, N=50):
     gene_set = []
     for gs in gene_sets:
         gene_set += gs
-        
+
     vocab = adata.var_names[adata.var["spectra_vocab"]]
     word2id = dict((v, idx) for idx, v in enumerate(vocab))
     id2word = dict((idx, v) for idx, v in enumerate(vocab))
-    
-    net = Network(height='750px', width='100%', bgcolor='#FFFFFF', font_color='black', notebook = True)
+
+    net = Network(
+        height="750px",
+        width="100%",
+        bgcolor="#FFFFFF",
+        font_color="black",
+        notebook=True,
+    )
     net.barnes_hut()
     idxs = []
     for term in gene_set:
         idxs.append(word2id[term])
-    ests = list(set(list(mat[idxs,:].sum(axis = 0).argsort()[::-1][:N]) + idxs))
+    ests = list(set(list(mat[idxs, :].sum(axis=0).argsort()[::-1][:N]) + idxs))
     ests_names = []
-    count = 0 
-    
+    count = 0
+
     color_map = []
     for gene_set in gene_sets:
-        random_color = ["#"+''.join([random.choice('ABCDEF0123456789') for i in range(6)])]
+        random_color = [
+            "#" + "".join([random.choice("ABCDEF0123456789") for i in range(6)])
+        ]
         color_map.append(random_color[0])
-        
+
     for est in ests:
         ests_names.append(id2word[est])
         if est not in idxs:
-            net.add_node(count, label = id2word[est], color = '#00ff1e')
+            net.add_node(count, label=id2word[est], color="#00ff1e")
         else:
             for i in range(len(gene_sets)):
                 if id2word[est] in gene_sets[i]:
                     color = color_map[i]
                     break
-            net.add_node(count, label = id2word[est], color = color)
+            net.add_node(count, label=id2word[est], color=color)
         count += 1
-        
-    inferred_mat = mat[ests,:][:,ests]
+
+    inferred_mat = mat[ests, :][:, ests]
     for i in range(len(inferred_mat)):
-        for j in range(i+1, len(inferred_mat)):
-            if inferred_mat[i,j] > thres:
+        for j in range(i + 1, len(inferred_mat)):
+            if inferred_mat[i, j] > thres:
                 net.add_edge(i, j)
     neighbor_map = net.get_adj_list()
     for node in net.nodes:
-        node['value'] = len(neighbor_map[node['id']])
+        node["value"] = len(neighbor_map[node["id"]])
 
     return net
 
+
 def gene_set_graph(gene_sets):
     """
     input
     [
     ["a","b", ... ],
     ["b", "d"],
-    
-    ... 
+
+    ...
     ]
     """
-    
-    net = Network(height='750px', width='100%', bgcolor='#FFFFFF', font_color='black', notebook = True)
+
+    net = Network(
+        height="750px",
+        width="100%",
+        bgcolor="#FFFFFF",
+        font_color="black",
+        notebook=True,
+    )
     net.barnes_hut()
     count = 0
-    #create nodes
+    # create nodes
     genes = []
     for gene_set in gene_sets:
         genes += gene_set
-    
+
     color_map = []
     for gene_set in gene_sets:
-        random_color = ["#"+''.join([random.choice('ABCDEF0123456789') for i in range(6)])]
+        random_color = [
+            "#" + "".join([random.choice("ABCDEF0123456789") for i in range(6)])
+        ]
         color_map.append(random_color[0])
-        
-    for gene in genes:          
+
+    for gene in genes:
         for i in range(len(gene_sets)):
             if gene in gene_sets[i]:
                 color = color_map[i]
                 break
-        net.add_node(gene, label = gene, color = color)
+        net.add_node(gene, label=gene, color=color)
 
     for gene_set in gene_sets:
         for i in range(len(gene_set)):
-            for j in range(i+1, len(gene_set)):
+            for j in range(i + 1, len(gene_set)):
                 net.add_edge(gene_set[i], gene_set[j])
 
-        
     neighbor_map = net.get_adj_list()
     for node in net.nodes:
-        node['value'] = len(neighbor_map[node['id']])
+        node["value"] = len(neighbor_map[node["id"]])
 
     return net
```

### Comparing `scSpectra-0.1.0/Spectra/Spectra_util.py` & `scspectra-0.2.0/src/Spectra/Spectra_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import numpy as np 
-from collections import OrderedDict 
+import numpy as np
+from collections import OrderedDict
 import pkg_resources
 import pandas as pd
-import torch 
-#from adjustText import adjust_text
+import torch
+
+# from adjustText import adjust_text
 from opt_einsum import contract
 import scipy
+
 """
 methods 
 _______
 
 amatrix(gene_set_list, gene2id) 
 
 amatrix_weighted(gene_set_list, gene2id)
@@ -23,336 +25,416 @@
 overlap_coefficient()
 
 label_marker_genes()
 
 
 """
 
-def overlap_coefficient(list1, list2): 
-    """ 
+
+def overlap_coefficient(list1, list2):
+    """
     Computes overlap coefficient between two lists
-    """ 
+    """
     intersection = len(list(set(list1).intersection(set(list2))))
-    union = min(len(list1),len(list2))# + len(list2)) - intersection
+    union = min(len(list1), len(list2))  # + len(list2)) - intersection
     return float(intersection) / union
 
 
-def check_gene_set_dictionary(adata, annotations, obs_key='cell_type_annotations',global_key='global', return_dict = True,min_len=3,use_cell_types=True):
-    '''
-    Filters annotations dictionary to contain only genes contained in the adata. 
+def check_gene_set_dictionary(
+    adata,
+    annotations,
+    obs_key="cell_type_annotations",
+    global_key="global",
+    return_dict=True,
+    min_len=3,
+    use_cell_types=True,
+):
+    """
+    Filters annotations dictionary to contain only genes contained in the adata.
     Checks that annotations dictionary cell type keys and adata cell types are identical.
     Checks that all gene sets in annotations dictionary contain >2 genes after filtering.
 
-    
+
     adata: AnnData , data to use with Spectra
     annotations: dict , gene set annotations dictionary to use with Spectra
     obs_key: str , column name for cell type annotations in adata.obs
     global_key: str , key for global gene sests in gene set annotation dictionary
     return_dict: bool , return filtered gene set annotation dictionary
     min_len: int, minimum length of gene sets
-    
+
     returns: dict , filtered gene set annotation dictionary
-    
-    '''
-    #test if keys match
-    if use_cell_types == False:
-        annotations = {global_key:annotations}
+
+    """
+    # test if keys match
     if use_cell_types:
-        adata_labels  = list(set(adata.obs[obs_key]))+[global_key]#cell type labels in adata object
+        adata_labels = list(set(adata.obs[obs_key])) + [
+            global_key
+        ]  # cell type labels in adata object
     else:
-        adata_labels  = [global_key]
+        annotations = {global_key: annotations}
+        adata_labels = [global_key]
     annotation_labels = list(annotations.keys())
     matching_celltype_labels = list(set(adata_labels).intersection(annotation_labels))
-    if set(annotation_labels)!=set(adata_labels):
-        missing_adata = set(adata_labels)-set(annotation_labels)
+    if set(annotation_labels) != set(adata_labels):
+        missing_adata = set(adata_labels) - set(annotation_labels)
         missing_dict = set(annotation_labels) - set(adata_labels)
-        raise ValueError('The following adata labels are missing in the gene set annotation dictionary:',missing_dict,
-                        'The following gene set annotation dictionary keys are missing in the adata labels:',missing_adata)
+        raise ValueError(
+            "The following adata labels are missing in the gene set annotation dictionary:",
+            missing_dict,
+            "The following gene set annotation dictionary keys are missing in the adata labels:",
+            missing_adata,
+        )
         dict_keys_OK = False
     else:
-        print('Cell type labels in gene set annotation dictionary and AnnData object are identical')
+        print(
+            "Cell type labels in gene set annotation dictionary and AnnData object are identical"
+        )
         dict_keys_OK = True
-        
-    #check that gene sets in dictionary have len >2
+
+    # check that gene sets in dictionary have len >2
     annotations_new = {}
-    for k,v in annotations.items():
+    for k, v in annotations.items():
         annotations_new[k] = {}
-        for k2,v2 in v.items():
-            gs= [x for x in v2 if x in adata.var_names]
-            if len(gs)<min_len:
-                print('removing gene set',k2,'for cell type',k,'which is of length',len(v2),len(gs),'genes are found in the data.',
-                      'minimum length is',min_len)
+        for k2, v2 in v.items():
+            gs = [x for x in v2 if x in adata.var_names]
+            if len(gs) < min_len:
+                print(
+                    "removing gene set",
+                    k2,
+                    "for cell type",
+                    k,
+                    "which is of length",
+                    len(v2),
+                    len(gs),
+                    "genes are found in the data.",
+                    "minimum length is",
+                    min_len,
+                )
             else:
                 annotations_new[k][k2] = gs
-            
+
+    # raise error if no gene sets remain
+    if not use_cell_types and len(annotations_new[global_key]) == 0:
+        raise ValueError(
+            "No gene sets remain in the gene set annotation dictionary. Please make sure that gene names correspond to names found in `adata.var_names`. See: https://github.com/dpeerlab/spectra/issues/34."
+        )
+
     if dict_keys_OK:
-        print('Your gene set annotation dictionary is now correctly formatted.')
+        print("Your gene set annotation dictionary is now correctly formatted.")
     if return_dict:
         if use_cell_types == False:
             return annotations_new[global_key]
         else:
             return annotations_new
 
 
-def label_marker_genes(marker_genes, gs_dict, threshold = 0.4):
-    '''
+def label_marker_genes(marker_genes, gs_dict, threshold=0.4):
+    """
     label an array of marker genes using the gene_set_dictionary in est_spectra
     returns a dataframe of overlap coefficients for each gene set annotation and marker gene
     marker_genes: array factors x marker genes or a KnowledgeBase object
     label an array containing marker genes by its overlap with a dictionary of gene sets from the knowledge base:
     KnowledgeBase.celltype_process_dict
-    '''
+    """
 
     overlap_df = pd.DataFrame()
-    marker_set_len_dict = {} #len of gene sets to resolve ties
+    marker_set_len_dict = {}  # len of gene sets to resolve ties
     for i, v in pd.DataFrame(marker_genes).T.items():
         overlap_temp = []
         gs_names_temp = []
-        
+
         for gs_name, gs in gs_dict.items():
             marker_set_len_dict[gs_name] = len(gs)
-            overlap_temp.append(overlap_coefficient(set(gs),set(v)))
+            overlap_temp.append(overlap_coefficient(set(gs), set(v)))
             gs_names_temp.append(gs_name)
-        overlap_df_temp = pd.DataFrame(overlap_temp, columns=[i],index=gs_names_temp).T
-        overlap_df = pd.concat([overlap_df,overlap_df_temp])
-    overlap_df.loc['gene_set_length'] = list(overlap_df.columns.map(marker_set_len_dict))
-
-    #find maximum overlap coefficient gene set label for each factor, resolve ties by gene set length
-    marker_gene_labels = [] #gene sets
-    
+        overlap_df_temp = pd.DataFrame(overlap_temp, columns=[i], index=gs_names_temp).T
+        overlap_df = pd.concat([overlap_df, overlap_df_temp])
+    overlap_df.loc["gene_set_length"] = list(
+        overlap_df.columns.map(marker_set_len_dict)
+    )
+
+    # find maximum overlap coefficient gene set label for each factor, resolve ties by gene set length
+    marker_gene_labels = []  # gene sets
+
     marker_gene_list = list(overlap_df.index)
-    marker_gene_list.remove('gene_set_length')
+    marker_gene_list.remove("gene_set_length")
     for marker_set in marker_gene_list:
-        #resolve ties in overlap_coefficient by selecting the bigger gene set
-        max_overlap = overlap_df.loc[[marker_set,'gene_set_length']].T.sort_values(by='gene_set_length',ascending=True).sort_values(by=marker_set,ascending=True)[marker_set].index[-1]
-        
-        if overlap_df.loc[marker_set].sort_values().values[-1] >threshold:
+        # resolve ties in overlap_coefficient by selecting the bigger gene set
+        max_overlap = (
+            overlap_df.loc[[marker_set, "gene_set_length"]]
+            .T.sort_values(by="gene_set_length", ascending=True)
+            .sort_values(by=marker_set, ascending=True)[marker_set]
+            .index[-1]
+        )
+
+        if overlap_df.loc[marker_set].sort_values().values[-1] > threshold:
             marker_gene_labels.append(max_overlap)
         else:
             marker_gene_labels.append(marker_set)
-    overlap_df = overlap_df.drop(index='gene_set_length')
+    overlap_df = overlap_df.drop(index="gene_set_length")
     overlap_df.index = marker_gene_labels
     return overlap_df
 
 
-def amatrix(gene_set_list,gene2id):
-    """ 
+def amatrix(gene_set_list, gene2id):
+    """
     creates adjacency matrix from gene set list
-    """ 
+    """
     n = len(gene2id)
-    adj_matrix = np.zeros((n,n))
+    adj_matrix = np.zeros((n, n))
     for gene_set in gene_set_list:
         for i in range(len(gene_set)):
             for j in range(len(gene_set)):
                 g1 = gene_set[i]
                 g2 = gene_set[j]
-                if (g1 in gene2id)&(g2 in gene2id):
-                    adj_matrix[gene2id[g1],gene2id[g2]] = 1
+                if (g1 in gene2id) & (g2 in gene2id):
+                    adj_matrix[gene2id[g1], gene2id[g2]] = 1
     return adj_matrix
 
+
 def amatrix_weighted(gene_set_list, gene2id):
     """
     Creates weighted adjacency matrix from gene sets
-    uses 1/{n choose 2} as edge weights - edge weights accumulate additively  
+    uses 1/{n choose 2} as edge weights - edge weights accumulate additively
     """
     n = len(gene2id)
-    adj_matrix = np.zeros((n,n))
+    adj_matrix = np.zeros((n, n))
     ws = []
     for gene_set in gene_set_list:
         if len(gene_set) > 1:
-            w = 1.0/(len(gene_set)*(len(gene_set)-1)/2.0)
+            w = 1.0 / (len(gene_set) * (len(gene_set) - 1) / 2.0)
         else:
             w = 1.0
         ws.append(w)
         for i in range(len(gene_set)):
             for j in range(len(gene_set)):
                 g1 = gene_set[i]
                 g2 = gene_set[j]
-                if (g1 in gene2id)&(g2 in gene2id):
-                    adj_matrix[gene2id[g1],gene2id[g2]] += w
+                if (g1 in gene2id) & (g2 in gene2id):
+                    adj_matrix[gene2id[g1], gene2id[g2]] += w
     med = np.median(np.array(ws))
-    return adj_matrix/float(med)
+    return adj_matrix / float(med)
+
 
 def unravel_dict(dict_):
     lst = []
     for key in dict_.keys():
         lst.append(dict_[key])
-    return lst 
-def process_gene_sets(gs_dict, gene2id, weighted = True):
-    """ 
+    return lst
+
+
+def process_gene_sets(gs_dict, gene2id, weighted=True):
+    """
     { "global": {"<gene set name>": [<gene 1>, <gene 2>, ...]}
     }
-    """ 
+    """
     adict = OrderedDict()
     adict["global"] = amatrix(unravel_dict(gs_dict["global"]), gene2id)
-    weights = None 
+    weights = None
 
     if weighted:
         weights = OrderedDict()
         weights["global"] = amatrix_weighted(unravel_dict(gs_dict["global"]), gene2id)
 
     for key in gs_dict.keys():
         if len(gs_dict[key]) > 0:
-            adict[key] = amatrix(unravel_dict(gs_dict[key]),gene2id) 
+            adict[key] = amatrix(unravel_dict(gs_dict[key]), gene2id)
             if weighted:
                 weights[key] = amatrix_weighted(unravel_dict(gs_dict[key]), gene2id)
-        else: 
+        else:
             adict[key] = []
             if weighted:
                 weights[key] = []
 
     return adict, weights
 
-def process_gene_sets_no_celltypes(gs_dict, gene2id, weighted = True):
-    """ 
+
+def process_gene_sets_no_celltypes(gs_dict, gene2id, weighted=True):
+    """
     input: {"<gene set name>": [<gene 1>, <gene 2>, ...]}
     }
-    gene2id {gene name: index in vocab} 
+    gene2id {gene name: index in vocab}
 
-    weighted: whether to return NoneType or weighted adjacency matrix 
+    weighted: whether to return NoneType or weighted adjacency matrix
     """
     adict = amatrix(unravel_dict(gs_dict), gene2id)
-    weights = None 
+    weights = None
     if weighted:
-        weights = amatrix_weighted(unravel_dict(gs_dict) , gene2id)
+        weights = amatrix_weighted(unravel_dict(gs_dict), gene2id)
     return adict, weights
 
 
-def get_factor_celltypes(adata, obs_key, cellscore_obsm_key = 'SPECTRA_cell_scores'):
-    '''
+def get_factor_celltypes(adata, obs_key, cellscore_obsm_key="SPECTRA_cell_scores"):
+    """
     Assigns Spectra factors to cell types by analyzing the factor cell scores.
     Cell type specific factors will have zero cell scores except in their respective cell type
-    
+
     adata: AnnData , object containing the Spectra output
     obs_key: str , column name in adata.obs containing the cell type annotations
     cellscore_obsm_key: str , key for adata.obsm containing the Spectra cell scores
-    
+
     returns: dict , dictionary of {factor index : 'cell type'}
-    '''
-    
-    #get cellscores
+    """
+
+    # get cellscores
     import pandas as pd
+
     cell_scores_df = pd.DataFrame(adata.obsm[cellscore_obsm_key])
-    cell_scores_df['celltype'] = list(adata.obs[obs_key])
-    
-    #find global and cell type specific fators
-    global_factors_series = (cell_scores_df.groupby('celltype').mean() !=0).all()
-    global_factors = [factor for factor in global_factors_series.index if global_factors_series[factor]]
-    specific_cell_scores = (cell_scores_df.groupby('celltype').mean()).T[~global_factors_series].T
+    cell_scores_df["celltype"] = list(adata.obs[obs_key])
+
+    # find global and cell type specific fators
+    global_factors_series = (cell_scores_df.groupby("celltype").mean() != 0).all()
+    global_factors = [
+        factor
+        for factor in global_factors_series.index
+        if global_factors_series[factor]
+    ]
+    specific_cell_scores = (
+        (cell_scores_df.groupby("celltype").mean()).T[~global_factors_series].T
+    )
     specific_factors = {}
-    
-    for i in set(cell_scores_df['celltype']):
-        specific_factors[i]=[factor for factor in specific_cell_scores.loc[i].index if specific_cell_scores.loc[i,factor]]
-    
-    #inverse dict factor:celltype
+
+    for i in set(cell_scores_df["celltype"]):
+        specific_factors[i] = [
+            factor
+            for factor in specific_cell_scores.loc[i].index
+            if specific_cell_scores.loc[i, factor]
+        ]
+
+    # inverse dict factor:celltype
     factors_inv = {}
-    for i,v in specific_factors.items():
+    for i, v in specific_factors.items():
         for factor in v:
-            factors_inv[factor]=i
-    
-    #add global
+            factors_inv[factor] = i
+
+    # add global
 
     for factor in global_factors:
-        factors_inv[factor]= 'global'
-            
+        factors_inv[factor] = "global"
+
     return factors_inv
 
 
-#importance and information score functions 
-import torch 
+# importance and information score functions
+import torch
 
 
-def mimno_coherence_single(w1,w2,W):
+def mimno_coherence_single(w1, w2, W):
     eps = 0.01
     dw1 = W[:, w1] > 0
     dw2 = W[:, w2] > 0
     N = W.shape[0]
 
-    dw1w2 = (dw1 & dw2).float().sum() 
-    dw1 = dw1.float().sum() 
-    dw2 = dw2.float().sum() 
-    if (dw1 == 0)|(dw2 == 0):
-        return(-.1*np.inf)
-    return ((dw1w2 + 1)/(dw2)).log()
+    dw1w2 = (dw1 & dw2).float().sum()
+    dw1 = dw1.float().sum()
+    dw2 = dw2.float().sum()
+    if (dw1 == 0) | (dw2 == 0):
+        return -0.1 * np.inf
+    return ((dw1w2 + 1) / (dw2)).log()
+
 
-def mimno_coherence_2011(words, W): 
+def mimno_coherence_2011(words, W):
     score = 0
-    V= len(words)
+    V = len(words)
 
     for j1 in range(1, V):
         for j2 in range(j1):
             score += mimno_coherence_single(words[j1], words[j2], W)
-    denom = V*(V-1)/2
-    return(score/denom)
+    denom = V * (V - 1) / 2
+    return score / denom
 
 
-
-def holdout_loss(model, adata, cell_type,labels):
+def holdout_loss(model, adata, cell_type, labels):
     if "spectra_vocab" not in adata.var.columns:
-        print("adata requires spectra_vocab attribute.") 
+        print("adata requires spectra_vocab attribute.")
         return None
-    
+
     idx_to_use = adata.var["spectra_vocab"]
     X = adata.X[:, idx_to_use]
     if type(X) == scipy.sparse.csr.csr_matrix:
-        X = np.array(X.todense()) 
+        X = np.array(X.todense())
     X = torch.Tensor(X)
     loss_cf = 0.0
-    theta_global = torch.softmax(model.internal_model.theta["global"], dim = 1)
-    eta_global = (model.internal_model.eta["global"]).exp()/(1.0 + (model.internal_model.eta["global"]).exp())
-    eta_global = 0.5*(eta_global + eta_global.T)
-    gene_scaling_global = model.internal_model.gene_scaling["global"].exp()/(1.0 + model.internal_model.gene_scaling["global"].exp())
-    kappa_global = model.internal_model.kappa["global"].exp()/(1 + model.internal_model.kappa["global"].exp())
-    rho_global = model.internal_model.rho["global"].exp()/(1. + model.internal_model.rho["global"].exp())
-    #loop through cell types and evaluate loss at every cell type
-
-    kappa = model.internal_model.kappa[cell_type].exp()/(1 + model.internal_model.kappa[cell_type].exp())
-    rho = model.internal_model.rho[cell_type].exp()/(1 + model.internal_model.rho[cell_type].exp())
-    gene_scaling_ct = model.internal_model.gene_scaling[cell_type].exp()/(1.0 + model.internal_model.gene_scaling[cell_type].exp())
+    theta_global = torch.softmax(model.internal_model.theta["global"], dim=1)
+    eta_global = (model.internal_model.eta["global"]).exp() / (
+        1.0 + (model.internal_model.eta["global"]).exp()
+    )
+    eta_global = 0.5 * (eta_global + eta_global.T)
+    gene_scaling_global = model.internal_model.gene_scaling["global"].exp() / (
+        1.0 + model.internal_model.gene_scaling["global"].exp()
+    )
+    kappa_global = model.internal_model.kappa["global"].exp() / (
+        1 + model.internal_model.kappa["global"].exp()
+    )
+    rho_global = model.internal_model.rho["global"].exp() / (
+        1.0 + model.internal_model.rho["global"].exp()
+    )
+    # loop through cell types and evaluate loss at every cell type
+
+    kappa = model.internal_model.kappa[cell_type].exp() / (
+        1 + model.internal_model.kappa[cell_type].exp()
+    )
+    rho = model.internal_model.rho[cell_type].exp() / (
+        1 + model.internal_model.rho[cell_type].exp()
+    )
+    gene_scaling_ct = model.internal_model.gene_scaling[cell_type].exp() / (
+        1.0 + model.internal_model.gene_scaling[cell_type].exp()
+    )
     X_c = X[labels == cell_type]
-    adj_matrix = model.internal_model.adj_matrix[cell_type] 
+    adj_matrix = model.internal_model.adj_matrix[cell_type]
     weights = model.internal_model.weights[cell_type]
     adj_matrix_1m = model.internal_model.adj_matrix_1m[cell_type]
-    theta_ct = torch.softmax(model.internal_model.theta[cell_type], dim = 1)
-    eta_ct = (model.internal_model.eta[cell_type]).exp()/(1.0 + (model.internal_model.eta[cell_type]).exp())
-    eta_ct = 0.5*(eta_ct + eta_ct.T)
-    theta_global_ = contract('jk,j->jk',theta_global, gene_scaling_global + model.internal_model.delta)
-    theta_ct_ = contract('jk,j->jk',theta_ct, gene_scaling_ct + model.internal_model.delta)
-    theta = torch.cat((theta_global_, theta_ct_),1)
+    theta_ct = torch.softmax(model.internal_model.theta[cell_type], dim=1)
+    eta_ct = (model.internal_model.eta[cell_type]).exp() / (
+        1.0 + (model.internal_model.eta[cell_type]).exp()
+    )
+    eta_ct = 0.5 * (eta_ct + eta_ct.T)
+    theta_global_ = contract(
+        "jk,j->jk", theta_global, gene_scaling_global + model.internal_model.delta
+    )
+    theta_ct_ = contract(
+        "jk,j->jk", theta_ct, gene_scaling_ct + model.internal_model.delta
+    )
+    theta = torch.cat((theta_global_, theta_ct_), 1)
     alpha = torch.exp(model.internal_model.alpha[cell_type])
-    
-    recon = contract('ik,jk->ij', alpha, theta) 
-    term1 = -1.0*(torch.xlogy(X_c,recon) - recon).sum()
-    tot_loss = model.internal_model.lam*term1
-    
+
+    recon = contract("ik,jk->ij", alpha, theta)
+    term1 = -1.0 * (torch.xlogy(X_c, recon) - recon).sum()
+    tot_loss = model.internal_model.lam * term1
+
     lst = []
     for j in range(theta.shape[1]):
         mask = torch.ones(theta.shape[1])
         mask[j] = 0
-        mask = mask.reshape(1,-1)
-        recon = contract('ik,jk->ij', alpha, theta*mask) 
-        term1 = -1.0*(torch.xlogy(X_c,recon) - recon).sum()
-        loss_cf = model.internal_model.lam*term1
-        lst.append(((loss_cf - tot_loss)/tot_loss).detach().numpy().item())
-        
-    return(np.array(lst))
+        mask = mask.reshape(1, -1)
+        recon = contract("ik,jk->ij", alpha, theta * mask)
+        term1 = -1.0 * (torch.xlogy(X_c, recon) - recon).sum()
+        loss_cf = model.internal_model.lam * term1
+        lst.append(((loss_cf - tot_loss) / tot_loss).detach().numpy().item())
+
+    return np.array(lst)
+
+
 def get_information_score(adata, idxs, cell_type):
     if "spectra_vocab" not in adata.var.columns:
         print("adata requires spectra_vocab attribute.")
         return None
 
     idx_to_use = adata.var["spectra_vocab"]
     X = adata.X[:, idx_to_use]
     if type(X) == scipy.sparse.csr.csr_matrix:
         X = np.array(X.todense())
     X = torch.Tensor(X)
     lst = []
-    for j in range(idxs.shape[0]):
-        lst.append(mimno_coherence_2011(list(idxs[j,:]), X[labels == cell_type]))
-    return(lst)
+    # TODO: Fix undefined "labels" variable
+    # for j in range(idxs.shape[0]):
+    # lst.append(mimno_coherence_2011(list(idxs[j,:]), X[labels == cell_type]))
+    return lst
+
+
 """
 def plot_scores(info_scores, importance_scores, eta):
     plt.figure(figsize=(12, 8))
 
     # Create a scatter plot of all the points
     plt.scatter(info_scores, importance_scores, c=eta, cmap="coolwarm", edgecolors="black")
```

### Comparing `scSpectra-0.1.0/Spectra/attend.py` & `scspectra-0.2.0/src/Spectra/attend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,125 +1,143 @@
 """
 
 """
 
+
 class attend(nn.Module):
     """
-    per (i,j): 
-    
+    per (i,j):
+
     X \approx lam* (g_j + delta) <Theta_i, Eps_proj * Gamma_j>
-    
+
     Penalize KL(A, Gamma) / lam
-    
+
     Parameters:
-    
+
     g
     Theta
     Eps
     Gamma
-    
+
     -----
-    
-    Usage : 
-    bin_matrix = # binary gene set matrix 
-    
+
+    Usage :
+    bin_matrix = # binary gene set matrix
+
     bin_matrix = (bin_matrix + 0.001)/(bin_matrix + 0.001).sum(axis = 0)
     model = attend(X = X, K = 30, gene_set_matrix = bin_matrix, delta = 0.0, lam = 10e-5, beta = 10e-1)
     epsilon = model.assignments.softmax(dim = 1).detach().numpy()
     """
-    def __init__(self, X, K, gene_set_matrix, delta = 0.001, lam = 10e-4,beta = 3.0):
+
+    def __init__(self, X, K, gene_set_matrix, delta=0.001, lam=10e-4, beta=3.0):
         super(attend, self).__init__()
         self.p = X.shape[1]
         self.n = X.shape[0]
-        self.K = K 
-        self.X = torch.Tensor(X) 
+        self.K = K
+        self.X = torch.Tensor(X)
         self.gene_set_matrix = torch.Tensor(gene_set_matrix)
         self.L = gene_set_matrix.shape[0]
-        self.lambda_ = lam 
+        self.lambda_ = lam
         self.delta = delta
         self.beta = beta
-        self.theta = nn.Parameter(Normal(0.,1.).sample([self.n, self.K]))
-        self.gamma = nn.Parameter(Normal(0.,1.).sample([self.p, self.L]))
-        self.gene_scalings = nn.Parameter(Normal(0.,1.).sample([self.p]))
-        self.assignments = nn.Parameter(Normal(0.,1.).sample([self.K,self.L]))
-    
-    def loss(self): 
-        #compute the Poisson reconstruction loss
-        gamma = self.gamma.softmax(dim = 1)
+        self.theta = nn.Parameter(Normal(0.0, 1.0).sample([self.n, self.K]))
+        self.gamma = nn.Parameter(Normal(0.0, 1.0).sample([self.p, self.L]))
+        self.gene_scalings = nn.Parameter(Normal(0.0, 1.0).sample([self.p]))
+        self.assignments = nn.Parameter(Normal(0.0, 1.0).sample([self.K, self.L]))
+
+    def loss(self):
+        # compute the Poisson reconstruction loss
+        gamma = self.gamma.softmax(dim=1)
         theta = self.theta.exp()
-        gene_scaling = self.gene_scalings.exp()/(1 + self.gene_scalings.exp())
-        epsilon = self.assignments.softmax(dim = 1)
-        reconstruction  = contract('il,lj,kj,k->ik',theta,epsilon,gamma,gene_scaling + self.delta)
-        loss_1 = (-1*torch.xlogy(self.X, reconstruction) + reconstruction).sum()
-        #compute loss between gamma and gene set matrix
-        loss_2 = -1*torch.xlogy(self.gene_set_matrix,gamma.T).sum()
-        loss_3 = -1*torch.logdet(contract('ij,kj->ik',epsilon, epsilon))
-        
-        #loss_2 = -1*torch.corrcoef(self.gene_set_matrix,gamma.T)
-        return self.lambda_*loss_1 + loss_2 + self.beta*loss_3
+        gene_scaling = self.gene_scalings.exp() / (1 + self.gene_scalings.exp())
+        epsilon = self.assignments.softmax(dim=1)
+        reconstruction = contract(
+            "il,lj,kj,k->ik", theta, epsilon, gamma, gene_scaling + self.delta
+        )
+        loss_1 = (-1 * torch.xlogy(self.X, reconstruction) + reconstruction).sum()
+        # compute loss between gamma and gene set matrix
+        loss_2 = -1 * torch.xlogy(self.gene_set_matrix, gamma.T).sum()
+        loss_3 = -1 * torch.logdet(contract("ij,kj->ik", epsilon, epsilon))
+
+        # loss_2 = -1*torch.corrcoef(self.gene_set_matrix,gamma.T)
+        return self.lambda_ * loss_1 + loss_2 + self.beta * loss_3
+
     def store_parameters(self):
         self.cell_scores = 0
         self.factors = 0
-        
-        
+
+
 def return_factors(model):
-    gamma = model.gamma.softmax(dim = 1)
-    gene_scaling = model.gene_scalings.exp()/(1 + model.gene_scalings.exp())
-    epsilon = model.assignments.softmax(dim = 1)
-    factor_unscaled  = contract('lj,kj,k->lk',epsilon,gamma,gene_scaling + model.delta).detach().numpy()
-    factor_scaled = factor_unscaled/(factor_unscaled.sum(axis = 0) + 0.01)
+    gamma = model.gamma.softmax(dim=1)
+    gene_scaling = model.gene_scalings.exp() / (1 + model.gene_scalings.exp())
+    epsilon = model.assignments.softmax(dim=1)
+    factor_unscaled = (
+        contract("lj,kj,k->lk", epsilon, gamma, gene_scaling + model.delta)
+        .detach()
+        .numpy()
+    )
+    factor_scaled = factor_unscaled / (factor_unscaled.sum(axis=0) + 0.01)
     return factor_scaled
 
-def return_markers(factor_matrix, id2word,n_top_vals = 100):
-    idx_matrix = np.argsort(factor_matrix,axis = 1)[:,::-1][:,:n_top_vals]
+
+def return_markers(factor_matrix, id2word, n_top_vals=100):
+    idx_matrix = np.argsort(factor_matrix, axis=1)[:, ::-1][:, :n_top_vals]
     df = pd.DataFrame(np.zeros(idx_matrix.shape))
     for i in range(idx_matrix.shape[0]):
         for j in range(idx_matrix.shape[1]):
-            df.iloc[i,j] = id2word[idx_matrix[i,j]]
+            df.iloc[i, j] = id2word[idx_matrix[i, j]]
     return df
 
-def matching(markers, gene_names_dict, threshold = 0.4):
-        """
-        best match based on overlap coefficient
-        """
-        
-        matches = []
-        jaccards = []
-        for i in range(markers.shape[0]):
-            max_jacc = 0.0 
-            best = ""
-            for key in gene_names_dict.keys():
-                t = gene_names_dict[key]
-
-                jacc = spectra_util.overlap_coefficient(list(markers.iloc[i,:]),t)
-                if jacc > max_jacc:
-                    max_jacc = jacc
-                    best = key 
-            matches.append(best)
-            jaccards.append(max_jacc)
-        
-        return matches,jaccards
-        
-        
-def train(model, lr_schedule = [1.0,.5,.1,.01,.001,.0001],num_epochs = 10000, verbose = False): 
-        opt = torch.optim.Adam(model.parameters(), lr=lr_schedule[0])
-        counter = 0
-        last = np.inf
-
-        for i in tqdm(range(num_epochs)):
-            #print(counter)
-            opt.zero_grad()
-            
-            loss = model.loss()
-            
-            loss.backward()
-            opt.step()
-        
-            if loss.item() >= last:
-                counter += 1
-                if int(counter/3) >= len(lr_schedule):
-                    break
-                if counter % 3 == 0:
-                    opt = torch.optim.Adam(model.parameters(), lr=lr_schedule[int(counter/3)])
-                    if verbose:
-                        print("UPDATING LR TO " + str(lr_schedule[int(counter/3)]))
-            last = loss.item() 
+
+def matching(markers, gene_names_dict, threshold=0.4):
+    """
+    best match based on overlap coefficient
+    """
+
+    matches = []
+    jaccards = []
+    for i in range(markers.shape[0]):
+        max_jacc = 0.0
+        best = ""
+        for key in gene_names_dict.keys():
+            t = gene_names_dict[key]
+
+            jacc = spectra_util.overlap_coefficient(list(markers.iloc[i, :]), t)
+            if jacc > max_jacc:
+                max_jacc = jacc
+                best = key
+        matches.append(best)
+        jaccards.append(max_jacc)
+
+    return matches, jaccards
+
+
+def train(
+    model,
+    lr_schedule=[1.0, 0.5, 0.1, 0.01, 0.001, 0.0001],
+    num_epochs=10000,
+    verbose=False,
+):
+    opt = torch.optim.Adam(model.parameters(), lr=lr_schedule[0])
+    counter = 0
+    last = np.inf
+
+    for i in tqdm(range(num_epochs)):
+        # print(counter)
+        opt.zero_grad()
+
+        loss = model.loss()
+
+        loss.backward()
+        opt.step()
+
+        if loss.item() >= last:
+            counter += 1
+            if int(counter / 3) >= len(lr_schedule):
+                break
+            if counter % 3 == 0:
+                opt = torch.optim.Adam(
+                    model.parameters(), lr=lr_schedule[int(counter / 3)]
+                )
+                if verbose:
+                    print("UPDATING LR TO " + str(lr_schedule[int(counter / 3)]))
+        last = loss.item()
```

### Comparing `scSpectra-0.1.0/Spectra/data/default_gene_sets.json` & `scspectra-0.2.0/src/Spectra/data/default_gene_sets.json`

 * *Files identical despite different names*

### Comparing `scSpectra-0.1.0/Spectra/data/sample_data.h5ad` & `scspectra-0.2.0/src/Spectra/data/sample_data.h5ad`

 * *Files identical despite different names*

### Comparing `scSpectra-0.1.0/Spectra/initialization.py` & `scspectra-0.2.0/src/Spectra/initialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-import torch 
-import numpy as np 
+import torch
+import numpy as np
 from collections import OrderedDict
 
-def mimno_coherence_single(w1,w2,W):
+
+def mimno_coherence_single(w1, w2, W):
     eps = 0.01
     dw1 = W[:, w1] > 0
     dw2 = W[:, w2] > 0
     N = W.shape[0]
 
-    dw1w2 = (dw1 & dw2).float().sum() 
-    dw1 = dw1.float().sum() 
-    dw2 = dw2.float().sum() 
+    dw1w2 = (dw1 & dw2).float().sum()
+    dw1 = dw1.float().sum()
+    dw2 = dw2.float().sum()
+
+    return ((dw1w2 + 1) / (dw2)).log()
 
-    return ((dw1w2 + 1)/(dw2)).log()
 
-def mimno_coherence_2011(words, W): 
+def mimno_coherence_2011(words, W):
     score = 0
-    V= len(words)
+    V = len(words)
 
     for j1 in range(1, V):
         for j2 in range(j1):
             score += mimno_coherence_single(words[j1], words[j2], W)
-    denom = V*(V-1)/2
-    return(score/denom)
+    denom = V * (V - 1) / 2
+    return score / denom
+
 
 def compute_init_scores_noct(gs_dict, word2id, W):
     init_scores = OrderedDict()
-    keys = list(gs_dict.keys()) 
-    for key in keys: 
-        gs = gs_dict[key] 
-        idxs = [] 
+    keys = list(gs_dict.keys())
+    for key in keys:
+        gs = gs_dict[key]
+        idxs = []
         for word in gs:
             if word in word2id:
                 idxs.append(word2id[word])
-        #idxs = [word2id[word] for word in gs] 
-        coh = mimno_coherence_2011(idxs,W)
-        init_scores[key] = coh.item() 
+        # idxs = [word2id[word] for word in gs]
+        coh = mimno_coherence_2011(idxs, W)
+        init_scores[key] = coh.item()
     return init_scores
-        
+
+
 def compute_init_scores(gs_dict, word2id, W):
     keys = list(gs_dict.keys())
     init_scores = OrderedDict()
     for key in keys:
         if len(gs_dict[key]) > 0:
             inner_keys = list(gs_dict[key].keys())
-            init_scores[key] = OrderedDict() 
+            init_scores[key] = OrderedDict()
             for inner_key in inner_keys:
                 gs = gs_dict[key][inner_key]
-                idxs = [] 
-                for word in gs: 
+                idxs = []
+                for word in gs:
                     if word in word2id:
                         idxs.append(word2id[word])
-                #idxs = [word2id[word] for word in gs]
+                # idxs = [word2id[word] for word in gs]
                 coh = mimno_coherence_2011(idxs, W)
-                init_scores[key][inner_key] = coh.item() 
-        else: 
-            init_scores[key] = {} 
-            
-        
-    return init_scores 
+                init_scores[key][inner_key] = coh.item()
+        else:
+            init_scores[key] = {}
 
+    return init_scores
```

