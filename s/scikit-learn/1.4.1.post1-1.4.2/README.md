# Comparing `tmp/scikit-learn-1.4.1.post1.tar.gz` & `tmp/scikit-learn-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-learn-1.4.1.post1.tar", last modified: Thu Feb 15 14:01:57 2024, max compression
+gzip compressed data, was "scikit-learn-1.4.2.tar", last modified: Tue Apr  9 14:20:32 2024, max compression
```

## Comparing `scikit-learn-1.4.1.post1.tar` & `scikit-learn-1.4.2.tar`

### file list

```diff
@@ -1,1603 +1,1604 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.882463 scikit-learn-1.4.1.post1/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-02-15 14:01:57.882463 scikit-learn-1.4.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.650464 scikit-learn-1.4.1.post1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/authors_emeritus.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.650464 scikit-learn-1.4.1.post1/doc/binder/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25058 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/common_pitfalls.rst
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/communication_team.rst
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/communication_team_emeritus.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.650464 scikit-learn-1.4.1.post1/doc/computing/
--rw-r--r--   0 runner    (1001) docker     (127)    17218 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/computing/computational_performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/computing/parallelism.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/computing/scaling_strategies.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/computing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    27224 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/contents.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/contributor_experience_team.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/contributor_experience_team_emeritus.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/data_transforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.654464 scikit-learn-1.4.1.post1/doc/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/datasets/loading_other_datasets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/datasets/real_world.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/datasets/sample_generators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/datasets/toy_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.654464 scikit-learn-1.4.1.post1/doc/developers/
--rw-r--r--   0 runner    (1001) docker     (127)    19897 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/advanced_installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/bug_triaging.rst
--rw-r--r--   0 runner    (1001) docker     (127)    61458 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/cython.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38663 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/develop.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/maintainer.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15265 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/minimal_reproducer.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/tips.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/developers/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/dispatching.rst
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/documentation_team.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23949 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)    90170 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/governance.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.666464 scikit-learn-1.4.1.post1/doc/images/
--rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/axa-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    17847 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/axa.png
--rw-r--r--   0 runner    (1001) docker     (127)    31049 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/bcg.png
--rw-r--r--   0 runner    (1001) docker     (127)    54774 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/beta_divergence.png
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/bnp-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    21156 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/bnp.png
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/cds-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/chanel-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/chanel.png
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/columbia-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/columbia.png
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/czi_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/dataiku-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/dataiku.png
--rw-r--r--   0 runner    (1001) docker     (127)    18585 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/digicosme.png
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/dysco.png
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/fnrs-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    18012 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/fujitsu.png
--rw-r--r--   0 runner    (1001) docker     (127)    89394 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/generated-doc-ci.png
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/google-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    45148 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/grid_search_cross_validation.png
--rw-r--r--   0 runner    (1001) docker     (127)   101880 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/grid_search_workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/huggingface_logo-noborder.png
--rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/inria-logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/inria-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/intel-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/intel.png
--rw-r--r--   0 runner    (1001) docker     (127)    27033 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/iris.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/iris.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/last_digit.png
--rw-r--r--   0 runner    (1001) docker     (127)    13032 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/lda_model_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/logo_APHP.png
--rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/logo_APHP_text.png
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/microsoft-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/microsoft.png
--rw-r--r--   0 runner    (1001) docker     (127)   761071 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/ml_map.png
--rw-r--r--   0 runner    (1001) docker     (127)    26546 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/multi_org_chart.png
--rw-r--r--   0 runner    (1001) docker     (127)    89381 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/multilayerperceptron_network.png
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/no_image.png
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/nvidia-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    10764 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/nvidia.png
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/nyu_short_color.png
--rw-r--r--   0 runner    (1001) docker     (127)    45027 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/permuted_non_predictive_feature.png
--rw-r--r--   0 runner    (1001) docker     (127)    43181 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/permuted_predictive_feature.png
--rw-r--r--   0 runner    (1001) docker     (127)    31108 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/plot_digits_classification.png
--rw-r--r--   0 runner    (1001) docker     (127)   124459 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/plot_face_recognition_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    86623 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/plot_face_recognition_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/png-logo-inria-la-fondation.png
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/quansight-labs-small.png
--rw-r--r--   0 runner    (1001) docker     (127)   124931 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/quansight-labs.png
--rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/rbm_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/scikit-learn-logo-notext.png
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/scikit-learn-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    29042 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/sloan_banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/sloan_logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    38356 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/sydney-primary.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/sydney-stacked-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    32077 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/target_encoder_cross_validation.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/telecom-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    35103 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/telecom.png
--rw-r--r--   0 runner    (1001) docker     (127)    84599 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/images/visual-studio-build-tools-selection.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.666464 scikit-learn-1.4.1.post1/doc/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/includes/big_toc_css.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/includes/bigger_toc_css.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/jupyter_lite_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.666464 scikit-learn-1.4.1.post1/doc/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    48838 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/1280px-scikit-learn-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.666464 scikit-learn-1.4.1.post1/doc/logos/brand_colors/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/brand_colors/colorswatch_29ABE2_cyan.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/brand_colors/colorswatch_9B4600_brown.png
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/brand_colors/colorswatch_F7931E_orange.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.666464 scikit-learn-1.4.1.post1/doc/logos/brand_guidelines/
--rw-r--r--   0 runner    (1001) docker     (127)   104582 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/brand_guidelines/scikitlearn_logo_clearspace_updated.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2238 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/favicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)   120865 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/identity.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-notext.png
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-thumb.png
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-without-subtitle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    37902 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo.bmp
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/metadata_routing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/model_persistence.rst
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/model_selection.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.674464 scikit-learn-1.4.1.post1/doc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/array_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/biclustering.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/calibration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    42830 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    94103 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/clustering.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24659 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/compose.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/covariance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/cross_decomposition.rst
--rw-r--r--   0 runner    (1001) docker     (127)    40831 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    46874 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/decomposition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/density.rst
--rw-r--r--   0 runner    (1001) docker     (127)    70083 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/ensemble.rst
--rw-r--r--   0 runner    (1001) docker     (127)    44474 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/feature_extraction.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/feature_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24659 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/gaussian_process.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.674464 scikit-learn-1.4.1.post1/doc/modules/glm_data/
--rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/glm_data/lasso_enet_coordinate_descent.png
--rw-r--r--   0 runner    (1001) docker     (127)    63830 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/glm_data/poisson_gamma_tweedie_distributions.png
--rw-r--r--   0 runner    (1001) docker     (127)    33777 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/grid_search.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/impute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/isotonic.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/kernel_approximation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/kernel_ridge.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/lda_qda.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/learning_curve.rst
--rw-r--r--   0 runner    (1001) docker     (127)    79723 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/linear_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30280 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/manifold.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/mixture.rst
--rw-r--r--   0 runner    (1001) docker     (127)   121343 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/multiclass.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/naive_bayes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38706 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/neighbors.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/neural_networks_supervised.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/neural_networks_unsupervised.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/outlier_detection.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/partial_dependence.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/permutation_importance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    53915 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/preprocessing_targets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/random_projection.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/semi_supervised.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24946 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/sgd.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34865 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/svm.rst
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/tree.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/modules/unsupervised_reduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/preface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/presentations.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/related_projects.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/roadmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.674464 scikit-learn-1.4.1.post1/doc/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/sphinxext/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/sphinxext/add_toctree_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1908 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/sphinxext/allow_nan_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/sphinxext/doi_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/sphinxext/github_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/sphinxext/sphinx_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/supervised_learning.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.678464 scikit-learn-1.4.1.post1/doc/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/class_with_call.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/deprecated_class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/deprecated_class_with_call.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/deprecated_class_without_init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/deprecated_function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/display_all_class_methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/display_only_from_estimator.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/function.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/generate_deprecated.sh
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/numpydoc_docstring.rst
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/templates/redirects.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.678464 scikit-learn-1.4.1.post1/doc/testimonials/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/testimonials/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    41412 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/aweber.png
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/bestofmedia-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/betaworks.png
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/birchbox.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    65058 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/bnp_paribas_cardif.png
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/booking.png
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/change-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/dataiku_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/datapublica.png
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/datarobot.png
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/evernote.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/howaboutwe.png
--rw-r--r--   0 runner    (1001) docker     (127)    31051 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/huggingface.png
--rw-r--r--   0 runner    (1001) docker     (127)    85087 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/infonea.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/inria.png
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/jpmorgan.png
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/lovely.png
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/machinalis.png
--rw-r--r--   0 runner    (1001) docker     (127)    47018 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/mars.png
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/okcupid.png
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/ottogroup_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/peerindex.png
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/phimeca.png
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/rangespan.png
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/solido_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/spotify.png
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/telecomparistech.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/yhat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22810 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/images/zopa.png
--rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/testimonials/testimonials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.630464 scikit-learn-1.4.1.post1/doc/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/javascript.html
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.630464 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    26939 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)   155712 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/css/vendor/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/details-permalink.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    58030 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/vendor/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    72818 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/vendor/jquery-3.6.3.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/theme.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tune_toc.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.682464 scikit-learn-1.4.1.post1/doc/tutorial/basic/
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/basic/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/common_includes/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/common_includes/info.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/ML_MAPS_README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/parse_path.py
--rw-r--r--   0 runner    (1001) docker     (127)   230678 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/svg2imagemap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/putting_together.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/supervised_learning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/unsupervised_learning.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.630464 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/languages/
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/languages/fetch_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/movie_reviews/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/movie_reviews/fetch_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/skeletons/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/skeletons/exercise_01_language_train_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/skeletons/exercise_02_sentiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.686464 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/exercise_01_language_train_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/exercise_02_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/generate_skeletons.py
--rw-r--r--   0 runner    (1001) docker     (127)    21039 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/working_with_text_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/unsupervised_learning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/visualizations.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.690464 scikit-learn-1.4.1.post1/doc/whats_new/
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/_contributors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/changelog_legend.inc
--rw-r--r--   0 runner    (1001) docker     (127)    44658 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/older_versions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.13.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.14.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.15.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23270 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.16.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.17.rst
--rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.18.rst
--rw-r--r--   0 runner    (1001) docker     (127)    48325 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.19.rst
--rw-r--r--   0 runner    (1001) docker     (127)    79828 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.20.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50044 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.21.rst
--rw-r--r--   0 runner    (1001) docker     (127)    52900 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.22.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38648 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.23.rst
--rw-r--r--   0 runner    (1001) docker     (127)    46490 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v0.24.rst
--rw-r--r--   0 runner    (1001) docker     (127)    57815 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)    65715 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)    48895 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)    45212 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)    48026 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new/v1.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/doc/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.690464 scikit-learn-1.4.1.post1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.694464 scikit-learn-1.4.1.post1/examples/applications/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31775 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_cyclical_feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_digits_denoising.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_face_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_model_complexity_influence.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_out_of_core_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_outlier_detection_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_prediction_latency.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_species_distribution_modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_stock_market.py
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_time_series_lagged_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_tomography_l1_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/plot_topics_extraction_with_nmf_lda.py
--rw-r--r--   0 runner    (1001) docker     (127)    11537 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/svm_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/applications/wikipedia_principal_eigenvector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.694464 scikit-learn-1.4.1.post1/examples/bicluster/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/bicluster/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/bicluster/plot_bicluster_newsgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/bicluster/plot_spectral_biclustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/bicluster/plot_spectral_coclustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.694464 scikit-learn-1.4.1.post1/examples/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/calibration/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/calibration/plot_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/calibration/plot_calibration_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/calibration/plot_calibration_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/calibration/plot_compare_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.694464 scikit-learn-1.4.1.post1/examples/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/classification/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/classification/plot_classification_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/classification/plot_classifier_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/classification/plot_digits_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/classification/plot_lda.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/classification/plot_lda_qda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.702464 scikit-learn-1.4.1.post1/examples/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_adjusted_for_chance_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_affinity_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_agglomerative_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_agglomerative_clustering_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_agglomerative_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_birch_vs_minibatchkmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_bisect_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_cluster_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_cluster_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_coin_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_coin_ward_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_color_quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_dbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_dict_face_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_digits_agglomeration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_digits_linkage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_face_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_feature_agglomeration_vs_univariate_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_inductive_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_plusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_silhouette_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_stability_low_dim_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_linkage_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_mean_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_mini_batch_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_segmentation_toy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cluster/plot_ward_structured_vs_unstructured.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.702464 scikit-learn-1.4.1.post1/examples/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/plot_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/plot_column_transformer_mixed_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/plot_compare_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/plot_digits_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/plot_feature_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/compose/plot_transformed_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.702464 scikit-learn-1.4.1.post1/examples/covariance/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/covariance/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/covariance/plot_covariance_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/covariance/plot_lw_vs_oas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/covariance/plot_mahalanobis_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/covariance/plot_robust_vs_empirical_covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/covariance/plot_sparse_cov.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.702464 scikit-learn-1.4.1.post1/examples/cross_decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cross_decomposition/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cross_decomposition/plot_compare_cross_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/cross_decomposition/plot_pcr_vs_pls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.702464 scikit-learn-1.4.1.post1/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/datasets/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/datasets/plot_digits_last_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/datasets/plot_iris_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/datasets/plot_random_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/datasets/plot_random_multilabel_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.706464 scikit-learn-1.4.1.post1/examples/decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_faces_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_ica_blind_source_separation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_ica_vs_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_image_denoising.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_kernel_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_pca_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_pca_vs_fa_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_pca_vs_lda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_sparse_coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/decomposition/plot_varimax_fa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.706464 scikit-learn-1.4.1.post1/examples/developing_estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/developing_estimators/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/developing_estimators/sklearn_is_fitted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.710464 scikit-learn-1.4.1.post1/examples/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_adaboost_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_adaboost_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_adaboost_twoclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_bias_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_ensemble_oob.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_feature_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_hist_grad_boosting_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_importances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_importances_faces.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_oob.py
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_isolation_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_monotonic_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_random_forest_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_random_forest_regression_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_stack_predictors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_voting_decision_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_voting_probas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/ensemble/plot_voting_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.710464 scikit-learn-1.4.1.post1/examples/exercises/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/exercises/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/exercises/plot_cv_diabetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/exercises/plot_digits_classification_exercise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/exercises/plot_iris_exercise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.710464 scikit-learn-1.4.1.post1/examples/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/plot_f_test_vs_mi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/plot_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/plot_feature_selection_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/plot_rfe_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/plot_rfe_with_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/feature_selection/plot_select_from_model_diabetes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.714464 scikit-learn-1.4.1.post1/examples/gaussian_process/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_compare_gpr_krr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc_isoprobability.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc_xor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_co2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_noisy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_noisy_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_on_structured_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_prior_posterior.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.714464 scikit-learn-1.4.1.post1/examples/impute/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/impute/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/impute/plot_iterative_imputer_variants_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/impute/plot_missing_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.714464 scikit-learn-1.4.1.post1/examples/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/inspection/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/inspection/plot_causal_interpretation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/inspection/plot_linear_model_coefficient_interpretation.py
--rw-r--r--   0 runner    (1001) docker     (127)    21224 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/inspection/plot_partial_dependence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/inspection/plot_permutation_importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/inspection/plot_permutation_importance_multicollinear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.714464 scikit-learn-1.4.1.post1/examples/kernel_approximation/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/kernel_approximation/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/kernel_approximation/plot_scalable_poly_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.722464 scikit-learn-1.4.1.post1/examples/linear_model/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_bayesian_ridge_curvefit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_elastic_net_precomputed_gram_matrix_with_weighted_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_huber_vs_ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_iris_logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_and_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_coordinate_descent_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_dense_vs_sparse_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_lars_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic_l1_l2_sparsity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic_multinomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_multi_task_lasso_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_nnls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ols_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ols_ridge_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_omp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22613 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_poisson_regression_non_normal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_polynomial_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_quantile_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ransac.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ridge_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_ridge_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_robust_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_penalties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_separating_hyperplane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_weighted_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sgdocsvm_vs_ocsvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sparse_logistic_regression_20newsgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_sparse_logistic_regression_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_theilsen.py
--rw-r--r--   0 runner    (1001) docker     (127)    23618 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/linear_model/plot_tweedie_regression_insurance_claims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.722464 scikit-learn-1.4.1.post1/examples/manifold/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/plot_compare_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/plot_lle_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/plot_manifold_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/plot_mds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/plot_swissroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/manifold/plot_t_sne_perplexity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.722464 scikit-learn-1.4.1.post1/examples/miscellaneous/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_anomaly_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_display_object_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_estimator_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_isotonic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_johnson_lindenstrauss_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_kernel_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_kernel_ridge_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    24865 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_metadata_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_multioutput_face_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16466 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_outlier_detection_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_partial_dependence_visualization_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_pipeline_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_roc_curve_visualization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/miscellaneous/plot_set_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.726464 scikit-learn-1.4.1.post1/examples/mixture/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_concentration_prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_covariances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_sin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.730464 scikit-learn-1.4.1.post1/examples/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_cv_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_refit_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)    23047 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_text_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_learning_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_likelihood_ratios.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_multi_metric_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_nested_cross_validation_iris.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_permutation_tests_for_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_randomized_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_roc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_roc_crossval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_successive_halving_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_successive_halving_iterations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_train_error_vs_test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_underfitting_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/model_selection/plot_validation_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.730464 scikit-learn-1.4.1.post1/examples/multiclass/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/multiclass/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/multiclass/plot_multiclass_overview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.730464 scikit-learn-1.4.1.post1/examples/multioutput/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/multioutput/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/multioutput/plot_classifier_chain_yeast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.730464 scikit-learn-1.4.1.post1/examples/neighbors/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/approximate_nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_caching_nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_digits_kde_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_kde_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_lof_novelty_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_lof_outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_nca_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_nca_dim_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_nca_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_nearest_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neighbors/plot_species_kde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.730464 scikit-learn-1.4.1.post1/examples/neural_networks/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neural_networks/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neural_networks/plot_mlp_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neural_networks/plot_mlp_training_curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neural_networks/plot_mnist_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/neural_networks/plot_rbm_logistic_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.734464 scikit-learn-1.4.1.post1/examples/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14781 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_all_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_discretization_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_discretization_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_map_data_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_scaling_importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/preprocessing/plot_target_encoder_cross_val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.734464 scikit-learn-1.4.1.post1/examples/release_highlights/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_0_22_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_0_23_0.py
--rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_0_24_0.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_2_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_3_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_4_0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.734464 scikit-learn-1.4.1.post1/examples/semi_supervised/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/plot_label_propagation_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/plot_label_propagation_digits_active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/plot_label_propagation_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/plot_self_training_varying_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/plot_semi_supervised_newsgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/semi_supervised/plot_semi_supervised_versus_svm_iris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.738464 scikit-learn-1.4.1.post1/examples/svm/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_custom_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_iris_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_linearsvc_support_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_oneclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_rbf_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_separating_hyperplane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_separating_hyperplane_unbalanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_anova.py
--rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_scale_c.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_svm_tie_breaking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/svm/plot_weighted_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.738464 scikit-learn-1.4.1.post1/examples/text/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/text/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/text/plot_document_classification_20newsgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/text/plot_document_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/text/plot_hashing_vs_dict_vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.738464 scikit-learn-1.4.1.post1/examples/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/tree/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/tree/plot_cost_complexity_pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/tree/plot_iris_dtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/tree/plot_tree_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/tree/plot_tree_regression_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/examples/tree/plot_unveil_tree_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.742464 scikit-learn-1.4.1.post1/scikit_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-02-15 14:01:57.000000 scikit-learn-1.4.1.post1/scikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-02-15 14:01:57.000000 scikit-learn-1.4.1.post1/scikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 14:01:57.000000 scikit-learn-1.4.1.post1/scikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 14:01:57.000000 scikit-learn-1.4.1.post1/scikit_learn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-15 14:01:57.000000 scikit-learn-1.4.1.post1/scikit_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-15 14:01:57.000000 scikit-learn-1.4.1.post1/scikit_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-15 14:01:57.882463 scikit-learn-1.4.1.post1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    23219 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.746464 scikit-learn-1.4.1.post1/sklearn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.746464 scikit-learn-1.4.1.post1/sklearn/__check_build/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/__check_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/__check_build/_check_build.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/__check_build/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.746464 scikit-learn-1.4.1.post1/sklearn/_build_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_build_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_build_utils/openmp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_build_utils/pre_build_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_build_utils/tempita.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_build_utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_distributor_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_isotonic.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.746464 scikit-learn-1.4.1.post1/sklearn/_loss/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/_loss.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    50281 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/_loss.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    41236 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.746464 scikit-learn-1.4.1.post1/sklearn/_loss/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    48281 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_loss/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/_min_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    53077 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    49547 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.750464 scikit-learn-1.4.1.post1/sklearn/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_affinity_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    49039 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_agglomerative.py
--rw-r--r--   0 runner    (1001) docker     (127)    22157 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_bicluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    26249 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_birch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_bisect_k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_dbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_dbscan_inner.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_feature_agglomeration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.750464 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_linkage.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_reachability.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    27800 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    41849 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.754464 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/tests/test_reachibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hierarchical_fast.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    15905 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_hierarchical_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_common.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_common.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_elkan.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_lloyd.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_minibatch.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    82683 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)    20156 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_mean_shift.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44710 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)    30496 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.754464 scikit-learn-1.4.1.post1/sklearn/cluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_affinity_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_bicluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_birch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_bisect_k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_dbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_feature_agglomeration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (127)    32593 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    48900 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_mean_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_spectral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.754464 scikit-learn-1.4.1.post1/sklearn/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57863 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/compose/_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/compose/_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.754464 scikit-learn-1.4.1.post1/sklearn/compose/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/compose/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    88405 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/compose/tests/test_column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/compose/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.758464 scikit-learn-1.4.1.post1/sklearn/covariance/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/_elliptic_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/_empirical_covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)    39099 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/_graph_lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)    33901 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/_robust_covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)    27837 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/_shrunk_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.758464 scikit-learn-1.4.1.post1/sklearn/covariance/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_elliptic_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_graphical_lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_robust_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.758464 scikit-learn-1.4.1.post1/sklearn/cross_decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cross_decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36773 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cross_decomposition/_pls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.758464 scikit-learn-1.4.1.post1/sklearn/cross_decomposition/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cross_decomposition/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22294 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/cross_decomposition/tests/test_pls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.762464 scikit-learn-1.4.1.post1/sklearn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_arff_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    46825 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_covtype.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_kddcup99.py
--rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_lfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_olivetti_faces.py
--rw-r--r--   0 runner    (1001) docker     (127)    41405 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_openml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_rcv1.py
--rw-r--r--   0 runner    (1001) docker     (127)    74553 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_samples_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_species_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_svmlight_format_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_svmlight_format_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/_twenty_newsgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.762464 scikit-learn-1.4.1.post1/sklearn/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/boston_house_prices.csv
--rw-r--r--   0 runner    (1001) docker     (127)   119913 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/breast_cancer.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/diabetes_data_raw.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/diabetes_target.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    57523 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/digits.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/linnerud_exercise.csv
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/linnerud_physiological.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/data/wine_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.766464 scikit-learn-1.4.1.post1/sklearn/datasets/descr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/breast_cancer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/california_housing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/covtype.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/diabetes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/digits.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/iris.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/kddcup99.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/lfw.rst
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/linnerud.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/olivetti_faces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/rcv1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/species_distributions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/twenty_newsgroups.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/descr/wine_data.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.766464 scikit-learn-1.4.1.post1/sklearn/datasets/images/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/images/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   196653 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/images/china.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   142987 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/images/flower.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.770464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.770464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.770464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.770464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/api-v1-jd-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/api-v1-jdf-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/api-v1-jdq-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/data-v1-dl-1.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.770464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jd-1119.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdf-1119.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdl-dn-adult-census-l-2-dv-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdl-dn-adult-census-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdq-1119.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/data-v1-dl-54002.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.774464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/api-v1-jd-1590.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdf-1590.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdq-1590.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/data-v1-dl-1595261.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.774464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jd-2.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jdf-2.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jdl-dn-anneal-l-2-dv-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jdl-dn-anneal-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jdq-2.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/data-v1-dl-1666876.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.774464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-292.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-40981.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jdf-292.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jdf-40981.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jdl-dn-australian-l-2-dv-1-s-dact.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jdl-dn-australian-l-2-dv-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jdl-dn-australian-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/data-v1-dl-49822.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.774464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/api-v1-jd-3.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/api-v1-jdf-3.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/api-v1-jdq-3.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/data-v1-dl-3.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.778464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jd-40589.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdf-40589.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdl-dn-emotions-l-2-dv-3.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdl-dn-emotions-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdq-40589.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/data-v1-dl-4644182.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.778464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jd-40675.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdf-40675.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdl-dn-glass2-l-2-dv-1-s-dact.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdl-dn-glass2-l-2-dv-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdl-dn-glass2-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdq-40675.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/data-v1-dl-4965250.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.778464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/api-v1-jd-40945.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/api-v1-jdf-40945.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/api-v1-jdq-40945.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)    32243 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/data-v1-dl-16826755.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.778464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jd-40966.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdf-40966.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdl-dn-miceprotein-l-2-dv-4.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdl-dn-miceprotein-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdq-40966.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/data-v1-dl-17928620.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.782464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/api-v1-jd-42074.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/api-v1-jdf-42074.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/api-v1-jdq-42074.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/data-v1-dl-21552912.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.782464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/api-v1-jd-42585.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/api-v1-jdf-42585.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/api-v1-jdq-42585.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/data-v1-dl-21854866.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.782464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jd-561.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jdf-561.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jdl-dn-cpu-l-2-dv-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jdl-dn-cpu-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jdq-561.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/data-v1-dl-52739.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.782464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jd-61.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jdf-61.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jdl-dn-iris-l-2-dv-1.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jdl-dn-iris-l-2-s-act-.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jdq-61.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/data-v1-dl-61.arff.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.786464 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/api-v1-jd-62.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/api-v1-jdf-62.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/api-v1-jdq-62.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/data-v1-dl-52352.arff.gz
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/svmlight_classification.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/svmlight_invalid.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/svmlight_invalid_order.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/svmlight_multilabel.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_20news.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_arff_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_covtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_kddcup99.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_lfw.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_olivetti_faces.py
--rw-r--r--   0 runner    (1001) docker     (127)    55329 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_openml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_rcv1.py
--rw-r--r--   0 runner    (1001) docker     (127)    23704 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_samples_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20269 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_svmlight_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.786464 scikit-learn-1.4.1.post1/sklearn/decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_cdnmf_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    76447 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_dict_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_factor_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26439 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_fastica.py
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_kernel_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    33064 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_lda.py
--rw-r--r--   0 runner    (1001) docker     (127)    82483 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_nmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_online_lda_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    28402 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_sparse_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/_truncated_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.790464 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_dict_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_factor_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15503 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_fastica.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    20772 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_kernel_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    34178 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_nmf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_online_lda.py
--rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_sparse_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_truncated_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)    37501 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.790464 scikit-learn-1.4.1.post1/sklearn/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43259 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_bagging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)   114121 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)    86549 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_gb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_gradient_boosting.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.794463 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_binning.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_bitset.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_bitset.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_gradient_boosting.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_predictor.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/common.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/common.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    92936 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)    31643 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/grower.py
--rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/histogram.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/splitting.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.794463 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_bitset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_compare_lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)    60892 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)    23152 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_grower.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_monotonic_contraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38639 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_warm_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_iforest.py
--rw-r--r--   0 runner    (1001) docker     (127)    39027 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_stacking.py
--rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_voting.py
--rw-r--r--   0 runner    (1001) docker     (127)    45369 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/_weight_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.798463 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30204 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_bagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    62547 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)    58784 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_iforest.py
--rw-r--r--   0 runner    (1001) docker     (127)    29896 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_stacking.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_voting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25403 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_weight_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.798463 scikit-learn-1.4.1.post1/sklearn/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/enable_halving_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/enable_hist_gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/enable_iterative_imputer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.798463 scikit-learn-1.4.1.post1/sklearn/experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/tests/test_enable_hist_gradient_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/tests/test_enable_iterative_imputer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/experimental/tests/test_enable_successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.798463 scikit-learn-1.4.1.post1/sklearn/externals/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/README
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38341 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_arff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.798463 scikit-learn-1.4.1.post1/sklearn/externals/_packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.798463 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.802464 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/sparse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/sparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.802464 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/sparse/csgraph/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/sparse/csgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18150 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/_scipy/sparse/csgraph/_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/externals/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.802464 scikit-learn-1.4.1.post1/sklearn/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/_dict_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/_hashing_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/_stop_words.py
--rw-r--r--   0 runner    (1001) docker     (127)    23024 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.802464 scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_dict_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_feature_hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    53098 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    78015 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_extraction/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.806464 scikit-learn-1.4.1.post1/sklearn/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_from_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18323 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_mutual_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_rfe.py
--rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)    40350 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_univariate_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/_variance_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.806464 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_chi2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_feature_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_from_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_mutual_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    20881 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_rfe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_variance_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.806464 scikit-learn-1.4.1.post1/sklearn/gaussian_process/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36524 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/_gpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    28140 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/_gpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    85400 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.806464 scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/_mini_sequence_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/test_gpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    29775 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/test_gpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/test_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.810464 scikit-learn-1.4.1.post1/sklearn/impute/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40012 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35716 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)    14662 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/_knn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.810464 scikit-learn-1.4.1.post1/sklearn/impute/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    59674 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/tests/test_impute.py
--rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/impute/tests/test_knn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.810464 scikit-learn-1.4.1.post1/sklearn/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31782 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_partial_dependence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_pd_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_permutation_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.810464 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/decision_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)    59995 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/partial_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.810464 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21278 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/tests/test_boundary_decision_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/_plot/tests/test_plot_partial_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.810464 scikit-learn-1.4.1.post1/sklearn/inspection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33329 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/tests/test_partial_dependence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/tests/test_pd_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19940 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/inspection/tests/test_permutation_importance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/isotonic.py
--rw-r--r--   0 runner    (1001) docker     (127)    40838 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/kernel_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/kernel_ridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.814463 scikit-learn-1.4.1.post1/sklearn/linear_model/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29747 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_cd_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   109065 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_coordinate_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.818463 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19275 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/_newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    31930 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/glm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.818463 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40696 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/tests/test_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_huber.py
--rw-r--r--   0 runner    (1001) docker     (127)    81551 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_least_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    26796 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_linear_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    84028 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)    37378 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_omp.py
--rw-r--r--   0 runner    (1001) docker     (127)    19323 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_passive_aggressive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_ransac.py
--rw-r--r--   0 runner    (1001) docker     (127)    93020 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_sag.py
--rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_sag_fast.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_sgd_fast.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    23941 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_sgd_fast.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_sgd_fast_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    89642 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_stochastic_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    15814 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/_theil_sen.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.822463 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    56926 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_coordinate_descent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_huber.py
--rw-r--r--   0 runner    (1001) docker     (127)    29553 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_least_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_linear_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    75541 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_omp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_passive_aggressive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_ransac.py
--rw-r--r--   0 runner    (1001) docker     (127)    70145 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    31398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_sag.py
--rw-r--r--   0 runner    (1001) docker     (127)    70696 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_sparse_coordinate_descent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_theil_sen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.822463 scikit-learn-1.4.1.post1/sklearn/manifold/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_barnes_hut_tsne.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_isomap.py
--rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_locally_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    23693 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_mds.py
--rw-r--r--   0 runner    (1001) docker     (127)    29120 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    43994 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_t_sne.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.822463 scikit-learn-1.4.1.post1/sklearn/manifold/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_isomap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_locally_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_mds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    38871 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_t_sne.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.826464 scikit-learn-1.4.1.post1/sklearn/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)   121687 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_dist_metrics.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    91783 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_dist_metrics.pyx.tp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.830464 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_argkmin_classmode.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_base.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    18353 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_base.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_classmode.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)    29726 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors_classmode.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_fast.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.830464 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/det_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/roc_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.830464 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_common_curve_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_confusion_matrix_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_det_curve_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_precision_recall_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_predict_error_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_roc_curve_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    75994 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    33389 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.830464 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_bicluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_expected_mutual_info_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    44498 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)    17063 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.834463 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_bicluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17873 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)    85973 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.834463 scikit-learn-1.4.1.post1/sklearn/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   101469 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    60017 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_dist_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56671 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    53017 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_pairwise_distances_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    82385 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    27231 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    53184 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_score_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.834463 scikit-learn-1.4.1.post1/sklearn/mixture/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18718 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33467 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/_bayesian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/_gaussian_mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.834463 scikit-learn-1.4.1.post1/sklearn/mixture/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/tests/test_bayesian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    47721 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/tests/test_gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/mixture/tests/test_mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.838463 scikit-learn-1.4.1.post1/sklearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35291 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    75511 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    43900 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/_search_successive_halving.py
--rw-r--r--   0 runner    (1001) docker     (127)    99167 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    88502 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.838463 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    19330 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    84676 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    71585 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    28876 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_successive_halving.py
--rw-r--r--   0 runner    (1001) docker     (127)    88874 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    43819 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    40821 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)    55670 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/naive_bayes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.842463 scikit-learn-1.4.1.post1/sklearn/neighbors/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_ball_tree.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)    51658 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)   100766 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_binary_tree.pxi.tp
--rw-r--r--   0 runner    (1001) docker     (127)    31731 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    25037 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11092 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_kd_tree.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_lof.py
--rw-r--r--   0 runner    (1001) docker     (127)    19586 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_nca.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_nearest_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_partition_nodes.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_partition_nodes.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_quad_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    23721 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_quad_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    18123 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.842463 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_ball_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_kd_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_lof.py
--rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_nca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_nearest_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)    81900 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_neighbors_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_neighbors_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_quad_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.846463 scikit-learn-1.4.1.post1/sklearn/neural_network/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    60524 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/_multilayer_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/_rbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/_stochastic_optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.846463 scikit-learn-1.4.1.post1/sklearn/neural_network/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31862 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_rbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_stochastic_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    66341 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.846463 scikit-learn-1.4.1.post1/sklearn/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_csr_polynomial_expansion.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   125337 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    67754 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30810 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    47444 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/_target_encoder_fast.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.850463 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    94200 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    78684 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23634 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    42411 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)    27915 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    28095 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/random_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.850463 scikit-learn-1.4.1.post1/sklearn/semi_supervised/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/semi_supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21294 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/semi_supervised/_label_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/semi_supervised/_self_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.850463 scikit-learn-1.4.1.post1/sklearn/semi_supervised/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/semi_supervised/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/semi_supervised/tests/test_label_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/semi_supervised/tests/test_self_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.854463 scikit-learn-1.4.1.post1/sklearn/svm/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42474 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    66940 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_liblinear.pxi
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_liblinear.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_libsvm.pxi
--rw-r--r--   0 runner    (1001) docker     (127)    26994 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_libsvm.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_libsvm_sparse.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/_newrand.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.642464 scikit-learn-1.4.1.post1/sklearn/svm/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.854463 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/_cython_blas_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/liblinear_helper.c
--rw-r--r--   0 runner    (1001) docker     (127)    62634 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/linear.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/linear.h
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/tron.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/tron.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.854463 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/LIBSVM_CHANGES
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/_svm_cython_blas_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/libsvm_helper.c
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/libsvm_sparse_helper.c
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/libsvm_template.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    69105 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/svm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/svm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.854463 scikit-learn-1.4.1.post1/sklearn/svm/src/newrand/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/src/newrand/newrand.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.854463 scikit-learn-1.4.1.post1/sklearn/svm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    49059 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/svm/tests/test_svm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.862463 scikit-learn-1.4.1.post1/sklearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/metadata_routing_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/random_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    28614 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)    40422 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_check_build.py
--rw-r--r--   0 runner    (1001) docker     (127)    19553 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_docstring_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    21319 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_isotonic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_kernel_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_kernel_ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_metadata_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_metaestimators.py
--rw-r--r--   0 runner    (1001) docker     (127)    22521 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_metaestimators_metadata_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_min_dependencies_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)    33480 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    29175 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)    35027 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_naive_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)    63837 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_public_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19583 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tests/test_random_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.862463 scikit-learn-1.4.1.post1/sklearn/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75272 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_criterion.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    62083 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_criterion.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    39293 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_reingold_tilford.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_splitter.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    60816 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_splitter.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    72935 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_tree.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    16808 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.862463 scikit-learn-1.4.1.post1/sklearn/tree/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    18590 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/tests/test_monotonic_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/tests/test_reingold_tilford.py
--rw-r--r--   0 runner    (1001) docker     (127)    94675 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/tree/tests/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.874463 scikit-learn-1.4.1.post1/sklearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    40703 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_arpack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18876 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_array_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_available_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_cython_blas.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_cython_blas.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_estimator_html_repr.css
--rw-r--r--   0 runner    (1001) docker     (127)    18308 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_estimator_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_fast_dict.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_fast_dict.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_heap.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_heap.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_isfinite.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_joblib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    54375 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_metadata_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    13093 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_openmp_helpers.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_openmp_helpers.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_param_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_random.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_random.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_seq_dataset.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_seq_dataset.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_set_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_sorting.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_sorting.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    39674 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_typedefs.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_typedefs.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_vector_sentinel.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_vector_sentinel.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_weight_vector.pxd.tp
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/_weight_vector.pyx.tp
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/arrayfuncs.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/class_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)   167648 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    44378 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/extmath.py
--rw-r--r--   0 runner    (1001) docker     (127)    14005 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/metadata_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/metaestimators.py
--rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/murmurhash.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/murmurhash.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    22673 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/sparsefuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20393 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/sparsefuncs_fast.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.874463 scikit-learn-1.4.1.post1/sklearn/utils/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/src/MurmurHash3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/src/MurmurHash3.h
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:57.882463 scikit-learn-1.4.1.post1/sklearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_arpack.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_array_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_class_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_cython_blas.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_cython_templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)    43757 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18057 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_estimator_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    36993 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_extmath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_fast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_metaestimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_murmurhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24201 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_param_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    27339 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_seq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_set_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_shortest_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    34923 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_sparsefuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    27802 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29562 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    69344 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/tests/test_weight_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    88758 2024-02-15 14:01:39.000000 scikit-learn-1.4.1.post1/sklearn/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.318612 scikit-learn-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-09 14:20:32.318612 scikit-learn-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.094610 scikit-learn-1.4.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/authors_emeritus.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.094610 scikit-learn-1.4.2/doc/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25058 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/common_pitfalls.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/communication_team.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/communication_team_emeritus.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.094610 scikit-learn-1.4.2/doc/computing/
+-rw-r--r--   0 runner    (1001) docker     (127)    17218 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/computing/computational_performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/computing/parallelism.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/computing/scaling_strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/computing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27224 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/contributor_experience_team.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/contributor_experience_team_emeritus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/data_transforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.094610 scikit-learn-1.4.2/doc/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/datasets/loading_other_datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/datasets/real_world.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/datasets/sample_generators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/datasets/toy_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.098610 scikit-learn-1.4.2/doc/developers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19897 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/advanced_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/bug_triaging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61458 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/cython.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38663 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/maintainer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15265 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/minimal_reproducer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14388 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/tips.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/developers/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/dispatching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/documentation_team.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23949 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    90170 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/governance.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.110610 scikit-learn-1.4.2/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/axa-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17847 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/axa.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31049 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/bcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54774 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/beta_divergence.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/bnp-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21156 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/bnp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/cds-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/chanel-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/chanel.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/columbia-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/columbia.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/czi_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/dataiku-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/dataiku.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18585 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/digicosme.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/dysco.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/fnrs-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18012 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/fujitsu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89394 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/generated-doc-ci.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/google-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45148 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/grid_search_cross_validation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101880 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/grid_search_workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/huggingface_logo-noborder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/inria-logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/inria-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/intel-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/intel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27033 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/iris.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/iris.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/last_digit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13032 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/lda_model_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/logo_APHP.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/logo_APHP_text.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/microsoft-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/microsoft.png
+-rw-r--r--   0 runner    (1001) docker     (127)   761071 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/ml_map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26546 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/multi_org_chart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89381 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/multilayerperceptron_network.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/no_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/nvidia-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10764 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/nvidia.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/nyu_short_color.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45027 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/permuted_non_predictive_feature.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43181 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/permuted_predictive_feature.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31108 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/plot_digits_classification.png
+-rw-r--r--   0 runner    (1001) docker     (127)   124459 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/plot_face_recognition_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86623 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/plot_face_recognition_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/png-logo-inria-la-fondation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20223 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/probabl.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/quansight-labs-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)   124931 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/quansight-labs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/rbm_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/scikit-learn-logo-notext.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/scikit-learn-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29042 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/sloan_banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/sloan_logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38356 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/sydney-primary.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/sydney-stacked-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32077 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/target_encoder_cross_validation.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/telecom-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35103 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/telecom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84599 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/images/visual-studio-build-tools-selection.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.110610 scikit-learn-1.4.2/doc/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/includes/big_toc_css.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/includes/bigger_toc_css.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/jupyter_lite_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.114610 scikit-learn-1.4.2/doc/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    48838 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/1280px-scikit-learn-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.114610 scikit-learn-1.4.2/doc/logos/brand_colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/brand_colors/colorswatch_29ABE2_cyan.png
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/brand_colors/colorswatch_9B4600_brown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/brand_colors/colorswatch_F7931E_orange.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.114610 scikit-learn-1.4.2/doc/logos/brand_guidelines/
+-rw-r--r--   0 runner    (1001) docker     (127)   104582 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/brand_guidelines/scikitlearn_logo_clearspace_updated.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2238 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/favicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)   120865 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/identity.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo-notext.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo-thumb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo-without-subtitle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    37902 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/logos/scikit-learn-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/metadata_routing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/model_persistence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/model_selection.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.122610 scikit-learn-1.4.2/doc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/array_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/biclustering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/calibration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    42830 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    94103 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/clustering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24659 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/compose.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/covariance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/cross_decomposition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    40831 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46874 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/decomposition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/density.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    70083 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/ensemble.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    44474 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/feature_extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/feature_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24659 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/gaussian_process.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.122610 scikit-learn-1.4.2/doc/modules/glm_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/glm_data/lasso_enet_coordinate_descent.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63830 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/glm_data/poisson_gamma_tweedie_distributions.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33777 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/grid_search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/impute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/isotonic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/kernel_approximation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/kernel_ridge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/lda_qda.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/learning_curve.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    79723 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/linear_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30280 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/manifold.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/mixture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   121343 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/multiclass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/naive_bayes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38706 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/neighbors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/neural_networks_supervised.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/neural_networks_unsupervised.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/outlier_detection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/partial_dependence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/permutation_importance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    53915 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/preprocessing_targets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/random_projection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/semi_supervised.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24946 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/sgd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34865 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/svm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/tree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/modules/unsupervised_reduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/preface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/presentations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/related_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/roadmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.122610 scikit-learn-1.4.2/doc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/sphinxext/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/sphinxext/add_toctree_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1908 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/sphinxext/allow_nan_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/sphinxext/doi_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/sphinxext/github_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/sphinxext/sphinx_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/supervised_learning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.126610 scikit-learn-1.4.2/doc/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/class_with_call.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/deprecated_class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/deprecated_class_with_call.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/deprecated_class_without_init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/deprecated_function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/display_all_class_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/display_only_from_estimator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/function.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/generate_deprecated.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    17331 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/numpydoc_docstring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/templates/redirects.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.126610 scikit-learn-1.4.2/doc/testimonials/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.130610 scikit-learn-1.4.2/doc/testimonials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    41412 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/aweber.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/bestofmedia-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/betaworks.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/birchbox.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    65058 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/bnp_paribas_cardif.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/booking.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/change-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/dataiku_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/datapublica.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/datarobot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/evernote.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/howaboutwe.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31051 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/huggingface.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85087 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/infonea.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/inria.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/jpmorgan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/lovely.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/machinalis.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47018 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/mars.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/okcupid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/ottogroup_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/peerindex.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/phimeca.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/rangespan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/solido_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/telecomparistech.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/yhat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22810 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/images/zopa.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/testimonials/testimonials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.070609 scikit-learn-1.4.2/doc/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.130610 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.070609 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.130610 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.130610 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)   155712 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/css/vendor/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.130610 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/details-permalink.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.130610 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    58030 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/vendor/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    72818 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/vendor/jquery-3.6.3.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/themes/scikit-learn-modern/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tune_toc.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/basic/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/common_includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/common_includes/info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/machine_learning_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/machine_learning_map/ML_MAPS_README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/machine_learning_map/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/machine_learning_map/parse_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230678 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/machine_learning_map/pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/machine_learning_map/svg2imagemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/statistical_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/statistical_inference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/statistical_inference/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/statistical_inference/putting_together.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/statistical_inference/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/statistical_inference/supervised_learning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/statistical_inference/unsupervised_learning.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/text_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.070609 scikit-learn-1.4.2/doc/tutorial/text_analytics/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/text_analytics/data/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/data/languages/fetch_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/text_analytics/data/movie_reviews/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/data/movie_reviews/fetch_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/text_analytics/skeletons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/skeletons/exercise_01_language_train_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/skeletons/exercise_02_sentiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.134610 scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/exercise_01_language_train_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/exercise_02_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/generate_skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21039 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/tutorial/text_analytics/working_with_text_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/unsupervised_learning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/visualizations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.138610 scikit-learn-1.4.2/doc/whats_new/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/_contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/changelog_legend.inc
+-rw-r--r--   0 runner    (1001) docker     (127)    44662 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/older_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.13.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.14.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.15.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23270 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.16.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.17.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.18.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    48325 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.19.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    79828 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.20.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    50044 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.21.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    52900 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.22.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38648 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.23.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46490 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v0.24.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    57815 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    65715 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    48895 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    45212 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    48140 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new/v1.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/doc/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.138610 scikit-learn-1.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.142610 scikit-learn-1.4.2/examples/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31775 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_cyclical_feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_digits_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_face_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_model_complexity_influence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_out_of_core_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_outlier_detection_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_prediction_latency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_species_distribution_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_stock_market.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16513 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_time_series_lagged_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_tomography_l1_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/plot_topics_extraction_with_nmf_lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11537 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/svm_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/applications/wikipedia_principal_eigenvector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.142610 scikit-learn-1.4.2/examples/bicluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/bicluster/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/bicluster/plot_bicluster_newsgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/bicluster/plot_spectral_biclustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/bicluster/plot_spectral_coclustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.142610 scikit-learn-1.4.2/examples/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/calibration/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/calibration/plot_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/calibration/plot_calibration_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/calibration/plot_calibration_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/calibration/plot_compare_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.146610 scikit-learn-1.4.2/examples/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/classification/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/classification/plot_classification_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/classification/plot_classifier_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/classification/plot_digits_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/classification/plot_lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/classification/plot_lda_qda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.150610 scikit-learn-1.4.2/examples/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_adjusted_for_chance_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_affinity_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_agglomerative_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_agglomerative_clustering_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_agglomerative_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_birch_vs_minibatchkmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_bisect_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_cluster_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_cluster_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_coin_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_coin_ward_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_color_quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_dict_face_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_digits_agglomeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_digits_linkage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_face_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_feature_agglomeration_vs_univariate_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_inductive_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_kmeans_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_kmeans_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_kmeans_plusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_kmeans_silhouette_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_kmeans_stability_low_dim_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_linkage_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_mean_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_mini_batch_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_segmentation_toy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cluster/plot_ward_structured_vs_unstructured.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.150610 scikit-learn-1.4.2/examples/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/plot_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/plot_column_transformer_mixed_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/plot_compare_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/plot_digits_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/plot_feature_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/compose/plot_transformed_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.150610 scikit-learn-1.4.2/examples/covariance/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/covariance/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/covariance/plot_covariance_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/covariance/plot_lw_vs_oas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/covariance/plot_mahalanobis_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/covariance/plot_robust_vs_empirical_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/covariance/plot_sparse_cov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.150610 scikit-learn-1.4.2/examples/cross_decomposition/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cross_decomposition/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cross_decomposition/plot_compare_cross_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/cross_decomposition/plot_pcr_vs_pls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.150610 scikit-learn-1.4.2/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/datasets/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/datasets/plot_digits_last_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/datasets/plot_iris_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/datasets/plot_random_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/datasets/plot_random_multilabel_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.154610 scikit-learn-1.4.2/examples/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_faces_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_ica_blind_source_separation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_ica_vs_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_image_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_kernel_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_pca_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_pca_vs_fa_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_pca_vs_lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_sparse_coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/decomposition/plot_varimax_fa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.154610 scikit-learn-1.4.2/examples/developing_estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/developing_estimators/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/developing_estimators/sklearn_is_fitted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.158610 scikit-learn-1.4.2/examples/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_adaboost_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_adaboost_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_adaboost_twoclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_bias_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_ensemble_oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_feature_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_forest_hist_grad_boosting_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_forest_importances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_forest_importances_faces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_forest_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_isolation_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_monotonic_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_random_forest_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_random_forest_regression_multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_stack_predictors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_voting_decision_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_voting_probas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/ensemble/plot_voting_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.158610 scikit-learn-1.4.2/examples/exercises/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/exercises/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/exercises/plot_cv_diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/exercises/plot_digits_classification_exercise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/exercises/plot_iris_exercise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.158610 scikit-learn-1.4.2/examples/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/plot_f_test_vs_mi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/plot_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/plot_feature_selection_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/plot_rfe_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/plot_rfe_with_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/feature_selection/plot_select_from_model_diabetes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.162611 scikit-learn-1.4.2/examples/gaussian_process/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_compare_gpr_krr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpc_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpc_isoprobability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpc_xor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_co2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_noisy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_noisy_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_on_structured_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_prior_posterior.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.162611 scikit-learn-1.4.2/examples/impute/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/impute/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/impute/plot_iterative_imputer_variants_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/impute/plot_missing_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.162611 scikit-learn-1.4.2/examples/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/inspection/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/inspection/plot_causal_interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/inspection/plot_linear_model_coefficient_interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21224 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/inspection/plot_partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/inspection/plot_permutation_importance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/inspection/plot_permutation_importance_multicollinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.162611 scikit-learn-1.4.2/examples/kernel_approximation/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/kernel_approximation/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/kernel_approximation/plot_scalable_poly_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.170611 scikit-learn-1.4.2/examples/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_bayesian_ridge_curvefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_elastic_net_precomputed_gram_matrix_with_weighted_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_huber_vs_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_iris_logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_lasso_and_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_lasso_coordinate_descent_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_lasso_dense_vs_sparse_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_lasso_lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_lasso_lars_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_lasso_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_logistic_l1_l2_sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_logistic_multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_logistic_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_multi_task_lasso_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_nnls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ols_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ols_ridge_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_omp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22613 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_poisson_regression_non_normal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_polynomial_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_quantile_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ridge_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_ridge_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_robust_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_penalties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_separating_hyperplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgd_weighted_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sgdocsvm_vs_ocsvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sparse_logistic_regression_20newsgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_sparse_logistic_regression_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_theilsen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23618 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/linear_model/plot_tweedie_regression_insurance_claims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.170611 scikit-learn-1.4.2/examples/manifold/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/plot_compare_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/plot_lle_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/plot_manifold_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/plot_mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/plot_swissroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/manifold/plot_t_sne_perplexity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.174611 scikit-learn-1.4.2/examples/miscellaneous/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_anomaly_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_display_object_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_estimator_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_isotonic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_johnson_lindenstrauss_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_kernel_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_kernel_ridge_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24865 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_metadata_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_multioutput_face_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16466 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_outlier_detection_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_partial_dependence_visualization_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_pipeline_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_roc_curve_visualization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/miscellaneous/plot_set_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.174611 scikit-learn-1.4.2/examples/mixture/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_concentration_prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_gmm_covariances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_gmm_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_gmm_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_gmm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/mixture/plot_gmm_sin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.178611 scikit-learn-1.4.2/examples/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_cv_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_grid_search_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_grid_search_refit_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23047 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_grid_search_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_grid_search_text_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_learning_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_likelihood_ratios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_multi_metric_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_nested_cross_validation_iris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_permutation_tests_for_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_randomized_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14496 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_roc_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_successive_halving_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_successive_halving_iterations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_train_error_vs_test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_underfitting_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/model_selection/plot_validation_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.178611 scikit-learn-1.4.2/examples/multiclass/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/multiclass/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/multiclass/plot_multiclass_overview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.178611 scikit-learn-1.4.2/examples/multioutput/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/multioutput/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/multioutput/plot_classifier_chain_yeast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.178611 scikit-learn-1.4.2/examples/neighbors/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/approximate_nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_caching_nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_digits_kde_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_kde_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_lof_novelty_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_lof_outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_nca_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_nca_dim_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_nca_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_nearest_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neighbors/plot_species_kde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.182611 scikit-learn-1.4.2/examples/neural_networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neural_networks/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neural_networks/plot_mlp_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neural_networks/plot_mlp_training_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neural_networks/plot_mnist_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/neural_networks/plot_rbm_logistic_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.182611 scikit-learn-1.4.2/examples/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14781 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_all_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_discretization_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_discretization_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_map_data_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_scaling_importance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/preprocessing/plot_target_encoder_cross_val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.182611 scikit-learn-1.4.2/examples/release_highlights/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_0_22_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_0_23_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_0_24_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_4_0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.182611 scikit-learn-1.4.2/examples/semi_supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/plot_label_propagation_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/plot_label_propagation_digits_active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/plot_label_propagation_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/plot_self_training_varying_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/plot_semi_supervised_newsgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/semi_supervised/plot_semi_supervised_versus_svm_iris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.186611 scikit-learn-1.4.2/examples/svm/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_custom_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_iris_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_linearsvc_support_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_oneclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_rbf_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_separating_hyperplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_separating_hyperplane_unbalanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_anova.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_scale_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_svm_tie_breaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/svm/plot_weighted_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.186611 scikit-learn-1.4.2/examples/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/text/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/text/plot_document_classification_20newsgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/text/plot_document_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/text/plot_hashing_vs_dict_vectorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.186611 scikit-learn-1.4.2/examples/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/tree/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/tree/plot_cost_complexity_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/tree/plot_iris_dtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/tree/plot_tree_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/tree/plot_tree_regression_multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/examples/tree/plot_unveil_tree_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.190611 scikit-learn-1.4.2/scikit_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-09 14:20:31.000000 scikit-learn-1.4.2/scikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    58757 2024-04-09 14:20:32.000000 scikit-learn-1.4.2/scikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:20:31.000000 scikit-learn-1.4.2/scikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:20:31.000000 scikit-learn-1.4.2/scikit_learn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 14:20:31.000000 scikit-learn-1.4.2/scikit_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 14:20:31.000000 scikit-learn-1.4.2/scikit_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 14:20:32.318612 scikit-learn-1.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23006 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.194611 scikit-learn-1.4.2/sklearn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.194611 scikit-learn-1.4.2/sklearn/__check_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/__check_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/__check_build/_check_build.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/__check_build/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.194611 scikit-learn-1.4.2/sklearn/_build_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_build_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_build_utils/openmp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_build_utils/pre_build_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_build_utils/tempita.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_build_utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_distributor_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_isotonic.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.194611 scikit-learn-1.4.2/sklearn/_loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/_loss.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    50281 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/_loss.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41236 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.194611 scikit-learn-1.4.2/sklearn/_loss/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48281 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_loss/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/_min_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53077 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49547 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.198611 scikit-learn-1.4.2/sklearn/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_affinity_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49039 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_agglomerative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22157 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_bicluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26249 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_birch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_bisect_k_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_dbscan_inner.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_feature_agglomeration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.198611 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_linkage.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_reachability.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    27800 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    41849 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.202611 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hdbscan/tests/test_reachibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hierarchical_fast.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    15905 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_hierarchical_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_k_means_common.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_k_means_common.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_k_means_elkan.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_k_means_lloyd.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_k_means_minibatch.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    82683 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20156 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_mean_shift.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44710 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30496 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.202611 scikit-learn-1.4.2/sklearn/cluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_affinity_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_bicluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_birch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_bisect_k_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_feature_agglomeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32593 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48900 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_k_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_mean_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cluster/tests/test_spectral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.202611 scikit-learn-1.4.2/sklearn/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57863 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/compose/_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/compose/_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.202611 scikit-learn-1.4.2/sklearn/compose/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/compose/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88405 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/compose/tests/test_column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13153 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/compose/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.206611 scikit-learn-1.4.2/sklearn/covariance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/_elliptic_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/_empirical_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39099 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/_graph_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33901 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/_robust_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27837 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/_shrunk_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.206611 scikit-learn-1.4.2/sklearn/covariance/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/tests/test_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/tests/test_elliptic_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/tests/test_graphical_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/covariance/tests/test_robust_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.206611 scikit-learn-1.4.2/sklearn/cross_decomposition/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cross_decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36773 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cross_decomposition/_pls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.206611 scikit-learn-1.4.2/sklearn/cross_decomposition/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cross_decomposition/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22294 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/cross_decomposition/tests/test_pls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.210611 scikit-learn-1.4.2/sklearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_arff_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46825 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_covtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_kddcup99.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_lfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_olivetti_faces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41405 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_openml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_rcv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74553 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_samples_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_species_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_svmlight_format_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_svmlight_format_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/_twenty_newsgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.210611 scikit-learn-1.4.2/sklearn/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34742 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/boston_house_prices.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   119913 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/breast_cancer.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/diabetes_data_raw.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/diabetes_target.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    57523 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/digits.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/linnerud_exercise.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/linnerud_physiological.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/data/wine_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.214611 scikit-learn-1.4.2/sklearn/datasets/descr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/breast_cancer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/california_housing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/covtype.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/diabetes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/digits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/iris.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/kddcup99.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/lfw.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/linnerud.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/olivetti_faces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/rcv1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/species_distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/twenty_newsgroups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/descr/wine_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.214611 scikit-learn-1.4.2/sklearn/datasets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/images/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196653 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/images/china.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   142987 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/images/flower.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.214611 scikit-learn-1.4.2/sklearn/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.218611 scikit-learn-1.4.2/sklearn/datasets/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.218611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.218611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/api-v1-jd-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/api-v1-jdf-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/api-v1-jdq-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/data-v1-dl-1.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.218611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jd-1119.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdf-1119.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdl-dn-adult-census-l-2-dv-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdl-dn-adult-census-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdq-1119.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/data-v1-dl-54002.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.218611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/api-v1-jd-1590.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdf-1590.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdq-1590.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/data-v1-dl-1595261.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.218611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jd-2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jdf-2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jdl-dn-anneal-l-2-dv-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jdl-dn-anneal-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jdq-2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/data-v1-dl-1666876.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.222611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-292.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-40981.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jdf-292.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jdf-40981.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jdl-dn-australian-l-2-dv-1-s-dact.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jdl-dn-australian-l-2-dv-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jdl-dn-australian-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/data-v1-dl-49822.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.222611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/api-v1-jd-3.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/api-v1-jdf-3.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/api-v1-jdq-3.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/data-v1-dl-3.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.222611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jd-40589.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdf-40589.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdl-dn-emotions-l-2-dv-3.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdl-dn-emotions-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdq-40589.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/data-v1-dl-4644182.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.222611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jd-40675.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdf-40675.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdl-dn-glass2-l-2-dv-1-s-dact.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdl-dn-glass2-l-2-dv-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdl-dn-glass2-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdq-40675.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/data-v1-dl-4965250.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.226611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/api-v1-jd-40945.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/api-v1-jdf-40945.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/api-v1-jdq-40945.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    32243 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/data-v1-dl-16826755.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.226611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jd-40966.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdf-40966.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdl-dn-miceprotein-l-2-dv-4.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdl-dn-miceprotein-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdq-40966.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/data-v1-dl-17928620.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.226611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/api-v1-jd-42074.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/api-v1-jdf-42074.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/api-v1-jdq-42074.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/data-v1-dl-21552912.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.226611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/api-v1-jd-42585.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/api-v1-jdf-42585.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/api-v1-jdq-42585.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/data-v1-dl-21854866.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.226611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jd-561.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jdf-561.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jdl-dn-cpu-l-2-dv-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jdl-dn-cpu-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jdq-561.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/data-v1-dl-52739.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.230611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jd-61.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jdf-61.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jdl-dn-iris-l-2-dv-1.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jdl-dn-iris-l-2-s-act-.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jdq-61.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/data-v1-dl-61.arff.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.230611 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/api-v1-jd-62.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/api-v1-jdf-62.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/api-v1-jdq-62.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/data-v1-dl-52352.arff.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/svmlight_classification.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/svmlight_invalid.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/svmlight_invalid_order.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/data/svmlight_multilabel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_20news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_arff_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_covtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_kddcup99.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_lfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_olivetti_faces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55329 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_openml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_rcv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23704 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_samples_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20269 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/datasets/tests/test_svmlight_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.230611 scikit-learn-1.4.2/sklearn/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_cdnmf_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    76447 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_dict_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_factor_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26439 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_fastica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_kernel_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33064 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82483 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_online_lda_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    28402 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_sparse_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/_truncated_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.234611 scikit-learn-1.4.2/sklearn/decomposition/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_dict_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_factor_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15503 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_fastica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20772 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_kernel_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34178 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15825 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_online_lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35081 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_sparse_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/decomposition/tests/test_truncated_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37501 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.234611 scikit-learn-1.4.2/sklearn/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43259 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_bagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114121 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86549 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_gb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_gradient_boosting.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.238611 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_binning.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_bitset.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_bitset.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_gradient_boosting.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_predictor.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/common.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/common.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    92936 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31643 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/grower.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/histogram.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52483 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/splitting.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.238611 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_bitset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_compare_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60892 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23152 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_grower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_monotonic_contraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38639 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_warm_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    20427 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_iforest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39027 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_stacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23331 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_voting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45369 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/_weight_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/ensemble/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30204 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_bagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62547 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58784 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_iforest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29896 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_stacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_voting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25403 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/ensemble/tests/test_weight_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/enable_halving_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/enable_hist_gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/enable_iterative_imputer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/tests/test_enable_hist_gradient_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/tests/test_enable_iterative_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/experimental/tests/test_enable_successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/externals/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/README
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38341 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_arff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/externals/_packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/externals/_scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_scipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/externals/_scipy/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_scipy/sparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.242612 scikit-learn-1.4.2/sklearn/externals/_scipy/sparse/csgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_scipy/sparse/csgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18150 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/_scipy/sparse/csgraph/_laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/externals/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.246611 scikit-learn-1.4.2/sklearn/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/_dict_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/_hashing_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/_stop_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23024 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.246611 scikit-learn-1.4.2/sklearn/feature_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_dict_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_feature_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53098 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78015 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_extraction/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.246611 scikit-learn-1.4.2/sklearn/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18323 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_mutual_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_rfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40350 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_univariate_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/_variance_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.246611 scikit-learn-1.4.2/sklearn/feature_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_chi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_feature_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_mutual_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20881 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_rfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/feature_selection/tests/test_variance_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/gaussian_process/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36524 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/_gpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28140 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/_gpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85400 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/gaussian_process/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/tests/_mini_sequence_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/tests/test_gpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29775 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/tests/test_gpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/gaussian_process/tests/test_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/impute/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40012 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35716 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14662 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/_knn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/impute/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59674 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/tests/test_impute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/impute/tests/test_knn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31782 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_pd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_permutation_importance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/inspection/_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_plot/decision_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59995 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_plot/partial_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.250611 scikit-learn-1.4.2/sklearn/inspection/_plot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_plot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21278 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_plot/tests/test_boundary_decision_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/_plot/tests/test_plot_partial_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.254612 scikit-learn-1.4.2/sklearn/inspection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33329 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/tests/test_partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/tests/test_pd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19940 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/inspection/tests/test_permutation_importance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/isotonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40838 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/kernel_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/kernel_ridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.258612 scikit-learn-1.4.2/sklearn/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29747 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_cd_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   109065 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_coordinate_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.258612 scikit-learn-1.4.2/sklearn/linear_model/_glm/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_glm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19275 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_glm/_newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31930 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_glm/glm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.258612 scikit-learn-1.4.2/sklearn/linear_model/_glm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_glm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40696 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_glm/tests/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_huber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81551 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_least_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26796 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_linear_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84028 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37378 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_omp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19323 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_passive_aggressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93020 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_sag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_sag_fast.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_sgd_fast.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    23941 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_sgd_fast.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_sgd_fast_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    89642 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_stochastic_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15814 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/_theil_sen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.262612 scikit-learn-1.4.2/sklearn/linear_model/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56926 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_coordinate_descent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_huber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29553 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_least_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_linear_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75541 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_omp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_passive_aggressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70145 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_sag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70696 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_sparse_coordinate_descent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/linear_model/tests/test_theil_sen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.262612 scikit-learn-1.4.2/sklearn/manifold/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_barnes_hut_tsne.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_isomap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_locally_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23693 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29120 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_spectral_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43994 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_t_sne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.262612 scikit-learn-1.4.2/sklearn/manifold/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/tests/test_isomap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/tests/test_locally_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/tests/test_mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/tests/test_spectral_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38871 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/manifold/tests/test_t_sne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.266612 scikit-learn-1.4.2/sklearn/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121687 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_dist_metrics.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    91783 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_dist_metrics.pyx.tp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.266612 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_argkmin_classmode.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_base.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    18353 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_base.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_classmode.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    29726 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors_classmode.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_pairwise_fast.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.266612 scikit-learn-1.4.2/sklearn/metrics/_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/det_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/roc_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.270612 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_common_curve_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_confusion_matrix_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_det_curve_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_precision_recall_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_predict_error_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_roc_curve_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75994 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61720 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33389 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.270612 scikit-learn-1.4.2/sklearn/metrics/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/_bicluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/_expected_mutual_info_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    44498 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/_supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17063 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.270612 scikit-learn-1.4.2/sklearn/metrics/cluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_bicluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17873 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)    85973 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.274612 scikit-learn-1.4.2/sklearn/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101469 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60017 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_dist_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56671 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53017 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_pairwise_distances_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82385 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27231 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53184 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/metrics/tests/test_score_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.274612 scikit-learn-1.4.2/sklearn/mixture/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18718 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33467 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/_bayesian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/_gaussian_mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.274612 scikit-learn-1.4.2/sklearn/mixture/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/tests/test_bayesian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47721 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/tests/test_gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/mixture/tests/test_mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.274612 scikit-learn-1.4.2/sklearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35291 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75511 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43900 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/_search_successive_halving.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99167 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88502 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.278612 scikit-learn-1.4.2/sklearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19330 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84676 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71585 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28876 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/test_successive_halving.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88874 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/model_selection/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43819 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40821 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55670 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/naive_bayes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.278612 scikit-learn-1.4.2/sklearn/neighbors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_ball_tree.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    51658 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100766 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_binary_tree.pxi.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    31731 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25037 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11092 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_kd_tree.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_lof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19586 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_nca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_nearest_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_partition_nodes.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_partition_nodes.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_quad_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    23721 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_quad_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    18123 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.282612 scikit-learn-1.4.2/sklearn/neighbors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_ball_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_kd_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_lof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_nca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_nearest_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81900 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_neighbors_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_neighbors_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neighbors/tests/test_quad_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.282612 scikit-learn-1.4.2/sklearn/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60524 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/_multilayer_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/_rbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/_stochastic_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.282612 scikit-learn-1.4.2/sklearn/neural_network/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31862 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/tests/test_rbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/neural_network/tests/test_stochastic_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66341 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.286612 scikit-learn-1.4.2/sklearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_csr_polynomial_expansion.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   125337 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67754 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30800 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47444 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/_target_encoder_fast.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.286612 scikit-learn-1.4.2/sklearn/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94473 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78684 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23634 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42411 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27915 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/preprocessing/tests/test_target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28095 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/random_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.286612 scikit-learn-1.4.2/sklearn/semi_supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/semi_supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21294 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/semi_supervised/_label_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/semi_supervised/_self_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.286612 scikit-learn-1.4.2/sklearn/semi_supervised/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/semi_supervised/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/semi_supervised/tests/test_label_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/semi_supervised/tests/test_self_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.290612 scikit-learn-1.4.2/sklearn/svm/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42474 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66940 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_liblinear.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_liblinear.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_libsvm.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)    26994 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_libsvm.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_libsvm_sparse.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/_newrand.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.086610 scikit-learn-1.4.2/sklearn/svm/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.290612 scikit-learn-1.4.2/sklearn/svm/src/liblinear/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/_cython_blas_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/liblinear_helper.c
+-rw-r--r--   0 runner    (1001) docker     (127)    62634 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/linear.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/linear.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/tron.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/liblinear/tron.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.294612 scikit-learn-1.4.2/sklearn/svm/src/libsvm/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/LIBSVM_CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/_svm_cython_blas_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/libsvm_helper.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/libsvm_sparse_helper.c
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/libsvm_template.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    69105 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/svm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/libsvm/svm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.294612 scikit-learn-1.4.2/sklearn/svm/src/newrand/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/src/newrand/newrand.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.294612 scikit-learn-1.4.2/sklearn/svm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49059 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/svm/tests/test_svm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.298612 scikit-learn-1.4.2/sklearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/metadata_routing_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/random_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28614 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40422 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_check_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19553 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_docstring_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21319 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_isotonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_kernel_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_kernel_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_metadata_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_metaestimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22521 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_metaestimators_metadata_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_min_dependencies_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33480 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29175 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35027 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_naive_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63837 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_public_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19583 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tests/test_random_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.302612 scikit-learn-1.4.2/sklearn/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75272 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_criterion.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    62083 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_criterion.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    39293 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_reingold_tilford.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_splitter.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    60816 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_splitter.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    72935 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_tree.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    16808 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.302612 scikit-learn-1.4.2/sklearn/tree/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18590 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/tests/test_monotonic_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/tests/test_reingold_tilford.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94675 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/tree/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.314612 scikit-learn-1.4.2/sklearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    40703 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_arpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18876 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_array_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_available_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_cython_blas.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_cython_blas.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_estimator_html_repr.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18308 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_estimator_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_fast_dict.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_fast_dict.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_heap.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_heap.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_isfinite.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_joblib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54375 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_metadata_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13093 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_openmp_helpers.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_openmp_helpers.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_param_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_random.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_random.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_seq_dataset.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_seq_dataset.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_set_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_sorting.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_sorting.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39674 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_typedefs.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_typedefs.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_vector_sentinel.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_vector_sentinel.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_weight_vector.pxd.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/_weight_vector.pyx.tp
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/arrayfuncs.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/class_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167648 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44378 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/extmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/metadata_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/metaestimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/murmurhash.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/murmurhash.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22673 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/sparsefuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20393 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/sparsefuncs_fast.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.314612 scikit-learn-1.4.2/sklearn/utils/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/src/MurmurHash3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/src/MurmurHash3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:32.318612 scikit-learn-1.4.2/sklearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_arpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_array_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_class_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_cython_blas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_cython_templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43757 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18057 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_estimator_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36993 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_extmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_fast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_metaestimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_murmurhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24201 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_param_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27339 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_seq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_set_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_shortest_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34923 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_sparsefuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27802 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29562 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69302 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/tests/test_weight_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88758 2024-04-09 14:20:12.000000 scikit-learn-1.4.2/sklearn/utils/validation.py
```

### Comparing `scikit-learn-1.4.1.post1/COPYING` & `scikit-learn-1.4.2/COPYING`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/MANIFEST.in` & `scikit-learn-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/Makefile` & `scikit-learn-1.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/PKG-INFO` & `scikit-learn-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-learn
-Version: 1.4.1.post1
+Version: 1.4.2
 Summary: A set of python modules for machine learning and data mining
 Home-page: https://scikit-learn.org
 Maintainer: Andreas Mueller
 Maintainer-email: amueller@ais.uni-bonn.de
 License: new BSD
 Download-URL: https://pypi.org/project/scikit-learn/#files
 Project-URL: Bug Tracker, https://github.com/scikit-learn/scikit-learn/issues
```

### Comparing `scikit-learn-1.4.1.post1/README.rst` & `scikit-learn-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/Makefile` & `scikit-learn-1.4.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/about.rst` & `scikit-learn-1.4.2/doc/about.rst`

 * *Files 3% similar despite different names*

```diff
@@ -150,63 +150,91 @@
 Scikit-Learn is a community driven project, however institutional and private
 grants help to assure its sustainability.
 
 The project would like to thank the following funders.
 
 ...................................
 
+
+.. raw:: html
+
+   <div class="sk-sponsor-div">
+   <div class="sk-sponsor-div-box">
+
+`:probabl. <https://probabl.ai>`_ funds Adrin Jalali, Arturo Amor,
+François Goupil, Guillaume Lemaitre, Jérémie du Boisberranger, Olivier Grisel, and
+Stefanie Senger.
+
+.. raw:: html
+
+   </div>
+
+   <div class="sk-sponsor-div-box">
+
+.. image:: images/probabl.png
+   :width: 75pt
+   :align: center
+   :target: https://probabl.ai
+
+.. raw:: html
+
+   </div>
+   </div>
+
+..........
+
 .. raw:: html
 
    <div class="sk-sponsor-div">
    <div class="sk-sponsor-div-box">
 
 The `Members <https://scikit-learn.fondation-inria.fr/en/home/#sponsors>`_ of
 the `Scikit-Learn Consortium at Inria Foundation
-<https://scikit-learn.fondation-inria.fr/en/home/>`_  fund Arturo Amor,
-François Goupil, Guillaume Lemaitre, Jérémie du Boisberranger, and Olivier Grisel.
+<https://scikit-learn.fondation-inria.fr/en/home/>`_ help at maintaining and
+improving the project through their financial support.
 
 .. raw:: html
 
    </div>
 
 .. |chanel| image:: images/chanel.png
-   :width: 70pt
+   :width: 55pt
    :target: https://www.chanel.com
 
 .. |axa| image:: images/axa.png
-   :width: 50pt
+   :width: 40pt
    :target: https://www.axa.fr/
 
 .. |bnp| image:: images/bnp.png
-   :width: 150pt
+   :width: 120pt
    :target: https://www.bnpparibascardif.com/
 
 .. |dataiku| image:: images/dataiku.png
-   :width: 70pt
+   :width: 55pt
    :target: https://www.dataiku.com/
 
 .. |hf| image:: images/huggingface_logo-noborder.png
-   :width: 70pt
+   :width: 55pt
    :target: https://huggingface.co
 
 .. |nvidia| image:: images/nvidia.png
-   :width: 70pt
+   :width: 55pt
    :target: https://www.nvidia.com
 
 .. |inria| image:: images/inria-logo.jpg
-   :width: 100pt
+   :width: 75pt
    :target: https://www.inria.fr
 
 
 .. raw:: html
 
    <div class="sk-sponsor-div-box">
 
 .. table::
-   :class: sk-sponsor-table align-default
+   :class: sk-sponsor-table
 
    +----------+-----------+
    |       |chanel|       |
    +----------+-----------+
    |                      |
    +----------+-----------+
    |  |axa|   |    |bnp|  |
@@ -251,75 +279,74 @@
    :target: https://nvidia.com
 
 .. raw:: html
 
    </div>
    </div>
 
-
 ..........
 
 .. raw:: html
 
    <div class="sk-sponsor-div">
    <div class="sk-sponsor-div-box">
 
-`Hugging Face <https://huggingface.co/>`_ funded Adrin Jalali in 2022,
-2023 and is part of the scikit-learn consortium at Inria.
+`Microsoft <https://microsoft.com/>`_ funds Andreas Müller since 2020.
 
 .. raw:: html
 
    </div>
 
    <div class="sk-sponsor-div-box">
 
-.. image:: images/huggingface_logo-noborder.png
-   :width: 55pt
+.. image:: images/microsoft.png
+   :width: 100pt
    :align: center
-   :target: https://huggingface.co/
+   :target: https://www.microsoft.com/
 
 .. raw:: html
 
    </div>
    </div>
 
 ...........
 
 .. raw:: html
 
    <div class="sk-sponsor-div">
    <div class="sk-sponsor-div-box">
 
-`Microsoft <https://microsoft.com/>`_ funds Andreas Müller since 2020.
+`Quansight Labs <https://labs.quansight.org>`_ funds Lucy Liu since 2022.
 
 .. raw:: html
 
    </div>
 
    <div class="sk-sponsor-div-box">
 
-.. image:: images/microsoft.png
+.. image:: images/quansight-labs.png
    :width: 100pt
    :align: center
-   :target: https://www.microsoft.com/
+   :target: https://labs.quansight.org
 
 .. raw:: html
 
    </div>
    </div>
 
-...........
+Past Sponsors
+.............
 
 .. raw:: html
 
    <div class="sk-sponsor-div">
    <div class="sk-sponsor-div-box">
 
-`Quansight Labs <https://labs.quansight.org>`_ funds Lucy Liu and
-Meekail Zain since 2022 and funded Thomas J. Fan from 2021 to 2023.
+`Quansight Labs <https://labs.quansight.org>`_ funded Meekail Zain in 2022 and 2023 and,
+funded Thomas J. Fan from 2021 to 2023.
 
 .. raw:: html
 
    </div>
 
    <div class="sk-sponsor-div-box">
 
@@ -329,16 +356,15 @@
    :target: https://labs.quansight.org
 
 .. raw:: html
 
    </div>
    </div>
 
-Past Sponsors
-.............
+...........
 
 .. raw:: html
 
    <div class="sk-sponsor-div">
    <div class="sk-sponsor-div-box">
 
 `Columbia University <https://columbia.edu/>`_ funded Andreas Müller
```

### Comparing `scikit-learn-1.4.1.post1/doc/authors.rst` & `scikit-learn-1.4.2/doc/authors.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/authors_emeritus.rst` & `scikit-learn-1.4.2/doc/authors_emeritus.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/common_pitfalls.rst` & `scikit-learn-1.4.2/doc/common_pitfalls.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/communication_team.rst` & `scikit-learn-1.4.2/doc/communication_team.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/computing/computational_performance.rst` & `scikit-learn-1.4.2/doc/computing/computational_performance.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/computing/parallelism.rst` & `scikit-learn-1.4.2/doc/computing/parallelism.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/computing/scaling_strategies.rst` & `scikit-learn-1.4.2/doc/computing/scaling_strategies.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/conf.py` & `scikit-learn-1.4.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/conftest.py` & `scikit-learn-1.4.2/doc/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/contributor_experience_team.rst` & `scikit-learn-1.4.2/doc/contributor_experience_team.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/data_transforms.rst` & `scikit-learn-1.4.2/doc/data_transforms.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/datasets/loading_other_datasets.rst` & `scikit-learn-1.4.2/doc/datasets/loading_other_datasets.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/datasets/real_world.rst` & `scikit-learn-1.4.2/doc/datasets/real_world.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/datasets/sample_generators.rst` & `scikit-learn-1.4.2/doc/datasets/sample_generators.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/datasets/toy_dataset.rst` & `scikit-learn-1.4.2/doc/datasets/toy_dataset.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/datasets.rst` & `scikit-learn-1.4.2/doc/datasets.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/advanced_installation.rst` & `scikit-learn-1.4.2/doc/developers/advanced_installation.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/bug_triaging.rst` & `scikit-learn-1.4.2/doc/developers/bug_triaging.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/contributing.rst` & `scikit-learn-1.4.2/doc/developers/contributing.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/cython.rst` & `scikit-learn-1.4.2/doc/developers/cython.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/develop.rst` & `scikit-learn-1.4.2/doc/developers/develop.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/maintainer.rst` & `scikit-learn-1.4.2/doc/developers/maintainer.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/minimal_reproducer.rst` & `scikit-learn-1.4.2/doc/developers/minimal_reproducer.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/performance.rst` & `scikit-learn-1.4.2/doc/developers/performance.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/plotting.rst` & `scikit-learn-1.4.2/doc/developers/plotting.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/tips.rst` & `scikit-learn-1.4.2/doc/developers/tips.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/developers/utilities.rst` & `scikit-learn-1.4.2/doc/developers/utilities.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/documentation_team.rst` & `scikit-learn-1.4.2/doc/documentation_team.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/faq.rst` & `scikit-learn-1.4.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/getting_started.rst` & `scikit-learn-1.4.2/doc/getting_started.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/glossary.rst` & `scikit-learn-1.4.2/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/governance.rst` & `scikit-learn-1.4.2/doc/governance.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/axa-small.png` & `scikit-learn-1.4.2/doc/images/axa-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/axa.png` & `scikit-learn-1.4.2/doc/images/axa.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/bcg.png` & `scikit-learn-1.4.2/doc/images/bcg.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/beta_divergence.png` & `scikit-learn-1.4.2/doc/images/beta_divergence.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/bnp-small.png` & `scikit-learn-1.4.2/doc/images/bnp-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/bnp.png` & `scikit-learn-1.4.2/doc/images/bnp.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/cds-logo.png` & `scikit-learn-1.4.2/doc/images/cds-logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/chanel-small.png` & `scikit-learn-1.4.2/doc/images/chanel-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/chanel.png` & `scikit-learn-1.4.2/doc/images/chanel.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/columbia-small.png` & `scikit-learn-1.4.2/doc/images/columbia-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/columbia.png` & `scikit-learn-1.4.2/doc/images/columbia.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/czi_logo.svg` & `scikit-learn-1.4.2/doc/images/czi_logo.svg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/dataiku-small.png` & `scikit-learn-1.4.2/doc/images/dataiku-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/dataiku.png` & `scikit-learn-1.4.2/doc/images/dataiku.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/digicosme.png` & `scikit-learn-1.4.2/doc/images/digicosme.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/dysco.png` & `scikit-learn-1.4.2/doc/images/dysco.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/fnrs-logo-small.png` & `scikit-learn-1.4.2/doc/images/fnrs-logo-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/fujitsu.png` & `scikit-learn-1.4.2/doc/images/fujitsu.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/generated-doc-ci.png` & `scikit-learn-1.4.2/doc/images/generated-doc-ci.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/google-small.png` & `scikit-learn-1.4.2/doc/images/google-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/grid_search_cross_validation.png` & `scikit-learn-1.4.2/doc/images/grid_search_cross_validation.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/grid_search_workflow.png` & `scikit-learn-1.4.2/doc/images/grid_search_workflow.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/huggingface_logo-noborder.png` & `scikit-learn-1.4.2/doc/images/huggingface_logo-noborder.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/inria-logo.jpg` & `scikit-learn-1.4.2/doc/images/inria-logo.jpg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/inria-small.png` & `scikit-learn-1.4.2/doc/images/inria-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/intel-small.png` & `scikit-learn-1.4.2/doc/images/intel-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/intel.png` & `scikit-learn-1.4.2/doc/images/intel.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/iris.pdf` & `scikit-learn-1.4.2/doc/images/iris.pdf`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/iris.svg` & `scikit-learn-1.4.2/doc/images/iris.svg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/last_digit.png` & `scikit-learn-1.4.2/doc/images/last_digit.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/lda_model_graph.png` & `scikit-learn-1.4.2/doc/images/lda_model_graph.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/logo_APHP.png` & `scikit-learn-1.4.2/doc/images/logo_APHP.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/logo_APHP_text.png` & `scikit-learn-1.4.2/doc/images/logo_APHP_text.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/microsoft-small.png` & `scikit-learn-1.4.2/doc/images/microsoft-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/microsoft.png` & `scikit-learn-1.4.2/doc/images/microsoft.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/ml_map.png` & `scikit-learn-1.4.2/doc/images/ml_map.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/multi_org_chart.png` & `scikit-learn-1.4.2/doc/images/multi_org_chart.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/multilayerperceptron_network.png` & `scikit-learn-1.4.2/doc/images/multilayerperceptron_network.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/no_image.png` & `scikit-learn-1.4.2/doc/images/no_image.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/nvidia-small.png` & `scikit-learn-1.4.2/doc/images/nvidia-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/nvidia.png` & `scikit-learn-1.4.2/doc/images/nvidia.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/nyu_short_color.png` & `scikit-learn-1.4.2/doc/images/nyu_short_color.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/permuted_non_predictive_feature.png` & `scikit-learn-1.4.2/doc/images/permuted_non_predictive_feature.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/permuted_predictive_feature.png` & `scikit-learn-1.4.2/doc/images/permuted_predictive_feature.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/plot_digits_classification.png` & `scikit-learn-1.4.2/doc/images/plot_digits_classification.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/plot_face_recognition_1.png` & `scikit-learn-1.4.2/doc/images/plot_face_recognition_1.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/plot_face_recognition_2.png` & `scikit-learn-1.4.2/doc/images/plot_face_recognition_2.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/png-logo-inria-la-fondation.png` & `scikit-learn-1.4.2/doc/images/png-logo-inria-la-fondation.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/quansight-labs-small.png` & `scikit-learn-1.4.2/doc/images/quansight-labs-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/quansight-labs.png` & `scikit-learn-1.4.2/doc/images/quansight-labs.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/rbm_graph.png` & `scikit-learn-1.4.2/doc/images/rbm_graph.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/scikit-learn-logo-notext.png` & `scikit-learn-1.4.2/doc/images/scikit-learn-logo-notext.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/scikit-learn-logo-small.png` & `scikit-learn-1.4.2/doc/images/scikit-learn-logo-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/sloan_banner.png` & `scikit-learn-1.4.2/doc/images/sloan_banner.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/sloan_logo-small.png` & `scikit-learn-1.4.2/doc/images/sloan_logo-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/sydney-primary.jpeg` & `scikit-learn-1.4.2/doc/images/sydney-primary.jpeg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/sydney-stacked-small.png` & `scikit-learn-1.4.2/doc/images/sydney-stacked-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/target_encoder_cross_validation.svg` & `scikit-learn-1.4.2/doc/images/target_encoder_cross_validation.svg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/telecom-small.png` & `scikit-learn-1.4.2/doc/images/telecom-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/telecom.png` & `scikit-learn-1.4.2/doc/images/telecom.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/images/visual-studio-build-tools-selection.png` & `scikit-learn-1.4.2/doc/images/visual-studio-build-tools-selection.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/includes/big_toc_css.rst` & `scikit-learn-1.4.2/doc/includes/big_toc_css.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/includes/bigger_toc_css.rst` & `scikit-learn-1.4.2/doc/includes/bigger_toc_css.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/inspection.rst` & `scikit-learn-1.4.2/doc/inspection.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/install.rst` & `scikit-learn-1.4.2/doc/install.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/1280px-scikit-learn-logo.png` & `scikit-learn-1.4.2/doc/logos/1280px-scikit-learn-logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/README.md` & `scikit-learn-1.4.2/doc/logos/README.md`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/brand_guidelines/scikitlearn_logo_clearspace_updated.png` & `scikit-learn-1.4.2/doc/logos/brand_guidelines/scikitlearn_logo_clearspace_updated.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/favicon.ico` & `scikit-learn-1.4.2/doc/logos/favicon.ico`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/identity.pdf` & `scikit-learn-1.4.2/doc/logos/identity.pdf`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-notext.png` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo-notext.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-small.png` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo-small.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-thumb.png` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo-thumb.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo-without-subtitle.svg` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo-without-subtitle.svg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo.bmp` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo.bmp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo.png` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/logos/scikit-learn-logo.svg` & `scikit-learn-1.4.2/doc/logos/scikit-learn-logo.svg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/make.bat` & `scikit-learn-1.4.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/metadata_routing.rst` & `scikit-learn-1.4.2/doc/metadata_routing.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/model_persistence.rst` & `scikit-learn-1.4.2/doc/model_persistence.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/array_api.rst` & `scikit-learn-1.4.2/doc/modules/array_api.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/biclustering.rst` & `scikit-learn-1.4.2/doc/modules/biclustering.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/calibration.rst` & `scikit-learn-1.4.2/doc/modules/calibration.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/classes.rst` & `scikit-learn-1.4.2/doc/modules/classes.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/clustering.rst` & `scikit-learn-1.4.2/doc/modules/clustering.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/compose.rst` & `scikit-learn-1.4.2/doc/modules/compose.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/covariance.rst` & `scikit-learn-1.4.2/doc/modules/covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/cross_decomposition.rst` & `scikit-learn-1.4.2/doc/modules/cross_decomposition.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/cross_validation.rst` & `scikit-learn-1.4.2/doc/modules/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/decomposition.rst` & `scikit-learn-1.4.2/doc/modules/decomposition.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/density.rst` & `scikit-learn-1.4.2/doc/modules/density.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/ensemble.rst` & `scikit-learn-1.4.2/doc/modules/ensemble.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/feature_extraction.rst` & `scikit-learn-1.4.2/doc/modules/feature_extraction.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/feature_selection.rst` & `scikit-learn-1.4.2/doc/modules/feature_selection.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/gaussian_process.rst` & `scikit-learn-1.4.2/doc/modules/gaussian_process.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/glm_data/lasso_enet_coordinate_descent.png` & `scikit-learn-1.4.2/doc/modules/glm_data/lasso_enet_coordinate_descent.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/glm_data/poisson_gamma_tweedie_distributions.png` & `scikit-learn-1.4.2/doc/modules/glm_data/poisson_gamma_tweedie_distributions.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/grid_search.rst` & `scikit-learn-1.4.2/doc/modules/grid_search.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/impute.rst` & `scikit-learn-1.4.2/doc/modules/impute.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/isotonic.rst` & `scikit-learn-1.4.2/doc/modules/isotonic.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/kernel_approximation.rst` & `scikit-learn-1.4.2/doc/modules/kernel_approximation.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/kernel_ridge.rst` & `scikit-learn-1.4.2/doc/modules/kernel_ridge.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/lda_qda.rst` & `scikit-learn-1.4.2/doc/modules/lda_qda.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/learning_curve.rst` & `scikit-learn-1.4.2/doc/modules/learning_curve.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/linear_model.rst` & `scikit-learn-1.4.2/doc/modules/linear_model.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/manifold.rst` & `scikit-learn-1.4.2/doc/modules/manifold.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/metrics.rst` & `scikit-learn-1.4.2/doc/modules/metrics.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/mixture.rst` & `scikit-learn-1.4.2/doc/modules/mixture.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/model_evaluation.rst` & `scikit-learn-1.4.2/doc/modules/model_evaluation.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/multiclass.rst` & `scikit-learn-1.4.2/doc/modules/multiclass.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/naive_bayes.rst` & `scikit-learn-1.4.2/doc/modules/naive_bayes.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/neighbors.rst` & `scikit-learn-1.4.2/doc/modules/neighbors.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/neural_networks_supervised.rst` & `scikit-learn-1.4.2/doc/modules/neural_networks_supervised.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/neural_networks_unsupervised.rst` & `scikit-learn-1.4.2/doc/modules/neural_networks_unsupervised.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/outlier_detection.rst` & `scikit-learn-1.4.2/doc/modules/outlier_detection.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/partial_dependence.rst` & `scikit-learn-1.4.2/doc/modules/partial_dependence.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/permutation_importance.rst` & `scikit-learn-1.4.2/doc/modules/permutation_importance.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/preprocessing.rst` & `scikit-learn-1.4.2/doc/modules/preprocessing.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/preprocessing_targets.rst` & `scikit-learn-1.4.2/doc/modules/preprocessing_targets.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/random_projection.rst` & `scikit-learn-1.4.2/doc/modules/random_projection.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/semi_supervised.rst` & `scikit-learn-1.4.2/doc/modules/semi_supervised.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/sgd.rst` & `scikit-learn-1.4.2/doc/modules/sgd.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/svm.rst` & `scikit-learn-1.4.2/doc/modules/svm.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/tree.rst` & `scikit-learn-1.4.2/doc/modules/tree.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/modules/unsupervised_reduction.rst` & `scikit-learn-1.4.2/doc/modules/unsupervised_reduction.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/preface.rst` & `scikit-learn-1.4.2/doc/preface.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/presentations.rst` & `scikit-learn-1.4.2/doc/presentations.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/related_projects.rst` & `scikit-learn-1.4.2/doc/related_projects.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/roadmap.rst` & `scikit-learn-1.4.2/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/sphinxext/add_toctree_functions.py` & `scikit-learn-1.4.2/doc/sphinxext/add_toctree_functions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/sphinxext/allow_nan_estimators.py` & `scikit-learn-1.4.2/doc/sphinxext/allow_nan_estimators.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/sphinxext/doi_role.py` & `scikit-learn-1.4.2/doc/sphinxext/doi_role.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/sphinxext/github_link.py` & `scikit-learn-1.4.2/doc/sphinxext/github_link.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/sphinxext/sphinx_issues.py` & `scikit-learn-1.4.2/doc/sphinxext/sphinx_issues.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/supervised_learning.rst` & `scikit-learn-1.4.2/doc/supervised_learning.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/support.rst` & `scikit-learn-1.4.2/doc/support.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/templates/deprecated_class.rst` & `scikit-learn-1.4.2/doc/templates/deprecated_class.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/templates/deprecated_class_with_call.rst` & `scikit-learn-1.4.2/doc/templates/deprecated_class_with_call.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/templates/display_all_class_methods.rst` & `scikit-learn-1.4.2/doc/templates/display_all_class_methods.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/templates/index.html` & `scikit-learn-1.4.2/doc/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,16 @@
     <div class="row">
       <div class="col-md-4">
         <h4 class="sk-landing-call-header">News</h4>
         <ul class="sk-landing-call-list list-unstyled">
         <li><strong>On-going development:</strong>
         <a href="whats_new/v1.5.html#version-1-5-0">scikit-learn 1.5 (Changelog)</a>
         </li>
+        <li><strong>April 2024.</strong> scikit-learn 1.4.2 is available for download (<a href="whats_new/v1.4.html#version-1-4-2">Changelog</a>).
+        </li>
         <li><strong>February 2024.</strong> scikit-learn 1.4.1.post1 is available for download (<a href="whats_new/v1.4.html#version-1-4-1-post1">Changelog</a>).
         </li>
         <li><strong>January 2024.</strong> scikit-learn 1.4.0 is available for download (<a href="whats_new/v1.4.html#version-1-4-0">Changelog</a>).
         </li>
         <li><strong>October 2023.</strong> scikit-learn 1.3.2 is available for download (<a href="whats_new/v1.3.html#version-1-3-2">Changelog</a>).
         </li>
 	      <li><strong>September 2023.</strong> scikit-learn 1.3.1 is available for download (<a href="whats_new/v1.3.html#version-1-3-1">Changelog</a>).
@@ -247,14 +249,15 @@
 <div class="container-fluid py-3">
   <div class="container sk-landing-container">
         <a class="sk-footer-funding-link" href="about.html#funding">
         <div class="text-center">
                 <p class="mt-2">
                   scikit-learn development and maintenance are financially supported by
                 </p>
+                <img class="sk-footer-funding-logo" src="_static/probabl.png" title="Probabl">
                 <img class="sk-footer-funding-logo" src="_static/inria-small.png" title="INRIA">
                 <img class="sk-footer-funding-logo" src="_static/chanel-small.png" title="Chanel" >
                 <img class="sk-footer-funding-logo" src="_static/axa-small.png" title="AXA Assurances" >
                 <img class="sk-footer-funding-logo" src="_static/bnp-small.png" title="BNP Paris Bas Cardif" >
                 <img class="sk-footer-funding-logo" src="_static/microsoft-small.png" title="Microsoft" >
                 <img class="sk-footer-funding-logo" src="_static/dataiku-small.png" title="Dataiku" >
                 <img class="sk-footer-funding-logo" src="_static/huggingface_logo-noborder.png" title="Hugging Face" >
```

#### html2text {}

```diff
@@ -45,14 +45,15 @@
 Feature extraction and normalization.
 AApppplliiccaattiioonnss:: Transforming input data such as text for use with machine
 learning algorithms. AAllggoorriitthhmmss:: _p_r_e_p_r_o_c_e_s_s_i_n_g, _f_e_a_t_u_r_e_ _e_x_t_r_a_c_t_i_o_n, and _m_o_r_e_._._.
 _[_D_e_m_o_n_s_t_r_a_t_i_n_g_ _t_h_e_ _d_i_f_f_e_r_e_n_t_ _s_t_r_a_t_e_g_i_e_s_ _o_f_ _K_B_i_n_s_D_i_s_c_r_e_t_i_z_e_r_]
 _E_x_a_m_p_l_e_s
 ****** NNeewwss ******
     * OOnn--ggooiinngg ddeevveellooppmmeenntt:: _s_c_i_k_i_t_-_l_e_a_r_n_ _1_._5_ _(_C_h_a_n_g_e_l_o_g_)
+    * AApprriill 22002244.. scikit-learn 1.4.2 is available for download (_C_h_a_n_g_e_l_o_g).
     * FFeebbrruuaarryy 22002244.. scikit-learn 1.4.1.post1 is available for download
       (_C_h_a_n_g_e_l_o_g).
     * JJaannuuaarryy 22002244.. scikit-learn 1.4.0 is available for download (_C_h_a_n_g_e_l_o_g).
     * OOccttoobbeerr 22002233.. scikit-learn 1.3.2 is available for download (_C_h_a_n_g_e_l_o_g).
     * SSeepptteemmbbeerr 22002233.. scikit-learn 1.3.1 is available for download (_C_h_a_n_g_e_l_o_g).
     * JJuunnee 22002233.. scikit-learn 1.3.0 is available for download (_C_h_a_n_g_e_l_o_g).
     * AAllll rreelleeaasseess:: _WW_hh_aa_tt_''_ss_ _nn_ee_ww_ _(_C_h_a_n_g_e_l_o_g_)
@@ -81,12 +82,12 @@
 [telecomparistech]""TThhee ggrreeaatt bbeenneeffiitt ooff sscciikkiitt--lleeaarrnn iiss iittss ffaasstt lleeaarrnniinngg ccuurrvvee
 [[......]]""
 [aweber]""IItt aalllloowwss uuss ttoo ddoo AAWWeessoommee ssttuuffff wwee wwoouulldd nnoott ootthheerrwwiissee aaccccoommpplliisshh""
 [yhat]""sscciikkiitt--lleeaarrnn mmaakkeess ddooiinngg aaddvvaanncceedd aannaallyyssiiss iinn PPyytthhoonn aacccceessssiibbllee ttoo
 aannyyoonnee..""
 _M_o_r_e_ _t_e_s_t_i_m_o_n_i_a_l_s
 _s_c_i_k_i_t_-_l_e_a_r_n_ _d_e_v_e_l_o_p_m_e_n_t_ _a_n_d_ _m_a_i_n_t_e_n_a_n_c_e_ _a_r_e_ _f_i_n_a_n_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _b_y
-_[___s_t_a_t_i_c_/_i_n_r_i_a_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_c_h_a_n_e_l_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_a_x_a_-_s_m_a_l_l_._p_n_g_]
-_[___s_t_a_t_i_c_/_b_n_p_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_m_i_c_r_o_s_o_f_t_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_d_a_t_a_i_k_u_-_s_m_a_l_l_._p_n_g_]
-_[___s_t_a_t_i_c_/_h_u_g_g_i_n_g_f_a_c_e___l_o_g_o_-_n_o_b_o_r_d_e_r_._p_n_g_]_[___s_t_a_t_i_c_/_n_v_i_d_i_a_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/
-_q_u_a_n_s_i_g_h_t_-_l_a_b_s_-_s_m_a_l_l_._p_n_g_]
+_[___s_t_a_t_i_c_/_p_r_o_b_a_b_l_._p_n_g_]_[___s_t_a_t_i_c_/_i_n_r_i_a_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_c_h_a_n_e_l_-_s_m_a_l_l_._p_n_g_]
+_[___s_t_a_t_i_c_/_a_x_a_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_b_n_p_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_m_i_c_r_o_s_o_f_t_-_s_m_a_l_l_._p_n_g_]
+_[___s_t_a_t_i_c_/_d_a_t_a_i_k_u_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_h_u_g_g_i_n_g_f_a_c_e___l_o_g_o_-_n_o_b_o_r_d_e_r_._p_n_g_]_[___s_t_a_t_i_c_/
+_n_v_i_d_i_a_-_s_m_a_l_l_._p_n_g_]_[___s_t_a_t_i_c_/_q_u_a_n_s_i_g_h_t_-_l_a_b_s_-_s_m_a_l_l_._p_n_g_]
 {% endblock %}
```

### Comparing `scikit-learn-1.4.1.post1/doc/templates/redirects.html` & `scikit-learn-1.4.2/doc/templates/redirects.html`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/aweber.png` & `scikit-learn-1.4.2/doc/testimonials/images/aweber.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/bestofmedia-logo.png` & `scikit-learn-1.4.2/doc/testimonials/images/bestofmedia-logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/betaworks.png` & `scikit-learn-1.4.2/doc/testimonials/images/betaworks.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/birchbox.jpg` & `scikit-learn-1.4.2/doc/testimonials/images/birchbox.jpg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/bnp_paribas_cardif.png` & `scikit-learn-1.4.2/doc/testimonials/images/bnp_paribas_cardif.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/booking.png` & `scikit-learn-1.4.2/doc/testimonials/images/booking.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/change-logo.png` & `scikit-learn-1.4.2/doc/testimonials/images/change-logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/dataiku_logo.png` & `scikit-learn-1.4.2/doc/testimonials/images/dataiku_logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/datapublica.png` & `scikit-learn-1.4.2/doc/testimonials/images/datapublica.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/datarobot.png` & `scikit-learn-1.4.2/doc/testimonials/images/datarobot.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/evernote.png` & `scikit-learn-1.4.2/doc/testimonials/images/evernote.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/howaboutwe.png` & `scikit-learn-1.4.2/doc/testimonials/images/howaboutwe.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/huggingface.png` & `scikit-learn-1.4.2/doc/testimonials/images/huggingface.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/infonea.jpg` & `scikit-learn-1.4.2/doc/testimonials/images/infonea.jpg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/inria.png` & `scikit-learn-1.4.2/doc/testimonials/images/inria.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/jpmorgan.png` & `scikit-learn-1.4.2/doc/testimonials/images/jpmorgan.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/lovely.png` & `scikit-learn-1.4.2/doc/testimonials/images/lovely.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/machinalis.png` & `scikit-learn-1.4.2/doc/testimonials/images/machinalis.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/mars.png` & `scikit-learn-1.4.2/doc/testimonials/images/mars.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/okcupid.png` & `scikit-learn-1.4.2/doc/testimonials/images/okcupid.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/ottogroup_logo.png` & `scikit-learn-1.4.2/doc/testimonials/images/ottogroup_logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/peerindex.png` & `scikit-learn-1.4.2/doc/testimonials/images/peerindex.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/phimeca.png` & `scikit-learn-1.4.2/doc/testimonials/images/phimeca.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/rangespan.png` & `scikit-learn-1.4.2/doc/testimonials/images/rangespan.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/solido_logo.png` & `scikit-learn-1.4.2/doc/testimonials/images/solido_logo.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/spotify.png` & `scikit-learn-1.4.2/doc/testimonials/images/spotify.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/telecomparistech.jpg` & `scikit-learn-1.4.2/doc/testimonials/images/telecomparistech.jpg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/yhat.png` & `scikit-learn-1.4.2/doc/testimonials/images/yhat.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/images/zopa.png` & `scikit-learn-1.4.2/doc/testimonials/images/zopa.png`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/testimonials/testimonials.rst` & `scikit-learn-1.4.2/doc/testimonials/testimonials.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/javascript.html` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/javascript.html`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/layout.html` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/layout.html`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   <meta charset="utf-8">
   {{ metatags }}
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 
   {% block htmltitle %}
   <title>{{ title|striptags|e }}{{ titlesuffix }}</title>
   {% endblock %}
-  <link rel="canonical" href="http://scikit-learn.org/stable/{{pagename}}.html" />
+  <link rel="canonical" href="https://scikit-learn.org/stable/{{pagename}}.html" />
 
   {% if favicon_url %}
   <link rel="shortcut icon" href="{{ favicon_url|e }}"/>
   {% endif %}
 
   <link rel="stylesheet" href="{{ pathto('_static/css/vendor/bootstrap.min.css', 1) }}" type="text/css" />
   {%- for css in css_files %}
@@ -65,15 +65,15 @@
             <a href="#" role="button" class="btn sk-btn-rellink py-1 disabled"">Next</a>
           {%- endif %}
         </div>
         {%- if pagename != "install" %}
         <div class="alert alert-danger p-1 mb-2" role="alert">
           <p class="text-center mb-0">
           <strong>scikit-learn {{ release }}</strong><br/>
-          <a href="http://scikit-learn.org/dev/versions.html">Other versions</a>
+          <a href="https://scikit-learn.org/dev/versions.html">Other versions</a>
           </p>
         </div>
         {%- endif %}
         <div class="alert alert-warning p-1 mb-2" role="alert">
           <p class="text-center mb-0">
             Please <a class="font-weight-bold" href="{{ pathto('about').replace('#', '') }}#citing-scikit-learn"><string>cite us</string></a> if you use the software.
           </p>
```

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/nav.html` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/nav.html`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/css/theme.css` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/css/theme.css`

 * *Files 1% similar despite different names*

```diff
@@ -1316,14 +1316,18 @@
 
 @media screen and (min-width: 500px) {
   div.sk-sponsor-div-box, div.sk-testimonial-div-box {
     width: 50%;
   }
 }
 
+div.sk-sponsor-div-box table.sk-sponsor-table {
+  display: table;
+}
+
 table.sk-sponsor-table tr, table.sk-sponsor-table tr:nth-child(odd) {
   border-style: none;
   background-color: white;
   vertical-align: middle;
   text-align: center;
 }
```

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/css/vendor/bootstrap.min.css` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/css/vendor/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/details-permalink.js` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/details-permalink.js`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/vendor/bootstrap.min.js` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/vendor/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/themes/scikit-learn-modern/static/js/vendor/jquery-3.6.3.slim.min.js` & `scikit-learn-1.4.2/doc/themes/scikit-learn-modern/static/js/vendor/jquery-3.6.3.slim.min.js`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tune_toc.rst` & `scikit-learn-1.4.2/doc/tune_toc.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/basic/tutorial.rst` & `scikit-learn-1.4.2/doc/tutorial/basic/tutorial.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/index.rst` & `scikit-learn-1.4.2/doc/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/ML_MAPS_README.txt` & `scikit-learn-1.4.2/doc/tutorial/machine_learning_map/ML_MAPS_README.txt`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/index.rst` & `scikit-learn-1.4.2/doc/tutorial/machine_learning_map/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/parse_path.py` & `scikit-learn-1.4.2/doc/tutorial/machine_learning_map/parse_path.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/pyparsing.py` & `scikit-learn-1.4.2/doc/tutorial/machine_learning_map/pyparsing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/machine_learning_map/svg2imagemap.py` & `scikit-learn-1.4.2/doc/tutorial/machine_learning_map/svg2imagemap.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/index.rst` & `scikit-learn-1.4.2/doc/tutorial/statistical_inference/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/model_selection.rst` & `scikit-learn-1.4.2/doc/tutorial/statistical_inference/model_selection.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/putting_together.rst` & `scikit-learn-1.4.2/doc/tutorial/statistical_inference/putting_together.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/settings.rst` & `scikit-learn-1.4.2/doc/tutorial/statistical_inference/settings.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/supervised_learning.rst` & `scikit-learn-1.4.2/doc/tutorial/statistical_inference/supervised_learning.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/statistical_inference/unsupervised_learning.rst` & `scikit-learn-1.4.2/doc/tutorial/statistical_inference/unsupervised_learning.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/.gitignore` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/languages/fetch_data.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/data/languages/fetch_data.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/data/movie_reviews/fetch_data.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/data/movie_reviews/fetch_data.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/skeletons/exercise_01_language_train_model.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/skeletons/exercise_01_language_train_model.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/skeletons/exercise_02_sentiment.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/skeletons/exercise_02_sentiment.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/exercise_01_language_train_model.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/exercise_01_language_train_model.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/exercise_02_sentiment.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/exercise_02_sentiment.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/solutions/generate_skeletons.py` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/solutions/generate_skeletons.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/tutorial/text_analytics/working_with_text_data.rst` & `scikit-learn-1.4.2/doc/tutorial/text_analytics/working_with_text_data.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/user_guide.rst` & `scikit-learn-1.4.2/doc/user_guide.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/visualizations.rst` & `scikit-learn-1.4.2/doc/visualizations.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/_contributors.rst` & `scikit-learn-1.4.2/doc/whats_new/_contributors.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/changelog_legend.inc` & `scikit-learn-1.4.2/doc/whats_new/changelog_legend.inc`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/older_versions.rst` & `scikit-learn-1.4.2/doc/whats_new/older_versions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1120,15 +1120,15 @@
 applications to real-world datasets.
 
 
 Changelog
 ---------
 
 - New `stochastic gradient
-  <http://scikit-learn.org/stable/modules/sgd.html>`_ descent
+  <https://scikit-learn.org/stable/modules/sgd.html>`_ descent
   module by Peter Prettenhofer. The module comes with complete
   documentation and examples.
 
 - Improved svm module: memory consumption has been reduced by 50%,
   heuristic to automatically set class weights, possibility to
   assign weights to samples (see
   :ref:`sphx_glr_auto_examples_svm_plot_weighted_samples.py` for an example).
@@ -1252,17 +1252,17 @@
 
 Documentation
 -------------
 
 - Improved documentation for many modules, now separating
   narrative documentation from the class reference. As an example,
   see `documentation for the SVM module
-  <http://scikit-learn.org/stable/modules/svm.html>`_ and the
+  <https://scikit-learn.org/stable/modules/svm.html>`_ and the
   complete `class reference
-  <http://scikit-learn.org/stable/modules/classes.html>`_.
+  <https://scikit-learn.org/stable/modules/classes.html>`_.
 
 Fixes
 -----
 
 - API changes: adhere variable names to PEP-8, give more
   meaningful names.
 
@@ -1276,15 +1276,15 @@
 --------
 
 - new examples using some of the mlcomp datasets:
   ``sphx_glr_auto_examples_mlcomp_sparse_document_classification.py`` (since removed) and
   :ref:`sphx_glr_auto_examples_text_plot_document_classification_20newsgroups.py`
 
 - Many more examples. `See here
-  <http://scikit-learn.org/stable/auto_examples/index.html>`_
+  <https://scikit-learn.org/stable/auto_examples/index.html>`_
   the full list of examples.
 
 
 External dependencies
 ---------------------
 
 - Joblib is now a dependency of this package, although it is
```

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.13.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.13.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.14.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.14.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.15.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.15.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.16.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.16.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.17.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.17.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.18.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.18.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.19.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.19.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.20.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.20.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.21.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.21.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.22.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.22.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.23.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.23.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v0.24.rst` & `scikit-learn-1.4.2/doc/whats_new/v0.24.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v1.0.rst` & `scikit-learn-1.4.2/doc/whats_new/v1.0.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v1.1.rst` & `scikit-learn-1.4.2/doc/whats_new/v1.1.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v1.2.rst` & `scikit-learn-1.4.2/doc/whats_new/v1.2.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v1.3.rst` & `scikit-learn-1.4.2/doc/whats_new/v1.3.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new/v1.4.rst` & `scikit-learn-1.4.2/doc/whats_new/v1.4.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 ===========
 
 For a short description of the main highlights of the release, please refer to
 :ref:`sphx_glr_auto_examples_release_highlights_plot_release_highlights_1_4_0.py`.
 
 .. include:: changelog_legend.inc
 
+.. _changes_1_4_2:
+
+Version 1.4.2
+=============
+
+**April 2024**
+
+This release only includes support for numpy 2.
+
 .. _changes_1_4_1:
 
 Version 1.4.1.post1
 ===================
 
 **February 2024**
```

### Comparing `scikit-learn-1.4.1.post1/doc/whats_new.rst` & `scikit-learn-1.4.2/doc/whats_new.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_cyclical_feature_engineering.py` & `scikit-learn-1.4.2/examples/applications/plot_cyclical_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_digits_denoising.py` & `scikit-learn-1.4.2/examples/applications/plot_digits_denoising.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_face_recognition.py` & `scikit-learn-1.4.2/examples/applications/plot_face_recognition.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_model_complexity_influence.py` & `scikit-learn-1.4.2/examples/applications/plot_model_complexity_influence.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_out_of_core_classification.py` & `scikit-learn-1.4.2/examples/applications/plot_out_of_core_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_outlier_detection_wine.py` & `scikit-learn-1.4.2/examples/applications/plot_outlier_detection_wine.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_prediction_latency.py` & `scikit-learn-1.4.2/examples/applications/plot_prediction_latency.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_species_distribution_modeling.py` & `scikit-learn-1.4.2/examples/applications/plot_species_distribution_modeling.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_stock_market.py` & `scikit-learn-1.4.2/examples/applications/plot_stock_market.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_time_series_lagged_features.py` & `scikit-learn-1.4.2/examples/applications/plot_time_series_lagged_features.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_tomography_l1_reconstruction.py` & `scikit-learn-1.4.2/examples/applications/plot_tomography_l1_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/plot_topics_extraction_with_nmf_lda.py` & `scikit-learn-1.4.2/examples/applications/plot_topics_extraction_with_nmf_lda.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/svm_gui.py` & `scikit-learn-1.4.2/examples/applications/svm_gui.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/applications/wikipedia_principal_eigenvector.py` & `scikit-learn-1.4.2/examples/applications/wikipedia_principal_eigenvector.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/bicluster/plot_bicluster_newsgroups.py` & `scikit-learn-1.4.2/examples/bicluster/plot_bicluster_newsgroups.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/bicluster/plot_spectral_biclustering.py` & `scikit-learn-1.4.2/examples/bicluster/plot_spectral_biclustering.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/bicluster/plot_spectral_coclustering.py` & `scikit-learn-1.4.2/examples/bicluster/plot_spectral_coclustering.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/calibration/plot_calibration.py` & `scikit-learn-1.4.2/examples/calibration/plot_calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/calibration/plot_calibration_curve.py` & `scikit-learn-1.4.2/examples/calibration/plot_calibration_curve.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/calibration/plot_calibration_multiclass.py` & `scikit-learn-1.4.2/examples/calibration/plot_calibration_multiclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/classification/plot_classification_probability.py` & `scikit-learn-1.4.2/examples/classification/plot_classification_probability.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/classification/plot_classifier_comparison.py` & `scikit-learn-1.4.2/examples/classification/plot_classifier_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/classification/plot_digits_classification.py` & `scikit-learn-1.4.2/examples/classification/plot_digits_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/classification/plot_lda.py` & `scikit-learn-1.4.2/examples/classification/plot_lda.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/classification/plot_lda_qda.py` & `scikit-learn-1.4.2/examples/classification/plot_lda_qda.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_adjusted_for_chance_measures.py` & `scikit-learn-1.4.2/examples/cluster/plot_adjusted_for_chance_measures.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_affinity_propagation.py` & `scikit-learn-1.4.2/examples/cluster/plot_affinity_propagation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_agglomerative_clustering.py` & `scikit-learn-1.4.2/examples/cluster/plot_agglomerative_clustering.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_agglomerative_clustering_metrics.py` & `scikit-learn-1.4.2/examples/cluster/plot_agglomerative_clustering_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_agglomerative_dendrogram.py` & `scikit-learn-1.4.2/examples/cluster/plot_agglomerative_dendrogram.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_birch_vs_minibatchkmeans.py` & `scikit-learn-1.4.2/examples/cluster/plot_birch_vs_minibatchkmeans.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_bisect_kmeans.py` & `scikit-learn-1.4.2/examples/cluster/plot_bisect_kmeans.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_cluster_comparison.py` & `scikit-learn-1.4.2/examples/cluster/plot_cluster_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_cluster_iris.py` & `scikit-learn-1.4.2/examples/cluster/plot_cluster_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_coin_segmentation.py` & `scikit-learn-1.4.2/examples/cluster/plot_coin_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_coin_ward_segmentation.py` & `scikit-learn-1.4.2/examples/cluster/plot_coin_ward_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_color_quantization.py` & `scikit-learn-1.4.2/examples/cluster/plot_color_quantization.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_dbscan.py` & `scikit-learn-1.4.2/examples/cluster/plot_dbscan.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_dict_face_patches.py` & `scikit-learn-1.4.2/examples/cluster/plot_dict_face_patches.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_digits_agglomeration.py` & `scikit-learn-1.4.2/examples/cluster/plot_digits_agglomeration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_digits_linkage.py` & `scikit-learn-1.4.2/examples/cluster/plot_digits_linkage.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_face_compress.py` & `scikit-learn-1.4.2/examples/cluster/plot_face_compress.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_feature_agglomeration_vs_univariate_selection.py` & `scikit-learn-1.4.2/examples/cluster/plot_feature_agglomeration_vs_univariate_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_hdbscan.py` & `scikit-learn-1.4.2/examples/cluster/plot_hdbscan.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_inductive_clustering.py` & `scikit-learn-1.4.2/examples/cluster/plot_inductive_clustering.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_assumptions.py` & `scikit-learn-1.4.2/examples/cluster/plot_kmeans_assumptions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_digits.py` & `scikit-learn-1.4.2/examples/cluster/plot_kmeans_digits.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_plusplus.py` & `scikit-learn-1.4.2/examples/cluster/plot_kmeans_plusplus.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_silhouette_analysis.py` & `scikit-learn-1.4.2/examples/cluster/plot_kmeans_silhouette_analysis.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_kmeans_stability_low_dim_dense.py` & `scikit-learn-1.4.2/examples/cluster/plot_kmeans_stability_low_dim_dense.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_linkage_comparison.py` & `scikit-learn-1.4.2/examples/cluster/plot_linkage_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_mean_shift.py` & `scikit-learn-1.4.2/examples/cluster/plot_mean_shift.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_mini_batch_kmeans.py` & `scikit-learn-1.4.2/examples/cluster/plot_mini_batch_kmeans.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_optics.py` & `scikit-learn-1.4.2/examples/cluster/plot_optics.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_segmentation_toy.py` & `scikit-learn-1.4.2/examples/cluster/plot_segmentation_toy.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cluster/plot_ward_structured_vs_unstructured.py` & `scikit-learn-1.4.2/examples/cluster/plot_ward_structured_vs_unstructured.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/compose/plot_column_transformer.py` & `scikit-learn-1.4.2/examples/compose/plot_column_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/compose/plot_column_transformer_mixed_types.py` & `scikit-learn-1.4.2/examples/compose/plot_column_transformer_mixed_types.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/compose/plot_compare_reduction.py` & `scikit-learn-1.4.2/examples/compose/plot_compare_reduction.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/compose/plot_digits_pipe.py` & `scikit-learn-1.4.2/examples/compose/plot_digits_pipe.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/compose/plot_feature_union.py` & `scikit-learn-1.4.2/examples/compose/plot_feature_union.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/compose/plot_transformed_target.py` & `scikit-learn-1.4.2/examples/compose/plot_transformed_target.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/covariance/plot_covariance_estimation.py` & `scikit-learn-1.4.2/examples/covariance/plot_covariance_estimation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/covariance/plot_lw_vs_oas.py` & `scikit-learn-1.4.2/examples/covariance/plot_lw_vs_oas.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/covariance/plot_mahalanobis_distances.py` & `scikit-learn-1.4.2/examples/covariance/plot_mahalanobis_distances.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/covariance/plot_robust_vs_empirical_covariance.py` & `scikit-learn-1.4.2/examples/covariance/plot_robust_vs_empirical_covariance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/covariance/plot_sparse_cov.py` & `scikit-learn-1.4.2/examples/covariance/plot_sparse_cov.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cross_decomposition/plot_compare_cross_decomposition.py` & `scikit-learn-1.4.2/examples/cross_decomposition/plot_compare_cross_decomposition.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/cross_decomposition/plot_pcr_vs_pls.py` & `scikit-learn-1.4.2/examples/cross_decomposition/plot_pcr_vs_pls.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/datasets/plot_digits_last_image.py` & `scikit-learn-1.4.2/examples/datasets/plot_digits_last_image.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/datasets/plot_iris_dataset.py` & `scikit-learn-1.4.2/examples/datasets/plot_iris_dataset.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/datasets/plot_random_dataset.py` & `scikit-learn-1.4.2/examples/datasets/plot_random_dataset.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/datasets/plot_random_multilabel_dataset.py` & `scikit-learn-1.4.2/examples/datasets/plot_random_multilabel_dataset.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_faces_decomposition.py` & `scikit-learn-1.4.2/examples/decomposition/plot_faces_decomposition.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_ica_blind_source_separation.py` & `scikit-learn-1.4.2/examples/decomposition/plot_ica_blind_source_separation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_ica_vs_pca.py` & `scikit-learn-1.4.2/examples/decomposition/plot_ica_vs_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_image_denoising.py` & `scikit-learn-1.4.2/examples/decomposition/plot_image_denoising.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_incremental_pca.py` & `scikit-learn-1.4.2/examples/decomposition/plot_incremental_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_kernel_pca.py` & `scikit-learn-1.4.2/examples/decomposition/plot_kernel_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_pca_iris.py` & `scikit-learn-1.4.2/examples/decomposition/plot_pca_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_pca_vs_fa_model_selection.py` & `scikit-learn-1.4.2/examples/decomposition/plot_pca_vs_fa_model_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_pca_vs_lda.py` & `scikit-learn-1.4.2/examples/decomposition/plot_pca_vs_lda.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_sparse_coding.py` & `scikit-learn-1.4.2/examples/decomposition/plot_sparse_coding.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/decomposition/plot_varimax_fa.py` & `scikit-learn-1.4.2/examples/decomposition/plot_varimax_fa.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/developing_estimators/sklearn_is_fitted.py` & `scikit-learn-1.4.2/examples/developing_estimators/sklearn_is_fitted.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_adaboost_multiclass.py` & `scikit-learn-1.4.2/examples/ensemble/plot_adaboost_multiclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_adaboost_regression.py` & `scikit-learn-1.4.2/examples/ensemble/plot_adaboost_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_adaboost_twoclass.py` & `scikit-learn-1.4.2/examples/ensemble/plot_adaboost_twoclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_bias_variance.py` & `scikit-learn-1.4.2/examples/ensemble/plot_bias_variance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_ensemble_oob.py` & `scikit-learn-1.4.2/examples/ensemble/plot_ensemble_oob.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_feature_transformation.py` & `scikit-learn-1.4.2/examples/ensemble/plot_feature_transformation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_hist_grad_boosting_comparison.py` & `scikit-learn-1.4.2/examples/ensemble/plot_forest_hist_grad_boosting_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_importances.py` & `scikit-learn-1.4.2/examples/ensemble/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_importances_faces.py` & `scikit-learn-1.4.2/examples/ensemble/plot_forest_importances_faces.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_forest_iris.py` & `scikit-learn-1.4.2/examples/ensemble/plot_forest_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_categorical.py` & `scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_categorical.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_early_stopping.py` & `scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_early_stopping.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_oob.py` & `scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_oob.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_quantile.py` & `scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_quantile.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_regression.py` & `scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_gradient_boosting_regularization.py` & `scikit-learn-1.4.2/examples/ensemble/plot_gradient_boosting_regularization.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_isolation_forest.py` & `scikit-learn-1.4.2/examples/ensemble/plot_isolation_forest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_monotonic_constraints.py` & `scikit-learn-1.4.2/examples/ensemble/plot_monotonic_constraints.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_random_forest_embedding.py` & `scikit-learn-1.4.2/examples/ensemble/plot_random_forest_embedding.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_random_forest_regression_multioutput.py` & `scikit-learn-1.4.2/examples/ensemble/plot_random_forest_regression_multioutput.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_stack_predictors.py` & `scikit-learn-1.4.2/examples/ensemble/plot_stack_predictors.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_voting_decision_regions.py` & `scikit-learn-1.4.2/examples/ensemble/plot_voting_decision_regions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_voting_probas.py` & `scikit-learn-1.4.2/examples/ensemble/plot_voting_probas.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/ensemble/plot_voting_regressor.py` & `scikit-learn-1.4.2/examples/ensemble/plot_voting_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/exercises/plot_cv_diabetes.py` & `scikit-learn-1.4.2/examples/exercises/plot_cv_diabetes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/exercises/plot_digits_classification_exercise.py` & `scikit-learn-1.4.2/examples/exercises/plot_digits_classification_exercise.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/exercises/plot_iris_exercise.py` & `scikit-learn-1.4.2/examples/exercises/plot_iris_exercise.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/feature_selection/plot_f_test_vs_mi.py` & `scikit-learn-1.4.2/examples/feature_selection/plot_f_test_vs_mi.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/feature_selection/plot_feature_selection.py` & `scikit-learn-1.4.2/examples/feature_selection/plot_feature_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/feature_selection/plot_feature_selection_pipeline.py` & `scikit-learn-1.4.2/examples/feature_selection/plot_feature_selection_pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/feature_selection/plot_rfe_digits.py` & `scikit-learn-1.4.2/examples/feature_selection/plot_rfe_digits.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/feature_selection/plot_rfe_with_cross_validation.py` & `scikit-learn-1.4.2/examples/feature_selection/plot_rfe_with_cross_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/feature_selection/plot_select_from_model_diabetes.py` & `scikit-learn-1.4.2/examples/feature_selection/plot_select_from_model_diabetes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_compare_gpr_krr.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_compare_gpr_krr.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpc.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc_iris.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpc_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc_isoprobability.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpc_isoprobability.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpc_xor.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpc_xor.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_co2.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_co2.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_noisy.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_noisy.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_noisy_targets.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_noisy_targets.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_on_structured_data.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_on_structured_data.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/gaussian_process/plot_gpr_prior_posterior.py` & `scikit-learn-1.4.2/examples/gaussian_process/plot_gpr_prior_posterior.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/impute/plot_iterative_imputer_variants_comparison.py` & `scikit-learn-1.4.2/examples/impute/plot_iterative_imputer_variants_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/impute/plot_missing_values.py` & `scikit-learn-1.4.2/examples/impute/plot_missing_values.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/inspection/plot_causal_interpretation.py` & `scikit-learn-1.4.2/examples/inspection/plot_causal_interpretation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/inspection/plot_linear_model_coefficient_interpretation.py` & `scikit-learn-1.4.2/examples/inspection/plot_linear_model_coefficient_interpretation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/inspection/plot_partial_dependence.py` & `scikit-learn-1.4.2/examples/inspection/plot_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/inspection/plot_permutation_importance.py` & `scikit-learn-1.4.2/examples/inspection/plot_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/inspection/plot_permutation_importance_multicollinear.py` & `scikit-learn-1.4.2/examples/inspection/plot_permutation_importance_multicollinear.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/kernel_approximation/plot_scalable_poly_kernels.py` & `scikit-learn-1.4.2/examples/kernel_approximation/plot_scalable_poly_kernels.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ard.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ard.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_bayesian_ridge_curvefit.py` & `scikit-learn-1.4.2/examples/linear_model/plot_bayesian_ridge_curvefit.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_elastic_net_precomputed_gram_matrix_with_weighted_samples.py` & `scikit-learn-1.4.2/examples/linear_model/plot_elastic_net_precomputed_gram_matrix_with_weighted_samples.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_huber_vs_ridge.py` & `scikit-learn-1.4.2/examples/linear_model/plot_huber_vs_ridge.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_iris_logistic.py` & `scikit-learn-1.4.2/examples/linear_model/plot_iris_logistic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_and_elasticnet.py` & `scikit-learn-1.4.2/examples/linear_model/plot_lasso_and_elasticnet.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_coordinate_descent_path.py` & `scikit-learn-1.4.2/examples/linear_model/plot_lasso_coordinate_descent_path.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_dense_vs_sparse_data.py` & `scikit-learn-1.4.2/examples/linear_model/plot_lasso_dense_vs_sparse_data.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_lars.py` & `scikit-learn-1.4.2/examples/linear_model/plot_lasso_lars.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_lars_ic.py` & `scikit-learn-1.4.2/examples/linear_model/plot_lasso_lars_ic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_lasso_model_selection.py` & `scikit-learn-1.4.2/examples/linear_model/plot_lasso_model_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic.py` & `scikit-learn-1.4.2/examples/linear_model/plot_logistic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic_l1_l2_sparsity.py` & `scikit-learn-1.4.2/examples/linear_model/plot_logistic_l1_l2_sparsity.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic_multinomial.py` & `scikit-learn-1.4.2/examples/linear_model/plot_logistic_multinomial.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_logistic_path.py` & `scikit-learn-1.4.2/examples/linear_model/plot_logistic_path.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_multi_task_lasso_support.py` & `scikit-learn-1.4.2/examples/linear_model/plot_multi_task_lasso_support.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_nnls.py` & `scikit-learn-1.4.2/examples/linear_model/plot_nnls.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ols.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ols.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ols_3d.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ols_3d.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ols_ridge_variance.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ols_ridge_variance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_omp.py` & `scikit-learn-1.4.2/examples/linear_model/plot_omp.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_poisson_regression_non_normal_loss.py` & `scikit-learn-1.4.2/examples/linear_model/plot_poisson_regression_non_normal_loss.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_polynomial_interpolation.py` & `scikit-learn-1.4.2/examples/linear_model/plot_polynomial_interpolation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_quantile_regression.py` & `scikit-learn-1.4.2/examples/linear_model/plot_quantile_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ransac.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ransac.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ridge_coeffs.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ridge_coeffs.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_ridge_path.py` & `scikit-learn-1.4.2/examples/linear_model/plot_ridge_path.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_robust_fit.py` & `scikit-learn-1.4.2/examples/linear_model/plot_robust_fit.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_comparison.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_early_stopping.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_early_stopping.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_iris.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_loss_functions.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_loss_functions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_penalties.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_penalties.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_separating_hyperplane.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_separating_hyperplane.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgd_weighted_samples.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgd_weighted_samples.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sgdocsvm_vs_ocsvm.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sgdocsvm_vs_ocsvm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sparse_logistic_regression_20newsgroups.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sparse_logistic_regression_20newsgroups.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_sparse_logistic_regression_mnist.py` & `scikit-learn-1.4.2/examples/linear_model/plot_sparse_logistic_regression_mnist.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_theilsen.py` & `scikit-learn-1.4.2/examples/linear_model/plot_theilsen.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/linear_model/plot_tweedie_regression_insurance_claims.py` & `scikit-learn-1.4.2/examples/linear_model/plot_tweedie_regression_insurance_claims.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/manifold/plot_compare_methods.py` & `scikit-learn-1.4.2/examples/manifold/plot_compare_methods.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/manifold/plot_lle_digits.py` & `scikit-learn-1.4.2/examples/manifold/plot_lle_digits.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/manifold/plot_manifold_sphere.py` & `scikit-learn-1.4.2/examples/manifold/plot_manifold_sphere.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/manifold/plot_mds.py` & `scikit-learn-1.4.2/examples/manifold/plot_mds.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/manifold/plot_swissroll.py` & `scikit-learn-1.4.2/examples/manifold/plot_swissroll.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/manifold/plot_t_sne_perplexity.py` & `scikit-learn-1.4.2/examples/manifold/plot_t_sne_perplexity.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_anomaly_comparison.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_anomaly_comparison.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_display_object_visualization.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_display_object_visualization.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_estimator_representation.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_estimator_representation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_isotonic_regression.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_isotonic_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_johnson_lindenstrauss_bound.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_johnson_lindenstrauss_bound.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_kernel_approximation.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_kernel_approximation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_kernel_ridge_regression.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_kernel_ridge_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_metadata_routing.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_metadata_routing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_multilabel.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_multilabel.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_multioutput_face_completion.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_multioutput_face_completion.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_outlier_detection_bench.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_outlier_detection_bench.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_partial_dependence_visualization_api.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_partial_dependence_visualization_api.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_pipeline_display.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_pipeline_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_roc_curve_visualization_api.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_roc_curve_visualization_api.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/miscellaneous/plot_set_output.py` & `scikit-learn-1.4.2/examples/miscellaneous/plot_set_output.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_concentration_prior.py` & `scikit-learn-1.4.2/examples/mixture/plot_concentration_prior.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_gmm.py` & `scikit-learn-1.4.2/examples/mixture/plot_gmm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_covariances.py` & `scikit-learn-1.4.2/examples/mixture/plot_gmm_covariances.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_init.py` & `scikit-learn-1.4.2/examples/mixture/plot_gmm_init.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_pdf.py` & `scikit-learn-1.4.2/examples/mixture/plot_gmm_pdf.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_selection.py` & `scikit-learn-1.4.2/examples/mixture/plot_gmm_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/mixture/plot_gmm_sin.py` & `scikit-learn-1.4.2/examples/mixture/plot_gmm_sin.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_confusion_matrix.py` & `scikit-learn-1.4.2/examples/model_selection/plot_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_cv_indices.py` & `scikit-learn-1.4.2/examples/model_selection/plot_cv_indices.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_cv_predict.py` & `scikit-learn-1.4.2/examples/model_selection/plot_cv_predict.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_det.py` & `scikit-learn-1.4.2/examples/model_selection/plot_det.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_digits.py` & `scikit-learn-1.4.2/examples/model_selection/plot_grid_search_digits.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_refit_callable.py` & `scikit-learn-1.4.2/examples/model_selection/plot_grid_search_refit_callable.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_stats.py` & `scikit-learn-1.4.2/examples/model_selection/plot_grid_search_stats.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_grid_search_text_feature_extraction.py` & `scikit-learn-1.4.2/examples/model_selection/plot_grid_search_text_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_learning_curve.py` & `scikit-learn-1.4.2/examples/model_selection/plot_learning_curve.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_likelihood_ratios.py` & `scikit-learn-1.4.2/examples/model_selection/plot_likelihood_ratios.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_multi_metric_evaluation.py` & `scikit-learn-1.4.2/examples/model_selection/plot_multi_metric_evaluation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_nested_cross_validation_iris.py` & `scikit-learn-1.4.2/examples/model_selection/plot_nested_cross_validation_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_permutation_tests_for_classification.py` & `scikit-learn-1.4.2/examples/model_selection/plot_permutation_tests_for_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_precision_recall.py` & `scikit-learn-1.4.2/examples/model_selection/plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_randomized_search.py` & `scikit-learn-1.4.2/examples/model_selection/plot_randomized_search.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_roc.py` & `scikit-learn-1.4.2/examples/model_selection/plot_roc.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_roc_crossval.py` & `scikit-learn-1.4.2/examples/model_selection/plot_roc_crossval.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_successive_halving_heatmap.py` & `scikit-learn-1.4.2/examples/model_selection/plot_successive_halving_heatmap.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_successive_halving_iterations.py` & `scikit-learn-1.4.2/examples/model_selection/plot_successive_halving_iterations.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_train_error_vs_test_error.py` & `scikit-learn-1.4.2/examples/model_selection/plot_train_error_vs_test_error.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_underfitting_overfitting.py` & `scikit-learn-1.4.2/examples/model_selection/plot_underfitting_overfitting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/model_selection/plot_validation_curve.py` & `scikit-learn-1.4.2/examples/model_selection/plot_validation_curve.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/multiclass/plot_multiclass_overview.py` & `scikit-learn-1.4.2/examples/multiclass/plot_multiclass_overview.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/multioutput/plot_classifier_chain_yeast.py` & `scikit-learn-1.4.2/examples/multioutput/plot_classifier_chain_yeast.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/approximate_nearest_neighbors.py` & `scikit-learn-1.4.2/examples/neighbors/approximate_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_caching_nearest_neighbors.py` & `scikit-learn-1.4.2/examples/neighbors/plot_caching_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_classification.py` & `scikit-learn-1.4.2/examples/neighbors/plot_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_digits_kde_sampling.py` & `scikit-learn-1.4.2/examples/neighbors/plot_digits_kde_sampling.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_kde_1d.py` & `scikit-learn-1.4.2/examples/neighbors/plot_kde_1d.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_lof_novelty_detection.py` & `scikit-learn-1.4.2/examples/neighbors/plot_lof_novelty_detection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_lof_outlier_detection.py` & `scikit-learn-1.4.2/examples/neighbors/plot_lof_outlier_detection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_nca_classification.py` & `scikit-learn-1.4.2/examples/neighbors/plot_nca_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_nca_dim_reduction.py` & `scikit-learn-1.4.2/examples/neighbors/plot_nca_dim_reduction.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_nca_illustration.py` & `scikit-learn-1.4.2/examples/neighbors/plot_nca_illustration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_nearest_centroid.py` & `scikit-learn-1.4.2/examples/neighbors/plot_nearest_centroid.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_regression.py` & `scikit-learn-1.4.2/examples/neighbors/plot_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neighbors/plot_species_kde.py` & `scikit-learn-1.4.2/examples/neighbors/plot_species_kde.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neural_networks/plot_mlp_alpha.py` & `scikit-learn-1.4.2/examples/neural_networks/plot_mlp_alpha.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neural_networks/plot_mlp_training_curves.py` & `scikit-learn-1.4.2/examples/neural_networks/plot_mlp_training_curves.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neural_networks/plot_mnist_filters.py` & `scikit-learn-1.4.2/examples/neural_networks/plot_mnist_filters.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/neural_networks/plot_rbm_logistic_classification.py` & `scikit-learn-1.4.2/examples/neural_networks/plot_rbm_logistic_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_all_scaling.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_all_scaling.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_discretization.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_discretization.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_discretization_classification.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_discretization_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_discretization_strategies.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_discretization_strategies.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_map_data_to_normal.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_map_data_to_normal.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_scaling_importance.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_scaling_importance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_target_encoder.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_target_encoder.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/preprocessing/plot_target_encoder_cross_val.py` & `scikit-learn-1.4.2/examples/preprocessing/plot_target_encoder_cross_val.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_0_22_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_0_22_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_0_23_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_0_23_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_0_24_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_0_24_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_0_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_0_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_1_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_1_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_2_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_2_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_3_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_3_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/release_highlights/plot_release_highlights_1_4_0.py` & `scikit-learn-1.4.2/examples/release_highlights/plot_release_highlights_1_4_0.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/semi_supervised/plot_label_propagation_digits.py` & `scikit-learn-1.4.2/examples/semi_supervised/plot_label_propagation_digits.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/semi_supervised/plot_label_propagation_digits_active_learning.py` & `scikit-learn-1.4.2/examples/semi_supervised/plot_label_propagation_digits_active_learning.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/semi_supervised/plot_label_propagation_structure.py` & `scikit-learn-1.4.2/examples/semi_supervised/plot_label_propagation_structure.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/semi_supervised/plot_self_training_varying_threshold.py` & `scikit-learn-1.4.2/examples/semi_supervised/plot_self_training_varying_threshold.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/semi_supervised/plot_semi_supervised_newsgroups.py` & `scikit-learn-1.4.2/examples/semi_supervised/plot_semi_supervised_newsgroups.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/semi_supervised/plot_semi_supervised_versus_svm_iris.py` & `scikit-learn-1.4.2/examples/semi_supervised/plot_semi_supervised_versus_svm_iris.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_custom_kernel.py` & `scikit-learn-1.4.2/examples/svm/plot_custom_kernel.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_iris_svc.py` & `scikit-learn-1.4.2/examples/svm/plot_iris_svc.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_linearsvc_support_vectors.py` & `scikit-learn-1.4.2/examples/svm/plot_linearsvc_support_vectors.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_oneclass.py` & `scikit-learn-1.4.2/examples/svm/plot_oneclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_rbf_parameters.py` & `scikit-learn-1.4.2/examples/svm/plot_rbf_parameters.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_separating_hyperplane.py` & `scikit-learn-1.4.2/examples/svm/plot_separating_hyperplane.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_separating_hyperplane_unbalanced.py` & `scikit-learn-1.4.2/examples/svm/plot_separating_hyperplane_unbalanced.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_anova.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_anova.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_kernels.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_kernels.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_margin.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_margin.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_nonlinear.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_nonlinear.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_regression.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_scale_c.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_scale_c.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_svm_tie_breaking.py` & `scikit-learn-1.4.2/examples/svm/plot_svm_tie_breaking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/svm/plot_weighted_samples.py` & `scikit-learn-1.4.2/examples/svm/plot_weighted_samples.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/text/plot_document_classification_20newsgroups.py` & `scikit-learn-1.4.2/examples/text/plot_document_classification_20newsgroups.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/text/plot_document_clustering.py` & `scikit-learn-1.4.2/examples/text/plot_document_clustering.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/text/plot_hashing_vs_dict_vectorizer.py` & `scikit-learn-1.4.2/examples/text/plot_hashing_vs_dict_vectorizer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/tree/plot_cost_complexity_pruning.py` & `scikit-learn-1.4.2/examples/tree/plot_cost_complexity_pruning.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/tree/plot_iris_dtc.py` & `scikit-learn-1.4.2/examples/tree/plot_iris_dtc.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/tree/plot_tree_regression.py` & `scikit-learn-1.4.2/examples/tree/plot_tree_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/tree/plot_tree_regression_multioutput.py` & `scikit-learn-1.4.2/examples/tree/plot_tree_regression_multioutput.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/examples/tree/plot_unveil_tree_structure.py` & `scikit-learn-1.4.2/examples/tree/plot_unveil_tree_structure.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/meson.build` & `scikit-learn-1.4.2/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/pyproject.toml` & `scikit-learn-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = [
     "setuptools",
     "wheel",
     "Cython>=3.0.8",
-    "numpy>=1.25",
+    "numpy==2.0.0rc1",
     "scipy>=1.6.0",
 ]
 
 [tool.black]
 line-length = 88
 target_version = ['py39', 'py310', 'py311']
 preview = true
```

### Comparing `scikit-learn-1.4.1.post1/scikit_learn.egg-info/PKG-INFO` & `scikit-learn-1.4.2/scikit_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-learn
-Version: 1.4.1.post1
+Version: 1.4.2
 Summary: A set of python modules for machine learning and data mining
 Home-page: https://scikit-learn.org
 Maintainer: Andreas Mueller
 Maintainer-email: amueller@ais.uni-bonn.de
 License: new BSD
 Download-URL: https://pypi.org/project/scikit-learn/#files
 Project-URL: Bug Tracker, https://github.com/scikit-learn/scikit-learn/issues
```

### Comparing `scikit-learn-1.4.1.post1/scikit_learn.egg-info/SOURCES.txt` & `scikit-learn-1.4.2/scikit_learn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 doc/images/nyu_short_color.png
 doc/images/permuted_non_predictive_feature.png
 doc/images/permuted_predictive_feature.png
 doc/images/plot_digits_classification.png
 doc/images/plot_face_recognition_1.png
 doc/images/plot_face_recognition_2.png
 doc/images/png-logo-inria-la-fondation.png
+doc/images/probabl.png
 doc/images/quansight-labs-small.png
 doc/images/quansight-labs.png
 doc/images/rbm_graph.png
 doc/images/scikit-learn-logo-notext.png
 doc/images/scikit-learn-logo-small.png
 doc/images/sloan_banner.png
 doc/images/sloan_logo-small.png
```

### Comparing `scikit-learn-1.4.1.post1/scikit_learn.egg-info/requires.txt` & `scikit-learn-1.4.2/scikit_learn.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-numpy<2.0,>=1.19.5
+numpy>=1.19.5
 scipy>=1.6.0
 joblib>=1.2.0
 threadpoolctl>=2.0.0
 
 [benchmark]
 matplotlib>=3.3.4
 pandas>=1.1.5
```

### Comparing `scikit-learn-1.4.1.post1/setup.cfg` & `scikit-learn-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/setup.py` & `scikit-learn-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,20 +610,14 @@
         zip_safe=False,  # the package can run out of an .egg file
         extras_require={
             key: min_deps.tag_to_packages[key]
             for key in ["examples", "docs", "tests", "benchmark"]
         },
     )
 
-    # Overwrite the dependencies to not allow for NumPy >= 2.0
-    metadata["install_requires"] = [
-        f"{dep},<2.0" if dep.startswith("numpy") else dep
-        for dep in metadata["install_requires"]
-    ]
-
     commands = [arg for arg in sys.argv[1:] if not arg.startswith("-")]
     if not all(
         command in ("egg_info", "dist_info", "clean", "check") for command in commands
     ):
         if sys.version_info < required_python_version:
             required_version = "%d.%d" % required_python_version
             raise RuntimeError(
```

### Comparing `scikit-learn-1.4.1.post1/sklearn/__check_build/__init__.py` & `scikit-learn-1.4.2/sklearn/__check_build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/__init__.py` & `scikit-learn-1.4.2/sklearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # learning algorithms in the tightly-knit world of scientific Python
 # packages (numpy, scipy, matplotlib).
 #
 # It aims to provide simple and efficient solutions to learning problems
 # that are accessible to everybody and reusable in various contexts:
 # machine-learning as a versatile tool for science and engineering.
 #
-# See http://scikit-learn.org for complete documentation.
+# See https://scikit-learn.org for complete documentation.
 
 import logging
 import os
 import random
 import sys
 
 from ._config import config_context, get_config, set_config
@@ -38,15 +38,15 @@
 #   X.Y.ZbN   # Beta release
 #   X.Y.ZrcN  # Release Candidate
 #   X.Y.Z     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "1.4.1.post1"
+__version__ = "1.4.2"
 
 
 # On OSX, we can get a runtime error due to multiple OpenMP libraries loaded
 # simultaneously. This can happen for instance when calling BLAS inside a
 # prange. Setting the following environment variable allows multiple OpenMP
 # libraries to be loaded. It should not degrade performances since we manually
 # take care of potential over-subcription performance issues, in sections of
```

### Comparing `scikit-learn-1.4.1.post1/sklearn/_build_utils/__init__.py` & `scikit-learn-1.4.2/sklearn/_build_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_build_utils/openmp_helpers.py` & `scikit-learn-1.4.2/sklearn/_build_utils/openmp_helpers.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_build_utils/pre_build_helpers.py` & `scikit-learn-1.4.2/sklearn/_build_utils/pre_build_helpers.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_build_utils/tempita.py` & `scikit-learn-1.4.2/sklearn/_build_utils/tempita.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_config.py` & `scikit-learn-1.4.2/sklearn/_config.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_isotonic.pyx` & `scikit-learn-1.4.2/sklearn/_isotonic.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/__init__.py` & `scikit-learn-1.4.2/sklearn/_loss/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/_loss.pxd` & `scikit-learn-1.4.2/sklearn/_loss/_loss.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/_loss.pyx.tp` & `scikit-learn-1.4.2/sklearn/_loss/_loss.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/link.py` & `scikit-learn-1.4.2/sklearn/_loss/link.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/loss.py` & `scikit-learn-1.4.2/sklearn/_loss/loss.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/tests/test_link.py` & `scikit-learn-1.4.2/sklearn/_loss/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_loss/tests/test_loss.py` & `scikit-learn-1.4.2/sklearn/_loss/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/_min_dependencies.py` & `scikit-learn-1.4.2/sklearn/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/base.py` & `scikit-learn-1.4.2/sklearn/base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/calibration.py` & `scikit-learn-1.4.2/sklearn/calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/__init__.py` & `scikit-learn-1.4.2/sklearn/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_affinity_propagation.py` & `scikit-learn-1.4.2/sklearn/cluster/_affinity_propagation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_agglomerative.py` & `scikit-learn-1.4.2/sklearn/cluster/_agglomerative.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_bicluster.py` & `scikit-learn-1.4.2/sklearn/cluster/_bicluster.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_birch.py` & `scikit-learn-1.4.2/sklearn/cluster/_birch.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_bisect_k_means.py` & `scikit-learn-1.4.2/sklearn/cluster/_bisect_k_means.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_dbscan.py` & `scikit-learn-1.4.2/sklearn/cluster/_dbscan.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_dbscan_inner.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_dbscan_inner.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_feature_agglomeration.py` & `scikit-learn-1.4.2/sklearn/cluster/_feature_agglomeration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_linkage.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_linkage.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_reachability.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_reachability.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_tree.pxd` & `scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_tree.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/_tree.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_hdbscan/_tree.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/hdbscan.py` & `scikit-learn-1.4.2/sklearn/cluster/_hdbscan/hdbscan.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hdbscan/tests/test_reachibility.py` & `scikit-learn-1.4.2/sklearn/cluster/_hdbscan/tests/test_reachibility.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_hierarchical_fast.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_hierarchical_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_common.pxd` & `scikit-learn-1.4.2/sklearn/cluster/_k_means_common.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_common.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_k_means_common.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_elkan.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_k_means_elkan.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_lloyd.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_k_means_lloyd.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_k_means_minibatch.pyx` & `scikit-learn-1.4.2/sklearn/cluster/_k_means_minibatch.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_kmeans.py` & `scikit-learn-1.4.2/sklearn/cluster/_kmeans.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_mean_shift.py` & `scikit-learn-1.4.2/sklearn/cluster/_mean_shift.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_optics.py` & `scikit-learn-1.4.2/sklearn/cluster/_optics.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/_spectral.py` & `scikit-learn-1.4.2/sklearn/cluster/_spectral.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/meson.build` & `scikit-learn-1.4.2/sklearn/cluster/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/common.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_affinity_propagation.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_affinity_propagation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_bicluster.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_bicluster.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_birch.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_birch.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_bisect_k_means.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_bisect_k_means.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_dbscan.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_dbscan.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_feature_agglomeration.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_feature_agglomeration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_hdbscan.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_hdbscan.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_hierarchical.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_hierarchical.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_k_means.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_k_means.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_mean_shift.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_mean_shift.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_optics.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_optics.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cluster/tests/test_spectral.py` & `scikit-learn-1.4.2/sklearn/cluster/tests/test_spectral.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/compose/_column_transformer.py` & `scikit-learn-1.4.2/sklearn/compose/_column_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/compose/_target.py` & `scikit-learn-1.4.2/sklearn/compose/_target.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/compose/tests/test_column_transformer.py` & `scikit-learn-1.4.2/sklearn/compose/tests/test_column_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/compose/tests/test_target.py` & `scikit-learn-1.4.2/sklearn/compose/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/conftest.py` & `scikit-learn-1.4.2/sklearn/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/__init__.py` & `scikit-learn-1.4.2/sklearn/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/_elliptic_envelope.py` & `scikit-learn-1.4.2/sklearn/covariance/_elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/_empirical_covariance.py` & `scikit-learn-1.4.2/sklearn/covariance/_empirical_covariance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/_graph_lasso.py` & `scikit-learn-1.4.2/sklearn/covariance/_graph_lasso.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/_robust_covariance.py` & `scikit-learn-1.4.2/sklearn/covariance/_robust_covariance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/_shrunk_covariance.py` & `scikit-learn-1.4.2/sklearn/covariance/_shrunk_covariance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_covariance.py` & `scikit-learn-1.4.2/sklearn/covariance/tests/test_covariance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_elliptic_envelope.py` & `scikit-learn-1.4.2/sklearn/covariance/tests/test_elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_graphical_lasso.py` & `scikit-learn-1.4.2/sklearn/covariance/tests/test_graphical_lasso.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/covariance/tests/test_robust_covariance.py` & `scikit-learn-1.4.2/sklearn/covariance/tests/test_robust_covariance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cross_decomposition/_pls.py` & `scikit-learn-1.4.2/sklearn/cross_decomposition/_pls.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/cross_decomposition/tests/test_pls.py` & `scikit-learn-1.4.2/sklearn/cross_decomposition/tests/test_pls.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/__init__.py` & `scikit-learn-1.4.2/sklearn/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_arff_parser.py` & `scikit-learn-1.4.2/sklearn/datasets/_arff_parser.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_base.py` & `scikit-learn-1.4.2/sklearn/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_california_housing.py` & `scikit-learn-1.4.2/sklearn/datasets/_california_housing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_covtype.py` & `scikit-learn-1.4.2/sklearn/datasets/_covtype.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_kddcup99.py` & `scikit-learn-1.4.2/sklearn/datasets/_kddcup99.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_lfw.py` & `scikit-learn-1.4.2/sklearn/datasets/_lfw.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_olivetti_faces.py` & `scikit-learn-1.4.2/sklearn/datasets/_olivetti_faces.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_openml.py` & `scikit-learn-1.4.2/sklearn/datasets/_openml.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_rcv1.py` & `scikit-learn-1.4.2/sklearn/datasets/_rcv1.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_samples_generator.py` & `scikit-learn-1.4.2/sklearn/datasets/_samples_generator.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_species_distributions.py` & `scikit-learn-1.4.2/sklearn/datasets/_species_distributions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_svmlight_format_fast.pyx` & `scikit-learn-1.4.2/sklearn/datasets/_svmlight_format_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_svmlight_format_io.py` & `scikit-learn-1.4.2/sklearn/datasets/_svmlight_format_io.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/_twenty_newsgroups.py` & `scikit-learn-1.4.2/sklearn/datasets/_twenty_newsgroups.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/boston_house_prices.csv` & `scikit-learn-1.4.2/sklearn/datasets/data/boston_house_prices.csv`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/breast_cancer.csv` & `scikit-learn-1.4.2/sklearn/datasets/data/breast_cancer.csv`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/diabetes_data_raw.csv.gz` & `scikit-learn-1.4.2/sklearn/datasets/data/diabetes_data_raw.csv.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/diabetes_target.csv.gz` & `scikit-learn-1.4.2/sklearn/datasets/data/diabetes_target.csv.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/digits.csv.gz` & `scikit-learn-1.4.2/sklearn/datasets/data/digits.csv.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/iris.csv` & `scikit-learn-1.4.2/sklearn/datasets/data/iris.csv`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/data/wine_data.csv` & `scikit-learn-1.4.2/sklearn/datasets/data/wine_data.csv`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/breast_cancer.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/breast_cancer.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/california_housing.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/california_housing.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/covtype.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/covtype.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/diabetes.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/diabetes.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/digits.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/digits.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/iris.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/iris.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/kddcup99.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/kddcup99.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/lfw.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/lfw.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/linnerud.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/linnerud.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/olivetti_faces.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/olivetti_faces.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/rcv1.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/rcv1.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/species_distributions.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/species_distributions.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/twenty_newsgroups.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/twenty_newsgroups.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/descr/wine_data.rst` & `scikit-learn-1.4.2/sklearn/datasets/descr/wine_data.rst`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/images/README.txt` & `scikit-learn-1.4.2/sklearn/datasets/images/README.txt`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/images/china.jpg` & `scikit-learn-1.4.2/sklearn/datasets/images/china.jpg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/images/flower.jpg` & `scikit-learn-1.4.2/sklearn/datasets/images/flower.jpg`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/api-v1-jd-1.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/api-v1-jd-1.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/api-v1-jdf-1.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/api-v1-jdf-1.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1/data-v1-dl-1.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1/data-v1-dl-1.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jd-1119.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jd-1119.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdf-1119.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdf-1119.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdq-1119.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/api-v1-jdq-1119.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1119/data-v1-dl-54002.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1119/data-v1-dl-54002.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/api-v1-jd-1590.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/api-v1-jd-1590.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdf-1590.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdf-1590.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdq-1590.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/api-v1-jdq-1590.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_1590/data-v1-dl-1595261.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_1590/data-v1-dl-1595261.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jd-2.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jd-2.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jdf-2.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jdf-2.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/api-v1-jdq-2.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/api-v1-jdq-2.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_2/data-v1-dl-1666876.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_2/data-v1-dl-1666876.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-292.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-292.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-40981.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/api-v1-jd-40981.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_292/data-v1-dl-49822.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_292/data-v1-dl-49822.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/api-v1-jd-3.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/api-v1-jd-3.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/api-v1-jdf-3.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/api-v1-jdf-3.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/api-v1-jdq-3.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/api-v1-jdq-3.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_3/data-v1-dl-3.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_3/data-v1-dl-3.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jd-40589.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jd-40589.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdf-40589.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdf-40589.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdq-40589.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/api-v1-jdq-40589.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40589/data-v1-dl-4644182.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40589/data-v1-dl-4644182.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdq-40675.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/api-v1-jdq-40675.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40675/data-v1-dl-4965250.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40675/data-v1-dl-4965250.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/api-v1-jdq-40945.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/api-v1-jdq-40945.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40945/data-v1-dl-16826755.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40945/data-v1-dl-16826755.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jd-40966.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jd-40966.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdf-40966.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdf-40966.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdq-40966.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/api-v1-jdq-40966.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_40966/data-v1-dl-17928620.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_40966/data-v1-dl-17928620.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/api-v1-jd-42074.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/api-v1-jd-42074.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/api-v1-jdq-42074.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/api-v1-jdq-42074.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42074/data-v1-dl-21552912.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42074/data-v1-dl-21552912.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/api-v1-jd-42585.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/api-v1-jd-42585.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_42585/data-v1-dl-21854866.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_42585/data-v1-dl-21854866.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jd-561.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jd-561.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/api-v1-jdq-561.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/api-v1-jdq-561.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_561/data-v1-dl-52739.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_561/data-v1-dl-52739.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jd-61.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jd-61.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/api-v1-jdq-61.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/api-v1-jdq-61.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_61/data-v1-dl-61.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_61/data-v1-dl-61.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/api-v1-jd-62.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/api-v1-jd-62.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/api-v1-jdf-62.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/api-v1-jdf-62.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/api-v1-jdq-62.json.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/api-v1-jdq-62.json.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/data/openml/id_62/data-v1-dl-52352.arff.gz` & `scikit-learn-1.4.2/sklearn/datasets/tests/data/openml/id_62/data-v1-dl-52352.arff.gz`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_20news.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_20news.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_arff_parser.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_arff_parser.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_california_housing.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_california_housing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_covtype.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_covtype.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_kddcup99.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_kddcup99.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_lfw.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_lfw.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_olivetti_faces.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_olivetti_faces.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_openml.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_openml.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_rcv1.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_rcv1.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_samples_generator.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_samples_generator.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/datasets/tests/test_svmlight_format.py` & `scikit-learn-1.4.2/sklearn/datasets/tests/test_svmlight_format.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/__init__.py` & `scikit-learn-1.4.2/sklearn/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_base.py` & `scikit-learn-1.4.2/sklearn/decomposition/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_cdnmf_fast.pyx` & `scikit-learn-1.4.2/sklearn/decomposition/_cdnmf_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_dict_learning.py` & `scikit-learn-1.4.2/sklearn/decomposition/_dict_learning.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_factor_analysis.py` & `scikit-learn-1.4.2/sklearn/decomposition/_factor_analysis.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_fastica.py` & `scikit-learn-1.4.2/sklearn/decomposition/_fastica.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_incremental_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/_incremental_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_kernel_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/_kernel_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_lda.py` & `scikit-learn-1.4.2/sklearn/decomposition/_lda.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_nmf.py` & `scikit-learn-1.4.2/sklearn/decomposition/_nmf.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_online_lda_fast.pyx` & `scikit-learn-1.4.2/sklearn/decomposition/_online_lda_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_sparse_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/_sparse_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/_truncated_svd.py` & `scikit-learn-1.4.2/sklearn/decomposition/_truncated_svd.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_dict_learning.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_dict_learning.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_factor_analysis.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_factor_analysis.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_fastica.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_fastica.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_incremental_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_incremental_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_kernel_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_kernel_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_nmf.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_nmf.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_online_lda.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_online_lda.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_sparse_pca.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_sparse_pca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/decomposition/tests/test_truncated_svd.py` & `scikit-learn-1.4.2/sklearn/decomposition/tests/test_truncated_svd.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/discriminant_analysis.py` & `scikit-learn-1.4.2/sklearn/discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/dummy.py` & `scikit-learn-1.4.2/sklearn/dummy.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/__init__.py` & `scikit-learn-1.4.2/sklearn/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_bagging.py` & `scikit-learn-1.4.2/sklearn/ensemble/_bagging.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_base.py` & `scikit-learn-1.4.2/sklearn/ensemble/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_forest.py` & `scikit-learn-1.4.2/sklearn/ensemble/_forest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_gb.py` & `scikit-learn-1.4.2/sklearn/ensemble/_gb.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_gradient_boosting.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_gradient_boosting.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_binning.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_binning.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_bitset.pxd` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_bitset.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_bitset.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_bitset.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_gradient_boosting.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_gradient_boosting.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/_predictor.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/_predictor.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/binning.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/binning.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/common.pxd` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/common.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/common.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/common.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/gradient_boosting.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/grower.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/grower.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/histogram.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/histogram.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/meson.build` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/predictor.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/predictor.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/splitting.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/splitting.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_binning.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_bitset.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_bitset.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_compare_lightgbm.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_compare_lightgbm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_gradient_boosting.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_grower.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_grower.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_histogram.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_monotonic_contraints.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_monotonic_contraints.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_predictor.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_predictor.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_splitting.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_splitting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/tests/test_warm_start.py` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/tests/test_warm_start.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_hist_gradient_boosting/utils.pyx` & `scikit-learn-1.4.2/sklearn/ensemble/_hist_gradient_boosting/utils.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_iforest.py` & `scikit-learn-1.4.2/sklearn/ensemble/_iforest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_stacking.py` & `scikit-learn-1.4.2/sklearn/ensemble/_stacking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_voting.py` & `scikit-learn-1.4.2/sklearn/ensemble/_voting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/_weight_boosting.py` & `scikit-learn-1.4.2/sklearn/ensemble/_weight_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_bagging.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_bagging.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_forest.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_forest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_gradient_boosting.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_iforest.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_iforest.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_stacking.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_stacking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_voting.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_voting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/ensemble/tests/test_weight_boosting.py` & `scikit-learn-1.4.2/sklearn/ensemble/tests/test_weight_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/exceptions.py` & `scikit-learn-1.4.2/sklearn/exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/experimental/enable_halving_search_cv.py` & `scikit-learn-1.4.2/sklearn/experimental/enable_halving_search_cv.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/experimental/enable_hist_gradient_boosting.py` & `scikit-learn-1.4.2/sklearn/experimental/enable_hist_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/experimental/enable_iterative_imputer.py` & `scikit-learn-1.4.2/sklearn/experimental/enable_iterative_imputer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/experimental/tests/test_enable_hist_gradient_boosting.py` & `scikit-learn-1.4.2/sklearn/experimental/tests/test_enable_hist_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/experimental/tests/test_enable_iterative_imputer.py` & `scikit-learn-1.4.2/sklearn/experimental/tests/test_enable_iterative_imputer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/experimental/tests/test_enable_successive_halving.py` & `scikit-learn-1.4.2/sklearn/experimental/tests/test_enable_successive_halving.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/externals/_arff.py` & `scikit-learn-1.4.2/sklearn/externals/_arff.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/externals/_packaging/_structures.py` & `scikit-learn-1.4.2/sklearn/externals/_packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/externals/_packaging/version.py` & `scikit-learn-1.4.2/sklearn/externals/_packaging/version.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/externals/_scipy/sparse/csgraph/_laplacian.py` & `scikit-learn-1.4.2/sklearn/externals/_scipy/sparse/csgraph/_laplacian.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/_dict_vectorizer.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/_dict_vectorizer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/_hash.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/_hash.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/_hashing_fast.pyx` & `scikit-learn-1.4.2/sklearn/feature_extraction/_hashing_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/_stop_words.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/_stop_words.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/image.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/image.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_dict_vectorizer.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_dict_vectorizer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_feature_hasher.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_feature_hasher.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_image.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/tests/test_text.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_extraction/text.py` & `scikit-learn-1.4.2/sklearn/feature_extraction/text.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/__init__.py` & `scikit-learn-1.4.2/sklearn/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_base.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_from_model.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_from_model.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_mutual_info.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_mutual_info.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_rfe.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_rfe.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_sequential.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_sequential.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_univariate_selection.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_univariate_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/_variance_threshold.py` & `scikit-learn-1.4.2/sklearn/feature_selection/_variance_threshold.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_chi2.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_chi2.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_feature_select.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_feature_select.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_from_model.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_from_model.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_mutual_info.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_mutual_info.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_rfe.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_rfe.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_sequential.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_sequential.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/feature_selection/tests/test_variance_threshold.py` & `scikit-learn-1.4.2/sklearn/feature_selection/tests/test_variance_threshold.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/_gpc.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/_gpc.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/_gpr.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/_gpr.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/kernels.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/kernels.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/_mini_sequence_kernel.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/tests/_mini_sequence_kernel.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/test_gpc.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/tests/test_gpc.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/test_gpr.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/tests/test_gpr.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/gaussian_process/tests/test_kernels.py` & `scikit-learn-1.4.2/sklearn/gaussian_process/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/__init__.py` & `scikit-learn-1.4.2/sklearn/impute/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/_base.py` & `scikit-learn-1.4.2/sklearn/impute/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/_iterative.py` & `scikit-learn-1.4.2/sklearn/impute/_iterative.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/_knn.py` & `scikit-learn-1.4.2/sklearn/impute/_knn.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/impute/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/impute/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/tests/test_impute.py` & `scikit-learn-1.4.2/sklearn/impute/tests/test_impute.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/impute/tests/test_knn.py` & `scikit-learn-1.4.2/sklearn/impute/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_partial_dependence.py` & `scikit-learn-1.4.2/sklearn/inspection/_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_pd_utils.py` & `scikit-learn-1.4.2/sklearn/inspection/_pd_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_permutation_importance.py` & `scikit-learn-1.4.2/sklearn/inspection/_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_plot/decision_boundary.py` & `scikit-learn-1.4.2/sklearn/inspection/_plot/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_plot/partial_dependence.py` & `scikit-learn-1.4.2/sklearn/inspection/_plot/partial_dependence.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_plot/tests/test_boundary_decision_display.py` & `scikit-learn-1.4.2/sklearn/inspection/_plot/tests/test_boundary_decision_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/_plot/tests/test_plot_partial_dependence.py` & `scikit-learn-1.4.2/sklearn/inspection/_plot/tests/test_plot_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/tests/test_partial_dependence.py` & `scikit-learn-1.4.2/sklearn/inspection/tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/tests/test_pd_utils.py` & `scikit-learn-1.4.2/sklearn/inspection/tests/test_pd_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/inspection/tests/test_permutation_importance.py` & `scikit-learn-1.4.2/sklearn/inspection/tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/isotonic.py` & `scikit-learn-1.4.2/sklearn/isotonic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/kernel_approximation.py` & `scikit-learn-1.4.2/sklearn/kernel_approximation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/kernel_ridge.py` & `scikit-learn-1.4.2/sklearn/kernel_ridge.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/__init__.py` & `scikit-learn-1.4.2/sklearn/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_base.py` & `scikit-learn-1.4.2/sklearn/linear_model/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_bayes.py` & `scikit-learn-1.4.2/sklearn/linear_model/_bayes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_cd_fast.pyx` & `scikit-learn-1.4.2/sklearn/linear_model/_cd_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_coordinate_descent.py` & `scikit-learn-1.4.2/sklearn/linear_model/_coordinate_descent.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/_newton_solver.py` & `scikit-learn-1.4.2/sklearn/linear_model/_glm/_newton_solver.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/glm.py` & `scikit-learn-1.4.2/sklearn/linear_model/_glm/glm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_glm/tests/test_glm.py` & `scikit-learn-1.4.2/sklearn/linear_model/_glm/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_huber.py` & `scikit-learn-1.4.2/sklearn/linear_model/_huber.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_least_angle.py` & `scikit-learn-1.4.2/sklearn/linear_model/_least_angle.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_linear_loss.py` & `scikit-learn-1.4.2/sklearn/linear_model/_linear_loss.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_logistic.py` & `scikit-learn-1.4.2/sklearn/linear_model/_logistic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_omp.py` & `scikit-learn-1.4.2/sklearn/linear_model/_omp.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_passive_aggressive.py` & `scikit-learn-1.4.2/sklearn/linear_model/_passive_aggressive.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_perceptron.py` & `scikit-learn-1.4.2/sklearn/linear_model/_perceptron.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_quantile.py` & `scikit-learn-1.4.2/sklearn/linear_model/_quantile.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_ransac.py` & `scikit-learn-1.4.2/sklearn/linear_model/_ransac.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_ridge.py` & `scikit-learn-1.4.2/sklearn/linear_model/_ridge.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_sag.py` & `scikit-learn-1.4.2/sklearn/linear_model/_sag.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_sag_fast.pyx.tp` & `scikit-learn-1.4.2/sklearn/linear_model/_sag_fast.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_sgd_fast.pxd` & `scikit-learn-1.4.2/sklearn/linear_model/_sgd_fast.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_sgd_fast.pyx.tp` & `scikit-learn-1.4.2/sklearn/linear_model/_sgd_fast.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_sgd_fast_helpers.h` & `scikit-learn-1.4.2/sklearn/linear_model/_sgd_fast_helpers.h`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_stochastic_gradient.py` & `scikit-learn-1.4.2/sklearn/linear_model/_stochastic_gradient.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/_theil_sen.py` & `scikit-learn-1.4.2/sklearn/linear_model/_theil_sen.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/meson.build` & `scikit-learn-1.4.2/sklearn/linear_model/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_bayes.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_bayes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_coordinate_descent.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_coordinate_descent.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_huber.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_huber.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_least_angle.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_least_angle.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_linear_loss.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_linear_loss.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_logistic.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_logistic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_omp.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_omp.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_passive_aggressive.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_passive_aggressive.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_perceptron.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_perceptron.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_quantile.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_ransac.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_ransac.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_ridge.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_ridge.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_sag.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_sag.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_sgd.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_sgd.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_sparse_coordinate_descent.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_sparse_coordinate_descent.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/linear_model/tests/test_theil_sen.py` & `scikit-learn-1.4.2/sklearn/linear_model/tests/test_theil_sen.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/__init__.py` & `scikit-learn-1.4.2/sklearn/manifold/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_barnes_hut_tsne.pyx` & `scikit-learn-1.4.2/sklearn/manifold/_barnes_hut_tsne.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_isomap.py` & `scikit-learn-1.4.2/sklearn/manifold/_isomap.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_locally_linear.py` & `scikit-learn-1.4.2/sklearn/manifold/_locally_linear.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_mds.py` & `scikit-learn-1.4.2/sklearn/manifold/_mds.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_spectral_embedding.py` & `scikit-learn-1.4.2/sklearn/manifold/_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_t_sne.py` & `scikit-learn-1.4.2/sklearn/manifold/_t_sne.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/_utils.pyx` & `scikit-learn-1.4.2/sklearn/manifold/_utils.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_isomap.py` & `scikit-learn-1.4.2/sklearn/manifold/tests/test_isomap.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_locally_linear.py` & `scikit-learn-1.4.2/sklearn/manifold/tests/test_locally_linear.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_mds.py` & `scikit-learn-1.4.2/sklearn/manifold/tests/test_mds.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_spectral_embedding.py` & `scikit-learn-1.4.2/sklearn/manifold/tests/test_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/manifold/tests/test_t_sne.py` & `scikit-learn-1.4.2/sklearn/manifold/tests/test_t_sne.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/meson.build` & `scikit-learn-1.4.2/sklearn/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/__init__.py` & `scikit-learn-1.4.2/sklearn/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_base.py` & `scikit-learn-1.4.2/sklearn/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_classification.py` & `scikit-learn-1.4.2/sklearn/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_dist_metrics.pxd.tp` & `scikit-learn-1.4.2/sklearn/metrics/_dist_metrics.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_dist_metrics.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_dist_metrics.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/__init__.py` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pxd.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_argkmin.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_argkmin_classmode.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_argkmin_classmode.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_base.pxd.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_base.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_base.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_base.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pxd.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_datasets_pair.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_dispatcher.py` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pxd.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_middle_term_computer.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pxd.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors_classmode.pyx.tp` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/_radius_neighbors_classmode.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_distances_reduction/meson.build` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_distances_reduction/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_pairwise_fast.pyx` & `scikit-learn-1.4.2/sklearn/metrics/_pairwise_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/confusion_matrix.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/det_curve.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/det_curve.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/precision_recall_curve.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/regression.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/roc_curve.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/roc_curve.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_common_curve_display.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_common_curve_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_confusion_matrix_display.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_confusion_matrix_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_det_curve_display.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_det_curve_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_precision_recall_display.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_precision_recall_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_predict_error_display.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_predict_error_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_plot/tests/test_roc_curve_display.py` & `scikit-learn-1.4.2/sklearn/metrics/_plot/tests/test_roc_curve_display.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_ranking.py` & `scikit-learn-1.4.2/sklearn/metrics/_ranking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_regression.py` & `scikit-learn-1.4.2/sklearn/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/_scorer.py` & `scikit-learn-1.4.2/sklearn/metrics/_scorer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/__init__.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_bicluster.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/_bicluster.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_expected_mutual_info_fast.pyx` & `scikit-learn-1.4.2/sklearn/metrics/cluster/_expected_mutual_info_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_supervised.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/_supervised.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/_unsupervised.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/_unsupervised.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_bicluster.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_bicluster.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_supervised.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_supervised.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/cluster/tests/test_unsupervised.py` & `scikit-learn-1.4.2/sklearn/metrics/cluster/tests/test_unsupervised.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/meson.build` & `scikit-learn-1.4.2/sklearn/metrics/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/pairwise.py` & `scikit-learn-1.4.2/sklearn/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_classification.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_dist_metrics.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_dist_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_pairwise.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_pairwise.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_pairwise_distances_reduction.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_pairwise_distances_reduction.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_ranking.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_regression.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/metrics/tests/test_score_objects.py` & `scikit-learn-1.4.2/sklearn/metrics/tests/test_score_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/mixture/_base.py` & `scikit-learn-1.4.2/sklearn/mixture/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/mixture/_bayesian_mixture.py` & `scikit-learn-1.4.2/sklearn/mixture/_bayesian_mixture.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/mixture/_gaussian_mixture.py` & `scikit-learn-1.4.2/sklearn/mixture/_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/mixture/tests/test_bayesian_mixture.py` & `scikit-learn-1.4.2/sklearn/mixture/tests/test_bayesian_mixture.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/mixture/tests/test_gaussian_mixture.py` & `scikit-learn-1.4.2/sklearn/mixture/tests/test_gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/mixture/tests/test_mixture.py` & `scikit-learn-1.4.2/sklearn/mixture/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/__init__.py` & `scikit-learn-1.4.2/sklearn/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/_plot.py` & `scikit-learn-1.4.2/sklearn/model_selection/_plot.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/_search.py` & `scikit-learn-1.4.2/sklearn/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/_search_successive_halving.py` & `scikit-learn-1.4.2/sklearn/model_selection/_search_successive_halving.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/_split.py` & `scikit-learn-1.4.2/sklearn/model_selection/_split.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/_validation.py` & `scikit-learn-1.4.2/sklearn/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/tests/common.py` & `scikit-learn-1.4.2/sklearn/model_selection/tests/common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_plot.py` & `scikit-learn-1.4.2/sklearn/model_selection/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_search.py` & `scikit-learn-1.4.2/sklearn/model_selection/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_split.py` & `scikit-learn-1.4.2/sklearn/model_selection/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_successive_halving.py` & `scikit-learn-1.4.2/sklearn/model_selection/tests/test_successive_halving.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/model_selection/tests/test_validation.py` & `scikit-learn-1.4.2/sklearn/model_selection/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/multiclass.py` & `scikit-learn-1.4.2/sklearn/multiclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/multioutput.py` & `scikit-learn-1.4.2/sklearn/multioutput.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/naive_bayes.py` & `scikit-learn-1.4.2/sklearn/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/__init__.py` & `scikit-learn-1.4.2/sklearn/neighbors/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_ball_tree.pyx.tp` & `scikit-learn-1.4.2/sklearn/neighbors/_ball_tree.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_base.py` & `scikit-learn-1.4.2/sklearn/neighbors/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_binary_tree.pxi.tp` & `scikit-learn-1.4.2/sklearn/neighbors/_binary_tree.pxi.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_classification.py` & `scikit-learn-1.4.2/sklearn/neighbors/_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_graph.py` & `scikit-learn-1.4.2/sklearn/neighbors/_graph.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_kd_tree.pyx.tp` & `scikit-learn-1.4.2/sklearn/neighbors/_kd_tree.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_kde.py` & `scikit-learn-1.4.2/sklearn/neighbors/_kde.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_lof.py` & `scikit-learn-1.4.2/sklearn/neighbors/_lof.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_nca.py` & `scikit-learn-1.4.2/sklearn/neighbors/_nca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_nearest_centroid.py` & `scikit-learn-1.4.2/sklearn/neighbors/_nearest_centroid.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_partition_nodes.pyx` & `scikit-learn-1.4.2/sklearn/neighbors/_partition_nodes.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_quad_tree.pxd` & `scikit-learn-1.4.2/sklearn/neighbors/_quad_tree.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_quad_tree.pyx` & `scikit-learn-1.4.2/sklearn/neighbors/_quad_tree.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_regression.py` & `scikit-learn-1.4.2/sklearn/neighbors/_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/_unsupervised.py` & `scikit-learn-1.4.2/sklearn/neighbors/_unsupervised.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/meson.build` & `scikit-learn-1.4.2/sklearn/neighbors/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_ball_tree.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_ball_tree.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_graph.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_kd_tree.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_kd_tree.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_kde.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_kde.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_lof.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_lof.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_nca.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_nca.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_nearest_centroid.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_nearest_centroid.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_neighbors.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_neighbors_pipeline.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_neighbors_pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_neighbors_tree.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_neighbors_tree.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neighbors/tests/test_quad_tree.py` & `scikit-learn-1.4.2/sklearn/neighbors/tests/test_quad_tree.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/_base.py` & `scikit-learn-1.4.2/sklearn/neural_network/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/_multilayer_perceptron.py` & `scikit-learn-1.4.2/sklearn/neural_network/_multilayer_perceptron.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/_rbm.py` & `scikit-learn-1.4.2/sklearn/neural_network/_rbm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/_stochastic_optimizers.py` & `scikit-learn-1.4.2/sklearn/neural_network/_stochastic_optimizers.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/neural_network/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_mlp.py` & `scikit-learn-1.4.2/sklearn/neural_network/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_rbm.py` & `scikit-learn-1.4.2/sklearn/neural_network/tests/test_rbm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/neural_network/tests/test_stochastic_optimizers.py` & `scikit-learn-1.4.2/sklearn/neural_network/tests/test_stochastic_optimizers.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/pipeline.py` & `scikit-learn-1.4.2/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/__init__.py` & `scikit-learn-1.4.2/sklearn/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_csr_polynomial_expansion.pyx` & `scikit-learn-1.4.2/sklearn/preprocessing/_csr_polynomial_expansion.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_data.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_discretization.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_discretization.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_encoders.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_encoders.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_function_transformer.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_function_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_label.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_label.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,15 +823,15 @@
 
         # (make safe for tuples)
         dtype = int if all(isinstance(c, int) for c in tmp) else object
         class_mapping = np.empty(len(tmp), dtype=dtype)
         class_mapping[:] = tmp
         self.classes_, inverse = np.unique(class_mapping, return_inverse=True)
         # ensure yt.indices keeps its current dtype
-        yt.indices = np.array(inverse[yt.indices], dtype=yt.indices.dtype, copy=False)
+        yt.indices = np.asarray(inverse[yt.indices], dtype=yt.indices.dtype)
 
         if not self.sparse_output:
             yt = yt.toarray()
 
         return yt
 
     def transform(self, y):
```

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_polynomial.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_polynomial.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_target_encoder.py` & `scikit-learn-1.4.2/sklearn/preprocessing/_target_encoder.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/_target_encoder_fast.pyx` & `scikit-learn-1.4.2/sklearn/preprocessing/_target_encoder_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_data.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,21 @@
     n_samples = 10
     n_features = 3
     if add_sample_weight:
         sample_weight = np.ones(n_samples)
     else:
         sample_weight = None
     with_mean = True
-    for dtype in [np.float16, np.float32, np.float64]:
+    if sparse_container is not None:
+        # scipy sparse containers do not support float16, see
+        # https://github.com/scipy/scipy/issues/7408 for more details.
+        supported_dtype = [np.float64, np.float32]
+    else:
+        supported_dtype = [np.float64, np.float32, np.float16]
+    for dtype in supported_dtype:
         X = rng.randn(n_samples, n_features).astype(dtype)
         if sparse_container is not None:
             X = sparse_container(X)
             with_mean = False
 
         scaler = StandardScaler(with_mean=with_mean)
         X_scaled = scaler.fit(X, sample_weight=sample_weight).transform(X)
```

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_discretization.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_encoders.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_function_transformer.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_label.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_polynomial.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/preprocessing/tests/test_target_encoder.py` & `scikit-learn-1.4.2/sklearn/preprocessing/tests/test_target_encoder.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/random_projection.py` & `scikit-learn-1.4.2/sklearn/random_projection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/semi_supervised/_label_propagation.py` & `scikit-learn-1.4.2/sklearn/semi_supervised/_label_propagation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/semi_supervised/_self_training.py` & `scikit-learn-1.4.2/sklearn/semi_supervised/_self_training.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/semi_supervised/tests/test_label_propagation.py` & `scikit-learn-1.4.2/sklearn/semi_supervised/tests/test_label_propagation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/semi_supervised/tests/test_self_training.py` & `scikit-learn-1.4.2/sklearn/semi_supervised/tests/test_self_training.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/__init__.py` & `scikit-learn-1.4.2/sklearn/svm/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_base.py` & `scikit-learn-1.4.2/sklearn/svm/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_bounds.py` & `scikit-learn-1.4.2/sklearn/svm/_bounds.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_classes.py` & `scikit-learn-1.4.2/sklearn/svm/_classes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_liblinear.pxi` & `scikit-learn-1.4.2/sklearn/svm/_liblinear.pxi`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_liblinear.pyx` & `scikit-learn-1.4.2/sklearn/svm/_liblinear.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_libsvm.pxi` & `scikit-learn-1.4.2/sklearn/svm/_libsvm.pxi`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_libsvm.pyx` & `scikit-learn-1.4.2/sklearn/svm/_libsvm.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/_libsvm_sparse.pyx` & `scikit-learn-1.4.2/sklearn/svm/_libsvm_sparse.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/meson.build` & `scikit-learn-1.4.2/sklearn/svm/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/COPYRIGHT` & `scikit-learn-1.4.2/sklearn/svm/src/liblinear/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/liblinear_helper.c` & `scikit-learn-1.4.2/sklearn/svm/src/liblinear/liblinear_helper.c`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/linear.cpp` & `scikit-learn-1.4.2/sklearn/svm/src/liblinear/linear.cpp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/linear.h` & `scikit-learn-1.4.2/sklearn/svm/src/liblinear/linear.h`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/tron.cpp` & `scikit-learn-1.4.2/sklearn/svm/src/liblinear/tron.cpp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/liblinear/tron.h` & `scikit-learn-1.4.2/sklearn/svm/src/liblinear/tron.h`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/LIBSVM_CHANGES` & `scikit-learn-1.4.2/sklearn/svm/src/libsvm/LIBSVM_CHANGES`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/libsvm_helper.c` & `scikit-learn-1.4.2/sklearn/svm/src/libsvm/libsvm_helper.c`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/libsvm_sparse_helper.c` & `scikit-learn-1.4.2/sklearn/svm/src/libsvm/libsvm_sparse_helper.c`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/svm.cpp` & `scikit-learn-1.4.2/sklearn/svm/src/libsvm/svm.cpp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/libsvm/svm.h` & `scikit-learn-1.4.2/sklearn/svm/src/libsvm/svm.h`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/src/newrand/newrand.h` & `scikit-learn-1.4.2/sklearn/svm/src/newrand/newrand.h`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/tests/test_bounds.py` & `scikit-learn-1.4.2/sklearn/svm/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/tests/test_sparse.py` & `scikit-learn-1.4.2/sklearn/svm/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/svm/tests/test_svm.py` & `scikit-learn-1.4.2/sklearn/svm/tests/test_svm.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/metadata_routing_common.py` & `scikit-learn-1.4.2/sklearn/tests/metadata_routing_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/random_seed.py` & `scikit-learn-1.4.2/sklearn/tests/random_seed.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_base.py` & `scikit-learn-1.4.2/sklearn/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_build.py` & `scikit-learn-1.4.2/sklearn/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_calibration.py` & `scikit-learn-1.4.2/sklearn/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_common.py` & `scikit-learn-1.4.2/sklearn/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_config.py` & `scikit-learn-1.4.2/sklearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_discriminant_analysis.py` & `scikit-learn-1.4.2/sklearn/tests/test_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_docstring_parameters.py` & `scikit-learn-1.4.2/sklearn/tests/test_docstring_parameters.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_docstrings.py` & `scikit-learn-1.4.2/sklearn/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_dummy.py` & `scikit-learn-1.4.2/sklearn/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_isotonic.py` & `scikit-learn-1.4.2/sklearn/tests/test_isotonic.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_kernel_approximation.py` & `scikit-learn-1.4.2/sklearn/tests/test_kernel_approximation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_kernel_ridge.py` & `scikit-learn-1.4.2/sklearn/tests/test_kernel_ridge.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_metadata_routing.py` & `scikit-learn-1.4.2/sklearn/tests/test_metadata_routing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_metaestimators.py` & `scikit-learn-1.4.2/sklearn/tests/test_metaestimators.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_metaestimators_metadata_routing.py` & `scikit-learn-1.4.2/sklearn/tests/test_metaestimators_metadata_routing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_min_dependencies_readme.py` & `scikit-learn-1.4.2/sklearn/tests/test_min_dependencies_readme.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_multiclass.py` & `scikit-learn-1.4.2/sklearn/tests/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_multioutput.py` & `scikit-learn-1.4.2/sklearn/tests/test_multioutput.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_naive_bayes.py` & `scikit-learn-1.4.2/sklearn/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_pipeline.py` & `scikit-learn-1.4.2/sklearn/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_public_functions.py` & `scikit-learn-1.4.2/sklearn/tests/test_public_functions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tests/test_random_projection.py` & `scikit-learn-1.4.2/sklearn/tests/test_random_projection.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/__init__.py` & `scikit-learn-1.4.2/sklearn/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_classes.py` & `scikit-learn-1.4.2/sklearn/tree/_classes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_criterion.pxd` & `scikit-learn-1.4.2/sklearn/tree/_criterion.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_criterion.pyx` & `scikit-learn-1.4.2/sklearn/tree/_criterion.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_export.py` & `scikit-learn-1.4.2/sklearn/tree/_export.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_reingold_tilford.py` & `scikit-learn-1.4.2/sklearn/tree/_reingold_tilford.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_splitter.pxd` & `scikit-learn-1.4.2/sklearn/tree/_splitter.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_splitter.pyx` & `scikit-learn-1.4.2/sklearn/tree/_splitter.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_tree.pxd` & `scikit-learn-1.4.2/sklearn/tree/_tree.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_tree.pyx` & `scikit-learn-1.4.2/sklearn/tree/_tree.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_utils.pxd` & `scikit-learn-1.4.2/sklearn/tree/_utils.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/_utils.pyx` & `scikit-learn-1.4.2/sklearn/tree/_utils.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/meson.build` & `scikit-learn-1.4.2/sklearn/tree/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/tests/test_export.py` & `scikit-learn-1.4.2/sklearn/tree/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/tests/test_monotonic_tree.py` & `scikit-learn-1.4.2/sklearn/tree/tests/test_monotonic_tree.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/tests/test_reingold_tilford.py` & `scikit-learn-1.4.2/sklearn/tree/tests/test_reingold_tilford.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/tree/tests/test_tree.py` & `scikit-learn-1.4.2/sklearn/tree/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/__init__.py` & `scikit-learn-1.4.2/sklearn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_arpack.py` & `scikit-learn-1.4.2/sklearn/utils/_arpack.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_array_api.py` & `scikit-learn-1.4.2/sklearn/utils/_array_api.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_available_if.py` & `scikit-learn-1.4.2/sklearn/utils/_available_if.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_bunch.py` & `scikit-learn-1.4.2/sklearn/utils/_bunch.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_cython_blas.pxd` & `scikit-learn-1.4.2/sklearn/utils/_cython_blas.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_cython_blas.pyx` & `scikit-learn-1.4.2/sklearn/utils/_cython_blas.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_encode.py` & `scikit-learn-1.4.2/sklearn/utils/_encode.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_estimator_html_repr.css` & `scikit-learn-1.4.2/sklearn/utils/_estimator_html_repr.css`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_estimator_html_repr.py` & `scikit-learn-1.4.2/sklearn/utils/_estimator_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_fast_dict.pyx` & `scikit-learn-1.4.2/sklearn/utils/_fast_dict.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_heap.pyx` & `scikit-learn-1.4.2/sklearn/utils/_heap.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_isfinite.pyx` & `scikit-learn-1.4.2/sklearn/utils/_isfinite.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_joblib.py` & `scikit-learn-1.4.2/sklearn/utils/_joblib.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_mask.py` & `scikit-learn-1.4.2/sklearn/utils/_mask.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_metadata_requests.py` & `scikit-learn-1.4.2/sklearn/utils/_metadata_requests.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_mocking.py` & `scikit-learn-1.4.2/sklearn/utils/_mocking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_openmp_helpers.pxd` & `scikit-learn-1.4.2/sklearn/utils/_openmp_helpers.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_openmp_helpers.pyx` & `scikit-learn-1.4.2/sklearn/utils/_openmp_helpers.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_param_validation.py` & `scikit-learn-1.4.2/sklearn/utils/_param_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_plotting.py` & `scikit-learn-1.4.2/sklearn/utils/_plotting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_pprint.py` & `scikit-learn-1.4.2/sklearn/utils/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_random.pxd` & `scikit-learn-1.4.2/sklearn/utils/_random.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_random.pyx` & `scikit-learn-1.4.2/sklearn/utils/_random.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_response.py` & `scikit-learn-1.4.2/sklearn/utils/_response.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_seq_dataset.pxd.tp` & `scikit-learn-1.4.2/sklearn/utils/_seq_dataset.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_seq_dataset.pyx.tp` & `scikit-learn-1.4.2/sklearn/utils/_seq_dataset.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_set_output.py` & `scikit-learn-1.4.2/sklearn/utils/_set_output.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_show_versions.py` & `scikit-learn-1.4.2/sklearn/utils/_show_versions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_sorting.pyx` & `scikit-learn-1.4.2/sklearn/utils/_sorting.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_tags.py` & `scikit-learn-1.4.2/sklearn/utils/_tags.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_testing.py` & `scikit-learn-1.4.2/sklearn/utils/_testing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_typedefs.pxd` & `scikit-learn-1.4.2/sklearn/utils/_typedefs.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_vector_sentinel.pyx` & `scikit-learn-1.4.2/sklearn/utils/_vector_sentinel.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_weight_vector.pxd.tp` & `scikit-learn-1.4.2/sklearn/utils/_weight_vector.pxd.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/_weight_vector.pyx.tp` & `scikit-learn-1.4.2/sklearn/utils/_weight_vector.pyx.tp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/arrayfuncs.pyx` & `scikit-learn-1.4.2/sklearn/utils/arrayfuncs.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/class_weight.py` & `scikit-learn-1.4.2/sklearn/utils/class_weight.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/deprecation.py` & `scikit-learn-1.4.2/sklearn/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/discovery.py` & `scikit-learn-1.4.2/sklearn/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/estimator_checks.py` & `scikit-learn-1.4.2/sklearn/utils/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/extmath.py` & `scikit-learn-1.4.2/sklearn/utils/extmath.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/fixes.py` & `scikit-learn-1.4.2/sklearn/utils/fixes.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,22 +252,25 @@
 # TODO: Remove when Scipy 1.6 is the minimum supported version
 try:
     from scipy.integrate import trapezoid  # type: ignore  # noqa
 except ImportError:
     from scipy.integrate import trapz as trapezoid  # type: ignore  # noqa
 
 
-# TODO: Remove when Pandas > 2.2 is the minimum supported version
+# TODO: Adapt when Pandas > 2.2 is the minimum supported version
 def pd_fillna(pd, frame):
     pd_version = parse_version(pd.__version__).base_version
     if parse_version(pd_version) < parse_version("2.2"):
         frame = frame.fillna(value=np.nan)
     else:
+        infer_objects_kwargs = (
+            {} if parse_version(pd_version) >= parse_version("3") else {"copy": False}
+        )
         with pd.option_context("future.no_silent_downcasting", True):
-            frame = frame.fillna(value=np.nan).infer_objects(copy=False)
+            frame = frame.fillna(value=np.nan).infer_objects(**infer_objects_kwargs)
     return frame
 
 
 # TODO: remove when SciPy 1.12 is the minimum supported version
 def _preserve_dia_indices_dtype(
     sparse_container, original_container_format, requested_sparse_format
 ):
```

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/graph.py` & `scikit-learn-1.4.2/sklearn/utils/graph.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/meson.build` & `scikit-learn-1.4.2/sklearn/utils/meson.build`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/metadata_routing.py` & `scikit-learn-1.4.2/sklearn/utils/metadata_routing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/metaestimators.py` & `scikit-learn-1.4.2/sklearn/utils/metaestimators.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/multiclass.py` & `scikit-learn-1.4.2/sklearn/utils/multiclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/murmurhash.pxd` & `scikit-learn-1.4.2/sklearn/utils/murmurhash.pxd`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/murmurhash.pyx` & `scikit-learn-1.4.2/sklearn/utils/murmurhash.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/optimize.py` & `scikit-learn-1.4.2/sklearn/utils/optimize.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/parallel.py` & `scikit-learn-1.4.2/sklearn/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/random.py` & `scikit-learn-1.4.2/sklearn/utils/random.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/sparsefuncs.py` & `scikit-learn-1.4.2/sklearn/utils/sparsefuncs.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/sparsefuncs_fast.pyx` & `scikit-learn-1.4.2/sklearn/utils/sparsefuncs_fast.pyx`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/src/MurmurHash3.cpp` & `scikit-learn-1.4.2/sklearn/utils/src/MurmurHash3.cpp`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/src/MurmurHash3.h` & `scikit-learn-1.4.2/sklearn/utils/src/MurmurHash3.h`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/stats.py` & `scikit-learn-1.4.2/sklearn/utils/stats.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_array_api.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_array_api.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_arrayfuncs.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_bunch.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_bunch.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_class_weight.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_class_weight.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_cython_blas.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_cython_blas.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_cython_templating.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_cython_templating.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_deprecation.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_encode.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_estimator_checks.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_estimator_checks.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_estimator_html_repr.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_estimator_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_extmath.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_extmath.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_fast_dict.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_fast_dict.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_fixes.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_fixes.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_graph.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_metaestimators.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_metaestimators.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_mocking.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_mocking.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_multiclass.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_murmurhash.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_murmurhash.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_optimize.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_parallel.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_param_validation.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_param_validation.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_plotting.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_pprint.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_random.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_response.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_seq_dataset.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_seq_dataset.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_set_output.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_set_output.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_shortest_path.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_shortest_path.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_show_versions.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_sparsefuncs.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_sparsefuncs.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_stats.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_tags.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_testing.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_typedefs.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_typedefs.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_utils.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_validation.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1628,15 +1628,14 @@
         check_array(df, accept_sparse=["csr", "csc"])
 
 
 @pytest.mark.parametrize(
     "ntype1, ntype2, expected_subtype",
     [
         ("double", "longdouble", np.floating),
-        ("float16", "half", np.floating),
         ("single", "float32", np.floating),
         ("double", "float64", np.floating),
         ("int8", "byte", np.integer),
         ("short", "int16", np.integer),
         ("intc", "int32", np.integer),
         ("intp", "long", np.integer),
         ("int", "long", np.integer),
```

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/tests/test_weight_vector.py` & `scikit-learn-1.4.2/sklearn/utils/tests/test_weight_vector.py`

 * *Files identical despite different names*

### Comparing `scikit-learn-1.4.1.post1/sklearn/utils/validation.py` & `scikit-learn-1.4.2/sklearn/utils/validation.py`

 * *Files identical despite different names*

