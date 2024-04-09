# Comparing `tmp/baypy-1.1.2.tar.gz` & `tmp/baypy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baypy-1.1.2.tar", last modified: Mon Mar 18 22:46:35 2024, max compression
+gzip compressed data, was "dist/baypy-1.2.0.tar", last modified: Tue Apr  9 16:31:42 2024, max compression
```

## Comparing `baypy-1.1.2.tar` & `baypy-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-18 22:46:35.000000 baypy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-18 22:46:25.000000 baypy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/analysis/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/diagnostics/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy/model/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20363 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/model/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/regression/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/regression/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/regression/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-03-18 22:46:25.000000 baypy-1.1.2/baypy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-18 22:46:35.000000 baypy-1.1.2/baypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 22:46:35.000000 baypy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-18 22:46:25.000000 baypy-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-09 16:31:42.000000 baypy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-09 16:31:32.000000 baypy-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/analysis/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/diagnostics/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/model/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:31:42.000000 baypy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-09 16:31:32.000000 baypy-1.2.0/setup.py
```

### Comparing `baypy-1.1.2/baypy/analysis/functions.py` & `baypy-1.2.0/baypy/analysis/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import matplotlib.pyplot as plt
 from ..model import Model
 import numpy as np
 import pandas as pd
-from scipy.stats import gaussian_kde, norm
-from ..utils import flatten_matrix, matrices_to_frame
+from scipy.stats import gaussian_kde
+from ..utils import flatten_matrix
 
 
 def trace_plot(posteriors: dict) -> None:
-    """Plots the traces and the probability density for each posterior.
+    """it plots the traces and the probability density for each posterior. \n
     The plot shows the traces for each Markov chain, for each regression variable and the relative posterior density.
     The plot layout has number of rows equal to the number of regression variables and two columns: traces on the left
     and densities on the right.
 
     Parameters
     ----------
-    posteriors : dict
-        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-        with a number of rows equal to the number of iterations and a number of columns equal to the number of Markov
-        chains.
-
-    Raises
-    ------
-    TypeError
-        - If ``posteriors`` is not a ``dict``,
-        - if a posterior sample is not a ``numpy.ndarray``.
-    KeyError
-        If ``posteriors`` does not contain ``intercept`` key.
-    ValueError
-        If a posterior sample is an empty ``numpy.ndarray``.
-
-    See Also
-    --------
-    :py:class:`baypy.regression.linear_regression.LinearRegression`
+    ``posteriors`` : :py:class:`dict`
+        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+        :py:class:`numpy.ndarray` with a number of rows equal to the number of iterations and a number of columns equal
+        to the number of Markov chains.
+
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``posteriors`` is not a :py:class:`dict`,
+           - if a posterior sample is not a :py:class:`numpy.ndarray`.
+       ``KeyError``
+           If ``posteriors`` does not contain ``'intercept'`` key.
+       ``ValueError``
+           If a posterior sample is an empty :py:class:`numpy.ndarray`.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>`
     """
     if not isinstance(posteriors, dict):
         raise TypeError("Parameter 'posteriors' must be a dictionary")
 
     if not all([isinstance(posterior_sample, np.ndarray) for posterior_sample in posteriors.values()]):
         raise TypeError("All posteriors data must be an instance of 'numpy.ndarray'")
 
@@ -79,60 +81,62 @@
     posterior_support = np.linspace(np.min(posterior), np.max(posterior), 1000)
     posterior_kde = gaussian_kde(posterior)(posterior_support)
 
     return posterior_support, posterior_kde
 
 
 def summary(posteriors: dict, alpha: float = 0.05, quantiles: list = None, print_summary: bool = True) -> dict:
-    """Prints a statistical summary for each posterior.
+    """It prints a statistical summary for each posterior.
 
     Parameters
     ----------
-    posteriors : dict
-        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-        with a number of rows equal to the number of iterations and a number of columns equal to the number of Markov
-        chains.
-    alpha : float
+    ``posteriors`` : :py:class:`dict`
+        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+        :py:class:`numpy.ndarray` with a number of rows equal to the number of iterations and a number of columns equal
+        to the number of Markov chains.
+    ``alpha`` : :py:class:`float`, optional
         Significance level. It is used to compute the Highest Posterior Density (HPD) interval. It must be between ``0``
-        and ``1``.
-    quantiles : list, optional
+        and ``1``. Default is ``0.05``.
+    ``quantiles`` : :py:class:`list`, optional
         List of the quantiles to compute, for each posterior. It cannot be empty. It must contain only float between
         ``0`` and ``1``. Default is ``[0.025, 0.25, 0.5, 0.75, 0.975]``.
-    print_summary : bool, optional
+    ``print_summary`` : :py:class:`bool`, optional
         If ``True`` prints the statistical posterior summary report. Default is ``True``.
 
     Returns
     -------
-    dict
+    :py:class:`dict`
         Dictionary with statistical summary of posteriors. It contains:
-            - key ``n_chain``, the number of Markov chains,
-            - key ``n_iterations``, the number of regression iterations,
-            - key ``summary``, the statistical summary of the posteriors, as a pandas.DataFrame,
-            - key ``quantiles``, quantiles summary of the posteriors, as a pandas.DataFrame.
-
-    Raises
-    ------
-    TypeError
-        - If ``posteriors`` is not a ``dict``,
-        - if a posterior sample is not a ``numpy.ndarray``,
-        - if ``alpha`` is not a ``float``,
-        - if ``quantiles`` is not a ``list``,
-        - if a ``quantiles`` value is not a ``float``,
-        - if ``print_summary`` is not a ``bool``.
-    KeyError
-        If ``posteriors`` does not contain ``intercept`` key.
-    ValueError
-        - If a posterior sample is an empty ``numpy.ndarray``,
-        - if ``alpha`` is not between ``0`` and ``1``,
-        - if ``quantiles`` is an empty ``list``,
-        - if a ``quantiles`` value is not between ``0`` and ``1``.
-
-    See Also
-    --------
-    :py:class:`baypy.regression.linear_regression.LinearRegression`
+            - key ``'n_chain'``, the number of Markov chains,
+            - key ``'n_iterations'``, the number of regression iterations,
+            - key ``'summary'``, the statistical summary of the posteriors, as a :py:class:`pandas.DataFrame`,
+            - key ``'quantiles'``, quantiles summary of the posteriors, as a :py:class:`pandas.DataFrame`.
+
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``posteriors`` is not a :py:class:`dict`,
+           - if a posterior sample is not a :py:class:`numpy.ndarray`,
+           - if ``alpha`` is not a :py:class:`float`,
+           - if ``quantiles`` is not a :py:class:`list`,
+           - if a ``quantiles`` value is not a :py:class:`float`,
+           - if ``print_summary`` is not a :py:class:`bool`.
+       ``KeyError``
+           If ``posteriors`` does not contain ``'intercept'`` key.
+       ``ValueError``
+           - If a posterior sample is an empty :py:class:`numpy.ndarray`,
+           - if ``alpha`` is not between ``0`` and ``1``,
+           - if ``quantiles`` is an empty :py:class:`list`,
+           - if a ``quantiles`` value is not between ``0`` and ``1``.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>`
     """
     if not isinstance(posteriors, dict):
         raise TypeError("Parameter 'posteriors' must be a dictionary")
 
     if not all([isinstance(posterior_sample, np.ndarray) for posterior_sample in posteriors.values()]):
         raise TypeError("All posteriors data must be an instance of 'numpy.ndarray'")
 
@@ -191,15 +195,15 @@
         print(f'Number of chains:      {n_chains:>6}')
         print(f'Sample size per chian: {n_iterations:>6}')
         print()
         print(f'Empirical mean, standard deviation, {credibility_mass} HPD interval for each variable:')
         print()
         print(general_summary.to_string())
         print()
-        print(f'Quantiles for each variable:')
+        print('Quantiles for each variable:')
         print()
         print(quantiles_summary.to_string())
 
     return {'n_chains': n_chains, 'n_iterations': n_iterations,
             'summary': general_summary, 'quantiles': quantiles_summary}
 
 
@@ -215,179 +219,186 @@
     hpdi_min = x[min_idx]
     hpdi_max = x[min_idx + interval_idx_included]
 
     return hpdi_min, hpdi_max
 
 
 def residuals_plot(model: Model) -> None:
-    r"""Plots the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
+    r"""It plots the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
 
     Parameters
     ----------
-    model : baypy.model.model.Model
+    ``model`` : :py:class:`Model <baypy.model.model.Model>`
         The model with data, regressors, response variable and priors to be solved through Monte Carlo sampling.
 
-    Raises
-    ------
-    TypeError
-        If ``model`` is not a ``baypy.model.model.Model``.
-    ValueError
-        - If a ``model.posteriors`` is ``None`` because the sampling has not been done yet,
-        - if a posterior key is not a column of ``model.data``,
-        - if ``model.data`` is an empty ``pandas.DataFrame``,
-        - if ``model.response_variable`` is not a column of ``model.data``.
-
-    See Also
-    --------
-    :py:class:`baypy.regression.linear_regression.LinearRegression`
-
-    Notes
-    -----
-    Predicted values are computed at data points :math:`X` using the posteriors means for each regressor's parameter.
-    In the case of linear model:
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           If ``model`` is not a :py:class:`Model <baypy.model.model.Model>`.
+       ``ValueError``
+           - If a ``model.posteriors`` is :py:obj:`None` because the sampling has not been done yet,
+           - if a posterior key is not a column of ``model.data``,
+           - if ``model.data`` is an empty :py:class:`pandas.DataFrame`,
+           - if ``model.response_variable`` is not a column of ``model.data``.
+
+    .. admonition:: Notes
+       :class: tip
+
+       Predicted values are computed at data points :math:`X` using the posteriors means for each regressor's parameter.
+       In the case of linear model:
+
+       .. math::
+           \hat{y_i} = \beta_0 + \sum_{j = 1}^{m} \beta_j x_{i,j}
 
-    .. math::
-        \hat{y_i} = \beta_0 + \sum_{j = 1}^{m} \beta_j x_{i,j}
+       while residuals are the difference between the observed values and the predicted values of the
+       ``response_variable``:
 
-    while residuals are the difference between the observed values and the predicted values of the
-    ``response_variable``:
+       .. math::
+           \epsilon_i = y_i - \hat{y_i}
 
-    .. math::
-        \epsilon_i = y_i - \hat{y_i}
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>`
     """
     if not isinstance(model, Model):
         raise TypeError(f"Parameter 'model' must be an instance of '{Model.__module__}.{Model.__name__}'")
 
     if model.posteriors is None:
         raise ValueError("Posteriors not available, run 'baypy.regression.Regression.sample' to generate posteriors")
 
-    for posterior, posterior_samples in model.posteriors.items():
+    for posterior in model.posteriors.keys():
         if (posterior not in ['intercept', 'variance']) and (posterior not in model.data.columns):
             raise ValueError(f"Column '{posterior}' not found in 'model.data'")
 
     if model.data.empty:
         raise ValueError("Parameter 'model.data' cannot be an empty 'pandas.DataFrame'")
 
     if model.response_variable not in model.data.columns:
         raise ValueError(f"Column '{model.response_variable}' not found in 'model.data'")
 
     data = model.residuals()
 
-    fig, ax = plt.subplots()
+    _, ax = plt.subplots()
 
     ax.plot(data['predicted'], data['residuals'], marker = 'o', linestyle = '', alpha = 0.5)
 
     ax.set_xlabel('Predicted')
     ax.set_ylabel('Residuals')
 
     ax.tick_params(bottom = False, top = False, left = False, right = False)
 
     plt.tight_layout()
 
     plt.show()
 
 
 def compute_DIC(model: Model, print_summary: bool = True) -> dict:
-    r"""Computes and prints the Deviance Information Criterion (DIC) for the fitted model.
+    r"""It computes and prints the Deviance Information Criterion (DIC) for the fitted model.
 
     Parameters
     ----------
-    model : baypy.model.model.Model
+    ``model`` : :py:class:`Model <baypy.model.model.Model>`
         The model with data, regressors, response variable and priors to be solved through Monte Carlo sampling.
-    print_summary : bool, optional
+    ``print_summary`` : :py:class:`bool`, optional
         If ``True`` prints the deviance summary report. Default is ``True``.
 
     Returns
     -------
-    dict
+    :py:class:`dict`
         Dictionary with deviance summary. It contains:
-            - key ``deviance at posterior means``,
-            - key ``posterior mean deviance``,
-            - key ``effective number of parameters``,
-            - key ``DIC``.
-
-    Raises
-    ------
-    TypeError
-        - If ``model`` is not a ``baypy.model.model.Model``,
-        - if ``print_summary`` is not a ``bool``.
-    ValueError
-        - If a ``model.posteriors`` is ``None`` because the sampling has not been done yet,
-        - if a posterior key is not a column of ``model.data``,
-        - if ``model.data`` is an empty ``pandas.DataFrame``,
-        - if ``model.response_variable`` is not a column of ``model.data``.
-
-    See Also
-    --------
-    :py:class:`baypy.regression.linear_regression.LinearRegression`
-
-    Notes
-    -----
-    The DIC measures posterior predictive error by penalizing the fit of a model (deviance) by its complexity,
-    determined by the effective number of parameters.
-    Comparing some alternative models, the smaller the DIC of a model, the *better* the model.
-    Consider a linear regression of the response variable :math:`y` with respect to regressors :math:`X`, according to
-    the following model:
-
-    .. math::
-        y \sim N(\mu, \sigma^2)
-    .. math::
-        \mu = \beta_0 + B X = \beta_0 + \sum_{j = 1}^m \beta_j x_j
-
-    then the *likelyhood* is:
-
-    .. math::
-        p \left( y \left\vert B,\sigma^2 \right. \right) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp{- \frac{\left(y - \mu
-        \right)^2}{2 \sigma^2}} .
-
-    The *deviance* [1]_ [2]_ is defined as:
-
-    .. math::
-        D \left( y, B, \sigma^2 \right) = -2\log p \left( y \left\vert B,\sigma^2 \right. \right) .
-
-    The *deviance* at posterior mean of :math:`B` and :math:`\sigma^2`, denoted by :math:`\overline{B}` and
-    :math:`\overline{\sigma^2}` is:
-
-    .. math::
-        D_{{\overline{\beta}}, \overline{\sigma^2}} (y) = D \left( y, \overline{B}, \overline{\sigma^2} \right)
-
-    while the posterior mean deviance is:
-
-    .. math::
-        \overline{D} \left( y, B, \sigma^2 \right) = E \left( D(y, B, \sigma^2) \left. \right\vert y \right) .
-
-    and the *effective number of parameter* is defined as:
-
-    .. math::
-        pD = \overline{D} \left( y, B, \sigma^2 \right) - D_{{\overline{\beta}}, \overline{\sigma^2}} (y) .
-
-    The *Deviance Information Criterion* [1]_ is:
-
-    .. math::
-        DIC = 2 \overline{D} \left( y, B, \sigma^2 \right) - D_{{\overline{\beta}}, \overline{\sigma^2}} (y) =
-        \overline{D} \left( y, B, \sigma^2 \right) + pD =
-        D_{{\overline{B}}, \overline{\sigma^2}} (y) + 2pD .
+            - key ``'Deviance at posterior means'``,
+            - key ``'Posterior mean deviance'``,
+            - key ``'Effective number of parameters'``,
+            - key ``'Deviance Information Criterion'``.
 
-    References
-    ----------
-    .. [1] O. Spiegelhalter DJ, Best NG, Carlin BP, van der Linde A. Bayesian measures of model complexity and fit.
-       J R Statist Soc B. 2002;64:583–616.
-    .. [2] Gelman A, Carlin JB, Stern HS, Rubin DS. Bayesian Data Analysis. 2. Chapman & Hall/CRC; Boca Raton,
-       Florida: 2004.
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``model`` is not a :py:class:`Model <baypy.model.model.Model>`,
+           - if ``print_summary`` is not a :py:class:`bool`.
+       ``ValueError``
+           - If a ``model.posteriors`` is :py:obj:`None` because the sampling has not been done yet,
+           - if a posterior key is not a column of ``model.data``,
+           - if ``model.data`` is an empty :py:class:`pandas.DataFrame`,
+           - if ``model.response_variable`` is not a column of ``model.data``.
+
+    .. admonition:: Notes
+       :class: tip
+
+       The DIC measures posterior predictive error by penalizing the fit of a model (deviance) by its complexity,
+       determined by the effective number of parameters.
+       Comparing some alternative models, the smaller the DIC of a model, the *better* the model.
+       Consider a linear regression of the response variable :math:`y` with respect to regressors :math:`X`, according
+       to the following model:
+
+       .. math::
+           y \sim N(\mu, \sigma^2)
+       .. math::
+           \mu = \beta_0 + B X = \beta_0 + \sum_{j = 1}^m \beta_j x_j
+
+       then the *likelyhood* is:
+
+       .. math::
+           p \left( y \left\vert B,\sigma^2 \right. \right) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp{- \frac{\left(y - \mu
+           \right)^2}{2 \sigma^2}} .
+
+       The *deviance* [1]_ [2]_ is defined as:
+
+       .. math::
+           D \left( y, B, \sigma^2 \right) = -2\log p \left( y \left\vert B,\sigma^2 \right. \right) .
+
+       The *deviance* at posterior mean of :math:`B` and :math:`\sigma^2`, denoted by :math:`\overline{B}` and
+       :math:`\overline{\sigma^2}` is:
+
+       .. math::
+           D_{{\overline{\beta}}, \overline{\sigma^2}} (y) = D \left( y, \overline{B}, \overline{\sigma^2} \right)
+
+       while the posterior mean deviance is:
+
+       .. math::
+           \overline{D} \left( y, B, \sigma^2 \right) = E \left( D(y, B, \sigma^2) \left. \right\vert y \right) .
+
+       and the *effective number of parameter* is defined as:
+
+       .. math::
+           pD = \overline{D} \left( y, B, \sigma^2 \right) - D_{{\overline{\beta}}, \overline{\sigma^2}} (y) .
+
+       The *Deviance Information Criterion* [1]_ is:
+
+       .. math::
+           DIC = 2 \overline{D} \left( y, B, \sigma^2 \right) - D_{{\overline{\beta}}, \overline{\sigma^2}} (y) =
+           \overline{D} \left( y, B, \sigma^2 \right) + pD =
+           D_{{\overline{B}}, \overline{\sigma^2}} (y) + 2pD .
+
+    .. admonition:: References
+       :class: note
+
+       .. [1] O. Spiegelhalter DJ, Best NG, Carlin BP, van der Linde A. Bayesian measures of model complexity and fit.
+          J R Statist Soc B. 2002;64:583–616.
+       .. [2] Gelman A, Carlin JB, Stern HS, Rubin DS. Bayesian Data Analysis. 2. Chapman & Hall/CRC; Boca Raton,
+          Florida: 2004.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>`
     """
     if not isinstance(model, Model):
         raise TypeError(f"Parameter 'model' must be an instance of '{Model.__module__}.{Model.__name__}'")
 
     if model.posteriors is None:
         raise ValueError("Posteriors not available, run 'baypy.regression.Regression.sample' to generate posteriors")
 
     if not isinstance(print_summary, bool):
         raise TypeError("Parameter 'print_summary' must be a boolean")
 
-    for posterior, posterior_samples in model.posteriors.items():
+    for posterior, _ in model.posteriors.items():
         if (posterior not in ['intercept', 'variance']) and (posterior not in model.data.columns):
             raise ValueError(f"Column '{posterior}' not found in 'model.data'")
 
     if model.data.empty:
         raise ValueError("Parameter 'model.data' cannot be an empty 'pandas.DataFrame'")
 
     if model.response_variable not in model.data.columns:
@@ -397,21 +408,21 @@
     posterior_mean_deviance = _compute_posterior_mean_deviance(model = model)
     effective_number_of_parameters = posterior_mean_deviance - deviance_at_posterior_means
     DIC = effective_number_of_parameters + posterior_mean_deviance
 
     if print_summary:
         print(f"Deviance at posterior means     {deviance_at_posterior_means:>12.2f}")
         print(f"Posterior mean deviance         {posterior_mean_deviance:>12.2f}")
-        print(f"Effective number of parameteres {effective_number_of_parameters:>12.2f}")
-        print(f"Deviace Information Criterion   {DIC:>12.2f}")
+        print(f"Effective number of parameters  {effective_number_of_parameters:>12.2f}")
+        print(f"Deviance Information Criterion  {DIC:>12.2f}")
 
-    return {'deviance at posterior means': deviance_at_posterior_means,
-            'posterior mean deviance': posterior_mean_deviance,
-            'effective number of parameters': effective_number_of_parameters,
-            'DIC': DIC}
+    return {'Deviance at posterior means': deviance_at_posterior_means,
+            'Posterior mean deviance': posterior_mean_deviance,
+            'Effective number of parameters': effective_number_of_parameters,
+            'Deviance Information Criterion': DIC}
 
 
 def _compute_deviance_at_posterior_means(model: Model) -> float:
     data = model._compute_model_parameters_at_posterior_means()
     likelihood = model.likelihood(data = data)
 
     return -2*np.sum(np.log(likelihood))
```

### Comparing `baypy-1.1.2/baypy/diagnostics/functions.py` & `baypy-1.2.0/baypy/diagnostics/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from ..utils import flatten_matrix
 
 
 def autocorrelation_plot(posteriors: dict, max_lags: int = 30) -> None:
-    """Plots the auto-correlation for each Markov chain for each regression variable.
+    """It plots the auto-correlation for each Markov chain for each regression variable. \n
     The plot shows the auto-correlation trend from lag ``0`` (when auto-correlation is always ``1``) up to ``max_lags``.
     The plot layout has number of rows equal to the number of regression variables and a number of columns equal to the
     number of chains.
 
     Parameters
     ----------
-    posteriors : dict
-        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-        with a number of rows equal to the number of iterations and a number of columns equal to the number of Markov
-        chains.
-    max_lags : int, optional
+    ``posteriors`` : :py:class:`dict`
+        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+        :py:class:`numpy.ndarray` with a number of rows equal to the number of iterations and a number of columns equal
+        to the number of Markov chains.
+    ``max_lags`` : :py:class:`int`, optional
         Maximum number of lags to which compute the auto-correlation. The default is ``30``.
 
-    Raises
-    ------
-    TypeError
-        - If ``posteriors`` is not a ``dict``,
-        - if a posterior sample is not a ``numpy.ndarray``,
-        - if ``max_lags`` is not a ``int``.
-    KeyError
-        If ``posteriors`` does not contain ``intercept`` key.
-    ValueError
-        - If a posterior sample is an empty ``numpy.ndarray``,
-        - if ``max_lags`` is less or equal to ``0``.
-
-    See Also
-    --------
-    :py:func:`baypy.diagnostics.functions.autocorrelation_summary`
-    :py:func:`baypy.diagnostics.functions.effective_sample_size`
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``posteriors`` is not a :py:class:`dict`,
+           - if a posterior sample is not a :py:class:`numpy.ndarray`,
+           - if ``max_lags`` is not an :py:class:`int`.
+       ``KeyError``
+           If ``posteriors`` does not contain ``'intercept'`` key.
+       ``ValueError``
+           - If a posterior sample is an empty :py:class:`numpy.ndarray`,
+           - if ``max_lags`` is less or equal to ``0``.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:func:`autocorrelation_summary <baypy.diagnostics.functions.autocorrelation_summary>` \n
+       :py:func:`effective_sample_size <baypy.diagnostics.functions.effective_sample_size>`
     """
     if not isinstance(posteriors, dict):
         raise TypeError("Parameter 'posteriors' must be a dictionary")
 
     if not all([isinstance(posterior_sample, np.ndarray) for posterior_sample in posteriors.values()]):
         raise TypeError("All posteriors data must be an instance of 'numpy.ndarray'")
 
@@ -54,15 +56,15 @@
     if max_lags <= 0:
         raise ValueError("Parameter 'max_lags' must be greater than 0")
 
     variable_names = list(posteriors.keys())
     n_variables = len(variable_names)
     n_iterations, n_chains = posteriors['intercept'].shape
 
-    fig, ax = plt.subplots(nrows = n_variables,
+    _, ax = plt.subplots(nrows = n_variables,
                            ncols = n_chains,
                            figsize = (min(1.5*n_chains + 3, 10), min(1.5*n_variables + 2, 10)),
                            sharex = 'all',
                            sharey = 'all')
 
     if n_chains > 1:
         for k in range(n_chains):
@@ -100,59 +102,62 @@
         plt.tight_layout()
         plt.subplots_adjust(left = 0.14)
 
     plt.show()
 
 
 def autocorrelation_summary(posteriors: dict, lags: list = None, print_summary: bool = True) -> pd.DataFrame:
-    """Prints the auto-correlation summary for each regression variable.
+    """It prints the auto-correlation summary for each regression variable. \n
     The summary reports the auto-correlation values at the lags listed in ``lags``.
 
     Parameters
     ----------
-    posteriors : dict
-        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-        with a number of rows equal to the number of iterations and a number of columns equal to the number of Markov
-        chains.
-    lags : list, optional
-        List of the lags to which compute the auto-correlation. It cannot be an empty ``list``. It must contain only
-        positive integers. The default is ``[0, 1, 5, 10, 30]``.
-    print_summary : bool, optional
+    ``posteriors`` : :py:class:`dict`
+        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+        :py:class:`numpy.ndarray` with a number of rows equal to the number of iterations and a number of columns equal
+        to the number of Markov chains.
+    ``lags`` : :py:class:`list`, optional
+        List of the lags to which compute the auto-correlation. It cannot be an empty :py:class:`list`. It must contain
+        only positive integers. The default is ``[0, 1, 5, 10, 30]``.
+    ``print_summary`` : :py:class:`bool`, optional
         If ``True`` prints the autocorrelation summary report. Default is ``True``.
 
     Returns
     -------
-    pd.DataFrame
+    :py:class:`pandas.DataFrame`
         The dataframe with a number of row equal to the number of element in ``lags`` and a number of columns equal to
         the number of model variables. Lags are reported in dataframe index.
 
-    Raises
-    ------
-    TypeError
-        - If ``posteriors`` is not a ``dict``,
-        - if a posterior sample is not a ``numpy.ndarray``,
-        - if ``lags`` is not a ``list``,
-        - if ``lags`` does not contain only ``int``,
-        - if ``print_summary`` is not a ``bool``.
-    KeyError
-        If ``posteriors`` does not contain ``intercept`` key.
-    ValueError
-        - If a posterior sample is an empty ``numpy.ndarray``,
-        - if ``lags`` is an empty ``list``,
-        - if a value in ``lags`` is a negative ``int``.
-
-    See Also
-    --------
-    :py:func:`baypy.diagnostics.functions.autocorrelation_plot`
-    :py:func:`baypy.diagnostics.functions.effective_sample_size`
-
-    Notes
-    -----
-    The reported auto-correlation for each variable is a mean of auto-correlations for the chains of that variable, for
-    each chain.
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``posteriors`` is not a :py:class:`dict`,
+           - if a posterior sample is not a :py:class:`numpy.ndarray`,
+           - if ``lags`` is not a :py:class:`list`,
+           - if ``lags`` does not contain only :py:class:`int`,
+           - if ``print_summary`` is not a :py:class:`bool`.
+       ``KeyError``
+           If ``posteriors`` does not contain ``'intercept'`` key.
+       ``ValueError``
+           - If a posterior sample is an empty :py:class:`numpy.ndarray`,
+           - if ``lags`` is an empty :py:class:`list`,
+           - if a value in ``lags`` is a negative :py:class:`int`.
+
+    .. admonition:: Notes
+       :class: tip
+
+       The reported auto-correlation for each variable is a mean of auto-correlations for the chains of that variable,
+       for each chain.
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:func:`autocorrelation_plot <baypy.diagnostics.functions.autocorrelation_plot>` \n
+       :py:func:`effective_sample_size <baypy.diagnostics.functions.effective_sample_size>`
     """
     if not isinstance(posteriors, dict):
         raise TypeError("Parameter 'posteriors' must be a dictionary")
 
     if not all([isinstance(posterior_sample, np.ndarray) for posterior_sample in posteriors.values()]):
         raise TypeError("All posteriors data must be an instance of 'numpy.ndarray'")
 
@@ -194,52 +199,55 @@
     if print_summary:
         print(acorr_summary.to_string())
 
     return acorr_summary
 
 
 def effective_sample_size(posteriors: dict, print_summary: bool = True) -> pd.DataFrame:
-    """Computes and prints the effective number of sample for each posterior.
+    """It computes and prints the effective number of sample for each posterior.
 
     Parameters
     ----------
-    posteriors : dict
-        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-        with a number of rows equals to the number of iterations and a number of columns equal to the number of Markov
-        chains.
-    print_summary : bool, optional
+    ``posteriors`` : :py:class:`dict`
+        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+        :py:class:`numpy.ndarray` with a number of rows equals to the number of iterations and a number of columns equal
+        to the number of Markov chains.
+    ``print_summary`` : :py:class:`bool`, optional
         If ``True`` prints the effective sample size summary report. Default is ``True``.
 
     Returns
     -------
-    pd.DataFrame
+    :py:class:`pandas.DataFrame`
         The dataframe with a single row and a number of columns equal to the number of model variables. The unique index
-        of the dataframe is ``Effective Sample Size``.
+        of the dataframe is ``'Effective Sample Size'``.
+
+    .. admonition:: Raises
+       :class: warning
+
+       ``TypeError``
+           - If ``posteriors`` is not a :py:class:`dict`,
+           - if a posterior sample is not a :py:class:`numpy.ndarray`,
+           - if ``print_summary`` is not a :py:class:`bool`.
+       ``KeyError``
+           If ``posteriors`` does not contain ``'intercept'`` key.
+       ``ValueError``
+           If a posterior sample is an empty :py:class:`numpy.ndarray`.
+
+    .. admonition:: Notes
+       :class: tip
+
+       The effective number of sample could be theoretically equal to the number of iterations in case of no
+       auto-correlation of the Markov chain. The greater the auto-correlation of the Markov chain, the smaller the
+       effective sample size of the posterior.
+
+    .. admonition:: See Also
+       :class: seealso
 
-    Raises
-    ------
-    TypeError
-        - If ``posteriors`` is not a ``dict``,
-        - if a posterior sample is not a ``numpy.ndarray``,
-        - if ``print_summary`` is not a ``bool``.
-    KeyError
-        If ``posteriors`` does not contain ``intercept`` key.
-    ValueError
-        If a posterior sample is an empty ``numpy.ndarray``.
-
-    See Also
-    --------
-    :py:func:`baypy.diagnostics.functions.autocorrelation_plot`
-    :py:func:`baypy.diagnostics.functions.autocorrelation_summary`
-
-    Notes
-    -----
-    The effective number of sample could be theoretically equal to the number of iterations in case of no
-    auto-correlation of the Markov chain. The greater the auto-correlation of the Markov chain, the smaller the
-    effective sample size of the posterior.
+       :py:func:`autocorrelation_plot <baypy.diagnostics.functions.autocorrelation_plot>` \n
+       :py:func:`autocorrelation_summary <baypy.diagnostics.functions.autocorrelation_summary>`
     """
     if not isinstance(posteriors, dict):
         raise TypeError("Parameter 'posteriors' must be a dictionary")
 
     if not all([isinstance(posterior_sample, np.ndarray) for posterior_sample in posteriors.values()]):
         raise TypeError("All posteriors data must be an instance of 'numpy.ndarray'")
```

### Comparing `baypy-1.1.2/baypy/model/linear_model.py` & `baypy-1.2.0/baypy/model/linear_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,45 +2,46 @@
 import pandas as pd
 import numpy as np
 from scipy.stats import norm
 from ..utils import flatten_matrix, matrices_to_frame, dot_product
 
 
 class LinearModel(Model):
-    r"""baypy.model.model.LinearModel object.
+    r""":py:class:`LinearModel <baypy.model.linear_model.LinearModel>` object.
 
     Attributes
     ----------
-    :py:attr:`baypy.model.linear_model.LinearModel.data` : pandas.DataFrame
-        Data for the linear regression model, is a ``pandas.DataFrame`` containing all regressor variables
+    :py:attr:`data` : :py:class:`pandas.DataFrame`
+        Data for the linear regression model, is a :py:class:`pandas.DataFrame` containing all regressor variables
         :math:`X` and the response variable :math:`y`.
-    :py:attr:`baypy.model.linear_model.LinearModel.response_variable` : string
+    :py:attr:`response_variable` : :py:class:`str`
         Response variable :math:`y` of the linear model.
-    :py:attr:`baypy.model.linear_model.LinearModel.priors` : dict
+    :py:attr:`priors` : :py:class:`dict`
         Priors for the regressors' and variance parameters.
-    :py:attr:`baypy.model.linear_model.LinearModel.variable_names` : list
-        The list of all model variables: the regressors :math:`X`, including the ``intercept`` and the ``variance``
+    :py:attr:`variable_names` : :py:class:`list`
+        The list of all model variables: the regressors :math:`X`, including the ``'intercept'`` and the ``'variance'``
         :math:`\sigma^2`.
-    :py:attr:`baypy.model.linear_model.LinearModel.posteriors` : dict
-        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-        with a number of rows equals to the number of iterations and a number of columns equal to the number of Markov
-        chains.
+    :py:attr:`posteriors` : :py:class:`dict`
+        Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+        :py:class:`numpy.ndarray` with a number of rows equals to the number of iterations and a number of columns equal
+        to the number of Markov chains.
 
     Methods
     -------
-    :py:meth:`baypy.model.linear_model.LinearModel.posteriors_to_frame()`
-        Organizes the ``posteriors`` in a ``pandas.DataFrame``.
-    :py:meth:`baypy.model.linear_model.LinearModel.residuals`
-        Compute the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
-    :py:meth:`baypy.model.linear_model.LinearModel.predict_distribution`
-        Predicts a posterior distribution for an unobserved values.
-    :py:meth:`baypy.model.linear_model.LinearModel.likelihood`
-        Computes the likelihood of observations ``model.response_variable`` given a model ``'mean'`` and ``'variance'``.
-    :py:meth:`baypy.model.linear_model.LinearModel.log_likelihood`
-        Computes the log likelihood of observations ``model.response_variable`` given a model ``'mean'`` and
+    :py:meth:`posteriors_to_frame`
+        It organizes the ``posteriors`` in a :py:class:`pandas.DataFrame`.
+    :py:meth:`residuals`
+        It computes the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
+    :py:meth:`predict_distribution`
+        It predicts a posterior distribution for an unobserved values.
+    :py:meth:`likelihood`
+        It computes the likelihood of observations :py:attr:`response_variable` given a model ``'mean'`` and
+        ``'variance'``.
+    :py:meth:`log_likelihood`
+        It computes the log likelihood of observations :py:attr:`response_variable` given a model ``'mean'`` and
         ``'variance'``.
     """
 
 
     def __init__(self):
 
         self.__data = None
@@ -48,31 +49,31 @@
         self.__priors = None
         self.__variable_names = None
         self.__posteriors = None
 
 
     @property
     def data(self) -> pd.DataFrame:
-        r"""Data for the linear regression model, is a ``pandas.DataFrame`` containing all regressor variables
+        r"""Data for the linear regression model, is a :py:class:`pandas.DataFrame` containing all regressor variables
         :math:`X` and the response variable :math:`y`.
 
         Returns
         -------
-        pandas.DataFrame
+        :py:class:`pandas.DataFrame`
             Observed data of the model. It cannot be empty. It must contain regressor variables :math:`X` and the
-            response variable :math:`y`.
+            :py:attr:`response_variable` :math:`y`.
+
+        .. admonition:: Raises
+           :class: warning
 
-        Raises
-        ------
-        TypeError
-            If :py:attr:`data` is not an instance of ``pandas.DataFrame``.
-        ValueError
-            If :py:attr:`data` is an empty ``pandas.DataFrame``.
+           ``TypeError``
+               If :py:attr:`data` is not an instance of :py:class:`pandas.DataFrame`.
+           ``ValueError``
+               If :py:attr:`data` is an empty :py:class:`pandas.DataFrame`.
         """
-        assert super().data is None
         return self.__data
 
 
     @data.setter
     def data(self, data: pd.DataFrame) -> None:
         super(LinearModel, type(self)).data.fset(self, data)
         self.__data = data
@@ -80,108 +81,110 @@
 
     @property
     def response_variable(self) -> str:
         r"""Response variable :math:`y` of the linear model.
 
         Returns
         -------
-        string
+        :py:class:`str`
             Name of the response variable :math:`y`. In must be one of the columns of :py:attr:`data`.
 
-        Raises
-        ------
-        TypeError
-            If :py:attr:`response_variable` is not a ``str``.
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If :py:attr:`response_variable` is not a :py:class:`str`.
         """
-        assert super().response_variable is None
         return self.__response_variable
 
 
     @response_variable.setter
     def response_variable(self, response_variable: str) -> None:
         super(LinearModel, type(self)).response_variable.fset(self, response_variable)
         self.__response_variable = response_variable
 
 
     @property
     def priors(self) -> dict:
         r"""Priors for the regressors' and variance parameters.
-        Each prior is a key-value pair, where the value is a ``dict`` with:
+        Each prior is a key-value pair, where the value is a :py:class:`dict` with:
 
         - hyperparameter names as keys
         - hyperparameter values as values.
 
         Returns
         -------
-        dict
-            Priors for each random variable. It must contain an ``intercept`` and a ``variance`` keys. Each value must
-            be a ``dict`` with hyperparameter names as key and hyperparameter values as values.
-
-        Raises
-        ------
-        TypeError
-            - If :py:attr:`priors` is not a ``dict``,
-            - if a :py:attr:`priors`' value is not a ``dict``.
-        ValueError
-            - If :py:attr:`priors` is an empty ``dict``,
-            - if a :py:attr:`priors`' value is an empty ``dict``,
-            - if a ``variance`` value is not positive,
-            - if a ``shape`` value is not positive,
-            - if a ``scale`` value is not positive.
-        KeyError
-            - If :py:attr:`priors` does not contain both ``intercept`` and ``variance`` keys,
-            - if a prior's hyperparameters are not:
-                + ``mean`` and ``variance`` for a regression parameter :math:`\beta_j` or
-                + ``shape`` and ``scale`` for ``variance`` :math:`\sigma^2`.
-
-        Notes
-        -----
-        To each random variables is assigned a prior distribution:
-
-        - to each regressor parameter :math:`\beta_j` is assigned a normal prior distribution with hyperparameters
-          ``mean`` :math:`\beta_j^0` and ``variance`` :math:`\Sigma_{\beta_j}^0`:
-
-          .. math::
-            \beta_j \sim N(\beta_j^0 , \Sigma_{\beta_j}^0)
-
-        - to variance :math:`\sigma^2` is assigned an inverse gamma distribution with hyperparameters ``shape``
-          :math:`\kappa^0` and ``scale`` :math:`\theta^0`:
-
-          .. math::
-            \sigma^2 \sim \text{Inv-}\Gamma(\kappa^0, \theta^0)
-
-        Examples
-        --------
-        Consider a linear regression of the response variable :math:`y` with respect to regressors :math:`x_1`,
-        :math:`x_2` and :math:`x_3`, according to the following model:
-
-        .. math::
-            y \sim N(\mu, \sigma^2)
-        .. math::
-            \mu = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \beta_3 x_3
-
-        then the sampler would require priors for:
-            - parameter :math:`\beta_0` of variable ``intercept``, with ``mean`` :math:`\beta_0^0` and ``variance``
-              :math:`\Sigma_{\beta_0}^0`
-            - parameter :math:`\beta_1` of variable :math:`x_1`, with ``mean`` :math:`\beta_1^0` and ``variance``
-              :math:`\Sigma_{\beta_1}^0`
-            - parameter :math:`\beta_2` of variable :math:`x_2`, with ``mean`` :math:`\beta_2^0` and ``variance``
-              :math:`\Sigma_{\beta_2}^0`
-            - parameter :math:`\beta_3` of variable :math:`x_3`, with ``mean`` :math:`\beta_3^0` and ``variance``
-              :math:`\Sigma_{\beta_3}^0`
-            - variable :math:`\sigma^2`, with ``shape`` :math:`\kappa^0` and ``scale`` :math:`\theta^0`
-
-        >>> model = baypy.model.LinearModel()
-        >>> model.set_priors({'intercept': {'mean': 0, 'variance': 1e6},
-        ...                   'x_1': {'mean': 0, 'variance': 1e6},
-        ...                   'x_2': {'mean': 0, 'variance': 1e6},
-        ...                   'x_3': {'mean': 0, 'variance': 1e6},
-        ...                   'variance': {'shape': 1, 'scale': 1e-6}})
+        :py:class:`dict`
+            Priors for each random variable. It must contain an ``'intercept'`` and a ``'variance'`` keys. Each value
+            must be a :py:class:`dict` with hyperparameter names as key and hyperparameter values as values.
+
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If :py:attr:`priors` is not a :py:class:`dict`,
+               - if a :py:attr:`priors`' value is not a :py:class:`dict`.
+           ``ValueError``
+               - If :py:attr:`priors` is an empty :py:class:`dict`,
+               - if a :py:attr:`priors`' value is an empty :py:class:`dict`,
+               - if a ``'variance'`` value is not positive,
+               - if a ``'shape'`` value is not positive,
+               - if a ``'scale'`` value is not positive.
+           ``KeyError``
+               - If :py:attr:`priors` does not contain both ``'intercept'`` and ``'variance'`` keys,
+               - if a prior's hyperparameters are not:
+                   + ``'mean'`` and ``'variance'`` for a regression parameter :math:`\beta_j` or
+                   + ``'shape'`` and ``'scale'`` for ``variance`` :math:`\sigma^2`.
+
+        .. admonition:: Notes
+           :class: tip
+
+           To each random variables is assigned a prior distribution:
+
+           - to each regressor parameter :math:`\beta_j` is assigned a normal prior distribution with hyperparameters
+             ``'mean'`` :math:`\beta_j^0` and ``'variance'`` :math:`\Sigma_{\beta_j}^0`:
+
+             .. math::
+               \beta_j \sim N(\beta_j^0 , \Sigma_{\beta_j}^0)
+
+           - to variance :math:`\sigma^2` is assigned an inverse gamma distribution with hyperparameters ``'shape'``
+             :math:`\kappa^0` and ``'scale'`` :math:`\theta^0`:
+
+             .. math::
+               \sigma^2 \sim \text{Inv-}\Gamma(\kappa^0, \theta^0)
+
+        .. admonition:: Examples
+           :class: important
+
+           Consider a linear regression of the :py:attr:`response_variable` :math:`y` with respect to regressors :math:`x_1`,
+           :math:`x_2` and :math:`x_3`, according to the following model:
+
+           .. math::
+               y \sim N(\mu, \sigma^2)
+           .. math::
+               \mu = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \beta_3 x_3
+
+           then the sampler would require priors for:
+               - parameter :math:`\beta_0` of variable ``'intercept'``, with ``'mean'`` :math:`\beta_0^0` and
+                 ``'variance'`` :math:`\Sigma_{\beta_0}^0`
+               - parameter :math:`\beta_1` of variable :math:`x_1`, with ``'mean'`` :math:`\beta_1^0` and ``'variance'``
+                 :math:`\Sigma_{\beta_1}^0`
+               - parameter :math:`\beta_2` of variable :math:`x_2`, with ``'mean'`` :math:`\beta_2^0` and ``'variance'``
+                 :math:`\Sigma_{\beta_2}^0`
+               - parameter :math:`\beta_3` of variable :math:`x_3`, with ``'mean'`` :math:`\beta_3^0` and ``'variance'``
+                 :math:`\Sigma_{\beta_3}^0`
+               - variable :math:`\sigma^2`, with ``'shape'`` :math:`\kappa^0` and ``'scale'`` :math:`\theta^0`
+
+           >>> model = baypy.model.LinearModel()
+           >>> model.priors = {'intercept': {'mean': 0, 'variance': 1e6},
+           ...                 'x_1': {'mean': 0, 'variance': 1e6},
+           ...                 'x_2': {'mean': 0, 'variance': 1e6},
+           ...                 'x_3': {'mean': 0, 'variance': 1e6},
+           ...                 'variance': {'shape': 1, 'scale': 1e-6}}
         """
-        assert super().priors is None
         return self.__priors
 
 
     @priors.setter
     def priors(self, priors: dict) -> None:
         super(LinearModel, type(self)).priors.fset(self, priors)
 
@@ -214,114 +217,114 @@
 
     @property
     def variable_names(self) -> list:
         r"""Variables of the linear model.
 
         Returns
         -------
-        list
-            The list of all model variables: the regressors :math:`X`, including the ``intercept`` and the ``variance``
-            :math:`\sigma^2`.
+        :py:class:`list`
+            The list of all model variables: the regressors :math:`X`, including the ``'intercept'`` and the
+            ``'variance'`` :math:`\sigma^2`.
         """
-        assert super().variable_names is None
         return self.__variable_names
 
 
     @property
     def posteriors(self) -> dict:
         r"""Posteriors of the regressors' and variance parameters.
-        Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
+        Posteriors and relative samples are key-value pairs. Each sample is a :py:class:`numpy.ndarray`
         with a number of rows equals to the number of iterations and a number of columns equal to the number of Markov
         chains.
 
         Returns
         -------
-        dict
-            Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a ``numpy.ndarray``
-            with a number of rows equals to the number of iterations and a number of columns equal to the number of
-            Markov chains.
-
-        Raises
-        ------
-        TypeError
-            - If :py:attr:`posteriors` is not a ``dict``,
-            - if a posterior sample is not a ``numpy.ndarray``.
-        KeyError
-            If :py:attr:`posteriors` does not contain both ``intercept`` and ``variance`` keys.
-        ValueError
-            If a posterior sample is an empty ``numpy.ndarray``.
+        :py:class:`dict`
+            Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
+            :py:class:`numpy.ndarray` with a number of rows equals to the number of iterations and a number of columns
+            equal to the number of Markov chains.
+
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If :py:attr:`posteriors` is not a :py:class:`dict`,
+               - if a posterior sample is not a :py:class:`numpy.ndarray`.
+           ``KeyError``
+               If :py:attr:`posteriors` does not contain both ``'intercept'`` and ``'variance'`` keys.
+           ``ValueError``
+               If a posterior sample is an empty :py:class:`numpy.ndarray`.
         """
-        assert super().posteriors is None
         return self.__posteriors
 
 
     @posteriors.setter
     def posteriors(self, posteriors: dict) -> None:
         super(LinearModel, type(self)).posteriors.fset(self, posteriors)
 
         if 'variance' not in posteriors.keys():
             raise KeyError("Parameter 'posteriors' must contain a 'variance' key")
 
         self.__posteriors = posteriors
 
 
     def posteriors_to_frame(self) -> pd.DataFrame:
-        """Organizes the :py:attr:`posteriors` in a ``pandas.DataFrame``. Each posterior is a frame column. The length
-        of the frame is the number of sampling iterations times the number of sampling chains.
+        """It organizes the :py:attr:`posteriors` in a :py:class:`pandas.DataFrame`. Each posterior is a frame column.
+        The length of the frame is the number of sampling iterations times the number of sampling chains.
 
         Returns
         -------
-        pandas.DataFrame
-            Returns posterior samples. Posteriors are organized in a ``pandas.DataFrame``, one for each column. The
-            length of the frame is the number of sampling iterations times the number of sampling chains.
-
-        Raises
-        ------
-        ValueError
-            If :py:attr:`posteriors` are not available because the method
-            :py:meth:`baypy.regression.LinearRegression.sample` has not been called yet.
+        :py:class:`pandas.DataFrame`
+            Returns posterior samples. Posteriors are organized in a :py:class:`pandas.DataFrame`, one for each column.
+            The length of the frame is the number of sampling iterations times the number of sampling chains.
+
+        .. admonition:: Raises
+           :class: warning
+
+           ``ValueError``
+               If :py:attr:`posteriors` are not available because the method
+               :py:meth:`LinearRegression.sample <baypy.regression.linear_regression.LinearRegression.sample>` has not
+               been called yet.
         """
-        assert super().posteriors_to_frame() is None
         if self.__posteriors is None:
             raise ValueError("Posteriors not available, run 'baypy.regression.LinearRegression.sample' to generate "
                              "posteriors")
         return matrices_to_frame(matrices_dict = self.__posteriors)
 
 
     def residuals(self) -> pd.DataFrame:
-        r"""Compute the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
+        r"""It compute the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
 
         Returns
         -------
-        pandas.DataFrame
-            Returns a copy of :py:attr:`data` with 3 more columns: ``intercept``, ``predicted`` and ``residuals``.
+        :py:class:`pandas.DataFrame`
+            Returns a copy of :py:attr:`data` with 3 more columns: ``'intercept'``, ``'predicted'`` and ``'residuals'``.
 
-        Raises
-        ------
-        ValueError
-            - If :py:attr:`data` is ``None`` because the property :py:attr:`data` has not been set,
-            - if :py:attr:`response_variable` is not a column of :py:attr:`data`,
-            - If a :py:attr:`posteriors` is ``None`` because the sampling has not been done yet.
-
-        Notes
-        -----
-        Predicted values are computed at data points :math:`X` using the posteriors means for each regressor's
-        parameter:
+        .. admonition:: Raises
+           :class: warning
 
-        .. math::
-            \hat{y_i} = \beta_0 + \sum_{j = 1}^{m} \beta_j x_{i,j}
+           ``ValueError``
+               - If :py:attr:`data` is :py:obj:`None` because the property :py:attr:`data` has not been set,
+               - if :py:attr:`response_variable` is not a column of :py:attr:`data`,
+               - If a :py:attr:`posteriors` is :py:obj:`None` because the sampling has not been done yet.
 
-        while residuals are the difference between the observed values and the predicted values of the
-        :py:attr:`response_variable`:
+        .. admonition:: Notes
+           :class: tip
 
-        .. math::
-            \epsilon_i = y_i - \hat{y_i}
-        """
-        assert super().residuals() is None
+           Predicted values are computed at data points :math:`X` using the posteriors means for each regressor's
+           parameter:
+
+           .. math::
+               \hat{y_i} = \beta_0 + \sum_{j = 1}^{m} \beta_j x_{i,j}
+
+           while residuals are the difference between the observed values and the predicted values of the
+           :py:attr:`response_variable`:
 
+           .. math::
+               \epsilon_i = y_i - \hat{y_i}
+        """
         if self.__data is None:
             raise ValueError("Data not available, set data with 'baypy.model.LinearModel.data")
 
         if self.__response_variable not in self.__data.columns:
             raise ValueError(f"Column '{self.__response_variable}' not found in 'data'")
 
         if self.__posteriors is None:
@@ -336,41 +339,43 @@
         data['predicted'] = dot_product(data = data, regressors = posterior_means)
         data['residuals'] = data[self.__response_variable] - data['predicted']
 
         return data
 
 
     def predict_distribution(self, predictors: dict) -> np.ndarray:
-        """Predicts a posterior distribution for an unobserved values. For each posterior sample, it draws a sample from
-         the likelihood.
+        """It predicts a posterior distribution for an unobserved values. For each posterior sample, it draws a sample
+        from the likelihood.
 
         Parameters
         ----------
-        predictors : dict
+        ``predictors`` : :py:class:`dict`
             Values of predictors :math:`X` at which compute the posterior distribution. Each predictor has to be set as
             a key-value pair.
 
         Returns
         -------
-        numpy.ndarray
+        :py:class:`numpy.ndarray`
             Array of the predicted posterior distribution. It contains a number of element equal to the number of
             regression iterations times the number of model Markov chains.
 
-        Raises
-        ------
-        TypeError
-            If ``predictors`` is not a ``dict``.
-        KeyError
-            If a ``predictors`` key is not a key of ``posteriors``.
-        ValueError
-            If ``predictors`` is an empty ``dict``.
-
-        See Also
-        --------
-        :py:class:`baypy.regression.linear_regression.LinearRegression`
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If ``predictors`` is not a :py:class:`dict`.
+           ``KeyError``
+               If a ``predictors`` key is not a key of :py:attr:`posteriors`.
+           ``ValueError``
+               If ``predictors`` is an empty :py:class:`dict`.
+
+        .. admonition:: See Also
+           :class: seealso
+
+           :py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>`
         """
         super().predict_distribution(predictors = predictors)
 
         for regressor in predictors.keys():
             if regressor not in self.__posteriors.keys():
                 raise KeyError(f"Regressor '{regressor}' not found in 'posteriors' keys")
 
@@ -379,93 +384,97 @@
 
         return norm.rvs(loc = prediction['mean'],
                         scale = np.sqrt(prediction['variance']),
                         size = len(prediction))
 
 
     def likelihood(self, data: pd.DataFrame) -> np.ndarray:
-        r"""Computes the likelihood of observations :py:attr:`response_variable` given a model ``'mean'`` and
+        r"""It computes the likelihood of observations :py:attr:`response_variable` given a model ``'mean'`` and
         ``'variance'``.
 
         Parameters
         ----------
-        data: pandas.DataFrame
+        ``data``: :py:class:`pandas.DataFrame`
             Data to use for likelihood computation. It cannot be empty. It must contain columns
             :py:attr:`response_variable`, ``'mean'`` and ``'variance'``.
 
         Returns
         -------
-        numpy.ndarray
+        :py:class:`numpy.ndarray`
             Array of computed likelihood. It has the same length of ``data``. Each element is a likelihood computation
             of each row of ``data``.
 
-        Raises
-        ------
-        TypeError
-            If ``data`` is not an instance of ``pandas.DataFrame``.
-        ValueError
-            - If ``data`` is an empty ``pandas.DataFrame``,
-            - if :py:attr:`response_variable` is not a column of ``data``,
-            - if ``'mean'`` is not a column of ``data``,
-            - if ``'variance'`` is not a column of ``data``.
-
-        Notes
-        -----
-        The likelihood is computed with the normal distribution probability density function:
+        .. admonition:: Raises
+           :class: warning
 
-        .. math::
-            L(y) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp{- \frac{\left(y - \mu \right)^2}{2 \sigma^2}}
+           ``TypeError``
+               If ``data`` is not an instance of :py:class:`pandas.DataFrame`.
+           ``ValueError``
+               - If ``data`` is an empty :py:class:`pandas.DataFrame`,
+               - if :py:attr:`response_variable` is not a column of ``data``,
+               - if ``'mean'`` is not a column of ``data``,
+               - if ``'variance'`` is not a column of ``data``.
+
+        .. admonition:: Notes
+           :class: tip
 
-        where :math:`\mu` is the ``'mean'`` column and :math:`\sigma^2` is the ``'variance'`` column.
+           The likelihood is computed with the normal distribution probability density function:
+
+           .. math::
+               L(y) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp{- \frac{\left(y - \mu \right)^2}{2 \sigma^2}}
+
+           where :math:`\mu` is the ``'mean'`` column and :math:`\sigma^2` is the ``'variance'`` column.
         """
         super().likelihood(data = data)
 
         for col in [self.__response_variable, 'mean', 'variance']:
             if col not in data.columns:
                 raise ValueError(f"Column '{col}' not found in 'data'")
 
         return norm.pdf(x = data[self.__response_variable],
                         loc = data['mean'],
                         scale = np.sqrt(data['variance']))
 
 
     def log_likelihood(self, data: pd.DataFrame) -> np.ndarray:
-        r"""Computes the log likelihood of observations :py:attr:`response_variable` given a model ``'mean'`` and
+        r"""It computes the log likelihood of observations :py:attr:`response_variable` given a model ``'mean'`` and
         ``'variance'``.
 
         Parameters
         ----------
-        data: pandas.DataFrame
+        ``data``: :py:class:`pandas.DataFrame`
             Data to use for log likelihood computation. It cannot be empty. It must contain columns
             :py:attr:`response_variable`, ``'mean'`` and ``'variance'``.
 
         Returns
         -------
-        numpy.ndarray
+        :py:class:`numpy.ndarray`
             Array of computed log likelihood. It has the same length of ``data``. Each element is a log likelihood
             computation of each row of ``data``.
 
-        Raises
-        ------
-        TypeError
-            If ``data`` is not an instance of ``pandas.DataFrame``.
-        ValueError
-            - If ``data`` is an empty ``pandas.DataFrame``,
-            - if :py:attr:`response_variable` is not a column of ``data``,
-            - if ``'mean'`` is not a column of ``data``,
-            - if ``'variance'`` is not a column of ``data``.
-
-        Notes
-        -----
-        The log likelihood is computed as the log of the normal distribution probability density function:
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               If ``data`` is not an instance of :py:class:`pandas.DataFrame`.
+           ``ValueError``
+               - If ``data`` is an empty :py:class:`pandas.DataFrame`,
+               - if :py:attr:`response_variable` is not a column of ``data``,
+               - if ``'mean'`` is not a column of ``data``,
+               - if ``'variance'`` is not a column of ``data``.
+
+        .. admonition:: Notes
+           :class: tip
+
+           The log likelihood is computed as the log of the normal distribution probability density function:
 
-        .. math::
-            l(y) = - \frac{1}{2} \log{2 \pi \sigma^2} - \frac{1}{2} \frac{\left(y - \mu \right)^2}{\sigma^2}
+           .. math::
+               l(y) = - \frac{1}{2} \log{2 \pi \sigma^2} - \frac{1}{2} \frac{\left(y - \mu \right)^2}{\sigma^2}
 
-        where :math:`\mu` is the ``'mean'`` column and :math:`\sigma^2` is the ``'variance'`` column.
+           where :math:`\mu` is the ``'mean'`` column and :math:`\sigma^2` is the ``'variance'`` column.
         """
         super().log_likelihood(data = data)
 
         for col in [self.__response_variable, 'mean', 'variance']:
             if col not in data.columns:
                 raise ValueError(f"Column '{col}' not found in 'data'")
```

### Comparing `baypy-1.1.2/baypy/model/model.py` & `baypy-1.2.0/baypy/model/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from abc import ABC, abstractmethod
 import numpy as np
 import pandas as pd
 
 
 class Model(ABC):
+    """:py:class:`Model <baypy.model.model.Model>` object. \n
+    Abstract base class for creating model objects.
 
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearModel <baypy.model.linear_model.LinearModel>`
+    """
 
     @property
     @abstractmethod
     def data(self) -> None: ...
 
 
     @data.setter
```

### Comparing `baypy-1.1.2/baypy/regression/functions.py` & `baypy-1.2.0/baypy/regression/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,137 +1,143 @@
 import numpy as np
 import pandas as pd
 from scipy.stats import invgamma, multivariate_normal
 from baypy.utils import flatten_matrix
 
 
 def sample_sigma2(y: pd.Series, X: np.ndarray, beta: np.ndarray, k_1: float, theta_0: float) -> float:
-    r"""Draws a sample for the variance from an inverse-gamma conditional posterior distribution at each regression
+    r"""It draws a sample for the variance from an inverse-gamma conditional posterior distribution at each regression
     iteration.
 
     Parameters
     ----------
-    y : pd.Series
+    ``y`` : :py:class:`pandas.Series`
         Vector of the response variable :math:`y`. It has a number of rows equal to the number of observed data.
-    X : numpy.ndarray
+    ``X`` : :py:class:`numpy.ndarray`
         Regressors matrix :math:`X`. It has a number of rows equal to the number of observed data and a number of
         columns equal to the number of regressors.
-    beta : numpy.ndarray
-        Regressors' parameters array of the model. It is sampled by the function ``sample_beta`` at each iteration.
-    k_1 : float
-        Sum of the variance prior ``shape`` and the number of observed data.
-    theta_0 : float
-        Variance prior ``scale``.
+    ``beta`` : :py:class:`numpy.ndarray`
+        Regressors' parameters array of the model. It is sampled by the function
+        :py:func:`sample_beta <baypy.regression.functions.sample_beta>` at each iteration.
+    ``k_1`` : :py:class:`float`
+        Sum of the variance prior ``'shape'`` and the number of observed data.
+    ``theta_0`` : :py:class:`float`
+        Variance prior ``'scale'``.
 
     Returns
     -------
-    numpy.ndarray
+    :py:class:`numpy.ndarray`
         Sampled variance :math:`\sigma^2`.
 
-    See Also
-    --------
-    :py:func:`baypy.regression.functions.sample_beta`
+    .. admonition:: Notes
+       :class: tip
 
-    Notes
-    -----
-    The variance is drawn from an inverse-gamma distribution. The conditional posterior distribution is:
+       The variance is drawn from an inverse-gamma distribution. The conditional posterior distribution is:
 
-    .. math::
-        H \left( \sigma^2 \left\vert B, y \right. \right) \sim
-        \text{Inv-}\Gamma \left( \frac{\kappa_1}{2}, \frac{\theta_1}{2} \right)
+       .. math::
+           H \left( \sigma^2 \left\vert B, y \right. \right) \sim
+           \text{Inv-}\Gamma \left( \frac{\kappa_1}{2}, \frac{\theta_1}{2} \right)
 
-    where :math:`B` is the :math:`\beta_j` vector, :math:`\kappa_1` is:
+       where :math:`B` is the :math:`\beta_j` vector, :math:`\kappa_1` is:
 
-    .. math::
-        \kappa_1 = \kappa_0 + n
+       .. math::
+           \kappa_1 = \kappa_0 + n
 
-    where :math:`n` is the number of observed data and :math:`\theta_1` is:
+       where :math:`n` is the number of observed data and :math:`\theta_1` is:
 
-    .. math::
-        \theta_1 = \theta_0 + \left( y - X B \right)^T \left( y - X B \right) .
+       .. math::
+           \theta_1 = \theta_0 + \left( y - X B \right)^T \left( y - X B \right) .
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:func:`sample_beta <baypy.regression.functions.sample_beta>`
     """
     y_X_beta = y - flatten_matrix(np.dot(X, beta))
     theta_1 = theta_0 + np.dot(y_X_beta.transpose(), y_X_beta)
 
     return invgamma.rvs(a = k_1/2, scale = theta_1/2)
 
 
 def sample_beta(Xt_X: np.ndarray, Xt_y: np.ndarray, sigma2: float, Sigma_0_inv: np.ndarray,
                 Sigma_0_inv_Beta_0: np.ndarray) -> np.ndarray:
-    r"""Draws a sample for each regressor parameter from a normal conditional posterior distribution at each regression
-    iteration.
+    r"""it draws a sample for each regressor parameter from a normal conditional posterior distribution at each
+    regression iteration.
 
     Parameters
     ----------
-    Xt_X : numpy.ndarray
-       Dot product of transposed regressors with themselves: :math:`X^T X`. It is a symmetric matrix with a
-       number of rows and columns equal to the number of regressors.
-    Xt_y : numpy.ndarray
-        Dot product of transposed regressors with the response variable: :math:`X^T y`. It is a one-dimensional
-        array with a number of rows equal to the number of regressors.
-    sigma2 : float
-        Variance of the model. It is sampled by the function ``sample_sigma2`` at each iteration.
-    Sigma_0_inv : numpy.ndarray
+    ``Xt_X`` : :py:class:`numpy.ndarray`
+       Dot product of transposed regressors with themselves: :math:`X^T X`. It is a symmetric matrix with a number of
+       rows and columns equal to the number of regressors.
+    ``Xt_y`` : :py:class:`numpy.ndarray`
+        Dot product of transposed regressors with the response variable: :math:`X^T y`. It is a one-dimensional array
+        with a number of rows equal to the number of regressors.
+    ``sigma2`` : :py:class:`float`
+        Variance of the model. It is sampled by the function
+        :py:func:`sample_sigma2 <baypy.regression.functions.sample_sigma2>` at each iteration.
+    ``Sigma_0_inv`` : :py:class:`numpy.ndarray`
         Regressors' parameters variance priors matrix. It is a symmetric matrix with a number of rows and columns equal
         to the number of regressors. It is the inverse of a matrix which has regressors' parameters' prior variances
         on the diagonal and ``0`` everywhere else.
-    Sigma_0_inv_Beta_0 : numpy.ndarray
+    ``Sigma_0_inv_Beta_0`` : :py:class:`numpy.ndarray`
         Dot product of ``Sigma_0_inv`` with a one-dimensional vector which has regressors' parameters' prior means on
         rows.
 
     Returns
     -------
-    numpy.ndarray
+    :py:class:`numpy.ndarray`
         Array of the sampled regressors' parameters :math:`B`. It has a number of element equal to the number of
         regressors.
 
-    See Also
-    --------
-    :py:func:`baypy.regression.functions.sample_sigma2`
-
-    Notes
-    -----
-    The regressors' parameters are drawn from a multivariate normal distribution. The conditional posterior
-    distribution is:
-
-    .. math::
-        H \left( B \left\vert \sigma^2, y \right. \right) \sim N(M, V)
-
-    where :math:`M` is a one-dimensional vector with a number of rows equal to the number of regressors:
-
-    .. math::
-        M = \left( \Sigma_0^{-1} + \frac{1}{\sigma^2} X^T X \right)^{-1} \left( \Sigma_0^{-1} B_0 + \frac{1}{\sigma^2}
-        X^T y \right)
-
-    and :math:`V` is a symmetric matrix with a number of rows and columns equal to the number of regressors:
-
-    .. math::
-        V = \left( \Sigma_0^{-1} + \frac{1}{\sigma^2} X^T X \right)^{-1} .
-
-    :math:`B_0` is:
-
-    .. math::
-        B_0 =
-        \begin{bmatrix}
-            \beta_0^0 \\
-            \beta_1^0 \\
-            \vdots    \\
-            \beta_m^0
-        \end{bmatrix}
-
-    and :math:`\Sigma_0^{-1}` is:
-
-    .. math::
-        \Sigma_0^{-1} =
-        \begin{bmatrix}
-            \Sigma_{\beta_0}^0 & 0 & \dots & 0 \\
-            0 & \Sigma_{\beta_1}^0 & \dots & 0 \\
-            \vdots & \vdots & \ddots & 0       \\
-            0 & 0 & 0 & \Sigma_{\beta_m}^0
-        \end{bmatrix}
+    .. admonition:: Notes
+       :class: tip
+
+       The regressors' parameters are drawn from a multivariate normal distribution. The conditional posterior
+       distribution is:
+
+       .. math::
+           H \left( B \left\vert \sigma^2, y \right. \right) \sim N(M, V)
+
+       where :math:`M` is a one-dimensional vector with a number of rows equal to the number of regressors:
+
+       .. math::
+           M = \left( \Sigma_0^{-1} + \frac{1}{\sigma^2} X^T X \right)^{-1} \left( \Sigma_0^{-1} B_0 + \frac{1}{\sigma^2}
+           X^T y \right)
+
+       and :math:`V` is a symmetric matrix with a number of rows and columns equal to the number of regressors:
+
+       .. math::
+           V = \left( \Sigma_0^{-1} + \frac{1}{\sigma^2} X^T X \right)^{-1} .
+
+       :math:`B_0` is:
+
+       .. math::
+           B_0 =
+           \begin{bmatrix}
+               \beta_0^0 \\
+               \beta_1^0 \\
+               \vdots    \\
+               \beta_m^0
+           \end{bmatrix}
+
+       and :math:`\Sigma_0^{-1}` is:
+
+       .. math::
+           \Sigma_0^{-1} =
+           \begin{bmatrix}
+               \Sigma_{\beta_0}^0 & 0 & \dots & 0 \\
+               0 & \Sigma_{\beta_1}^0 & \dots & 0 \\
+               \vdots & \vdots & \ddots & 0       \\
+               0 & 0 & 0 & \Sigma_{\beta_m}^0
+           \end{bmatrix}
+
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:func:`sample_sigma2 <baypy.regression.functions.sample_sigma2>`
     """
     V = np.linalg.inv(Sigma_0_inv + Xt_X/sigma2)
     M = np.dot(V, Sigma_0_inv_Beta_0 + Xt_y/sigma2)
     beta = multivariate_normal.rvs(mean = flatten_matrix(M), cov = V, size = 1)
 
     if Xt_X.shape != (1, 1):
         return beta
```

### Comparing `baypy-1.1.2/baypy/regression/linear_regression.py` & `baypy-1.2.0/baypy/regression/linear_regression.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,86 @@
 from baypy.regression.functions import sample_sigma2
 from baypy.regression.functions import sample_beta
 from baypy.model import Model
 from .regression import Regression
 import numpy as np
-import pandas as pd
 from scipy.stats import norm, invgamma
 
 
 class LinearRegression(Regression):
-    r"""baypy.regression.linear_regression.LinearRegression object.
+    r""":py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>` object.
 
     Methods
     -------
-    :meth:`baypy.regression.linear_regression.LinearRegression.sample()`
-        Samples a sequence of observations from the full posterior distribution of regressors' parameters
+    :meth:`sample`
+        It samples a sequence of observations from the full posterior distribution of regressors' parameters
         :math:`\beta_j` and ``variance`` :math:`\sigma^2`.
 
-    See Also
-    --------
-    :py:class:`baypy.model.linear_model.LinearModel`
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearModel <baypy.model.linear_model.LinearModel>`
     """
 
 
     @staticmethod
     def sample(model: Model, n_iterations: int, burn_in_iterations: int, n_chains: int, seed: int = None) -> None:
-        r"""Samples a sequence of observations from the full posterior distribution of regressors' parameters
+        r"""It samples a sequence of observations from the full posterior distribution of regressors' parameters
         :math:`\beta_j` and ``variance`` :math:`\sigma^2`.
         First ``burn_in_iterations`` are discarded since they may not accurately represent the desired distribution.
         For each variable, it generates ``n_chain`` Markov chains.
 
         Parameters
         ----------
-        model : baypy.model.model.Model
+        ``model`` : :py:class:`Model <baypy.model.model.Model>`
             The model with data, regressors, response variable and priors to be solved through Monte Carlo sampling.
-        n_iterations : int
+        ``n_iterations`` : :py:class:`int`
             Number of total sampling iteration for each chain. It must be a strictly positive integer.
-        burn_in_iterations : int
+        ``burn_in_iterations`` : :py:class:`int`
             Number of burn-in iteration for each chain. It must be a positive integer or ``0``.
-        n_chains : int
+        ``n_chains`` : :py:class:`int`
             Number of chains. It must be a strictly positive integer.
-        seed : int, optional
+        ``seed`` : :py:class:`int`, optional
             Random seed to use for reproducibility of the sampling.
 
-        Raises
-        ------
-        TypeError
-            - If ``model`` is not a ``baypy.model.model.Model``,
-            - if ``n_iterations`` is not a ``int``,
-            - if ``burn_in_iterations`` is not a ``int``,
-            - if ``n_chains`` is not a ``int``,
-            - if ``seed`` is not a ``int``.
-        ValueError
-            - If ``model.data`` is ``None``,
-            - if ``model.response_variable`` is ``None``,
-            - if ``model.response_variable`` is not a column of ``model.data``
-            - if ``model.priors`` is ``None``,
-            - if a ``model.priors`` key is not a column of ``model.data``,
-            - If ``n_iterations`` is equal to or less than ``0``,
-            - if ``burn_in_iterations`` is less than ``0``,
-            - if ``n_chains`` is equal to or less than ``0``,
-            - if ``seed`` is not between ``0`` and ``2**32 - 1``.
-
-        Notes
-        -----
-        The linear regression model of the response variable :math:`y` with respect to regressors :math:`X` is:
-
-        .. math::
-            y \sim N(\mu, \sigma^2)
-        .. math::
-            \mu = \beta_0 + B X = \beta_0 + \sum_{j = 1}^m \beta_j x_j
-
-        and the likelihood is:
-
-        .. math::
-            p \left( y \left\vert B,\sigma^2 \right. \right) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp{- \frac{\left(y -
-            \mu \right)^2}{2 \sigma^2}} .
+        .. admonition:: Raises
+           :class: warning
+
+           ``TypeError``
+               - If ``model`` is not a :py:class:`Model <baypy.model.model.Model>`,
+               - if ``n_iterations`` is not an :py:class:`int`,
+               - if ``burn_in_iterations`` is not an :py:class:`int`,
+               - if ``n_chains`` is not an :py:class:`int`,
+               - if ``seed`` is not an :py:class:`int`.
+           ``ValueError``
+               - If ``model.data`` is :py:obj:`None`,
+               - if ``model.response_variable`` is :py:obj:`None`,
+               - if ``model.response_variable`` is not a column of ``model.data``
+               - if ``model.priors`` is :py:obj:`None`,
+               - if a ``model.priors`` key is not a column of ``model.data``,
+               - If ``n_iterations`` is equal to or less than ``0``,
+               - if ``burn_in_iterations`` is less than ``0``,
+               - if ``n_chains`` is equal to or less than ``0``,
+               - if ``seed`` is not between ``0`` and ``2**32 - 1``.
+
+        .. admonition:: Notes
+           :class: tip
+
+           The linear regression model of the response variable :math:`y` with respect to regressors :math:`X` is:
+
+           .. math::
+               y \sim N(\mu, \sigma^2)
+           .. math::
+               \mu = \beta_0 + B X = \beta_0 + \sum_{j = 1}^m \beta_j x_j
+
+           and the likelihood is:
+
+           .. math::
+               p \left( y \left\vert B,\sigma^2 \right. \right) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp{- \frac{\left(y -
+               \mu \right)^2}{2 \sigma^2}} .
         """
         super(LinearRegression, LinearRegression).sample(model = model, n_iterations = n_iterations,
                                                          burn_in_iterations = burn_in_iterations, n_chains = n_chains,
                                                          seed = seed)
         data = model.data.copy()
 
         regressor_names = model.variable_names.copy()
@@ -112,18 +114,18 @@
             np.random.seed(seed)
 
         beta = [[norm.rvs(loc = model.priors[regressor]['mean'],
                           scale = np.sqrt(model.priors[regressor]['variance']))
                  for regressor in regressor_names] for _ in range(n_chains)]
         sigma2 = [invgamma.rvs(a = k_0, scale = theta_0) for _ in range(n_chains)]
 
-        for i in range(burn_in_iterations + n_iterations + 1):
+        for _ in range(burn_in_iterations + n_iterations + 1):
             for k in range(n_chains):
-                [posteriors[regressor][k].append(beta[k][j])
-                 for j, regressor in enumerate(regressor_names, 0)]
+                for j, regressor in enumerate(regressor_names, 0):
+                    posteriors[regressor][k].append(beta[k][j])
                 posteriors['variance'][k].append(sigma2[k])
 
             beta = [sample_beta(Xt_X = Xt_X,
                                 Xt_y = Xt_y,
                                 sigma2 = sigma2[k],
                                 Sigma_0_inv = Sigma_0_inv,
                                 Sigma_0_inv_Beta_0 = Sigma_0_inv_Beta_0) for k in range(n_chains)]
```

### Comparing `baypy-1.1.2/baypy/regression/regression.py` & `baypy-1.2.0/baypy/regression/regression.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from abc import ABC, abstractmethod
 from baypy.model import Model
-import pandas as pd
 
 
 class Regression(ABC):
+    """:py:class:`Regression <baypy.regression.regression.Regression>` object. \n
+    Abstract base class for creating regression objects.
 
+    .. admonition:: See Also
+       :class: seealso
+
+       :py:class:`LinearRegression <baypy.regression.linear_regression.LinearRegression>`
+    """
 
     @staticmethod
     @abstractmethod
     def sample(model: Model, n_iterations: int, burn_in_iterations: int, n_chains: int, seed: int = None) -> None:
         if not isinstance(model, Model):
             raise TypeError(f"Parameter 'model' must be an instance of '{Model.__module__}.{Model.__name__}'")
```

### Comparing `baypy-1.1.2/baypy/utils.py` & `baypy-1.2.0/baypy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,37 +11,39 @@
         Matrix with ``M`` rows and ``N`` columns.
 
     Returns
     -------
     numpy.ndarray
         Flatten array with ``M*N`` elements.
 
-    Raises
-    ------
-    TypeError
-        If ``matrix`` is not a ``numpy.ndarray``.
-    ValueError
-        If ``matrix`` is an empty ``numpy.ndarray``.
-
-    Examples
-    --------
-    >>> import numpy
-    >>> a = numpy.array([[1, 2], [3, 4], [5, 6]])
-    >>> a
-    >>> array([[1, 2],
-    ...        [3, 4],
-    ...        [5, 6]])
-    >>> flatten_matrix(a)
-    >>> array([1, 2, 3, 4, 5, 6])
+    .. admonition:: Raises
+       :class: warning
+
+       TypeError
+           If ``matrix`` is not a ``numpy.ndarray``.
+       ValueError
+           If ``matrix`` is an empty ``numpy.ndarray``.
+
+    .. admonition:: Examples
+       :class: important
+
+       >>> import numpy
+       >>> a = numpy.array([[1, 2], [3, 4], [5, 6]])
+       >>> a
+       >>> array([[1, 2],
+       ...        [3, 4],
+       ...        [5, 6]])
+       >>> flatten_matrix(a)
+       >>> array([1, 2, 3, 4, 5, 6])
     """
     if not isinstance(matrix, np.ndarray):
         raise TypeError("Parameter 'matrix' must be an instance of 'numpy.ndarray'")
 
     if matrix.size == 0:
-        raise ValueError(f"Parameter 'matrix' is empty")
+        raise ValueError("Parameter 'matrix' is empty")
 
     return np.asarray(matrix).reshape(-1)
 
 
 def matrices_to_frame(matrices_dict: dict) -> pd.DataFrame:
     """Organizes a dictionary of matrices in a ``pandas.DataFrame``. Each matrix becomes a frame column, with column
     name equal to the matrix' relative key in the dictionary. If the matrix has dimensions ``(M, N``), then the relative
@@ -55,39 +57,41 @@
 
     Returns
     -------
     pandas.DataFrame
         Reorganized matrices frame. Matrices are organized in a ``pandas.DataFrame``, one for each column. The
         length of the frame is ``M*N``.
 
-    Raises
-    ------
-    TypeError
-        - If ``matrices_dict`` is not a ``dict``,
-        - if a ``matrices_dict`` value is not a ``numpy.ndarray``.
-    ValueError
-        If a ``matrices_dict`` value is an empty ``numpy.ndarray``.
-
-    Examples
-    --------
-    >>> import numpy
-    >>> a = numpy.array([[1, 2], [3, 4], [5, 6]])
-    >>> b = numpy.array([[7, 8], [9, 10], [11, 12]])
-    >>> d = {'a': a, 'b': b}
-    >>> matrices_to_frame(d)
-    >>>    a   b
-    >>> 0  1   7
-    >>> 1  2   8
-    >>> 2  3   9
-    >>> 3  4  10
-    >>> 4  5  11
-    >>> 5  6  12
+    .. admonition:: Raises
+       :class: warning
+
+       TypeError
+           - If ``matrices_dict`` is not a ``dict``,
+           - if a ``matrices_dict`` value is not a ``numpy.ndarray``.
+       ValueError
+           If a ``matrices_dict`` value is an empty ``numpy.ndarray``.
+
+    .. admonition:: Examples
+       :class: important
+
+       >>> import numpy
+       >>> a = numpy.array([[1, 2], [3, 4], [5, 6]])
+       >>> b = numpy.array([[7, 8], [9, 10], [11, 12]])
+       >>> d = {'a': a, 'b': b}
+       >>> matrices_to_frame(d)
+       >>>    a   b
+       >>> 0  1   7
+       >>> 1  2   8
+       >>> 2  3   9
+       >>> 3  4  10
+       >>> 4  5  11
+       >>> 5  6  12
     """
     if not isinstance(matrices_dict, dict):
-        raise TypeError(f"Parameter 'matrices_dict' must be a dictionary")
+        raise TypeError("Parameter 'matrices_dict' must be a dictionary")
 
     for matrix_name, matrix in matrices_dict.items():
         if not isinstance(matrix, np.ndarray):
             raise TypeError(f"Matrix '{matrix_name}' must be an instance of 'numpy.ndarray'")
 
         if matrix.size == 0:
             raise ValueError(f"Matrix '{matrix_name}' is empty")
@@ -109,33 +113,35 @@
 
     Returns
     -------
     numpy.ndarray
         Array of computed dot product. Each element is the dot product of a ``data`` row with respect to each
         ``regressors``. It has the same length of ``data``.
 
-    Raises
-    ------
-    TypeError
-        - If ``data`` is not a ``pandas.DataFrame``,
-        - if ``regressors`` is not a ``dict``,
-        - if a ``regressors`` value is not a ``int`` or a ``float``.
-    KeyError
-        If a ``regressors`` key is not a column of ``data``.
-    ValueError
-        - If ``data`` is an empty ``pandas.DataFrame``,
-        - if ``regressors`` is an empty ``dict``.
-
-    Examples
-    --------
-    >>> import pandas as pd
-    >>> data = pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]})
-    >>> regressors = {'a': 2, 'b': -1}
-    >>> dot_product(data = data, regressors = regressors)
-    >>> array([-2, -1,  0])
+    .. admonition:: Raises
+       :class: warning
+
+       TypeError
+           - If ``data`` is not a ``pandas.DataFrame``,
+           - if ``regressors`` is not a ``dict``,
+           - if a ``regressors`` value is not a ``int`` or a ``float``.
+       KeyError
+           If a ``regressors`` key is not a column of ``data``.
+       ValueError
+           - If ``data`` is an empty ``pandas.DataFrame``,
+           - if ``regressors`` is an empty ``dict``.
+
+    .. admonition:: Examples
+       :class: important
+
+       >>> import pandas as pd
+       >>> data = pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]})
+       >>> regressors = {'a': 2, 'b': -1}
+       >>> dot_product(data = data, regressors = regressors)
+       >>> array([-2, -1,  0])
     """
     if not isinstance(data, pd.DataFrame):
         raise TypeError("Parameter 'data' must be an instance of 'pandas.DataFrame'")
 
     if data.empty:
         raise ValueError("Parameter 'data' cannot be an empty 'pandas.DataFrame'")
```

### Comparing `baypy-1.1.2/baypy.egg-info/SOURCES.txt` & `baypy-1.2.0/baypy.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README.md
+README.rst
 setup.py
 baypy/__init__.py
 baypy/utils.py
 baypy.egg-info/PKG-INFO
 baypy.egg-info/SOURCES.txt
 baypy.egg-info/dependency_links.txt
 baypy.egg-info/requires.txt
```

### Comparing `baypy-1.1.2/setup.py` & `baypy-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 import subprocess
 
 version = subprocess.run(['git', 'describe', '--tags'], stdout = subprocess.PIPE).stdout.decode('utf-8').strip()
 
-with open('README.md', 'r') as f:
+with open('README.rst', 'r') as f:
     long_description = f.read()
 
 def read_requirements(path: str):
     with open(path) as file:
         lines = file.readlines()
 
     return [line.replace('==', ' >= ').replace('\n', '') for line in lines]
@@ -21,15 +21,15 @@
 setup(name = 'baypy',
       version = version,
       description = "A python package for solving bayesian regression models "
                     "through a Monte Carlo Markov chain sampling",
       packages = find_packages(where = '.'),
       py_modules = ['__init__', 'utils'],
       long_description = long_description,
-      long_description_content_type = 'text/markdown',
+      long_description_content_type = 'text/x-rst',
       url = 'https://github.com/AndreaBlengino/baypy',
       project_urls = {'Source': 'https://github.com/AndreaBlengino/baypy',
                       'Tracker': 'https://github.com/AndreaBlengino/baypy/issues',
                       'Documentation': 'https://baypy.readthedocs.io/en/latest/index.html'},
       author = 'Andrea Blengino',
       author_email = 'ing.andrea.blengino@gmail.com',
       license = 'GNU GPL3',
```

