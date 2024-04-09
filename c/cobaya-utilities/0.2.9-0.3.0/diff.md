# Comparing `tmp/cobaya_utilities-0.2.9.tar.gz` & `tmp/cobaya_utilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobaya_utilities-0.2.9.tar", last modified: Fri Mar 29 06:57:28 2024, max compression
+gzip compressed data, was "cobaya_utilities-0.3.0.tar", last modified: Tue Apr  9 04:34:46 2024, max compression
```

## Comparing `cobaya_utilities-0.2.9.tar` & `cobaya_utilities-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:57:28.716969 cobaya_utilities-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-29 06:57:28.716969 cobaya_utilities-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:57:28.716969 cobaya_utilities-0.2.9/cobaya_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/cobaya_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 06:57:28.716969 cobaya_utilities-0.2.9/cobaya_utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/cobaya_utilities/fisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/cobaya_utilities/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    22784 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/cobaya_utilities/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/cobaya_utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 06:57:28.716969 cobaya_utilities-0.2.9/cobaya_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-29 06:57:28.000000 cobaya_utilities-0.2.9/cobaya_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-29 06:57:28.000000 cobaya_utilities-0.2.9/cobaya_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 06:57:28.000000 cobaya_utilities-0.2.9/cobaya_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 06:57:28.000000 cobaya_utilities-0.2.9/cobaya_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 06:57:28.000000 cobaya_utilities-0.2.9/cobaya_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 06:57:28.716969 cobaya_utilities-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83635 2024-03-29 06:57:24.000000 cobaya_utilities-0.2.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/cobaya_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/cobaya_utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22174 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/cobaya_utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 04:34:46.000000 cobaya_utilities-0.3.0/cobaya_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:34:46.158883 cobaya_utilities-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83635 2024-04-09 04:34:43.000000 cobaya_utilities-0.3.0/versioneer.py
```

### Comparing `cobaya_utilities-0.2.9/PKG-INFO` & `cobaya_utilities-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobaya_utilities
-Version: 0.2.9
+Version: 0.3.0
 Summary: A set of functions to deal with MCMC output from cobaya
 Home-page: https://github.com/xgarrido/cobaya_utilities.git
 Author: Xavier Garrido
 Author-email: xavier.garrido@lal.in2p3.fr
 Keywords: cobaya,MCMC,plot
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

### Comparing `cobaya_utilities-0.2.9/README.rst` & `cobaya_utilities-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.2.9/cobaya_utilities/fisher.py` & `cobaya_utilities-0.3.0/cobaya_utilities/fisher.py`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.2.9/cobaya_utilities/plots.py` & `cobaya_utilities-0.3.0/cobaya_utilities/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import os
+import re
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from getdist import plots
 from getdist.plots import get_subplot_plotter
 from matplotlib.lines import Line2D
 from scipy import stats
 
-from .tools import _get_path
+from .tools import _get_chain_filenames, _get_path
 
 
 def set_style(
     use_seaborn=False,
     seaborn_style="ticks",
     seaborn_context="paper",
     palette="tab10",
@@ -147,14 +148,15 @@
     plot_settings = GetDistPlotSettings()
     plot_settings.solid_colors = colors
     plot_settings.line_styles = colors
     plot_settings.num_plot_contours = num_plot_contours
     plot_settings.linewidth = linewidth
     plot_settings.legend_fontsize = 15
     plot_settings.legend_colored_text = True
+    plot_settings.figure_legend_loc = "best"
     plot_settings.scaling = False
     return plot_settings
 
 
 def triangle_plot(*args, **kwargs):
     """Overloaded triangle_plot function with additional features"""
     g = get_subplot_plotter(settings=get_default_settings())
@@ -188,15 +190,15 @@
 
     if priors := kwargs.get("priors"):
         show_priors(
             g,
             priors,
             color=kwargs.get("prior_color", "gray"),
             with_legend=kwargs.get("prior_legend", True),
-            legend_kwargs=dict(loc="best"),
+            legend_kwargs=dict(loc=kwargs.get("prior_legend_loc", "upper right")),
         )
 
     if kwargs.get("despine", True):
         despine(g, all_axes=True)
 
     if legend_kwargs:
         g.add_legend(legend_labels, **legend_kwargs)
@@ -225,14 +227,15 @@
     burnin=0.4,
     no_cache=False,
     as_dict=True,
     selected=None,
     excluded=None,
     select_first=None,
     no_progress_bar=True,
+    Rminus1_max_value=None,
 ):
     """Print MCMC sample size given a set of directories
 
     Parameters
     ----------
     mcmc_samples: dict
       a dict holding a name as key for the sample and a corresponding directory as value
@@ -249,14 +252,16 @@
       list of selected samples
     excluded: list
       list of excluded samples
     select_fist: str
       set the name of the first sample to return
     no_progress_bar: bool
       either enable or disable progress bar from tqdm
+    Rminus1_max_value: float
+      the maximal accepted R-1 value
     """
     from getdist import loadMCSamples
     from tqdm.auto import tqdm
 
     selected = selected or list(mcmc_samples.keys())
     excluded = excluded or []
 
@@ -270,32 +275,51 @@
 
     if select_first:
         selected.remove(select_first)
         selected = [select_first] + selected
 
     default_prefix = prefix
     samples, labels, colors = [], [], []
+    regex = re.compile(r".*mcmc\.([0-9]+).progress")
+
     for name in (pbar := tqdm(selected, disable=no_progress_bar)):
         pbar.set_description(f"Loading '{name}'")
         value = mcmc_samples[name]
         if isinstance(value, str):
             value = dict(path=value)
         path = _get_path(name, value)
         prefix = value.get("prefix", default_prefix)
         labels += [value.get("label", name)]
         colors += [value.get("color", f"C{selected.index(name)}")]
-
-        samples += [
-            loadMCSamples(
-                os.path.join(path, prefix),
-                settings={"ignore_rows": burnin},
-                no_cache=no_cache,
-                chain_exclude=value.get("exclude"),
-            )
-        ]
+        if Rminus1_max_value:
+            exclude = []
+            files = _get_chain_filenames(path, prefix, suffix=".progress")
+            for fn in files:
+                idx = 1 if not (m := regex.match(fn)) else int(m.group(1))
+                with open(fn) as f:
+                    cols = [a.strip() for a in f.readline().lstrip("#").split()]
+                df = pd.read_csv(
+                    fn, names=cols, comment="#", sep=" ", skipinitialspace=True, index_col=False
+                )
+                if df.N.empty:
+                    exclude += [idx]
+                elif df.Rminus1.iloc[-1] > Rminus1_max_value:
+                    exclude += [idx]
+                value.update(exclude=exclude)
+        try:
+            samples += [
+                loadMCSamples(
+                    os.path.join(path, prefix),
+                    settings={"ignore_rows": burnin},
+                    no_cache=no_cache,
+                    chain_exclude=value.get("exclude"),
+                )
+            ]
+        except OSError:
+            print(f"WANRING: No chains of {name} found or fulfill the requirement!")
     if as_dict:
         return samples, dict(legend_labels=labels, colors=colors, diag1d_kwargs={"colors": colors})
     return samples, labels, colors
 
 
 def show_results(g, results, with_legend=True, legend_kwargs=None):
     """Show results values on a given set of axes
@@ -328,45 +352,48 @@
         loc="upper left",
     )
     kwargs |= legend_kwargs or {}
     if with_legend:
         add_legend(**kwargs)
 
 
-def show_priors(g, priors, color="gray", ls="--", with_legend=True, legend_kwargs=None):
+def show_priors(
+    g, priors, color="gray", ls="--", with_label=False, with_legend=True, legend_kwargs=None
+):
     """Show prior values on a given set of axes
     Parameters
     ----------
     g: getdist.plots
       the getdist plotter instance
     priors: dict
       dictionary holding loc/scale value for normal distribution
     color: str
       the color name
     ls: str
       the line style
+    with_label: bool
+      append parameter name to the legend (default: False)
     with_legend: bool
       add legend
     legend_kwargs: dict
       set legend kwargs
     """
     for par, val in priors.items():
         if not (ax := g.get_axes_for_params(par)):
             continue
+        label = rf"${ax.getdist_params[0].label}$ prior" if with_label else "prior"
         if isinstance(val, float):
             ax.axvline(val, color=color, ls=ls)
         else:
             x = np.linspace(*ax.get_xlim(), 100)
             y = stats.norm.pdf(x, *val)
-            ax.plot(
-                x, y / y.max(), color=color, ls=ls, label=rf"${ax.getdist_params[0].label}$ prior"
-            )
+            ax.plot(x, y / y.max(), color=color, ls=ls, label=label)
         if with_legend:
             legend_kwargs = legend_kwargs or dict(loc="upper left", bbox_to_anchor=(1, 1))
-            ax.legend(**legend_kwargs)
+            ax.legend(labelcolor="linecolor", **legend_kwargs)
 
 
 def show_tau_prior(g, loc=0.054, scale=0.0073, color="gray", ls="--"):
     """Dedicated function to plot tau prior
 
     Parameters
     ----------
@@ -398,15 +425,17 @@
     kwargs = {"left": True} or kwargs
     if all_axes:
         sns.despine(fig=g.fig, **kwargs)
     else:
         sns.despine(ax=g.subplots[0, 0], **kwargs)
 
 
-def plot_mean_values(samples, params, colors=None, palette=None, labels=None, figsize=None):
+def plot_mean_values(
+    samples, params, colors=None, palette=None, labels=None, figsize=None, **kwargs
+):
     """Plot mean and sigma values from posterior distributions
 
     Parameters
     ----------
     samples: list
       a list holding getdist MCSamples
     params: dict or list
@@ -470,14 +499,15 @@
         else:
             axes[j].spines["left"].set_visible(False)
         if not np.all(chi2s[j] == None):
             pvalue = stats.chi2.sf(np.sum(chi2s[j]), nsamples)
             axes[j].set_title(f"$P(\chi^2)$ = {pvalue:.3f}", fontsize=10)
 
     # Add labels
+    labels = labels or kwargs.get("legend_labels")
     if labels is not None:
         ax = axes[0]
         for i, label in enumerate(labels):
             ax.text(
                 ax.get_xlim()[0],
                 i,
                 label,
@@ -496,15 +526,17 @@
             cm.ScalarMappable(norm=colors.Normalize(vmin=vmin, vmax=vmax), cmap=cmap),
             ax=axes,
             label=r"$\chi^2$" if use_stats_color == "chi2" else r"$p$-value",
             shrink=0.8,
         )
 
 
-def plot_mean_distributions(samples, params, colors="0.7", return_results=False, nx=None):
+def plot_mean_distributions(
+    samples, params, priors=None, colors="0.7", return_results=False, nx=None
+):
     """Plot mean KDE distributions
 
     Parameters
     ----------
     samples: list
       a list holding getdist MCSamples
     params: dict or list
@@ -519,50 +551,63 @@
     from getdist.plots import get_subplot_plotter
 
     nsamples = len(samples)
     g = get_subplot_plotter(subplot_size=3, subplot_size_ratio=1.4)
     g.settings.line_styles = (
         nsamples * ["-" + colors] if isinstance(colors, str) else ["-" + color for color in colors]
     )
-    nx = nx or nsamples
+    nx = nx or len(params)
     g.plots_1d(samples, params, nx=nx, legend_labels=[], lws=2)
 
+    priors = priors or {}
     results = {}
     axes = g.subplots.flatten()
     for i, name in enumerate(params):
         ax = axes[i]
         if not ax:
             continue
         means, sigmas = np.empty(nsamples), np.empty(nsamples)
         for j, sample in enumerate(samples):
             marge = sample.getMargeStats()
             par = marge.parWithName(name)
             means[j], sigmas[j] = par.mean, par.err
         mu = np.average(means, weights=1 / sigmas**2)
         sigma = np.mean(sigmas)
-        x = np.linspace(*ax.get_xlim(), 1000)
+        sigma = np.std(means)
+        x = np.linspace(*ax.get_xlim(), 100)
         y = stats.norm.pdf(x, mu, sigma)
         ax.plot(x, y / y.max(), color="black", lw=2.5)
-        if params.get(name) is not None:
-            param = params.get(name)
+        if (param := params.get(name)) is not None:
             if isinstance(param, (tuple, list)):
                 y = stats.norm.pdf(x, *param)
                 ax.plot(x, y / y.max(), color="black", ls="--", lw=2.5)
             else:
                 ax.axvline(param, color="red", lw=3)
-            legend = ax.legend([], loc="upper right")
-            legend.set_title(
-                r"$\frac{{{:.1f}\,\sigma}}{{\sqrt{{N_{{\rm sim}}}}}}$".format(
+            labels, handles = [], []
+            if priors.get(name):
+                labels = [rf"prior"]
+                handles = [Line2D([0], [0], color="blue", ls="--")]
+
+            legend = ax.legend(
+                handles,
+                labels,
+                labelcolor="linecolor",
+                bbox_to_anchor=(1, 1),
+                loc="upper center",
+                title=r"$\frac{{{:.1f}\,\sigma}}{{\sqrt{{N_{{\rm sim}}}}}}$".format(
                     (mu - param) / sigma * np.sqrt(nsamples)
                 ),
-                prop={"size": 16},
+                title_fontsize=16,
             )
         results[ax.get_xlabel()] = {"value rec.": mu, "$\sigma$ rec.": sigma}
         ax.spines.left.set_visible(False)
 
+    if priors:
+        show_priors(g, priors, color="blue", with_legend=False)
+
     if return_results:
         return pd.DataFrame.from_dict(results, orient="index")
 
 
 def add_legend(obj, labels=None, colors=None, ls=None, **kwargs):
     """Add legend
```

### Comparing `cobaya_utilities-0.2.9/cobaya_utilities/tools.py` & `cobaya_utilities-0.3.0/cobaya_utilities/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                         current_steps = int(current_steps)
                         total_steps = (
                             current_steps
                             if current_steps > total_steps
                             else total_steps + current_steps
                         )
                 accepted_steps = int(accepted_steps)
-                rate = accepted_steps / total_steps
+                rate = accepted_steps / total_steps if total_steps != 0 else None
                 for field, content in zip(
                     ["R-1", "accept.", "total", "rate"], [None, accepted_steps, total_steps, rate]
                 ):
                     data[name].update({(mcmc_name, field): content})
             if with_gelman_rubin:
                 files = _get_chain_filenames(path, suffix=".progress")
                 for fn in sorted(files):
@@ -231,29 +231,30 @@
 
     s.format(
         {sub: "{:.1%}".format for sub in [(name, "rate") for name in all_mcmc_names]}, na_rep=""
     ).apply(_style_table, axis=None)
     return s
 
 
-def print_results(samples, params, labels, limit=1):
+def print_results(samples, params, labels=None, limit=1, **kwargs):
     """Print results given a set of MCMC samples and a list of parameters
 
     Parameters
     ----------
     samples: list
       a list of MCSamples.
     params: list
       a list of parameters.
     labels: list
       a list of labels to be used as row index.
     limit: int
       the confidence limit of the results (default: 1 i.e. 68%).
     """
     params = params if isinstance(params, list) else list(params.keys())
+    labels = labels or kwargs.get("legend_labels")
     labels = labels if isinstance(labels, list) else list(labels.keys())
     d, cols = {}, {}
 
     merge_renames = {}
     for sample in samples:
         merge_renames = mergeRenames(
             sample.getParamNames().getRenames(keep_empty=True), merge_renames
@@ -321,16 +322,16 @@
           a unique list of parameter names
         ncol: int
           the number of columns within the plot
         highlight_burnin: float
           the fraction of samples to highlight (below the burnin value, the color is faded)
         ignore_rows: float
           the fraction of samples to ignore
-        show_mean_std: bool
-          show the mean/std values over the different samples
+        show_mean_std: bool or str
+          show the mean/std values over the different samples. It can either True/False or "rolling".
         show_only_mcmc: int or list
           only show chains given their number
         no_cache: bool
           remove the getdist cache
         markers: dict
     :      dictionnary holding the "expected" value for a parameter
         markers_args: dict
@@ -414,35 +415,55 @@
             #         color_palettes[color_name] = sns.blend_palette(
             #             ["white", color_name], n_colors=len(files) + 1
             #         )
             #     color = color_palettes[color_name][imcmc]
             if samples.shape[0] < min_chain_size:
                 min_chain_size = samples.shape[0]
             for i, p in enumerate(selected_params):
-                axes[i].set_ylabel(r"${}$".format(lookup[p].get("label")))
+                axes[i].set_ylabel(rf"${lookup[p].get('label')}$")
                 y = samples[:, lookup[p].get("pos")]
                 x = np.arange(len(y))
                 idx_burnin = -int(highlight_burnin * len(y))
                 axes[i].plot(x[idx_burnin:], y[idx_burnin:], alpha=0.75, color=color)
                 if highlight_burnin > 0.0:
                     axes[i].plot(x[: idx_burnin + 1], y[: idx_burnin + 1], alpha=0.25, color=color)
                 if p in markers:
                     axes[i].axhline(markers[p], **markers_args)
                 if prior := priors.get(p):
                     mu, sigma = prior
                     axes[i].axhspan(mu - sigma, mu + sigma, **priors_args)
                 chains.setdefault(p, []).append(y)
 
         if show_mean_std:
+
+            def _moving_average(x, w):
+                return np.convolve(x, np.ones(w), "valid") / w
+
             for i, p in enumerate(selected_params):
-                data = np.array([chain[:min_chain_size] for chain in chains[p]])
-                mu, std = np.mean(data), np.std(data)
-                axes[i].axhline(mu, color="0.6", lw=1)
-                for sign in [-1, +1]:
-                    axes[i].axhline(mu + std * sign, color="0.6", ls="--", lw=1)
+                if show_mean_std == "rolling":
+                    max_size = np.max([chain.size for chain in chains[p]])
+                    data = np.full((len(chains[p]), max_size), np.nan)
+                    for j, chain in enumerate(chains[p]):
+                        data[j, : len(chain)] = chain
+                    x = np.arange(max_size)
+                    mu, std = np.nanmean(data, axis=0), np.nanstd(data, axis=0)
+                    std[std == 0.0] = np.nan
+                    window = int(0.2 * max_size)
+                    x = _moving_average(x, window)
+                    mu = _moving_average(mu, window)
+                    std = _moving_average(std, window)
+                    axes[i].plot(x, mu, color="0.6", lw=1)
+                    for sign in [-1, +1]:
+                        axes[i].plot(x, mu + std * sign, color="0.6", ls="--", lw=1)
+                else:
+                    data = np.array([chain[:min_chain_size] for chain in chains[p]])
+                    mu, std = np.mean(data), np.std(data)
+                    axes[i].axhline(mu, color="0.6", lw=1)
+                    for sign in [-1, +1]:
+                        axes[i].axhline(mu + std * sign, color="0.6", ls="--", lw=1)
 
         # Remove axes with no data inside
         _ = [fig.delaxes(ax) for ax in axes if not len(ax.get_lines())]
         leg = fig.legend(
             [Line2D([0], [0], color=f"C{int(f.split('.')[-2])-1}") for f in files],
             [f"mcmc #{f.split('.')[-2]}" for f in files],
             bbox_to_anchor=(0.5, 1.025),
@@ -524,33 +545,39 @@
             fig.delaxes(axes[i, 0])
             fig.delaxes(axes[i, 1])
     if not fig.axes:
         plt.close(fig)
     return fig
 
 
-def get_sampled_parameters(mcmc_samples, prefix="mcmc", return_params=False):
+def get_sampled_parameters(
+    mcmc_samples, prefix="mcmc", return_params=False, with_priors=False, column_width="150px"
+):
     """Print MCMC sampled parameters
 
     Parameters
     ----------
     mcmc_samples: dict
       a dict holding a name as key for the sample and a corresponding directory as value
       or a dict configuration
     prefix: str
       prefix for chain names (default is "mcmc.")
     return_params: bool
       return dict of params for each MCMC chain (default false)
+    column_width: str
+      the column width of the output dataframe (default: 150px)
     """
 
     create_symlink(mcmc_samples, prefix)
-    r1 = re.compile(r".*mcmc\] \*.*: (.*)")
+    r1 = re.compile(r".*mcmc\] \*.*[0-9+] : (.*)")
     r2 = re.compile(r".*model\].*Input: (.*)")
 
-    latex_params = {}
+    rprior = re.compile(r".*lambda (.*):.*stats.norm.logpdf.*loc=(.*),.*scale=(.*).*\)")
+
+    params_info = {}
     sampled_params = {}
     for name, value in mcmc_samples.items():
         path = _get_path(name, value)
         name = value.get("label", name) if isinstance(value, dict) else name
         files = _get_chain_filenames(path, prefix=prefix, suffix=".log")
         if not files:
             print(f"Missing log files for chains '{name}' within path '{path}'!")
@@ -567,18 +594,49 @@
         with open(files[0]) as f:
             for line in f:
                 found = r1.findall(line) or r2.findall(line)
                 if len(found) == 0:
                     continue
                 params = eval(found[0])
                 sampled_params.setdefault(name, []).extend(params)
-                latex_params.setdefault(name, []).extend(
+                params_info.setdefault((name, "parameter"), []).extend(
                     [latex_table.get(par, par) for par in params]
                 )
                 if "Sampling!" in line:
                     break
+        if not with_priors:
+            continue
+
+        # Get priors
+        external_priors = {}
+        for k, v in updated_yaml.get("prior", {}).items():
+            found = rprior.findall(v)
+            if len(found) == 0:
+                continue
+            param, loc, scale = found[0]
+            external_priors[param] = f"$\mathcal{{G}}({float(loc)}, {float(scale)})$"
+        for param in sampled_params.get(name, []):
+            if param not in (params := updated_yaml.get("params")):
+                raise ValueError("Sampled paremeter can not be found within input parameters !")
+
+            if param in external_priors:
+                params_info.setdefault((name, "prior"), []).append(external_priors[param])
+                continue
 
-    df = pd.DataFrame.from_dict(latex_params, orient="index").T.fillna("")
-    df = df.style.set_properties(width="150px")
+            input_priors = params.get(param).get("prior", {})
+            if dist := input_priors.get("dist"):
+                if dist == "norm":
+                    loc, scale = input_priors.get("loc"), input_priors.get("scale")
+                    params_info.setdefault((name, "prior"), []).append(
+                        f"$\mathcal{{G}}({loc}, {scale})$"
+                    )
+            elif input_priors.get("min") or input_priors.get("max"):
+                min, max = input_priors.get("min"), input_priors.get("max")
+                params_info.setdefault((name, "prior"), []).append(f"$\mathcal{{U}}({min}, {max})$")
+
+    # print(params_info)
+    df = pd.DataFrame.from_dict(params_info, orient="index").T.fillna("").drop_duplicates()
+    df.columns = params_info.keys() if with_priors else sampled_params.keys()
+    df = df.style.set_properties(width=column_width)
     if return_params:
         return df, sampled_params
     return df
```

### Comparing `cobaya_utilities-0.2.9/cobaya_utilities.egg-info/PKG-INFO` & `cobaya_utilities-0.3.0/cobaya_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobaya_utilities
-Version: 0.2.9
+Version: 0.3.0
 Summary: A set of functions to deal with MCMC output from cobaya
 Home-page: https://github.com/xgarrido/cobaya_utilities.git
 Author: Xavier Garrido
 Author-email: xavier.garrido@lal.in2p3.fr
 Keywords: cobaya,MCMC,plot
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

### Comparing `cobaya_utilities-0.2.9/pyproject.toml` & `cobaya_utilities-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.2.9/setup.py` & `cobaya_utilities-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.2.9/versioneer.py` & `cobaya_utilities-0.3.0/versioneer.py`

 * *Files identical despite different names*

