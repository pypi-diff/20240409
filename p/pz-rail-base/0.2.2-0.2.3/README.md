# Comparing `tmp/pz-rail-base-0.2.2.tar.gz` & `tmp/pz-rail-base-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.2.2.tar", last modified: Mon Apr  8 16:32:47 2024, max compression
+gzip compressed data, was "pz-rail-base-0.2.3.tar", last modified: Tue Apr  9 18:21:35 2024, max compression
```

## Comparing `pz-rail-base-0.2.2.tar` & `pz-rail-base-0.2.3.tar`

### file list

```diff
@@ -1,156 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.057174 pz-rail-base-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-08 16:32:47.057174 pz-rail-base-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:32:47.057174 pz-rail-base-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.021174 pz-rail-base-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-08 16:32:47.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 16:32:46.000000 pz-rail-base-0.2.2/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    25183 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/point_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/util_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.029173 pz-rail-base-0.2.2/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/equal_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/uniform_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/dist_to_dist_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/dist_to_point_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/point_to_point_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/single_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/evaluation/stats_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.021174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.033174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.037174 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.037174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.037174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.041174 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.045174 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.025174 pz-rail-base-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/cli/hello_world.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/cli/single_number.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/core/test_point_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/creation/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/creation/test_degraders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/estimation/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:32:47.053174 pz-rail-base-0.2.2/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-08 16:32:39.000000 pz-rail-base-0.2.2/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.122435 pz-rail-base-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-09 18:21:35.122435 pz-rail-base-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:21:35.122435 pz-rail-base-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.082434 pz-rail-base-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:21:34.000000 pz-rail-base-0.2.3/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25183 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/point_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/util_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/degradation/addRandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/noisifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/dist_to_dist_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/dist_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/point_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/single_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/stats_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.106434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.106434 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.106434 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.110435 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/cli/hello_world.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/cli/single_number.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_point_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/creation/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.github/pull_request_template.md` & `pz-rail-base-0.2.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.github/workflows/linting.yml` & `pz-rail-base-0.2.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.github/workflows/smoke-test.yml` & `pz-rail-base-0.2.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.2.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.gitignore` & `pz-rail-base-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/.pre-commit-config.yaml` & `pz-rail-base-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/LICENSE` & `pz-rail-base-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/PKG-INFO` & `pz-rail-base-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.2
+Version: 0.2.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.2/README.md` & `pz-rail-base-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/pyproject.toml` & `pz-rail-base-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/pz_rail_base.egg-info/PKG-INFO` & `pz-rail-base-0.2.3/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.2
+Version: 0.2.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.2/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.2.3/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 src/rail/core/introspection.py
 src/rail/core/point_estimation.py
 src/rail/core/stage.py
 src/rail/core/util_stages.py
 src/rail/core/utils.py
 src/rail/creation/degrader.py
 src/rail/creation/engine.py
+src/rail/creation/noisifier.py
+src/rail/creation/selector.py
+src/rail/creation/degradation/addRandom.py
 src/rail/creation/degradation/quantityCut.py
 src/rail/estimation/classifier.py
 src/rail/estimation/estimator.py
 src/rail/estimation/informer.py
 src/rail/estimation/summarizer.py
 src/rail/estimation/algos/equal_count.py
 src/rail/estimation/algos/naive_stack.py
```

### Comparing `pz-rail-base-0.2.2/src/rail/cli/commands.py` & `pz-rail-base-0.2.3/src/rail/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/cli/options.py` & `pz-rail-base-0.2.3/src/rail/cli/options.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/cli/scripts.py` & `pz-rail-base-0.2.3/src/rail/cli/scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/__init__.py` & `pz-rail-base-0.2.3/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/algo_utils.py` & `pz-rail-base-0.2.3/src/rail/core/algo_utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/common_params.py` & `pz-rail-base-0.2.3/src/rail/core/common_params.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/data.py` & `pz-rail-base-0.2.3/src/rail/core/data.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/introspection.py` & `pz-rail-base-0.2.3/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/point_estimation.py` & `pz-rail-base-0.2.3/src/rail/core/point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/stage.py` & `pz-rail-base-0.2.3/src/rail/core/stage.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/util_stages.py` & `pz-rail-base-0.2.3/src/rail/core/util_stages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/core/utils.py` & `pz-rail-base-0.2.3/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.2.3/src/rail/creation/degradation/quantityCut.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Degrader that applies a cut to given columns."""
 
 from numbers import Number
 
 import numpy as np
-from rail.creation.degrader import Degrader
+from rail.creation.selector import Selector
 
 
-class QuantityCut(Degrader):
+class QuantityCut(Selector):
     """Degrader that applies a cut to the given columns.
 
     Note that if a galaxy fails any of the cuts on any one of its columns, that
     galaxy is removed from the sample.
     """
 
     name = "QuantityCut"
-    config_options = Degrader.config_options.copy()
+    config_options = Selector.config_options.copy()
     config_options.update(cuts=dict)
 
     def __init__(self, args, comm=None):
         """Constructor.
         
         Performs standard Degrader initialization as well as defining the cuts 
         to be applied.
         """
-        Degrader.__init__(self, args, comm=comm)
+        Selector.__init__(self, args, comm=comm)
         self.cuts = None
         self.set_cuts(self.config["cuts"])
 
     def set_cuts(self, cuts: dict):
         """Defines the cuts to be applied.
 
         Parameters
@@ -78,40 +78,41 @@
                     )
                 # if all of these checks passed, save the cuts
                 self.cuts[quantity] = (cut[0], cut[1])
             # if the cut isn't a number or iterable, it's the wrong type
             else:
                 raise TypeError(bad_cut_msg)
 
-    def run(self):
+    def _select(self):
         """Applies cuts.
 
         Notes
         -----
         Gets the input data from the data store under this stage's 'input' tag.
 
         Puts the data into the data store under this stage's 'output' tag.
         """
         data = self.get_data("input")
 
         # get overlap of columns from data and columns on which to make cuts
         columns = set(self.cuts.keys()).intersection(data.columns)
 
         if len(columns) == 0:  # pragma: no cover
-            self.add_data("output", data)
+            return np.ones(len(data), dtype=int)
         else:
             # generate a pandas query from the cuts
             query = [
                 f"{col} > {self.cuts[col][0]} & {col} < {self.cuts[col][1]}"
                 for col in columns
             ]
             query = " & ".join(query)
-
-            out_data = data.query(query)
-            self.add_data("output", out_data)
+            out_indices = data.query(query).index.values
+            out_mask = np.zeros(len(data), dtype=int)
+            out_mask[out_indices] = 1
+            return out_mask
 
     def __repr__(self):  # pragma: no cover
         """Pretty print this object."""
         printMsg = "Degrader that applies the following cuts to a pandas DataFrame:\n"
         printMsg += "{column: (min, max), ...}\n"
         printMsg += self.cuts.__str__()
         return printMsg
```

### Comparing `pz-rail-base-0.2.2/src/rail/creation/degrader.py` & `pz-rail-base-0.2.3/src/rail/creation/degrader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and returns a pandas DataFrame, and wraps the run method.
 """
 
 from rail.core.stage import RailStage
 from rail.core.data import PqHandle
 
 
-class Degrader(RailStage):
+class Degrader(RailStage):  # pragma: no cover
     """Base class Degraders, which apply various degradations to synthetic 
     photometric data.
 
     Degraders take "input" data in the form of pandas dataframes in Parquet 
     files and provide as "output" another pandas dataframes written to Parquet 
     files.
     """
```

### Comparing `pz-rail-base-0.2.2/src/rail/creation/engine.py` & `pz-rail-base-0.2.3/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/equal_count.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/equal_count.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/naive_stack.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/naive_stack.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/point_est_hist.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/point_est_hist.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/random_gauss.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/random_gauss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/train_z.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/train_z.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/uniform_binning.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/uniform_binning.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/algos/var_inf.py` & `pz-rail-base-0.2.3/src/rail/estimation/algos/var_inf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/classifier.py` & `pz-rail-base-0.2.3/src/rail/estimation/classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/estimator.py` & `pz-rail-base-0.2.3/src/rail/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/informer.py` & `pz-rail-base-0.2.3/src/rail/estimation/informer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/estimation/summarizer.py` & `pz-rail-base-0.2.3/src/rail/estimation/summarizer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/dist_to_dist_evaluator.py` & `pz-rail-base-0.2.3/src/rail/evaluation/dist_to_dist_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/dist_to_point_evaluator.py` & `pz-rail-base-0.2.3/src/rail/evaluation/dist_to_point_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/evaluator.py` & `pz-rail-base-0.2.3/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.2.3/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.2.3/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.2.3/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/point_to_point_evaluator.py` & `pz-rail-base-0.2.3/src/rail/evaluation/point_to_point_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/evaluation/single_evaluator.py` & `pz-rail-base-0.2.3/src/rail/evaluation/single_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/output_BPZ_lite.hdf5` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.2.3/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/src/rail/stages/__init__.py` & `pz-rail-base-0.2.3/src/rail/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/cli/hello_world.ipynb` & `pz-rail-base-0.2.3/tests/cli/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/cli/single_number.ipynb` & `pz-rail-base-0.2.3/tests/cli/single_number.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/cli/test_scripts.py` & `pz-rail-base-0.2.3/tests/cli/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/core/test_core.py` & `pz-rail-base-0.2.3/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/core/test_introspection.py` & `pz-rail-base-0.2.3/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/core/test_pipeline.py` & `pz-rail-base-0.2.3/tests/core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/core/test_point_estimation.py` & `pz-rail-base-0.2.3/tests/core/test_point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/creation/test_degraders.py` & `pz-rail-base-0.2.3/tests/creation/test_degraders.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from rail.core.data import DATA_STORE, TableHandle
 from rail.core.util_stages import ColumnMapper
 from rail.creation.degradation.quantityCut import QuantityCut
-# from rail.creation.degradation.spectroscopic_selections import *
+from rail.creation.degradation.addRandom import AddColumnOfRandom
 
 
 @pytest.fixture
 def data():
     """Some dummy data to use below."""
 
     DS = DATA_STORE()
@@ -67,18 +67,37 @@
         QuantityCut.make_stage(cuts=cuts)
 
 
 def test_QuantityCut_returns_correct_shape(data):
     """Make sure QuantityCut is returning the correct shape"""
 
     cuts = {
-        "u": 0,
-        "y": (1, 2),
+        "u": 30,
+        "redshift": (1, 2),
     }
     degrader = QuantityCut.make_stage(cuts=cuts)
 
     degraded_data = degrader(data).data
 
-    assert degraded_data.shape == data.data.query("u < 0 & y > 1 & y < 2").shape
+    assert degraded_data.shape == data.data.query("u < 30 & redshift > 1 & redshift < 2").shape
     os.remove(degrader.get_output(degrader.get_aliased_tag("output"), final_name=True))
 
+    
+    degrader_w_flag = QuantityCut.make_stage(name="degrader_w_flag", cuts=cuts, drop_rows=False)
 
+    degraded_data_w_flag = degrader_w_flag(data).data
+
+    test_mask = np.zeros(len(data.data), dtype=int)
+    out_indices = data.data.query("u < 30 & redshift > 1 & redshift < 2").index.values
+    test_mask[out_indices] = 1
+    
+    assert (degraded_data_w_flag['flag'] == test_mask).all()
+    os.remove(degrader_w_flag.get_output(degrader_w_flag.get_aliased_tag("output"), final_name=True))
+
+
+
+def test_add_random(data):
+
+    add_random = AddColumnOfRandom.make_stage()
+
+    test_data = add_random(data, seed=1234).data
+    assert len(test_data[add_random.config.col_name]) == len(data.data)
```

### Comparing `pz-rail-base-0.2.2/tests/estimation/test_algos.py` & `pz-rail-base-0.2.3/tests/estimation/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/estimation/test_classifier.py` & `pz-rail-base-0.2.3/tests/estimation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/estimation/test_summarizers.py` & `pz-rail-base-0.2.3/tests/estimation/test_summarizers.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.2/tests/evaluation/test_evaluation.py` & `pz-rail-base-0.2.3/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

