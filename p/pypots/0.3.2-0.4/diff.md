# Comparing `tmp/pypots-0.3.2.tar.gz` & `tmp/pypots-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.3.2.tar", last modified: Tue Mar 19 09:27:08 2024, max compression
+gzip compressed data, was "pypots-0.4.tar", last modified: Tue Apr  9 13:48:49 2024, max compression
```

## Comparing `pypots-0.3.2.tar` & `pypots-0.4.tar`

### file list

```diff
@@ -1,219 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.888664 pypots-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-19 09:25:15.000000 pypots-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-19 09:25:15.000000 pypots-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26673 2024-03-19 09:27:08.888664 pypots-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24858 2024-03-19 09:25:15.000000 pypots-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.868664 pypots-0.3.2/pypots/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24074 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.868664 pypots-0.3.2/pypots/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.868664 pypots-0.3.2/pypots/classification/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.868664 pypots-0.3.2/pypots/classification/brits/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/brits/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/brits/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.868664 pypots-0.3.2/pypots/classification/grud/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/grud/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/grud/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/classification/grud/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/grud/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/grud/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/classification/raindrop/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/raindrop/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/raindrop/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/classification/raindrop/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/raindrop/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/raindrop/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/classification/raindrop/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/pypots_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/clustering/crli/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/crli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/crli/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/clustering/crli/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/crli/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/crli/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/crli/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/clustering/vader/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/vader/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/vader/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.872664 pypots-0.3.2/pypots/clustering/vader/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/vader/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/vader/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/clustering/vader/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/data/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/generating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/load_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/load_specific_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/data/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/saving/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/saving/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17516 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/forecasting/bttf/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/bttf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/bttf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/forecasting/bttf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/bttf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/bttf/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/forecasting/bttf/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/imputation/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/imputation/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9960 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/imputation/brits/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/brits/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/brits/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/brits/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.876664 pypots-0.3.2/pypots/imputation/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/csdi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/csdi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/csdi/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/csdi/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/csdi/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/csdi/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/gpvae/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/gpvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/gpvae/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/gpvae/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/gpvae/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/gpvae/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/gpvae/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/gpvae/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/locf/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/locf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/locf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/locf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/locf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/locf/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/mean/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mean/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/median/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/median/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/median/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/mrnn/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mrnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mrnn/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mrnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/mrnn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mrnn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mrnn/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/mrnn/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/saits/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/saits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/saits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/saits/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/saits/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/saits/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.880664 pypots-0.3.2/pypots/imputation/timesnet/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/imputation/timesnet/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/timesnet/modules/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/imputation/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/transformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/transformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/imputation/transformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/transformer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/transformer/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/imputation/usgan/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/usgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/usgan/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/usgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/imputation/usgan/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/usgan/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/usgan/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/imputation/usgan/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/functional/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/nn/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/transformer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/transformer/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/nn/modules/transformer/pos_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.884664 pypots-0.3.2/pypots/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.888664 pypots-0.3.2/pypots/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/constant_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/exponential_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/lambda_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/linear_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/multiplicative_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/multistep_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/lr_scheduler/step_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.888664 pypots-0.3.2/pypots/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.888664 pypots-0.3.2/pypots/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/metrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/metrics/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.888664 pypots-0.3.2/pypots/utils/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/visual/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-19 09:25:15.000000 pypots-0.3.2/pypots/utils/visual/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:27:08.868664 pypots-0.3.2/pypots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26673 2024-03-19 09:27:08.000000 pypots-0.3.2/pypots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-03-19 09:27:08.000000 pypots-0.3.2/pypots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:27:08.000000 pypots-0.3.2/pypots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-19 09:27:08.000000 pypots-0.3.2/pypots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-19 09:27:08.000000 pypots-0.3.2/pypots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 09:27:08.000000 pypots-0.3.2/pypots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-19 09:27:08.888664 pypots-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-19 09:25:15.000000 pypots-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 13:46:55.000000 pypots-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 13:46:55.000000 pypots-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27890 2024-04-09 13:48:49.892830 pypots-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26077 2024-04-09 13:46:55.000000 pypots-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-09 13:46:55.000000 pypots-0.4/pypots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22426 2024-04-09 13:46:55.000000 pypots-0.4/pypots/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/brits/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/modules/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/grud/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/modules/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/raindrop/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/pypots_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/crli/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/vader/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/generating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/load_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/load_specific_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/data/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/saving/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/saving/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/forecasting/bttf/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/forecasting/bttf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/autoformer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/modules/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/brits/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/crossformer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17279 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/csdi/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/dlinear/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/modules/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/etsformer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/fedformer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/gpvae/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/informer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/locf/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/locf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/modules/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mean/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/median/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/median/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/median/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/mrnn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/patchtst/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/saits/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/modules/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/timesnet/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/imputation/transformer/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/modules/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/imputation/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17811 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/imputation/usgan/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/modules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/modules/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/functional/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/rnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/constant_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/exponential_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/lambda_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/linear_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/multiplicative_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/multistep_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/step_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/utils/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/visual/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/visual/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27890 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 13:48:49.892830 pypots-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-09 13:46:55.000000 pypots-0.4/setup.py
```

### Comparing `pypots-0.3.2/LICENSE` & `pypots-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/PKG-INFO` & `pypots-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.3.2
+Version: 0.4
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
 Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/
 Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
@@ -166,28 +166,28 @@
 PyPOTS is available on both [PyPI](https://pypi.python.org/pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots).
 You can install PyPOTS as shown below:
 
 ``` bash
 # via pip
 pip install pypots            # the first time installation
 pip install pypots --upgrade  # update pypots to the latest version
+# install from the latest source code with the latest features but may be not officially released yet
+pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
 
 # via conda
 conda install -c conda-forge pypots  # the first time installation
 conda update  -c conda-forge pypots  # update pypots to the latest version
-````
-
-Alternatively, you can install from the latest source code with the latest features but may be not officially released yet:
-> pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
+```
 
 
 ## ❖ Usage
-Besides [BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial notebook
-on Google Colab <a href="https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ"><img src="https://img.shields.io/badge/GoogleColab-PyPOTS_Tutorials-F9AB00?logo=googlecolab&logoColor=white" alt="Colab tutorials" align="center"/></a>.
-If you have further questions, please refer to PyPOTS documentation [docs.pypots.com](https://docs.pypots.com).
+Besides [BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial notebook on Google Colab
+<a href="https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ">
+<img src="https://img.shields.io/badge/GoogleColab-PyPOTS_Tutorials-F9AB00?logo=googlecolab&logoColor=white" alt="Colab tutorials" align="center"/>
+</a>. If you have further questions, please refer to PyPOTS documentation [docs.pypots.com](https://docs.pypots.com).
 You can also [raise an issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-community).
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details open>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
 
@@ -208,15 +208,15 @@
 X = X.reshape(num_samples, 48, -1)
 X_ori = X  # keep X_ori for validation
 X = mcar(X, 0.1)  # randomly hold out 10% observed values as ground truth
 dataset = {"X": X}  # X for model input
 print(X.shape)  # (11988, 48, 37), 11988 samples and each sample has 48 time steps, 37 features
 
 # Model training. This is PyPOTS showtime.
-saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
 # Here I use the whole dataset as the training set because ground truth is not visible to the model, you can also split it into train/val/test sets
 saits.fit(dataset)
 imputation = saits.impute(dataset)  # impute the originally-missing values and artificially-missing values
 indicating_mask = np.isnan(X) ^ np.isnan(X_ori)  # indicating mask for imputation error calculation
 mae = calc_mae(imputation, np.nan_to_num(X_ori), indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
 ```
 </details>
@@ -226,38 +226,50 @@
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
 The currently available algorithms of four tasks are cataloged in the following table with four partitions.
 The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
 
-|   ***`Imputation`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|:----------------------:|:-----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**  |                                                                       **Full name of the algorithm/model**                                                                        | **Year** |
-|       Neural Net       |    SAITS    |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
-|       Neural Net       | Transformer | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
-|       Neural Net       |  TimesNet   |                                                       Temporal 2D-Variation Modeling for General Time Series Analysis [^14]                                                       |   2023   |
-|       Neural Net       |    CSDI     |                                              Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]                                              |   2021   |
-|       Neural Net       |   US-GAN    |                                                          Unsupervised GAN for Multivariate Time Series Imputation [^10]                                                           |   2021   |
-|       Neural Net       |   GP-VAE    |                                                                  Gaussian Process Variational Autoencoder [^11]                                                                   |   2020   |
-|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    M-RNN    |                                                                  Multi-directional Recurrent Neural Network [^9]                                                                  |   2019   |
-|         Naive          |    LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
-| ***`Classification`*** |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    GRU-D    |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
-|       Neural Net       |  Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
-|   ***`Clustering`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
-|       Neural Net       |    VaDER    |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
-|  ***`Forecasting`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|     Probabilistic      |    BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
+🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
+and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+
+|   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
+|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
+|        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
+|       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
+|       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
+|       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
+|       Neural Net       |  TimesNet   |              Temporal 2D-Variation Modeling for General Time Series Analysis [^14]              |   2023   |
+|       Neural Net       |  PatchTST   |         A Time Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18]          |   2023   |
+|       Neural Net       |   DLinear   |                  Are Transformers Effective for Time Series Forecasting? [^17]                  |   2023   |
+|       Neural Net       |  ETSformer  |              Exponential Smoothing Transformers for Time-series Forecasting [^19]               |   2023   |
+|       Neural Net       |  FEDformer  |        Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting [^20]         |   2022   |
+|       Neural Net       |  Informer   |          Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [^21]           |   2021   |
+|       Neural Net       | Autoformer  |     Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting [^15]     |   2021   |
+|       Neural Net       |    CSDI     |     Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]     |   2021   |
+|       Neural Net       |   US-GAN    |                 Unsupervised GAN for Multivariate Time Series Imputation [^10]                  |   2021   |
+|       Neural Net       |   GP-VAE    |                         Gaussian Process Variational Autoencoder [^11]                          |   2020   |
+|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
+|       Neural Net       |    M-RNN    |                         Multi-directional Recurrent Neural Network [^9]                         |   2019   |
+|         Naive          |  LOCF/NOCB  |              Last Observation Carried Forward / Next Observation Carried Backward               |    -     |
+|         Naive          |   Median    |                                     Median Value Imputation                                     |    -     |
+|         Naive          |    Mean     |                                      Mean Value Imputation                                      |    -     |
+| ***`Classification`*** |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
+|       Neural Net       |    GRU-D    |         Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]         |   2018   |
+|       Neural Net       |  Raindrop   |           Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]            |   2022   |
+|   ***`Clustering`***   |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|       Neural Net       |    CRLI     |             Clustering Representation Learning on Incomplete time-series data [^6]              |   2021   |
+|       Neural Net       |    VaDER    |                         Variational Deep Embedding with Recurrence [^7]                         |   2019   |
+|  ***`Forecasting`***   |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|     Probabilistic      |    BTTF     |                           Bayesian Temporal Tensor Factorization [^8]                           |   2021   |
 
 
 ## ❖ Citing PyPOTS
 > [!TIP]
 > **[Updates in Feb 2024]** 😎 Our survey paper [Deep Learning for Multivariate Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on arXiv.
 The code is open source in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation).
 We comprehensively review the literature of the state-of-the-art deep-learning imputation methods for time series,
@@ -283,15 +295,15 @@
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
 doi={10.48550/arXiv.2305.18811},
 }
 ```
-
+or
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
 
 ## ❖ Contribution
 You're very welcome to contribute to this exciting project!
@@ -352,14 +364,22 @@
 [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal Factorization for Multidimensional Time Series Prediction](https://arxiv.org/abs/1910.06366). *IEEE transactions on pattern analysis and machine intelligence*.
 [^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019). [Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE Transactions on Biomedical Engineering*.
 [^10]: Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021). [Generative Semi-supervised Learning for Multivariate Time Series Imputation](https://ojs.aaai.org/index.php/AAAI/article/view/17086). *AAAI 2021*.
 [^11]: Fortuin, V., Baranchuk, D., Raetsch, G. & Mandt, S. (2020). [GP-VAE: Deep Probabilistic Time Series Imputation](https://proceedings.mlr.press/v108/fortuin20a.html). *AISTATS 2020*.
 [^12]: Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021). [CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation](https://proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-Abstract.html). *NeurIPS 2021*.
 [^13]: Rubin, D. B. (1976). [Inference and missing data](https://academic.oup.com/biomet/article-abstract/63/3/581/270932). *Biometrika*.
 [^14]: Wu, H., Hu, T., Liu, Y., Zhou, H., Wang, J., & Long, M. (2023). [TimesNet: Temporal 2d-variation modeling for general time series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023*
+[^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting](https://proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-Abstract.html). *NeurIPS 2021*.
+[^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
+[^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
+[^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
+[^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
+[^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
+[^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
+
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.3.2 Summary: A Python Toolbox for
+Metadata-Version: 2.1 Name: pypots Version: 0.4 Summary: A Python Toolbox for
 Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
 Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
 https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
 WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
 PyPOTS/archive/main.zip Keywords: data science,data mining,neural
 networks,machine learning,deep learning,artificial intelligence,time-series
@@ -79,39 +79,39 @@
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
 install PyPOTS as shown below: ``` bash # via pip pip install pypots # the
 first time installation pip install pypots --upgrade # update pypots to the
-latest version # via conda conda install -c conda-forge pypots # the first time
-installation conda update -c conda-forge pypots # update pypots to the latest
-version ```` Alternatively, you can install from the latest source code with
-the latest features but may be not officially released yet: > pip install
-https://github.com/WenjieDu/PyPOTS/archive/main.zip ## â Usage Besides
-[BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple
-and quick-start tutorial notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you
-have further questions, please refer to PyPOTS documentation [docs.pypots.com]
-(https://docs.pypots.com). You can also [raise an issue](https://github.com/
-WenjieDu/PyPOTS/issues) or [ask in our community](#-community). We present you
-a usage example of imputing missing values in time series with PyPOTS below,
-you can click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn
-PPhhyyssiiooNNeett22001122 ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from
-sklearn.preprocessing import StandardScaler from pygrinder import mcar from
-pypots.data import load_specific_dataset from pypots.imputation import SAITS
-from pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but
-PyPOTS can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
+latest version # install from the latest source code with the latest features
+but may be not officially released yet pip install https://github.com/WenjieDu/
+PyPOTS/archive/main.zip # via conda conda install -c conda-forge pypots # the
+first time installation conda update -c conda-forge pypots # update pypots to
+the latest version ``` ## â Usage Besides [BrewPOTS](https://github.com/
+WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial
+notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further questions,
+please refer to PyPOTS documentation [docs.pypots.com](https://
+docs.pypots.com). You can also [raise an issue](https://github.com/WenjieDu/
+PyPOTS/issues) or [ask in our community](#-community). We present you a usage
+example of imputing missing values in time series with PyPOTS below, you can
+click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn PPhhyyssiiooNNeett22001122
+ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from sklearn.preprocessing import
+StandardScaler from pygrinder import mcar from pypots.data import
+load_specific_dataset from pypots.imputation import SAITS from
+pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but PyPOTS
+can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
 automatically download and extract it. X = data['X'] num_samples = len(X
 ['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
 StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
 X_ori = X # keep X_ori for validation X = mcar(X, 0.1) # randomly hold out 10%
 observed values as ground truth dataset = {"X": X} # X for model input print
 (X.shape) # (11988, 48, 37), 11988 samples and each sample has 48 time steps,
 37 features # Model training. This is PyPOTS showtime. saits = SAITS
-(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_heads=4,
+(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4,
 d_k=64, d_v=64, dropout=0.1, epochs=10) # Here I use the whole dataset as the
 training set because ground truth is not visible to the model, you can also
 split it into train/val/test sets saits.fit(dataset) imputation = saits.impute
 (dataset) # impute the originally-missing values and artificially-missing
 values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
 imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
 indicating_mask) # calculate mean absolute error on the ground truth
@@ -119,68 +119,81 @@
 imputation, classification, clustering, and forecasting tasks on multivariate
 time series with missing values. The currently available algorithms of four
 tasks are cataloged in the following table with four partitions. The paper
 references are all listed at the bottom of this readme file. Please refer to
 them if you want more details. ð Since **v0.2**, all neural-network models
 in PyPOTS has got hyperparameter-optimization support. This functionality is
 implemented with the [Microsoft NNI](https://github.com/microsoft/nni)
-framework. | ***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:---------------------
--:|:-----------:|:-------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------:|:--------:| | **Type** | **Abbr.** |
-**Full name of the algorithm/model** | **Year** | | Neural Net | SAITS | Self-
-Attention-based Imputation for Time Series [^1] | 2023 | | Neural Net |
-Transformer | Attention is All you Need [^2];
-Self-Attention-based Imputation for Time Series [^1];
-Note: proposed in [^2], and re-implemented as an imputation model in [^1]. |
-2017 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for General
-Time Series Analysis [^14] | 2023 | | Neural Net | CSDI | Conditional Score-
+framework. ð¥ Note that Transformer, Crossformer, PatchTST, DLinear,
+ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation
+methods in their original papers, and they cannot accept POTS as input. **To
+make them applicable on POTS data, we apply the embedding strategy the same as
+we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).** |
+***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:----------------------:|:----------
+-:|:---------------------------------------------------------------------------
+--------------------:|:--------:| | **Type** | **Abbr.** | **Full name of the
+algorithm/model** | **Year** | | Neural Net | SAITS | Self-Attention-based
+Imputation for Time Series [^1] | 2023 | | Neural Net | Transformer | Attention
+is All you Need [^2] | 2017 | | Neural Net | Crossformer | Transformer
+Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting
+[^16] | 2023 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for
+General Time Series Analysis [^14] | 2023 | | Neural Net | PatchTST | A Time
+Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18] | 2023
+| | Neural Net | DLinear | Are Transformers Effective for Time Series
+Forecasting? [^17] | 2023 | | Neural Net | ETSformer | Exponential Smoothing
+Transformers for Time-series Forecasting [^19] | 2023 | | Neural Net |
+FEDformer | Frequency Enhanced Decomposed Transformer for Long-term Series
+Forecasting [^20] | 2022 | | Neural Net | Informer | Beyond Efficient
+Transformer for Long Sequence Time-Series Forecasting [^21] | 2021 | | Neural
+Net | Autoformer | Decomposition Transformers with Auto-Correlation for Long-
+Term Series Forecasting [^15] | 2021 | | Neural Net | CSDI | Conditional Score-
 based Diffusion Models for Probabilistic Time Series Imputation [^12] | 2021 |
 | Neural Net | US-GAN | Unsupervised GAN for Multivariate Time Series
 Imputation [^10] | 2021 | | Neural Net | GP-VAE | Gaussian Process Variational
 Autoencoder [^11] | 2020 | | Neural Net | BRITS | Bidirectional Recurrent
 Imputation for Time Series [^3] | 2018 | | Neural Net | M-RNN | Multi-
-directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF | Last
-Observation Carried Forward | - | | ***`Classification`*** | ð¥ | ð¥ | ð¥
-| | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
-**Year** | | Neural Net | BRITS | Bidirectional Recurrent Imputation for Time
-Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent Neural Networks for
-Multivariate Time Series with Missing Values [^4] | 2018 | | Neural Net |
-Raindrop | Graph-Guided Network for Irregularly Sampled Multivariate Time
-Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ | ð¥ | | **Type** |
-**Abbr.** | **Full name of the algorithm/model/paper** | **Year** | | Neural
-Net | CRLI | Clustering Representation Learning on Incomplete time-series data
-[^6] | 2021 | | Neural Net | VaDER | Variational Deep Embedding with Recurrence
-[^7] | 2019 | | ***`Forecasting`*** | ð¥ | ð¥ | ð¥ | | **Type** |
-**Abbr.** | **Full name of the algorithm/model/paper** | **Year** | |
-Probabilistic | BTTF | Bayesian Temporal Tensor Factorization [^8] | 2021 | ##
-â Citing PyPOTS > [!TIP] > **[Updates in Feb 2024]** ð Our survey paper
-[Deep Learning for Multivariate Time Series Imputation: A Survey](https://
-arxiv.org/abs/2402.04059) has been released on arXiv. The code is open source
-in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/
-Awesome_Imputation). We comprehensively review the literature of the state-of-
-the-art deep-learning imputation methods for time series, provide a taxonomy
-for them, and discuss the challenges and future directions in this field. > >
-**[Updates in Jun 2023]** ð A short version of the PyPOTS paper is accepted
-by the 9th SIGKDD international workshop on Mining and Learning from Time
-Series ([MiLeTS'23](https://kdd-milets.github.io/milets2023/))).
-**Additionally**, PyPOTS has been included as a [PyTorch Ecosystem](https://
-pytorch.org/ecosystem/) project. The paper introducing PyPOTS is available on
-arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing to
-publish it in prestigious academic venues, e.g. JMLR (track for [Machine
-Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use PyPOTS
-in your work, please cite it as below and ðstar this repository to make
-others notice this library. ð¤ There are scientific research projects using
-PyPOTS and referencing in their papers. Here is [an incomplete list of them]
-(https://scholar.google.com/
+directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF/NOCB | Last
+Observation Carried Forward / Next Observation Carried Backward | - | | Naive |
+Median | Median Value Imputation | - | | Naive | Mean | Mean Value Imputation |
+- | | ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** |
+**Full name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
+Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
+GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
+Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
+Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
+| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Neural Net | CRLI | Clustering Representation
+Learning on Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER |
+Variational Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`***
+| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
+Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
+2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
+Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
+arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
+github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
+literature of the state-of-the-art deep-learning imputation methods for time
+series, provide a taxonomy for them, and discuss the challenges and future
+directions in this field. > > **[Updates in Jun 2023]** ð A short version of
+the PyPOTS paper is accepted by the 9th SIGKDD international workshop on Mining
+and Learning from Time Series ([MiLeTS'23](https://kdd-milets.github.io/
+milets2023/))). **Additionally**, PyPOTS has been included as a [PyTorch
+Ecosystem](https://pytorch.org/ecosystem/) project. The paper introducing
+PyPOTS is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
+and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
+(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
+)). If you use PyPOTS in your work, please cite it as below and ðstar this
+repository to make others notice this library. ð¤ There are scientific
+research projects using PyPOTS and referencing in their papers. Here is [an
+incomplete list of them](https://scholar.google.com/
 scholar?as_ylo=2022&q=%E2%80%9CPyPOTS%E2%80%9D&hl=en>). ``` bibtex @article
 {du2023pypots, title={{PyPOTS: a Python toolbox for data mining on Partially-
 Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
 archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
-2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du. (2023). >
+2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
 PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series. >
 arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ## â Contribution
 You're very welcome to contribute to this exciting project! By committing your
 code, you'll 1. make your well-established model out-of-the-box for PyPOTS
 users to run, and help your work obtain more exposure and impact. Take a look
 at our [inclusion criteria](https://docs.pypots.com/en/latest/
 faq.html#inclusion-criteria). You can utilize the `template` folder in each
@@ -243,9 +256,29 @@
 Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021). [CSDI: Conditional Score-
 based Diffusion Models for Probabilistic Time Series Imputation](https://
 proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-
 Abstract.html). *NeurIPS 2021*. [^13]: Rubin, D. B. (1976). [Inference and
 missing data](https://academic.oup.com/biomet/article-abstract/63/3/581/
 270932). *Biometrika*. [^14]: Wu, H., Hu, T., Liu, Y., Zhou, H., Wang, J., &
 Long, M. (2023). [TimesNet: Temporal 2d-variation modeling for general time
-series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023* ð 
-Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023*
+[^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition
+transformers with auto-correlation for long-term series forecasting](https://
+proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-
+Abstract.html). *NeurIPS 2021*. [^16]: Zhang, Y., & Yan, J. (2023).
+[Crossformer: Transformer utilizing cross-dimension dependency for multivariate
+time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR
+2023*. [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers
+effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/
+article/view/26317). *AAAI 2023* [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., &
+Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting
+with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
+[^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer:
+Exponential Smoothing Transformers for Time-series Forecasting](https://
+openreview.net/forum?id=5m_3whfo483). *ICLR 2023* [^20]: Zhou, T., Ma, Z., Wen,
+Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced
+decomposed transformer for long-term series forecasting](https://
+proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*. [^21]: Zhou, H., Zhang,
+S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer:
+Beyond efficient transformer for long sequence time-series forecasting](https:/
+/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. ð  Visits
+_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.3.2/README.md` & `pypots-0.4/pypots.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: pypots
+Version: 0.4
+Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
+Home-page: https://pypots.com/
+Author: Wenjie Du
+Author-email: wenjay.du@gmail.com
+License: BSD-3-Clause
+Project-URL: Documentation, https://docs.pypots.com/
+Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
+Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
+Project-URL: Download, https://github.com/WenjieDu/PyPOTS/archive/main.zip
+Keywords: data science,data mining,neural networks,machine learning,deep learning,artificial intelligence,time-series analysis,time series,imputation,interpolation,classification,clustering,forecasting,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: basic
+Provides-Extra: optional
+Provides-Extra: full
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: dev
+License-File: LICENSE
+
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img src="https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg" width="200" align="right">
 </a>
 
 <h3 align="center">Welcome to PyPOTS</h3>
 
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
@@ -128,28 +166,28 @@
 PyPOTS is available on both [PyPI](https://pypi.python.org/pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots).
 You can install PyPOTS as shown below:
 
 ``` bash
 # via pip
 pip install pypots            # the first time installation
 pip install pypots --upgrade  # update pypots to the latest version
+# install from the latest source code with the latest features but may be not officially released yet
+pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
 
 # via conda
 conda install -c conda-forge pypots  # the first time installation
 conda update  -c conda-forge pypots  # update pypots to the latest version
-````
-
-Alternatively, you can install from the latest source code with the latest features but may be not officially released yet:
-> pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
+```
 
 
 ## ❖ Usage
-Besides [BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial notebook
-on Google Colab <a href="https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ"><img src="https://img.shields.io/badge/GoogleColab-PyPOTS_Tutorials-F9AB00?logo=googlecolab&logoColor=white" alt="Colab tutorials" align="center"/></a>.
-If you have further questions, please refer to PyPOTS documentation [docs.pypots.com](https://docs.pypots.com).
+Besides [BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial notebook on Google Colab
+<a href="https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ">
+<img src="https://img.shields.io/badge/GoogleColab-PyPOTS_Tutorials-F9AB00?logo=googlecolab&logoColor=white" alt="Colab tutorials" align="center"/>
+</a>. If you have further questions, please refer to PyPOTS documentation [docs.pypots.com](https://docs.pypots.com).
 You can also [raise an issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-community).
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details open>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
 
@@ -170,15 +208,15 @@
 X = X.reshape(num_samples, 48, -1)
 X_ori = X  # keep X_ori for validation
 X = mcar(X, 0.1)  # randomly hold out 10% observed values as ground truth
 dataset = {"X": X}  # X for model input
 print(X.shape)  # (11988, 48, 37), 11988 samples and each sample has 48 time steps, 37 features
 
 # Model training. This is PyPOTS showtime.
-saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
 # Here I use the whole dataset as the training set because ground truth is not visible to the model, you can also split it into train/val/test sets
 saits.fit(dataset)
 imputation = saits.impute(dataset)  # impute the originally-missing values and artificially-missing values
 indicating_mask = np.isnan(X) ^ np.isnan(X_ori)  # indicating mask for imputation error calculation
 mae = calc_mae(imputation, np.nan_to_num(X_ori), indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
 ```
 </details>
@@ -188,38 +226,50 @@
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
 The currently available algorithms of four tasks are cataloged in the following table with four partitions.
 The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
 
-|   ***`Imputation`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|:----------------------:|:-----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**  |                                                                       **Full name of the algorithm/model**                                                                        | **Year** |
-|       Neural Net       |    SAITS    |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
-|       Neural Net       | Transformer | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
-|       Neural Net       |  TimesNet   |                                                       Temporal 2D-Variation Modeling for General Time Series Analysis [^14]                                                       |   2023   |
-|       Neural Net       |    CSDI     |                                              Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]                                              |   2021   |
-|       Neural Net       |   US-GAN    |                                                          Unsupervised GAN for Multivariate Time Series Imputation [^10]                                                           |   2021   |
-|       Neural Net       |   GP-VAE    |                                                                  Gaussian Process Variational Autoencoder [^11]                                                                   |   2020   |
-|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    M-RNN    |                                                                  Multi-directional Recurrent Neural Network [^9]                                                                  |   2019   |
-|         Naive          |    LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
-| ***`Classification`*** |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    GRU-D    |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
-|       Neural Net       |  Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
-|   ***`Clustering`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
-|       Neural Net       |    VaDER    |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
-|  ***`Forecasting`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|     Probabilistic      |    BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
+🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
+and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+
+|   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
+|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
+|        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
+|       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
+|       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
+|       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
+|       Neural Net       |  TimesNet   |              Temporal 2D-Variation Modeling for General Time Series Analysis [^14]              |   2023   |
+|       Neural Net       |  PatchTST   |         A Time Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18]          |   2023   |
+|       Neural Net       |   DLinear   |                  Are Transformers Effective for Time Series Forecasting? [^17]                  |   2023   |
+|       Neural Net       |  ETSformer  |              Exponential Smoothing Transformers for Time-series Forecasting [^19]               |   2023   |
+|       Neural Net       |  FEDformer  |        Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting [^20]         |   2022   |
+|       Neural Net       |  Informer   |          Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [^21]           |   2021   |
+|       Neural Net       | Autoformer  |     Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting [^15]     |   2021   |
+|       Neural Net       |    CSDI     |     Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]     |   2021   |
+|       Neural Net       |   US-GAN    |                 Unsupervised GAN for Multivariate Time Series Imputation [^10]                  |   2021   |
+|       Neural Net       |   GP-VAE    |                         Gaussian Process Variational Autoencoder [^11]                          |   2020   |
+|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
+|       Neural Net       |    M-RNN    |                         Multi-directional Recurrent Neural Network [^9]                         |   2019   |
+|         Naive          |  LOCF/NOCB  |              Last Observation Carried Forward / Next Observation Carried Backward               |    -     |
+|         Naive          |   Median    |                                     Median Value Imputation                                     |    -     |
+|         Naive          |    Mean     |                                      Mean Value Imputation                                      |    -     |
+| ***`Classification`*** |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
+|       Neural Net       |    GRU-D    |         Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]         |   2018   |
+|       Neural Net       |  Raindrop   |           Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]            |   2022   |
+|   ***`Clustering`***   |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|       Neural Net       |    CRLI     |             Clustering Representation Learning on Incomplete time-series data [^6]              |   2021   |
+|       Neural Net       |    VaDER    |                         Variational Deep Embedding with Recurrence [^7]                         |   2019   |
+|  ***`Forecasting`***   |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|     Probabilistic      |    BTTF     |                           Bayesian Temporal Tensor Factorization [^8]                           |   2021   |
 
 
 ## ❖ Citing PyPOTS
 > [!TIP]
 > **[Updates in Feb 2024]** 😎 Our survey paper [Deep Learning for Multivariate Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on arXiv.
 The code is open source in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation).
 We comprehensively review the literature of the state-of-the-art deep-learning imputation methods for time series,
@@ -245,15 +295,15 @@
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
 doi={10.48550/arXiv.2305.18811},
 }
 ```
-
+or
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
 
 ## ❖ Contribution
 You're very welcome to contribute to this exciting project!
@@ -314,14 +364,22 @@
 [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal Factorization for Multidimensional Time Series Prediction](https://arxiv.org/abs/1910.06366). *IEEE transactions on pattern analysis and machine intelligence*.
 [^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019). [Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE Transactions on Biomedical Engineering*.
 [^10]: Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021). [Generative Semi-supervised Learning for Multivariate Time Series Imputation](https://ojs.aaai.org/index.php/AAAI/article/view/17086). *AAAI 2021*.
 [^11]: Fortuin, V., Baranchuk, D., Raetsch, G. & Mandt, S. (2020). [GP-VAE: Deep Probabilistic Time Series Imputation](https://proceedings.mlr.press/v108/fortuin20a.html). *AISTATS 2020*.
 [^12]: Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021). [CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation](https://proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-Abstract.html). *NeurIPS 2021*.
 [^13]: Rubin, D. B. (1976). [Inference and missing data](https://academic.oup.com/biomet/article-abstract/63/3/581/270932). *Biometrika*.
 [^14]: Wu, H., Hu, T., Liu, Y., Zhou, H., Wang, J., & Long, M. (2023). [TimesNet: Temporal 2d-variation modeling for general time series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023*
+[^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting](https://proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-Abstract.html). *NeurIPS 2021*.
+[^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
+[^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
+[^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
+[^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
+[^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
+[^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
+
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,33 @@
-_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
+Metadata-Version: 2.1 Name: pypots Version: 0.4 Summary: A Python Toolbox for
+Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
+Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
+Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
+https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
+WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
+PyPOTS/archive/main.zip Keywords: data science,data mining,neural
+networks,machine learning,deep learning,artificial intelligence,time-series
+analysis,time
+series,imputation,interpolation,classification,clustering,forecasting,partially
+observed,irregular sampled,partially-observed time series,incomplete time
+series,missing data,missing values Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: Intended Audience :: Healthcare Industry Classifier:
+License :: OSI Approved :: BSD License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Requires-Python: >=3.7.0 Description-Content-Type: text/
+markdown Provides-Extra: basic Provides-Extra: optional Provides-Extra: full
+Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
+LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
                  _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
@@ -54,39 +79,39 @@
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
 install PyPOTS as shown below: ``` bash # via pip pip install pypots # the
 first time installation pip install pypots --upgrade # update pypots to the
-latest version # via conda conda install -c conda-forge pypots # the first time
-installation conda update -c conda-forge pypots # update pypots to the latest
-version ```` Alternatively, you can install from the latest source code with
-the latest features but may be not officially released yet: > pip install
-https://github.com/WenjieDu/PyPOTS/archive/main.zip ## â Usage Besides
-[BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple
-and quick-start tutorial notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you
-have further questions, please refer to PyPOTS documentation [docs.pypots.com]
-(https://docs.pypots.com). You can also [raise an issue](https://github.com/
-WenjieDu/PyPOTS/issues) or [ask in our community](#-community). We present you
-a usage example of imputing missing values in time series with PyPOTS below,
-you can click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn
-PPhhyyssiiooNNeett22001122 ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from
-sklearn.preprocessing import StandardScaler from pygrinder import mcar from
-pypots.data import load_specific_dataset from pypots.imputation import SAITS
-from pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but
-PyPOTS can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
+latest version # install from the latest source code with the latest features
+but may be not officially released yet pip install https://github.com/WenjieDu/
+PyPOTS/archive/main.zip # via conda conda install -c conda-forge pypots # the
+first time installation conda update -c conda-forge pypots # update pypots to
+the latest version ``` ## â Usage Besides [BrewPOTS](https://github.com/
+WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial
+notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further questions,
+please refer to PyPOTS documentation [docs.pypots.com](https://
+docs.pypots.com). You can also [raise an issue](https://github.com/WenjieDu/
+PyPOTS/issues) or [ask in our community](#-community). We present you a usage
+example of imputing missing values in time series with PyPOTS below, you can
+click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn PPhhyyssiiooNNeett22001122
+ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from sklearn.preprocessing import
+StandardScaler from pygrinder import mcar from pypots.data import
+load_specific_dataset from pypots.imputation import SAITS from
+pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but PyPOTS
+can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
 automatically download and extract it. X = data['X'] num_samples = len(X
 ['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
 StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
 X_ori = X # keep X_ori for validation X = mcar(X, 0.1) # randomly hold out 10%
 observed values as ground truth dataset = {"X": X} # X for model input print
 (X.shape) # (11988, 48, 37), 11988 samples and each sample has 48 time steps,
 37 features # Model training. This is PyPOTS showtime. saits = SAITS
-(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_heads=4,
+(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4,
 d_k=64, d_v=64, dropout=0.1, epochs=10) # Here I use the whole dataset as the
 training set because ground truth is not visible to the model, you can also
 split it into train/val/test sets saits.fit(dataset) imputation = saits.impute
 (dataset) # impute the originally-missing values and artificially-missing
 values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
 imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
 indicating_mask) # calculate mean absolute error on the ground truth
@@ -94,68 +119,81 @@
 imputation, classification, clustering, and forecasting tasks on multivariate
 time series with missing values. The currently available algorithms of four
 tasks are cataloged in the following table with four partitions. The paper
 references are all listed at the bottom of this readme file. Please refer to
 them if you want more details. ð Since **v0.2**, all neural-network models
 in PyPOTS has got hyperparameter-optimization support. This functionality is
 implemented with the [Microsoft NNI](https://github.com/microsoft/nni)
-framework. | ***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:---------------------
--:|:-----------:|:-------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------:|:--------:| | **Type** | **Abbr.** |
-**Full name of the algorithm/model** | **Year** | | Neural Net | SAITS | Self-
-Attention-based Imputation for Time Series [^1] | 2023 | | Neural Net |
-Transformer | Attention is All you Need [^2];
-Self-Attention-based Imputation for Time Series [^1];
-Note: proposed in [^2], and re-implemented as an imputation model in [^1]. |
-2017 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for General
-Time Series Analysis [^14] | 2023 | | Neural Net | CSDI | Conditional Score-
+framework. ð¥ Note that Transformer, Crossformer, PatchTST, DLinear,
+ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation
+methods in their original papers, and they cannot accept POTS as input. **To
+make them applicable on POTS data, we apply the embedding strategy the same as
+we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).** |
+***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:----------------------:|:----------
+-:|:---------------------------------------------------------------------------
+--------------------:|:--------:| | **Type** | **Abbr.** | **Full name of the
+algorithm/model** | **Year** | | Neural Net | SAITS | Self-Attention-based
+Imputation for Time Series [^1] | 2023 | | Neural Net | Transformer | Attention
+is All you Need [^2] | 2017 | | Neural Net | Crossformer | Transformer
+Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting
+[^16] | 2023 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for
+General Time Series Analysis [^14] | 2023 | | Neural Net | PatchTST | A Time
+Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18] | 2023
+| | Neural Net | DLinear | Are Transformers Effective for Time Series
+Forecasting? [^17] | 2023 | | Neural Net | ETSformer | Exponential Smoothing
+Transformers for Time-series Forecasting [^19] | 2023 | | Neural Net |
+FEDformer | Frequency Enhanced Decomposed Transformer for Long-term Series
+Forecasting [^20] | 2022 | | Neural Net | Informer | Beyond Efficient
+Transformer for Long Sequence Time-Series Forecasting [^21] | 2021 | | Neural
+Net | Autoformer | Decomposition Transformers with Auto-Correlation for Long-
+Term Series Forecasting [^15] | 2021 | | Neural Net | CSDI | Conditional Score-
 based Diffusion Models for Probabilistic Time Series Imputation [^12] | 2021 |
 | Neural Net | US-GAN | Unsupervised GAN for Multivariate Time Series
 Imputation [^10] | 2021 | | Neural Net | GP-VAE | Gaussian Process Variational
 Autoencoder [^11] | 2020 | | Neural Net | BRITS | Bidirectional Recurrent
 Imputation for Time Series [^3] | 2018 | | Neural Net | M-RNN | Multi-
-directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF | Last
-Observation Carried Forward | - | | ***`Classification`*** | ð¥ | ð¥ | ð¥
-| | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
-**Year** | | Neural Net | BRITS | Bidirectional Recurrent Imputation for Time
-Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent Neural Networks for
-Multivariate Time Series with Missing Values [^4] | 2018 | | Neural Net |
-Raindrop | Graph-Guided Network for Irregularly Sampled Multivariate Time
-Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ | ð¥ | | **Type** |
-**Abbr.** | **Full name of the algorithm/model/paper** | **Year** | | Neural
-Net | CRLI | Clustering Representation Learning on Incomplete time-series data
-[^6] | 2021 | | Neural Net | VaDER | Variational Deep Embedding with Recurrence
-[^7] | 2019 | | ***`Forecasting`*** | ð¥ | ð¥ | ð¥ | | **Type** |
-**Abbr.** | **Full name of the algorithm/model/paper** | **Year** | |
-Probabilistic | BTTF | Bayesian Temporal Tensor Factorization [^8] | 2021 | ##
-â Citing PyPOTS > [!TIP] > **[Updates in Feb 2024]** ð Our survey paper
-[Deep Learning for Multivariate Time Series Imputation: A Survey](https://
-arxiv.org/abs/2402.04059) has been released on arXiv. The code is open source
-in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/
-Awesome_Imputation). We comprehensively review the literature of the state-of-
-the-art deep-learning imputation methods for time series, provide a taxonomy
-for them, and discuss the challenges and future directions in this field. > >
-**[Updates in Jun 2023]** ð A short version of the PyPOTS paper is accepted
-by the 9th SIGKDD international workshop on Mining and Learning from Time
-Series ([MiLeTS'23](https://kdd-milets.github.io/milets2023/))).
-**Additionally**, PyPOTS has been included as a [PyTorch Ecosystem](https://
-pytorch.org/ecosystem/) project. The paper introducing PyPOTS is available on
-arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing to
-publish it in prestigious academic venues, e.g. JMLR (track for [Machine
-Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use PyPOTS
-in your work, please cite it as below and ðstar this repository to make
-others notice this library. ð¤ There are scientific research projects using
-PyPOTS and referencing in their papers. Here is [an incomplete list of them]
-(https://scholar.google.com/
+directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF/NOCB | Last
+Observation Carried Forward / Next Observation Carried Backward | - | | Naive |
+Median | Median Value Imputation | - | | Naive | Mean | Mean Value Imputation |
+- | | ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** |
+**Full name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
+Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
+GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
+Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
+Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
+| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Neural Net | CRLI | Clustering Representation
+Learning on Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER |
+Variational Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`***
+| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
+Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
+2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
+Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
+arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
+github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
+literature of the state-of-the-art deep-learning imputation methods for time
+series, provide a taxonomy for them, and discuss the challenges and future
+directions in this field. > > **[Updates in Jun 2023]** ð A short version of
+the PyPOTS paper is accepted by the 9th SIGKDD international workshop on Mining
+and Learning from Time Series ([MiLeTS'23](https://kdd-milets.github.io/
+milets2023/))). **Additionally**, PyPOTS has been included as a [PyTorch
+Ecosystem](https://pytorch.org/ecosystem/) project. The paper introducing
+PyPOTS is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
+and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
+(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
+)). If you use PyPOTS in your work, please cite it as below and ðstar this
+repository to make others notice this library. ð¤ There are scientific
+research projects using PyPOTS and referencing in their papers. Here is [an
+incomplete list of them](https://scholar.google.com/
 scholar?as_ylo=2022&q=%E2%80%9CPyPOTS%E2%80%9D&hl=en>). ``` bibtex @article
 {du2023pypots, title={{PyPOTS: a Python toolbox for data mining on Partially-
 Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
 archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
-2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du. (2023). >
+2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
 PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series. >
 arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ## â Contribution
 You're very welcome to contribute to this exciting project! By committing your
 code, you'll 1. make your well-established model out-of-the-box for PyPOTS
 users to run, and help your work obtain more exposure and impact. Take a look
 at our [inclusion criteria](https://docs.pypots.com/en/latest/
 faq.html#inclusion-criteria). You can utilize the `template` folder in each
@@ -218,9 +256,29 @@
 Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021). [CSDI: Conditional Score-
 based Diffusion Models for Probabilistic Time Series Imputation](https://
 proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-
 Abstract.html). *NeurIPS 2021*. [^13]: Rubin, D. B. (1976). [Inference and
 missing data](https://academic.oup.com/biomet/article-abstract/63/3/581/
 270932). *Biometrika*. [^14]: Wu, H., Hu, T., Liu, Y., Zhou, H., Wang, J., &
 Long, M. (2023). [TimesNet: Temporal 2d-variation modeling for general time
-series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023* ð 
-Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023*
+[^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition
+transformers with auto-correlation for long-term series forecasting](https://
+proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-
+Abstract.html). *NeurIPS 2021*. [^16]: Zhang, Y., & Yan, J. (2023).
+[Crossformer: Transformer utilizing cross-dimension dependency for multivariate
+time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR
+2023*. [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers
+effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/
+article/view/26317). *AAAI 2023* [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., &
+Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting
+with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
+[^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer:
+Exponential Smoothing Transformers for Time-series Forecasting](https://
+openreview.net/forum?id=5m_3whfo483). *ICLR 2023* [^20]: Zhou, T., Ma, Z., Wen,
+Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced
+decomposed transformer for long-term series forecasting](https://
+proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*. [^21]: Zhou, H., Zhang,
+S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer:
+Beyond efficient transformer for long sequence time-series forecasting](https:/
+/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. ð  Visits
+_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.3.2/pypots/__init__.py` & `pypots-0.4/pypots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.3.2"
+__version__ = "0.4"
 
 
 from . import imputation, classification, clustering, forecasting, optim, data, utils
 
 __all__ = [
     "imputation",
     "classification",
```

### Comparing `pypots-0.3.2/pypots/base.py` & `pypots-0.4/pypots/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,64 +328,14 @@
                     self.model.module.load_state_dict(loaded_model.state_dict())
             else:
                 self.model = loaded_model.model
         except Exception as e:
             raise e
         logger.info(f"Model loaded successfully from {path}")
 
-    def save_model(
-        self,
-        saving_path: str,
-        overwrite: bool = False,
-    ) -> None:
-        """Save the model with current parameters to a disk file.
-
-        A ``.pypots`` extension will be appended to the filename if it does not already have one.
-        Please note that such an extension is not necessary, but to indicate the saved model is from PyPOTS framework
-        so people can distinguish.
-
-        Parameters
-        ----------
-        saving_path :
-            The given path to save the model. The directory will be created if it does not exist.
-
-        overwrite :
-            Whether to overwrite the model file if the path already exists.
-
-        Warnings
-        --------
-        The method save_model is deprecated. Please use `save()` instead.
-        """
-        logger.warning(
-            "🚨DeprecationWarning: The method save_model is deprecated. Please use `save()` instead."
-        )
-        self.save(saving_path, overwrite)
-
-    def load_model(self, path: str) -> None:
-        """Load the saved model from a disk file.
-
-        Parameters
-        ----------
-        path :
-            The local path to a disk file saving the trained model.
-
-        Notes
-        -----
-        If the training environment and the deploying/test environment use the same type of device (GPU/CPU),
-        you can load the model directly with torch.load(model_path).
-
-        Warnings
-        --------
-        The method load_model is deprecated. Please use `load()` instead.
-        """
-        logger.warning(
-            "🚨DeprecationWarning: The method load_model is deprecated. Please use `load()` instead."
-        )
-        self.load(path)
-
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
@@ -496,14 +446,16 @@
         A dictionary contains the trained model that achieves the best performance according to the loss defined,
         i.e. the lowest loss.
 
     best_loss : float, default = inf,
         The criteria to judge whether the model's performance is the best so far.
         Usually the lower, the better.
 
+    best_epoch : int, default = -1,
+        The epoch number when the best loss is got.
 
     Notes
     -----
     Optimizers are necessary for training deep-learning neural networks, but we don't put a parameter ``optimizer``
     here because some models (e.g. GANs) need more than one optimizer (e.g. one for generator, one for discriminator),
     and ``optimizer`` is ambiguous for them. Therefore, we leave optimizers as parameters for concrete model
     implementations, and you can pass any number of optimizers to your model when implementing it,
@@ -540,16 +492,16 @@
         self.patience = patience
         self.original_patience = patience
         self.num_workers = num_workers
 
         self.model = None
         self.optimizer = None
         self.best_model_dict = None
-        # WDU: may enable users to customize the criteria in the future
         self.best_loss = float("inf")
+        self.best_epoch = -1
 
     def _print_model_size(self) -> None:
         """Print the number of trainable parameters in the initialized NN model."""
         num_params = sum(p.numel() for p in self.model.parameters() if p.requires_grad)
         logger.info(
             f"{self.__class__.__name__} initialized with the given hyperparameters, "
             f"the number of trainable parameters: {num_params:,}"
```

### Comparing `pypots-0.3.2/pypots/classification/base.py` & `pypots-0.4/pypots/classification/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,39 +308,40 @@
                             results = self.model.forward(inputs)
                             epoch_val_loss_collector.append(
                                 results["loss"].sum().item()
                             )
 
                     mean_val_loss = np.mean(epoch_val_loss_collector)
 
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "classification_loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
 
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -372,15 +373,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
```

### Comparing `pypots-0.3.2/pypots/classification/brits/data.py` & `pypots-0.4/pypots/classification/brits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/classification/brits/model.py` & `pypots-0.4/pypots/classification/brits/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 The implementation of BRITS for the partially-observed time-series classification task.
 
-Refer to the paper "Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018).
-BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018."
+Refer to the paper "Wei Cao, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
+BRITS: Bidirectional recurrent imputation for time series.
+In Advances in Neural Information Processing Systems, volume 31. Curran Associates, Inc., 2018."
 
 Notes
 -----
-Partial implementation uses code from https://github.com/caow13/BRITS. The bugs in the original implementation
-are fixed here.
+Partial implementation uses code from https://github.com/caow13/BRITS.
+The bugs in the original implementation are fixed here.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Optional, Union
@@ -86,21 +87,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Cao, Wei, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
-        "Brits: Bidirectional recurrent imputation for time series."
-        Advances in neural information processing systems 31 (2018).
-        <https://arxiv.org/pdf/1805.10572>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_classes: int,
```

### Comparing `pypots-0.3.2/pypots/classification/brits/modules/core.py` & `pypots-0.4/pypots/classification/brits/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/classification/grud/data.py` & `pypots-0.4/pypots/classification/grud/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/classification/grud/model.py` & `pypots-0.4/pypots/classification/grud/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of GRU-D for the partially-observed time-series imputation task.
 
-Refer to the paper "Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018).
-Recurrent Neural Networks for Multivariate Time Series with Missing Values. Scientific Reports."
+Refer to the paper "Zhengping Che, Sanjay Purushotham, Kyunghyun Cho, David Sontag, and Yan Liu.
+Recurrent Neural Networks for Multivariate Time Series with Missing Values.
+Scientific Reports, 8(1):6085, April 2018."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
@@ -76,21 +77,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Che, Zhengping, Sanjay Purushotham, Kyunghyun Cho, David Sontag, and Yan Liu.
-        "Recurrent neural networks for multivariate time series with missing values."
-        Scientific reports 8, no. 1 (2018): 6085.
-        <https://www.nature.com/articles/s41598-018-24271-9.pdf>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_classes: int,
```

### Comparing `pypots-0.3.2/pypots/classification/grud/modules/core.py` & `pypots-0.4/pypots/classification/grud/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/classification/raindrop/data.py` & `pypots-0.4/pypots/classification/raindrop/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/classification/raindrop/model.py` & `pypots-0.4/pypots/classification/raindrop/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of Raindrop for the partially-observed time-series classification task.
 
-Refer to the paper "Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022).
-Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022."
+Refer to the paper "Xiang Zhang, Marko Zeman, Theodoros Tsiligkaridis, and Marinka Zitnik.
+Graph-guided network for irregularly sampled multivariate time series.
+In ICLR, 2022."
 
 """
 
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
@@ -42,15 +43,15 @@
     n_layers :
         The number of layers in the Transformer encoder in the Raindrop model.
 
     d_model :
         The dimension of the Transformer encoder backbone.
         It is the input dimension of the multi-head self-attention layers.
 
-    d_inner :
+    d_ffn :
         The dimension of the layer in the Feed-Forward Networks (FFN).
 
     n_heads :
         The number of heads in the multi-head self-attention mechanism.
 
     dropout :
         The dropout rate for all fully-connected layers in the model.
@@ -102,30 +103,24 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Zhang, Xiang, Marko Zeman, Theodoros Tsiligkaridis, and Marinka Zitnik.
-        "Graph-guided network for irregularly sampled multivariate time series."
-        International Conference on Learning Representations (ICLR). 2022.
-        <https://openreview.net/forum?id=Kwm8I7dU-l5>`_
     """
 
     def __init__(
         self,
         n_steps,
         n_features,
         n_classes,
         n_layers,
         d_model,
-        d_inner,
+        d_ffn,
         n_heads,
         dropout,
         d_static=0,
         aggregation="mean",
         sensor_wise_mask=False,
         static=False,
         batch_size=32,
@@ -152,15 +147,15 @@
         self.n_steps = n_steps
 
         # set up the model
         self.model = _Raindrop(
             n_features,
             n_layers,
             d_model,
-            d_inner,
+            d_ffn,
             n_heads,
             n_classes,
             dropout,
             n_steps,
             d_static,
             aggregation,
             sensor_wise_mask,
```

### Comparing `pypots-0.3.2/pypots/classification/raindrop/modules/core.py` & `pypots-0.4/pypots/classification/raindrop/modules/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,30 +40,30 @@
 
 class _Raindrop(nn.Module):
     def __init__(
         self,
         n_features,
         n_layers,
         d_model,
-        d_inner,
+        d_ffn,
         n_heads,
         n_classes,
         dropout=0.3,
         max_len=215,
         d_static=9,
         aggregation="mean",
         sensor_wise_mask=False,
         static=False,
         device=None,
     ):
         super().__init__()
         self.n_layers = n_layers
         self.n_features = n_features
         self.d_model = d_model
-        self.d_inner = d_inner
+        self.d_ffn = d_ffn
         self.n_heads = n_heads
         self.n_classes = n_classes
         self.dropout = dropout
         self.max_len = max_len
         self.d_static = d_static
         self.aggregation = aggregation
         self.sensor_wise_mask = sensor_wise_mask
@@ -80,21 +80,21 @@
         self.encoder = nn.Linear(n_features * self.d_ob, n_features * self.d_ob)
         d_pe = 16
         self.pos_encoder = PositionalEncoding(d_pe, max_len)
         if self.sensor_wise_mask:
             dim_check = n_features * (self.d_ob + d_pe)
             assert dim_check % n_heads == 0, "dim_check must be divisible by n_heads"
             encoder_layers = TransformerEncoderLayer(
-                n_features * (self.d_ob + d_pe), n_heads, d_inner, dropout
+                n_features * (self.d_ob + d_pe), n_heads, d_ffn, dropout
             )
         else:
             dim_check = d_model + d_pe
             assert dim_check % n_heads == 0, "dim_check must be divisible by n_heads"
             encoder_layers = TransformerEncoderLayer(
-                d_model + d_pe, n_heads, d_inner, dropout
+                d_model + d_pe, n_heads, d_ffn, dropout
             )
         self.transformer_encoder = TransformerEncoder(encoder_layers, n_layers)
 
         self.R_u = Parameter(torch.Tensor(1, self.n_features * self.d_ob))
 
         self.ob_propagation = ObservationPropagation(
             in_channels=max_len * self.d_ob,
```

### Comparing `pypots-0.3.2/pypots/classification/raindrop/modules/submodules.py` & `pypots-0.4/pypots/classification/raindrop/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/base.py` & `pypots-0.4/pypots/cli/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/dev.py` & `pypots-0.4/pypots/cli/dev.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/doc.py` & `pypots-0.4/pypots/cli/doc.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/env.py` & `pypots-0.4/pypots/cli/env.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/pypots_cli.py` & `pypots-0.4/pypots/cli/pypots_cli.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/tuning.py` & `pypots-0.4/pypots/cli/tuning.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/cli/utils.py` & `pypots-0.4/pypots/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/clustering/base.py` & `pypots-0.4/pypots/clustering/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,29 +317,30 @@
                                 results["loss"].sum().item()
                             )
 
                     mean_val_loss = np.mean(epoch_val_loss_collector)
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 if os.getenv("enable_tuning", False):
@@ -365,15 +366,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Union[dict, str] = None,
         file_type: str = "h5py",
```

### Comparing `pypots-0.3.2/pypots/clustering/crli/data.py` & `pypots-0.4/pypots/clustering/crli/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/clustering/crli/model.py` & `pypots-0.4/pypots/clustering/crli/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The implementation of CRLI (Clustering Representation Learning on Incomplete time-series data) for
 the partially-observed time-series clustering task.
 
-Refer to the paper "Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021).
-Learning Representations for Incomplete Time Series Clustering. AAAI 2021."
+Refer to the paper "Qianli Ma, Chuxin Chen, Sen Li, and Garrison W. Cottrell.
+Learning Representations for Incomplete Time Series Clustering.
+In AAAI, 35(10):8837–8846, May 2021."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import os
@@ -105,22 +106,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Ma, Qianli, Chuxin Chen, Sen Li, and Garrison W. Cottrell. 2021.
-        "Learning Representations for Incomplete Time Series Clustering".
-        Proceedings of the AAAI Conference on Artificial Intelligence 35 (10):8837-46.
-        https://doi.org/10.1609/aaai.v35i10.17070.
-        <https://ojs.aaai.org/index.php/AAAI/article/view/17070>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_clusters: int,
@@ -272,25 +265,25 @@
                         for idx, data in enumerate(val_loader):
                             inputs = self._assemble_input_for_validating(data)
                             results = self.model.forward(inputs, training=True)
                             epoch_val_loss_G_collector.append(
                                 results["generation_loss"].sum().item()
                             )
                     mean_val_G_loss = np.mean(epoch_val_loss_G_collector)
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "generation_loss": mean_val_G_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"generator training loss: {mean_epoch_train_G_loss:.4f}, "
                         f"discriminator training loss: {mean_epoch_train_D_loss:.4f}, "
-                        f"generator validating loss: {mean_val_G_loss:.4f}"
+                        f"generator validation loss: {mean_val_G_loss:.4f}"
                     )
                     mean_loss = mean_val_G_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"generator training loss: {mean_epoch_train_G_loss:.4f}, "
                         f"discriminator training loss: {mean_epoch_train_D_loss:.4f}"
@@ -299,14 +292,15 @@
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 if os.getenv("enable_tuning", False):
@@ -338,15 +332,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
```

### Comparing `pypots-0.3.2/pypots/clustering/crli/modules/core.py` & `pypots-0.4/pypots/clustering/crli/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/clustering/crli/modules/submodules.py` & `pypots-0.4/pypots/clustering/crli/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/clustering/vader/data.py` & `pypots-0.4/pypots/clustering/vader/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/clustering/vader/model.py` & `pypots-0.4/pypots/clustering/vader/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The implementation of VaDER for the partially-observed time-series clustering task.
 
-Refer to the paper "Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A.,
-Hofmann-Apitius, M., & Fröhlich, H. (2019).
-Deep learning for clustering of multivariate clinical patient trajectories with missing values. GigaScience."
+Refer to the paper "Johann de Jong, Mohammad Asif Emon, Ping Wu, Reagon Karki, Meemansa Sood, Patrice Godard,
+Ashar Ahmad, Henri Vrooman, Martin Hofmann-Apitius, and Holger Fröhlich.
+Deep learning for clustering of multivariate clinical patient trajectories with missing values.
+GigaScience, 8(11):giz134, November 2019."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
@@ -88,24 +89,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `de Jong, Johann, Mohammad Asif Emon, Ping Wu, Reagon Karki, Meemansa Sood, Patrice Godard,
-    Ashar Ahmad, Henri Vrooman, Martin Hofmann-Apitius, and Holger Fröhlich.
-    "Deep learning for clustering of multivariate clinical patient trajectories with missing values."
-    GigaScience 8, no. 11 (2019): giz134.
-    <https://academic.oup.com/gigascience/article-pdf/8/11/giz134/30797160/giz134.pdf>`_
-
-
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_clusters: int,
@@ -289,39 +280,40 @@
                             results = self.model.forward(inputs)
                             epoch_val_loss_collector.append(
                                 results["loss"].sum().item()
                             )
 
                     mean_val_loss = np.mean(epoch_val_loss_collector)
 
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
 
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -353,15 +345,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
```

### Comparing `pypots-0.3.2/pypots/clustering/vader/modules/core.py` & `pypots-0.4/pypots/clustering/vader/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/clustering/vader/modules/submodules.py` & `pypots-0.4/pypots/clustering/vader/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/__init__.py` & `pypots-0.4/pypots/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/base.py` & `pypots-0.4/pypots/data/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/generating.py` & `pypots-0.4/pypots/data/generating.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/load_preprocessing.py` & `pypots-0.4/pypots/data/load_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/load_specific_datasets.py` & `pypots-0.4/pypots/data/load_specific_datasets.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/saving/h5.py` & `pypots-0.4/pypots/data/saving/h5.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/saving/pickle.py` & `pypots-0.4/pypots/data/saving/pickle.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/data/utils.py` & `pypots-0.4/pypots/data/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/forecasting/base.py` & `pypots-0.4/pypots/forecasting/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,39 +302,40 @@
                                 .detach()
                                 .item()
                             )
                             forecasting_loss_collector.append(forecasting_mse)
 
                     mean_val_loss = np.mean(forecasting_loss_collector)
 
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "forecasting_loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
 
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -366,15 +367,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
```

### Comparing `pypots-0.3.2/pypots/forecasting/bttf/model.py` & `pypots-0.4/pypots/forecasting/bttf/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The implementation of BTTF (Bayesian Temporal Tensor Factorization) for the partially-observed time-series
 forecasting task.
 
-Refer to the paper "Chen, X., & Sun, L. (2021).
+Refer to the paper "Xinyu Chen and Lijun Sun.
 Bayesian Temporal Factorization for Multidimensional Time Series Prediction.
-IEEE transactions on pattern analysis and machine intelligence."
+IEEE Transactions on Pattern Analysis and Machine Intelligence, pages 1–1, 2021."
 
 Notes
 -----
 This numpy implementation is the same with the official one from https://github.com/xinychen/transdim.
 
 """
 
@@ -65,21 +65,14 @@
 
     Notes
     -----
     1). ``n_steps`` must be larger than ``pred_step``;
 
     2). ``n_steps - pred_step`` must be larger than ``max(time_lags)``;
 
-    References
-    ----------
-    .. [1] `Chen, Xinyu, and Lijun Sun.
-        "Bayesian temporal factorization for multidimensional time series prediction."
-        IEEE Transactions on Pattern Analysis and Machine Intelligence 44, no. 9 (2021): 4659-4673.
-        <https://arxiv.org/pdf/1910.06366>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         pred_step: int,
```

### Comparing `pypots-0.3.2/pypots/forecasting/bttf/modules/core.py` & `pypots-0.4/pypots/forecasting/bttf/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/forecasting/bttf/modules/submodules.py` & `pypots-0.4/pypots/forecasting/bttf/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/base.py` & `pypots-0.4/pypots/imputation/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,39 +305,40 @@
                                 .detach()
                                 .item()
                             )
                             imputation_loss_collector.append(imputation_mse)
 
                     mean_val_loss = np.mean(imputation_loss_collector)
 
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "imputation_loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
 
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -369,15 +370,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
```

### Comparing `pypots-0.3.2/pypots/imputation/brits/data.py` & `pypots-0.4/pypots/imputation/brits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/brits/model.py` & `pypots-0.4/pypots/imputation/brits/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 The implementation of BRITS for the partially-observed time-series imputation task.
 
-Refer to the paper "Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018).
-BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018."
+Refer to the paper "Wei Cao, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
+BRITS: Bidirectional recurrent imputation for time series.
+In Advances in Neural Information Processing Systems, volume 31. Curran Associates, Inc., 2018."
 
 Notes
 -----
-Partial implementation uses code from https://github.com/caow13/BRITS. The bugs in the original implementation
-are fixed here.
+Partial implementation uses code from https://github.com/caow13/BRITS.
+The bugs in the original implementation are fixed here.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
@@ -78,21 +79,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Cao, Wei, Dong Wang, Jian Li, Hao Zhou, Lei Li, and Yitan Li.
-        "Brits: Bidirectional recurrent imputation for time series."
-        Advances in neural information processing systems 31 (2018).
-        <https://arxiv.org/pdf/1805.10572>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
```

### Comparing `pypots-0.3.2/pypots/imputation/brits/modules/core.py` & `pypots-0.4/pypots/imputation/brits/modules/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,28 +97,31 @@
         )
         self.hist_reg = nn.Linear(self.rnn_hidden_size, self.n_features)
         self.feat_reg = FeatureRegression(self.n_features)
         self.combining_weight = nn.Linear(self.n_features * 2, self.n_features)
 
     def impute(
         self, inputs: dict, direction: str
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         """The imputation function.
         Parameters
         ----------
         inputs :
             Input data, a dictionary includes feature values, missing masks, and time-gap values.
 
         direction :
             A keyword to extract data from parameter `data`.
 
         Returns
         -------
         imputed_data :
-            [batch size, sequence length, feature number]
+            Input data with missing parts imputed. Shape of [batch size, sequence length, feature number].
+
+        estimations :
+            Reconstructed data. Shape of [batch size, sequence length, feature number].
 
         hidden_states: tensor,
             [batch size, RNN hidden size]
 
         reconstruction_loss :
             reconstruction loss
 
@@ -168,15 +171,15 @@
             inputs = torch.cat([c_c, m], dim=1)
             hidden_states, cell_states = self.rnn_cell(
                 inputs, (hidden_states, cell_states)
             )
 
         estimations = torch.cat(estimations, dim=1)
         imputed_data = masks * values + (1 - masks) * estimations
-        return imputed_data, hidden_states, reconstruction_loss
+        return imputed_data, estimations, hidden_states, reconstruction_loss
 
     def forward(self, inputs: dict, direction: str = "forward") -> dict:
         """Forward processing of the NN module.
         Parameters
         ----------
         inputs :
             The input data.
@@ -186,24 +189,27 @@
 
         Returns
         -------
         dict,
             A dictionary includes all results.
 
         """
-        imputed_data, hidden_state, reconstruction_loss = self.impute(inputs, direction)
+        imputed_data, estimations, hidden_state, reconstruction_loss = self.impute(
+            inputs, direction
+        )
         # for each iteration, reconstruction_loss increases its value for 3 times
         reconstruction_loss /= self.n_steps * 3
 
         ret_dict = {
             "consistency_loss": torch.tensor(
                 0.0, device=imputed_data.device
             ),  # single direction, has no consistency loss
             "reconstruction_loss": reconstruction_loss,
             "imputed_data": imputed_data,
+            "reconstructed_data": estimations,
             "final_hidden_state": hidden_state,
         }
         return ret_dict
 
 
 class _BRITS(nn.Module):
     """model BRITS: Bidirectional RITS
@@ -300,14 +306,17 @@
     def forward(self, inputs: dict, training: bool = True) -> dict:
         # Results from the forward RITS.
         ret_f = self.rits_f(inputs, "forward")
         # Results from the backward RITS.
         ret_b = self._reverse(self.rits_b(inputs, "backward"))
 
         imputed_data = (ret_f["imputed_data"] + ret_b["imputed_data"]) / 2
+        reconstructed_data = (
+            ret_f["reconstructed_data"] + ret_b["reconstructed_data"]
+        ) / 2
 
         results = {
             "imputed_data": imputed_data,
         }
 
         # if in training mode, return results with losses
         if training:
@@ -319,9 +328,12 @@
                 consistency_loss
                 + ret_f["reconstruction_loss"]
                 + ret_b["reconstruction_loss"]
             )
 
             # `loss` is always the item for backward propagating to update the model
             results["loss"] = loss
+            results["reconstructed_data"] = reconstructed_data
+            results["f_reconstructed_data"] = ret_f["reconstructed_data"]
+            results["b_reconstructed_data"] = ret_b["reconstructed_data"]
 
         return results
```

### Comparing `pypots-0.3.2/pypots/imputation/brits/modules/submodules.py` & `pypots-0.4/pypots/imputation/brits/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/csdi/data.py` & `pypots-0.4/pypots/imputation/csdi/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/csdi/model.py` & `pypots-0.4/pypots/imputation/csdi/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of CSDI for the partially-observed time-series imputation task.
 
-Refer to the paper Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021).
-CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation. NeurIPS 2021.
+Refer to the paper "Yusuke Tashiro, Jiaming Song, Yang Song, and Stefano Ermon.
+CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation.
+In NeurIPS, 2021."
 
 Notes
 -----
 Partial implementation uses code from the official implementation https://github.com/ermongroup/CSDI.
 
 """
 
@@ -39,15 +40,15 @@
 
     Parameters
     ----------
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
-        The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
+        The number of layers in the CSDI model.
 
     n_heads :
         The number of heads in the multi-head attention mechanism.
 
     n_channels :
         The number of residual channels.
 
@@ -113,21 +114,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Yusuke Tashiro, Jiaming Song, Yang Song, Stefano Ermon.
-        "CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation".
-        NeurIPS 2021.
-        <https://proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-Abstract.html>`_
-
     """
 
     def __init__(
         self,
         n_features: int,
         n_layers: int,
         n_heads: int,
@@ -260,39 +254,40 @@
                             results = self.model.forward(
                                 inputs, training=False, n_sampling_times=0
                             )
                             val_loss_collector.append(results["loss"].sum().item())
 
                     mean_val_loss = np.asarray(val_loss_collector).mean()
 
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "validating_loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
 
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -324,15 +319,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
         n_sampling_times: int = 1,
```

### Comparing `pypots-0.3.2/pypots/imputation/csdi/modules/core.py` & `pypots-0.4/pypots/imputation/csdi/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/csdi/modules/submodules.py` & `pypots-0.4/pypots/imputation/csdi/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/gpvae/data.py` & `pypots-0.4/pypots/imputation/gpvae/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/gpvae/model.py` & `pypots-0.4/pypots/imputation/gpvae/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of GP-VAE for the partially-observed time-series imputation task.
 
-Refer to the paper Fortuin V, Baranchuk D, Rätsch G, et al.
-GP-VAE: Deep probabilistic time series imputation. AISTATS. PMLR, 2020: 1651-1661.
+Refer to the paper "Vincent Fortuin, Dmitry Baranchuk, Gunnar Rätsch, and Stephan Mandt.
+GP-VAE: Deep probabilistic time series imputation.
+In International conference on artificial intelligence and statistics, pages 1651–1661. PMLR, 2020."
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
@@ -30,15 +31,15 @@
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mse
 
 
 class GPVAE(BaseNNImputer):
-    """The PyTorch implementation of the GPVAE model :cite:`fortuin2020GPVAEDeep`.
+    """The PyTorch implementation of the GPVAE model :cite:`fortuin2020gpvae`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
@@ -111,22 +112,14 @@
     model_saving_strategy : str
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
-    References
-    ----------
-    .. [1] `Fortuin, V., Baranchuk, D., Raetsch, G. &amp; Mandt, S.. (2020).
-        "GP-VAE: Deep Probabilistic Time Series Imputation".
-        <i>Proceedings of the Twenty Third International Conference on Artificial Intelligence and Statistics</i>,
-        in <i>Proceedings of Machine Learning Research</i> 108:1651-1661
-        <https://proceedings.mlr.press/v108/fortuin20a.html>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         latent_size: int,
@@ -291,39 +284,40 @@
                                 .detach()
                                 .item()
                             )
                             imputation_loss_collector.append(imputation_mse)
 
                     mean_val_loss = np.mean(imputation_loss_collector)
 
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "imputation_loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
 
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"training loss: {mean_train_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - training loss: {mean_train_loss:.4f}"
                     )
                     mean_loss = mean_train_loss
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -355,15 +349,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
```

### Comparing `pypots-0.3.2/pypots/imputation/gpvae/modules/core.py` & `pypots-0.4/pypots/imputation/gpvae/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/gpvae/modules/submodules.py` & `pypots-0.4/pypots/imputation/gpvae/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/locf/model.py` & `pypots-0.4/pypots/imputation/locf/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/locf/modules/core.py` & `pypots-0.4/pypots/imputation/locf/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/mean/model.py` & `pypots-0.4/pypots/imputation/mean/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/median/model.py` & `pypots-0.4/pypots/imputation/median/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/mrnn/data.py` & `pypots-0.4/pypots/imputation/mrnn/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/mrnn/model.py` & `pypots-0.4/pypots/imputation/mrnn/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """
-PyTorch MRNN model for the time-series imputation task.
+PyTorch M-RNN model for the time-series imputation task.
+
+Refer to the paper "Jinsung Yoon, William R. Zame, and Mihaela van der Schaar.
+Estimating missing data in temporal data streams using multi-directional recurrent neural networks.
+EEE Transactions on Biomedical Engineering, 66(5):14771490, 2019."
 
 This implementation is inspired by the official one https://github.com/jsyoon0823/MRNN.
 Some part of the code is from https://github.com/WenjieDu/SAITS.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
@@ -74,22 +78,14 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `J. Yoon, W. R. Zame and M. van der Schaar,
-        "Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks,"
-        in IEEE Transactions on Biomedical Engineering,
-        vol. 66, no. 5, pp. 1477-1490, May 2019, doi: 10.1109/TBME.2018.2874712.
-        <https://arxiv.org/pdf/1711.08742>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
```

### Comparing `pypots-0.3.2/pypots/imputation/mrnn/modules/core.py` & `pypots-0.4/pypots/imputation/mrnn/modules/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/mrnn/modules/submodules.py` & `pypots-0.4/pypots/imputation/mrnn/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/saits/data.py` & `pypots-0.4/pypots/imputation/saits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/saits/model.py` & `pypots-0.4/pypots/imputation/saits/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of SAITS for the partially-observed time-series imputation task.
 
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
+Refer to the paper "Wenjie Du, David Cote, and Yan Liu.
+SAITS: Self-Attention-based Imputation for Time Series.
+Expert Systems with Applications, 219:119619, 2023."
 
 Notes
 -----
 Partial implementation uses code from https://github.com/WenjieDu/SAITS.
 
 """
 
@@ -44,15 +45,15 @@
     n_layers :
         The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
 
     d_model :
         The dimension of the model's backbone.
         It is the input dimension of the multi-head DMSA layers.
 
-    d_inner :
+    d_ffn :
         The dimension of the layer in the Feed-Forward Networks (FFN).
 
     n_heads :
         The number of heads in the multi-head DMSA mechanism.
         ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
 
     d_k :
@@ -119,30 +120,23 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Du, Wenjie, David Côté, and Yan Liu.
-        "Saits: Self-attention-based imputation for time series".
-        Expert Systems with Applications 219 (2023): 119619.
-        <https://arxiv.org/pdf/2202.08516>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float = 0,
         attn_dropout: float = 0,
         diagonal_attention_mask: bool = True,
         ORT_weight: int = 1,
@@ -178,15 +172,15 @@
             )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.n_layers = n_layers
         self.d_model = d_model
-        self.d_inner = d_inner
+        self.d_ffn = d_ffn
         self.n_heads = n_heads
         self.d_k = d_k
         self.d_v = d_v
         self.dropout = dropout
         self.attn_dropout = attn_dropout
         self.diagonal_attention_mask = diagonal_attention_mask
         self.ORT_weight = ORT_weight
@@ -194,15 +188,15 @@
 
         # set up the model
         self.model = _SAITS(
             self.n_layers,
             self.n_steps,
             self.n_features,
             self.d_model,
-            self.d_inner,
+            self.d_ffn,
             self.n_heads,
             self.d_k,
             self.d_v,
             self.dropout,
             self.attn_dropout,
             self.diagonal_attention_mask,
             self.ORT_weight,
```

### Comparing `pypots-0.3.2/pypots/imputation/saits/modules/core.py` & `pypots-0.4/pypots/imputation/saits/modules/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 from typing import Tuple, Optional, Callable
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ....nn.modules.transformer import EncoderLayer, PositionalEncoding
+from ....nn.modules.transformer.attention import ScaledDotProductAttention
 from ....utils.metrics import calc_mae
 
 
 class _SAITS(nn.Module):
     def __init__(
         self,
         n_layers: int,
         n_steps: int,
         n_features: int,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float,
         attn_dropout: float,
         diagonal_attention_mask: bool = True,
         ORT_weight: float = 1,
@@ -51,34 +52,34 @@
         self.MIT_weight = MIT_weight
         self.customized_loss_func = customized_loss_func
 
         self.layer_stack_for_first_block = nn.ModuleList(
             [
                 EncoderLayer(
                     d_model,
-                    d_inner,
+                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     dropout,
-                    attn_dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
         self.layer_stack_for_second_block = nn.ModuleList(
             [
                 EncoderLayer(
                     d_model,
-                    d_inner,
+                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     dropout,
-                    attn_dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
         self.dropout = nn.Dropout(p=dropout)
         self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
```

### Comparing `pypots-0.3.2/pypots/imputation/timesnet/data.py` & `pypots-0.4/pypots/imputation/timesnet/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/timesnet/model.py` & `pypots-0.4/pypots/imputation/etsformer/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 """
-The implementation of Transformer for the partially-observed time-series imputation task.
+The implementation of ETSformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
+Refer to the paper "Gerald Woo, Chenghao Liu, Doyen Sahoo, Akshat Kumar, and Steven Hoi.
+ETSformer: Exponential smoothing transformers for time-series forecasting.
+In ICLR, 2023."
 
 Notes
 -----
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
+Partial implementation uses code from https://github.com/salesforce/ETSformer
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .data import DatasetForTimesNet
-from .modules.core import _TimesNet
+from .data import DatasetForETSformer
+from .modules.core import _ETSformer
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
-class TimesNet(BaseNNImputer):
-    """The PyTorch implementation of the TimesNet model.
-    TimesNet is originally proposed by Wu et al. in :cite:`wu2023timesnet`.
+class ETSformer(BaseNNImputer):
+    """The PyTorch implementation of the ETSformer model.
+    ETSformer is originally proposed by Woo et al. in :cite:`woo2023etsformer`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
-    n_layers :
-        The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
+    n_e_layers :
+        The number of layers in the ETSformer encoder.
 
-    top_k :
-        The number of top-k amplitude values to be selected to  obtain the most significant frequencies.
+    n_d_layers :
+        The number of layers in the ETSformer decoder.
+
+    n_heads :
+        The number of heads in each layer of ETSformer.
 
     d_model :
         The dimension of the model.
 
     d_ffn :
         The dimension of the feed-forward network.
 
-    n_kernels :
-        The number of 2D kernels (2D convolutional layers) to use in the submodule InceptionBlockV1.
+    top_k :
+        Top-K Fourier bases.
 
     dropout :
         The dropout rate for the model.
 
-    apply_nonstationary_norm :
-        Whether to apply non-stationary normalization to the input data for TimesNet.
-        Please refer to :cite:`liu2022nonstationary` for details about non-stationary normalization,
-        which is not the idea of the original TimesNet paper. Hence, we make it optional and default not to use here.
-
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -99,35 +98,27 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    Attributes
-    ----------
-    model : :class:`torch.nn.Module`
-        The underlying Transformer model.
-
-    optimizer : :class:`pypots.optim.Optimizer`
-        The optimizer for model training.
-
     """
 
     def __init__(
         self,
-        n_steps: int,
-        n_features: int,
-        n_layers: int,
-        top_k: int,
-        d_model: int,
-        d_ffn: int,
-        n_kernels: int,
+        n_steps,
+        n_features,
+        n_e_layers,
+        n_d_layers,
+        n_heads,
+        d_model,
+        d_ffn,
+        top_k,
         dropout: float = 0,
-        apply_nonstationary_norm: bool = False,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -142,33 +133,33 @@
             saving_path,
             model_saving_strategy,
         )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
-        self.n_layers = n_layers
-        self.top_k = top_k
+        self.n_heads = n_heads
+        self.n_e_layers = n_e_layers
+        self.n_d_layers = n_d_layers
         self.d_model = d_model
         self.d_ffn = d_ffn
-        self.n_kernels = n_kernels
         self.dropout = dropout
-        self.apply_nonstationary_norm = apply_nonstationary_norm
+        self.top_k = top_k
 
         # set up the model
-        self.model = _TimesNet(
-            self.n_layers,
+        self.model = _ETSformer(
             self.n_steps,
             self.n_features,
-            self.top_k,
+            self.n_e_layers,
+            self.n_d_layers,
+            self.n_heads,
             self.d_model,
             self.d_ffn,
-            self.n_kernels,
             self.dropout,
-            self.apply_nonstationary_norm,
+            self.top_k,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
@@ -207,28 +198,28 @@
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForTimesNet(
+        training_set = DatasetForETSformer(
             train_set, return_X_ori=False, return_labels=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
             if not check_X_ori_in_val_set(val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForTimesNet(
+            val_set = DatasetForETSformer(
                 val_set, return_X_ori=True, return_labels=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
```

### Comparing `pypots-0.3.2/pypots/imputation/timesnet/modules/core.py` & `pypots-0.4/pypots/imputation/timesnet/modules/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import torch.nn as nn
 
-from .embedding import DataEmbedding
-from .layer import TimesBlock
+from .submodules import TimesBlock
 from ....nn.functional import nonstationary_norm, nonstationary_denorm
+from ....nn.modules.transformer.embedding import DataEmbedding
 from ....utils.metrics import calc_mse
 
 
 class _TimesNet(nn.Module):
     def __init__(
         self,
         n_layers,
```

### Comparing `pypots-0.3.2/pypots/imputation/timesnet/modules/layer.py` & `pypots-0.4/pypots/imputation/timesnet/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/transformer/data.py` & `pypots-0.4/pypots/imputation/transformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/transformer/model.py` & `pypots-0.4/pypots/imputation/transformer/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of Transformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
+Refer to the paper "Wenjie Du, David Cote, and Yan Liu.
+SAITS: Self-Attention-based Imputation for Time Series.
+Expert Systems with Applications, 219:119619, 2023."
 
 Notes
 -----
 Partial implementation uses code from https://github.com/WenjieDu/SAITS.
 
 """
 
@@ -46,15 +47,15 @@
     n_layers :
         The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
 
     d_model :
         The dimension of the model's backbone.
         It is the input dimension of the multi-head self-attention layers.
 
-    d_inner :
+    d_ffn :
         The dimension of the layer in the Feed-Forward Networks (FFN).
 
     n_heads :
         The number of heads in the multi-head self-attention mechanism.
         ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
 
     d_k :
@@ -113,36 +114,23 @@
         The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
-    References
-    ----------
-    .. [1] `Vaswani, Ashish, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser,
-        and Illia Polosukhin.
-        "Attention is all you need."
-        Advances in neural information processing systems 30 (2017).
-        <https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf>`_
-
-    .. [2] `Du, Wenjie, David Côté, and Yan Liu.
-        "Saits: Self-attention-based imputation for time series".
-        Expert Systems with Applications 219 (2023): 119619.
-        <https://arxiv.org/pdf/2202.08516>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float = 0,
         attn_dropout: float = 0,
         ORT_weight: int = 1,
         MIT_weight: int = 1,
@@ -176,30 +164,30 @@
             )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.n_layers = n_layers
         self.d_model = d_model
-        self.d_inner = d_inner
+        self.d_ffn = d_ffn
         self.n_heads = n_heads
         self.d_k = d_k
         self.d_v = d_v
         self.dropout = dropout
         self.attn_dropout = attn_dropout
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _TransformerEncoder(
             self.n_layers,
             self.n_steps,
             self.n_features,
             self.d_model,
-            self.d_inner,
+            self.d_ffn,
             self.n_heads,
             self.d_k,
             self.d_v,
             self.dropout,
             self.attn_dropout,
             self.ORT_weight,
             self.MIT_weight,
```

### Comparing `pypots-0.3.2/pypots/imputation/transformer/modules/core.py` & `pypots-0.4/pypots/imputation/transformer/modules/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 
 from typing import Tuple
 
 import torch
 import torch.nn as nn
 
 from ....nn.modules.transformer import EncoderLayer, PositionalEncoding
+from ....nn.modules.transformer.attention import ScaledDotProductAttention
 from ....utils.metrics import calc_mae
 
 
 class _TransformerEncoder(nn.Module):
     def __init__(
         self,
         n_layers: int,
         d_time: int,
         d_feature: int,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float,
         attn_dropout: float,
         ORT_weight: float = 1,
         MIT_weight: float = 1,
@@ -44,20 +45,20 @@
         self.ORT_weight = ORT_weight
         self.MIT_weight = MIT_weight
 
         self.layer_stack = nn.ModuleList(
             [
                 EncoderLayer(
                     d_model,
-                    d_inner,
+                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     dropout,
-                    attn_dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
         self.embedding = nn.Linear(actual_d_feature, d_model)
         self.position_enc = PositionalEncoding(d_model, n_positions=d_time)
```

### Comparing `pypots-0.3.2/pypots/imputation/usgan/data.py` & `pypots-0.4/pypots/imputation/usgan/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/imputation/usgan/model.py` & `pypots-0.4/pypots/imputation/usgan/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The implementation of USGAN for the partially-observed time-series imputation task.
 
-Refer to the paper "Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021).
-Generative Semi-supervised Learning for Multivariate Time Series Imputation. AAAI 2021."
+Refer to the paper "Xiaoye Miao, Yangyang Wu, Jun Wang, Yunjun Gao, Xudong Mao, and Jianwei Yin.
+Generative Semi-supervised Learning for Multivariate Time Series Imputation.
+In AAAI, 35(10):8983–8991, May 2021."
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import os
@@ -98,21 +99,14 @@
     model_saving_strategy : str
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
-    References
-    ----------
-    .. [1] `Miao, Xiaoye, Yangyang Wu, Jun Wang, Yunjun Gao, Xudong Mao, and Jianwei Yin. 2021.
-       "Generative Semi-Supervised Learning for Multivariate Time Series Imputation".
-       Proceedings of the AAAI Conference on Artificial Intelligence 35 (10):8983-91.
-       <https://doi.org/10.1609/aaai.v35i10.17086>`_
-
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
@@ -238,25 +232,22 @@
     ) -> None:
         # each training starts from the very beginning, so reset the loss and model dict here
         self.best_loss = float("inf")
         self.best_model_dict = None
 
         try:
             training_step = 0
-            epoch_train_loss_G_collector = []
-            epoch_train_loss_D_collector = []
             for epoch in range(1, self.epochs + 1):
                 self.model.train()
+                step_train_loss_G_collector = []
+                step_train_loss_D_collector = []
                 for idx, data in enumerate(training_loader):
                     training_step += 1
                     inputs = self._assemble_input_for_training(data)
 
-                    step_train_loss_G_collector = []
-                    step_train_loss_D_collector = []
-
                     if idx % self.G_steps == 0:
                         self.G_optimizer.zero_grad()
                         results = self.model.forward(
                             inputs, training_object="generator"
                         )
                         results["generation_loss"].backward()
                         self.G_optimizer.step()
@@ -274,30 +265,27 @@
                         step_train_loss_D_collector.append(
                             results["discrimination_loss"].item()
                         )
 
                     mean_step_train_D_loss = np.mean(step_train_loss_D_collector)
                     mean_step_train_G_loss = np.mean(step_train_loss_G_collector)
 
-                    epoch_train_loss_D_collector.append(mean_step_train_D_loss)
-                    epoch_train_loss_G_collector.append(mean_step_train_G_loss)
-
                     # save training loss logs into the tensorboard file for every step if in need
                     # Note: the `training_step` is not the actual number of steps that Discriminator and Generator get
                     # trained, the actual number should be D_steps*training_step and G_steps*training_step accordingly
                     if self.summary_writer is not None:
                         loss_results = {
                             "generation_loss": mean_step_train_G_loss,
                             "discrimination_loss": mean_step_train_D_loss,
                         }
                         self._save_log_into_tb_file(
                             training_step, "training", loss_results
                         )
-                mean_epoch_train_D_loss = np.mean(epoch_train_loss_D_collector)
-                mean_epoch_train_G_loss = np.mean(epoch_train_loss_G_collector)
+                mean_epoch_train_D_loss = np.mean(step_train_loss_D_collector)
+                mean_epoch_train_G_loss = np.mean(step_train_loss_G_collector)
 
                 if val_loader is not None:
                     self.model.eval()
                     imputation_loss_collector = []
                     with torch.no_grad():
                         for idx, data in enumerate(val_loader):
                             inputs = self._assemble_input_for_validating(data)
@@ -311,25 +299,25 @@
                                 .sum()
                                 .detach()
                                 .item()
                             )
                             imputation_loss_collector.append(imputation_mse)
 
                     mean_val_loss = np.mean(imputation_loss_collector)
-                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    # save validation loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "validating_loss": mean_val_loss,
                         }
                         self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"generator training loss: {mean_epoch_train_G_loss:.4f}, "
                         f"discriminator training loss: {mean_epoch_train_D_loss:.4f}, "
-                        f"validating loss: {mean_val_loss:.4f}"
+                        f"validation loss: {mean_val_loss:.4f}"
                     )
                     mean_loss = mean_val_loss
                 else:
                     logger.info(
                         f"Epoch {epoch:03d} - "
                         f"generator training loss: {mean_epoch_train_G_loss:.4f}, "
                         f"discriminator training loss: {mean_epoch_train_D_loss:.4f}"
@@ -338,14 +326,15 @@
 
                 if np.isnan(mean_loss):
                     logger.warning(
                         f"‼️ Attention: got NaN loss in Epoch {epoch}. This may lead to unexpected errors."
                     )
 
                 if mean_loss < self.best_loss:
+                    self.best_epoch = epoch
                     self.best_loss = mean_loss
                     self.best_model_dict = self.model.state_dict()
                     self.patience = self.original_patience
                 else:
                     self.patience -= 1
 
                 # save the model if necessary
@@ -377,15 +366,17 @@
                     "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.isnan(self.best_loss):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
-        logger.info("Finished training.")
+        logger.info(
+            f"Finished training. The best model is from epoch#{self.best_epoch}."
+        )
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
```

### Comparing `pypots-0.3.2/pypots/imputation/usgan/modules/core.py` & `pypots-0.4/pypots/imputation/usgan/modules/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # License: BSD-3-Clause
 
 from typing import Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from ....utils.metrics import calc_mse
 
 from .submodules import Discriminator
 from ...brits.modules import _BRITS
 
 
 class _USGAN(nn.Module):
     """USGAN model"""
@@ -58,28 +59,35 @@
 
         results = self.generator(inputs, training=training)
 
         # if in training mode, return results with losses
         if training:
             forward_X = inputs["forward"]["X"]
             forward_missing_mask = inputs["forward"]["missing_mask"]
-
-            inputs["discrimination"] = self.discriminator(
-                forward_X, forward_missing_mask
-            )
+            imputed_data = results["imputed_data"]
 
             if training_object == "discriminator":
+                inputs["discrimination"] = self.discriminator(
+                    imputed_data.detach(), forward_missing_mask
+                )
                 l_D = F.binary_cross_entropy_with_logits(
                     inputs["discrimination"], forward_missing_mask
                 )
                 results["discrimination_loss"] = l_D
             else:
-                inputs["discrimination"] = inputs["discrimination"].detach()
-                l_G = F.binary_cross_entropy_with_logits(
+                inputs["discrimination"] = self.discriminator(
+                    imputed_data, forward_missing_mask
+                )
+                l_G = -F.binary_cross_entropy_with_logits(
                     inputs["discrimination"],
-                    1 - forward_missing_mask,
+                    forward_missing_mask,
                     weight=1 - forward_missing_mask,
                 )
-                loss_gene = l_G + self.lambda_mse * results["loss"]
+                reconstruction_loss = calc_mse(
+                    forward_X, results["reconstructed_data"], forward_missing_mask
+                ) + 0.1 * calc_mse(
+                    results["f_reconstructed_data"], results["b_reconstructed_data"]
+                )
+                loss_gene = l_G + self.lambda_mse * reconstruction_loss
                 results["generation_loss"] = loss_gene
 
         return results
```

### Comparing `pypots-0.3.2/pypots/imputation/usgan/modules/submodules.py` & `pypots-0.4/pypots/imputation/usgan/modules/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/nn/functional/normalization.py` & `pypots-0.4/pypots/nn/functional/normalization.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/nn/modules/rnn.py` & `pypots-0.4/pypots/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/nn/modules/transformer/attention.py` & `pypots-0.4/pypots/nn/modules/transformer/attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,38 @@
 # License: BSD-3-Clause
 
 from typing import Tuple, Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from abc import abstractmethod
 
 
-class ScaledDotProductAttention(nn.Module):
+class AttentionOperator(nn.Module):
+    """
+    The abstract class for all attention layers.
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    @abstractmethod
+    def forward(
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        raise NotImplementedError
+
+
+class ScaledDotProductAttention(AttentionOperator):
     """Scaled dot-product attention.
 
     Parameters
     ----------
     temperature:
         The temperature for scaling.
 
@@ -40,23 +61,26 @@
 
     def forward(
         self,
         q: torch.Tensor,
         k: torch.Tensor,
         v: torch.Tensor,
         attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Forward processing of the scaled dot-product attention.
 
         Parameters
         ----------
         q:
             Query tensor.
+
         k:
             Key tensor.
+
         v:
             Value tensor.
 
         attn_mask:
             Masking tensor for the attention map. The shape should be [batch_size, n_heads, n_steps, n_steps].
             0 in attn_mask means values at the according position in the attention map will be masked out.
 
@@ -102,53 +126,47 @@
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
-    dropout:
-        The dropout rate.
-
-    attn_dropout:
-        The dropout rate for the attention map.
+    attention_operator:
+        The attention operator, e.g. the self-attention proposed in Transformer.
 
     """
 
     def __init__(
         self,
         n_heads: int,
         d_model: int,
         d_k: int,
         d_v: int,
-        dropout: float,
-        attn_dropout: float,
+        attention_operator: AttentionOperator,
     ):
         super().__init__()
 
         self.n_heads = n_heads
         self.d_k = d_k
         self.d_v = d_v
 
         self.w_qs = nn.Linear(d_model, n_heads * d_k, bias=False)
         self.w_ks = nn.Linear(d_model, n_heads * d_k, bias=False)
         self.w_vs = nn.Linear(d_model, n_heads * d_v, bias=False)
 
-        self.attention = ScaledDotProductAttention(d_k**0.5, attn_dropout)
+        self.attention_operator = attention_operator
         self.fc = nn.Linear(n_heads * d_v, d_model, bias=False)
 
-        self.dropout = nn.Dropout(dropout)
-        self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
-
     def forward(
         self,
         q: torch.Tensor,
         k: torch.Tensor,
         v: torch.Tensor,
         attn_mask: Optional[torch.Tensor],
+        **kwargs,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Forward processing of the multi-head attention module.
 
         Parameters
         ----------
         q:
             Query tensor.
@@ -173,36 +191,29 @@
 
         """
         # the input q, k, v currently have 3 dimensions [batch_size, n_steps, d_tensor]
         # d_tensor could be n_heads*d_k, n_heads*d_v
 
         # keep useful variables
         batch_size, n_steps = q.size(0), q.size(1)
-        residual = v
+        k_n_steps = k.size(1)
 
         # now separate the last dimension of q, k, v into different heads -> [batch_size, n_steps, n_heads, d_k or d_v]
         q = self.w_qs(q).view(batch_size, n_steps, self.n_heads, self.d_k)
-        k = self.w_ks(k).view(batch_size, n_steps, self.n_heads, self.d_k)
-        v = self.w_vs(v).view(batch_size, n_steps, self.n_heads, self.d_v)
+        k = self.w_ks(k).view(batch_size, k_n_steps, self.n_heads, self.d_k)
+        v = self.w_vs(v).view(batch_size, k_n_steps, self.n_heads, self.d_v)
 
         # transpose for self-attention calculation -> [batch_size, n_steps, d_k or d_v, n_heads]
         q, k, v = q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2)
 
         if attn_mask is not None:
             # broadcasting on the head axis
             attn_mask = attn_mask.unsqueeze(1)
 
-        v, attn_weights = self.attention(q, k, v, attn_mask)
+        v, attn_weights = self.attention_operator(q, k, v, attn_mask, **kwargs)
 
         # transpose back -> [batch_size, n_steps, n_heads, d_v]
         # then merge the last two dimensions to combine all the heads -> [batch_size, n_steps, n_heads*d_v]
         v = v.transpose(1, 2).contiguous().view(batch_size, n_steps, -1)
         v = self.fc(v)
 
-        # apply dropout and residual connection
-        v = self.dropout(v)
-        v += residual
-
-        # apply layer-norm
-        v = self.layer_norm(v)
-
         return v, attn_weights
```

### Comparing `pypots-0.3.2/pypots/nn/modules/transformer/auto_encoder.py` & `pypots-0.4/pypots/nn/modules/transformer/auto_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 # License: BSD-3-Clause
 
 from typing import Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
+from .attention import ScaledDotProductAttention
+from .embedding import PositionalEncoding
 from .layers import EncoderLayer, DecoderLayer
-from .pos_enc import PositionalEncoding
 
 
 class Encoder(nn.Module):
     """Transformer encoder.
 
     Parameters
     ----------
@@ -28,15 +29,15 @@
     n_features:
         The number of features in the input tensor.
 
     d_model:
         The dimension of the module manipulation space.
         The input tensor will be projected to a space with d_model dimensions.
 
-    d_inner:
+    d_ffn:
         The dimension of the hidden layer in the feed-forward network.
 
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
@@ -54,15 +55,15 @@
 
     def __init__(
         self,
         n_layers: int,
         n_steps: int,
         n_features: int,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
@@ -70,20 +71,20 @@
         self.embedding = nn.Linear(n_features, d_model)
         self.dropout = nn.Dropout(dropout)
         self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
         self.enc_layer_stack = nn.ModuleList(
             [
                 EncoderLayer(
                     d_model,
-                    d_inner,
+                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     dropout,
-                    attn_dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
     def forward(
         self,
@@ -141,15 +142,15 @@
     n_features:
         The number of features in the input tensor.
 
     d_model:
         The dimension of the module manipulation space.
         The input tensor will be projected to a space with d_model dimensions.
 
-    d_inner:
+    d_ffn:
         The dimension of the hidden layer in the feed-forward network.
 
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
@@ -167,35 +168,36 @@
 
     def __init__(
         self,
         n_layers: int,
         n_steps: int,
         n_features: int,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
         self.embedding = nn.Linear(n_features, d_model)
         self.dropout = nn.Dropout(dropout)
         self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
         self.layer_stack = nn.ModuleList(
             [
                 DecoderLayer(
                     d_model,
-                    d_inner,
+                    d_ffn,
                     n_heads,
                     d_k,
                     d_v,
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
+                    ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     dropout,
-                    attn_dropout,
                 )
                 for _ in range(n_layers)
             ]
         )
 
     def forward(
         self,
```

### Comparing `pypots-0.3.2/pypots/nn/modules/transformer/layers.py` & `pypots-0.4/pypots/nn/modules/transformer/layers.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from typing import Tuple, Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .attention import MultiHeadAttention
+from .attention import MultiHeadAttention, AttentionOperator
 
 
 class PositionWiseFeedForward(nn.Module):
     """Position-wise feed forward network (FFN) in Transformer.
 
     Parameters
     ----------
@@ -69,53 +69,55 @@
     """Transformer encoder layer.
 
     Parameters
     ----------
     d_model:
         The dimension of the input tensor.
 
-    d_inner:
+    d_ffn:
         The dimension of the hidden layer.
 
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
+    slf_attn_opt:
+        The attention operator for the self multi-head attention module in the encoder layer.
+
     dropout:
         The dropout rate.
 
-    attn_dropout:
-        The dropout rate for the attention map.
     """
 
     def __init__(
         self,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        slf_attn_opt: AttentionOperator,
         dropout: float = 0.1,
-        attn_dropout: float = 0.1,
     ):
         super().__init__()
-        self.slf_attn = MultiHeadAttention(
-            n_heads, d_model, d_k, d_v, dropout, attn_dropout
-        )
-        self.pos_ffn = PositionWiseFeedForward(d_model, d_inner, dropout)
+        self.slf_attn = MultiHeadAttention(n_heads, d_model, d_k, d_v, slf_attn_opt)
+        self.dropout = nn.Dropout(dropout)
+        self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        self.pos_ffn = PositionWiseFeedForward(d_model, d_ffn, dropout)
 
     def forward(
         self,
         enc_input: torch.Tensor,
         src_mask: Optional[torch.Tensor] = None,
+        **kwargs,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Forward processing of the encoder layer.
 
         Parameters
         ----------
         enc_input:
             Input tensor.
@@ -133,72 +135,82 @@
 
         """
         enc_output, attn_weights = self.slf_attn(
             enc_input,
             enc_input,
             enc_input,
             attn_mask=src_mask,
+            **kwargs,
         )
+
+        # apply dropout and residual connection
+        enc_output = self.dropout(enc_output)
+        enc_output += enc_input
+
+        # apply layer-norm
+        enc_output = self.layer_norm(enc_output)
+
         enc_output = self.pos_ffn(enc_output)
         return enc_output, attn_weights
 
 
 class DecoderLayer(nn.Module):
     """Transformer decoder layer.
 
     Parameters
     ----------
     d_model:
         The dimension of the input tensor.
 
-    d_inner:
+    d_ffn:
         The dimension of the hidden layer.
 
     n_heads:
         The number of heads in multi-head attention.
 
     d_k:
         The dimension of the key and query tensor.
 
     d_v:
         The dimension of the value tensor.
 
+    slf_attn_opt:
+        The attention operator for the self multi-head attention module in the decoder layer.
+
+    enc_attn_opt:
+        The attention operator for the encoding multi-head attention module in the decoder layer.
+
     dropout:
         The dropout rate.
 
-    attn_dropout:
-        The dropout rate for the attention map.
-
     """
 
     def __init__(
         self,
         d_model: int,
-        d_inner: int,
+        d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
+        slf_attn_opt: AttentionOperator,
+        enc_attn_opt: AttentionOperator,
         dropout: float = 0.1,
-        attn_dropout: float = 0.1,
     ):
         super().__init__()
-        self.slf_attn = MultiHeadAttention(
-            n_heads, d_model, d_k, d_v, dropout, attn_dropout
-        )
-        self.enc_attn = MultiHeadAttention(
-            n_heads, d_model, d_k, d_v, dropout, attn_dropout
-        )
-        self.pos_ffn = PositionWiseFeedForward(d_model, d_inner, dropout)
+        self.slf_attn = MultiHeadAttention(n_heads, d_model, d_k, d_v, slf_attn_opt)
+        self.enc_attn = MultiHeadAttention(n_heads, d_model, d_k, d_v, enc_attn_opt)
+        self.pos_ffn = PositionWiseFeedForward(d_model, d_ffn, dropout)
 
     def forward(
         self,
         dec_input: torch.Tensor,
         enc_output: torch.Tensor,
         slf_attn_mask: Optional[torch.Tensor] = None,
         dec_enc_attn_mask: Optional[torch.Tensor] = None,
+        **kwargs,
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """Forward processing of the decoder layer.
 
         Parameters
         ----------
         dec_input:
             Input tensor.
@@ -223,14 +235,22 @@
             The self-attention map.
 
         dec_enc_attn:
             The encoding attention map.
 
         """
         dec_output, dec_slf_attn = self.slf_attn(
-            dec_input, dec_input, dec_input, attn_mask=slf_attn_mask
+            dec_input,
+            dec_input,
+            dec_input,
+            attn_mask=slf_attn_mask,
+            **kwargs,
         )
         dec_output, dec_enc_attn = self.enc_attn(
-            dec_output, enc_output, enc_output, attn_mask=dec_enc_attn_mask
+            dec_output,
+            enc_output,
+            enc_output,
+            attn_mask=dec_enc_attn_mask,
+            **kwargs,
         )
         dec_output = self.pos_ffn(dec_output)
         return dec_output, dec_slf_attn, dec_enc_attn
```

### Comparing `pypots-0.3.2/pypots/optim/adadelta.py` & `pypots-0.4/pypots/optim/adadelta.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/adagrad.py` & `pypots-0.4/pypots/optim/adagrad.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/adam.py` & `pypots-0.4/pypots/optim/adam.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/adamw.py` & `pypots-0.4/pypots/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/base.py` & `pypots-0.4/pypots/optim/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/__init__.py` & `pypots-0.4/pypots/optim/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/base.py` & `pypots-0.4/pypots/optim/lr_scheduler/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/constant_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/constant_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/exponential_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/exponential_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/lambda_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/lambda_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/linear_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/linear_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/multiplicative_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/multiplicative_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/multistep_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/multistep_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/lr_scheduler/step_lrs.py` & `pypots-0.4/pypots/optim/lr_scheduler/step_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/rmsprop.py` & `pypots-0.4/pypots/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/optim/sgd.py` & `pypots-0.4/pypots/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/file.py` & `pypots-0.4/pypots/utils/file.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/metrics/__init__.py` & `pypots-0.4/pypots/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/metrics/classification.py` & `pypots-0.4/pypots/utils/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/metrics/clustering.py` & `pypots-0.4/pypots/utils/metrics/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/metrics/error.py` & `pypots-0.4/pypots/utils/metrics/error.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/random.py` & `pypots-0.4/pypots/utils/random.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/visual/clustering.py` & `pypots-0.4/pypots/utils/visual/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots/utils/visual/data.py` & `pypots-0.4/pypots/utils/visual/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.3.2/pypots.egg-info/PKG-INFO` & `pypots-0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,7 @@
-Metadata-Version: 2.1
-Name: pypots
-Version: 0.3.2
-Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
-Home-page: https://pypots.com/
-Author: Wenjie Du
-Author-email: wenjay.du@gmail.com
-License: BSD-3-Clause
-Project-URL: Documentation, https://docs.pypots.com/
-Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
-Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
-Project-URL: Download, https://github.com/WenjieDu/PyPOTS/archive/main.zip
-Keywords: data science,data mining,neural networks,machine learning,deep learning,artificial intelligence,time-series analysis,time series,imputation,interpolation,classification,clustering,forecasting,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: basic
-Provides-Extra: optional
-Provides-Extra: full
-Provides-Extra: test
-Provides-Extra: doc
-Provides-Extra: dev
-License-File: LICENSE
-
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img src="https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg" width="200" align="right">
 </a>
 
 <h3 align="center">Welcome to PyPOTS</h3>
 
 <p align="center"><i>a Python toolbox for machine learning on Partially-Observed Time Series</i></p>
@@ -166,28 +128,28 @@
 PyPOTS is available on both [PyPI](https://pypi.python.org/pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots).
 You can install PyPOTS as shown below:
 
 ``` bash
 # via pip
 pip install pypots            # the first time installation
 pip install pypots --upgrade  # update pypots to the latest version
+# install from the latest source code with the latest features but may be not officially released yet
+pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
 
 # via conda
 conda install -c conda-forge pypots  # the first time installation
 conda update  -c conda-forge pypots  # update pypots to the latest version
-````
-
-Alternatively, you can install from the latest source code with the latest features but may be not officially released yet:
-> pip install https://github.com/WenjieDu/PyPOTS/archive/main.zip
+```
 
 
 ## ❖ Usage
-Besides [BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial notebook
-on Google Colab <a href="https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ"><img src="https://img.shields.io/badge/GoogleColab-PyPOTS_Tutorials-F9AB00?logo=googlecolab&logoColor=white" alt="Colab tutorials" align="center"/></a>.
-If you have further questions, please refer to PyPOTS documentation [docs.pypots.com](https://docs.pypots.com).
+Besides [BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial notebook on Google Colab
+<a href="https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ">
+<img src="https://img.shields.io/badge/GoogleColab-PyPOTS_Tutorials-F9AB00?logo=googlecolab&logoColor=white" alt="Colab tutorials" align="center"/>
+</a>. If you have further questions, please refer to PyPOTS documentation [docs.pypots.com](https://docs.pypots.com).
 You can also [raise an issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-community).
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details open>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
 
@@ -208,15 +170,15 @@
 X = X.reshape(num_samples, 48, -1)
 X_ori = X  # keep X_ori for validation
 X = mcar(X, 0.1)  # randomly hold out 10% observed values as ground truth
 dataset = {"X": X}  # X for model input
 print(X.shape)  # (11988, 48, 37), 11988 samples and each sample has 48 time steps, 37 features
 
 # Model training. This is PyPOTS showtime.
-saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4, d_k=64, d_v=64, dropout=0.1, epochs=10)
 # Here I use the whole dataset as the training set because ground truth is not visible to the model, you can also split it into train/val/test sets
 saits.fit(dataset)
 imputation = saits.impute(dataset)  # impute the originally-missing values and artificially-missing values
 indicating_mask = np.isnan(X) ^ np.isnan(X_ori)  # indicating mask for imputation error calculation
 mae = calc_mae(imputation, np.nan_to_num(X_ori), indicating_mask)  # calculate mean absolute error on the ground truth (artificially-missing values)
 ```
 </details>
@@ -226,38 +188,50 @@
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
 The currently available algorithms of four tasks are cataloged in the following table with four partitions.
 The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
 
-|   ***`Imputation`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|:----------------------:|:-----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**  |                                                                       **Full name of the algorithm/model**                                                                        | **Year** |
-|       Neural Net       |    SAITS    |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
-|       Neural Net       | Transformer | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
-|       Neural Net       |  TimesNet   |                                                       Temporal 2D-Variation Modeling for General Time Series Analysis [^14]                                                       |   2023   |
-|       Neural Net       |    CSDI     |                                              Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]                                              |   2021   |
-|       Neural Net       |   US-GAN    |                                                          Unsupervised GAN for Multivariate Time Series Imputation [^10]                                                           |   2021   |
-|       Neural Net       |   GP-VAE    |                                                                  Gaussian Process Variational Autoencoder [^11]                                                                   |   2020   |
-|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    M-RNN    |                                                                  Multi-directional Recurrent Neural Network [^9]                                                                  |   2019   |
-|         Naive          |    LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
-| ***`Classification`*** |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    GRU-D    |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
-|       Neural Net       |  Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
-|   ***`Clustering`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
-|       Neural Net       |    VaDER    |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
-|  ***`Forecasting`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|     Probabilistic      |    BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
+🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
+and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+
+|   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
+|:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
+|        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
+|       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
+|       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
+|       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
+|       Neural Net       |  TimesNet   |              Temporal 2D-Variation Modeling for General Time Series Analysis [^14]              |   2023   |
+|       Neural Net       |  PatchTST   |         A Time Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18]          |   2023   |
+|       Neural Net       |   DLinear   |                  Are Transformers Effective for Time Series Forecasting? [^17]                  |   2023   |
+|       Neural Net       |  ETSformer  |              Exponential Smoothing Transformers for Time-series Forecasting [^19]               |   2023   |
+|       Neural Net       |  FEDformer  |        Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting [^20]         |   2022   |
+|       Neural Net       |  Informer   |          Beyond Efficient Transformer for Long Sequence Time-Series Forecasting [^21]           |   2021   |
+|       Neural Net       | Autoformer  |     Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting [^15]     |   2021   |
+|       Neural Net       |    CSDI     |     Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation [^12]     |   2021   |
+|       Neural Net       |   US-GAN    |                 Unsupervised GAN for Multivariate Time Series Imputation [^10]                  |   2021   |
+|       Neural Net       |   GP-VAE    |                         Gaussian Process Variational Autoencoder [^11]                          |   2020   |
+|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
+|       Neural Net       |    M-RNN    |                         Multi-directional Recurrent Neural Network [^9]                         |   2019   |
+|         Naive          |  LOCF/NOCB  |              Last Observation Carried Forward / Next Observation Carried Backward               |    -     |
+|         Naive          |   Median    |                                     Median Value Imputation                                     |    -     |
+|         Naive          |    Mean     |                                      Mean Value Imputation                                      |    -     |
+| ***`Classification`*** |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|       Neural Net       |    BRITS    |                     Bidirectional Recurrent Imputation for Time Series [^3]                     |   2018   |
+|       Neural Net       |    GRU-D    |         Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]         |   2018   |
+|       Neural Net       |  Raindrop   |           Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]            |   2022   |
+|   ***`Clustering`***   |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|       Neural Net       |    CRLI     |             Clustering Representation Learning on Incomplete time-series data [^6]              |   2021   |
+|       Neural Net       |    VaDER    |                         Variational Deep Embedding with Recurrence [^7]                         |   2019   |
+|  ***`Forecasting`***   |     🚥      |                                               🚥                                                |    🚥    |
+|        **Type**        |  **Abbr.**  |                           **Full name of the algorithm/model/paper**                            | **Year** |
+|     Probabilistic      |    BTTF     |                           Bayesian Temporal Tensor Factorization [^8]                           |   2021   |
 
 
 ## ❖ Citing PyPOTS
 > [!TIP]
 > **[Updates in Feb 2024]** 😎 Our survey paper [Deep Learning for Multivariate Time Series Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on arXiv.
 The code is open source in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/Awesome_Imputation).
 We comprehensively review the literature of the state-of-the-art deep-learning imputation methods for time series,
@@ -283,15 +257,15 @@
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
 doi={10.48550/arXiv.2305.18811},
 }
 ```
-
+or
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
 
 ## ❖ Contribution
 You're very welcome to contribute to this exciting project!
@@ -352,14 +326,22 @@
 [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal Factorization for Multidimensional Time Series Prediction](https://arxiv.org/abs/1910.06366). *IEEE transactions on pattern analysis and machine intelligence*.
 [^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019). [Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE Transactions on Biomedical Engineering*.
 [^10]: Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021). [Generative Semi-supervised Learning for Multivariate Time Series Imputation](https://ojs.aaai.org/index.php/AAAI/article/view/17086). *AAAI 2021*.
 [^11]: Fortuin, V., Baranchuk, D., Raetsch, G. & Mandt, S. (2020). [GP-VAE: Deep Probabilistic Time Series Imputation](https://proceedings.mlr.press/v108/fortuin20a.html). *AISTATS 2020*.
 [^12]: Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021). [CSDI: Conditional Score-based Diffusion Models for Probabilistic Time Series Imputation](https://proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-Abstract.html). *NeurIPS 2021*.
 [^13]: Rubin, D. B. (1976). [Inference and missing data](https://academic.oup.com/biomet/article-abstract/63/3/581/270932). *Biometrika*.
 [^14]: Wu, H., Hu, T., Liu, Y., Zhou, H., Wang, J., & Long, M. (2023). [TimesNet: Temporal 2d-variation modeling for general time series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023*
+[^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition transformers with auto-correlation for long-term series forecasting](https://proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-Abstract.html). *NeurIPS 2021*.
+[^16]: Zhang, Y., & Yan, J. (2023). [Crossformer: Transformer utilizing cross-dimension dependency for multivariate time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR 2023*.
+[^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317). *AAAI 2023*
+[^18]: Nie, Y., Nguyen, N. H., Sinthong, P., & Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
+[^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer: Exponential Smoothing Transformers for Time-series Forecasting](https://openreview.net/forum?id=5m_3whfo483).  *ICLR 2023*
+[^20]: Zhou, T., Ma, Z., Wen, Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting](https://proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*.
+[^21]: Zhou, H., Zhang, S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer: Beyond efficient transformer for long sequence time-series forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*.
+
 
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits%20since%20May%202022&edge_flat=false">
 </a>
```

#### html2text {}

```diff
@@ -1,33 +1,8 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.3.2 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
-Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
-Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
-https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
-WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
-PyPOTS/archive/main.zip Keywords: data science,data mining,neural
-networks,machine learning,deep learning,artificial intelligence,time-series
-analysis,time
-series,imputation,interpolation,classification,clustering,forecasting,partially
-observed,irregular sampled,partially-observed time series,incomplete time
-series,missing data,missing values Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: Intended Audience :: Healthcare Industry Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development :: Libraries ::
-Application Frameworks Requires-Python: >=3.7.0 Description-Content-Type: text/
-markdown Provides-Extra: basic Provides-Extra: optional Provides-Extra: full
-Provides-Extra: test Provides-Extra: doc Provides-Extra: dev License-File:
-LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]
                           ******** WWeellccoommee ttoo PPyyPPOOTTSS ********
     a Python toolbox for machine learning on Partially-Observed Time Series
 _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_p_o_w_e_r_e_d_ _b_y_ _P_y_t_o_r_c_h_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]
   _[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e
   _C_l_i_m_a_t_e_ _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _c_o_v_e_r_a_g_e_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_D_o_c_s_ _b_u_i_l_d_i_n_g_]
                  _[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]_[_a_r_X_i_v_ _D_O_I_]
 â¦¿ `Motivation`: Due to all kinds of reasons like failure of collection
@@ -79,39 +54,39 @@
        ?â???ï?¸? WWeellccoommee ttoo tthhee uunniivveerrssee ooff PPyyPPOOTTSS.. EEnnjjooyy iitt aanndd hhaavvee ffuunn!!
 ## â Installation You can refer to [the installation instruction](https://
 docs.pypots.com/en/latest/install.html) in PyPOTS documentation for a guideline
 with more details. PyPOTS is available on both [PyPI](https://pypi.python.org/
 pypi/pypots) and [Anaconda](https://anaconda.org/conda-forge/pypots). You can
 install PyPOTS as shown below: ``` bash # via pip pip install pypots # the
 first time installation pip install pypots --upgrade # update pypots to the
-latest version # via conda conda install -c conda-forge pypots # the first time
-installation conda update -c conda-forge pypots # update pypots to the latest
-version ```` Alternatively, you can install from the latest source code with
-the latest features but may be not officially released yet: > pip install
-https://github.com/WenjieDu/PyPOTS/archive/main.zip ## â Usage Besides
-[BrewPOTS](https://github.com/WenjieDu/BrewPOTS), you can also find a simple
-and quick-start tutorial notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you
-have further questions, please refer to PyPOTS documentation [docs.pypots.com]
-(https://docs.pypots.com). You can also [raise an issue](https://github.com/
-WenjieDu/PyPOTS/issues) or [ask in our community](#-community). We present you
-a usage example of imputing missing values in time series with PyPOTS below,
-you can click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn
-PPhhyyssiiooNNeett22001122 ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from
-sklearn.preprocessing import StandardScaler from pygrinder import mcar from
-pypots.data import load_specific_dataset from pypots.imputation import SAITS
-from pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but
-PyPOTS can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
+latest version # install from the latest source code with the latest features
+but may be not officially released yet pip install https://github.com/WenjieDu/
+PyPOTS/archive/main.zip # via conda conda install -c conda-forge pypots # the
+first time installation conda update -c conda-forge pypots # update pypots to
+the latest version ``` ## â Usage Besides [BrewPOTS](https://github.com/
+WenjieDu/BrewPOTS), you can also find a simple and quick-start tutorial
+notebook on Google Colab _[_C_o_l_a_b_ _t_u_t_o_r_i_a_l_s_]. If you have further questions,
+please refer to PyPOTS documentation [docs.pypots.com](https://
+docs.pypots.com). You can also [raise an issue](https://github.com/WenjieDu/
+PyPOTS/issues) or [ask in our community](#-community). We present you a usage
+example of imputing missing values in time series with PyPOTS below, you can
+click it to view. CClliicckk hheerree ttoo sseeee aann eexxaammppllee aappppllyyiinngg SSAAIITTSS oonn PPhhyyssiiooNNeett22001122
+ffoorr iimmppuuttaattiioonn:: ``` python import numpy as np from sklearn.preprocessing import
+StandardScaler from pygrinder import mcar from pypots.data import
+load_specific_dataset from pypots.imputation import SAITS from
+pypots.utils.metrics import calc_mae # Data preprocessing. Tedious, but PyPOTS
+can help. data = load_specific_dataset('physionet_2012') # PyPOTS will
 automatically download and extract it. X = data['X'] num_samples = len(X
 ['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
 StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
 X_ori = X # keep X_ori for validation X = mcar(X, 0.1) # randomly hold out 10%
 observed values as ground truth dataset = {"X": X} # X for model input print
 (X.shape) # (11988, 48, 37), 11988 samples and each sample has 48 time steps,
 37 features # Model training. This is PyPOTS showtime. saits = SAITS
-(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128, n_heads=4,
+(n_steps=48, n_features=37, n_layers=2, d_model=256, d_ffn=128, n_heads=4,
 d_k=64, d_v=64, dropout=0.1, epochs=10) # Here I use the whole dataset as the
 training set because ground truth is not visible to the model, you can also
 split it into train/val/test sets saits.fit(dataset) imputation = saits.impute
 (dataset) # impute the originally-missing values and artificially-missing
 values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
 imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
 indicating_mask) # calculate mean absolute error on the ground truth
@@ -119,68 +94,81 @@
 imputation, classification, clustering, and forecasting tasks on multivariate
 time series with missing values. The currently available algorithms of four
 tasks are cataloged in the following table with four partitions. The paper
 references are all listed at the bottom of this readme file. Please refer to
 them if you want more details. ð Since **v0.2**, all neural-network models
 in PyPOTS has got hyperparameter-optimization support. This functionality is
 implemented with the [Microsoft NNI](https://github.com/microsoft/nni)
-framework. | ***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:---------------------
--:|:-----------:|:-------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------:|:--------:| | **Type** | **Abbr.** |
-**Full name of the algorithm/model** | **Year** | | Neural Net | SAITS | Self-
-Attention-based Imputation for Time Series [^1] | 2023 | | Neural Net |
-Transformer | Attention is All you Need [^2];
-Self-Attention-based Imputation for Time Series [^1];
-Note: proposed in [^2], and re-implemented as an imputation model in [^1]. |
-2017 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for General
-Time Series Analysis [^14] | 2023 | | Neural Net | CSDI | Conditional Score-
+framework. ð¥ Note that Transformer, Crossformer, PatchTST, DLinear,
+ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation
+methods in their original papers, and they cannot accept POTS as input. **To
+make them applicable on POTS data, we apply the embedding strategy the same as
+we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).** |
+***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:----------------------:|:----------
+-:|:---------------------------------------------------------------------------
+--------------------:|:--------:| | **Type** | **Abbr.** | **Full name of the
+algorithm/model** | **Year** | | Neural Net | SAITS | Self-Attention-based
+Imputation for Time Series [^1] | 2023 | | Neural Net | Transformer | Attention
+is All you Need [^2] | 2017 | | Neural Net | Crossformer | Transformer
+Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting
+[^16] | 2023 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for
+General Time Series Analysis [^14] | 2023 | | Neural Net | PatchTST | A Time
+Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18] | 2023
+| | Neural Net | DLinear | Are Transformers Effective for Time Series
+Forecasting? [^17] | 2023 | | Neural Net | ETSformer | Exponential Smoothing
+Transformers for Time-series Forecasting [^19] | 2023 | | Neural Net |
+FEDformer | Frequency Enhanced Decomposed Transformer for Long-term Series
+Forecasting [^20] | 2022 | | Neural Net | Informer | Beyond Efficient
+Transformer for Long Sequence Time-Series Forecasting [^21] | 2021 | | Neural
+Net | Autoformer | Decomposition Transformers with Auto-Correlation for Long-
+Term Series Forecasting [^15] | 2021 | | Neural Net | CSDI | Conditional Score-
 based Diffusion Models for Probabilistic Time Series Imputation [^12] | 2021 |
 | Neural Net | US-GAN | Unsupervised GAN for Multivariate Time Series
 Imputation [^10] | 2021 | | Neural Net | GP-VAE | Gaussian Process Variational
 Autoencoder [^11] | 2020 | | Neural Net | BRITS | Bidirectional Recurrent
 Imputation for Time Series [^3] | 2018 | | Neural Net | M-RNN | Multi-
-directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF | Last
-Observation Carried Forward | - | | ***`Classification`*** | ð¥ | ð¥ | ð¥
-| | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
-**Year** | | Neural Net | BRITS | Bidirectional Recurrent Imputation for Time
-Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent Neural Networks for
-Multivariate Time Series with Missing Values [^4] | 2018 | | Neural Net |
-Raindrop | Graph-Guided Network for Irregularly Sampled Multivariate Time
-Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ | ð¥ | | **Type** |
-**Abbr.** | **Full name of the algorithm/model/paper** | **Year** | | Neural
-Net | CRLI | Clustering Representation Learning on Incomplete time-series data
-[^6] | 2021 | | Neural Net | VaDER | Variational Deep Embedding with Recurrence
-[^7] | 2019 | | ***`Forecasting`*** | ð¥ | ð¥ | ð¥ | | **Type** |
-**Abbr.** | **Full name of the algorithm/model/paper** | **Year** | |
-Probabilistic | BTTF | Bayesian Temporal Tensor Factorization [^8] | 2021 | ##
-â Citing PyPOTS > [!TIP] > **[Updates in Feb 2024]** ð Our survey paper
-[Deep Learning for Multivariate Time Series Imputation: A Survey](https://
-arxiv.org/abs/2402.04059) has been released on arXiv. The code is open source
-in the GitHub repo [Awesome_Imputation](https://github.com/WenjieDu/
-Awesome_Imputation). We comprehensively review the literature of the state-of-
-the-art deep-learning imputation methods for time series, provide a taxonomy
-for them, and discuss the challenges and future directions in this field. > >
-**[Updates in Jun 2023]** ð A short version of the PyPOTS paper is accepted
-by the 9th SIGKDD international workshop on Mining and Learning from Time
-Series ([MiLeTS'23](https://kdd-milets.github.io/milets2023/))).
-**Additionally**, PyPOTS has been included as a [PyTorch Ecosystem](https://
-pytorch.org/ecosystem/) project. The paper introducing PyPOTS is available on
-arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing to
-publish it in prestigious academic venues, e.g. JMLR (track for [Machine
-Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use PyPOTS
-in your work, please cite it as below and ðstar this repository to make
-others notice this library. ð¤ There are scientific research projects using
-PyPOTS and referencing in their papers. Here is [an incomplete list of them]
-(https://scholar.google.com/
+directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF/NOCB | Last
+Observation Carried Forward / Next Observation Carried Backward | - | | Naive |
+Median | Median Value Imputation | - | | Naive | Mean | Mean Value Imputation |
+- | | ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** |
+**Full name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
+Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
+GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
+Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
+Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
+| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Neural Net | CRLI | Clustering Representation
+Learning on Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER |
+Variational Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`***
+| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
+Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
+2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
+Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
+arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
+github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
+literature of the state-of-the-art deep-learning imputation methods for time
+series, provide a taxonomy for them, and discuss the challenges and future
+directions in this field. > > **[Updates in Jun 2023]** ð A short version of
+the PyPOTS paper is accepted by the 9th SIGKDD international workshop on Mining
+and Learning from Time Series ([MiLeTS'23](https://kdd-milets.github.io/
+milets2023/))). **Additionally**, PyPOTS has been included as a [PyTorch
+Ecosystem](https://pytorch.org/ecosystem/) project. The paper introducing
+PyPOTS is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
+and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
+(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
+)). If you use PyPOTS in your work, please cite it as below and ðstar this
+repository to make others notice this library. ð¤ There are scientific
+research projects using PyPOTS and referencing in their papers. Here is [an
+incomplete list of them](https://scholar.google.com/
 scholar?as_ylo=2022&q=%E2%80%9CPyPOTS%E2%80%9D&hl=en>). ``` bibtex @article
 {du2023pypots, title={{PyPOTS: a Python toolbox for data mining on Partially-
 Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
 archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
-2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du. (2023). >
+2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
 PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series. >
 arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ## â Contribution
 You're very welcome to contribute to this exciting project! By committing your
 code, you'll 1. make your well-established model out-of-the-box for PyPOTS
 users to run, and help your work obtain more exposure and impact. Take a look
 at our [inclusion criteria](https://docs.pypots.com/en/latest/
 faq.html#inclusion-criteria). You can utilize the `template` folder in each
@@ -243,9 +231,29 @@
 Tashiro, Y., Song, J., Song, Y., & Ermon, S. (2021). [CSDI: Conditional Score-
 based Diffusion Models for Probabilistic Time Series Imputation](https://
 proceedings.neurips.cc/paper/2021/hash/cfe8504bda37b575c70ee1a8276f3486-
 Abstract.html). *NeurIPS 2021*. [^13]: Rubin, D. B. (1976). [Inference and
 missing data](https://academic.oup.com/biomet/article-abstract/63/3/581/
 270932). *Biometrika*. [^14]: Wu, H., Hu, T., Liu, Y., Zhou, H., Wang, J., &
 Long, M. (2023). [TimesNet: Temporal 2d-variation modeling for general time
-series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023* ð 
-Visits_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
+series analysis](https://openreview.net/forum?id=ju_Uqw384Oq). *ICLR 2023*
+[^15]: Wu, H., Xu, J., Wang, J., & Long, M. (2021). [Autoformer: Decomposition
+transformers with auto-correlation for long-term series forecasting](https://
+proceedings.neurips.cc/paper/2021/hash/bcc0d400288793e8bdcd7c19a8ac0c2b-
+Abstract.html). *NeurIPS 2021*. [^16]: Zhang, Y., & Yan, J. (2023).
+[Crossformer: Transformer utilizing cross-dimension dependency for multivariate
+time series forecasting](https://openreview.net/forum?id=vSVLM2j9eie). *ICLR
+2023*. [^17]: Zeng, A., Chen, M., Zhang, L., & Xu, Q. (2023). [Are transformers
+effective for time series forecasting?](https://ojs.aaai.org/index.php/AAAI/
+article/view/26317). *AAAI 2023* [^18]: Nie, Y., Nguyen, N. H., Sinthong, P., &
+Kalagnanam, J. (2023). [A time series is worth 64 words: Long-term forecasting
+with transformers](https://openreview.net/forum?id=Jbdc0vTOcol). *ICLR 2023*
+[^19]: Woo, G., Liu, C., Sahoo, D., Kumar, A., & Hoi, S. (2023). [ETSformer:
+Exponential Smoothing Transformers for Time-series Forecasting](https://
+openreview.net/forum?id=5m_3whfo483). *ICLR 2023* [^20]: Zhou, T., Ma, Z., Wen,
+Q., Wang, X., Sun, L., & Jin, R. (2022). [FEDformer: Frequency enhanced
+decomposed transformer for long-term series forecasting](https://
+proceedings.mlr.press/v162/zhou22g.html). *ICML 2022*. [^21]: Zhou, H., Zhang,
+S., Peng, J., Zhang, S., Li, J., Xiong, H., & Zhang, W. (2021). [Informer:
+Beyond efficient transformer for long sequence time-series forecasting](https:/
+/ojs.aaai.org/index.php/AAAI/article/view/17325). *AAAI 2021*. ð  Visits
+_[_P_y_P_O_T_S_ _v_i_s_i_t_s_]
```

### Comparing `pypots-0.3.2/pypots.egg-info/SOURCES.txt` & `pypots-0.4/pypots.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -66,80 +66,119 @@
 pypots/forecasting/bttf/__init__.py
 pypots/forecasting/bttf/model.py
 pypots/forecasting/bttf/modules/__init__.py
 pypots/forecasting/bttf/modules/core.py
 pypots/forecasting/bttf/modules/submodules.py
 pypots/imputation/__init__.py
 pypots/imputation/base.py
+pypots/imputation/autoformer/__init__.py
+pypots/imputation/autoformer/data.py
+pypots/imputation/autoformer/model.py
+pypots/imputation/autoformer/modules/__init__.py
+pypots/imputation/autoformer/modules/core.py
+pypots/imputation/autoformer/modules/submodules.py
 pypots/imputation/brits/__init__.py
 pypots/imputation/brits/data.py
 pypots/imputation/brits/model.py
 pypots/imputation/brits/modules/__init__.py
 pypots/imputation/brits/modules/core.py
 pypots/imputation/brits/modules/submodules.py
+pypots/imputation/crossformer/__init__.py
+pypots/imputation/crossformer/data.py
+pypots/imputation/crossformer/model.py
+pypots/imputation/crossformer/modules/__init__.py
+pypots/imputation/crossformer/modules/core.py
+pypots/imputation/crossformer/modules/submodules.py
 pypots/imputation/csdi/__init__.py
 pypots/imputation/csdi/data.py
 pypots/imputation/csdi/model.py
 pypots/imputation/csdi/modules/__init__.py
 pypots/imputation/csdi/modules/core.py
 pypots/imputation/csdi/modules/submodules.py
+pypots/imputation/dlinear/__init__.py
+pypots/imputation/dlinear/data.py
+pypots/imputation/dlinear/model.py
+pypots/imputation/dlinear/modules/__init__.py
+pypots/imputation/dlinear/modules/core.py
+pypots/imputation/etsformer/__init__.py
+pypots/imputation/etsformer/data.py
+pypots/imputation/etsformer/model.py
+pypots/imputation/etsformer/modules/__init__.py
+pypots/imputation/etsformer/modules/core.py
+pypots/imputation/etsformer/modules/submodules.py
+pypots/imputation/fedformer/__init__.py
+pypots/imputation/fedformer/data.py
+pypots/imputation/fedformer/model.py
+pypots/imputation/fedformer/modules/__init__.py
+pypots/imputation/fedformer/modules/core.py
+pypots/imputation/fedformer/modules/submodules.py
 pypots/imputation/gpvae/__init__.py
 pypots/imputation/gpvae/data.py
 pypots/imputation/gpvae/model.py
 pypots/imputation/gpvae/modules/__init__.py
 pypots/imputation/gpvae/modules/core.py
 pypots/imputation/gpvae/modules/submodules.py
+pypots/imputation/informer/__init__.py
+pypots/imputation/informer/data.py
+pypots/imputation/informer/model.py
+pypots/imputation/informer/modules/__init__.py
+pypots/imputation/informer/modules/core.py
+pypots/imputation/informer/modules/submodules.py
 pypots/imputation/locf/__init__.py
 pypots/imputation/locf/model.py
 pypots/imputation/locf/modules/__init__.py
 pypots/imputation/locf/modules/core.py
 pypots/imputation/mean/__init__.py
 pypots/imputation/mean/model.py
 pypots/imputation/median/__init__.py
 pypots/imputation/median/model.py
 pypots/imputation/mrnn/__init__.py
 pypots/imputation/mrnn/data.py
 pypots/imputation/mrnn/model.py
 pypots/imputation/mrnn/modules/__init__.py
 pypots/imputation/mrnn/modules/core.py
 pypots/imputation/mrnn/modules/submodules.py
+pypots/imputation/patchtst/__init__.py
+pypots/imputation/patchtst/data.py
+pypots/imputation/patchtst/model.py
+pypots/imputation/patchtst/modules/__init__.py
+pypots/imputation/patchtst/modules/core.py
+pypots/imputation/patchtst/modules/submodules.py
 pypots/imputation/saits/__init__.py
 pypots/imputation/saits/data.py
 pypots/imputation/saits/model.py
 pypots/imputation/saits/modules/__init__.py
 pypots/imputation/saits/modules/core.py
 pypots/imputation/timesnet/__init__.py
 pypots/imputation/timesnet/data.py
 pypots/imputation/timesnet/model.py
 pypots/imputation/timesnet/modules/__init__.py
 pypots/imputation/timesnet/modules/core.py
-pypots/imputation/timesnet/modules/embedding.py
-pypots/imputation/timesnet/modules/layer.py
+pypots/imputation/timesnet/modules/submodules.py
 pypots/imputation/transformer/__init__.py
 pypots/imputation/transformer/data.py
 pypots/imputation/transformer/model.py
 pypots/imputation/transformer/modules/__init__.py
 pypots/imputation/transformer/modules/core.py
 pypots/imputation/usgan/__init__.py
 pypots/imputation/usgan/data.py
 pypots/imputation/usgan/model.py
 pypots/imputation/usgan/modules/__init__.py
 pypots/imputation/usgan/modules/core.py
 pypots/imputation/usgan/modules/submodules.py
-pypots/modules/__init__.py
 pypots/nn/__init__.py
 pypots/nn/functional/__init__.py
 pypots/nn/functional/normalization.py
 pypots/nn/modules/__init__.py
 pypots/nn/modules/rnn.py
 pypots/nn/modules/transformer/__init__.py
 pypots/nn/modules/transformer/attention.py
 pypots/nn/modules/transformer/auto_encoder.py
+pypots/nn/modules/transformer/embedding.py
 pypots/nn/modules/transformer/layers.py
-pypots/nn/modules/transformer/pos_enc.py
 pypots/optim/__init__.py
 pypots/optim/adadelta.py
 pypots/optim/adagrad.py
 pypots/optim/adam.py
 pypots/optim/adamw.py
 pypots/optim/base.py
 pypots/optim/rmsprop.py
```

### Comparing `pypots-0.3.2/pypots.egg-info/requires.txt` & `pypots-0.4/pypots.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 h5py
 numpy
 scipy
+sympy
+einops
 pandas
 matplotlib
 tensorboard
 scikit-learn
 torch>=1.10.0
 tsdb>=0.2
 pygrinder>=0.4
 
 [basic]
+h5py
 numpy
-scikit-learn
+scipy
+sympy
+einops
+pandas
 matplotlib
-pandas<2.0.0
-torch>=1.10.0
 tensorboard
-scipy
-h5py
+scikit-learn
+torch>=1.10.0
 tsdb>=0.2
 pygrinder>=0.4
 
 [dev]
 black
 flake8
 pre-commit
 jupyterlab
+h5py
 numpy
-scikit-learn
+scipy
+sympy
+einops
+pandas
 matplotlib
-pandas<2.0.0
-torch>=1.10.0
 tensorboard
-scipy
-h5py
+scikit-learn
+torch>=1.10.0
 tsdb>=0.2
 pygrinder>=0.4
 torch-geometric
 torch-scatter
 torch-sparse
 nni
 pytest-xdist
@@ -52,22 +58,24 @@
 furo
 sphinx
 sphinxcontrib-bibtex
 sphinxcontrib-gtagjs
 sphinx-autodoc-typehints
 
 [full]
+h5py
 numpy
-scikit-learn
+scipy
+sympy
+einops
+pandas
 matplotlib
-pandas<2.0.0
-torch>=1.10.0
 tensorboard
-scipy
-h5py
+scikit-learn
+torch>=1.10.0
 tsdb>=0.2
 pygrinder>=0.4
 torch-geometric
 torch-scatter
 torch-sparse
 nni
```

### Comparing `pypots-0.3.2/setup.py` & `pypots-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     ],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
         "h5py",
         "numpy",
         "scipy",
+        "sympy",
+        "einops",
         "pandas",
         "matplotlib",
         "tensorboard",
         "scikit-learn",
         "torch>=1.10.0",
         "tsdb>=0.2",
         "pygrinder>=0.4",
```

