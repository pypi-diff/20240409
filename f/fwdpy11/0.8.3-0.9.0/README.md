# Comparing `tmp/fwdpy11-0.8.3.tar.gz` & `tmp/fwdpy11-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fwdpy11-0.8.3.tar", last modified: Fri Jul 10 18:47:47 2020, max compression
+gzip compressed data, was "dist/fwdpy11-0.9.0.tar", last modified: Tue Aug  4 22:24:31 2020, max compression
```

## Comparing `fwdpy11-0.8.3.tar` & `fwdpy11-0.9.0.tar`

### file list

```diff
@@ -1,688 +1,707 @@
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.139408 fwdpy11-0.8.3/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.055408 fwdpy11-0.8.3/.circleci/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4015 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/.circleci/config.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)       30 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/.flake8
--rw-r--r--   0 kevin     (1000) kevin     (1000)       51 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/.gitignore
--rw-r--r--   0 kevin     (1000) kevin     (1000)      108 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/.gitmodules
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      904 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/.travis.yml
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      529 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/.ycm_extra_conf.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1278 2020-07-08 17:43:29.000000 fwdpy11-0.8.3/CMakeLists.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35147 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/COPYING
--rw-r--r--   0 kevin     (1000) kevin     (1000)      559 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/MANIFEST.in
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12549 2020-07-10 18:47:47.139408 fwdpy11-0.8.3/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9782 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/README.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)       27 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/_config.yml
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.059408 fwdpy11-0.8.3/doc/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      605 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/Makefile
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.051408 fwdpy11-0.8.3/doc/_build/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.051408 fwdpy11-0.8.3/doc/_build/html/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.059408 fwdpy11-0.8.3/doc/_build/html/_images/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    51220 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/_build/html/_images/localadaptation.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    64515 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/_build/html/_images/migtest.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    35892 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/_build/html/_images/moments_IM_gamma_minus_5.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    40452 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/_build/html/_images/moments_IM_neutral.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8325 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/_build/html/_images/tables.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4616 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/_build/html/_images/tree.png
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.059408 fwdpy11-0.8.3/doc/_build/html/_static/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      286 2020-05-03 15:18:47.000000 fwdpy11-0.8.3/doc/_build/html/_static/file.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       90 2020-05-03 15:18:47.000000 fwdpy11-0.8.3/doc/_build/html/_static/minus.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       90 2020-05-03 15:18:47.000000 fwdpy11-0.8.3/doc/_build/html/_static/plus.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7853 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/conf.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      294 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/environment.yml
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.059408 fwdpy11-0.8.3/doc/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2879 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/examples/IM.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      324 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/examples/bgs.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1652 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/examples/gss.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1301 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/doc/examples/gss_divergent_optima.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1381 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/examples/localadaptation.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1478 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/examples/migtest.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1383 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/doc/examples/precapitation.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    15282 2020-04-19 00:00:10.000000 fwdpy11-0.8.3/doc/examples/recapitation.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2167 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/doc/examples/recorder.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      410 2020-07-10 18:45:24.000000 fwdpy11-0.8.3/doc/examples/snowdrift.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)   100305 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/fwdpp.doxygen
--rw-r--r--   0 kevin     (1000) kevin     (1000)   100285 2020-04-18 21:57:15.000000 fwdpy11-0.8.3/doc/fwdpy11.doxygen
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.059408 fwdpy11-0.8.3/doc/images/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      256 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/Makefile
--rw-r--r--   0 kevin     (1000) kevin     (1000)    51220 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/localadaptation.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    64515 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/migtest.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35892 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/moments_IM_gamma_minus_5.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    40452 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/moments_IM_neutral.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1590 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/structures.dot
--rw-r--r--   0 kevin     (1000) kevin     (1000)   107628 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/structures.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1045 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/tables.dot
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8325 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/tables.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)      331 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/tree.dot
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4616 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/images/tree.png
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1520 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/index.rst
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.059408 fwdpy11-0.8.3/doc/misc/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    35453 2020-07-10 18:45:24.000000 fwdpy11-0.8.3/doc/misc/changelog.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      434 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/misc/deprecated.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3491 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/doc/misc/developersguide.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1341 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/misc/pubs.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5505 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/misc/references.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4597 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/misc/upgrade_path.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3430 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/misc/writingplugins.rst
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.063408 fwdpy11-0.8.3/doc/pages/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12135 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/advancedtopics.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      210 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/doc/pages/datamatrix.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4010 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/definitions.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1219 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/demographic_models.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      640 2020-04-21 18:07:23.000000 fwdpy11-0.8.3/doc/pages/functions.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      816 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/genetic_values.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      712 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/gvalue_to_fitness.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      269 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/gvaluenoise.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      206 2020-06-02 21:30:49.000000 fwdpy11-0.8.3/doc/pages/model_params.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    11439 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/mvdes.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2445 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/recorders.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1058 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/regiontypes.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    24188 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/softselection.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5476 2020-07-03 19:06:05.000000 fwdpy11-0.8.3/doc/pages/tablefs.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      724 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/tskit_tools.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7476 2020-04-17 19:50:03.000000 fwdpy11-0.8.3/doc/pages/tsoverview.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9650 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/doc/pages/tstypes.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    44140 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/pages/tutorial.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7082 2020-06-23 18:30:05.000000 fwdpy11-0.8.3/doc/pages/types.rst
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.063408 fwdpy11-0.8.3/doc/savefig/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    88886 2020-07-03 19:25:56.000000 fwdpy11-0.8.3/doc/savefig/efficient_timeseries_example.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    30665 2020-04-09 19:03:27.000000 fwdpy11-0.8.3/doc/savefig/gss_two_deme_effect_sizes.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    36220 2020-07-03 19:25:48.000000 fwdpy11-0.8.3/doc/savefig/mean_genetic_values_over_time.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35755 2020-07-03 19:25:50.000000 fwdpy11-0.8.3/doc/savefig/pi_over_time.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    44561 2020-07-03 19:25:52.000000 fwdpy11-0.8.3/doc/savefig/sfs_example.png
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.063408 fwdpy11-0.8.3/doc/unused_pages/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12826 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/0000a_anintroexample.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9869 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/0000a_objectoverview.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4864 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/0000a_tskit_interchange.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5053 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/0000a_working_with_genotypes_trees.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3427 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/mutation.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7301 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/recombination.rst
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4301 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/doc/unused_pages/tstimeseries.rst
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.063408 fwdpy11-0.8.3/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35147 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/examples/COPYING
--rw-r--r--   0 kevin     (1000) kevin     (1000)      708 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/examples/README.rst
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.063408 fwdpy11-0.8.3/examples/bgs/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3606 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/examples/bgs/bgs.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.063408 fwdpy11-0.8.3/examples/discrete_demography/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12254 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/examples/discrete_demography/IM.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7832 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/examples/discrete_demography/localadaptation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6213 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/examples/discrete_demography/migtest.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/examples/gss/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7839 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/examples/gss/DiploidPopulationGSSmo.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      759 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/examples/gss/Makefile
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2397 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/examples/gss/README.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      329 2020-04-17 18:22:02.000000 fwdpy11-0.8.3/examples/gss/compare.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1042 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/examples/gss/iterate_variants_in_tree_sequences.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      799 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/examples/gss/plot_genetic_values_from_tree_sequences.py
--rwxr-xr-x   0 kevin     (1000) kevin     (1000)      515 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/examples/gss/plotstats.R
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/examples/gss_divergent_optima/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2102 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/examples/gss_divergent_optima/gss_divergent_optima.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/examples/plugin/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      954 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/examples/plugin/CMakeLists.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      680 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/examples/plugin/gvalue_recorder.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      642 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/examples/plugin/test_plugin.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/examples/tskit/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6357 2020-04-19 00:00:10.000000 fwdpy11-0.8.3/examples/tskit/precapitate.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6325 2020-04-19 00:00:10.000000 fwdpy11-0.8.3/examples/tskit/recapitate.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      253 2020-04-19 00:17:34.000000 fwdpy11-0.8.3/examples/tskit/session.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/fwdpy11/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4950 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/CMakeLists.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2386 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2239 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/__main__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1172 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/_demography.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1368 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/_dev.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2713 2020-06-02 21:30:49.000000 fwdpy11-0.8.3/fwdpy11/_evolve_genomes.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6590 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/_evolvets.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/fwdpy11/_monkeypatch/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/_monkeypatch/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2637 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/_monkeypatch/_data_matrix.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9150 2020-07-08 17:43:29.000000 fwdpy11-0.8.3/fwdpy11/_monkeypatch/_diploid_population.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9398 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/_monkeypatch/_table_collection.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/fwdpy11/_types/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/_types/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    23627 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/_types/demography_debugger.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    11493 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/_types/model_params.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      116 2020-07-10 18:47:42.000000 fwdpy11-0.8.3/fwdpy11/_version.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3354 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/class_decorators.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/fwdpy11/demographic_models/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5986 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/demographic_models/IM.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      139 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/demographic_models/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2949 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/demographic_models/demographic_model_details.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    14354 2020-07-08 17:43:29.000000 fwdpy11-0.8.3/fwdpy11/demographic_models/human.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    16248 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/discrete_demography.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2157 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/ezparams.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6470 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/genetic_map_unit.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    17759 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/genetic_values.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.051408 fwdpy11-0.8.3/fwdpy11/headers/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.051408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.071408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8531 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/K_linked_regions_extensions.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      781 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/calculate_fitnesses.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      684 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/common_ind.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1711 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/confirm_mutation_counts.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2180 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/custom_diploid.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6898 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/custom_mutation.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5167 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/diploid_fixed_sh_ind.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7885 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/diploid_ind.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    17455 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/edge_buffering.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4222 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/evolve_generation_ts.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12527 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/juvenile_migration.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1440 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/load_table_collection.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3710 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/simplify_tables.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    18684 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2393 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      638 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_types.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.071408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/unused_source/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1491 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2430 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing_with_mutation.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    22549 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/wfevolvets.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1148 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/wfevolvets.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    16057 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/wfts_integration_test.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.075408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4082 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/GSLrng_t.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.075408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/algorithm/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3422 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/algorithm/compact_mutations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9973 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/data_matrix.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4457 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/debug.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1497 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/diploid.hh
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      994 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/diploid_population.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.075408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/extensions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6158 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/extensions/callbacks.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10022 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/extensions/regions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    30609 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/fitness_models.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7029 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/forward_types.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3043 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/forward_types_serialization.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1474 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/fwd_functional.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.075408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1694 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_interval.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1376 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_point.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1617 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/fixed_number_crossovers.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1277 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/genetic_map.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      492 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/genetic_map_unit.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1741 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_interval.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1388 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_point.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.075408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/gsl/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      360 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/gsl/deleter.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      472 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/gsl/tags.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      756 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/gsl_discrete.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      655 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/insertion_policies.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8633 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/data_matrix_details.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8416 2020-06-09 01:40:02.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/debug_details.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    21068 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/haploid_genome_cleaner.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2122 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/mutation_internal.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1596 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/rec_gamete_updater.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2189 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/recombination_common.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1490 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/sample_diploid_helpers.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1475 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/sampling_functions_details.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10765 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/type_traits.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      487 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/util.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      444 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/void_t.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/detail/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2970 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/detail/serialize_population.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5816 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/diploid.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3459 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/haploid_genome.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3678 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/mutation.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1933 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/scalar_serialization.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1100 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/serialize_population.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/meta/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      249 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/meta/always_false.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    20755 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/mutate_recombine.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6023 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/popgenmut.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2960 2020-05-14 19:25:52.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/diploid_population.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6725 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/popbase.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      545 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/tags.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      453 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/recbinder.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5754 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12829 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.tcc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1574 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sampling_functions.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/simfunctions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5550 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/simfunctions/recycling.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6626 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/simparams.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sugar/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    13096 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sugar/add_mutation.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3694 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sugar/change_neutral.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.079408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/tags/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      266 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/tags/tags.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.083408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4072 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/count_mutations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3289 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/decapitate.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      642 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/definitions.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.083408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/detail/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4029 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/detail/advance_marginal_tree_policies.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4076 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/detail/generate_data_matrix_details.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1033 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/edge.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1244 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/exceptions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2738 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/generate_data_matrix.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    11116 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/generate_offspring.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1125 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/get_parent_ids.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    13542 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.083408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4950 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/children.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1058 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_order.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2270 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_preorder.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7379 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/nodes.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3541 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/roots.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5426 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/samples.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1162 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/statistics.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      288 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1758 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mark_multiple_roots.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7111 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mutate_tables.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1336 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_record.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      700 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_tools.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      792 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/node.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.083408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6378 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/diploid_offspring.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10144 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/edge_buffer.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1253 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/mutations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      187 2020-06-09 17:03:47.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    15820 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recycling.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4456 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/remove_fixations_from_gametes.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    17632 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/serialization.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      505 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/serialization_version.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.083408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/simplification/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    28798 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/simplification/simplification.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      261 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/simplification_flags.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    16320 2020-06-22 23:25:50.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/simplify_tables.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      718 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/site.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5407 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/site_visitor.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      558 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/std_table_collection.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9097 2020-06-25 00:20:35.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6526 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection_functions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3233 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/table_simplifier.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    20804 2020-06-25 02:45:36.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/tree_visitor.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4978 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/visit_sites.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9032 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/type_traits.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.087408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      786 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/abstract_cloneable.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2342 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/enum_bitflags.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1449 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/named_type.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7671 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/nested_forward_lists.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1195 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/wrapped_range.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10253 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      258 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/version.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.087408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/src/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      444 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/src/fwdppConfig.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.051408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.087408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3031 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/fwdpp_fixtures.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      202 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/rng_fixture.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       61 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/sugar_fixtures.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2290 2020-05-14 19:25:52.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/sugar_fixtures.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.087408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      100 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/extensions_integration_tests.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5480 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/extensions_regionsIntegrationTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       95 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/sugar_integration_tests.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1461 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepopTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1180 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepop_custom_diploidTest.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.091408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      356 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/empty_table_collection.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2400 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1061 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1864 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/preorder_adl.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2161 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1612 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_infinite_sites.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2328 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_polytomy.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1399 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_ancestry_list.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2619 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_decapitate.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      794 2020-06-09 01:40:02.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_diploid_recording.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7885 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_edge_buffering_std_table_collection.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2301 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_data_matrix.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2837 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_offspring.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1804 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1278 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree_statistics.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1347 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_node_children_traversal.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      461 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_node_traversal_order_adl.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3512 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_preorder_node_traversal.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1336 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_root_traversal.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2911 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_sample_traversal.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      717 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_site_visitor.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1878 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_table_collection.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7834 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_tree_visitor.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      989 2020-06-06 22:15:39.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_visit_sites.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       98 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tree_sequence_tests.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3045 2020-06-17 21:24:15.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      905 2020-06-17 21:24:15.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12226 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1207 2020-06-17 21:24:15.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection_fxns.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5220 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/extensions_callbacksTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2317 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/extensions_regionsTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       93 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/extensions_unit_test.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       88 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/fwdpp_unit_tests.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1603 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/gameteTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3324 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/gamete_cleanerTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       90 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/genetic_map_tests.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3082 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/mutateTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      933 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/serializationTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    12336 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/siteDepFitnessTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      787 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_GSLrngTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8287 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_add_mutationTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1621 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_change_neutralTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1388 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_popgenmut.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       88 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_unit_tests.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1771 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_enum_bitflags.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8469 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_genetic_map.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6383 2020-05-14 19:25:52.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_mutate_recombine.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1248 2020-06-23 16:58:53.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_nested_forward_lists.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      787 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_recombination.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2079 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_simparams.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      693 2020-06-18 18:46:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_wrapped_range.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6795 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/type_traitsTest.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9201 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/utilTest.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/util/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2345 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/util/custom_dip.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4238 2020-05-08 23:04:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/util/quick_evolve_sugar.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    16148 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/DiscreteDemography.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4137 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/MassMigration.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4742 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/MigrationMatrix.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1877 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetDemeSize.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2138 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetExponentialGrowth.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5471 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetMigrationRates.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2139 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetSelfingRate.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1137 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/constants.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2352 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/exceptions.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    16665 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/apply_mass_migrations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5560 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/build_migration_lookup.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3533 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_properties.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2048 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_property_types.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5007 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/demographic_model_state.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1960 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/detail.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    11577 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/functions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4335 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/get_max_number_of_demes.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1323 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/migration_lookup.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4187 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/multideme_fitness_lookups.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3826 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/pick_parents.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6287 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/update_demographic_model_state.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1333 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolve/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5047 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolve/DiploidPopulation_generation.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2403 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/SampleRecorder.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7797 2020-06-25 18:34:29.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/evolve_generation_ts.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2668 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/recorders.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1208 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/sample_recorder_types.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6222 2020-06-25 20:24:21.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/simplify_tables.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_noise/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1572 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_noise/GeneticValueNoise.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1521 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_noise/NoNoise.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2469 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GSSmo.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1655 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsFitness.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1173 2020-05-28 17:29:52.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1981 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueToFitnessMap.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3628 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/MultivariateGSSmo.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1986 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/Optimum.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2971 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/PleiotropicOptima.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5627 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/DiploidGeneticValue.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3031 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/DiploidMultivariateEffectsStrictAdditive.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1167 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/default_update.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1986 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/GBR.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1150 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_GBR.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1331 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_multiplicative.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2783 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/dgvalue_pointer_vector.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/fwdpp_wrappers/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5179 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/fwdpp_wrappers/fwdpp_genetic_value.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.099408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/gsl/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      631 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/gsl/gsl_error_handler_wrapper.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/numpy/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2680 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/numpy/array.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/policies/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6027 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/policies/mutation.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2345 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/ConstantS.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1848 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/ExpS.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2150 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/GammaS.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2003 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/GaussianS.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2471 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/LogNormalS.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6104 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/MultivariateGaussianEffects.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2750 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/MutationRegions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2937 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/RecombinationRegions.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1482 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/Region.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2241 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/Sregion.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2127 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/UniformS.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    17222 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/mvDES.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1074 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/rng.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1069 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/samplers.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/sampling/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1864 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/sampling/data_matrix_functions.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1868 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/Diploid.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3464 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/Mutation.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4032 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/backwards_compat.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2616 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/diploid_metadata.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10977 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7810 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/sim_functions.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2263 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/Diploid.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8573 2020-06-29 20:13:19.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/DiploidPopulation.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3560 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/Mutation.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10551 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/Population.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      456 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/typedefs.hpp
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/util/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      923 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/util/clone_cloneable.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      657 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/util/convert_lists.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    18884 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/regions.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/src/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2265 2020-07-08 17:43:29.000000 fwdpy11-0.8.3/fwdpy11/src/_fwdpy11.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.103408 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9726 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/DiscreteDemography.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1655 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/MassMigration.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1640 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/MigrationMatrix.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1291 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetDemeSize.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1212 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetExponentialGrowth.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1400 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetMigrationRates.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1169 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetSelfingRate.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1168 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/exceptions.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1653 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/discrete_demography/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.107408 fwdpy11-0.8.3/fwdpy11/src/evolve_population/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      755 2020-06-07 03:09:23.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/cleanup_metadata.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      393 2020-06-07 03:09:23.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/cleanup_metadata.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3027 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/diploid_pop_fitness.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1128 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/diploid_pop_fitness.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      917 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/index_and_count_mutations.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      323 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/index_and_count_mutations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      395 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/init.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      243 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/no_stopping.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7458 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/no_tree_sequences.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2045 2020-06-29 20:13:19.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/remove_extinct_genomes.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      220 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/remove_extinct_genomes.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3604 2020-06-29 20:13:19.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/remove_extinct_mutations.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      222 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/remove_extinct_mutations.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1400 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/track_ancestral_counts.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      500 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/track_ancestral_counts.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2021 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/track_mutation_counts.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      330 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/track_mutation_counts.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      957 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/util.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      489 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/util.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    28064 2020-06-29 20:13:19.000000 fwdpy11-0.8.3/fwdpy11/src/evolve_population/with_tree_sequences.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.107408 fwdpy11-0.8.3/fwdpy11/src/fwdpp_functions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6160 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_functions/data_matrix_creation.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      210 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_functions/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.111408 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      434 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/BinomialInterval.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      354 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/BinomialPoint.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7628 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/DataMatrix.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1867 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/Edge.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1026 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/EdgeTable.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      383 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/FixedCrossovers.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      651 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/GeneticMapUnit.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2210 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/HaploidGenome.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      769 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/MutationBase.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2879 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/MutationRecord.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1136 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/MutationTable.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      217 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/NULL_NODE.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1455 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/Node.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1047 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/NodeTable.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      357 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/PoissonInterval.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      313 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/PoissonPoint.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1343 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/Site.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1046 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/SiteTable.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4013 2020-06-07 03:09:23.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/TableCollection.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1983 2020-06-23 18:30:05.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.111408 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_functions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3908 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_functions/change_effect_size.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      261 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_functions/init.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2091 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_functions/sort_gamete_keys.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.115408 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1551 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidGenotype.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4708 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidMetadata.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    16131 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidPopulation.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2936 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidVector.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1798 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/HaploidGenomeVector.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5421 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/Mutation.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1814 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/MutationVector.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    11087 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/PopulationBase.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      402 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/RecordNothing.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1161 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/get_individuals.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      855 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/init.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      441 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/rng.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4003 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/ts_from_tskit.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2680 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/tsrecorders.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.115408 fwdpy11-0.8.3/fwdpy11/src/genetic_value_noise/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1174 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_noise/GaussianNoise.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      322 2020-05-26 21:05:44.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_noise/GeneticValueNoise.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      253 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_noise/NoNoise.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      305 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_noise/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.119408 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      343 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/GSSmo.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      706 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/GeneticValueIsFitness.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      401 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/GeneticValueIsTrait.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1245 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/GeneticValueToFitnessMap.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      441 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/MultivariateGSSmo.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1318 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/Optimum.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1514 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/PleiotropicOptima.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      683 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.119408 fwdpy11-0.8.3/fwdpy11/src/genetic_values/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3705 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/Additive.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3530 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/DiploidGeneticValue.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1156 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/DiploidMultivariateEffectsStrictAdditive.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4440 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/GBR.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4023 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/Multiplicative.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1076 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/dgvalue_pointer_vector.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      706 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/genetic_values/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.119408 fwdpy11-0.8.3/fwdpy11/src/gsl/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1943 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/gsl/gsl_random.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      589 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/gsl/init.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.119408 fwdpy11-0.8.3/fwdpy11/src/regions/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      759 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/ConstantS.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      688 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/ExpS.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      766 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/GammaS.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      690 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/GaussianS.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1111 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/LogNormalS.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1291 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/MultivariateGaussianEffects.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1462 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/regions/MutationRegions.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1843 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/regions/RecombinationRegions.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      388 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/Region.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      936 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/Sregion.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      749 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/UniformS.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      834 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/regions/init.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5317 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/fwdpy11/src/regions/mvDES.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.123408 fwdpy11-0.8.3/fwdpy11/src/ts/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    20858 2020-06-23 18:30:05.000000 fwdpy11-0.8.3/fwdpy11/src/ts/DataMatrixIterator.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    17567 2020-06-23 18:30:05.000000 fwdpy11-0.8.3/fwdpy11/src/ts/TreeIterator.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     9925 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/ts/VariantIterator.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1925 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/ts/count_mutations.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3113 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/ts/data_matrix_from_tables.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2682 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/ts/infinite_sites.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      600 2020-05-08 22:56:22.000000 fwdpy11-0.8.3/fwdpy11/src/ts/init.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      212 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/ts/node_traversal.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      147 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/ts/node_traversal.hpp
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4311 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/fwdpy11/src/ts/simplify.cc
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.123408 fwdpy11-0.8.3/fwdpy11/tskit_tools/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      848 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/fwdpy11/tskit_tools/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      368 2020-06-02 21:30:49.000000 fwdpy11-0.8.3/fwdpy11/tskit_tools/_flags.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.067408 fwdpy11-0.8.3/fwdpy11.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12549 2020-07-10 18:47:42.000000 fwdpy11-0.8.3/fwdpy11.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)    26717 2020-07-10 18:47:46.000000 fwdpy11-0.8.3/fwdpy11.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2020-07-10 18:47:42.000000 fwdpy11-0.8.3/fwdpy11.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2020-03-30 21:43:01.000000 fwdpy11-0.8.3/fwdpy11.egg-info/not-zip-safe
--rw-r--r--   0 kevin     (1000) kevin     (1000)       48 2020-07-10 18:47:42.000000 fwdpy11-0.8.3/fwdpy11.egg-info/requires.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        8 2020-07-10 18:47:42.000000 fwdpy11-0.8.3/fwdpy11.egg-info/top_level.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      714 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/gplheader.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      732 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/gplheader_cpp.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1306 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/index.md
--rwxr-xr-x   0 kevin     (1000) kevin     (1000)    13997 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/install-sh
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.123408 fwdpy11-0.8.3/m4/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5036 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/m4/ax_cxx_compile_stdxx_11.m4
--rw-r--r--   0 kevin     (1000) kevin     (1000)    22072 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/m4/python.m4
--rw-r--r--   0 kevin     (1000) kevin     (1000)      116 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/readthedocs.yml
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      339 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/requirements.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       38 2020-07-10 18:47:47.139408 fwdpy11-0.8.3/setup.cfg
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7700 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/setup.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.139408 fwdpy11-0.8.3/tests/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3397 2020-07-10 18:45:24.000000 fwdpy11-0.8.3/tests/CMakeLists.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1602 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/EsizeZero.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)      540 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/call_Sregion.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1166 2020-04-13 17:46:17.000000 fwdpy11-0.8.3/tests/common_mako.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2052 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/custom_additive.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2271 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/custom_stateless_genotype.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6188 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/discrete_demography_roundtrips.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)      670 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/fixation_properties.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)      730 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/gsl_error.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2317 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/inherit_noise.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4516 2020-07-10 18:45:24.000000 fwdpy11-0.8.3/tests/ll_snowdrift.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1744 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/numpy_array_interface.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2977 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/pickling_composed_classes.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)      664 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/pickling_cpp.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)      375 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/poptools.cc
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2554 2020-06-02 21:30:49.000000 fwdpy11-0.8.3/tests/quick_pops.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1256 2020-07-10 18:45:24.000000 fwdpy11-0.8.3/tests/snowdrift.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      991 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/sregion_cdf.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)      710 2020-04-17 19:30:58.000000 fwdpy11-0.8.3/tests/testMultivariateGSSmo.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5078 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_DataMatrix.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7449 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/tests/test_DemographyDebugger.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4934 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_DiploidPopulation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      532 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_GSLerror.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4445 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_ModelParams.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2056 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/tests/test_Mutation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      640 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_SampleRecorder.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3403 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_Sregion_from_cdf.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8676 2020-04-17 18:19:05.000000 fwdpy11-0.8.3/tests/test_TableCollection_fs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6945 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_add_mutation.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      706 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_binary_format_compatibility.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1574 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/tests/test_class_decorators.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1507 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_custom_exceptions.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1881 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_custom_stateless_fitness.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     8509 2020-07-08 17:43:29.000000 fwdpy11-0.8.3/tests/test_demographic_models.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1356 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/tests/test_dgvalue_pointer_vector.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    37078 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_discrete_demography.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    34274 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_discrete_demography_with_tree_sequences.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4930 2020-06-02 21:30:49.000000 fwdpy11-0.8.3/tests/test_fixation_properties.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      813 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_fwdpp_types.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1864 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_genetic_value_noise.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3227 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_genetic_value_to_fitness.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6575 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_genetic_values.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1802 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/tests/test_inherited_noise.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3249 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_multivariate_effects.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      594 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_mutation_labels.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1650 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/tests/test_numpy.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1415 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_numpy_array_interface.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2785 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_opaque.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     6793 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/tests/test_pickling.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      485 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_pickling_composed_classes.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    14259 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_record_genetic_value_matrix.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    15446 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_regions.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1868 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_simple_parallel.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2388 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_stateful_fitness.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1122 2020-04-23 19:14:24.000000 fwdpy11-0.8.3/tests/test_stopping_criterion.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    62706 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/tests/test_tree_sequences.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    13049 2020-07-10 17:54:56.000000 fwdpy11-0.8.3/tests/test_tree_sequences_different_des_in_different_demes.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2616 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_tree_sequences_esize_zero_selected_variants.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5563 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/tests/test_tree_sequences_with_neutral_mutations.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3125 2020-04-17 18:19:05.000000 fwdpy11-0.8.3/tests/test_ts_from_msprime.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3997 2020-04-17 18:23:29.000000 fwdpy11-0.8.3/tests/test_util.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1418 2020-06-02 21:30:49.000000 fwdpy11-0.8.3/tests/test_wright_fisher.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2020-06-04 19:54:21.000000 fwdpy11-0.8.3/tests/throw_custom_exceptions.cc
--rw-r--r--   0 kevin     (1000) kevin     (1000)   645031 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/tests/v045.bin
--rw-r--r--   0 kevin     (1000) kevin     (1000)   139100 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/tests/v045.lzma
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-07-10 18:47:47.139408 fwdpy11-0.8.3/travis_scripts/
--rwxrwxr-x   0 kevin     (1000) kevin     (1000)     2287 2020-06-06 22:25:38.000000 fwdpy11-0.8.3/travis_scripts/build_script.sh
--rwxr-xr-x   0 kevin     (1000) kevin     (1000)      198 2020-03-22 23:26:04.000000 fwdpy11-0.8.3/travis_scripts/gsl2.sh
--rwxrwxr-x   0 kevin     (1000) kevin     (1000)     2046 2020-06-23 18:29:32.000000 fwdpy11-0.8.3/travis_scripts/installation_script.sh
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.567612 fwdpy11-0.9.0/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.455612 fwdpy11-0.9.0/.circleci/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4015 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/.circleci/config.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       30 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/.flake8
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       51 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/.gitignore
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      108 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/.gitmodules
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      904 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/.travis.yml
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      529 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/.ycm_extra_conf.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1278 2020-07-08 17:43:29.000000 fwdpy11-0.9.0/CMakeLists.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    35147 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/COPYING
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      559 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/MANIFEST.in
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12549 2020-08-04 22:24:31.567612 fwdpy11-0.9.0/PKG-INFO
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9782 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/README.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       27 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/_config.yml
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.459612 fwdpy11-0.9.0/doc/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      605 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/Makefile
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.451611 fwdpy11-0.9.0/doc/_build/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.451611 fwdpy11-0.9.0/doc/_build/html/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.459612 fwdpy11-0.9.0/doc/_build/html/_images/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    51220 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/_build/html/_images/localadaptation.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    64515 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/_build/html/_images/migtest.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    35892 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/_build/html/_images/moments_IM_gamma_minus_5.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    40452 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/_build/html/_images/moments_IM_neutral.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8325 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/_build/html/_images/tables.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4616 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/_build/html/_images/tree.png
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.459612 fwdpy11-0.9.0/doc/_build/html/_static/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      286 2020-05-03 15:18:47.000000 fwdpy11-0.9.0/doc/_build/html/_static/file.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       90 2020-05-03 15:18:47.000000 fwdpy11-0.9.0/doc/_build/html/_static/minus.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       90 2020-05-03 15:18:47.000000 fwdpy11-0.9.0/doc/_build/html/_static/plus.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7853 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/conf.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      294 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/environment.yml
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.463611 fwdpy11-0.9.0/doc/examples/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2879 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/examples/IM.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      324 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/examples/bgs.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1652 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/examples/gss.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1301 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/doc/examples/gss_divergent_optima.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1381 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/examples/localadaptation.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1478 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/examples/migtest.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1383 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/doc/examples/precapitation.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    47798 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/doc/examples/pysnowdrift.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      728 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/doc/examples/pysnowdrift.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    15282 2020-04-19 00:00:10.000000 fwdpy11-0.9.0/doc/examples/recapitation.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2167 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/doc/examples/recorder.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   100305 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/fwdpp.doxygen
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   100285 2020-04-18 21:57:15.000000 fwdpy11-0.9.0/doc/fwdpy11.doxygen
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.467611 fwdpy11-0.9.0/doc/images/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      256 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/Makefile
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    51220 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/localadaptation.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    64515 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/migtest.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    35892 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/moments_IM_gamma_minus_5.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    40452 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/moments_IM_neutral.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1590 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/structures.dot
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   107628 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/structures.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1045 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/tables.dot
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     8325 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/tables.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      331 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/tree.dot
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4616 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/images/tree.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1623 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/doc/index.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.467611 fwdpy11-0.9.0/doc/misc/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    36007 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/doc/misc/changelog.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      434 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/misc/deprecated.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3491 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/doc/misc/developersguide.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1341 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/misc/pubs.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5680 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/doc/misc/references.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4597 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/misc/upgrade_path.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.471611 fwdpy11-0.9.0/doc/pages/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    34289 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/doc/pages/advancedtopics.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      210 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/doc/pages/datamatrix.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4010 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/definitions.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1219 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/demographic_models.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      640 2020-04-21 18:07:23.000000 fwdpy11-0.9.0/doc/pages/functions.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      816 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/genetic_values.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1480 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/doc/pages/gslrandom.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      712 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/gvalue_to_fitness.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      269 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/gvaluenoise.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      206 2020-06-02 21:30:49.000000 fwdpy11-0.9.0/doc/pages/model_params.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11439 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/mvdes.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2445 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/recorders.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1058 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/regiontypes.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    24188 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/softselection.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5476 2020-07-03 19:06:05.000000 fwdpy11-0.9.0/doc/pages/tablefs.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      724 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/tskit_tools.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     7476 2020-04-17 19:50:03.000000 fwdpy11-0.9.0/doc/pages/tsoverview.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9650 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/doc/pages/tstypes.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    44140 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/pages/tutorial.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7082 2020-06-23 18:30:05.000000 fwdpy11-0.9.0/doc/pages/types.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.471611 fwdpy11-0.9.0/doc/savefig/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    88886 2020-07-03 19:25:56.000000 fwdpy11-0.9.0/doc/savefig/efficient_timeseries_example.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    30665 2020-04-09 19:03:27.000000 fwdpy11-0.9.0/doc/savefig/gss_two_deme_effect_sizes.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    36220 2020-07-03 19:25:48.000000 fwdpy11-0.9.0/doc/savefig/mean_genetic_values_over_time.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    35755 2020-07-03 19:25:50.000000 fwdpy11-0.9.0/doc/savefig/pi_over_time.png
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    44561 2020-07-03 19:25:52.000000 fwdpy11-0.9.0/doc/savefig/sfs_example.png
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.471611 fwdpy11-0.9.0/doc/technical/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11656 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/doc/technical/genetic_values.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3552 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/doc/technical/writingplugins.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.475612 fwdpy11-0.9.0/doc/unused_pages/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12826 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/0000a_anintroexample.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9869 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/0000a_objectoverview.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4864 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/0000a_tskit_interchange.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5053 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/0000a_working_with_genotypes_trees.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3427 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/mutation.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7301 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/recombination.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4301 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/doc/unused_pages/tstimeseries.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.475612 fwdpy11-0.9.0/examples/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    35147 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/examples/COPYING
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      708 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/examples/README.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.475612 fwdpy11-0.9.0/examples/bgs/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3606 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/examples/bgs/bgs.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.475612 fwdpy11-0.9.0/examples/discrete_demography/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12254 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/examples/discrete_demography/IM.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7832 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/examples/discrete_demography/localadaptation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6213 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/examples/discrete_demography/migtest.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.475612 fwdpy11-0.9.0/examples/gss/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7839 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/examples/gss/DiploidPopulationGSSmo.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      759 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/examples/gss/Makefile
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2397 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/examples/gss/README.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      329 2020-04-17 18:22:02.000000 fwdpy11-0.9.0/examples/gss/compare.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1042 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/examples/gss/iterate_variants_in_tree_sequences.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      799 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/examples/gss/plot_genetic_values_from_tree_sequences.py
+-rwxr-xr-x   0 kevin     (1000) kevin     (1000)      515 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/examples/gss/plotstats.R
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.475612 fwdpy11-0.9.0/examples/gss_divergent_optima/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2102 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/examples/gss_divergent_optima/gss_divergent_optima.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.479611 fwdpy11-0.9.0/examples/plugin/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      954 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/examples/plugin/CMakeLists.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      680 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/examples/plugin/gvalue_recorder.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      642 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/examples/plugin/test_plugin.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.479611 fwdpy11-0.9.0/examples/python_genetic_values/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3865 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/examples/python_genetic_values/pysnowdrift.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.479611 fwdpy11-0.9.0/examples/tskit/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6357 2020-04-19 00:00:10.000000 fwdpy11-0.9.0/examples/tskit/precapitate.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6325 2020-04-19 00:00:10.000000 fwdpy11-0.9.0/examples/tskit/recapitate.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      253 2020-04-19 00:17:34.000000 fwdpy11-0.9.0/examples/tskit/session.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.479611 fwdpy11-0.9.0/fwdpy11/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5078 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/CMakeLists.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2386 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2239 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/__main__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1172 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/_demography.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1368 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/_dev.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2675 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/_evolve_genomes.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6590 2020-07-11 18:11:18.000000 fwdpy11-0.9.0/fwdpy11/_evolvets.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.483611 fwdpy11-0.9.0/fwdpy11/_monkeypatch/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/_monkeypatch/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2637 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/_monkeypatch/_data_matrix.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9150 2020-07-08 17:43:29.000000 fwdpy11-0.9.0/fwdpy11/_monkeypatch/_diploid_population.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9398 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/_monkeypatch/_table_collection.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.483611 fwdpy11-0.9.0/fwdpy11/_types/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/_types/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    23627 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/fwdpy11/_types/demography_debugger.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11420 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/_types/model_params.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      116 2020-08-04 22:24:27.000000 fwdpy11-0.9.0/fwdpy11/_version.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3354 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/class_decorators.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      857 2020-07-17 03:30:29.000000 fwdpy11-0.9.0/fwdpy11/custom_genetic_value_decorators.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.483611 fwdpy11-0.9.0/fwdpy11/demographic_models/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5986 2020-07-23 20:45:18.000000 fwdpy11-0.9.0/fwdpy11/demographic_models/IM.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      139 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/demographic_models/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2949 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/demographic_models/demographic_model_details.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    14354 2020-07-31 17:31:54.000000 fwdpy11-0.9.0/fwdpy11/demographic_models/human.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16248 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/discrete_demography.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2157 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/ezparams.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6470 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/genetic_map_unit.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17759 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/fwdpy11/genetic_values.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.451611 fwdpy11-0.9.0/fwdpy11/headers/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.451611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.487611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8531 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/K_linked_regions_extensions.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      781 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/calculate_fitnesses.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      684 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/common_ind.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1711 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/confirm_mutation_counts.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2180 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/custom_diploid.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6898 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/custom_mutation.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5167 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/diploid_fixed_sh_ind.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7885 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/diploid_ind.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17455 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/edge_buffering.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4222 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/evolve_generation_ts.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12527 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/juvenile_migration.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1440 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/load_table_collection.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3710 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/simplify_tables.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    18684 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2393 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      638 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_types.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.487611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/unused_source/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1491 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2430 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing_with_mutation.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    22549 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/wfevolvets.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1148 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/wfevolvets.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16057 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/wfts_integration_test.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.491611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4082 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/GSLrng_t.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.491611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/algorithm/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3422 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/algorithm/compact_mutations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9973 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/data_matrix.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4457 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/debug.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1497 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/diploid.hh
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      994 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/diploid_population.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.491611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/extensions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6158 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/extensions/callbacks.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10022 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/extensions/regions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    30609 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/fitness_models.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7029 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/forward_types.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3043 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/forward_types_serialization.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1474 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/fwd_functional.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.491611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1694 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_interval.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1376 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_point.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1617 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/fixed_number_crossovers.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1277 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/genetic_map.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      492 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/genetic_map_unit.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1741 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_interval.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1388 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_point.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.491611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/gsl/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      360 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/gsl/deleter.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      472 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/gsl/tags.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      756 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/gsl_discrete.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      655 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/insertion_policies.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8633 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/data_matrix_details.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8416 2020-06-09 01:40:02.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/debug_details.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    21068 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/haploid_genome_cleaner.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2122 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/mutation_internal.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1596 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/rec_gamete_updater.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2189 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/recombination_common.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1490 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/sample_diploid_helpers.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1475 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/sampling_functions_details.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10765 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/type_traits.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      487 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/util.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      444 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/void_t.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/detail/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2970 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/detail/serialize_population.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5816 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/diploid.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3459 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/haploid_genome.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3678 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/mutation.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1933 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/scalar_serialization.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1100 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/serialize_population.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/meta/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      249 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/meta/always_false.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    20755 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/mutate_recombine.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6023 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/popgenmut.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2960 2020-05-14 19:25:52.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/diploid_population.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6725 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/popbase.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      545 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/tags.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      453 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/recbinder.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5754 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12829 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.tcc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1574 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sampling_functions.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/simfunctions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5550 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/simfunctions/recycling.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6666 2020-07-23 18:07:31.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/simparams.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sugar/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13096 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sugar/add_mutation.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3694 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sugar/change_neutral.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.495612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/tags/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      266 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/tags/tags.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.503611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4072 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/count_mutations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3289 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/decapitate.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      642 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/definitions.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.503611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/detail/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4029 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/detail/advance_marginal_tree_policies.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4076 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/detail/generate_data_matrix_details.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1033 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/edge.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1244 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/exceptions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2738 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/generate_data_matrix.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11116 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/generate_offspring.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1125 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/get_parent_ids.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13542 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.503611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4950 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/children.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1058 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_order.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2270 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_preorder.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7379 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/nodes.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3541 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/roots.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5426 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/samples.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1162 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/statistics.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      288 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1758 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mark_multiple_roots.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7111 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mutate_tables.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1336 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_record.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      700 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_tools.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      792 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/node.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.503611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6378 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/diploid_offspring.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10144 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/edge_buffer.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1253 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/mutations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      187 2020-06-09 17:03:47.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    15820 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recycling.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4456 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/remove_fixations_from_gametes.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17632 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/serialization.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      505 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/serialization_version.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.503611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/simplification/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    28798 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/simplification/simplification.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      261 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/simplification_flags.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16320 2020-06-22 23:25:50.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/simplify_tables.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      718 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/site.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5407 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/site_visitor.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      558 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/std_table_collection.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9097 2020-06-25 00:20:35.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6526 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection_functions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3233 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/table_simplifier.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    20804 2020-06-25 02:45:36.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/tree_visitor.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4978 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/visit_sites.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9032 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/type_traits.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.507611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      786 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/abstract_cloneable.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2342 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/enum_bitflags.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1449 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/named_type.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7671 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/nested_forward_lists.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1195 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/wrapped_range.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10253 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      258 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/version.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.507611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/src/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      444 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/src/fwdppConfig.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.451611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.507611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3031 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/fwdpp_fixtures.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      202 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/rng_fixture.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       61 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/sugar_fixtures.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2290 2020-05-14 19:25:52.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/sugar_fixtures.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.507611 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      100 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/extensions_integration_tests.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5480 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/extensions_regionsIntegrationTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       95 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/sugar_integration_tests.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1461 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepopTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1180 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepop_custom_diploidTest.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.511612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      356 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/empty_table_collection.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2400 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1061 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1864 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/preorder_adl.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2161 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1612 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_infinite_sites.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2328 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_polytomy.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1399 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_ancestry_list.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2619 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_decapitate.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      794 2020-06-09 01:40:02.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_diploid_recording.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7885 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_edge_buffering_std_table_collection.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2301 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_data_matrix.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2837 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_offspring.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1804 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1278 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree_statistics.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1347 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_node_children_traversal.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      461 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_node_traversal_order_adl.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3512 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_preorder_node_traversal.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1336 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_root_traversal.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2911 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_sample_traversal.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      717 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_site_visitor.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1878 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_table_collection.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7834 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_tree_visitor.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      989 2020-06-06 22:15:39.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_visit_sites.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       98 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tree_sequence_tests.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3045 2020-06-17 21:24:15.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      905 2020-06-17 21:24:15.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12226 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1207 2020-06-17 21:24:15.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection_fxns.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.515612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5220 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/extensions_callbacksTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2317 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/extensions_regionsTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       93 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/extensions_unit_test.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       88 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/fwdpp_unit_tests.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1603 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/gameteTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3324 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/gamete_cleanerTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       90 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/genetic_map_tests.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3082 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/mutateTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      933 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/serializationTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12336 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/siteDepFitnessTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      787 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_GSLrngTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8287 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_add_mutationTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1621 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_change_neutralTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1388 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_popgenmut.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       88 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_unit_tests.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1771 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_enum_bitflags.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8469 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_genetic_map.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6383 2020-05-14 19:25:52.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_mutate_recombine.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1248 2020-06-23 16:58:53.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_nested_forward_lists.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      787 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_recombination.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2079 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_simparams.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      693 2020-06-18 18:46:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_wrapped_range.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6795 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/type_traitsTest.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9201 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/utilTest.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.515612 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/util/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2345 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/util/custom_dip.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4238 2020-05-08 23:04:29.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/util/quick_evolve_sugar.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.519611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.519611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16148 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/DiscreteDemography.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4137 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/MassMigration.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4742 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/MigrationMatrix.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1877 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetDemeSize.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2138 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetExponentialGrowth.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5471 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetMigrationRates.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2139 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetSelfingRate.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1137 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/constants.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2352 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/exceptions.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.523611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16665 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/apply_mass_migrations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5560 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/build_migration_lookup.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3533 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_properties.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2048 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_property_types.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5007 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/demographic_model_state.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1960 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/detail.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11577 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/functions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4335 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/get_max_number_of_demes.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1323 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/migration_lookup.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4187 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/multideme_fitness_lookups.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3826 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/pick_parents.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6287 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/update_demographic_model_state.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1333 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.523611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolve/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5047 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolve/DiploidPopulation_generation.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.523611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2403 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/SampleRecorder.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7797 2020-07-13 19:28:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/evolve_generation_ts.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2668 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/recorders.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1208 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/sample_recorder_types.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6222 2020-06-25 20:24:21.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/simplify_tables.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.523611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_data/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3489 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_data/genetic_value_data.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.523611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_noise/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1432 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_noise/GeneticValueNoise.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1310 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_noise/NoNoise.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.523611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2541 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GSSmo.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1572 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsFitness.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1173 2020-05-28 17:29:52.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1988 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueToFitnessMap.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3635 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/MultivariateGSSmo.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1986 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/Optimum.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2971 2020-07-11 14:43:54.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/PleiotropicOptima.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4114 2020-07-31 15:55:45.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/DiploidGeneticValue.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2689 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/DiploidMultivariateEffectsStrictAdditive.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1167 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/default_update.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1986 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/GBR.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1150 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_GBR.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1331 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_multiplicative.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2777 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/dgvalue_pointer_vector.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/fwdpp_wrappers/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4291 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/fwdpp_wrappers/fwdpp_genetic_value.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/gsl/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      631 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/gsl/gsl_error_handler_wrapper.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/numpy/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2680 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/numpy/array.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/policies/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6027 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/policies/mutation.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2345 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/ConstantS.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1848 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/ExpS.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2150 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/GammaS.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2003 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/GaussianS.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2471 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/LogNormalS.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6104 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/MultivariateGaussianEffects.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2750 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/MutationRegions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2937 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/RecombinationRegions.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1482 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/Region.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2241 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/Sregion.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2127 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/UniformS.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17222 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/mvDES.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1074 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/rng.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1069 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/samplers.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.527611 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/sampling/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1864 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/sampling/data_matrix_functions.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.531612 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1868 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/Diploid.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3464 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/Mutation.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4032 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/backwards_compat.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2616 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/diploid_metadata.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10977 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7810 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/sim_functions.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.531612 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2263 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/Diploid.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8573 2020-06-29 20:13:19.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/DiploidPopulation.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3560 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/Mutation.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10551 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/Population.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      456 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/typedefs.hpp
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.531612 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/util/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2135 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/util/array_proxy.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      923 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/util/clone_cloneable.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      657 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/util/convert_lists.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    18884 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/regions.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.531612 fwdpy11-0.9.0/fwdpy11/src/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2332 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/_fwdpy11.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.531612 fwdpy11-0.9.0/fwdpy11/src/array_proxies/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1283 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/array_proxies/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.535611 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9726 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/DiscreteDemography.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1655 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/MassMigration.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1640 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/MigrationMatrix.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1291 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetDemeSize.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1212 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetExponentialGrowth.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1400 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetMigrationRates.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1169 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetSelfingRate.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1168 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/exceptions.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1653 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/discrete_demography/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.539611 fwdpy11-0.9.0/fwdpy11/src/evolve_population/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      755 2020-06-07 03:09:23.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/cleanup_metadata.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      393 2020-06-07 03:09:23.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/cleanup_metadata.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3491 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/diploid_pop_fitness.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1213 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/diploid_pop_fitness.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      917 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/index_and_count_mutations.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      323 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/index_and_count_mutations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      395 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/init.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      243 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/no_stopping.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7648 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/no_tree_sequences.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2045 2020-06-29 20:13:19.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/remove_extinct_genomes.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      220 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/remove_extinct_genomes.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3604 2020-06-29 20:13:19.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/remove_extinct_mutations.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      222 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/remove_extinct_mutations.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1400 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/track_ancestral_counts.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      500 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/track_ancestral_counts.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2021 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/track_mutation_counts.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      330 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/track_mutation_counts.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      957 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/util.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      489 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/util.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    28220 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/evolve_population/with_tree_sequences.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.539611 fwdpy11-0.9.0/fwdpy11/src/fwdpp_functions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6160 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_functions/data_matrix_creation.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      210 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_functions/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.539611 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      434 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/BinomialInterval.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      354 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/BinomialPoint.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7628 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/DataMatrix.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1867 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/Edge.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1026 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/EdgeTable.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      383 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/FixedCrossovers.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      651 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/GeneticMapUnit.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2210 2020-07-24 21:54:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/HaploidGenome.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      769 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/MutationBase.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2879 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/MutationRecord.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1136 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/MutationTable.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      217 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/NULL_NODE.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1455 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/Node.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1047 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/NodeTable.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      357 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/PoissonInterval.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      313 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/PoissonPoint.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1343 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/Site.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1046 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/SiteTable.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4013 2020-06-07 03:09:23.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/TableCollection.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1983 2020-06-23 18:30:05.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.543611 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_functions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3908 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_functions/change_effect_size.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      261 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_functions/init.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2091 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_functions/sort_gamete_keys.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.543611 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1551 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidGenotype.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4708 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidMetadata.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16131 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidPopulation.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2936 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidVector.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1798 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/HaploidGenomeVector.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5421 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/Mutation.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1814 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/MutationVector.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11087 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/PopulationBase.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      402 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/RecordNothing.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1161 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/get_individuals.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      855 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/init.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      441 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/rng.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4003 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/ts_from_tskit.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2680 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/tsrecorders.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.543611 fwdpy11-0.9.0/fwdpy11/src/genetic_value_noise/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      981 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_noise/GaussianNoise.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2876 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_noise/GeneticValueNoise.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      253 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_noise/NoNoise.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      305 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_noise/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.547611 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      343 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/GSSmo.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      706 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/GeneticValueIsFitness.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3158 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/GeneticValueIsTrait.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1245 2020-07-11 15:11:08.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/GeneticValueToFitnessMap.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      441 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/MultivariateGSSmo.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1318 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/Optimum.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1514 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/PleiotropicOptima.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      683 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.547611 fwdpy11-0.9.0/fwdpy11/src/genetic_values/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3414 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/Additive.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2069 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/DiploidGeneticValue.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      874 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/DiploidMultivariateEffectsStrictAdditive.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4106 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/GBR.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3758 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/Multiplicative.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6837 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/PyDiploidGeneticValue.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1076 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/dgvalue_pointer_vector.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      787 2020-07-16 20:11:58.000000 fwdpy11-0.9.0/fwdpy11/src/genetic_values/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.547611 fwdpy11-0.9.0/fwdpy11/src/gsl/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1943 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/gsl/gsl_random.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      589 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/gsl/init.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.547611 fwdpy11-0.9.0/fwdpy11/src/regions/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      759 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/ConstantS.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      688 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/ExpS.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      766 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/GammaS.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      690 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/GaussianS.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1111 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/LogNormalS.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1291 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/MultivariateGaussianEffects.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1462 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/regions/MutationRegions.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1843 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/regions/RecombinationRegions.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      388 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/Region.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      936 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/Sregion.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      749 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/UniformS.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      834 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/regions/init.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5317 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/fwdpy11/src/regions/mvDES.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.551612 fwdpy11-0.9.0/fwdpy11/src/ts/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    20858 2020-06-23 18:30:05.000000 fwdpy11-0.9.0/fwdpy11/src/ts/DataMatrixIterator.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17567 2020-06-23 18:30:05.000000 fwdpy11-0.9.0/fwdpy11/src/ts/TreeIterator.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9925 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/ts/VariantIterator.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1925 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/ts/count_mutations.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3113 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/ts/data_matrix_from_tables.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2682 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/ts/infinite_sites.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      600 2020-05-08 22:56:22.000000 fwdpy11-0.9.0/fwdpy11/src/ts/init.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      212 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/ts/node_traversal.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      147 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/ts/node_traversal.hpp
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4311 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/fwdpy11/src/ts/simplify.cc
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.551612 fwdpy11-0.9.0/fwdpy11/tskit_tools/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      848 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/fwdpy11/tskit_tools/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      368 2020-06-02 21:30:49.000000 fwdpy11-0.9.0/fwdpy11/tskit_tools/_flags.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.483611 fwdpy11-0.9.0/fwdpy11.egg-info/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12549 2020-08-04 22:24:27.000000 fwdpy11-0.9.0/fwdpy11.egg-info/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    27245 2020-08-04 22:24:31.000000 fwdpy11-0.9.0/fwdpy11.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2020-08-04 22:24:27.000000 fwdpy11-0.9.0/fwdpy11.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2020-03-30 21:43:01.000000 fwdpy11-0.9.0/fwdpy11.egg-info/not-zip-safe
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       48 2020-08-04 22:24:27.000000 fwdpy11-0.9.0/fwdpy11.egg-info/requires.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        8 2020-08-04 22:24:27.000000 fwdpy11-0.9.0/fwdpy11.egg-info/top_level.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      714 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/gplheader.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      732 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/gplheader_cpp.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1306 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/index.md
+-rwxr-xr-x   0 kevin     (1000) kevin     (1000)    13997 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/install-sh
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.551612 fwdpy11-0.9.0/m4/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5036 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/m4/ax_cxx_compile_stdxx_11.m4
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    22072 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/m4/python.m4
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      116 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/readthedocs.yml
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      339 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/requirements.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       38 2020-08-04 22:24:31.567612 fwdpy11-0.9.0/setup.cfg
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7490 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/setup.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.567612 fwdpy11-0.9.0/tests/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3397 2020-07-10 18:45:24.000000 fwdpy11-0.9.0/tests/CMakeLists.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1602 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/EsizeZero.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      540 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/call_Sregion.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1166 2020-04-13 17:46:17.000000 fwdpy11-0.9.0/tests/common_mako.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2032 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/custom_additive.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2043 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/custom_stateless_genotype.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6188 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/discrete_demography_roundtrips.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      670 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/fixation_properties.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      730 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/gsl_error.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2226 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/tests/inherit_noise.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3919 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/ll_snowdrift.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1744 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/numpy_array_interface.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2977 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/pickling_composed_classes.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      664 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/pickling_cpp.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      375 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/poptools.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1262 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/pyadditive.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1525 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/pyadditivegss.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2079 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/pygss.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1171 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/pynoise.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2554 2020-06-02 21:30:49.000000 fwdpy11-0.9.0/tests/quick_pops.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1341 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/tests/snowdrift.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      991 2020-04-17 19:30:58.000000 fwdpy11-0.9.0/tests/sregion_cdf.cc
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      710 2020-07-17 03:30:29.000000 fwdpy11-0.9.0/tests/testMultivariateGSSmo.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5078 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_DataMatrix.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7449 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/tests/test_DemographyDebugger.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4934 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_DiploidPopulation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      532 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_GSLerror.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4445 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_ModelParams.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2056 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/tests/test_Mutation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      640 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_SampleRecorder.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3403 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_Sregion_from_cdf.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     8676 2020-04-17 18:19:05.000000 fwdpy11-0.9.0/tests/test_TableCollection_fs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6945 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_add_mutation.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      706 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_binary_format_compatibility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1574 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/tests/test_class_decorators.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1507 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_custom_exceptions.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1881 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_custom_stateless_fitness.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    20967 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/tests/test_demographic_event_verbs.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8509 2020-07-08 17:43:29.000000 fwdpy11-0.9.0/tests/test_demographic_models.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1356 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/tests/test_dgvalue_pointer_vector.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    37078 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_discrete_demography.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    34274 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_discrete_demography_with_tree_sequences.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4930 2020-06-02 21:30:49.000000 fwdpy11-0.9.0/tests/test_fixation_properties.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      813 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_fwdpp_types.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1864 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_genetic_value_noise.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3227 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_genetic_value_to_fitness.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5812 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/tests/test_genetic_values.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1806 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/tests/test_inherited_noise.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3249 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_multivariate_effects.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      594 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_mutation_labels.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1650 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/tests/test_numpy.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1415 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_numpy_array_interface.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2785 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_opaque.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6793 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/tests/test_pickling.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      485 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_pickling_composed_classes.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6258 2020-07-31 15:55:38.000000 fwdpy11-0.9.0/tests/test_python_genetic_values.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    14259 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_record_genetic_value_matrix.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    15446 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_regions.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1868 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_simple_parallel.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2625 2020-07-27 15:27:22.000000 fwdpy11-0.9.0/tests/test_stateful_fitness.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1122 2020-04-23 19:14:24.000000 fwdpy11-0.9.0/tests/test_stopping_criterion.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    62706 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/tests/test_tree_sequences.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13049 2020-07-10 17:54:56.000000 fwdpy11-0.9.0/tests/test_tree_sequences_different_des_in_different_demes.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2616 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_tree_sequences_esize_zero_selected_variants.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5563 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/tests/test_tree_sequences_with_neutral_mutations.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3125 2020-04-17 18:19:05.000000 fwdpy11-0.9.0/tests/test_ts_from_msprime.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3997 2020-04-17 18:23:29.000000 fwdpy11-0.9.0/tests/test_util.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1418 2020-06-02 21:30:49.000000 fwdpy11-0.9.0/tests/test_wright_fisher.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2020-06-04 19:54:21.000000 fwdpy11-0.9.0/tests/throw_custom_exceptions.cc
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   645031 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/tests/v045.bin
+-rw-r--r--   0 kevin     (1000) kevin     (1000)   139100 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/tests/v045.lzma
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2020-08-04 22:24:31.567612 fwdpy11-0.9.0/travis_scripts/
+-rwxrwxr-x   0 kevin     (1000) kevin     (1000)     2287 2020-06-06 22:25:38.000000 fwdpy11-0.9.0/travis_scripts/build_script.sh
+-rwxr-xr-x   0 kevin     (1000) kevin     (1000)      198 2020-03-22 23:26:04.000000 fwdpy11-0.9.0/travis_scripts/gsl2.sh
+-rwxrwxr-x   0 kevin     (1000) kevin     (1000)     2046 2020-06-23 18:29:32.000000 fwdpy11-0.9.0/travis_scripts/installation_script.sh
```

### Comparing `fwdpy11-0.8.3/.circleci/config.yml` & `fwdpy11-0.9.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/.travis.yml` & `fwdpy11-0.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/.ycm_extra_conf.py` & `fwdpy11-0.9.0/.ycm_extra_conf.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/CMakeLists.txt` & `fwdpy11-0.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/COPYING` & `fwdpy11-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/MANIFEST.in` & `fwdpy11-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/PKG-INFO` & `fwdpy11-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdpy11
-Version: 0.8.3
+Version: 0.9.0
 Summary: Forward-time population genetic simulation in Python
 Home-page: http://molpopgen.github.io/fwdpy11
 Author: Kevin Thornton
 Author-email: krthornt@uci.edu
 License: GNU GPLv3+
 Description: fwdpy11
         *************************
```

### Comparing `fwdpy11-0.8.3/README.rst` & `fwdpy11-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/Makefile` & `fwdpy11-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/_build/html/_images/localadaptation.png` & `fwdpy11-0.9.0/doc/_build/html/_images/localadaptation.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/_build/html/_images/migtest.png` & `fwdpy11-0.9.0/doc/_build/html/_images/migtest.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/_build/html/_images/moments_IM_gamma_minus_5.png` & `fwdpy11-0.9.0/doc/_build/html/_images/moments_IM_gamma_minus_5.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/_build/html/_images/moments_IM_neutral.png` & `fwdpy11-0.9.0/doc/_build/html/_images/moments_IM_neutral.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/_build/html/_images/tables.png` & `fwdpy11-0.9.0/doc/_build/html/_images/tables.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/_build/html/_images/tree.png` & `fwdpy11-0.9.0/doc/_build/html/_images/tree.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/conf.py` & `fwdpy11-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/IM.rst` & `fwdpy11-0.9.0/doc/examples/IM.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/gss.rst` & `fwdpy11-0.9.0/doc/examples/gss.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/gss_divergent_optima.rst` & `fwdpy11-0.9.0/doc/examples/gss_divergent_optima.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/localadaptation.rst` & `fwdpy11-0.9.0/doc/examples/localadaptation.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/migtest.rst` & `fwdpy11-0.9.0/doc/examples/migtest.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/precapitation.rst` & `fwdpy11-0.9.0/doc/examples/precapitation.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/recapitation.rst` & `fwdpy11-0.9.0/doc/examples/recapitation.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/examples/recorder.rst` & `fwdpy11-0.9.0/doc/examples/recorder.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/fwdpp.doxygen` & `fwdpy11-0.9.0/doc/fwdpp.doxygen`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/fwdpy11.doxygen` & `fwdpy11-0.9.0/doc/fwdpy11.doxygen`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/localadaptation.png` & `fwdpy11-0.9.0/doc/images/localadaptation.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/migtest.png` & `fwdpy11-0.9.0/doc/images/migtest.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/moments_IM_gamma_minus_5.png` & `fwdpy11-0.9.0/doc/images/moments_IM_gamma_minus_5.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/moments_IM_neutral.png` & `fwdpy11-0.9.0/doc/images/moments_IM_neutral.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/structures.dot` & `fwdpy11-0.9.0/doc/images/structures.dot`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/structures.png` & `fwdpy11-0.9.0/doc/images/structures.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/tables.dot` & `fwdpy11-0.9.0/doc/images/tables.dot`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/tables.png` & `fwdpy11-0.9.0/doc/images/tables.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/images/tree.png` & `fwdpy11-0.9.0/doc/images/tree.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/index.rst` & `fwdpy11-0.9.0/doc/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,38 +14,43 @@
     :maxdepth: 1
 
     misc/changelog
     misc/upgrade_path
     misc/deprecated
     misc/pubs
     misc/developersguide
-    misc/writingplugins
 
 .. toctree::
     :caption: Concepts
     :maxdepth: 2
 
     pages/definitions
 
 .. toctree::
     :caption: Tutorials
 
     pages/tutorial.rst
-    pages/advancedtopics.rst
+    pages/advancedtopics
 
 .. toctree::
     :caption: Objects and concepts
 
     pages/softselection
     pages/mvdes
     pages/tsoverview
     pages/tstypes
     pages/tablefs.rst
     pages/recorders
 
+.. toctree::
+    :caption: Technical details
+
+    technical/genetic_values
+    technical/writingplugins
+
 
 .. toctree::
     :caption: Data types and functions
     :maxdepth: 2
 
     pages/types
     pages/genetic_values
@@ -53,30 +58,31 @@
     pages/gvaluenoise
     pages/regiontypes
     pages/datamatrix
     pages/model_params
     pages/functions
     pages/demographic_models
     pages/tskit_tools
+    pages/gslrandom.rst
 
 .. toctree::
     :caption: References
     :maxdepth: 1
 
     misc/references
 
 .. toctree::
     :caption: Examples
 
     examples/bgs
     examples/gss
-    examples/snowdrift
     examples/recorder
     examples/migtest
     examples/localadaptation
     examples/IM
     examples/gss_divergent_optima
     examples/precapitation
     examples/recapitation
+    examples/pysnowdrift
 
 .. todolist::
```

### Comparing `fwdpy11-0.8.3/doc/misc/changelog.rst` & `fwdpy11-0.9.0/doc/misc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Changelog
 ====================================================================================
 
 Major changes are listed below.  Each release likely contains fiddling with back-end code,
 updates to latest `fwdpp` version, etc.
 
+0.9.0
+****************************************
+
+This release enables custom genetic value models to be implemented in Python.
+To do so, the back-end for C++ genetic values was changed in a way that (hopefully!)
+future-proofs the API against future changes.  The approach taken to allowing
+Python genetic value types evolved quite a bit during development, so we won't
+refer to individual pull requests here.  Anyone interested can look at the 0.9.0
+milestone on GitHub.
+
+See :ref:`here <gvalues_python>` for the documentation on Python genetic values.
+
+
 0.8.3
 ****************************************
 
 * :func:`fwdpy11.DiploidPopulation.dump_tables_to_tskit` now populates
   the provenance table. :pr:`542`
 * Improve checking migration rates in :class:`fwdpy11.DemographyDebugger`. :pr:`545`
 * :class:`fwdpy11.DemographyDebugger` now makes a deep copy of input. :pr:`546`
```

### Comparing `fwdpy11-0.8.3/doc/misc/developersguide.rst` & `fwdpy11-0.9.0/doc/misc/developersguide.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/misc/pubs.rst` & `fwdpy11-0.9.0/doc/misc/pubs.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/misc/references.rst` & `fwdpy11-0.9.0/doc/misc/references.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 .. [Burger2000] Bürger, R. 2000. The Mathematical Theory of Selection, Recombination, and Mutation. Wiley.
 
 .. [Christiansen1974] Christiansen, Freddy Bugge. 1974. “Sufficient Conditions for Protected Polymorphism in a Subdivided Population.” The American Naturalist 108 (960): 157–66. DOI:10.1086/282896
 
 .. [Christiansen1975] Christiansen, Freddy Bugge. 1975. “Hard and Soft Selection in a Subdivided Population.” The American Naturalist 109 (965): 11–16. DOI:10.1086/282970
 
+.. [Doebeli2004] Doebeli, Michael, Christoph Hauert, and Timothy Killingback. 2004. “The Evolutionary Origin of Cooperators and Defectors.” Science 306 (5697): 859–62.
+
 .. [EyreWalker2010] Eyre-Walker, Adam. 2010. “Evolution in Health and Medicine Sackler Colloquium: Genetic Architecture of a Complex Trait and Its Implications for Fitness and Genome-Wide Association Studies.” Proceedings of the National Academy of Sciences of the United States of America 107 Suppl 1 (January): 1752–56.
 
 .. [Felsenstein1976] Felsenstein, J. 1976. “The Theoretical Population Genetics of Variable Selection and Migration.” Annual Review of Genetics 10: 253–80. DOI:10.1146/annurev.ge.10.120176.001345
 
 .. [Haller2019] Haller, B. C., J. Galloway, and J. Kelleher. 2019. “Tree‐sequence Recording in SLiM Opens New Horizons for Forward‐time Simulation of Whole Genomes.” Molecular Ecology. https://onlinelibrary.wiley.com/doi/abs/10.1111/1755-0998.12968. DOI:10.1111/1755-0998.12968
 
 .. [HillKeightley1988] Hill, W. G., and P. D. Keightley. 1988. “Interrelations of Mutation, Population Size, Artificial and Natural Selection.” In Proceedings of the Second International Conference on Quantitative Genetics, 57–70. Sinauer Sunderland, MA.
```

### Comparing `fwdpy11-0.8.3/doc/misc/upgrade_path.rst` & `fwdpy11-0.9.0/doc/misc/upgrade_path.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/misc/writingplugins.rst` & `fwdpy11-0.9.0/doc/technical/writingplugins.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,84 @@
 .. _writingplugins:
 
-Writing "plugins" using C++
+Writing "plugins" with C++
 ====================================================================================
 
-New functionality may be added through new Python code and/or new C++ code.  Further, you may use the existing C++ types
-in Python extensions depending on fwdpy11.  For example, you could write a custom "evolve" function for
-non-Wright-Fisher models.  Or, you could write custom genetic value objects.  There are several examples
-of custom genetic value objects in the unit tests.
+New functionality may be added through new Python code and/or new C++ code.
+Further, you may use the existing C++ types in Python extensions depending on
+``fwdpy11``.  For example, you could write a custom "evolve" function for
+non-Wright-Fisher models.  Or, you could write custom genetic value objects.
+There are several examples of custom genetic value objects in the unit tests.
 
 Finding the headers
 ---------------------------------------
 
-You can find the location of the installed header files programatically within Python:
+You can find the location of the installed header files using Python:
 
 .. ipython:: python
 
     import fwdpy11
 
     print(fwdpy11.get_includes())
     print(fwdpy11.get_fwdpp_includes())
 
-The above is useful for generating a functioning `setup.py` file.  Note that you will have to join the output with the
-proper compiler flags indicating include paths (typically `-I`).
+The above is useful for generating a functioning `setup.py` file.  Note that you will have
+to join the output with the proper compiler flags indicating include paths (typically `-I`).
 
 If using a `Makefile`, it is handy to get the above info via the shell, which is done as follows:
 
 .. code-block:: bash
 
-    python3 -m fwdpy11 --includes
+    python3 -m ``fwdpy11`` --includes
 
-The above command prepends the paths with `-I`.  If that is not desired, you may get the paths separately for fwdpp and
-fdwpy11:
+The above command prepends the paths with `-I`.  If that is not desired,
+you may get the paths separately for ``fwdpp`` and ``fwdpy11``:
 
 .. code-block:: bash
 
-    python3 -m fwdpy11 --fwdpp_headers
-    python3 -m fwdpy11 --fwdpy11_headers
+    python3 -m ``fwdpy11`` --fwdpp_headers
+    python3 -m ``fwdpy11`` --fwdpy11_headers
 
-The above two commands are useful when using tools like `cmake` to configure build systems.  Here is an example
-from one of the examples that comes with `fwdpy11`:
+Building with ``cmake``
+------------------------------------------
+
+The above two commands are useful when using tools like ``cmake`` to configure build systems.  Here is an example
+from one of the examples that comes with ``fwdpy11``:
 
 .. literalinclude:: ../../examples/plugin/CMakeLists.txt
 
 Mako headers for cppimport
 ------------------------------------------
 
-Extensions using cppimport_ require "mako" headers to guide compilation.  You make get a minimal header via the shell:
+Extensions using cppimport_ require ``mako`` headers to guide compilation.  You make get a minimal header via the shell:
 
 .. code-block:: bash
 
-    python3 -m fwdpy11 --mako
+    python3 -m ``fwdpy11`` --mako
 
 .. _cppimport: https://github.com/tbenthompson/cppimport
 
 
-Dealing with GSL errors in custom C++ code
+Dealing with ``GSL`` errors in custom C++ code
 ----------------------------------------------------------------------------------
 
-The GSL uses C-like error handling.  Here, this means that there is a global error handling function
+The ``GSL`` uses C-like error handling.  Here, this means that there is a global error handling function
 that will print the error to screen and then abort the running process.  The behavior of abort-on-error is not
 acceptable here, as the Python session itself will abort! 
 
-When fwpdy11 is imported, the default GSL behavior changes.  Instead of aborting, a `RuntimeError` will be raised.
-This exception will contain the entire string of text from the GSL error message.
+When ``fwdpy11`` is imported, the default ``GSL`` behavior changes.  Instead of aborting, a `RuntimeError` will be raised.
+This exception will contain the entire string of text from the ``GSL`` error message.
 
-However, if you write and C++ code using the GSL, you may wish to handle errors locally and maybe return `None` or throw
+However, if you write and C++ code using the ``GSL``, you may wish to handle errors locally and maybe return `None` or throw
 an exception with your own message in it.  To do so, you must do the following in your C++ code:
 
-1. Temporarily disable GSL error handling.
-2. Restore the fwdpy11 error handler at all possible exit paths from your code.
+1. Temporarily disable ``GSL`` error handling.
+2. Restore the ``fwdpy11`` error handler at all possible exit paths from your code.
 
-On paper, one could do all of the above using the C API found in the GSL.  However, fwdpy11 provides a class that
+On paper, one could do all of the above using the C API found in the ``GSL``.  However, ``fwdpy11`` provides a class that
 provides an idiomatic C++ approach to managing the error handler.  The C++ class `fwdpy11::gsl_error_handler_wrapper`,
 defined in `<fwdpy11/gsl/gsl_error_handler_wrapper.hpp>` provide a "smart pointer"-like wrapper around the error
 handler. The constructor disables the error handler, storing the value of the disabled handler.  The destructor restores
 the handler.
 
 To see this in action, check out the unit test file `tests/test_GSLerror.py` and its associated C++ file
 `tests/gsl_error.cc`.
```

### Comparing `fwdpy11-0.8.3/doc/pages/definitions.rst` & `fwdpy11-0.9.0/doc/pages/definitions.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/demographic_models.rst` & `fwdpy11-0.9.0/doc/pages/demographic_models.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/functions.rst` & `fwdpy11-0.9.0/doc/pages/functions.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/genetic_values.rst` & `fwdpy11-0.9.0/doc/pages/genetic_values.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/gvalue_to_fitness.rst` & `fwdpy11-0.9.0/doc/pages/gvalue_to_fitness.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/mvdes.rst` & `fwdpy11-0.9.0/doc/pages/mvdes.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/recorders.rst` & `fwdpy11-0.9.0/doc/pages/recorders.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/regiontypes.rst` & `fwdpy11-0.9.0/doc/pages/regiontypes.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/softselection.rst` & `fwdpy11-0.9.0/doc/pages/softselection.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/tablefs.rst` & `fwdpy11-0.9.0/doc/pages/tablefs.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/tskit_tools.rst` & `fwdpy11-0.9.0/doc/pages/tskit_tools.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/tsoverview.rst` & `fwdpy11-0.9.0/doc/pages/tsoverview.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/tstypes.rst` & `fwdpy11-0.9.0/doc/pages/tstypes.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/tutorial.rst` & `fwdpy11-0.9.0/doc/pages/tutorial.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/pages/types.rst` & `fwdpy11-0.9.0/doc/pages/types.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/savefig/efficient_timeseries_example.png` & `fwdpy11-0.9.0/doc/savefig/efficient_timeseries_example.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/savefig/gss_two_deme_effect_sizes.png` & `fwdpy11-0.9.0/doc/savefig/gss_two_deme_effect_sizes.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/savefig/mean_genetic_values_over_time.png` & `fwdpy11-0.9.0/doc/savefig/mean_genetic_values_over_time.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/savefig/pi_over_time.png` & `fwdpy11-0.9.0/doc/savefig/pi_over_time.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/savefig/sfs_example.png` & `fwdpy11-0.9.0/doc/savefig/sfs_example.png`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/0000a_anintroexample.rst` & `fwdpy11-0.9.0/doc/unused_pages/0000a_anintroexample.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/0000a_objectoverview.rst` & `fwdpy11-0.9.0/doc/unused_pages/0000a_objectoverview.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/0000a_tskit_interchange.rst` & `fwdpy11-0.9.0/doc/unused_pages/0000a_tskit_interchange.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/0000a_working_with_genotypes_trees.rst` & `fwdpy11-0.9.0/doc/unused_pages/0000a_working_with_genotypes_trees.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/mutation.rst` & `fwdpy11-0.9.0/doc/unused_pages/mutation.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/recombination.rst` & `fwdpy11-0.9.0/doc/unused_pages/recombination.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/doc/unused_pages/tstimeseries.rst` & `fwdpy11-0.9.0/doc/unused_pages/tstimeseries.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/COPYING` & `fwdpy11-0.9.0/examples/COPYING`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/README.rst` & `fwdpy11-0.9.0/examples/README.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/bgs/bgs.py` & `fwdpy11-0.9.0/examples/bgs/bgs.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/discrete_demography/IM.py` & `fwdpy11-0.9.0/examples/discrete_demography/IM.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/discrete_demography/localadaptation.py` & `fwdpy11-0.9.0/examples/discrete_demography/localadaptation.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/discrete_demography/migtest.py` & `fwdpy11-0.9.0/examples/discrete_demography/migtest.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss/DiploidPopulationGSSmo.py` & `fwdpy11-0.9.0/examples/gss/DiploidPopulationGSSmo.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss/Makefile` & `fwdpy11-0.9.0/examples/gss/Makefile`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss/README.rst` & `fwdpy11-0.9.0/examples/gss/README.rst`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss/iterate_variants_in_tree_sequences.py` & `fwdpy11-0.9.0/examples/gss/iterate_variants_in_tree_sequences.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss/plot_genetic_values_from_tree_sequences.py` & `fwdpy11-0.9.0/examples/gss/plot_genetic_values_from_tree_sequences.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss/plotstats.R` & `fwdpy11-0.9.0/examples/gss/plotstats.R`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/gss_divergent_optima/gss_divergent_optima.py` & `fwdpy11-0.9.0/examples/gss_divergent_optima/gss_divergent_optima.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/plugin/CMakeLists.txt` & `fwdpy11-0.9.0/examples/plugin/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 cmake_minimum_required(VERSION 2.8.12)
 project(gavlue_recorder)
 
 # As of 0.8.0, fwdpy11
-# is compiled with the C++15 language
+# is compiled with the C++14 language
 # standard (-std=c++14)
 set(CMAKE_CXX_EXTENSIONS OFF)
 set(CMAKE_CXX_STANDARD 14) 
 find_package(pybind11)
 message(STATUS "Found pybind11: ${pybind11_VERSION}")
-if(${pybind11_VERSION} VERSION_LESS '2.2.3')
-    message(FATAL_ERROR "pybind11 version must be >= '2.2.3'")
+if(${pybind11_VERSION} VERSION_LESS '2.4.3')
+    message(FATAL_ERROR "pybind11 version must be >= '2.4.3'")
 endif()
 
 execute_process(COMMAND python3 -m fwdpy11 --fwdpy11_headers OUTPUT_VARIABLE FP11HEADERS)
 execute_process(COMMAND python3 -m fwdpy11 --fwdpp_headers OUTPUT_VARIABLE FWDPPHEADERS)
 
 find_package(GSL REQUIRED)
 include_directories(BEFORE ${FP11HEADERS} ${FWDPPHEADERS})
```

### Comparing `fwdpy11-0.8.3/examples/plugin/gvalue_recorder.cc` & `fwdpy11-0.9.0/examples/plugin/gvalue_recorder.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/plugin/test_plugin.py` & `fwdpy11-0.9.0/examples/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/tskit/precapitate.py` & `fwdpy11-0.9.0/examples/tskit/precapitate.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/examples/tskit/recapitate.py` & `fwdpy11-0.9.0/examples/tskit/recapitate.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/CMakeLists.txt` & `fwdpy11-0.9.0/fwdpy11/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     src/regions/LogNormalS.cc)
 
 set(GSL_SOURCES src/gsl/init.cc
     src/gsl/gsl_random.cc)
 
 set(GENETIC_VALUE_SOURCES src/genetic_values/init.cc
     src/genetic_values/DiploidGeneticValue.cc
+    src/genetic_values/PyDiploidGeneticValue.cc
     src/genetic_values/Additive.cc
     src/genetic_values/Multiplicative.cc
     src/genetic_values/GBR.cc
     src/genetic_values/DiploidMultivariateEffectsStrictAdditive.cc
     src/genetic_values/dgvalue_pointer_vector.cc)
 
 set(GENETIC_VALUE_TO_FITNESS_SOURCES
@@ -101,26 +102,29 @@
     src/discrete_demography/SetDemeSize.cc
     src/discrete_demography/SetExponentialGrowth.cc
     src/discrete_demography/SetSelfingRate.cc
     src/discrete_demography/SetMigrationRates.cc
     src/discrete_demography/DiscreteDemography.cc
     src/discrete_demography/exceptions.cc)
 
+set (ARRAY_PROXY_SOURCES src/array_proxies/init.cc)
+
 set(ALL_SOURCES ${FWDPP_TYPES_SOURCES}
     ${FWDPP_FUNCTIONS_SOURCES}
     ${FWDPY11_TYPES_SOURCES}
     ${FWDPY11_FUNCTIONS_SOURCES}
     ${REGION_SOURCES}
     ${GENETIC_VALUE_NOISE_SOURCES}
     ${GENETIC_VALUE_TO_FITNESS_SOURCES}
     ${GENETIC_VALUE_SOURCES}
     ${TS_SOURCES}
     ${GSL_SOURCES}
     ${EVOLVE_POPULATION_SOURCES}
-    ${DISCRETE_DEMOGRAPHY_SOURCES})
+    ${DISCRETE_DEMOGRAPHY_SOURCES}
+    ${ARRAY_PROXY_SOURCES})
 
 set(LTO_OPTIONS)
 if(ENABLE_PROFILING OR DISABLE_LTO)
     set(LTO_OPTIONS NO_EXTRAS)
 endif()
 # These are the main modules
 pybind11_add_module(_fwdpy11 MODULE ${LTO_OPTIONS} src/_fwdpy11.cc ${ALL_SOURCES})
```

### Comparing `fwdpy11-0.8.3/fwdpy11/__init__.py` & `fwdpy11-0.9.0/fwdpy11/__init__.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/__main__.py` & `fwdpy11-0.9.0/fwdpy11/__main__.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_demography.py` & `fwdpy11-0.9.0/fwdpy11/_demography.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_dev.py` & `fwdpy11-0.9.0/fwdpy11/_dev.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_evolve_genomes.py` & `fwdpy11-0.9.0/fwdpy11/_evolve_genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
         Update to refactored ModelParams
     """
     import warnings
 
     # warnings.simplefilter("default")
     warnings.warn(
-        "Simulation without tree sequences is being considered for deprecation!",
-        PendingDeprecationWarning,
+        "Simulation without tree sequences is deprecated", DeprecationWarning,
     )
 
     from ._fwdpy11 import MutationRegions
     from ._fwdpy11 import evolve_without_tree_sequences
     from ._fwdpy11 import dispatch_create_GeneticMap
 
     pneutral = 0.0
```

### Comparing `fwdpy11-0.8.3/fwdpy11/_evolvets.py` & `fwdpy11-0.9.0/fwdpy11/_evolvets.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_monkeypatch/_data_matrix.py` & `fwdpy11-0.9.0/fwdpy11/_monkeypatch/_data_matrix.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_monkeypatch/_diploid_population.py` & `fwdpy11-0.9.0/fwdpy11/_monkeypatch/_diploid_population.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_monkeypatch/_table_collection.py` & `fwdpy11-0.9.0/fwdpy11/_monkeypatch/_table_collection.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_types/demography_debugger.py` & `fwdpy11-0.9.0/fwdpy11/_types/demography_debugger.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/_types/model_params.py` & `fwdpy11-0.9.0/fwdpy11/_types/model_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,17 +204,17 @@
         if isinstance(
             self.demography, fwdpy11.demographic_models.DemographicModelDetails
         ):
             return None
 
         # Otherwise, assume that it is a numpy array
         warnings.warn(
-            "attribute popsizes is being considered for"
-            " deprecation (along with simulations without tree sequences)",
-            PendingDeprecationWarning,
+            "attribute popsizes is deprecated"
+            " and will be removed in a future release.",
+            DeprecationWarning,
         )
         return self.demography
 
     @nregions.validator
     def validate_nregions(self, attribute, value):
         for i in value:
             attr.validators.instance_of(fwdpy11.Region)(self, attribute, i)
@@ -307,11 +307,11 @@
                 f"{len(self.popsizes)} instead"
             )
 
     @pself.validator
     def validate_pself(self, attribute, value):
         if value != 0.0:
             warnings.warn(
-                "attribute pself is being considered for"
-                " deprecation (along with simulations without tree sequences)",
-                PendingDeprecationWarning,
+                "attribute pself is deprecated"
+                " and will be removed in a future version",
+                DeprecationWarning,
             )
```

### Comparing `fwdpy11-0.8.3/fwdpy11/class_decorators.py` & `fwdpy11-0.9.0/fwdpy11/class_decorators.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/demographic_models/IM.py` & `fwdpy11-0.9.0/fwdpy11/demographic_models/IM.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/demographic_models/demographic_model_details.py` & `fwdpy11-0.9.0/fwdpy11/demographic_models/demographic_model_details.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/demographic_models/human.py` & `fwdpy11-0.9.0/fwdpy11/demographic_models/human.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/discrete_demography.py` & `fwdpy11-0.9.0/fwdpy11/discrete_demography.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/ezparams.py` & `fwdpy11-0.9.0/fwdpy11/ezparams.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/genetic_map_unit.py` & `fwdpy11-0.9.0/fwdpy11/genetic_map_unit.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/genetic_values.py` & `fwdpy11-0.9.0/fwdpy11/genetic_values.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/K_linked_regions_extensions.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/K_linked_regions_extensions.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/calculate_fitnesses.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/calculate_fitnesses.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/common_ind.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/common_ind.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/confirm_mutation_counts.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/confirm_mutation_counts.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/custom_diploid.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/custom_diploid.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/custom_mutation.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/custom_mutation.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/diploid_fixed_sh_ind.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/diploid_fixed_sh_ind.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/diploid_ind.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/diploid_ind.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/edge_buffering.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/edge_buffering.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/evolve_generation_ts.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/evolve_generation_ts.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/juvenile_migration.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/juvenile_migration.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/load_table_collection.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/load_table_collection.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/simplify_tables.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/simplify_tables.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_common.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_types.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/tree_sequence_examples_types.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing_with_mutation.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/unused_source/wfts_overlapping_generations_dynamic_indexing_with_mutation.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/wfevolvets.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/wfevolvets.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/wfevolvets.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/wfevolvets.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/examples/wfts_integration_test.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/examples/wfts_integration_test.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/GSLrng_t.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/GSLrng_t.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/algorithm/compact_mutations.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/algorithm/compact_mutations.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/data_matrix.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/data_matrix.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/debug.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/debug.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/diploid.hh` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/diploid.hh`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/diploid_population.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/diploid_population.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/extensions/callbacks.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/extensions/callbacks.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/extensions/regions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/extensions/regions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/fitness_models.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/fitness_models.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/forward_types.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/forward_types.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/forward_types_serialization.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/forward_types_serialization.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/fwd_functional.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/fwd_functional.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_interval.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_interval.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_point.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/binomial_point.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/fixed_number_crossovers.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/fixed_number_crossovers.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/genetic_map.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/genetic_map.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_interval.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_interval.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_point.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/genetic_map/poisson_point.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/gsl_discrete.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/gsl_discrete.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/insertion_policies.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/insertion_policies.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/data_matrix_details.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/data_matrix_details.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/debug_details.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/debug_details.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/haploid_genome_cleaner.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/haploid_genome_cleaner.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/mutation_internal.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/mutation_internal.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/rec_gamete_updater.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/rec_gamete_updater.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/recombination_common.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/recombination_common.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/sample_diploid_helpers.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/sample_diploid_helpers.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/sampling_functions_details.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/sampling_functions_details.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/internal/type_traits.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/internal/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/detail/serialize_population.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/detail/serialize_population.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/diploid.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/diploid.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/haploid_genome.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/haploid_genome.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/mutation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/mutation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/scalar_serialization.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/scalar_serialization.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/io/serialize_population.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/io/serialize_population.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/mutate_recombine.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/mutate_recombine.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/popgenmut.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/popgenmut.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/diploid_population.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/diploid_population.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/popbase.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/popbase.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/poptypes/tags.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/poptypes/tags.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.tcc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sample_diploid.tcc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sampling_functions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sampling_functions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/simfunctions/recycling.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/simfunctions/recycling.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/simparams.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/simparams.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
     /// is expected to be std::nullptr_t
     ///
     /// The heavy use of lambdas in fwdpp means that it is, in practice,
     /// nearly impossible to know the template parameter types.  Thus,
     /// objects of this type are made by calling fwdpp::make_genetic_parameters.
     ///
     /// \version 0.7.4 Added to library
+    /// \version 0.9.0 gvalue no longer const
     {
-        const genetic_value gvalue;
+        genetic_value gvalue;
         const mutation_function generate_mutations;
         const recombination_function generate_breakpoints;
         const interlocus_recombination_function interlocus_recombination;
         const parent_haploid_genome_swapping_function haploid_genome_swapper;
         flagged_mutation_queue mutation_recycling_bin;
         flagged_haploid_genome_queue haploid_genome_recycling_bin;
         std::vector<uint_t> neutral;
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sugar/add_mutation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sugar/add_mutation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/sugar/change_neutral.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/sugar/change_neutral.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/count_mutations.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/count_mutations.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/decapitate.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/decapitate.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/definitions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/definitions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/detail/advance_marginal_tree_policies.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/detail/advance_marginal_tree_policies.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/detail/generate_data_matrix_details.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/detail/generate_data_matrix_details.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/edge.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/edge.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/exceptions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/generate_data_matrix.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/generate_data_matrix.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/generate_offspring.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/generate_offspring.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/get_parent_ids.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/get_parent_ids.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/children.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/children.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_order.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_order.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_preorder.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/node_traversal_preorder.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/nodes.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/nodes.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/roots.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/roots.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/samples.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/samples.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/statistics.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/marginal_tree_functions/statistics.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mark_multiple_roots.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mark_multiple_roots.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mutate_tables.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mutate_tables.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_record.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_record.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_tools.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/mutation_tools.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/node.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/node.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/diploid_offspring.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/diploid_offspring.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/edge_buffer.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/edge_buffer.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recording/mutations.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recording/mutations.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/recycling.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/recycling.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/remove_fixations_from_gametes.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/remove_fixations_from_gametes.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/serialization.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/serialization.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/simplification/simplification.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/simplification/simplification.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/simplify_tables.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/simplify_tables.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/site.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/site.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/site_visitor.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/site_visitor.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/std_table_collection.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/std_table_collection.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection_functions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/table_collection_functions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/table_simplifier.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/table_simplifier.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/tree_visitor.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/tree_visitor.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/ts/visit_sites.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/ts/visit_sites.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/type_traits.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/abstract_cloneable.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/abstract_cloneable.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/enum_bitflags.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/enum_bitflags.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/named_type.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/named_type.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/nested_forward_lists.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/nested_forward_lists.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util/wrapped_range.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util/wrapped_range.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/fwdpp/util.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/fwdpp/util.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/fwdpp_fixtures.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/fwdpp_fixtures.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/fixtures/sugar_fixtures.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/fixtures/sugar_fixtures.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/extensions_regionsIntegrationTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/extensions_regionsIntegrationTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepopTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepopTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepop_custom_diploidTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/integration/sugar_singlepop_custom_diploidTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/independent_implementations.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/preorder_adl.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/preorder_adl.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_infinite_sites.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_infinite_sites.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_polytomy.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/simple_table_collection_polytomy.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_ancestry_list.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_ancestry_list.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_decapitate.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_decapitate.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_diploid_recording.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_diploid_recording.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_edge_buffering_std_table_collection.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_edge_buffering_std_table_collection.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_data_matrix.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_data_matrix.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_offspring.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_generate_offspring.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree_statistics.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_marginal_tree_statistics.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_node_children_traversal.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_node_children_traversal.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_preorder_node_traversal.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_preorder_node_traversal.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_root_traversal.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_root_traversal.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_sample_traversal.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_sample_traversal.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_site_visitor.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_site_visitor.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_table_collection.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_table_collection.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_tree_visitor.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_tree_visitor.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_visit_sites.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/test_visit_sites.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/tskit_utils.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection_fxns.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/tree_sequences/wfevolve_table_collection_fxns.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/extensions_callbacksTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/extensions_callbacksTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/extensions_regionsTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/extensions_regionsTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/gameteTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/gameteTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/gamete_cleanerTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/gamete_cleanerTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/mutateTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/mutateTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/serializationTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/serializationTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/siteDepFitnessTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/siteDepFitnessTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_GSLrngTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_GSLrngTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_add_mutationTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_add_mutationTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_change_neutralTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_change_neutralTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/sugar_popgenmut.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/sugar_popgenmut.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_enum_bitflags.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_enum_bitflags.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_genetic_map.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_genetic_map.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_mutate_recombine.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_mutate_recombine.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_nested_forward_lists.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_nested_forward_lists.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_recombination.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_recombination.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_simparams.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_simparams.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/test_wrapped_range.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/test_wrapped_range.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/type_traitsTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/type_traitsTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/unit/utilTest.cc` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/unit/utilTest.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/util/custom_dip.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/util/custom_dip.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpp/testsuite/util/quick_evolve_sugar.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpp/testsuite/util/quick_evolve_sugar.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/DiscreteDemography.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/DiscreteDemography.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/MassMigration.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/MassMigration.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/MigrationMatrix.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/MigrationMatrix.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetDemeSize.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetDemeSize.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetExponentialGrowth.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetExponentialGrowth.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetMigrationRates.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetMigrationRates.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/SetSelfingRate.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/SetSelfingRate.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/constants.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/constants.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/exceptions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/apply_mass_migrations.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/apply_mass_migrations.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/build_migration_lookup.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/build_migration_lookup.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_properties.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_properties.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_property_types.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/deme_property_types.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/demographic_model_state.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/demographic_model_state.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/detail.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/detail.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/functions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/functions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/get_max_number_of_demes.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/get_max_number_of_demes.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/migration_lookup.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/migration_lookup.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/multideme_fitness_lookups.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/multideme_fitness_lookups.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/pick_parents.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/pick_parents.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation/update_demographic_model_state.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation/update_demographic_model_state.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/discrete_demography/simulation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/discrete_demography/simulation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolve/DiploidPopulation_generation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolve/DiploidPopulation_generation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/SampleRecorder.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/SampleRecorder.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/evolve_generation_ts.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/evolve_generation_ts.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/recorders.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/recorders.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/sample_recorder_types.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/sample_recorder_types.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/evolvets/simplify_tables.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/evolvets/simplify_tables.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_noise/GeneticValueNoise.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_noise/GeneticValueNoise.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -19,26 +19,23 @@
 #ifndef FWDPY11_GENETIC_VALUES_NOISE_HPP__
 #define FWDPY11_GENETIC_VALUES_NOISE_HPP__
 
 #include <memory>
 #include <fwdpy11/types/Diploid.hpp>
 #include <fwdpy11/types/DiploidPopulation.hpp>
 #include <fwdpy11/rng.hpp>
+#include <fwdpy11/genetic_value_data/genetic_value_data.hpp>
 
 namespace fwdpy11
 {
     struct GeneticValueNoise
     ///ABC for random effects on trait values
     {
         virtual ~GeneticValueNoise() = default;
         virtual double
-        operator()(const GSLrng_t& /* rng */,
-                   const DiploidMetadata& /*offspring_metadata*/,
-                   const std::size_t /*parent1*/,
-                   const std::size_t /*parent2*/,
-                   const DiploidPopulation& /*pop*/) const = 0;
+        operator()(const DiploidGeneticValueNoiseData /*data*/) const = 0;
         virtual void update(const DiploidPopulation& /*pop*/) = 0;
-        virtual std::unique_ptr<GeneticValueNoise> clone() const = 0;
+        virtual std::shared_ptr<GeneticValueNoise> clone() const = 0;
     };
 } // namespace fwdpy11
 
 #endif
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_noise/NoNoise.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_noise/NoNoise.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -23,30 +23,26 @@
 #include "GeneticValueNoise.hpp"
 
 namespace fwdpy11
 {
     struct NoNoise : public GeneticValueNoise
     {
         double
-        operator()(const GSLrng_t& /*rng*/,
-                   const DiploidMetadata& /*offspring_metadata*/,
-                   const std::size_t /*parent1*/,
-                   const std::size_t /*parent2*/,
-                   const DiploidPopulation& /*pop*/) const override
+        operator()(const DiploidGeneticValueNoiseData /*data*/) const override
         {
             return 0.;
         }
 
         void
         update(const DiploidPopulation& /*pop*/) override
         {
         }
 
-        std::unique_ptr<GeneticValueNoise>
+        std::shared_ptr<GeneticValueNoise>
         clone() const override
         {
-            return std::unique_ptr<NoNoise>(new NoNoise());
+            return std::make_shared<NoNoise>();
         }
     };
 } // namespace fwdpy11
 
 #endif
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GSSmo.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GSSmo.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,20 @@
                     throw std::invalid_argument("optima not sorted by time");
                 }
             opt = optima[0].opt;
             VS = optima[0].VW;
         }
 
         double
-        operator()(const DiploidMetadata &metadata,
-                   const std::vector<double> & /*genetic_values*/) const override
+        operator()(const DiploidGeneticValueToFitnessData data) const override
         {
-            return std::exp(
-                -(std::pow(metadata.g + metadata.e - opt, 2.0) / (2.0 * VS)));
+            return std::exp(-(std::pow(data.offspring_metadata.get().g
+                                           + data.offspring_metadata.get().e - opt,
+                                       2.0)
+                              / (2.0 * VS)));
         }
 
         template <typename poptype>
         inline void
         update_details(const poptype &pop)
         {
             if (current_optimum < optima.size())
@@ -66,16 +67,16 @@
 
         void
         update(const DiploidPopulation &pop) override
         {
             update_details(pop);
         }
 
-        std::unique_ptr<GeneticValueToFitnessMap>
+        std::shared_ptr<GeneticValueToFitnessMap>
         clone() const override
         {
-            return std::unique_ptr<GSSmo>(new GSSmo(*this));
+            return std::make_shared<GSSmo>(*this);
         }
     };
 } // namespace fwdpy11
 
 #endif
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsFitness.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsFitness.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -28,29 +28,26 @@
     {
         explicit GeneticValueIsFitness(std::size_t ndim)
             : GeneticValueToFitnessMap(ndim, maps_to_fitness(true))
         {
         }
 
         double
-        operator()(
-            const DiploidMetadata &metadata,
-            const std::vector<double> & /*genetic_values*/) const override
+        operator()(const DiploidGeneticValueToFitnessData data) const override
         {
-            return metadata.g;
+            return data.offspring_metadata.get().g;
         }
 
         void
         update(const DiploidPopulation & /*pop*/) override
         {
         }
 
-        std::unique_ptr<GeneticValueToFitnessMap>
+        std::shared_ptr<GeneticValueToFitnessMap>
         clone() const override
         {
-            return std::unique_ptr<GeneticValueIsFitness>(
-                new GeneticValueIsFitness(this->total_dim));
+            return std::make_shared<GeneticValueIsFitness>(this->total_dim);
         }
     };
 } // namespace fwdpy11
 
 #endif
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueToFitnessMap.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueToFitnessMap.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #define FWDPY11_GENETIC_VALUE_TO_FITNESS_MAP_HPP__
 
 #include <memory>
 #include <pybind11/pybind11.h>
 #include <fwdpy11/types/DiploidPopulation.hpp>
 #include <fwdpy11/genetic_values/default_update.hpp>
 #include <fwdpp/util/named_type.hpp>
+#include <fwdpy11/genetic_value_data/genetic_value_data.hpp>
 
 namespace fwdpy11
 {
     struct genetic_value_maps_to_fitness
     {
     };
 
@@ -40,18 +41,17 @@
         const bool isfitness;
         explicit GeneticValueToFitnessMap(std::size_t ndim, const maps_to_fitness& m)
             : total_dim{ndim}, isfitness{m.get()}
         {
         }
         virtual ~GeneticValueToFitnessMap() = default;
         virtual double
-        operator()(const DiploidMetadata& /*metadata*/,
-                   const std::vector<double>& /*genetic_values*/) const = 0;
+        operator()(const DiploidGeneticValueToFitnessData /*data*/) const = 0;
         virtual void update(const DiploidPopulation& /*pop*/) = 0;
-        virtual std::unique_ptr<GeneticValueToFitnessMap> clone() const = 0;
+        virtual std::shared_ptr<GeneticValueToFitnessMap> clone() const = 0;
         virtual pybind11::tuple
         shape() const
         {
             return pybind11::make_tuple(total_dim);
         }
     };
 } //namespace fwdpy11
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/MultivariateGSSmo.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/MultivariateGSSmo.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -62,33 +62,33 @@
             if (!std::is_sorted(begin(optima), end(optima)))
                 {
                     throw std::invalid_argument("optima must be sorted by `when` field");
                 }
         }
 
         double
-        operator()(const DiploidMetadata & /*metadata*/,
-                   const std::vector<double> &values) const override
+        operator()(const DiploidGeneticValueToFitnessData data) const override
         {
-            if (values.size() != total_dim)
+            if (data.gvalues.get().size() != total_dim)
                 {
                     throw std::runtime_error("dimension mismatch");
                 }
             double sqdiff = 0.0;
-            for (std::size_t i = 0; i < values.size(); ++i)
+            for (std::size_t i = 0; i < data.gvalues.get().size(); ++i)
                 {
-                    sqdiff += gsl_pow_2(values[i] - optima[current_timepoint].optima[i]);
+                    sqdiff += gsl_pow_2(data.gvalues.get()[i]
+                                        - optima[current_timepoint].optima[i]);
                 }
             return std::exp(-sqdiff / (2.0 * optima[current_timepoint].VW));
         }
 
-        std::unique_ptr<GeneticValueToFitnessMap>
+        std::shared_ptr<GeneticValueToFitnessMap>
         clone() const override
         {
-            return std::unique_ptr<MultivariateGSSmo>(new MultivariateGSSmo(*this));
+            return std::make_shared<MultivariateGSSmo>(*this);
         }
 
         template <typename poptype>
         inline void
         update_details(const poptype &pop)
         {
             if (current_timepoint < optima.size() - 1
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/Optimum.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/Optimum.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/PleiotropicOptima.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_value_to_fitness/PleiotropicOptima.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/DiploidMultivariateEffectsStrictAdditive.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/DiploidMultivariateEffectsStrictAdditive.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -3,82 +3,69 @@
 
 #include <vector>
 #include <stdexcept>
 #include <algorithm>
 #include <functional>
 #include "DiploidGeneticValue.hpp"
 #include "default_update.hpp"
+#include <fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp>
 
 namespace fwdpy11
 {
-    struct DiploidMultivariateEffectsStrictAdditive
-        : public DiploidGeneticValue
+    struct DiploidMultivariateEffectsStrictAdditive : public DiploidGeneticValue
     {
         std::size_t focal_trait_index;
 
-        DiploidMultivariateEffectsStrictAdditive(
-            std::size_t ndim, std::size_t focal_trait,
-            const GeneticValueIsTrait &gv2w_)
-            : DiploidGeneticValue(ndim, gv2w_), focal_trait_index(focal_trait)
-        {
-            if (focal_trait_index >= ndim)
-                {
-                    throw std::invalid_argument(
-                        "focal trait index must by < number of traits");
-                }
-        }
-
-        DiploidMultivariateEffectsStrictAdditive(
-            std::size_t ndim, std::size_t focal_trait,
-            const GeneticValueIsTrait &gv2w_, const GeneticValueNoise &noise_)
-            : DiploidGeneticValue(ndim, gv2w_, noise_),
-              focal_trait_index(focal_trait)
+        DiploidMultivariateEffectsStrictAdditive(std::size_t ndim,
+                                                 std::size_t focal_trait,
+                                                 const GeneticValueIsTrait *gv2w_,
+                                                 const GeneticValueNoise *noise_)
+            : DiploidGeneticValue(ndim, gv2w_, noise_), focal_trait_index(focal_trait)
         {
             if (focal_trait_index >= ndim)
                 {
                     throw std::invalid_argument(
                         "focal trait index must by < number of traits");
                 }
         }
 
         double
-        calculate_gvalue(const std::size_t diploid_index,
-                         const DiploidMetadata& /*metadata*/,
-                         const DiploidPopulation& pop) const
+        calculate_gvalue(const fwdpy11::DiploidGeneticValueData data) override
         {
             std::fill(begin(gvalues), end(gvalues), 0.0);
 
+            const auto &pop = data.pop.get();
+            const auto diploid_index = data.offspring_metadata.get().label;
             for (auto key :
-                 pop.haploid_genomes[pop.diploids[diploid_index].first]
-                     .smutations)
+                 pop.haploid_genomes[pop.diploids[diploid_index].first].smutations)
                 {
                     const auto &mut = pop.mutations[key];
                     if (mut.esizes.size() != gvalues.size())
                         {
-                            throw std::runtime_error(
-                                "dimensionality mismatch");
+                            throw std::runtime_error("dimensionality mismatch");
                         }
-                    std::transform(begin(mut.esizes), end(mut.esizes),
-                                   begin(gvalues), begin(gvalues),
-                                   std::plus<double>());
+                    std::transform(begin(mut.esizes), end(mut.esizes), begin(gvalues),
+                                   begin(gvalues), std::plus<double>());
                 }
 
             for (auto key :
-                 pop.haploid_genomes[pop.diploids[diploid_index].second]
-                     .smutations)
+                 pop.haploid_genomes[pop.diploids[diploid_index].second].smutations)
                 {
                     const auto &mut = pop.mutations[key];
                     if (mut.esizes.size() != gvalues.size())
                         {
-                            throw std::runtime_error(
-                                "dimensionality mismatch");
+                            throw std::runtime_error("dimensionality mismatch");
                         }
-                    std::transform(begin(mut.esizes), end(mut.esizes),
-                                   begin(gvalues), begin(gvalues),
-                                   std::plus<double>());
+                    std::transform(begin(mut.esizes), end(mut.esizes), begin(gvalues),
+                                   begin(gvalues), std::plus<double>());
                 }
             return gvalues[focal_trait_index];
         }
+
+        void
+        update(const fwdpy11::DiploidPopulation & /*pop*/) override
+        {
+        }
     };
 } // namespace fwdpy11
 
 #endif
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/default_update.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/default_update.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/GBR.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/GBR.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_GBR.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_GBR.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_multiplicative.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/details/pickle_multiplicative.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/dgvalue_pointer_vector.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/dgvalue_pointer_vector.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     // simulations.
     // This class exists because our genetic value types
     // are held by Python in std::unique_ptr, and
     // pybind11 (correctly) doesn't allow unique_ptr<T>
     // to be passed as an argument to a C++ function.
     // Thus, we compromise with raw pointers stored in a vector.
     {
-        const std::vector<fwdpy11::DiploidGeneticValue *> genetic_values;
+        std::vector<fwdpy11::DiploidGeneticValue *> genetic_values;
 
         std::vector<fwdpy11::DiploidGeneticValue *>
         init_from_list(pybind11::list l)
         {
             if (l.empty())
                 {
                     throw std::invalid_argument(
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/genetic_values/fwdpp_wrappers/fwdpp_genetic_value.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/genetic_values/fwdpp_wrappers/fwdpp_genetic_value.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -64,69 +64,56 @@
             }
         };
 
         using callback_type = std::function<double(
             const fwdpp::site_dependent_genetic_value&, const std::size_t,
             const DiploidMetadata&, const DiploidPopulation&)>;
 
+        using make_return_value_t = std::function<double(double)>;
+
         callback_type
         init_callback(std::size_t n, double aa_scaling)
         {
             if (n == 1)
                 {
                     return single_deme_callback(aa_scaling);
                 }
             return multi_deme_callback(aa_scaling);
         }
 
         fwdpp::site_dependent_genetic_value gv;
         double aa_scaling;
-        std::function<double(double)> make_return_value;
+        make_return_value_t make_return_value;
         callback_type callback;
         bool isfitness;
 
       public:
-        template <typename make_return_value_fxn>
-        stateless_site_dependent_genetic_value_wrapper(std::size_t ndim, double scaling,
-                                                       make_return_value_fxn&& mrv)
-            : DiploidGeneticValue{ndim}, gv{}, aa_scaling(scaling),
-              make_return_value(std::forward<make_return_value_fxn>(mrv)),
-              callback(init_callback(ndim, aa_scaling)), isfitness(true)
-        {
-        }
-
-        template <typename make_return_value_fxn>
-        stateless_site_dependent_genetic_value_wrapper(
-            std::size_t ndim, double scaling, make_return_value_fxn&& mrv,
-            const GeneticValueToFitnessMap& gv2w_)
-            : DiploidGeneticValue{ndim, gv2w_}, gv{}, aa_scaling(scaling),
-              make_return_value(std::forward<make_return_value_fxn>(mrv)),
-              callback(init_callback(ndim, aa_scaling)), isfitness(gv2w->isfitness)
-        {
-        }
-
-        template <typename make_return_value_fxn>
         stateless_site_dependent_genetic_value_wrapper(
-            std::size_t ndim, double scaling, make_return_value_fxn&& mrv,
-            const GeneticValueToFitnessMap& gv2w_, const GeneticValueNoise& noise_)
+            std::size_t ndim, double scaling, make_return_value_t mrv,
+            const GeneticValueToFitnessMap* gv2w_, const GeneticValueNoise* noise_)
             : DiploidGeneticValue{ndim, gv2w_, noise_}, gv{}, aa_scaling(scaling),
-              make_return_value(std::forward<make_return_value_fxn>(mrv)),
+              make_return_value(std::move(mrv)),
               callback(init_callback(ndim, aa_scaling)), isfitness(gv2w->isfitness)
         {
         }
 
         double
-        calculate_gvalue(const std::size_t diploid_index,
-                         const DiploidMetadata& metadata,
-                         const DiploidPopulation& pop) const override
+        calculate_gvalue(const DiploidGeneticValueData data) override
         {
-            gvalues[0] = make_return_value(callback(gv, diploid_index, metadata, pop));
+            gvalues[0] = make_return_value(
+                callback(gv, data.offspring_metadata.get().label,
+                         data.offspring_metadata.get(), data.pop.get()));
             return gvalues[0];
         }
 
+        void
+        update(const fwdpy11::DiploidPopulation& /*pop*/) override
+        {
+        }
+
         double
         scaling() const
         {
             return aa_scaling;
         }
 
         bool
```

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/gsl/gsl_error_handler_wrapper.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/gsl/gsl_error_handler_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/numpy/array.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/numpy/array.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/policies/mutation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/policies/mutation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/ConstantS.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/ConstantS.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/ExpS.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/ExpS.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/GammaS.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/GammaS.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/GaussianS.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/GaussianS.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/LogNormalS.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/LogNormalS.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/MultivariateGaussianEffects.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/MultivariateGaussianEffects.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/MutationRegions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/MutationRegions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/RecombinationRegions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/RecombinationRegions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/Region.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/Region.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/Sregion.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/Sregion.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/UniformS.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/UniformS.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/regions/mvDES.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/regions/mvDES.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/rng.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/rng.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/samplers.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/samplers.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/sampling/data_matrix_functions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/sampling/data_matrix_functions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/Diploid.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/Diploid.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/Mutation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/Mutation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/backwards_compat.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/backwards_compat.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization/diploid_metadata.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization/diploid_metadata.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/serialization.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/serialization.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/sim_functions.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/sim_functions.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/Diploid.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/Diploid.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/DiploidPopulation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/DiploidPopulation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/Mutation.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/Mutation.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/types/Population.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/types/Population.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/util/clone_cloneable.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/util/clone_cloneable.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/headers/fwdpy11/util/convert_lists.hpp` & `fwdpy11-0.9.0/fwdpy11/headers/fwdpy11/util/convert_lists.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/regions.py` & `fwdpy11-0.9.0/fwdpy11/regions.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/_fwdpy11.cc` & `fwdpy11-0.9.0/fwdpy11/src/_fwdpy11.cc`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 void initialize_genetic_value_noise(py::module &);
 void initialize_genetic_value_to_fitness(py::module &);
 void init_genetic_values(py::module &);
 void init_GSL(py::module &);
 void init_ts(py::module &);
 void init_evolution_functions(py::module &);
 void init_discrete_demography(py::module &m);
+void init_array_proxies(py::module &m);
 
 PYBIND11_MODULE(_fwdpy11, m)
 {
     auto handler = gsl_set_error_handler_off();
 
     auto custom_handler = gsl_set_error_handler(&gsl_error_to_exception);
 
@@ -53,14 +54,15 @@
     initialize_genetic_value_noise(m);
     initialize_genetic_value_to_fitness(m);
     init_genetic_values(m);
     init_GSL(m);
     init_ts(m);
     init_evolution_functions(m);
     init_discrete_demography(m);
+    init_array_proxies(m);
 
     m.def(
         "pybind11_version",
         []() {
             py::dict rv;
             std::ostringstream o;
             o << PYBIND11_VERSION;
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/DiscreteDemography.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/DiscreteDemography.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/MassMigration.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/MassMigration.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/MigrationMatrix.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/MigrationMatrix.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetDemeSize.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetDemeSize.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetExponentialGrowth.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetExponentialGrowth.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetMigrationRates.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetMigrationRates.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/SetSelfingRate.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/SetSelfingRate.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/exceptions.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/exceptions.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/discrete_demography/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/discrete_demography/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/cleanup_metadata.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/cleanup_metadata.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/diploid_pop_fitness.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/diploid_pop_fitness.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #include "diploid_pop_fitness.hpp"
 
 void
 calculate_diploid_fitness(
     const fwdpy11::GSLrng_t &rng, fwdpy11::DiploidPopulation &pop,
-    const std::vector<fwdpy11::DiploidGeneticValue *> &gvalue_pointers,
+    std::vector<fwdpy11::DiploidGeneticValue *> &gvalue_pointers,
     const std::vector<std::size_t> &deme_to_gvalue_map,
     std::vector<fwdpy11::DiploidMetadata> &offspring_metadata,
     std::vector<double> &new_diploid_gvalues, const bool update_genotype_matrix)
 {
     // Calculate parental fitnesses
     double sum_parental_fitnesses = 0.0;
     new_diploid_gvalues.clear();
     for (std::size_t i = 0; i < offspring_metadata.size(); ++i)
         {
             auto idx = deme_to_gvalue_map[offspring_metadata[i].deme];
-            gvalue_pointers[idx]->operator()(rng, offspring_metadata[i].label, pop,
-                                             offspring_metadata[i]);
+            //gvalue_pointers[idx]->operator()(rng, offspring_metadata[i].label, pop,
+            //                                 offspring_metadata[i]);
+            gvalue_pointers[idx]->operator()(fwdpy11::DiploidGeneticValueData(
+                rng, pop, pop.diploid_metadata[offspring_metadata[i].parents[0]],
+                pop.diploid_metadata[offspring_metadata[i].parents[1]], i,
+                offspring_metadata[i]));
             if (update_genotype_matrix == true)
                 {
                     new_diploid_gvalues.insert(end(new_diploid_gvalues),
                                                begin(gvalue_pointers[idx]->gvalues),
                                                end(gvalue_pointers[idx]->gvalues));
                 }
             sum_parental_fitnesses += offspring_metadata[i].w;
@@ -33,23 +37,26 @@
             throw std::runtime_error("non-finite fitnesses encountered");
         }
 }
 
 fwdpp::gsl_ran_discrete_t_ptr
 calculate_diploid_fitness_genomes(
     const fwdpy11::GSLrng_t &rng, fwdpy11::DiploidPopulation &pop,
-    const fwdpy11::DiploidGeneticValue &genetic_value_fxn,
+    fwdpy11::DiploidGeneticValue &genetic_value_fxn,
     std::vector<fwdpy11::DiploidMetadata> &offspring_metadata)
 {
     // Calculate parental fitnesses
     std::vector<double> parental_fitnesses(pop.diploids.size());
     double sum_parental_fitnesses = 0.0;
     for (std::size_t i = 0; i < pop.diploids.size(); ++i)
         {
-            genetic_value_fxn(rng, i, pop, offspring_metadata[i]);
+            genetic_value_fxn(fwdpy11::DiploidGeneticValueData(
+                rng, pop, pop.diploid_metadata[offspring_metadata[i].parents[0]],
+                pop.diploid_metadata[offspring_metadata[i].parents[1]], i,
+                offspring_metadata[i]));
             parental_fitnesses[i] = offspring_metadata[i].w;
             sum_parental_fitnesses += parental_fitnesses[i];
         }
     // If the sum of parental fitnesses is not finite,
     // then the genetic value calculator returned a non-finite value/
     // Unfortunately, gsl_ran_discrete_preproc allows such values through
     // without raising an error, so we have to check things here.
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/diploid_pop_fitness.hpp` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/diploid_pop_fitness.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 #include <fwdpp/gsl_discrete.hpp>
 #include <fwdpy11/types/DiploidPopulation.hpp>
 #include <fwdpy11/genetic_values/DiploidGeneticValue.hpp>
 
 // Changed in 0.6.0 to return void, as sims w/tree
 // sequences generate fitness lookups via DiscreteDemography
-void calculate_diploid_fitness(
-    const fwdpy11::GSLrng_t &rng, fwdpy11::DiploidPopulation &pop,
-    const std::vector<fwdpy11::DiploidGeneticValue *>
-        &gvalue_pointers,
-    const std::vector<std::size_t> &deme_to_gvalue_map,
-    std::vector<fwdpy11::DiploidMetadata> &offspring_metadata,
-    std::vector<double> &new_diploid_gvalues,
-    const bool update_genotype_matrix);
+void
+calculate_diploid_fitness(const fwdpy11::GSLrng_t &rng, fwdpy11::DiploidPopulation &pop,
+                          std::vector<fwdpy11::DiploidGeneticValue *> &gvalue_pointers,
+                          const std::vector<std::size_t> &deme_to_gvalue_map,
+                          std::vector<fwdpy11::DiploidMetadata> &offspring_metadata,
+                          std::vector<double> &new_diploid_gvalues,
+                          const bool update_genotype_matrix);
 
 // This overload was added in 0.6.0 as a temporary
 // hack b/c sims with tree sequences generate fitness
 // lookups via DiscreteDemography
 fwdpp::gsl_ran_discrete_t_ptr calculate_diploid_fitness_genomes(
     const fwdpy11::GSLrng_t &rng, fwdpy11::DiploidPopulation &pop,
-    const fwdpy11::DiploidGeneticValue &genetic_value_fxn,
+    fwdpy11::DiploidGeneticValue &genetic_value_fxn,
     std::vector<fwdpy11::DiploidMetadata> &offspring_metadata);
 
 #endif
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/index_and_count_mutations.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/index_and_count_mutations.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/no_tree_sequences.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/no_tree_sequences.cc`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,16 @@
           };
     const auto bound_rmodel = [&rng, &rmodel]() { return rmodel(rng); };
 
     // A stateful fitness model will need its data up-to-date,
     // so we must call update(...) prior to calculating fitness,
     // else bad stuff like segfaults could happen.
     genetic_value_fxn.update(pop);
+    genetic_value_fxn.gv2w->update(pop);
+    genetic_value_fxn.noise_fxn->update(pop);
     std::vector<fwdpy11::DiploidMetadata> offspring_metadata(
         pop.diploid_metadata);
     auto lookup = calculate_diploid_fitness_genomes(
         rng, pop, genetic_value_fxn, offspring_metadata);
     pop.diploid_metadata.swap(offspring_metadata);
 
     // Generate our fxns for picking parents
@@ -167,20 +169,22 @@
             fwdpy11::evolve_generation(
                 rng, pop, N_next, mu_neutral + mu_selected, bound_mmodel,
                 bound_rmodel, pick_first_parent, pick_second_parent,
                 generate_offspring_metadata, offspring, offspring_metadata);
             handle_fixations(remove_selected_fixations, N_next, pop);
 
             pop.diploids.swap(offspring);
+            // TODO: deal with random effects
+            genetic_value_fxn.update(pop);
+            genetic_value_fxn.gv2w->update(pop);
+            genetic_value_fxn.noise_fxn->update(pop);
             lookup = calculate_diploid_fitness_genomes(
                 rng, pop, genetic_value_fxn, offspring_metadata);
             pop.diploid_metadata.swap(offspring_metadata);
             pop.N = N_next;
-            // TODO: deal with random effects
-            genetic_value_fxn.update(pop);
             recorder(pop); // The user may now analyze the pop'n
         }
 }
 
 void
 init_evolve_without_tree_sequences(py::module &m)
 {
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/remove_extinct_genomes.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/remove_extinct_genomes.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/remove_extinct_mutations.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/remove_extinct_mutations.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/track_ancestral_counts.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/track_ancestral_counts.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/track_mutation_counts.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/track_mutation_counts.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/util.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/util.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/evolve_population/with_tree_sequences.cc` & `fwdpy11-0.9.0/fwdpy11/src/evolve_population/with_tree_sequences.cc`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     fwdpy11::SampleRecorder &sr, const unsigned simplification_interval,
     ddemog::DiscreteDemography &demography, const std::uint32_t simlen,
     const double mu_neutral, const double mu_selected,
     const fwdpy11::MutationRegions &mmodel, const fwdpy11::GeneticMap &rmodel,
     // NOTE: gvalue_pointers is a change in 0.6.0,
     // and the object holds non-const bare pointers
     // to objects owned by Python.
-    const fwdpy11::dgvalue_pointer_vector_ &gvalue_pointers,
+    fwdpy11::dgvalue_pointer_vector_ &gvalue_pointers,
     fwdpy11::DiploidPopulation_sample_recorder recorder,
     std::function<bool(const fwdpy11::DiploidPopulation &, const bool)>
         &stopping_criteron,
     const double selfing_rate,
     // NOTE: this is the complement of what a user will input, which is "prune_selected"
     const bool preserve_selected_fixations, const bool suppress_edge_table_indexing,
     bool record_genotype_matrix, const bool track_mutation_counts_during_sim,
@@ -266,14 +266,16 @@
         }
     // A stateful fitness model will need its data up-to-date,
     // so we must call update(...) prior to calculating fitness,
     // else bad stuff like segfaults could happen.
     for (auto &i : genetics.gvalue)
         {
             i->update(pop);
+            i->gv2w->update(pop);
+            i->noise_fxn->update(pop);
         }
     std::vector<fwdpy11::DiploidMetadata> offspring_metadata(pop.diploid_metadata);
     std::vector<fwdpy11::DiploidGenotype> offspring;
     std::vector<double> new_diploid_gvalues;
     calculate_diploid_fitness(rng, pop, genetics.gvalue, deme_to_gvalue_map,
                               offspring_metadata, new_diploid_gvalues,
                               record_genotype_matrix);
@@ -395,14 +397,16 @@
             // metadata in the expected places for
             // calculate_diploid_fitness
             pop.diploid_metadata.swap(offspring_metadata);
             // TODO: deal with random effects
             for (auto &i : genetics.gvalue)
                 {
                     i->update(pop);
+                    i->gv2w->update(pop);
+                    i->noise_fxn->update(pop);
                 }
             pop.diploid_metadata.swap(offspring_metadata);
             calculate_diploid_fitness(rng, pop, genetics.gvalue, deme_to_gvalue_map,
                                       offspring_metadata, new_diploid_gvalues,
                                       record_genotype_matrix);
             pop.genetic_value_matrix.swap(new_diploid_gvalues);
             // TODO: abstract out these steps into a "cleanup_pop" function
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_functions/data_matrix_creation.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_functions/data_matrix_creation.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/DataMatrix.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/DataMatrix.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/Edge.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/Edge.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/EdgeTable.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/EdgeTable.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/GeneticMapUnit.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/GeneticMapUnit.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/HaploidGenome.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/HaploidGenome.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/MutationBase.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/MutationBase.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/MutationRecord.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/MutationRecord.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/MutationTable.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/MutationTable.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/Node.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/Node.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/NodeTable.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/NodeTable.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/Site.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/Site.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/SiteTable.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/SiteTable.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/TableCollection.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/TableCollection.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpp_types/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpp_types/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_functions/change_effect_size.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_functions/change_effect_size.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_functions/sort_gamete_keys.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_functions/sort_gamete_keys.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidGenotype.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidGenotype.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidMetadata.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidMetadata.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidPopulation.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidPopulation.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/DiploidVector.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/DiploidVector.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/HaploidGenomeVector.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/HaploidGenomeVector.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/Mutation.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/Mutation.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/MutationVector.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/MutationVector.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/PopulationBase.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/PopulationBase.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/get_individuals.hpp` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/get_individuals.hpp`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/ts_from_tskit.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/ts_from_tskit.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/fwdpy11_types/tsrecorders.cc` & `fwdpy11-0.9.0/fwdpy11/src/fwdpy11_types/tsrecorders.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_value_noise/GaussianNoise.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_value_noise/GaussianNoise.cc`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,28 @@
 
 struct GaussianNoise : public fwdpy11::GeneticValueNoise
 {
     const double sd, mean;
     GaussianNoise(const double s, const double m) : sd{ s }, mean{ m } {}
 
     double
-    operator()(const fwdpy11::GSLrng_t& rng,
-               const fwdpy11::DiploidMetadata& /*offspring_metadata*/,
-               const std::size_t /*parent1*/, const std::size_t /*parent2*/,
-               const fwdpy11::DiploidPopulation& /*pop*/) const override
+    operator()(const fwdpy11::DiploidGeneticValueNoiseData data) const override
     {
-        return mean + gsl_ran_gaussian_ziggurat(rng.get(), sd);
+        return mean + gsl_ran_gaussian_ziggurat(data.rng.get().get(), sd);
     }
 
     void
     update(const fwdpy11::DiploidPopulation& /*pop*/) override
     {
     }
 
-    std::unique_ptr<fwdpy11::GeneticValueNoise>
+    std::shared_ptr<fwdpy11::GeneticValueNoise>
     clone() const override
     {
-        return std::unique_ptr<GaussianNoise>(new GaussianNoise(*this));
+        return std::make_shared<GaussianNoise>(*this);
     }
 };
 
 void
 init_GaussianNoise(py::module& m)
 {
     py::class_<GaussianNoise, fwdpy11::GeneticValueNoise>(
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/GeneticValueIsFitness.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/GeneticValueIsFitness.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/GeneticValueToFitnessMap.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/GeneticValueToFitnessMap.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/Optimum.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/Optimum.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/PleiotropicOptima.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/PleiotropicOptima.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_value_to_fitness/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_value_to_fitness/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_values/Additive.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_values/Additive.cc`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 // You should have received a copy of the GNU General Public License
 // along with fwdpy11.  If not, see <http://www.gnu.org/licenses/>.
 //
 
 #include <functional>
 #include <fwdpy11/types/Mutation.hpp>
 #include <fwdpy11/genetic_values/fwdpp_wrappers/fwdpp_genetic_value.hpp>
+#include <fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp>
 #include <pybind11/pybind11.h>
 
 namespace
 {
     struct single_deme_additive_het
     {
         inline void
@@ -95,29 +96,21 @@
 
 namespace py = pybind11;
 
 void
 init_Additive(py::module& m)
 {
     py::class_<DiploidAdditive, fwdpy11::DiploidGeneticValue>(m, "_ll_Additive")
-        .def(py::init([](double scaling, py::object gvalue_to_fitness, py::object noise,
-                         std::size_t ndemes) {
-                 if (gvalue_to_fitness.is_none() && noise.is_none())
+        .def(py::init([](double scaling,
+                         const fwdpy11::GeneticValueIsTrait* gvalue_to_fitness,
+                         const fwdpy11::GeneticValueNoise* noise, std::size_t ndemes) {
+                 if (gvalue_to_fitness != nullptr)
                      {
-                         return DiploidAdditive(ndemes, scaling,
-                                                final_additive_fitness());
+                         return DiploidAdditive(ndemes, scaling, final_additive_trait(),
+                                                gvalue_to_fitness, noise);
                      }
-                 if (noise.is_none())
-                     {
-                         return DiploidAdditive(
-                             ndemes, scaling, final_additive_trait(),
-                             gvalue_to_fitness
-                                 .cast<const fwdpy11::GeneticValueIsTrait&>());
-                     }
-                 return DiploidAdditive(
-                     ndemes, scaling, final_additive_trait(),
-                     gvalue_to_fitness.cast<const fwdpy11::GeneticValueIsTrait&>(),
-                     noise.cast<const fwdpy11::GeneticValueNoise&>());
+                 return DiploidAdditive(ndemes, scaling, final_additive_fitness(),
+                                        gvalue_to_fitness, noise);
              }),
              py::arg("scaling"), py::arg("gvalue_to_fitness"), py::arg("noise"),
              py::arg("ndemes"));
 }
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_values/DiploidMultivariateEffectsStrictAdditive.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_values/DiploidMultivariateEffectsStrictAdditive.cc`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,15 @@
 
 void
 init_DiploidMultivariateEffectsStrictAdditive(py::module& m)
 {
     py::class_<fwdpy11::DiploidMultivariateEffectsStrictAdditive,
                fwdpy11::DiploidGeneticValue>(m, "_ll_StrictAdditiveMultivariateEffects")
         .def(py::init([](std::size_t ndimensions, std::size_t focal_trait,
-                         const fwdpy11::GeneticValueIsTrait& gvalue_to_fitness,
-                         py::object noise) {
-                 if (noise.is_none())
-                     {
-                         return fwdpy11::DiploidMultivariateEffectsStrictAdditive(
-                             ndimensions, focal_trait, gvalue_to_fitness);
-                     }
+                         const fwdpy11::GeneticValueIsTrait* gvalue_to_fitness,
+                         const fwdpy11::GeneticValueNoise* noise) {
                  return fwdpy11::DiploidMultivariateEffectsStrictAdditive(
-                     ndimensions, focal_trait, gvalue_to_fitness,
-                     noise.cast<const fwdpy11::GeneticValueNoise&>());
+                     ndimensions, focal_trait, gvalue_to_fitness, noise);
              }),
              py::arg("ndimensions"), py::arg("focal_trait"),
              py::arg("gvalue_to_fitness"), py::arg("noise"));
 }
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_values/GBR.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_values/GBR.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #include <fwdpy11/genetic_values/DiploidGeneticValue.hpp>
-#include <fwdpy11/genetic_value_to_fitness/GeneticValueToFitnessMap.hpp>
+#include <fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp>
 #include <fwdpy11/genetic_value_noise/GeneticValueNoise.hpp>
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 
 namespace
 {
@@ -71,47 +71,41 @@
         }
 
         const std::function<double(const std::size_t diploid_index,
                                    const fwdpy11::DiploidPopulation& pop)>
             f;
 
       public:
-        GBR(std::size_t ndim, const fwdpy11::GeneticValueToFitnessMap& gv2w_)
-            : fwdpy11::DiploidGeneticValue{ndim, gv2w_},
-              deme(0), f{generate_backend_function(total_dim, deme)}
-        {
-        }
-
-        GBR(std::size_t ndim, const fwdpy11::GeneticValueToFitnessMap& gv2w_,
-            const fwdpy11::GeneticValueNoise& noise_)
+        GBR(std::size_t ndim, const fwdpy11::GeneticValueToFitnessMap* gv2w_,
+            const fwdpy11::GeneticValueNoise* noise_)
             : fwdpy11::DiploidGeneticValue{ndim, gv2w_, noise_},
               deme(0), f{generate_backend_function(total_dim, deme)}
         {
         }
 
         double
-        calculate_gvalue(const std::size_t diploid_index,
-                         const fwdpy11::DiploidMetadata& /*metadata*/,
-                         const fwdpy11::DiploidPopulation& pop) const override
+        calculate_gvalue(const fwdpy11::DiploidGeneticValueData data) override
         {
-            deme = pop.diploid_metadata[diploid_index].deme;
-            gvalues[0] = f(diploid_index, pop);
+            deme = data.pop.get()
+                       .diploid_metadata[data.offspring_metadata.get().label]
+                       .deme;
+            gvalues[0] = f(data.offspring_metadata.get().label, data.pop.get());
             return gvalues[0];
         }
+
+        void
+        update(const fwdpy11::DiploidPopulation& /*pop*/) override
+        {
+        }
     };
 }
 
 void
 init_GBR(py::module& m)
 {
     py::class_<GBR, fwdpy11::DiploidGeneticValue>(m, "_ll_GBR")
-        .def(py::init([](const fwdpy11::GeneticValueIsTrait& gvalue_to_fitness,
-                         py::object noise) {
-                 if (noise.is_none())
-                     {
-                         return GBR(1, gvalue_to_fitness);
-                     }
-                 return GBR(1, gvalue_to_fitness,
-                            noise.cast<const fwdpy11::GeneticValueNoise&>());
+        .def(py::init([](const fwdpy11::GeneticValueIsTrait* gvalue_to_fitness,
+                         const fwdpy11::GeneticValueNoise* noise) {
+                 return GBR(1, gvalue_to_fitness, noise);
              }),
              py::arg("gvalue_to_fitness"), py::arg("noise"));
 }
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_values/Multiplicative.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_values/Multiplicative.cc`

 * *Files 11% similar despite different names*

```diff
@@ -97,29 +97,23 @@
 }
 
 void
 init_Multiplicative(py::module& m)
 {
     py::class_<DiploidMultiplicative, fwdpy11::DiploidGeneticValue>(m,
                                                                     "_ll_Multiplicative")
-        .def(py::init([](double scaling, py::object gvalue_to_fitness, py::object noise,
-                         std::size_t ndemes) {
-                 if (gvalue_to_fitness.is_none() && noise.is_none())
+        .def(py::init([](double scaling,
+                         const fwdpy11::GeneticValueIsTrait* gvalue_to_fitness,
+                         const fwdpy11::GeneticValueNoise* noise, std::size_t ndemes) {
+                 if (gvalue_to_fitness != nullptr)
                      {
                          return DiploidMultiplicative(ndemes, scaling,
-                                                      final_multiplicative_fitness());
+                                                      final_multiplicative_trait(),
+                                                      gvalue_to_fitness, noise);
                      }
-                 if (noise.is_none())
-                     {
-                         return DiploidMultiplicative(
-                             ndemes, scaling, final_multiplicative_trait(),
-                             gvalue_to_fitness
-                                 .cast<const fwdpy11::GeneticValueIsTrait&>());
-                     }
-                 return DiploidMultiplicative(
-                     ndemes, scaling, final_multiplicative_trait(),
-                     gvalue_to_fitness.cast<const fwdpy11::GeneticValueIsTrait&>(),
-                     noise.cast<const fwdpy11::GeneticValueNoise&>());
+                 return DiploidMultiplicative(ndemes, scaling,
+                                              final_multiplicative_fitness(),
+                                              gvalue_to_fitness, noise);
              }),
              py::arg("scaling"), py::arg("gvalue_to_fitness"), py::arg("noise"),
              py::arg("ndemes"));
 }
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_values/dgvalue_pointer_vector.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_values/dgvalue_pointer_vector.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/genetic_values/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/genetic_values/init.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 
 void init_DiploidGeneticValue(py::module&);
+void init_PyDiploidGeneticValue(py::module&);
 void init_Additive(py::module&);
 void init_Multiplicative(py::module&);
 void init_GBR(py::module&);
 void init_DiploidMultivariateEffectsStrictAdditive(py::module&);
 void init_dgvalue_pointer_vector(py::module&);
 
 void
 init_base_classes(py::module& m)
 {
     init_DiploidGeneticValue(m);
+    init_PyDiploidGeneticValue(m);
 }
 
 void
 init_genetic_value_classes(py::module& m)
 {
     init_Additive(m);
     init_Multiplicative(m);
```

### Comparing `fwdpy11-0.8.3/fwdpy11/src/gsl/gsl_random.cc` & `fwdpy11-0.9.0/fwdpy11/src/gsl/gsl_random.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/gsl/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/gsl/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/ConstantS.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/ConstantS.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/ExpS.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/ExpS.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/GammaS.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/GammaS.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/GaussianS.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/GaussianS.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/LogNormalS.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/LogNormalS.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/MultivariateGaussianEffects.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/MultivariateGaussianEffects.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/MutationRegions.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/MutationRegions.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/RecombinationRegions.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/RecombinationRegions.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/Sregion.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/Sregion.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/UniformS.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/UniformS.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/regions/mvDES.cc` & `fwdpy11-0.9.0/fwdpy11/src/regions/mvDES.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/DataMatrixIterator.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/DataMatrixIterator.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/TreeIterator.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/TreeIterator.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/VariantIterator.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/VariantIterator.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/count_mutations.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/count_mutations.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/data_matrix_from_tables.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/data_matrix_from_tables.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/infinite_sites.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/infinite_sites.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/init.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/init.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/src/ts/simplify.cc` & `fwdpy11-0.9.0/fwdpy11/src/ts/simplify.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11/tskit_tools/__init__.py` & `fwdpy11-0.9.0/fwdpy11/tskit_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/fwdpy11.egg-info/PKG-INFO` & `fwdpy11-0.9.0/fwdpy11.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdpy11
-Version: 0.8.3
+Version: 0.9.0
 Summary: Forward-time population genetic simulation in Python
 Home-page: http://molpopgen.github.io/fwdpy11
 Author: Kevin Thornton
 Author-email: krthornt@uci.edu
 License: GNU GPLv3+
 Description: fwdpy11
         *************************
```

### Comparing `fwdpy11-0.8.3/fwdpy11.egg-info/SOURCES.txt` & `fwdpy11-0.9.0/fwdpy11.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,18 @@
 doc/examples/IM.rst
 doc/examples/bgs.rst
 doc/examples/gss.rst
 doc/examples/gss_divergent_optima.rst
 doc/examples/localadaptation.rst
 doc/examples/migtest.rst
 doc/examples/precapitation.rst
+doc/examples/pysnowdrift.png
+doc/examples/pysnowdrift.rst
 doc/examples/recapitation.rst
 doc/examples/recorder.rst
-doc/examples/snowdrift.rst
 doc/images/Makefile
 doc/images/localadaptation.png
 doc/images/migtest.png
 doc/images/moments_IM_gamma_minus_5.png
 doc/images/moments_IM_neutral.png
 doc/images/structures.dot
 doc/images/structures.png
@@ -54,21 +55,21 @@
 doc/images/tree.png
 doc/misc/changelog.rst
 doc/misc/deprecated.rst
 doc/misc/developersguide.rst
 doc/misc/pubs.rst
 doc/misc/references.rst
 doc/misc/upgrade_path.rst
-doc/misc/writingplugins.rst
 doc/pages/advancedtopics.rst
 doc/pages/datamatrix.rst
 doc/pages/definitions.rst
 doc/pages/demographic_models.rst
 doc/pages/functions.rst
 doc/pages/genetic_values.rst
+doc/pages/gslrandom.rst
 doc/pages/gvalue_to_fitness.rst
 doc/pages/gvaluenoise.rst
 doc/pages/model_params.rst
 doc/pages/mvdes.rst
 doc/pages/recorders.rst
 doc/pages/regiontypes.rst
 doc/pages/softselection.rst
@@ -79,14 +80,16 @@
 doc/pages/tutorial.rst
 doc/pages/types.rst
 doc/savefig/efficient_timeseries_example.png
 doc/savefig/gss_two_deme_effect_sizes.png
 doc/savefig/mean_genetic_values_over_time.png
 doc/savefig/pi_over_time.png
 doc/savefig/sfs_example.png
+doc/technical/genetic_values.rst
+doc/technical/writingplugins.rst
 doc/unused_pages/0000a_anintroexample.rst
 doc/unused_pages/0000a_objectoverview.rst
 doc/unused_pages/0000a_tskit_interchange.rst
 doc/unused_pages/0000a_working_with_genotypes_trees.rst
 doc/unused_pages/mutation.rst
 doc/unused_pages/recombination.rst
 doc/unused_pages/tstimeseries.rst
@@ -103,26 +106,28 @@
 examples/gss/iterate_variants_in_tree_sequences.py
 examples/gss/plot_genetic_values_from_tree_sequences.py
 examples/gss/plotstats.R
 examples/gss_divergent_optima/gss_divergent_optima.py
 examples/plugin/CMakeLists.txt
 examples/plugin/gvalue_recorder.cc
 examples/plugin/test_plugin.py
+examples/python_genetic_values/pysnowdrift.py
 examples/tskit/precapitate.py
 examples/tskit/recapitate.py
 examples/tskit/session.py
 fwdpy11/CMakeLists.txt
 fwdpy11/__init__.py
 fwdpy11/__main__.py
 fwdpy11/_demography.py
 fwdpy11/_dev.py
 fwdpy11/_evolve_genomes.py
 fwdpy11/_evolvets.py
 fwdpy11/_version.py
 fwdpy11/class_decorators.py
+fwdpy11/custom_genetic_value_decorators.py
 fwdpy11/discrete_demography.py
 fwdpy11/ezparams.py
 fwdpy11/genetic_map_unit.py
 fwdpy11/genetic_values.py
 fwdpy11/regions.py
 fwdpy11.egg-info/PKG-INFO
 fwdpy11.egg-info/SOURCES.txt
@@ -362,14 +367,15 @@
 fwdpy11/headers/fwdpy11/discrete_demography/simulation/update_demographic_model_state.hpp
 fwdpy11/headers/fwdpy11/evolve/DiploidPopulation_generation.hpp
 fwdpy11/headers/fwdpy11/evolvets/SampleRecorder.hpp
 fwdpy11/headers/fwdpy11/evolvets/evolve_generation_ts.hpp
 fwdpy11/headers/fwdpy11/evolvets/recorders.hpp
 fwdpy11/headers/fwdpy11/evolvets/sample_recorder_types.hpp
 fwdpy11/headers/fwdpy11/evolvets/simplify_tables.hpp
+fwdpy11/headers/fwdpy11/genetic_value_data/genetic_value_data.hpp
 fwdpy11/headers/fwdpy11/genetic_value_noise/GeneticValueNoise.hpp
 fwdpy11/headers/fwdpy11/genetic_value_noise/NoNoise.hpp
 fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GSSmo.hpp
 fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsFitness.hpp
 fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueIsTrait.hpp
 fwdpy11/headers/fwdpy11/genetic_value_to_fitness/GeneticValueToFitnessMap.hpp
 fwdpy11/headers/fwdpy11/genetic_value_to_fitness/MultivariateGSSmo.hpp
@@ -404,17 +410,19 @@
 fwdpy11/headers/fwdpy11/serialization/backwards_compat.hpp
 fwdpy11/headers/fwdpy11/serialization/diploid_metadata.hpp
 fwdpy11/headers/fwdpy11/types/Diploid.hpp
 fwdpy11/headers/fwdpy11/types/DiploidPopulation.hpp
 fwdpy11/headers/fwdpy11/types/Mutation.hpp
 fwdpy11/headers/fwdpy11/types/Population.hpp
 fwdpy11/headers/fwdpy11/types/typedefs.hpp
+fwdpy11/headers/fwdpy11/util/array_proxy.hpp
 fwdpy11/headers/fwdpy11/util/clone_cloneable.hpp
 fwdpy11/headers/fwdpy11/util/convert_lists.hpp
 fwdpy11/src/_fwdpy11.cc
+fwdpy11/src/array_proxies/init.cc
 fwdpy11/src/discrete_demography/DiscreteDemography.cc
 fwdpy11/src/discrete_demography/MassMigration.cc
 fwdpy11/src/discrete_demography/MigrationMatrix.cc
 fwdpy11/src/discrete_demography/SetDemeSize.cc
 fwdpy11/src/discrete_demography/SetExponentialGrowth.cc
 fwdpy11/src/discrete_demography/SetMigrationRates.cc
 fwdpy11/src/discrete_demography/SetSelfingRate.cc
@@ -492,14 +500,15 @@
 fwdpy11/src/genetic_value_to_fitness/PleiotropicOptima.cc
 fwdpy11/src/genetic_value_to_fitness/init.cc
 fwdpy11/src/genetic_values/Additive.cc
 fwdpy11/src/genetic_values/DiploidGeneticValue.cc
 fwdpy11/src/genetic_values/DiploidMultivariateEffectsStrictAdditive.cc
 fwdpy11/src/genetic_values/GBR.cc
 fwdpy11/src/genetic_values/Multiplicative.cc
+fwdpy11/src/genetic_values/PyDiploidGeneticValue.cc
 fwdpy11/src/genetic_values/dgvalue_pointer_vector.cc
 fwdpy11/src/genetic_values/init.cc
 fwdpy11/src/gsl/gsl_random.cc
 fwdpy11/src/gsl/init.cc
 fwdpy11/src/regions/ConstantS.cc
 fwdpy11/src/regions/ExpS.cc
 fwdpy11/src/regions/GammaS.cc
@@ -538,14 +547,18 @@
 tests/gsl_error.cc
 tests/inherit_noise.cc
 tests/ll_snowdrift.cc
 tests/numpy_array_interface.cc
 tests/pickling_composed_classes.cc
 tests/pickling_cpp.cc
 tests/poptools.cc
+tests/pyadditive.py
+tests/pyadditivegss.py
+tests/pygss.py
+tests/pynoise.py
 tests/quick_pops.py
 tests/snowdrift.py
 tests/sregion_cdf.cc
 tests/testMultivariateGSSmo.cc
 tests/test_DataMatrix.py
 tests/test_DemographyDebugger.py
 tests/test_DiploidPopulation.py
@@ -556,14 +569,15 @@
 tests/test_Sregion_from_cdf.py
 tests/test_TableCollection_fs.py
 tests/test_add_mutation.py
 tests/test_binary_format_compatibility.py
 tests/test_class_decorators.py
 tests/test_custom_exceptions.py
 tests/test_custom_stateless_fitness.py
+tests/test_demographic_event_verbs.py
 tests/test_demographic_models.py
 tests/test_dgvalue_pointer_vector.py
 tests/test_discrete_demography.py
 tests/test_discrete_demography_with_tree_sequences.py
 tests/test_fixation_properties.py
 tests/test_fwdpp_types.py
 tests/test_genetic_value_noise.py
@@ -573,14 +587,15 @@
 tests/test_multivariate_effects.py
 tests/test_mutation_labels.py
 tests/test_numpy.py
 tests/test_numpy_array_interface.py
 tests/test_opaque.py
 tests/test_pickling.py
 tests/test_pickling_composed_classes.py
+tests/test_python_genetic_values.py
 tests/test_record_genetic_value_matrix.py
 tests/test_regions.py
 tests/test_simple_parallel.py
 tests/test_stateful_fitness.py
 tests/test_stopping_criterion.py
 tests/test_tree_sequences.py
 tests/test_tree_sequences_different_des_in_different_demes.py
```

### Comparing `fwdpy11-0.8.3/gplheader.txt` & `fwdpy11-0.9.0/gplheader.txt`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/gplheader_cpp.txt` & `fwdpy11-0.9.0/gplheader_cpp.txt`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/index.md` & `fwdpy11-0.9.0/index.md`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/install-sh` & `fwdpy11-0.9.0/install-sh`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/m4/ax_cxx_compile_stdxx_11.m4` & `fwdpy11-0.9.0/m4/ax_cxx_compile_stdxx_11.m4`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/m4/python.m4` & `fwdpy11-0.9.0/m4/python.m4`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/setup.py` & `fwdpy11-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,14 @@
 if sys.version_info[0] < 3:
     raise ValueError("Python 3 is required!")
 
 if pybind11.__version__ < PYBIND11_MIN_VERSION:
     raise RuntimeError(f"pybind11 >= {PYBIND11_MIN_VERSION} required")
 
 
-# clang/llvm is default for OS X builds.
-# can over-ride darwin-specific options
-# with setup.py --gcc install
-if "--gcc" in sys.argv:
-    USE_GCC = True
-    sys.argv.remove("--gcc")
-else:
-    USE_GCC = False
-
 if "--weffcpp" in sys.argv:
     USE_WEFFCPP = True
     sys.argv.remove("--weffcpp")
 else:
     USE_WEFFCPP = False
 
 if "--debug" in sys.argv:
```

### Comparing `fwdpy11-0.8.3/tests/CMakeLists.txt` & `fwdpy11-0.9.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/EsizeZero.cc` & `fwdpy11-0.9.0/tests/EsizeZero.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/call_Sregion.cc` & `fwdpy11-0.9.0/tests/call_Sregion.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/common_mako.py` & `fwdpy11-0.9.0/tests/common_mako.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/custom_additive.cc` & `fwdpy11-0.9.0/tests/custom_additive.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #include <algorithm> //for std::max
 #include <pybind11/pybind11.h>
 #include <fwdpy11/genetic_values/DiploidGeneticValue.hpp>
 #include <fwdpy11/genetic_values/default_update.hpp>
 
 struct additive : public fwdpy11::DiploidGeneticValue
 {
-    additive() : fwdpy11::DiploidGeneticValue(1) {}
+    additive() : fwdpy11::DiploidGeneticValue{1, nullptr, nullptr}
+    {
+    }
 
     double
-    calculate_gvalue(const std::size_t diploid_index,
-                     const fwdpy11::DiploidMetadata& /*metadata*/,
-                     const fwdpy11::DiploidPopulation& pop) const override
+    calculate_gvalue(const fwdpy11::DiploidGeneticValueData data) override
     {
+        const auto& pop = data.pop.get();
+        const auto diploid_index = data.offspring_metadata.get().label;
         double sum = 0;
-        for (auto m :
-             pop.haploid_genomes[pop.diploids[diploid_index].first].smutations)
+        for (auto m : pop.haploid_genomes[pop.diploids[diploid_index].first].smutations)
             {
                 sum += pop.mutations[m].s;
             }
-        for (auto m : pop.haploid_genomes[pop.diploids[diploid_index].second]
-                          .smutations)
+        for (auto m : pop.haploid_genomes[pop.diploids[diploid_index].second].smutations)
             {
                 sum += pop.mutations[m].s;
             }
         gvalues[0] = std::max(0.0, 1.0 + sum);
         return gvalues[0];
     }
```

### Comparing `fwdpy11-0.8.3/tests/custom_stateless_genotype.cc` & `fwdpy11-0.9.0/tests/custom_stateless_genotype.cc`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 #include <fwdpy11/genetic_values/DiploidGeneticValue.hpp>
 #include <fwdpy11/genetic_values/default_update.hpp>
 
 struct GeneralW : public fwdpy11::DiploidGeneticValue
 {
     fwdpp::site_dependent_genetic_value w;
 
-    GeneralW() : fwdpy11::DiploidGeneticValue{ 1 }, w{} {}
+    GeneralW() : fwdpy11::DiploidGeneticValue{1, nullptr, nullptr}, w{}
+    {
+    }
 
     inline double
-    calculate_gvalue(const std::size_t diploid_index,
-                     const fwdpy11::DiploidMetadata& /*metadata*/,
-                     const fwdpy11::DiploidPopulation& pop) const override
+    calculate_gvalue(const fwdpy11::DiploidGeneticValueData data) override
     {
-        gvalues[0]
-            = std::max(0.0, w(
-                                pop.diploids[diploid_index],
-                                pop.haploid_genomes, pop.mutations,
-                                [](double& g, const fwdpy11::Mutation& m) {
-                                    g *= (1.0 + m.s);
-                                },
-                                [](double& g, const fwdpy11::Mutation& m) {
-                                    g *= (1.0 + m.h);
-                                }, 1.0));
+        gvalues[0] = std::max(
+            0.0,
+            w(
+                data.pop.get().diploids[data.offspring_metadata.get().label],
+                data.pop.get().haploid_genomes, data.pop.get().mutations,
+                [](double& g, const fwdpy11::Mutation& m) { g *= (1.0 + m.s); },
+                [](double& g, const fwdpy11::Mutation& m) { g *= (1.0 + m.h); }, 1.0));
         return gvalues[0];
     }
 
     pybind11::object
     pickle() const
     {
         return pybind11::bytes("custom_stateless_genotype");
```

### Comparing `fwdpy11-0.8.3/tests/discrete_demography_roundtrips.cc` & `fwdpy11-0.9.0/tests/discrete_demography_roundtrips.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/fixation_properties.cc` & `fwdpy11-0.9.0/tests/fixation_properties.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/gsl_error.cc` & `fwdpy11-0.9.0/tests/gsl_error.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/inherit_noise.cc` & `fwdpy11-0.9.0/tests/inherit_noise.cc`

 * *Files 21% similar despite different names*

```diff
@@ -18,32 +18,34 @@
 //
 
 #include <pybind11/pybind11.h>
 #include <fwdpy11/genetic_value_noise/GeneticValueNoise.hpp>
 
 struct IneritedNoise : public fwdpy11::GeneticValueNoise
 {
+    std::uint32_t generation;
+
+    IneritedNoise() : GeneticValueNoise{}, generation{} {}
+
     double
-    operator()(const fwdpy11::GSLrng_t& /*rng*/,
-               const fwdpy11::DiploidMetadata& /*offspring_metadata*/,
-               const std::size_t parent1, const std::size_t /*parent2*/,
-               const fwdpy11::DiploidPopulation& pop) const override
+    operator()(const fwdpy11::DiploidGeneticValueNoiseData data) const override
     {
-        return pop.diploid_metadata[parent1].e + pop.generation;
+        return data.parent1_metadata.get().e + generation;
     }
 
     void
-    update(const fwdpy11::DiploidPopulation& /*pop*/) override
+    update(const fwdpy11::DiploidPopulation& pop) override
     {
+        generation = pop.generation;
     }
 
-    std::unique_ptr<fwdpy11::GeneticValueNoise>
+    std::shared_ptr<fwdpy11::GeneticValueNoise>
     clone() const override
     {
-        return std::unique_ptr<IneritedNoise>(new IneritedNoise());
+        return std::make_shared<IneritedNoise>();
     }
 
     pybind11::object
     pickle() const
     {
         return pybind11::bytes("IneritedNoise");
     }
@@ -61,14 +63,13 @@
 };
 
 PYBIND11_MODULE(inherit_noise, m)
 {
     pybind11::object imported_base
         = pybind11::module::import("fwdpy11").attr("GeneticValueNoise");
 
-    pybind11::class_<IneritedNoise, fwdpy11::GeneticValueNoise>(
-        m, "IneritedNoise")
+    pybind11::class_<IneritedNoise, fwdpy11::GeneticValueNoise>(m, "IneritedNoise")
         .def(pybind11::init<>())
         .def(pybind11::pickle(
             [](const IneritedNoise& self) { return self.pickle(); },
             [](pybind11::object o) { return IneritedNoise::unpickle(o); }));
 }
```

### Comparing `fwdpy11-0.8.3/tests/ll_snowdrift.cc` & `fwdpy11-0.9.0/tests/ll_snowdrift.cc`

 * *Files 16% similar despite different names*

```diff
@@ -26,101 +26,84 @@
  * The phenotypes get updated each generation during
  * the simulation.
  *
  * The phenotypes will be the simple additive model,
  * calculated using fwdpp's machinery.
  */
 {
-    const double b1, b2, c1, c2;
+    const double b1, b2, c1, c2, slope, sig0;
     // This is our stateful data,
     // which is a record of the
     // additive genetic values of all
     // diploids
     std::vector<double> phenotypes;
+    const fwdpp::additive_diploid additive;
 
     // This constructor is exposed to Python
-    snowdrift(double b1_, double b2_, double c1_, double c2_)
-        : fwdpy11::DiploidGeneticValue{ 1 }, b1(b1_), b2(b2_), c1(c1_),
-          c2(c2_), phenotypes()
-    {
-    }
-
-    //This constructor makes object unpickling
-    //a bit more idiomatic from the C++ point
-    //of view.  We implement it as a so-called
-    //"perfect-forwarding constructor" to
-    //initialize the phenotypes w/o extra copies.
-    template <typename T>
-    snowdrift(double b1_, double b2_, double c1_, double c2_, T &&p)
-        : fwdpy11::DiploidGeneticValue{ 1 }, b1(b1_), b2(b2_), c1(c1_),
-          c2(c2_), phenotypes(std::forward<T>(p))
+    snowdrift(double b1_, double b2_, double c1_, double c2_, double slope, double p0)
+        : fwdpy11::DiploidGeneticValue{1, nullptr, nullptr}, b1(b1_), b2(b2_), c1(c1_),
+          c2(c2_), slope(slope), sig0(1. / slope * std::log(p0 / (1. - p0))),
+          phenotypes(), additive{fwdpp::trait{2.0}}
     {
+        if (p0 == 0 || p0 == 1.)
+            {
+                throw std::invalid_argument("p0 must be 0 < p0 < 1");
+            }
     }
 
     double
-    calculate_gvalue(const std::size_t diploid_index,
-                     const fwdpy11::DiploidMetadata& /*metadata*/,
-                     const fwdpy11::DiploidPopulation& /*pop*/) const override
+    calculate_gvalue(const fwdpy11::DiploidGeneticValueData data) override
     // The call operator must return the genetic value of an individual
     {
-        gvalues[0] = phenotypes[diploid_index];
+        gvalues[0] = phenotypes[data.metadata_index];
         return gvalues[0];
     }
 
     double
     genetic_value_to_fitness(
-        const fwdpy11::DiploidMetadata &metadata) const override
+        const fwdpy11::DiploidGeneticValueToFitnessData data) override
     // This function converts genetic value to fitness.
     {
-        double fitness = 0.0;
-        double zself = metadata.g;
+        double zself = data.offspring_metadata.get().g;
         auto N = phenotypes.size();
-        for (std::size_t j = 0; j < N; ++j)
+        auto other = gsl_rng_uniform_int(data.rng.get().get(), N);
+        while (other == data.offspring_metadata.get().label)
             {
-                // A record of which diploid we are
-                // processesing is the label field of the meta data.
-                if (metadata.label != j)
-                    {
-                        double zpair = zself + phenotypes[j];
-                        // Payoff function from Fig 1
-                        double a = b1 * zpair + b2 * zpair * zpair - c1 * zself
-                                   - c2 * zself * zself;
-                        fitness += 1 + std::max(a, 0.0);
-                    }
+                other = gsl_rng_uniform_int(data.rng.get().get(), N);
             }
-        return fitness / double(N - 1);
+        double zpair = zself + phenotypes[other];
+        double a
+            = 1. + b1 * zpair + b2 * zpair * zpair - c1 * zself - c2 * zself * zself;
+        return std::max(a, 0.0);
     }
 
     void
     update(const fwdpy11::DiploidPopulation &pop) override
     // A stateful fitness model needs updating.
     {
-        phenotypes.resize(pop.N);
-        for (std::size_t i = 0; i < pop.N; ++i)
+        phenotypes.clear();
+        for (auto &md : pop.diploid_metadata)
             {
                 // A diploid tracks its index via
                 // fwdpy11::DiploidMetadata::label
-                phenotypes[pop.diploid_metadata[i].label]
-                    = fwdpp::additive_diploid(fwdpp::trait(2.0))(
-                        pop.diploids[i], pop.haploid_genomes, pop.mutations);
+                auto g = additive(pop.diploids[md.label], pop.haploid_genomes,
+                                  pop.mutations);
+                phenotypes.push_back(1. / (1. + std::exp(-slope * (g + sig0))));
             }
-        // This is strictly not necessary in this specific
-        // case, but it is required in general, so we
-        // do it here by way of example.
-        noise_fxn->update(pop);
     }
 };
 
 PYBIND11_MODULE(ll_snowdrift, m)
 {
     m.doc() = "Example of custom stateful fitness model.";
 
     // We need to import the Python version of our base class:
     pybind11::object imported_snowdrift_base_class_type
         = pybind11::module::import("fwdpy11").attr("DiploidGeneticValue");
 
     // Create a Python class based on our new type
     py::class_<snowdrift, fwdpy11::DiploidGeneticValue>(m, "_ll_DiploidSnowdrift")
-        .def(py::init<double, double, double, double>(), py::arg("b1"),
-             py::arg("b2"), py::arg("c1"), py::arg("c2"))
+        .def(py::init<double, double, double, double, double, double>(), py::arg("b1"),
+             py::arg("b2"), py::arg("c1"), py::arg("c2"), py::arg("slope"),
+             py::arg("p0"))
         .def_readwrite("phenotypes", &snowdrift::phenotypes);
 }
```

### Comparing `fwdpy11-0.8.3/tests/numpy_array_interface.cc` & `fwdpy11-0.9.0/tests/numpy_array_interface.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/pickling_composed_classes.cc` & `fwdpy11-0.9.0/tests/pickling_composed_classes.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/pickling_cpp.cc` & `fwdpy11-0.9.0/tests/pickling_cpp.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/quick_pops.py` & `fwdpy11-0.9.0/tests/quick_pops.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/snowdrift.py` & `fwdpy11-0.9.0/tests/snowdrift.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 @fwdpy11.class_decorators.attr_class_to_from_dict
 @attr.s()
 class DiploidSnowdrift(ll_snowdrift._ll_DiploidSnowdrift):
     """
     This is the user-facing Python representation of
     a simple snowdrift model.
     """
+
     b1 = attr.ib()
     b2 = attr.ib()
     c1 = attr.ib()
     c2 = attr.ib()
+    slope = attr.ib()
+    p0 = attr.ib()
 
     def __attrs_post_init__(self):
         # Need to initialize the C++ base class
-        super(DiploidSnowdrift, self).__init__(self.b1, self.b2, self.c1, self.c2)
+        super(DiploidSnowdrift, self).__init__(
+            self.b1, self.b2, self.c1, self.c2, self.slope, self.p0
+        )
 
     def __getstate__(self):
         # asdict is provided by the 2nd class
         # decorator (reading from bottom to top)
         # We pickle this class as a tuple.
         # Element 0 contains the kwargs + values
         # needed for __init__ and we send along
```

### Comparing `fwdpy11-0.8.3/tests/sregion_cdf.cc` & `fwdpy11-0.9.0/tests/sregion_cdf.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/testMultivariateGSSmo.cc` & `fwdpy11-0.9.0/tests/testMultivariateGSSmo.cc`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_DataMatrix.py` & `fwdpy11-0.9.0/tests/test_DataMatrix.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_DemographyDebugger.py` & `fwdpy11-0.9.0/tests/test_DemographyDebugger.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_DiploidPopulation.py` & `fwdpy11-0.9.0/tests/test_DiploidPopulation.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_GSLerror.py` & `fwdpy11-0.9.0/tests/test_GSLerror.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_ModelParams.py` & `fwdpy11-0.9.0/tests/test_ModelParams.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_Mutation.py` & `fwdpy11-0.9.0/tests/test_Mutation.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_SampleRecorder.py` & `fwdpy11-0.9.0/tests/test_SampleRecorder.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_Sregion_from_cdf.py` & `fwdpy11-0.9.0/tests/test_Sregion_from_cdf.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_TableCollection_fs.py` & `fwdpy11-0.9.0/tests/test_TableCollection_fs.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_add_mutation.py` & `fwdpy11-0.9.0/tests/test_add_mutation.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_binary_format_compatibility.py` & `fwdpy11-0.9.0/tests/test_binary_format_compatibility.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_class_decorators.py` & `fwdpy11-0.9.0/tests/test_class_decorators.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_custom_exceptions.py` & `fwdpy11-0.9.0/tests/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_custom_stateless_fitness.py` & `fwdpy11-0.9.0/tests/test_custom_stateless_fitness.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_demographic_models.py` & `fwdpy11-0.9.0/tests/test_demographic_models.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_dgvalue_pointer_vector.py` & `fwdpy11-0.9.0/tests/test_dgvalue_pointer_vector.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_discrete_demography.py` & `fwdpy11-0.9.0/tests/test_discrete_demography.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_discrete_demography_with_tree_sequences.py` & `fwdpy11-0.9.0/tests/test_discrete_demography_with_tree_sequences.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_fixation_properties.py` & `fwdpy11-0.9.0/tests/test_fixation_properties.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_fwdpp_types.py` & `fwdpy11-0.9.0/tests/test_fwdpp_types.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_genetic_value_noise.py` & `fwdpy11-0.9.0/tests/test_genetic_value_noise.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_genetic_value_to_fitness.py` & `fwdpy11-0.9.0/tests/test_genetic_value_to_fitness.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_genetic_values.py` & `fwdpy11-0.9.0/tests/test_genetic_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,32 +160,9 @@
         self.x = fwdpy11.GSS(0.0, 1.0)
 
     def testProperties(self):
         self.assertEqual(self.x.optimum, 0.0)
         self.assertEqual(self.x.VS, 1.0)
 
 
-class testGSSandGSSmoConsistency(unittest.TestCase):
-    """
-    This tests that GSS and GSSmo have opt and VS
-    in the same order.  If that were not true,
-    fitness calculations would come out differently
-    and the test would fail.
-    """
-
-    @classmethod
-    def setUp(self):
-        self.a = fwdpy11.Additive(2.0, fwdpy11.GSS(0.0, 1.0))
-        self.b = fwdpy11.Additive(
-            2.0, fwdpy11.GSSmo([fwdpy11.Optimum(when=0, optimum=0.0, VS=1.0)])
-        )
-        self.pop = fwdpy11.DiploidPopulation(1000)
-
-    def testFitnesses(self):
-        wa = [self.a.fitness(i, self.pop) for i in range(self.pop.N)]
-        wb = [self.b.fitness(i, self.pop) for i in range(self.pop.N)]
-        for i, j in zip(wa, wb):
-            self.assertEqual(i, j)
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `fwdpy11-0.8.3/tests/test_inherited_noise.py` & `fwdpy11-0.9.0/tests/test_inherited_noise.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,18 +36,18 @@
             ),
         }
 
     def test_noise_values_tree_sequences(self):
         params = fwdpy11.ModelParams(**self.pdict)
         fwdpy11.evolvets(self.rng, self.pop, params, 100)
         self.assertEqual(self.pop.generation, 3)
-        self.assertTrue(all([i.e == 6 for i in self.pop.diploid_metadata]) is True)
+        self.assertTrue(all([i.e == 6.0 for i in self.pop.diploid_metadata]) is True)
 
     def test_noise_values_without_tree_sequences(self):
         params = fwdpy11.ModelParams(**self.pdict)
         fwdpy11.evolve_genomes(self.rng, self.pop, params)
         self.assertEqual(self.pop.generation, 3)
-        self.assertTrue(all([i.e == 6 for i in self.pop.diploid_metadata]) is True)
+        self.assertTrue(all([i.e == 6.0 for i in self.pop.diploid_metadata]) is True)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `fwdpy11-0.8.3/tests/test_multivariate_effects.py` & `fwdpy11-0.9.0/tests/test_multivariate_effects.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_mutation_labels.py` & `fwdpy11-0.9.0/tests/test_mutation_labels.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_numpy.py` & `fwdpy11-0.9.0/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_numpy_array_interface.py` & `fwdpy11-0.9.0/tests/test_numpy_array_interface.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_opaque.py` & `fwdpy11-0.9.0/tests/test_opaque.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_pickling.py` & `fwdpy11-0.9.0/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_record_genetic_value_matrix.py` & `fwdpy11-0.9.0/tests/test_record_genetic_value_matrix.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_regions.py` & `fwdpy11-0.9.0/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_simple_parallel.py` & `fwdpy11-0.9.0/tests/test_simple_parallel.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_stateful_fitness.py` & `fwdpy11-0.9.0/tests/test_stateful_fitness.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import pickle
 import unittest
 
 import numpy as np
 
 import fwdpy11 as fp11
 import fwdpy11.ezparams
@@ -12,24 +13,28 @@
     """
     Temporal sampler checks that one can hook
     a stateful fitness model to a sampler
     and access its data and that the data
     are as expected.
     """
 
-    def __init__(self, f):
+    def __init__(self, f, slope, p0):
         self.f = f
+        self.slope = slope
+        self.p0 = p0
+        self.sig0 = (1.0 / slope) * math.log(self.p0 / (1.0 - self.p0))
 
     def __call__(self, pop, sampler):
         for i in range(pop.N):
             w = 0.0
             for m in pop.haploid_genomes[pop.diploids[i].first].smutations:
                 w += pop.mutations[m].s
             for m in pop.haploid_genomes[pop.diploids[i].second].smutations:
                 w += pop.mutations[m].s
+            w = 1.0 / (1.0 + math.exp(-self.slope * (w + self.sig0)))
             assert np.isclose(w, self.f.phenotypes[i])
 
 
 def evolve_snowdrift(args):
     """
     We write the function taking a tuple
     out of habit, simplifying later
@@ -42,33 +47,33 @@
     pop = fp11.DiploidPopulation(N, 1.0)
     # Initialize a random number generator
     rng = fp11.GSLrng(seed)
     p = {
         "sregions": [fp11.ExpS(0, 1, 1, -0.1, 1.0)],
         "recregions": [fp11.Region(0, 1, 1)],
         "nregions": [],
-        "gvalue": snowdrift.DiploidSnowdrift(0.2, -0.2, 1, -2),
+        "gvalue": snowdrift.DiploidSnowdrift(0.2, -0.2, 1, -2, 1, 0.3),
         # evolve for 100 generations so that unit tests are
         # fast
         "demography": fwdpy11.DiscreteDemography(),
         "simlen": 20,
         "rates": (0.0, 0.0025, 0.001),
         "prune_selected": False,
     }
     params = fwdpy11.ModelParams(**p)
-    sampler = SamplePhenotypes(params.gvalue)
+    sampler = SamplePhenotypes(params.gvalue, 1, 0.3)
     fp11.evolvets(rng, pop, params, 100, sampler)
     # return our pop
     return pop
 
 
 class testSnowdrift(unittest.TestCase):
     @classmethod
     def setUp(self):
-        self.f = snowdrift.DiploidSnowdrift(1, -1, 0.1, 0.2)
+        self.f = snowdrift.DiploidSnowdrift(1, -1, 0.1, 0.2, 1, 0.3)
 
     def testShape(self):
         s = self.f.shape
         self.assertEqual(len(s), 1)
         self.assertEqual(s[0], 1)
 
     def test_genetic_values(self):
```

### Comparing `fwdpy11-0.8.3/tests/test_stopping_criterion.py` & `fwdpy11-0.9.0/tests/test_stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_tree_sequences.py` & `fwdpy11-0.9.0/tests/test_tree_sequences.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_tree_sequences_different_des_in_different_demes.py` & `fwdpy11-0.9.0/tests/test_tree_sequences_different_des_in_different_demes.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_tree_sequences_esize_zero_selected_variants.py` & `fwdpy11-0.9.0/tests/test_tree_sequences_esize_zero_selected_variants.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_tree_sequences_with_neutral_mutations.py` & `fwdpy11-0.9.0/tests/test_tree_sequences_with_neutral_mutations.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_ts_from_msprime.py` & `fwdpy11-0.9.0/tests/test_ts_from_msprime.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_util.py` & `fwdpy11-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/test_wright_fisher.py` & `fwdpy11-0.9.0/tests/test_wright_fisher.py`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/v045.bin` & `fwdpy11-0.9.0/tests/v045.bin`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/tests/v045.lzma` & `fwdpy11-0.9.0/tests/v045.lzma`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/travis_scripts/build_script.sh` & `fwdpy11-0.9.0/travis_scripts/build_script.sh`

 * *Files identical despite different names*

### Comparing `fwdpy11-0.8.3/travis_scripts/installation_script.sh` & `fwdpy11-0.9.0/travis_scripts/installation_script.sh`

 * *Files identical despite different names*

